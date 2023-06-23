# Comparing `tmp/linopy-0.1.5.tar.gz` & `tmp/linopy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linopy-0.1.5.tar", last modified: Fri May  5 08:45:58 2023, max compression
+gzip compressed data, was "linopy-0.2.tar", last modified: Fri Jun 23 13:03:08 2023, max compression
```

## Comparing `linopy-0.1.5.tar` & `linopy-0.2.tar`

### file list

```diff
@@ -1,145 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.168245 linopy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 08:45:45.000000 linopy-0.1.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.148246 linopy-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 08:45:45.000000 linopy-0.1.5/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 08:45:45.000000 linopy-0.1.5/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-05 08:45:45.000000 linopy-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 08:45:45.000000 linopy-0.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-05 08:45:45.000000 linopy-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-05 08:45:45.000000 linopy-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-05 08:45:58.168245 linopy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-05 08:45:45.000000 linopy-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/benchmark_resource-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/environment.fixed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.152246 linopy-0.1.5/benchmark/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/notebooks/plot-benchmarks.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_jump.jl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmark_pyomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/concat-benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.156246 linopy-0.1.5/benchmark/scripts/leftovers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmark-linopy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/leftovers/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/merge-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/run-pyomo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-05 08:45:45.000000 linopy-0.1.5/benchmark/scripts/write-lp-file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/benchmark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/create-a-model.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/creating-constraints.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/creating-variables.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132092 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/manipulating-models.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/migrating-from-pyomo.nblink
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/solve-on-remote.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-05 08:45:45.000000 linopy-0.1.5/doc/syntax.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.160246 linopy-0.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/create-a-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/creating-constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/creating-variables.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/manipulating-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/migrating-from-pyomo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-05-05 08:45:45.000000 linopy-0.1.5/examples/solve-on-remote.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/linopy/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    30415 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    38511 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/monkey_patch_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-05-05 08:45:45.000000 linopy-0.1.5/linopy/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/linopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:45:58.000000 linopy-0.1.5/linopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 08:45:45.000000 linopy-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:45:58.168245 linopy-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-05 08:45:45.000000 linopy-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:45:58.164245 linopy-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_inconsistency_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_scalar_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_scalar_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variable_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-05 08:45:45.000000 linopy-0.1.5/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-23 13:02:58.000000 linopy-0.2/.coverage
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 13:02:58.000000 linopy-0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.084946 linopy-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.084946 linopy-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 13:02:58.000000 linopy-0.2/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 13:02:58.000000 linopy-0.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-23 13:02:58.000000 linopy-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 13:02:58.000000 linopy-0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-23 13:02:58.000000 linopy-0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 13:02:58.000000 linopy-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-23 13:03:08.100946 linopy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-23 13:02:58.000000 linopy-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/environment.fixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/notebooks/plot-benchmarks.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_jump.jl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_pyomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/concat-benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmark-linopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/merge-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-pyomo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/write-lp-file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 13:02:58.000000 linopy-0.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-23 13:02:58.000000 linopy-0.2/doc/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-23 13:02:58.000000 linopy-0.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-06-23 13:02:58.000000 linopy-0.2/doc/benchmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 13:02:58.000000 linopy-0.2/doc/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-23 13:02:58.000000 linopy-0.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-23 13:02:58.000000 linopy-0.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 13:02:58.000000 linopy-0.2/doc/create-a-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 13:02:58.000000 linopy-0.2/doc/creating-constraints.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 13:02:58.000000 linopy-0.2/doc/creating-variables.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-23 13:02:58.000000 linopy-0.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132092 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 13:02:58.000000 linopy-0.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 13:02:58.000000 linopy-0.2/doc/manipulating-models.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 13:02:58.000000 linopy-0.2/doc/migrating-from-pyomo.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-06-23 13:02:59.000000 linopy-0.2/doc/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 13:02:59.000000 linopy-0.2/doc/solve-on-remote.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-23 13:02:59.000000 linopy-0.2/doc/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-23 13:02:59.000000 linopy-0.2/doc/syntax.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-06-23 13:02:59.000000 linopy-0.2/examples/create-a-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-06-23 13:02:59.000000 linopy-0.2/examples/creating-constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-06-23 13:02:59.000000 linopy-0.2/examples/creating-variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 13:02:59.000000 linopy-0.2/examples/manipulating-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 13:02:59.000000 linopy-0.2/examples/migrating-from-pyomo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-06-23 13:02:59.000000 linopy-0.2/examples/solve-on-remote.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/linopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 13:02:59.000000 linopy-0.2/linopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-06-23 13:02:59.000000 linopy-0.2/linopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-23 13:02:59.000000 linopy-0.2/linopy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-23 13:02:59.000000 linopy-0.2/linopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29212 2023-06-23 13:02:59.000000 linopy-0.2/linopy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46449 2023-06-23 13:02:59.000000 linopy-0.2/linopy/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-23 13:02:59.000000 linopy-0.2/linopy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-23 13:02:59.000000 linopy-0.2/linopy/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-06-23 13:02:59.000000 linopy-0.2/linopy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 13:02:59.000000 linopy-0.2/linopy/monkey_patch_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-23 13:02:59.000000 linopy-0.2/linopy/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-06-23 13:02:59.000000 linopy-0.2/linopy/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-23 13:02:59.000000 linopy-0.2/linopy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-06-23 13:02:59.000000 linopy-0.2/linopy/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 13:03:08.000000 linopy-0.2/linopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/linopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 13:02:59.000000 linopy-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:03:08.100946 linopy-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-23 13:02:59.000000 linopy-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-23 13:02:59.000000 linopy-0.2/test/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-23 13:02:59.000000 linopy-0.2/test/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-23 13:02:59.000000 linopy-0.2/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 13:02:59.000000 linopy-0.2/test/test_inconsistency_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-23 13:02:59.000000 linopy-0.2/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-06-23 13:02:59.000000 linopy-0.2/test/test_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-23 13:02:59.000000 linopy-0.2/test/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-23 13:02:59.000000 linopy-0.2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-23 13:02:59.000000 linopy-0.2/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 13:02:59.000000 linopy-0.2/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-23 13:02:59.000000 linopy-0.2/test/test_quadratic_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-23 13:02:59.000000 linopy-0.2/test/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-23 13:02:59.000000 linopy-0.2/test/test_scalar_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-23 13:02:59.000000 linopy-0.2/test/test_scalar_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variable_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variables.py
```

### Comparing `linopy-0.1.5/.github/workflows/CI.yaml` & `linopy-0.2/.github/workflows/CI.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 name: CI
 
-on: [push]
+on:
+  push:
+    branches: [ master ]
+  pull_request:
+    branches: [ '*' ]
+  schedule:
+  - cron: "0 5 * * TUE"
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
```

### Comparing `linopy-0.1.5/.github/workflows/deploy.yml` & `linopy-0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/.pre-commit-config.yaml` & `linopy-0.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     -   id: absolufy-imports
 -   repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black", "--filter-files"]
 -   repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
     -   id: codespell
         types_or: [python, rst, markdown]
         files: ^(linopy|doc)/
 -   repo: https://github.com/aflc/pre-commit-jupyter
     rev: v1.2.1
     hooks:
```

### Comparing `linopy-0.1.5/PKG-INFO` & `linopy-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.1.5
+Version: 0.2
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
-License: GPLv3
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: solvers
 License-File: LICENSE.txt
 
-# linopy: Linear optimization with N-D labeled variables
+# linopy: Linear optimization with N-dimensional labeled variables
 
-[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
+[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License](https://img.shields.io/pypi/l/linopy.svg)](LICENSE.txt) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
 
-**linopy** is an open-source python package that facilitates **linear or mixed-integer optimisation** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and linear problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). The project aims to make linear programming in python easy, highly-flexible and performant.
+**linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) contnuous or binary variables with **coordinates**, e.g. time, consumers, etc.
@@ -45,14 +45,21 @@
 
 So far **linopy** is available on the PyPI repository
 
 ```bash
 pip install linopy
 ```
 
+or on conda-forge
+
+```bash
+conda install -c conda-forge linopy
+```
+
+
 ## Supported solvers
 
 **linopy** supports the following solvers
 
 * [Cbc](https://projects.coin-or.org/Cbc)
 * [GLPK](https://www.gnu.org/software/glpk/)
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
@@ -65,8 +72,8 @@
 
 # License
 
 Copyright 2021 Fabian Hofmann
 
 
 
-This package is published under license GNU Public License GPLv3
+This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.1.5/README.md` & `linopy-0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# linopy: Linear optimization with N-D labeled variables
+# linopy: Linear optimization with N-dimensional labeled variables
 
-[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
+[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License](https://img.shields.io/pypi/l/linopy.svg)](LICENSE.txt) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
 
-**linopy** is an open-source python package that facilitates **linear or mixed-integer optimisation** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and linear problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). The project aims to make linear programming in python easy, highly-flexible and performant.
+**linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) contnuous or binary variables with **coordinates**, e.g. time, consumers, etc.
@@ -24,14 +24,21 @@
 
 So far **linopy** is available on the PyPI repository
 
 ```bash
 pip install linopy
 ```
 
+or on conda-forge
+
+```bash
+conda install -c conda-forge linopy
+```
+
+
 ## Supported solvers
 
 **linopy** supports the following solvers
 
 * [Cbc](https://projects.coin-or.org/Cbc)
 * [GLPK](https://www.gnu.org/software/glpk/)
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
@@ -44,8 +51,8 @@
 
 # License
 
 Copyright 2021 Fabian Hofmann
 
 
 
-This package is published under license GNU Public License GPLv3
+This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.1.5/benchmark/README.md` & `linopy-0.2/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/Snakefile` & `linopy-0.2/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark-absolute.pdf` & `linopy-0.2/benchmark/benchmark-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark-absolute.png` & `linopy-0.2/benchmark/benchmark-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark-overhead.pdf` & `linopy-0.2/benchmark/benchmark-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark-overhead.png` & `linopy-0.2/benchmark/benchmark-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark_resource-absolute.pdf` & `linopy-0.2/benchmark/benchmark_resource-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark_resource-absolute.png` & `linopy-0.2/benchmark/benchmark_resource-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark_resource-overhead.pdf` & `linopy-0.2/benchmark/benchmark_resource-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/benchmark_resource-overhead.png` & `linopy-0.2/benchmark/benchmark_resource-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/environment.fixed.yaml` & `linopy-0.2/benchmark/environment.fixed.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/notebooks/plot-benchmarks.py.ipynb` & `linopy-0.2/benchmark/notebooks/plot-benchmarks.py.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_cvxpy.py` & `linopy-0.2/benchmark/scripts/benchmark_cvxpy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_gurobipy.py` & `linopy-0.2/benchmark/scripts/benchmark_gurobipy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_jump.jl` & `linopy-0.2/benchmark/scripts/benchmark_jump.jl`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_linopy.py` & `linopy-0.2/benchmark/scripts/benchmark_linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_ortools.py` & `linopy-0.2/benchmark/scripts/benchmark_ortools.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_pulp.py` & `linopy-0.2/benchmark/scripts/benchmark_pulp.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmark_pyomo.py` & `linopy-0.2/benchmark/scripts/benchmark_pyomo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/concat-benchmarks.py` & `linopy-0.2/benchmark/scripts/concat-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmark-linopy.py` & `linopy-0.2/benchmark/scripts/leftovers/benchmark-linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/leftovers/common.py` & `linopy-0.2/benchmark/scripts/leftovers/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/merge-benchmarks.py` & `linopy-0.2/benchmark/scripts/merge-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/plot-benchmarks.py` & `linopy-0.2/benchmark/scripts/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/benchmark/scripts/write-lp-file.py` & `linopy-0.2/benchmark/scripts/write-lp-file.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/Makefile` & `linopy-0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/_static/theme_overrides.css` & `linopy-0.2/doc/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/api.rst` & `linopy-0.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/benchmark.png` & `linopy-0.2/doc/benchmark.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/benchmark.rst` & `linopy-0.2/doc/benchmark.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/conf.py` & `linopy-0.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/contributing.rst` & `linopy-0.2/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/index.rst` & `linopy-0.2/doc/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -65,24 +65,24 @@
 -  `Cplex <https://www.ibm.com/de-de/analytics/cplex-optimizer>`__
 
 Note that these do have to be installed by the user separately.
 
 License
 =======
 
-Copyright 2021 Fabian Hofmann
+Copyright 2021-2023 Fabian Hofmann
 
-This package is published under license GNU Public License GPLv3
+This package is published under MIT license.
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/linopy
    :target: https://pypi.org/project/linopy/
 .. |CI| image:: https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg
    :target: https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml
-.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-   :target: https://www.gnu.org/licenses/gpl-3.0
+.. |License| image:: https://img.shields.io/pypi/l/linopy.svg
+   :target: https://mit-license.org/
 
 
 .. toctree::
    :hidden:
    :maxdepth: 2
    :caption: Getting started
```

### Comparing `linopy-0.1.5/doc/logo.pdf` & `linopy-0.2/doc/logo.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/logo.png` & `linopy-0.2/doc/logo.png`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/logo.py` & `linopy-0.2/doc/logo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/make.bat` & `linopy-0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/release_notes.rst` & `linopy-0.2/doc/release_notes.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,64 @@
 Release Notes
 =============
 
 .. Upcoming Release
 .. ----------------
 
+
+Version 0.2.0
+-------------
+
+
+**New Features**
+
+* Linopy now supports quadratic programming. Therefore a new class `QuadraticExpression` was created, which can be assigned to the objective function. The `QuadraticExpression` class supports the same arithmetic operations as the `LinearExpression` and can be created by multiplying two `Variable` or `LinearExpression` objects. Note for the latter, the number of stacked terms must be equal to one (`expr.nterm == 1`).
+* `LinearExpression`'s now support constant values. This allows defining linear expressions with numeric constant values, like `x + 5`.
+* When defining constraints, it is not needed to separate variables from constants anymore. Thus, expressions  like `x <= y` or `5 * x + 10 >= y` are supported.
+* The new default solver will now be the first element in `available_solvers`.
+* The classes `Variable`, `LinearExpression` and `Constraint` now have a `loc` method.
+* The classes `Variable`, `LinearExpression`, `Constraint`, `Variables` and `Constraints` now have a `flat` method, which returns a flattened `pandas.DataFrame` of the object in long-table format.
+* It is now possible to access variables and constraints by a dot notation. For example, `model.variables.x` returns the variable `x` of the model.
+* Variable assignment without explicit coordinates is now supported. In an internal step, integer coordinates are assigned to the dimensions without explicit coordinates.
+* The `groupby` function now supports passing `pandas.Dataframe`s as groupby keys. These allows to group by multiple variables at once.
+* The performance of the `groupby` function was strongly increased. In large operations a speedup of 10x was observed.
+* New test functions `assert_varequal`, `assert_conequal` were added to the `testing` module.
+
+
+**Deprecations**
+
+* The class `AnonymousConstraint` is now deprecated in the favor of `Constraint`. The latter can now be assigned to a model or not.
+* The `ravel` and `iter_ravel` method of the `Variables` and `Constraints` class is now deprecated in favor of the `flat` method.
+
+
+**Breaking Changes**
+
+* The `data` attribute of Variables and Constraints now returns a `xarray.Dataset` object instead of a `xarray.DataArray` object with the labels only.
+* The deprecated `groupby_sum` function was removed in favor of the `groupby` method.
+* The deprecated `rolling_sum` function was removed in favor of the `rolling` method.
+* The deprecated `eval` module was removed in favor of the arithmetic operations on the classes `Variable`, `LinearExpression` and `Constraint`.
+* The deprecated attribute `values` of the classes `Variable`, `LinearExpression` and `Constraint` was removed in favor of the `data` attribute.
+* The deprecated `to_array` method of the classes `Variable` and `Constraint` was removed in favor of the `data` attribute.
+* The deprecated `to_dataset` of the `LinearExpression` class was removed in favor of the `data` attribute.
+* The function `get_lower_bound`, `get_upper_bound`, `get_variable_labels`, `get_variable_types`, `get_objective_coefficient`, `get_constraint_labels`, `get_constraint_sense`, `get_constraint_rhs`, `get_constraint_matrix` were removed in favor of the `matrices` accessor, i.e. `ub`, `lb`, `vlabels`, etc.
+* The `LinearExpressionGroupby` class now takes a different set of arguments when initializing. These are `data: xr.Dataset`, `group: xr.DataArray`, `model: Any`, `kwargs: Mapping[str, Any]`.
+* When grouping with a `xr.DataArray` / `pd.Series` / `pd.DataFrame` and summing afterwards, the keyword arguments like `squeeze`, `restore_coords` are ignored.
+
+
+**Internal Changes**
+
+* The internal data fields in `Variable` and `Constraint` are now always broadcasted to have aligned indexes. This allows for a more consistent handling of the objects.
+* The inner structure of the `Variable`, `Variables`, `Constraint` and `Constraints` class has changed to a more stable design. All information of the `Variable` and the `Constraint` class is now stored in the `data` field. The `data` field is a `xarray.Dataset` object. The `Variables` and `Constraints` class "simple" containers for the `Variable` and `Constraint` objects, stored in dictionary under the `data` field. This design allows for a more flexible handling of individual variables and constraints.
+
+**Other**
+
+* License changed to MIT license.
+
+
+
 Version 0.1.5
 -------------
 
 
 * Add `sel` functions to `Constraint` and `AnonymousConstraint` to allow for selection and inspection of constraints by coordinate.
 * The printout of `Variables` and `Constraints` was refactored to a more concise layout.
 * The solving termination condition "other" is now tagged as solving status "warning".
```

### Comparing `linopy-0.1.5/doc/solvers.rst` & `linopy-0.2/doc/solvers.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/doc/syntax.rst` & `linopy-0.2/doc/syntax.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/examples/create-a-model.ipynb` & `linopy-0.2/examples/create-a-model.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9855151840828924%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(4, 'Constraints consist of the left hand side (lhs) and the "*

 * *            "righ hand side (rhs). The first constraint that we want to write down is \\n'), (5, "*

 * *            "'$3x + 7y >= 10$, which we can write just exactly in this way')], delete: [5, 4]}}, "*

 * *            "11: {'id': '60f41b76', 'source': ['3*x + 7*y - 10 >= 0']}, 12: {'id': '02abd938', "*

 * *            "'source': ['... and linopy will automatically take over the separation of variables "*

 * *            "expr […]*

```diff
@@ -92,34 +92,54 @@
             "id": "sonic-rebate",
             "metadata": {},
             "source": [
                 "Since both `x` and `y` are scalar variables, so their arrays also contain just one variable reference. The variable `x` points to the optimisation variable 1 and the variable `y` points to the optimisation variable 2. Later we will see the benefit of this behaviour.  \n",
                 "\n",
                 "### Adding Constraints\n",
                 "\n",
-                "Constraints consist of the left hand side (lhs) and the righ hand side (rhs). The lhs must contain all the variables with the corresponding coefficients, while the rhs is just constant. The first lhs of our two remaining constraints is \n",
-                "$3x + 7y$, which we can write just exactly in this way"
+                "Constraints consist of the left hand side (lhs) and the righ hand side (rhs). The first constraint that we want to write down is \n",
+                "$3x + 7y >= 10$, which we can write just exactly in this way"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ongoing-desktop",
+            "id": "fbb46cad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "3*x + 7*y"
+                "3*x + 7*y >= 10"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ambient-collect",
+            "id": "f4666bee",
             "metadata": {},
             "source": [
-                "When assigning to the model, we call the function `m.add_constraints`."
+                "Note, we can also mix the constant and the variable expression, like this"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "60f41b76",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "3*x + 7*y - 10 >= 0"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "02abd938",
+            "metadata": {},
+            "source": [
+                "... and linopy will automatically take over the separation of variables expression on the lhs, and constant values on the rhs.\n",
+                "\n",
+                "The constraint is currently not assigned to the model. We assign it by calling the function `m.add_constraints`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "hollywood-production",
             "metadata": {},
@@ -160,25 +180,35 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "preceding-limit",
             "metadata": {},
             "source": [
-                "The solution of the linear problem is stored in `m.solution` in fom of a `xarray.Dataset`. "
+                "The solution of the linear problem assinged to the variables under `solution` in fom of a `xarray.Dataset`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "electric-duration",
             "metadata": {},
             "outputs": [],
             "source": [
-                "m.solution"
+                "x.solution"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e6d31751",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "y.solution"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f2c1a9d5",
             "metadata": {},
             "source": [
@@ -331,15 +361,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "organized-hampshire",
             "metadata": {},
             "outputs": [],
             "source": [
                 "lhs = (y - y.shift(time=1)).sel(time=time[1:])\n",
-                "m.add_constraints(lhs, '<=', 0.5, name='Limited growth y')"
+                "m.add_constraints(lhs <= 0.5, name='Limited growth y')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "sustained-portrait",
             "metadata": {},
@@ -366,13 +396,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `linopy-0.1.5/examples/creating-constraints.ipynb` & `linopy-0.2/examples/creating-constraints.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9596310908084165%*

 * *Differences: {"'cells'": "{6: {'source': ['When applying one of the operators `<=`, `>=`, `==` to the "*

 * *            "expression, an unassigned constraint is built:']}, 11: {'source': ['We can now add "*

 * *            'the constraint to the model by passing the unassigned `Constraint` to the '*

 * *            "`.add_constraint` function. ']}, 13: {'source': ['The same output would be generated "*

 * *            "if passing lhs, sign and rhs as separate arguments to the function:']}, delete: [42, "*

 * *            '32, 31, 30, 29, 28, 2 […]*

```diff
@@ -79,15 +79,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ffe7dc45",
             "metadata": {},
             "source": [
-                "When applying one of the operators `<=`, `>=`, `==` to the expression, an anomymous constraint is built:"
+                "When applying one of the operators `<=`, `>=`, `==` to the expression, an unassigned constraint is built:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0301876e",
             "metadata": {},
@@ -126,17 +126,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aac468c3",
             "metadata": {},
             "source": [
-                "The attributes of the `AnonymousConstraint` are immutable, thus `con.rhs = 20` would raise an error. \n",
-                "\n",
-                "We can now add the constraint to the model by passing the `AnonymousConstraint` to the `.add_constraint` function.  "
+                "We can now add the constraint to the model by passing the unassigned `Constraint` to the `.add_constraint` function. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0adf929b",
             "metadata": {},
@@ -147,15 +145,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e78c2635",
             "metadata": {},
             "source": [
-                "Note the same output would be generated if passing lhs, sign and rhs as separate arguments to the function:"
+                "The same output would be generated if passing lhs, sign and rhs as separate arguments to the function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c084adec",
             "metadata": {},
@@ -221,138 +219,14 @@
                 "Now, an expression of shape 5 with one term is created. \n",
                 "\n",
                 "**Note:** It is strongly recommended to use `xarray.DataArray`'s for multiplying coefficients with `Variable`'s. It is also possible to use numpy arrays, however these are less secure considering the dimension handling. It is not recommended to use `pandas` objects, as these do not preserve the `linopy` types.  "
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f34b3e54",
-            "metadata": {},
-            "source": [
-                "## Using tuples\n",
-                "\n",
-                "For long expression, it can be more performant to create linear expressions with tuples instead of arithmetic operations, as the latter are calculated iteratively. Therefore, the model's `.linexpr` combines the expression parallelly and also ensures the correct conversion of data types. Let's create two other variables first"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "be747a85",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "y = m.add_variables()\n",
-                "z = m.add_variables()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "96f26023",
-            "metadata": {},
-            "source": [
-                "and a expression using the `.linexpr` function. Here, the convention is to pass pair of coefficients and variables for each term:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4b4b059b",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "tuples = (3, x), (-2, y), (6, z)\n",
-                "expr = m.linexpr(*tuples)\n",
-                "expr"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6920549e",
-            "metadata": {},
-            "source": [
-                "We can now use this expression in the `add_constraints` function."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "5f1ed8f8",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "con = m.add_constraints(expr >= 30)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f73f148b",
-            "metadata": {},
-            "source": [
-                "Again, combining variables with arrays of coefficients is possible and more secure with the usage of tuples. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "28418010",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "coeff = xr.DataArray(range(3), {'additional-dim': pd.RangeIndex(3)})\n",
-                "tuples = (coeff, x), (-2, y), (6, z)\n",
-                "expr = m.linexpr(*tuples)\n",
-                "expr"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6d85d87b",
-            "metadata": {},
-            "source": [
-                "Moreover, the usage of pandas objects as coefficients is possible. However in most cases, these have to have explicit dimension names, otherwise it will raise an error.  "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9ea726f2",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "coeff = pd.Series(range(3))\n",
-                "tuples = (coeff, x), (-2, y), (6, z)\n",
-                "\n",
-                "try:\n",
-                "    expr = m.linexpr(*tuples)\n",
-                "except ValueError as e:\n",
-                "    print(\"This raises an error:\", e)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "d7b48d11",
-            "metadata": {},
-            "source": [
-                "Correct would be:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f9e60919",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "coeff = coeff.rename_axis('additional-dim')\n",
-                "tuples = (coeff, x), (-2, y), (6, z)\n",
-                "m.linexpr(*tuples)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "9898f0c1",
             "metadata": {},
             "source": [
                 "## Using rules \n",
                 "\n",
                 "Similar to the implementation in Pyomo, expressions and constraints can be created using a combination of a function and a set of coordinates to iterate over. For creating expressions, the function itself has to return a `ScalarLinearExpression` which can be obtained by selecting single values of the variables are combining them: "
             ]
@@ -444,22 +318,14 @@
                 "         return (i / 2) * b[i, j] >= i\n",
                 "     else:\n",
                 "         return i * b[i, j]  == 0.\n",
                 "\n",
                 "con = m.add_constraints(bound, coords=coords)\n",
                 "con"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "d918f41c",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "@webio": {
             "lastCommId": null,
             "lastKernelId": null
         },
@@ -474,13 +340,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `linopy-0.1.5/examples/creating-variables.ipynb` & `linopy-0.2/examples/creating-variables.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/examples/manipulating-models.ipynb` & `linopy-0.2/examples/manipulating-models.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/examples/migrating-from-pyomo.ipynb` & `linopy-0.2/examples/migrating-from-pyomo.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/examples/solve-on-remote.ipynb` & `linopy-0.2/examples/solve-on-remote.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/linopy/__init__.py` & `linopy-0.2/linopy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 
 # Note: For intercepting multiplications between xarray dataarrays, Variables and Expressions
 # we need to extend their __mul__ functions with a quick special case
 import linopy.monkey_patch_xarray
 from linopy import model, remote
 from linopy.config import options
 from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
+from linopy.constraints import Constraint
 from linopy.expressions import merge
 from linopy.io import read_netcdf
 from linopy.model import LinearExpression, Model, Variable, available_solvers
 from linopy.remote import RemoteHandler
 from linopy.version import version as __version__
```

### Comparing `linopy-0.1.5/linopy/config.py` & `linopy-0.2/linopy/config.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/linopy/constants.py` & `linopy-0.2/linopy/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,21 +21,29 @@
 long_EQUAL = "=="
 short_GREATER_EQUAL = ">"
 short_LESS_EQUAL = "<"
 
 
 SIGNS = {EQUAL, GREATER_EQUAL, LESS_EQUAL}
 SIGNS_alternative = {long_EQUAL, short_GREATER_EQUAL, short_LESS_EQUAL}
+SIGNS_pretty = {EQUAL: "=", GREATER_EQUAL: "≥", LESS_EQUAL: "≤"}
 
 sign_replace_dict = {
     long_EQUAL: EQUAL,
     short_GREATER_EQUAL: GREATER_EQUAL,
     short_LESS_EQUAL: LESS_EQUAL,
 }
 
+TERM_DIM = "_term"
+STACKED_TERM_DIM = "_stacked_term"
+GROUPED_TERM_DIM = "_grouped_term"
+FACTOR_DIM = "_factor"
+CONCAT_DIM = "_concat"
+HELPER_DIMS = [TERM_DIM, STACKED_TERM_DIM, GROUPED_TERM_DIM, FACTOR_DIM, CONCAT_DIM]
+
 
 class ModelStatus(Enum):
     """
     Model status.
 
     The set of possible model status is a superset of the solver status
     set.
@@ -70,15 +78,15 @@
     @classmethod
     def from_termination_condition(
         cls, termination_condition: "TerminationCondition"
     ) -> "SolverStatus":
         for status in STATUS_TO_TERMINATION_CONDITION_MAP:
             if termination_condition in STATUS_TO_TERMINATION_CONDITION_MAP[status]:
                 return status
-        return cls.unknown
+        return cls("unknown")
 
 
 class TerminationCondition(Enum):
     """
     Termination condition of the solver.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linopy-0.1.5/linopy/constraints.py` & `linopy-0.2/linopy/constraints.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,368 +3,488 @@
 Linopy constraints module.
 
 This module contains implementations for the Constraint{s} class.
 """
 
 import functools
 import re
+import warnings
 from dataclasses import dataclass, field
 from itertools import product
-from typing import Any, Sequence, Union
+from typing import Any, Dict, Sequence, Union
 
 import dask
 import numpy as np
 import pandas as pd
 import xarray as xr
 from deprecation import deprecated
 from numpy import arange, array
-from scipy.sparse import coo_matrix
+from scipy.sparse import csc_matrix
 from xarray import DataArray, Dataset
 
 from linopy import expressions, variables
 from linopy.common import (
-    _merge_inplace,
-    dictsel,
+    LocIndexer,
+    align_lines_by_delimiter,
     forward_as_properties,
+    generate_indices_for_printout,
     has_optimized_model,
-    head_tail_range,
     is_constant,
     maybe_replace_signs,
     print_coord,
     print_single_expression,
     replace_by_map,
+    save_join,
 )
 from linopy.config import options
-from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
+from linopy.constants import (
+    EQUAL,
+    GREATER_EQUAL,
+    HELPER_DIMS,
+    LESS_EQUAL,
+    TERM_DIM,
+    SIGNS_pretty,
+)
 
 
 def conwrap(method, *default_args, **new_default_kwargs):
     @functools.wraps(method)
     def _conwrap(con, *args, **kwargs):
         for k, v in new_default_kwargs.items():
             kwargs.setdefault(k, v)
         return con.__class__(
-            method(con.labels, *default_args, *args, **kwargs), con.model, con.name
+            method(con.data, *default_args, *args, **kwargs), con.model, con.name
         )
 
     _conwrap.__doc__ = f"Wrapper for the xarray {method} function for linopy.Constraint"
     if new_default_kwargs:
         _conwrap.__doc__ += f" with default arguments: {new_default_kwargs}"
 
     return _conwrap
 
 
 def _con_unwrap(con):
-    if isinstance(con, Constraint):
-        return con.labels
-    return con
+    return con.data if isinstance(con, Constraint) else con
 
 
 @forward_as_properties(
-    labels=[
+    data=[
         "attrs",
         "coords",
         "indexes",
-        "name",
-        "shape",
-        "size",
-        "values",
         "dims",
-        "ndim",
+        "sizes",
     ],
+    labels=["values"],
     lhs=["nterm"],
+    rhs=["ndim", "shape", "size"],
 )
 class Constraint:
     """
     Projection to a single constraint in a model.
 
     The Constraint class is a subclass of xr.DataArray hence most xarray
     functions can be applied to it.
     """
 
-    __slots__ = ("_model", "_name", "_labels")
+    __slots__ = ("_data", "_model", "_assigned")
 
-    def __init__(self, labels: DataArray, model: Any, name: str):
+    def __init__(self, data: Dataset, model: Any, name: str = ""):
         """
         Initialize the Constraint.
 
         Parameters
         ----------
         labels : xarray.DataArray
             labels of the constraint.
         model : linopy.Model
             Underlying model.
         name : str
             Name of the constraint.
         """
-        self._labels = labels
+
+        from linopy.model import Model
+
+        if not isinstance(data, Dataset):
+            raise ValueError(f"data must be a Dataset, got {type(data)}")
+
+        if not isinstance(model, Model):
+            raise ValueError(f"model must be a Model, got {type(model)}")
+
+        # check that `labels`, `lower` and `upper`, `sign` and `mask` are in data
+        for attr in ("coeffs", "vars", "sign", "rhs"):
+            if attr not in data:
+                raise ValueError(f"missing '{attr}' in data")
+
+        data = data.assign_attrs(name=name)
+
+        (data,) = xr.broadcast(data, exclude=[TERM_DIM])
+
+        self._data = data
         self._model = model
-        self._name = name
+
+    @property
+    def data(self):
+        """
+        Get the underlying DataArray.
+        """
+        return self._data
 
     @property
     def labels(self):
         """
         Get the labels of the constraint.
         """
-        return self._labels
+        return self.data.labels if self.is_assigned else None
 
     @property
     def model(self):
         """
         Get the model of the constraint.
         """
         return self._model
 
     @property
     def name(self):
         """
-        Get the name of the constraint.
+        Return the name of the constraint.
         """
-        return self._name
+        return self.attrs["name"]
+
+    @property
+    def coord_dims(self):
+        return {k: self.data.dims[k] for k in self.dims if k not in HELPER_DIMS}
+
+    @property
+    def is_assigned(self):
+        return "labels" in self.data
 
     def __repr__(self):
         """
-        Get the string representation of the Constraint.
+        Print the constraint arrays.
         """
-        # return single if only one exist
-        if self.lhs.size == self.nterm:
-            expr_string = print_single_expression(
-                self.lhs.coeffs.values, self.lhs.vars.values, self.lhs.model
-            )
-            name_string = f" `{self.name}`" if self.name else ""
-            header_string = str(self.type) + name_string
-            header = f"{header_string}\n" + "-" * (len(header_string))
-            return f"{header}\n{expr_string} {self.sign.item()} {self.rhs.item()}"
-
-        # create header string
-        name_string = f"`{self.name}`" if self.name else ""
-        shape_string = ", ".join(
-            [f"{self.dims[i]}: {self.shape[i]}" for i in range(self.ndim)]
-        )
-        shape_string = f"({shape_string})"
-        n_masked = (~self.mask).sum().item()
-        mask_string = f" - {n_masked} masked entries" if n_masked else ""
-        header_string = f"{self.type} {name_string} {shape_string}" + mask_string
-        header = f"{header_string}\n" + "-" * (len(header_string))
-
-        # create data string, print only a few values
-        max_print = options["display_max_rows"]
-        split_at = max_print // 2
-        to_print = np.flatnonzero(self.mask)
-        if not len(to_print):
-            # case that all entries are masked
-            to_print = head_tail_range(self.size, max_print)
-            data_string = "None"
-            return f"{header}\n{data_string}"
-
-        truncate = len(to_print) > max_print
-        if truncate:
-            to_print = np.hstack([to_print[:split_at], to_print[-split_at:]])
-
-        # create string, we use numpy to get the indexes
-        data_string = ""
-        idx = np.unravel_index(to_print, self.shape)
-        coords = [self.indexes[dim][idx[i]] for i, dim in enumerate(self.dims)]
-
-        # loop over all values to LinearExpression(print
-        coord_strings = []
-        expr_strings = []
-        sign_strings = []
-        rhs_strings = []
-        trunc_strings = []
-        for i in range(len(to_print)):
-            coord = {dim: c[i] for dim, c in zip(self.dims, coords)}
-            coord_string = print_coord(coord) + ":"
-            expr_string = print_single_expression(
-                self.coeffs.sel(coord).values,
-                self.vars.sel(coord).values,
-                self.lhs.model,
+        max_lines = options["display_max_rows"]
+        dims = list(self.dims)
+        dim_sizes = list(self.sizes.values())[:-1]
+        size = np.prod(dim_sizes)  # that the number of theoretical printouts
+        masked_entries = self.mask.sum().values if self.mask is not None else 0
+        lines = []
+
+        header_string = f"{self.type} `{self.name}`" if self.name else f"{self.type}"
+
+        if size > 1:
+            for indices in generate_indices_for_printout(dim_sizes, max_lines):
+                if indices is None:
+                    lines.append("\t\t...")
+                else:
+                    coord = [
+                        self.data[dims[i]].values[ind] for i, ind in enumerate(indices)
+                    ]
+                    if self.mask is None or self.mask.values[indices]:
+                        expr = print_single_expression(
+                            self.coeffs.values[indices],
+                            self.vars.values[indices],
+                            0,
+                            self.model,
+                        )
+                        sign = SIGNS_pretty[self.sign.values[indices]]
+                        rhs = self.rhs.values[indices]
+                        line = f"{print_coord(coord)}: {expr} {sign} {rhs}"
+                    else:
+                        line = f"{print_coord(coord)}: None"
+                    lines.append(line)
+            lines = align_lines_by_delimiter(lines, list(SIGNS_pretty.values()))
+
+            shape_str = ", ".join(f"{d}: {s}" for d, s in zip(dims, dim_sizes))
+            mask_str = f" - {masked_entries} masked entries" if masked_entries else ""
+            underscore = "-" * (len(shape_str) + len(mask_str) + len(header_string) + 4)
+            lines.insert(0, f"{header_string} ({shape_str}){mask_str}:\n{underscore}")
+        elif size == 1:
+            expr = print_single_expression(self.coeffs, self.vars, 0, self.model)
+            lines.append(
+                f"{header_string}\n{'-'*len(header_string)}\n{expr} {SIGNS_pretty[self.sign.item()]} {self.rhs.item()}"
             )
-            sign_string = f"{self.sign.sel(**dictsel(coord, self.sign.dims)).item()}"
-            rhs_string = f"{self.rhs.sel(**dictsel(coord, self.rhs.dims)).item()}"
-            trunc_string = "\n\t\t..." if i == split_at - 1 and truncate else ""
-
-            coord_strings.append(coord_string)
-            expr_strings.append(expr_string)
-            sign_strings.append(sign_string)
-            rhs_strings.append(rhs_string)
-            trunc_strings.append(trunc_string)
+        else:
+            lines.append(f"{header_string}\n{'-'*len(header_string)}\n<empty>")
 
-        coord_width = max(len(c) for c in coord_strings)
-        expr_width = max(len(e) for e in expr_strings)
+        return "\n".join(lines)
 
-        data_string = ""
-        for c, e, s, r, t in zip(
-            coord_strings, expr_strings, sign_strings, rhs_strings, trunc_strings
-        ):
-            data_string += f"\n{c:<{coord_width}} {e:<{expr_width}} {s:<2} {r}{t}"
+    def __contains__(self, value):
+        return self.data.__contains__(value)
 
-        return f"{header}{data_string}"
+    @property
+    def type(self):
+        """
+        Get the type of the constraint.
+        """
+        return "Constraint" if self.is_assigned else "Constraint (unassigned)"
 
-    @deprecated(details="Use the `labels` property instead of `to_array`")
-    def to_array(self):
+    @property
+    def range(self):
         """
-        Convert the variable array to a xarray.DataArray.
+        Return the range of the constraint.
         """
-        return self.labels
+        return self.data.attrs["label_range"]
 
     @property
-    def type(self):
+    def term_dim(self):
         """
-        Get the type of the constraint.
+        Return the term dimension of the constraint.
         """
-        return "Constraint"
+        return TERM_DIM
 
     @property
     def mask(self):
         """
         Get the mask of the constraint.
 
-        The mask indicates on which coordinates the constraint array is enabled
+        The mask indicates on which coordinates the constraint is enabled
         (True) and disabled (False).
 
         Returns
         -------
         xr.DataArray
         """
-        return (self.labels != -1).astype(bool)
+        return self.data.get("mask")
 
     @property
     def coeffs(self):
         """
         Get the left-hand-side coefficients of the constraint.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.constraints.coeffs[self.name]
+        return self.data.coeffs
 
     @coeffs.setter
     def coeffs(self, value):
-        term_dim = self.name + "_term"
-        value = DataArray(value).broadcast_like(self.vars, exclude=[term_dim])
-        self.model.constraints.coeffs = self.model.constraints.coeffs.drop_vars(
-            self.name
-        ).assign({self.name: value})
+        value = DataArray(value).broadcast_like(self.vars, exclude=[self.term_dim])
+        self._data = self.data.assign(coeffs=value)
+        self.data["coeffs"] = value
 
     @property
     def vars(self):
         """
         Get the left-hand-side variables of the constraint.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.constraints.vars[self.name]
+        return self.data.vars
 
     @vars.setter
     def vars(self, value):
-        term_dim = self.name + "_term"
         if isinstance(value, variables.Variable):
             value = value.labels
         if not isinstance(value, DataArray):
             raise TypeError("Expected value to be of type DataArray or Variable")
-        value = value.broadcast_like(self.coeffs, exclude=[term_dim])
-        self.model.constraints.vars = self.model.constraints.vars.drop_vars(
-            self.name
-        ).assign({self.name: value})
+        value = value.broadcast_like(self.coeffs, exclude=[self.term_dim])
+        self.data["vars"] = value
 
     @property
     def lhs(self):
         """
         Get the left-hand-side linear expression of the constraint.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        term_dim = self.name + "_term"
-        coeffs = self.coeffs.rename({term_dim: "_term"})
-        vars = self.vars.rename({term_dim: "_term"})
-        ds = Dataset({"coeffs": coeffs, "vars": vars})
-        return expressions.LinearExpression(ds, self.model)
+        data = self.data[["coeffs", "vars"]].rename({self.term_dim: TERM_DIM})
+        return expressions.LinearExpression(data, self.model)
 
     @lhs.setter
     def lhs(self, value):
-        if not isinstance(value, expressions.LinearExpression):
-            raise TypeError("Assigned lhs must be a LinearExpression.")
-
-        value = value.rename(_term=self.name + "_term")
-        self.coeffs = value.coeffs
-        self.vars = value.vars
+        value = expressions.as_expression(
+            value, self.model, coords=self.coords, dims=self.coord_dims
+        )
+        self._data = self.data.drop_vars(["coeffs", "vars"]).assign(
+            coeffs=value.coeffs, vars=value.vars, rhs=self.rhs - value.const
+        )
 
     @property
     def sign(self):
         """
         Get the signs of the constraint.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.constraints.sign[self.name]
+        return self.data.sign
 
     @sign.setter
     @is_constant
     def sign(self, value):
         value = maybe_replace_signs(DataArray(value)).broadcast_like(self.sign)
-        self.model.constraints.sign[self.name] = value
+        self.data["sign"] = value
 
     @property
     def rhs(self):
         """
         Get the right hand side constants of the constraint.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.constraints.rhs[self.name]
+        return self.data.rhs
 
     @rhs.setter
-    @is_constant
     def rhs(self, value):
-        if isinstance(value, (variables.Variable, expressions.LinearExpression)):
-            raise TypeError(f"Assigned rhs must be a constant, got {type(value)}).")
-        value = DataArray(value).broadcast_like(self.rhs)
-        self.model.constraints.rhs[self.name] = value
+        value = expressions.as_expression(
+            value, self.model, coords=self.coords, dims=self.coord_dims
+        )
+        self.lhs = self.lhs - value.reset_const()
+        self.data["rhs"] = value.const
 
     @property
     @has_optimized_model
     def dual(self):
         """
         Get the dual values of the constraint.
 
         The function raises an error in case no model is set as a
         reference or the model status is not okay.
         """
-        if not list(self.model.dual):
+        if "dual" not in self.data:
             raise AttributeError(
                 "Underlying is optimized but does not have dual values stored."
             )
-        return self.model.dual[self.name]
+        return self.data["dual"]
+
+    @dual.setter
+    def dual(self, value):
+        """
+        Get the dual values of the constraint.
+        """
+        value = DataArray(value).broadcast_like(self.labels)
+        self.data["dual"] = value
 
     @property
     def shape(self):
         return self.labels.shape
 
-    sel = conwrap(DataArray.sel)
+    @classmethod
+    def from_rule(cls, model, rule, coords):
+        """
+        Create a constraint from a rule and a set of coordinates.
+
+        This functionality mirrors the assignment of constraints as done by
+        Pyomo.
+
+
+        Parameters
+        ----------
+        model : linopy.Model
+            Passed to function `rule` as a first argument.
+        rule : callable
+            Function to be called for each combinations in `coords`.
+            The first argument of the function is the underlying `linopy.Model`.
+            The following arguments are given by the coordinates for accessing
+            the variables. The function has to return a
+            `AnonymousScalarConstraint`. Therefore use the direct getter when
+            indexing variables in the linear expression.
+        coords : coordinate-like
+            Coordinates to processed by `xarray.DataArray`.
+            For each combination of coordinates, the function given by `rule` is called.
+            The order and size of coords has to be same as the argument list
+            followed by `model` in function `rule`.
+
+
+        Returns
+        -------
+        linopy.Constraint
+
+        Examples
+        --------
+        >>> from linopy import Model, LinearExpression, Constraint
+        >>> m = Model()
+        >>> coords = pd.RangeIndex(10), ["a", "b"]
+        >>> x = m.add_variables(0, 100, coords)
+        >>> def bound(m, i, j):
+        ...     if i % 2:
+        ...         return (i - 1) * x[i - 1, j] >= 0
+        ...     else:
+        ...         return i * x[i, j] >= 0
+        ...
+        >>> con = Constraint.from_rule(m, bound, coords)
+        >>> con = m.add_constraints(con)
+        """
+        if not isinstance(coords, xr.core.dataarray.DataArrayCoordinates):
+            coords = DataArray(coords=coords).coords
+        shape = list(map(len, coords.values()))
+
+        # test output type
+        output = rule(model, *[c.values[0] for c in coords.values()])
+        if not isinstance(output, AnonymousScalarConstraint) and output is not None:
+            msg = f"`rule` has to return AnonymousScalarConstraint not {type(output)}."
+            raise TypeError(msg)
 
-    isel = conwrap(DataArray.isel)
+        combinations = product(*[c.values for c in coords.values()])
+        placeholder_lhs = expressions.ScalarLinearExpression((np.nan,), (-1,), model)
+        placeholder = AnonymousScalarConstraint(placeholder_lhs, "=", np.nan)
+        cons = [rule(model, *coord) or placeholder for coord in combinations]
+        exprs = [con.lhs for con in cons]
+
+        lhs = expressions.LinearExpression._from_scalarexpression_list(
+            exprs, coords, model
+        )
+        sign = DataArray(array([c.sign for c in cons]).reshape(shape), coords)
+        rhs = DataArray(array([c.rhs for c in cons]).reshape(shape), coords)
+        data = lhs.data.assign(sign=sign, rhs=rhs)
+        return cls(data, model=model)
+
+    @property
+    def flat(self):
+        """
+        Convert the constraint to a pandas DataFrame.
+
+        The resulting DataFrame represents a long table format of the all
+        non-masked constraints with non-zero coefficients. It contains the
+        columns `labels`, `coeffs`, `vars`, `rhs`, `sign`.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+        """
+        ds = self.data
+        # if keys is not None:
+        #     if isinstance(keys, str):
+        #         keys = [keys]
+        #     ds = ds[keys]
+        if not ds.sizes:
+            # fallback for weird error raised due to missing index
+            df = pd.DataFrame({k: ds[k].item() for k in ds}, index=[0])
+        else:
+            df = ds.to_dataframe()
+        df = df[(df.labels != -1) & (df.vars != -1) & (df.coeffs != 0)]
+        # Group repeated variables in the same constraint
+        agg = dict(coeffs="sum", rhs="first", sign="first")
+        agg |= {k: "first" for k in df.columns if k not in agg}
+        df = df.groupby(["labels", "vars"], as_index=False).aggregate(agg)
+
+        any_nan = df.isna().any()
+        if any_nan.any():
+            fields = ", ".join("`" + df.columns[any_nan] + "`")
+            raise ValueError(
+                f"Constraint `{self.name}` contains nan's in field(s) {fields}"
+            )
+        return df
+
+    sel = conwrap(Dataset.sel)
+
+    isel = conwrap(Dataset.isel)
 
 
 @dataclass(repr=False)
 class Constraints:
     """
     A constraint container used for storing multiple constraint arrays.
     """
 
-    labels: Dataset = field(default_factory=Dataset)
-    coeffs: Dataset = field(default_factory=Dataset)
-    vars: Dataset = field(default_factory=Dataset)
-    sign: Dataset = field(default_factory=Dataset)
-    rhs: Dataset = field(default_factory=Dataset)
-    blocks: Dataset = field(default_factory=Dataset)
+    data: Dict[str, Constraint] = field(default_factory=dict)
     model: Any = None  # Model is not defined due to circular imports
 
     dataset_attrs = ["labels", "coeffs", "vars", "sign", "rhs"]
     dataset_names = [
         "Labels",
         "Left-hand-side coefficients",
         "Left-hand-side variables",
@@ -374,137 +494,172 @@
 
     def __repr__(self):
         """
         Return a string representation of the linopy model.
         """
         r = "linopy.model.Constraints"
         line = "-" * len(r)
-        r += f"\n{line}\n\n"
+        r += f"\n{line}\n"
 
-        labelprint = self.labels.__repr__()
-        coordspattern = r"(?s)(?<=\<xarray\.Dataset\>\n).*?(?=Data variables:)"
-        r += re.search(coordspattern, labelprint).group()
-        r += "Constraints:\n"
-        for name in self.labels:
-            r += f"  *  {name} ({', '.join(self.labels[name].coords)})\n"
+        for name, ds in self.items():
+            coords = " (" + ", ".join(ds.coords) + ")" if ds.coords else ""
+            r += f" * {name}{coords}\n"
+        if not len(list(self)):
+            r += "<empty>\n"
         return r
 
     def __getitem__(
         self, names: Union[str, Sequence[str]]
     ) -> Union[Constraint, "Constraints"]:
         if isinstance(names, str):
-            return Constraint(self.labels[names], self.model, names)
+            return self.data[names]
 
-        return self.__class__(
-            self.labels[names],
-            self.coeffs[names],
-            self.vars[names],
-            self.sign[names],
-            self.rhs[names],
-            self.model,
-        )
+        return self.__class__({name: self.data[name] for name in names}, self.model)
+
+    def __getattr__(self, name: str):
+        # If name is an attribute of self (including methods and properties), return that
+        if name in self.data:
+            return self.data[name]
+        else:
+            raise AttributeError(
+                f"Constraints has no attribute `{name}` or the attribute is not accessible, e.g. raises an error."
+            )
+
+    def __len__(self):
+        return self.data.__len__()
 
     def __iter__(self):
-        return self.labels.__iter__()
+        return self.data.__iter__()
 
-    _merge_inplace = _merge_inplace
+    def items(self):
+        return self.data.items()
 
     def _ipython_key_completions_(self):
         """
         Provide method for the key-autocompletions in IPython.
 
         See
         http://ipython.readthedocs.io/en/stable/config/integrating.html#tab-completion
         For the details.
         """
         return list(self)
 
-    def add(
-        self,
-        name,
-        labels: DataArray,
-        coeffs: DataArray,
-        vars: DataArray,
-        sign: DataArray,
-        rhs: DataArray,
-    ):
-        """
-        Add constraint `name`.
-        """
-        self._merge_inplace("labels", labels, name, fill_value=-1)
-        self._merge_inplace("coeffs", coeffs, name)
-        self._merge_inplace("vars", vars, name, fill_value=-1)
-        self._merge_inplace("sign", sign, name)
-        self._merge_inplace("rhs", rhs, name)
+    def add(self, constraint):
+        """
+        Add a constraint to the constraints constrainer.
+        """
+        self.data[constraint.name] = constraint
 
     def remove(self, name):
         """
         Remove constraint `name` from the constraints.
         """
-        for attr in self.dataset_attrs:
-            setattr(self, attr, getattr(self, attr).drop_vars(name))
+        self.data.pop(name)
+
+    @property
+    def loc(self):
+        return LocIndexer(self)
+
+    @property
+    def labels(self):
+        """
+        Get the labels of all constraints.
+        """
+        return save_join(*[v.labels.rename(k) for k, v in self.items()])
+
+    @property
+    def coeffs(self):
+        """
+        Get the coefficients of all constraints.
+        """
+        return save_join(*[v.coeffs.rename(k) for k, v in self.items()])
+
+    @property
+    def vars(self):
+        """
+        Get the variables of all constraints.
+        """
+        return save_join(*[v.vars.rename(k) for k, v in self.items()])
+
+    @property
+    def sign(self):
+        """
+        Get the signs of all constraints.
+        """
+        return save_join(*[v.sign.rename(k) for k, v in self.items()])
+
+    @property
+    def rhs(self):
+        """
+        Get the right-hand-side constants of all constraints.
+        """
+        return save_join(*[v.rhs.rename(k) for k, v in self.items()])
+
+    @property
+    def dual(self):
+        """
+        Get the dual values of all constraints.
+        """
+        try:
+            return save_join(*[v.dual.rename(k) for k, v in self.items()])
+        except AttributeError:
+            return Dataset()
 
     @property
     def coefficientrange(self):
         """
         Coefficient range of the constraint.
         """
-        return (
-            xr.concat(
-                [self.coeffs.min(), self.coeffs.max()],
-                dim=pd.Index(["min", "max"]),
-            )
-            .to_dataframe()
-            .T
-        )
+        d = {
+            k: [self[k].coeffs.min().item(), self[k].coeffs.max().item()] for k in self
+        }
+        return pd.DataFrame(d, index=["min", "max"]).T
 
     @property
     def ncons(self):
         """
-        Get the number all constraints which were at some point added to the
-        model.
+        Get the number all constraints effectively used by the model.
 
-        These also include constraints with missing labels.
+        These excludes constraints with missing labels.
         """
-        return self.ravel("labels", filter_missings=True).shape[0]
+        return len(self.flat.labels.unique())
 
     @property
     def inequalities(self):
         """
         Get the subset of constraints which are purely inequalities.
         """
-        return self[
-            [n for n, s in self.sign.items() if s in (LESS_EQUAL, GREATER_EQUAL)]
-        ]
+        return self[[n for n, s in self.items() if (s.sign != EQUAL).all()]]
 
     @property
     def equalities(self):
         """
         Get the subset of constraints which are purely equalities.
         """
-        return self[[n for n, s in self.sign.items() if s == EQUAL]]
+        return self[[n for n, s in self.items() if (s.sign == EQUAL).all()]]
 
     def sanitize_zeros(self):
         """
         Filter out terms with zero and close-to-zero coefficient.
         """
         for name in self:
-            not_zero = abs(self.coeffs[name]) > 1e-10
-            self.vars[name] = self.vars[name].where(not_zero, -1)
-            self.coeffs[name] = self.coeffs[name].where(not_zero)
+            not_zero = abs(self[name].coeffs) > 1e-10
+            self[name].vars = self[name].vars.where(not_zero, -1)
+            self[name].coeffs = self[name].coeffs.where(not_zero)
 
     def sanitize_missings(self):
         """
         Set constraints labels to -1 where all variables in the lhs are
         missing.
         """
         for name in self:
-            term_dim = name + "_term"
-            contains_non_missing = (self.vars[name] != -1).any(term_dim)
-            self.labels[name] = self.labels[name].where(contains_non_missing, -1)
+            contains_non_missing = (self[name].vars != -1).any(self[name].term_dim)
+            self[name].data["labels"] = self[name].labels.where(
+                contains_non_missing, -1
+            )
 
     def get_name_by_label(self, label):
         """
         Get the constraint name of the constraint containing the passed label.
 
         Parameters
         ----------
@@ -520,53 +675,50 @@
         Returns
         -------
         name : str
             Name of the containing constraint.
         """
         if not isinstance(label, (float, int)) or label < 0:
             raise ValueError("Label must be a positive number.")
-        for name, labels in self.labels.items():
-            if label in labels:
+        for name, ds in self.items():
+            if label in ds.labels:
                 return name
         raise ValueError(f"No constraint found containing the label {label}.")
 
-    def get_blocks(self, block_map):
+    def set_blocks(self, block_map):
         """
         Get a dataset of same shape as constraints.labels with block values.
 
         Let N be the number of blocks.
         The following cases are considered:
 
             * where are all vars are -1, the block is -1
             * where are all vars are 0, the block is 0
             * where all vars are n, the block is n
             * where vars are n or 0 (both present), the block is n
             * N+1 otherwise
         """
         N = block_map.max()
-        var_blocks = replace_by_map(self.vars, block_map)
-        res = xr.full_like(self.labels, N + 1, dtype=block_map.dtype)
 
-        for name, entries in var_blocks.items():
-            term_dim = f"{name}_term"
+        for name, constraint in self.items():
+            res = xr.full_like(constraint.labels, N + 1, dtype=block_map.dtype)
+            entries = replace_by_map(constraint.vars, block_map)
 
             not_zero = entries != 0
             not_missing = entries != -1
             for n in range(N + 1):
                 not_n = entries != n
                 mask = not_n & not_zero & not_missing
-                res[name] = res[name].where(mask.any(term_dim), n)
-
-            res[name] = res[name].where(not_missing.any(term_dim), -1)
-            res[name] = res[name].where(not_zero.any(term_dim), 0)
+                res = res.where(mask.any(constraint.term_dim), n)
 
-        self.blocks = res
-        self.var_blocks = var_blocks
-        return self.blocks
+            res = res.where(not_missing.any(constraint.term_dim), -1)
+            res = res.where(not_zero.any(constraint.term_dim), 0)
+            constraint.data["blocks"] = res
 
+    @deprecated("0.2", details="Use `to_dataframe` or `flat` instead.")
     def iter_ravel(self, key, broadcast_like="labels", filter_missings=False):
         """
         Create an generator which iterates over all arrays in `key` and
         flattens them.
 
         Parameters
         ----------
@@ -583,33 +735,28 @@
             When enabled, the data is load into memory. The default is False.
 
 
         Yields
         ------
         flat : np.array/dask.array
         """
-        if isinstance(key, str):
-            ds = getattr(self, key)
-        elif isinstance(key, xr.Dataset):
-            ds = key
-        else:
-            raise TypeError("Argument `key` must be of type string or xarray.Dataset")
-
         assert broadcast_like in ["labels", "vars"]
 
-        for name, values in getattr(self, broadcast_like).items():
-            broadcasted = ds[name].broadcast_like(values)
+        for name, constraint in self.items():
+            values = constraint.data[broadcast_like]
+            ds = constraint.data[key]
+            broadcasted = ds.broadcast_like(values)
             if values.chunks is not None:
                 broadcasted = broadcasted.chunk(values.chunks)
 
             if filter_missings:
                 flat = np.ravel(broadcasted)
                 mask = np.ravel(values) != -1
                 if broadcast_like != "labels":
-                    labels = np.ravel(self.labels[name].broadcast_like(values))
+                    labels = np.ravel(constraint.labels.broadcast_like(values))
                     mask &= labels != -1
                 flat = flat[mask]
                 if pd.isna(flat).any():
                     names = self.dataset_names
                     ds_name = names[self.dataset_attrs.index(key)]
                     bc_name = names[self.dataset_attrs.index(broadcast_like)]
                     err = (
@@ -617,14 +764,15 @@
                         f"where {bc_name.lower()} are defined (not -1)."
                     )
                     raise ValueError(err)
             else:
                 flat = broadcasted.data.ravel()
             yield flat
 
+    @deprecated("0.2", details="Use `to_dataframe` or `flat` instead.")
     def ravel(self, key, broadcast_like="labels", filter_missings=False, compute=True):
         """
         Ravel and concate all arrays in `key` while aligning to
         `broadcast_like`.
 
         Parameters
         ----------
@@ -643,263 +791,85 @@
         Returns
         -------
         flat
             One dimensional data with all values in `key`.
         """
         res = list(self.iter_ravel(key, broadcast_like, filter_missings))
         res = np.concatenate(res)
-        if compute:
-            return dask.compute(res)[0]
-        else:
-            return res
+        return dask.compute(res)[0] if compute else res
 
-    def to_matrix(self, filter_missings=False):
+    @property
+    def flat(self) -> pd.DataFrame:
         """
-        Construct a constraint matrix in sparse format.
-
-        Missing values, i.e. -1 in labels and vars, are ignored filtered
-        out.
+        Convert all constraint to a single pandas Dataframe.
 
-        If filter_missings is set to True, the index of the rows and
-        columns
-        correspond to the constraint and variable labels stored in the
-        model.
-        If set to False, the rows correspond to the constraints given by
-        `m.constraints.ravel('labels', filter_missings=True)` and
-        columns to
-        `m.variables.ravel('labels', filter_missings=True)` where `m` is
-        the
-        underlying model. The matrix has then a shape of (`m.ncons`,
-        `m.nvars`).
-        """
-        self.sanitize_missings()
-
-        keys = ["coeffs", "labels", "vars"]
-        data, rows, cols = [
-            self.ravel(k, broadcast_like="vars", filter_missings=True) for k in keys
-        ]
-        shape = (self.model._cCounter, self.model._xCounter)
+        The resulting dataframe is a long format with columns
+        `labels`, `coeffs`, `vars`, `rhs`, `sign`.
 
-        if filter_missings:
-            # We have to map the variables to the filtered layout
-            clabels = self.ravel("labels", filter_missings=True)
-            ncons = clabels.shape[0]
-            cmap = np.empty(self.model._cCounter)
-            cmap[clabels] = arange(clabels.shape[0])
-            rows = cmap[rows]
-
-            variables = self.model.variables
-            vlabels = variables.ravel("labels", filter_missings=True)
-            nvars = vlabels.shape[0]
-            vmap = np.empty(self.model._xCounter)
-            vmap[vlabels] = arange(nvars)
-            cols = vmap[cols]
-
-            shape = (ncons, nvars)  # same as model.nvars/ncons but already there
-
-        # Group repeated variables in the same constraint
-        df = pd.DataFrame({"data": data, "rows": rows, "cols": cols})
-        df = df.groupby(["rows", "cols"], as_index=False).sum()
-
-        return coo_matrix((df.data, (df.rows, df.cols)), shape=shape)
-
-
-@dataclass(repr=False)
-@forward_as_properties(
-    labels=[
-        "attrs",
-        "coords",
-        "indexes",
-        "shape",
-        "size",
-        "values",
-        "dims",
-        "ndim",
-    ],
-    lhs=["nterm", "coeffs", "vars"],
-)
-class AnonymousConstraint:
-    """
-    A constraint container used for storing multiple constraint arrays.
-    """
-
-    _lhs: "expressions.LinearExpression"
-    _sign: Union[DataArray, str]
-    _rhs: Union[DataArray, float, int]
-
-    def __post_init__(self):
-        """
-        Initialize a anonymous constraint.
+        Returns
+        -------
+        pd.DataFrame
         """
-        if isinstance(self.rhs, (variables.Variable, expressions.LinearExpression)):
-            raise TypeError(f"Assigned rhs must be a constant, got {type(self.rhs)}).")
-        lhs_data, rhs = xr.align(self.lhs.data, DataArray(self.rhs))
-        self._labels = (lhs_data.vars.chunk() + rhs).sum("_term")
-        self._labels.data = np.full(self.labels.shape, np.nan)
-        self._lhs = expressions.LinearExpression(lhs_data, self.lhs.model)
-        self._rhs = rhs
-        self._sign = DataArray(self.sign)
+        dfs = [self[k].flat for k in self]
+        if not len(dfs):
+            return pd.DataFrame(columns=["coeffs", "vars", "labels", "key"])
+        df = pd.concat(dfs, ignore_index=True)
+        unique_labels = df.labels.unique()
+        map_labels = pd.Series(np.arange(len(unique_labels)), index=unique_labels)
+        df["key"] = df.labels.map(map_labels)
+        return df
 
-    def __repr__(self):
-        """
-        Get the representation of the AnonymousConstraint.
+    def to_matrix(self, filter_missings=True):
         """
-        return Constraint.__repr__(self)
-
-    @property
-    def name(self):
-        return ""
-
-    @property
-    def type(self):
-        """
-        Get the type of the constraint.
-        """
-        # needed for __repr__ compatibility.
-        return "AnomymousConstraint"
+        Construct a constraint matrix in sparse format.
 
-    @property
-    def mask(self):
-        """
-        Get the mask of the constraint.
+        Missing values, i.e. -1 in labels and vars, are ignored filtered
+        out.
         """
-        # needed for __repr__ compatibility.
-        return xr.full_like(self.labels, True, dtype=bool)
+        # TODO: rename "filter_missings" to "~labels_as_coordinates"
+        cons = self.flat
 
-    @property
-    def labels(self):
-        """
-        Get the labels of the constraint.
-        """
-        return self._labels
+        if not len(self):
+            return None
 
-    @property
-    def lhs(self):
-        """
-        Get the left hand side of the constraint.
-        """
-        return self._lhs
+        if filter_missings:
+            vars = self.model.variables.flat
+            shape = (cons.key.max() + 1, vars.key.max() + 1)
+            cons["vars"] = cons.vars.map(vars.set_index("labels").key)
+            return csc_matrix((cons.coeffs, (cons.key, cons.vars)), shape=shape)
+        else:
+            shape = self.model.shape
+            return csc_matrix((cons.coeffs, (cons.labels, cons.vars)), shape=shape)
 
-    @property
-    def sign(self):
+    def reset_dual(self):
         """
-        Get the sign of the constraint.
+        Reset the stored solution of variables.
         """
-        return self._sign
+        for k, c in self.items():
+            if "dual" in c:
+                c._data = c.data.drop_vars("dual")
 
-    @property
-    def rhs(self):
-        """
-        Get the right hand side of the constraint.
-        """
-        return self._rhs
 
-    @classmethod
-    def from_rule(cls, model, rule, coords):
+# define AnonymousConstraint for backwards compatibility
+class AnonymousConstraint(Constraint):
+    def __init__(self, lhs, sign, rhs):
         """
-        Create a constraint from a rule and a set of coordinates.
-
-        This functionality mirrors the assignment of constraints as done by
-        Pyomo.
-
-
-        Parameters
-        ----------
-        model : linopy.Model
-            Passed to function `rule` as a first argument.
-        rule : callable
-            Function to be called for each combinations in `coords`.
-            The first argument of the function is the underlying `linopy.Model`.
-            The following arguments are given by the coordinates for accessing
-            the variables. The function has to return a
-            `AnonymousScalarConstraint`. Therefore use the direct getter when
-            indexing variables in the linear expression.
-        coords : coordinate-like
-            Coordinates to processed by `xarray.DataArray`.
-            For each combination of coordinates, the function given by `rule` is called.
-            The order and size of coords has to be same as the argument list
-            followed by `model` in function `rule`.
-
-
-        Returns
-        -------
-        linopy.AnonymousConstraint
-
-        Examples
-        --------
-        >>> from linopy import Model, LinearExpression
-        >>> m = Model()
-        >>> coords = pd.RangeIndex(10), ["a", "b"]
-        >>> x = m.add_variables(0, 100, coords)
-        >>> def bound(m, i, j):
-        ...     if i % 2:
-        ...         return (i - 1) * x[i - 1, j] >= 0
-        ...     else:
-        ...         return i * x[i, j] >= 0
-        ...
-        >>> con = AnonymousConstraint.from_rule(m, bound, coords)
-        >>> con = m.add_constraints(con)
+        Initialize a anonymous constraint.
         """
-        if not isinstance(coords, xr.core.dataarray.DataArrayCoordinates):
-            coords = DataArray(coords=coords).coords
-        shape = list(map(len, coords.values()))
-
-        # test output type
-        output = rule(model, *[c.values[0] for c in coords.values()])
-        if not isinstance(output, AnonymousScalarConstraint) and not output is None:
-            msg = f"`rule` has to return AnonymousScalarConstraint not {type(output)}."
-            raise TypeError(msg)
-
-        combinations = product(*[c.values for c in coords.values()])
-        placeholder_lhs = expressions.ScalarLinearExpression((np.nan,), (-1,), model)
-        placeholder = AnonymousScalarConstraint(placeholder_lhs, "=", np.nan)
-        cons = [rule(model, *coord) or placeholder for coord in combinations]
-        exprs = [con.lhs for con in cons]
-
-        lhs = expressions.LinearExpression._from_scalarexpression_list(
-            exprs, coords, model
+        # raise deprecation warning
+        warnings.warn(
+            "AnonymousConstraint is deprecated, use Constraint instead.",
         )
-        sign = DataArray(array([c.sign for c in cons]).reshape(shape), coords)
-        rhs = DataArray(array([c.rhs for c in cons]).reshape(shape), coords)
-        return cls(lhs, sign, rhs)
-
-    def sel(self, indexers=None, **indexer_kwargs):
-        """
-        Select a subset of the AnonymousConstraint array.
 
-        The function mirrors the behavior of the `xarray.Dataset.sel` function.
-        For further information please refer to its docstring.
-
-        Parameters
-        ----------
-        indexers : dict, optional
-            A dict with keys matching the dimensions and values given by scalars, slices or arrays. By default None.
-        **indexers_kwargs : {dim: indexer, ...}, optional
-            The keyword arguments form of ``indexers``.
-            One of indexers or indexers_kwargs must be provided.
-
-        Returns
-        -------
-        AnonymousConstraint
-            A new AnonymousConstraint including all values of the original
-            whose indexes lay within the realm of selection.
-        """
-
-        indexers = xr.core.utils.either_dict_or_kwargs(indexers, indexer_kwargs, "sel")
-
-        lhs_indexers = {k: v for k, v in indexers.items() if k in self.lhs.dims}
-        lhs = self.lhs.sel(lhs_indexers)
-
-        sign_indexers = {k: v for k, v in indexers.items() if k in self.sign.dims}
-        sign = self.sign.sel(sign_indexers)
-
-        rhs_indexers = {k: v for k, v in indexers.items() if k in self.rhs.dims}
-        rhs = self.rhs.sel(rhs_indexers)
-
-        return self.__class__(lhs, sign, rhs)
+        if not isinstance(lhs, expressions.LinearExpression):
+            raise TypeError(
+                f"Assigned lhs must be a LinearExpression, got {type(lhs)})."
+            )
+        data = lhs.data.assign(sign=sign, rhs=rhs)
+        super().__init__(data, lhs.model)
 
 
 class AnonymousScalarConstraint:
     """
     Container for anonymous scalar constraint.
 
     This contains a left-hand-side (lhs), a sign and a right-hand-side
@@ -921,15 +891,15 @@
         self._rhs = rhs
 
     def __repr__(self):
         """
         Get the representation of the AnonymousScalarConstraint.
         """
         expr_string = print_single_expression(
-            self.lhs.coeffs, self.lhs.vars, self.lhs.model
+            self.lhs.coeffs, self.lhs.vars, 0, self.lhs.model
         )
         return f"AnonymousScalarConstraint: {expr_string} {self.sign} {self.rhs}"
 
     @property
     def lhs(self):
         """
         Get the left hand side of the constraint.
@@ -946,9 +916,14 @@
     @property
     def rhs(self):
         """
         Get the right hand side of the constraint.
         """
         return self._rhs
 
+    def to_constraint(self):
+        data = self.lhs.to_linexpr().data.assign(sign=self.sign, rhs=self.rhs)
+        return Constraint(data=data, model=self.lhs.model)
+
+    @deprecated(details="Use to_constraint instead.")
     def to_anonymous_constraint(self):
-        return AnonymousConstraint(self.lhs.to_linexpr(), self.sign, self.rhs)
+        return self.to_constraint()
```

### Comparing `linopy-0.1.5/linopy/expressions.py` & `linopy-0.2/linopy/expressions.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,38 +4,51 @@
 Linopy expressions module.
 
 This module contains definition related to affine expressions.
 """
 
 import functools
 import logging
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from itertools import product, zip_longest
 from typing import Any, Mapping, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 import xarray.core.groupby
 import xarray.core.rolling
 from deprecation import deprecated
-from numpy import array, nan
+from numpy import arange, array, nan
+from scipy.sparse import csc_matrix
 from xarray import DataArray, Dataset
 from xarray.core.dataarray import DataArrayCoordinates
 
-from linopy import constraints, variables
+from linopy import constraints, expressions, variables
 from linopy.common import (
+    LocIndexer,
     as_dataarray,
+    check_common_keys_values,
+    fill_missing_coords,
     forward_as_properties,
-    head_tail_range,
-    print_coord,
+    generate_indices_for_printout,
+    get_index_map,
     print_single_expression,
 )
 from linopy.config import options
-from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
+from linopy.constants import (
+    EQUAL,
+    FACTOR_DIM,
+    GREATER_EQUAL,
+    GROUPED_TERM_DIM,
+    HELPER_DIMS,
+    LESS_EQUAL,
+    STACKED_TERM_DIM,
+    TERM_DIM,
+)
 
 
 def exprwrap(method, *default_args, **new_default_kwargs):
     @functools.wraps(method)
     def _exprwrap(expr, *args, **kwargs):
         for k, v in new_default_kwargs.items():
             kwargs.setdefault(k, v)
@@ -63,55 +76,159 @@
 @dataclass
 @forward_as_properties(groupby=["dims", "groups"])
 class LinearExpressionGroupby:
     """
     GroupBy object specialized to grouping LinearExpression objects.
     """
 
-    groupby: xr.core.groupby.DatasetGroupBy
+    data: xr.Dataset
+    group: xr.DataArray
     model: Any
+    kwargs: Mapping[str, Any] = field(default_factory=dict)
+
+    @property
+    def groupby(self):
+        """
+        Groups the data using the specified group and kwargs.
+
+        Returns
+        -------
+        xarray.core.groupby.DataArrayGroupBy
+            The groupby object.
+        """
+        return self.data.groupby(group=self.group, **self.kwargs)
 
     def map(self, func, shortcut=False, args=(), **kwargs):
+        """
+        Apply a specified function to the groupby object.
+
+        Parameters
+        ----------
+        func : callable
+            The function to apply.
+        shortcut : bool, optional
+            Whether to use shortcut or not.
+        args : tuple, optional
+            The arguments to pass to the function.
+        **kwargs
+            Arbitrary keyword arguments.
+
+        Returns
+        -------
+        LinearExpression
+            The result of applying the function to the groupby object.
+        """
+
         return LinearExpression(
             self.groupby.map(func, shortcut=shortcut, args=args, **kwargs), self.model
         )
 
-    def sum(self, **kwargs):
-        def func(ds):
-            ds = LinearExpression._sum(ds, self.groupby._group_dim)
-            ds = ds.assign_coords(_term=np.arange(len(ds._term)))
-            return ds
+    def sum(self, use_fallback=False, **kwargs):
+        """
+        Sum the groupby object.
+
+        There are two options to perform the summation over groups.
+        The first and faster option uses an internal reindexing mechanism, which
+        however ignores keyword arguments. This will be used when passing a
+        pandas object or a DataArray as group, and setting `use_fallack`
+        to False (default).
+        The second uses a mapping of xarray groups which performs slower but
+        also takes into account the keyword arguments.
+
+        Parameters
+        ----------
+        use_fallback : bool
+            Whether to use the fallback implementation, which is a sort of default
+            xarray implementation. If set to False, the operation will be much
+            faster but keyword arguments are ignored. Defaults to False.
+        **kwargs
+            Arbitrary keyword arguments.
+
+        Returns
+        -------
+        LinearExpression
+            The sum of the groupby object.
+        """
+        non_fallback_types = (pd.Series, pd.DataFrame, xr.DataArray)
+        if isinstance(self.group, non_fallback_types) and not use_fallback:
+            group = self.group
+            group_name = getattr(group, "name", "group") or "group"
+
+            if isinstance(group, DataArray):
+                group = group.to_pandas()
+
+            int_map = None
+            if isinstance(group, pd.DataFrame):
+                int_map = get_index_map(*group.values.T)
+                orig_group = group
+                group = group.apply(tuple, axis=1).map(int_map)
+
+            group_dim = group.index.name
+            arrays = [group, group.groupby(group).cumcount()]
+            idx = pd.MultiIndex.from_arrays(
+                arrays, names=[group_name, GROUPED_TERM_DIM]
+            )
+            ds = self.data.assign_coords({group_dim: idx})
+            ds = ds.unstack(group_dim, fill_value=LinearExpression.fill_value)
+            ds = LinearExpression._sum(ds, dims=GROUPED_TERM_DIM)
+
+            if int_map is not None:
+                index = ds.indexes["group"].map({v: k for k, v in int_map.items()})
+                index.names = orig_group.columns
+                index.name = group_name
+                ds = xr.Dataset(ds.assign_coords({group_name: index}))
+
+            return LinearExpression(ds, self.model)
 
-        return self.map(func, **kwargs)
+        else:
+
+            def func(ds):
+                ds = LinearExpression._sum(ds, self.groupby._group_dim)
+                ds = ds.assign_coords({TERM_DIM: np.arange(len(ds._term))})
+                return ds
+
+            return self.map(func, **kwargs)
 
     def roll(self, **kwargs):
+        """
+        Roll the groupby object.
+
+        **kwargs
+            Arbitrary keyword arguments.
+
+        Returns
+        -------
+        LinearExpression
+            The result of rolling over the groups.
+        """
         return self.map(Dataset.roll, **kwargs)
 
 
 @dataclass
 @forward_as_properties(rolling=["center", "dim", "obj", "rollings", "window"])
 class LinearExpressionRolling:
     """
     GroupBy object specialized to grouping LinearExpression objects.
     """
 
     rolling: xr.core.rolling.DataArrayRolling
     model: Any
 
     def sum(self, **kwargs):
+        data = self.rolling.construct("_rolling_term", keep_attrs=True)
         ds = (
-            self.rolling.construct("_rolling_term", keep_attrs=True)
-            .rename(_term="_stacked_term")
-            .stack(_term=["_stacked_term", "_rolling_term"])
-            .reset_index("_term", drop=True)
+            data[["coeffs", "vars"]]
+            .rename({TERM_DIM: STACKED_TERM_DIM})
+            .stack({TERM_DIM: [STACKED_TERM_DIM, "_rolling_term"]}, create_index=False)
         )
+        ds["const"] = data.const.sum("_rolling_term")
         return LinearExpression(ds, self.model)
 
 
-@forward_as_properties(data=["attrs", "coords", "indexes"])
+@forward_as_properties(data=["attrs", "coords", "indexes", "sizes"], const=["ndim"])
 class LinearExpression:
     """
     A linear expression consisting of terms of coefficients and variables.
 
     The LinearExpression class is a subclass of xarray.Dataset which allows to
     apply most xarray functions on it. However most arithmetic operations are
     overwritten. Like this you can easily expand and modify the linear
@@ -146,234 +263,241 @@
     <class 'linopy.expressions.LinearExpression'>
     """
 
     __slots__ = ("_data", "_model")
     __array_ufunc__ = None
     __array_priority__ = 10000
 
-    _fill_value = {"vars": -1, "coeffs": np.nan}
+    _fill_value = {"vars": -1, "coeffs": np.nan, "const": 0}
 
     def __init__(self, data, model):
         from linopy.model import Model
 
         if data is None:
-            da = xr.DataArray([], dims=["_term"])
-            data = Dataset({"coeffs": da, "vars": da})
-
-        if not isinstance(data, Dataset):
+            da = xr.DataArray([], dims=[TERM_DIM])
+            data = Dataset({"coeffs": da, "vars": da, "const": 0})
+        elif isinstance(data, DataArray):
+            # assume only constant are passed
+            const = fill_missing_coords(data)
+            da = xr.DataArray([], dims=[TERM_DIM])
+            data = Dataset({"coeffs": da, "vars": da, "const": const})
+        elif not isinstance(data, Dataset):
             raise ValueError(
-                f"data must be an instance of xarray.Dataset, got {type(data)}"
+                f"data must be an instance of xarray.Dataset or xarray.DataArray, got {type(data)}"
             )
 
         if not set(data).issuperset({"coeffs", "vars"}):
-            raise ValueError("data must contain the variables 'coeffs' and 'vars'")
-
-        term_dims = [d for d in data.dims if d.endswith("_term")]
-        if not term_dims:
-            raise ValueError("data must contain one dimension ending with '_term'")
-        term_dim = term_dims[0]
-
-        # make sure that all non-helper dims have coordinates
-        missing_coords = set(data.dims) - set(data.coords) - {term_dim}
-        if missing_coords:
             raise ValueError(
-                f"Dimensions {missing_coords} have no coordinates. For "
-                "consistency all dimensions must have coordinates."
+                "data must contain the fields 'coeffs' and 'vars' or 'const'"
             )
 
         if np.issubdtype(data.vars, np.floating):
             data["vars"] = data.vars.fillna(-1).astype(int)
+        if not np.issubdtype(data.coeffs, np.floating):
+            data["coeffs"] = data.coeffs.astype(float)
+
+        data = fill_missing_coords(data)
 
-        (data,) = xr.broadcast(data)
-        data = data.transpose(..., term_dim)
+        if TERM_DIM not in data.dims:
+            raise ValueError("data must contain one dimension ending with '_term'")
+
+        if "const" not in data:
+            data = data.assign(const=0)
+
+        data = xr.broadcast(data, exclude=HELPER_DIMS)[0]
+        data[["coeffs", "vars"]] = xr.broadcast(
+            data[["coeffs", "vars"]], exclude=[FACTOR_DIM]
+        )[0]
+
+        # transpose with new Dataset to really ensure correct order
+        data = Dataset(data.transpose(..., TERM_DIM))
 
         if not isinstance(model, Model):
             raise ValueError("model must be an instance of linopy.Model")
 
         self._model = model
         self._data = data
 
-    def unravel_coords(self, index):
-        idx = np.unravel_index(index, self.shape[:-1])
-        coords = [
-            self.indexes[dim][idx[i]]
-            for i, dim in enumerate(self.vars.dims)
-            if not dim.startswith("_")
-        ]
-        return list(zip(*coords))
-
     def __repr__(self):
         """
-        Get the string representation of the expression.
+        Print the expression arrays.
         """
-        nexprs = self.size // self.nterm
-
-        # don't loop over all values if not necessary
-        if self.size == self.nterm:
-            expr_string = print_single_expression(
-                self.coeffs.values, self.vars.values, self.model
-            )
-            return f"LinearExpression:\n-----------------\n{expr_string}"
-
-        # create header string
-        nonterm_dims = [(k, v) for k, v in self.dims.items() if not k.startswith("_")]
-        shape_string = "(" + ", ".join([f"{k}: {v}" for k, v in nonterm_dims]) + ")"
-        header = f"LinearExpression {shape_string}:\n{'-' * (18 + len(shape_string))}"
-
-        # create data string, print only a few values
-        max_print = options["display_max_rows"]
-        split_at = max_print // 2
-        to_print = head_tail_range(nexprs, max_print)
-        truncate = nexprs > max_print
-        coords = self.unravel_coords(to_print)
-
-        if not self.size:
-            return f"{header}\nNone"
-
-        # loop over all values to print
-        coord_strings = []
-        expr_strings = []
-        trunc_strings = []
-        for i, coord in enumerate(coords):
-            coord_string = print_coord(coord) + ":"
-            expr_string = print_single_expression(
-                self.coeffs.loc[coord].values, self.vars.loc[coord].values, self.model
+        max_lines = options["display_max_rows"]
+        dims = list(self.coord_dims)
+        dim_sizes = list(self.coord_dims.values())
+        size = np.prod(dim_sizes)  # that the number of theoretical printouts
+        masked_entries = self.mask.sum().values if self.mask is not None else 0
+        lines = []
+
+        header_string = self.type
+
+        if size > 1:
+            for indices in generate_indices_for_printout(dim_sizes, max_lines):
+                if indices is None:
+                    lines.append("\t\t...")
+                else:
+                    coord_values = ", ".join(
+                        str(self.data[dims[i]].values[ind])
+                        for i, ind in enumerate(indices)
+                    )
+                    if self.mask is None or self.mask.values[indices]:
+                        expr = print_single_expression(
+                            self.coeffs.values[indices],
+                            self.vars.values[indices],
+                            self.const.values[indices],
+                            self.model,
+                        )
+                        line = f"[{coord_values}]: {expr}"
+                    else:
+                        line = f"[{coord_values}]: None"
+                    lines.append(line)
+
+            shape_str = ", ".join(f"{d}: {s}" for d, s in zip(dims, dim_sizes))
+            mask_str = f" - {masked_entries} masked entries" if masked_entries else ""
+            underscore = "-" * (len(shape_str) + len(mask_str) + len(header_string) + 4)
+            lines.insert(0, f"{header_string} ({shape_str}){mask_str}:\n{underscore}")
+        elif size == 1:
+            expr = print_single_expression(
+                self.coeffs, self.vars, self.const, self.model
             )
-            trunc_string = "\n\t\t..." if i == split_at - 1 and truncate else ""
-
-            coord_strings.append(coord_string)
-            expr_strings.append(expr_string)
-            trunc_strings.append(trunc_string)
-
-        coord_width = max(len(c) for c in coord_strings)
-
-        data_string = ""
-        for c, e, t in zip(coord_strings, expr_strings, trunc_strings):
-            data_string += f"\n{c:<{coord_width}} {e}{t}"
+            lines.append(f"{header_string}\n{'-'*len(header_string)}\n{expr}")
+        else:
+            lines.append(f"{header_string}\n{'-'*len(header_string)}\n<empty>")
 
-        return f"{header}{data_string}"
+        return "\n".join(lines)
 
     def __add__(self, other):
         """
         Add an expression to others.
         """
-        if not isinstance(other, (LinearExpression, variables.Variable)):
-            raise TypeError(
-                "unsupported operand type(s) for +: " f"{type(self)} and {type(other)}"
-            )
-        if isinstance(other, variables.Variable):
-            other = LinearExpression.from_tuples((1, other))
-        return merge(self, other)
+        other = as_expression(
+            other, model=self.model, coords=self.coords, dims=self.coord_dims
+        )
+        return merge(self, other, cls=self.__class__)
 
     def __radd__(self, other):
         # This is needed for using python's sum function
-        if other == 0:
-            return self
-        else:
-            return NotImplemented
+        return self if other == 0 else NotImplemented
 
     def __sub__(self, other):
         """
         Subtract others from expression.
         """
-        if not isinstance(other, (LinearExpression, variables.Variable)):
-            raise TypeError(
-                "unsupported operand type(s) for +: " f"{type(self)} and {type(other)}"
-            )
-        return merge(self, -other)
+        other = as_expression(
+            other, model=self.model, coords=self.coords, dims=self.coord_dims
+        )
+        return merge(self, -other, cls=self.__class__)
 
     def __neg__(self):
         """
         Get the negative of the expression.
         """
-        return self.assign(coeffs=-self.coeffs)
+        return self.assign(coeffs=-self.coeffs, const=-self.const)
 
     def __mul__(self, other):
         """
         Multiply the expr by a factor.
         """
-        if isinstance(other, (LinearExpression, variables.Variable)):
+        if isinstance(other, QuadraticExpression):
             raise TypeError(
                 "unsupported operand type(s) for *: "
                 f"{type(self)} and {type(other)}. "
-                "Non-linear expressions are not yet supported."
+                "Higher order non-linear expressions are not yet supported."
+            )
+        elif isinstance(other, (variables.Variable, variables.ScalarVariable)):
+            other = other.to_linexpr()
+
+        if type(other) is LinearExpression:
+            if other.nterm > 1:
+                raise TypeError("Multiplication of multiple terms is not supported.")
+            ds = other.data[["coeffs", "vars"]].sel(_term=0).broadcast_like(self.data)
+            ds = ds.assign(const=other.const)
+            return merge(self, ds, dim=FACTOR_DIM, cls=QuadraticExpression)
+        else:
+            coeffs = self.coeffs * as_dataarray(
+                other, coords=self.coords, dims=self.coord_dims
             )
-        if isinstance(other, (pd.Series, pd.DataFrame)):
-            other = xr.DataArray(other)
-        coeffs = self.coeffs * other
-        assert set(coeffs.shape) == set(self.coeffs.shape)
-        return self.assign(coeffs=coeffs)
+            assert set(coeffs.shape) == set(self.coeffs.shape)
+            return self.assign(coeffs=coeffs)
 
     def __rmul__(self, other):
         """
         Right-multiply the expr by a factor.
         """
         return self.__mul__(other)
 
     def __div__(self, other):
-        if isinstance(other, (LinearExpression, variables.Variable)):
+        if isinstance(
+            other, (LinearExpression, variables.Variable, variables.ScalarVariable)
+        ):
             raise TypeError(
                 "unsupported operand type(s) for /: "
                 f"{type(self)} and {type(other)}"
                 "Non-linear expressions are not yet supported."
             )
         return self.__mul__(1 / other)
 
     def __truediv__(self, other):
         return self.__div__(other)
 
     def __le__(self, rhs):
-        return constraints.AnonymousConstraint(self, LESS_EQUAL, rhs)
+        return self.to_constraint(LESS_EQUAL, rhs)
 
     def __ge__(self, rhs):
-        return constraints.AnonymousConstraint(self, GREATER_EQUAL, rhs)
+        return self.to_constraint(GREATER_EQUAL, rhs)
 
     def __eq__(self, rhs):
-        return constraints.AnonymousConstraint(self, EQUAL, rhs)
+        return self.to_constraint(EQUAL, rhs)
 
     def __gt__(self, other):
         raise NotImplementedError(
             "Inequalities only ever defined for >= rather than >."
         )
 
     def __lt__(self, other):
         raise NotImplementedError(
             "Inequalities only ever defined for >= rather than >."
         )
 
-    @deprecated(details="Use the `data` property instead of `to_dataset`")
-    def to_dataset(self):
-        """
-        Convert the expression to a xarray.Dataset.
-        """
-        return self.data
+    @property
+    def loc(self):
+        return LocIndexer(self)
 
     @classmethod
     @property
     def fill_value(cls):
         return cls._fill_value
 
     @property
+    def type(self):
+        return "LinearExpression"
+
+    @property
     def data(self):
         return self._data
 
     @property
     def model(self):
         return self._model
 
     @property
     def dims(self):
         # do explicitly sort as in vars (same as in coeffs)
         return {k: self.data.dims[k] for k in self.vars.dims}
 
+    @deprecated(details="Use `coord_dims` instead")
     @property
     def non_helper_dims(self):
         return {k: self.data.dims[k] for k in self.dims if not k.startswith("_")}
 
     @property
+    def coord_dims(self):
+        return {k: self.data.dims[k] for k in self.dims if k not in HELPER_DIMS}
+
+    @property
     def vars(self):
         return self.data.vars
 
     @vars.setter
     def vars(self, value):
         self.data["vars"] = value
 
@@ -381,31 +505,45 @@
     def coeffs(self):
         return self.data.coeffs
 
     @coeffs.setter
     def coeffs(self, value):
         self.data["coeffs"] = value
 
+    @property
+    def const(self):
+        return self.data.const
+
+    @const.setter
+    def const(self, value):
+        self.data["const"] = value
+
+    # create a dummy for a mask, which can be implemented later
+    @property
+    def mask(self):
+        return None
+
     @classmethod
     def _sum(cls, expr: Union["LinearExpression", Dataset], dims=None) -> Dataset:
         data = _expr_unwrap(expr)
 
         if dims is None:
-            vars = DataArray(data.vars.data.ravel(), dims="_term")
-            coeffs = DataArray(data.coeffs.data.ravel(), dims="_term")
-            ds = xr.Dataset({"vars": vars, "coeffs": coeffs})
-
+            vars = DataArray(data.vars.data.ravel(), dims=TERM_DIM)
+            coeffs = DataArray(data.coeffs.data.ravel(), dims=TERM_DIM)
+            const = data.const.sum()
+            ds = xr.Dataset({"vars": vars, "coeffs": coeffs, "const": const})
         else:
-            dims = [d for d in np.atleast_1d(dims) if d != "_term"]
+            dims = [d for d in np.atleast_1d(dims) if d != TERM_DIM]
             ds = (
-                data.reset_index(dims, drop=True)
-                .rename(_term="_stacked_term")
-                .stack(_term=["_stacked_term"] + dims)
-                .reset_index("_term", drop=True)
+                data[["coeffs", "vars"]]
+                .reset_index(dims, drop=True)
+                .rename({TERM_DIM: STACKED_TERM_DIM})
+                .stack({TERM_DIM: [STACKED_TERM_DIM] + dims}, create_index=False)
             )
+            ds["const"] = data.const.sum(dims)
 
         return ds
 
     def sum(self, dims=None, drop_zeros=False) -> "LinearExpression":
         """
         Sum the expression over all or a subset of dimensions.
 
@@ -426,15 +564,15 @@
 
         if drop_zeros:
             res = res.densify_terms()
 
         return res
 
     @classmethod
-    def from_tuples(cls, *tuples, chunk=None):
+    def from_tuples(cls, *tuples, model=None, chunk=None):
         """
         Create a linear expression by using tuples of coefficients and
         variables.
 
         The function internally checks that all variables in the tuples belong to the same
         reference model.
 
@@ -463,56 +601,36 @@
         >>> m = Model()
         >>> x = m.add_variables(pd.Series([0, 0]), 1)
         >>> y = m.add_variables(4, pd.Series([8, 10]))
         >>> expr = LinearExpression.from_tuples((10, x), (1, y))
 
         This is the same as calling ``10*x + y`` but a bit more performant.
         """
-        # when assigning arrays to Datasets it is taken as coordinates
-        # support numpy arrays and convert them to dataarrays
         exprs = []
-        model = None
-        for c, v in tuples:
-            if not isinstance(v, variables.Variable):
-                raise TypeError(f"Expected type `linopy.Variable`, got {type(v)}")
-            # check that reference models are consistent
-            if model is None:
-                model = v.model
-            # TODO: Ensure equality of models
-            # else:
-            # assert model == model
-
-            if isinstance(v, variables.ScalarVariable):
-                v = v.label
-            elif isinstance(v, variables.Variable):
-                v = v.labels
-            v = as_dataarray(v)
-
-            if isinstance(c, np.ndarray) or _pd_series_wo_index_name(c):
-                c = DataArray(c, v.coords)
-            elif _pd_dataframe_wo_axes_names(c):
-                if v.ndim == 1:
-                    c = DataArray(c, v.coords, dims=("dim_0", v.dims[0]))
-                else:
-                    c = DataArray(c, v.coords)
+        for t in tuples:
+            if len(t) == 2:
+                # assume first element is coefficient and second is variable
+                c, v = t
+                if not isinstance(v, (variables.Variable, variables.ScalarVariable)):
+                    raise TypeError("Expected variable as second element of tuple.")
+                expr = v.to_linexpr(c)
+                const = None
+                if model is None:
+                    model = expr.model  # TODO: Ensure equality of models
+            elif len(t) == 1:
+                # assume that the element is a constant
+                c, v = None, None
+                (const,) = as_dataarray(t)
+                expr = LinearExpression(const, model)
             else:
-                c = as_dataarray(c)
-                # if a dimension is not in the coords, add it as a range index
-                for i, dim in enumerate(c.dims):
-                    if dim not in c.coords:
-                        c = c.assign_coords(**{dim: pd.RangeIndex(c.shape[i])})
+                raise ValueError("Expected tuples of length 1 or 2.")
 
-            ds = Dataset({"coeffs": c, "vars": v}).expand_dims("_term")
-            expr = cls(ds, model)
             exprs.append(expr)
 
-        if len(exprs) > 1:
-            return merge(exprs, cls=cls)
-        else:
-            return exprs[0]
+        return merge(exprs, cls=cls) if len(exprs) > 1 else exprs[0]
 
     @classmethod
     def from_rule(cls, model, rule, coords):
         """
         Create a linear expression from a rule and a set of coordinates.
 
         This functionality mirrors the assignment of linear expression as done by
@@ -568,32 +686,68 @@
 
         combinations = product(*[c.values for c in coords.values()])
         exprs = []
         placeholder = ScalarLinearExpression((np.nan,), (-1,), model)
         exprs = [rule(model, *coord) or placeholder for coord in combinations]
         return cls._from_scalarexpression_list(exprs, coords, model)
 
-    def _from_scalarexpression_list(exprs, coords: DataArrayCoordinates, model):
+    @classmethod
+    def _from_scalarexpression_list(cls, exprs, coords: DataArrayCoordinates, model):
         """
         Create a LinearExpression from a list of lists with different lengths.
         """
         shape = list(map(len, coords.values()))
 
         coeffs = array(tuple(zip_longest(*(e.coeffs for e in exprs), fillvalue=nan)))
         vars = array(tuple(zip_longest(*(e.vars for e in exprs), fillvalue=-1)))
 
         nterm = vars.shape[0]
         coeffs = coeffs.reshape((nterm, *shape))
         vars = vars.reshape((nterm, *shape))
 
-        coeffs = DataArray(coeffs, coords, dims=("_term", *coords))
-        vars = DataArray(vars, coords, dims=("_term", *coords))
-        ds = Dataset({"coeffs": coeffs, "vars": vars}).transpose(..., "_term")
+        coeffs = DataArray(coeffs, coords, dims=(TERM_DIM, *coords))
+        vars = DataArray(vars, coords, dims=(TERM_DIM, *coords))
+        ds = Dataset({"coeffs": coeffs, "vars": vars}).transpose(..., TERM_DIM)
+
+        return cls(ds, model)
+
+    def to_quadexpr(self):
+        """Convert LinearExpression to QuadraticExpression."""
+        vars = self.data.vars.expand_dims(FACTOR_DIM)
+        fill_value = self.fill_value["vars"]
+        vars = xr.concat([vars, xr.full_like(vars, fill_value)], dim=FACTOR_DIM)
+        data = self.data.assign(vars=vars)
+        return QuadraticExpression(data, self.model)
+
+    def to_constraint(self, sign, rhs):
+        """
+        Convert a linear expression to a constraint.
+
+        Parameters
+        ----------
+        sign : str, array-like
+            Sign(s) of the constraints.
+        rhs : constant, Variable, LinearExpression
+            Right-hand side of the constraint.
+
+        Returns
+        -------
+        Constraint with strict separation of the linear expressions of variables
+        which are moved to the left-hand-side and constant values which are moved
+        to the right-hand side.
+        """
+        all_to_lhs = (self - rhs).data
+        data = all_to_lhs[["coeffs", "vars"]].assign(sign=sign, rhs=-all_to_lhs.const)
+        return constraints.Constraint(data, model=self.model)
 
-        return LinearExpression(ds, model)
+    def reset_const(self):
+        """
+        Reset the constant of the linear expression to zero.
+        """
+        return self.__class__(self.data[["coeffs", "vars"]], self.model)
 
     def where(self, cond, other=xr.core.dtypes.NA, **kwargs):
         """
         Filter variables based on a condition.
 
         This operation call ``xarray.Dataset.where`` but sets the default
         fill value to -1 for variables and ensures preserving the linopy.LinearExpression type.
@@ -636,18 +790,15 @@
         Returns
         -------
         linopy.LinearExpression
         """
         return self - self.shift({dim: n})
 
     def groupby(
-        self,
-        group,
-        squeeze: "bool" = True,
-        restore_coord_dims: "bool" = None,
+        self, group, squeeze: "bool" = True, restore_coord_dims: "bool" = None, **kwargs
     ) -> LinearExpressionGroupby:
         """
         Returns a LinearExpressionGroupBy object for performing grouped
         operations.
 
         Docstring and arguments are borrowed from `xarray.Dataset.groupby`
 
@@ -667,47 +818,16 @@
         Returns
         -------
         grouped
             A `LinearExpressionGroupBy` containing the xarray groups and ensuring
             the correct return type.
         """
         ds = self.data
-        groups = ds.groupby(
-            group=group, squeeze=squeeze, restore_coord_dims=restore_coord_dims
-        )
-        return LinearExpressionGroupby(groups, model=self.model)
-
-    @deprecated("0.1.0", "0.1.2", details="Use groupby (followed by sum) instead.")
-    def groupby_sum(self, group):
-        """
-        Sum expression over groups.
-
-        The function works in the same manner as the xarray.Dataset.groupby
-        function, but automatically sums over all terms.
-
-        Parameters
-        ----------
-        group : DataArray or IndexVariable
-            Array whose unique values should be used to group the expressions.
-
-        Returns
-        -------
-        Grouped linear expression.
-        """
-        if isinstance(group, pd.Series):
-            logger.info("Converting group pandas.Series to xarray.DataArray")
-            group = group.to_xarray()
-        groups = xr.Dataset.groupby(self.data, group)
-
-        def func(ds):
-            ds = self._sum(ds, groups._group_dim)
-            ds = ds.assign_coords(_term=np.arange(len(ds._term)))
-            return ds
-
-        return self.__class__(groups.map(func), self.model)  # .reset_index('_term')
+        kwargs = dict(squeeze=squeeze, restore_coord_dims=restore_coord_dims, **kwargs)
+        return LinearExpressionGroupby(ds, group, model=self.model, kwargs=kwargs)
 
     def rolling(
         self,
         dim: "Mapping[Any, int]" = None,
         min_periods: "int" = None,
         center: "bool | Mapping[Any, bool]" = False,
         **window_kwargs: "int",
@@ -738,46 +858,14 @@
         """
         ds = self.data
         rolling = ds.rolling(
             dim=dim, min_periods=min_periods, center=center, **window_kwargs
         )
         return LinearExpressionRolling(rolling, model=self.model)
 
-    @deprecated("0.1.0", "0.1.2", details="Use rolling (followed by sum) instead.")
-    def rolling_sum(self, **kwargs):
-        """
-        Rolling sum of the linear expression.
-
-        Parameters
-        ----------
-        **kwargs :
-            Keyword arguments passed to ``xarray.Dataset.rolling``.
-
-        Returns
-        -------
-        linopy.LinearExpression
-        """
-        coeffs = xr.DataArray.rolling(self.coeffs, **kwargs).construct(
-            "_rolling_term", keep_attrs=True
-        )
-
-        vars = xr.DataArray.rolling(self.vars, **kwargs).construct(
-            "_rolling_term",
-            fill_value=self._fill_value["vars"],
-            keep_attrs=True,
-        )
-
-        ds = xr.Dataset({"coeffs": coeffs, "vars": vars})
-        ds = (
-            ds.rename(_term="_stacked_term")
-            .stack(_term=["_stacked_term", "_rolling_term"])
-            .reset_index("_term", drop=True)
-        )
-        return self.__class__(ds, self.model).assign_attrs(self.attrs)
-
     @property
     def nterm(self):
         """
         Get the number of terms in the linear expression.
         """
         return len(self.data._term)
 
@@ -790,29 +878,28 @@
         return self.vars.shape
 
     @property
     def size(self):
         """
         Get the total size of the linear expression.
         """
-        assert self.vars.size == self.coeffs.size
         return self.vars.size
 
     def empty(self):
         """
         Get whether the linear expression is empty.
         """
         return self.shape == (0,)
 
     def densify_terms(self):
         """
         Move all non-zero term entries to the front and cut off all-zero
         entries in the term-axis.
         """
-        data = self.data.transpose(..., "_term")
+        data = self.data.transpose(..., TERM_DIM)
 
         cdata = data.coeffs.data
         axis = cdata.ndim - 1
         nnz = np.nonzero(cdata)
         nterm = (cdata != 0).sum(axis).max()
 
         mod_nnz = list(nnz)
@@ -828,15 +915,15 @@
         vdata[tuple(mod_nnz)] = data.vars.data[nnz]
         data.vars.data = vdata
 
         cdata = np.zeros_like(cdata)
         cdata[tuple(mod_nnz)] = data.coeffs.data[nnz]
         data.coeffs.data = cdata
 
-        return self.__class__(data.sel(_term=slice(0, nterm)), self.model)
+        return self.__class__(data.sel({TERM_DIM: slice(0, nterm)}), self.model)
 
     def sanitize(self):
         """
         Sanitize LinearExpression by ensuring int dtype for variables.
 
         Returns
         -------
@@ -849,14 +936,49 @@
 
     def equals(self, other: "LinearExpression"):
         return self.data.equals(_expr_unwrap(other))
 
     def __iter__(self):
         return self.data.__iter__()
 
+    @property
+    def flat(self) -> pd.DataFrame:
+        """
+        Convert the expression to a pandas DataFrame.
+
+        The resulting DataFrame represents a long table format of the all
+        expressions with non-zero coefficients. It contains the
+        columns `coeffs` and `vars`.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+        """
+        ds = self.data
+        if not ds.sizes:
+            # fallback for weird error raised due to missing index
+            df = pd.DataFrame({k: ds[k].item() for k in ds}, index=[0])
+        else:
+            df = ds.to_dataframe()
+        if "mask" in df:
+            mask = df.pop("mask")
+            df = df[mask]
+        df = df[(df.vars != -1) & (df.coeffs != 0)]
+        # Group repeated variables in the same constraint
+        df = df.groupby("vars", as_index=False).sum()
+
+        any_nan = df.isna().any()
+        if any_nan.any():
+            fields = ", ".join("`" + df.columns[any_nan] + "`")
+            raise ValueError(
+                f"Expression `{self.name}` contains nan's in field(s) {fields}"
+            )
+
+        return df
+
     # Wrapped function which would convert variable to dataarray
     assign = exprwrap(Dataset.assign)
 
     assign_attrs = exprwrap(Dataset.assign_attrs)
 
     assign_coords = exprwrap(Dataset.assign_coords)
 
@@ -891,42 +1013,219 @@
     rename = exprwrap(Dataset.rename)
 
     rename_dims = exprwrap(Dataset.rename_dims)
 
     roll = exprwrap(Dataset.roll)
 
 
-def _pd_series_wo_index_name(ds):
-    if isinstance(ds, pd.Series):
-        if ds.index.name is None:
-            return True
-    return False
-
-
-def _pd_dataframe_wo_axes_names(df):
-    if isinstance(df, pd.DataFrame):
-        if df.index.name is None and df.columns.name is None:
-            return True
-        elif df.index.name is None or df.columns.name is None:
-            logger.warning(
-                "Pandas DataFrame has only one labeled axis. "
-                "This might lead to unexpected dimension alignment "
-                "of the resulting expression."
+@forward_as_properties(data=["attrs", "coords", "indexes", "sizes"])
+class QuadraticExpression(LinearExpression):
+    """
+    A quadratic expression consisting of terms of coefficients and variables.
+
+    The QuadraticExpression class is a subclass of LinearExpression which allows to
+    apply most xarray functions on it.
+    """
+
+    __slots__ = ("_data", "_model")
+    __array_ufunc__ = None
+    __array_priority__ = 10000
+
+    _fill_value = {"vars": -1, "coeffs": np.nan, "const": 0}
+
+    def __init__(self, data, model):
+        super().__init__(data, model)
+
+        if FACTOR_DIM not in data.vars.dims:
+            raise ValueError(f"Data does not include dimension {FACTOR_DIM}")
+        elif data.sizes[FACTOR_DIM] != 2:
+            raise ValueError(f"Size of dimension {FACTOR_DIM} must be 2.")
+
+        # transpose data to have _term as last dimension and _factor as second last
+        data = xr.Dataset(data.transpose(..., FACTOR_DIM, TERM_DIM))
+        self._data = data
+
+    def __mul__(self, other):
+        """
+        Multiply the expr by a factor.
+        """
+        if isinstance(
+            other,
+            (
+                LinearExpression,
+                QuadraticExpression,
+                variables.Variable,
+                variables.ScalarVariable,
+            ),
+        ):
+            raise TypeError(
+                "unsupported operand type(s) for *: "
+                f"{type(self)} and {type(other)}. "
+                "Higher order non-linear expressions are not yet supported."
             )
-            return False
-    return False
+        return super().__mul__(other)
+
+    @property
+    def type(self):
+        return "QuadraticExpression"
 
+    def __add__(self, other):
+        """
+        Add an expression to others.
+        """
+        other = as_expression(
+            other, model=self.model, coords=self.coords, dims=self.coord_dims
+        )
+        if type(other) is LinearExpression:
+            other = other.to_quadexpr()
+        return merge(self, other, cls=self.__class__)
 
-def merge(*exprs, dim="_term", cls=LinearExpression, **kwargs):
+    def __radd__(self, other):
+        """
+        Add others to expression.
+        """
+        if type(other) is LinearExpression:
+            other = other.to_quadexpr()
+            return other.__add__(self)
+        elif other == 0:
+            return self
+        else:
+            return NotImplemented
+
+    def __sub__(self, other):
+        """
+        Subtract others from expression.
+        """
+        other = as_expression(
+            other, model=self.model, coords=self.coords, dims=self.coord_dims
+        )
+        if type(other) is LinearExpression:
+            other = other.to_quadexpr()
+        return merge(self, -other, cls=self.__class__)
+
+    def __rsub__(self, other):
+        """
+        Subtract expression from others.
+        """
+        if type(other) is LinearExpression:
+            other = other.to_quadexpr()
+            return other.__sub__(self)
+        else:
+            NotImplemented
+
+    @classmethod
+    def _sum(cls, expr: "QuadraticExpression", dims=None) -> Dataset:
+        data = _expr_unwrap(expr)
+        dims = dims or list(set(data.dims) - set(HELPER_DIMS))
+        return LinearExpression._sum(expr, dims)
+
+    def to_constraint(self, sign, rhs):
+        raise NotImplementedError(
+            "Quadratic expressions cannot be used in constraints."
+        )
+
+    @property
+    def flat(self):
+        """
+        Return a flattened expression.
+        """
+        vars = self.data.vars.assign_coords(
+            {FACTOR_DIM: ["vars1", "vars2"]}
+        ).to_dataset(FACTOR_DIM)
+        ds = self.data.drop_vars("vars").assign(vars)
+        if not ds.sizes:
+            # fallback for weird error raised due to missing index
+            df = pd.DataFrame({k: ds[k].item() for k in ds}, index=[0])
+        else:
+            df = ds.to_dataframe()
+        if "mask" in df:
+            mask = df.pop("mask")
+            df = df[mask]
+        df = df[((df.vars1 != -1) | (df.vars2 != -1)) & (df.coeffs != 0)]
+        # Group repeated variables in the same constraint
+        df = df.groupby(["vars1", "vars2"], as_index=False).sum()
+
+        any_nan = df.isna().any()
+        if any_nan.any():
+            fields = ", ".join("`" + df.columns[any_nan] + "`")
+            raise ValueError(
+                f"Expression `{self.name}` contains nan's in field(s) {fields}"
+            )
+
+        return df
+
+    def to_matrix(self):
+        """
+        Return a sparse matrix representation of the expression only including
+        quadratic terms.
+
+        Note that the matrix is formulated following the convention of the
+        optimization problem, i.e. the quadratic term is 0.5 x^T Q x.
+        The matrix Q is therefore symmetric and the diagonal terms are doubled.
+
+        """
+        df = self.flat
+        # drop linear terms
+        df = df[(df.vars1 != -1) & (df.vars2 != -1)]
+
+        # symmetrize cross terms and double diagonal terms
+        cross_terms = df.vars1 != df.vars2
+        df.loc[~cross_terms, "coeffs"] *= 2
+        vals = dict(vars1=df.vars2[cross_terms], vars2=df.vars1[cross_terms])
+        df = pd.concat([df, df[cross_terms].assign(**vals)])
+
+        # assign matrix
+        data = df.coeffs
+        row = df.vars1
+        col = df.vars2
+        nvars = self.model.shape[1]
+        return csc_matrix((data, (row, col)), shape=(nvars, nvars))
+
+
+def as_expression(obj, model=None, **kwargs):
+    """
+    Convert an object to a LinearExpression or QuadraticExpression.
+
+    Parameters
+    ----------
+    obj : Variable, ScalarVariable, LinearExpression, array_like
+        Object to convert to LinearExpression.
+    model : linopy.Model, optional
+        Assigned model, by default None
+    **kwargs :
+        Keyword arguments passed to `linopy.as_dataarray`.
+
+    Returns
+    -------
+    expr : LinearExpression
+
+    Raises
+    ------
+    ValueError
+        If object cannot be converted to LinearExpression.
+    """
+    if isinstance(obj, LinearExpression):
+        return obj
+    elif isinstance(obj, (variables.Variable, variables.ScalarVariable)):
+        return obj.to_linexpr()
+    else:
+        try:
+            obj = as_dataarray(obj, **kwargs)
+        except ValueError as e:
+            raise ValueError("Cannot convert to LinearExpression") from e
+        return LinearExpression(obj, model)
+
+
+def merge(*exprs, dim=TERM_DIM, cls=LinearExpression, **kwargs):
     """
-    Merge multiple linear expression together.
+    Merge multiple expression together.
 
     This function is a bit faster than summing over multiple linear expressions.
     In case a list of LinearExpression with exactly the same shape is passed
-    and the dimension to concatenate on is "_term", the concatenation uses
+    and the dimension to concatenate on is TERM_DIM, the concatenation uses
     the coordinates of the first object as a basis which overrides the
     coordinates of the consecutive objects.
 
 
     Parameters
     ----------
     *exprs : tuple/list
@@ -940,46 +1239,56 @@
         {coords: "minimal", compat: "override"} or, in the special case described
         above, to {coords: "minimal", compat: "override", "join": "override"}.
 
     Returns
     -------
     res : linopy.LinearExpression
     """
-    if len(exprs) == 1:
-        exprs = exprs[0]  # assume a list of mergeable objects is given
-    else:
-        exprs = list(exprs)
-
-    override = False
-    if cls == LinearExpression and dim == "_term":
-        override = all(e.non_helper_dims == exprs[0].non_helper_dims for e in exprs)
+    linopy_types = (variables.Variable, LinearExpression, QuadraticExpression)
 
+    exprs = exprs[0] if len(exprs) == 1 else list(exprs)  # allow passing a list
     model = exprs[0].model
-    ds_list = [e.data if isinstance(e, cls) else e for e in exprs]
 
-    if cls == LinearExpression:
-        if not all(len(ds._term) == len(ds_list[0]._term) for ds in ds_list[1:]):
-            ds_list = [
-                ds.assign_coords(_term=np.arange(len(ds._term))) for ds in ds_list
-            ]
+    if cls in linopy_types and dim in HELPER_DIMS:
+        coord_dims = [
+            {k: v for k, v in e.dims.items() if k not in HELPER_DIMS} for e in exprs
+        ]
+        override = check_common_keys_values(coord_dims)
+    else:
+        override = False
+
+    data = [e.data if isinstance(e, linopy_types) else e for e in exprs]
+    for d in set(HELPER_DIMS) & set(_ for ds in data for _ in ds.dims):
+        if len({ds.dims[d] for ds in data}) > 1:
+            data = [ds.assign_coords({d: arange(ds.dims[d])}) for ds in data]
 
     if not kwargs:
-        kwargs = dict(fill_value=cls._fill_value, coords="minimal", compat="override")
+        kwargs = {
+            "fill_value": cls._fill_value,
+            "coords": "minimal",
+            "compat": "override",
+        }
         if override:
-            kwargs.update(dict(join="override"))
-
-    ds = xr.concat(ds_list, dim, **kwargs)
+            kwargs["join"] = "override"
 
-    if "_term" in ds.coords:
-        ds = ds.reset_index("_term", drop=True)
+    if dim == TERM_DIM:
+        ds = xr.concat([d[["coeffs", "vars"]] for d in data], dim, **kwargs)
+        const = xr.concat([d["const"] for d in data], dim, **kwargs).sum(TERM_DIM)
+        ds["const"] = const
+    elif dim == FACTOR_DIM:
+        ds = xr.concat([d[["vars"]] for d in data], dim, **kwargs)
+        coeffs = xr.concat([d["coeffs"] for d in data], dim, **kwargs).prod(FACTOR_DIM)
+        ds["coeffs"] = coeffs
+        const = xr.concat([d["const"] for d in data], dim, **kwargs).prod(FACTOR_DIM)
+        ds["const"] = const
+    else:
+        ds = xr.concat(data, dim, **kwargs)
 
-    # ensure that coordinates for non-helper dims are explicit
-    if isinstance(dim, str):
-        if dim not in ds.coords and not dim.startswith("_"):
-            ds = ds.assign_coords({dim: pd.RangeIndex(ds.dims[dim])})
+    for d in set(HELPER_DIMS) & set(ds.coords):
+        ds = ds.reset_index(d, drop=True)
 
     return cls(ds, model)
 
 
 class ScalarLinearExpression:
     """
     A scalar linear expression container.
@@ -993,15 +1302,15 @@
 
     def __init__(self, coeffs, vars, model):
         self._coeffs = coeffs
         self._vars = vars
         self._model = model
 
     def __repr__(self) -> str:
-        expr_string = print_single_expression(self.coeffs, self.vars, self.model)
+        expr_string = print_single_expression(self.coeffs, self.vars, 0, self.model)
         return f"ScalarLinearExpression: {expr_string}"
 
     @property
     def coeffs(self):
         return self._coeffs
 
     @property
@@ -1051,54 +1360,54 @@
 
     def __neg__(self):
         return ScalarLinearExpression(
             tuple(-c for c in self.coeffs), self.vars, self.model
         )
 
     def __mul__(self, other):
-        if not isinstance(other, (int, np.integer, float)):
+        if not isinstance(other, (int, float, np.number)):
             raise TypeError(
                 "unsupported operand type(s) for *: " f"{type(self)} and {type(other)}"
             )
 
         return ScalarLinearExpression(
             tuple(other * c for c in self.coeffs), self.vars, self.model
         )
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __div__(self, other):
-        if not isinstance(other, (int, np.integer, float)):
+        if not isinstance(other, (int, float, np.number)):
             raise TypeError(
                 "unsupported operand type(s) for /: " f"{type(self)} and {type(other)}"
             )
         return self.__mul__(1 / other)
 
     def __truediv__(self, other):
         return self.__div__(other)
 
     def __le__(self, other):
-        if not isinstance(other, (int, np.integer, float)):
+        if not isinstance(other, (int, float, np.number)):
             raise TypeError(
                 "unsupported operand type(s) for <=: " f"{type(self)} and {type(other)}"
             )
 
         return constraints.AnonymousScalarConstraint(self, LESS_EQUAL, other)
 
     def __ge__(self, other):
-        if not isinstance(other, (int, np.integer, float)):
+        if not isinstance(other, (int, float, np.number)):
             raise TypeError(
                 "unsupported operand type(s) for >=: " f"{type(self)} and {type(other)}"
             )
 
         return constraints.AnonymousScalarConstraint(self, GREATER_EQUAL, other)
 
     def __eq__(self, other):
-        if not isinstance(other, (int, np.integer, float)):
+        if not isinstance(other, (int, float, np.number)):
             raise TypeError(
                 "unsupported operand type(s) for ==: " f"{type(self)} and {type(other)}"
             )
 
         return constraints.AnonymousScalarConstraint(self, EQUAL, other)
 
     def __gt__(self, other):
@@ -1108,11 +1417,11 @@
 
     def __lt__(self, other):
         raise NotImplementedError(
             "Inequalities only ever defined for >= rather than >."
         )
 
     def to_linexpr(self):
-        coeffs = xr.DataArray(list(self.coeffs), dims="_term")
-        vars = xr.DataArray(list(self.vars), dims="_term")
+        coeffs = xr.DataArray(list(self.coeffs), dims=TERM_DIM)
+        vars = xr.DataArray(list(self.vars), dims=TERM_DIM)
         ds = xr.Dataset({"coeffs": coeffs, "vars": vars})
         return LinearExpression(ds, self.model)
```

### Comparing `linopy-0.1.5/linopy/io.py` & `linopy-0.2/linopy/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,227 +9,312 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numpy import asarray, concatenate, ones_like, zeros_like
+from scipy.sparse import csc_matrix, triu
 from tqdm import tqdm
 
 from linopy import solvers
-from linopy.constants import EQUAL, GREATER_EQUAL
+from linopy.constants import CONCAT_DIM, EQUAL, GREATER_EQUAL
 
 logger = logging.getLogger(__name__)
 
 
 ufunc_kwargs = dict(vectorize=True)
-concat_dim = "_concat_dim"
-concat_kwargs = dict(dim=concat_dim, coords="minimal")
+concat_kwargs = dict(dim=CONCAT_DIM, coords="minimal")
 
+TQDM_COLOR = "#80bfff"
 
-# IO functions
-def int_to_str(arr):
+
+def handle_batch(batch, f, batch_size):
     """
-    Convert numpy array to str typed array.
+    Write out a batch to a file and reset the batch.
     """
-    convert = np.frompyfunc(lambda i: "%i" % i, 1, 1)
-    return convert(arr)
+    if len(batch) >= batch_size:
+        f.writelines(batch)  # write out a batch
+        batch = []  # reset batch
+    return batch
 
 
-def float_to_str(arr, ensure_sign=True):
+def objective_write_linear_terms(df, f, batch, batch_size):
     """
-    Convert numpy array to str typed array.
+    Write the linear terms of the objective to a file.
     """
-    if ensure_sign:
-        convert = np.frompyfunc(lambda f: "%+.12g" % f, 1, 1)
-    else:
-        convert = np.frompyfunc(lambda f: "%.12g" % f, 1, 1)
-    return convert(arr)
+    coeffs = df.coeffs.values
+    vars = df.vars.values
+    for idx in range(len(coeffs)):
+        coeff = coeffs[idx]
+        var = vars[idx]
+        batch.append(f"{coeff:+.12g} x{var}\n")
+        batch = handle_batch(batch, f, batch_size)
+    return batch
 
 
-def fill_by(target_shape, where, fill, other=""):
+def objective_write_cross_terms(quadratic, f, batch, batch_size):
     """
-    Create array of `target_shape` with values from `fill` where `where` is
-    True.
+    Write the cross terms of the objective to a file.
     """
-    res = np.full(target_shape, other).astype(object)
-    res[where] = fill
-    return res
+    is_cross = quadratic.vars1 != quadratic.vars2
+    cross = quadratic[is_cross]
+    coeffs = cross.coeffs.values
+    vars1 = cross.vars1.values
+    vars2 = cross.vars2.values
+    for idx in range(len(coeffs)):
+        coeff = coeffs[idx]
+        var1 = vars1[idx]
+        var2 = vars2[idx]
+        batch.append(f"{coeff:+.12g} x{var1} * x{var2}\n")
+        batch = handle_batch(batch, f, batch_size)
+    return batch
 
 
-def objective_to_file(m, f, log=False):
+def objective_write_quad_terms(quadratic, f, batch, batch_size):
+    """
+    Write the quadratic terms of the objective to a file.
+    """
+    is_cross = quadratic.vars1 != quadratic.vars2
+    quad = quadratic[~is_cross]
+    coeffs = quad.coeffs.values
+    vars = quad.vars1.values
+    for idx in range(len(coeffs)):
+        coeff = coeffs[idx]
+        var = vars[idx]
+        batch.append(f"{coeff:+.12g} x{var} ^ 2\n")
+        batch = handle_batch(batch, f, batch_size)
+    return batch
+
+
+def objective_to_file(m, f, log=False, batch_size=10000):
     """
     Write out the objective of a model to a lp file.
     """
     if log:
         logger.info("Writing objective.")
 
     f.write("min\n\nobj:\n\n")
-    coeffs = m.objective.coeffs.values
-    vars = m.objective.vars.values
-    nnz = vars != -1
-    coeffs, vars = coeffs[nnz], vars[nnz]
+    df = m.objective.flat
 
-    if np.isnan(coeffs).any():
-        raise ValueError(
+    if np.isnan(df.coeffs).any():
+        logger.warning(
             "Objective coefficients are missing (nan) where variables are not (-1)."
         )
 
-    objective = float_to_str(coeffs) + " x" + int_to_str(vars)
-    f.write("\n".join(objective))
-    del objective
+    if m.is_linear:
+        batch = objective_write_linear_terms(df, f, [], batch_size)
 
+    elif m.is_quadratic:
+        is_linear = (df.vars1 == -1) | (df.vars2 == -1)
+        linear = df[is_linear]
+        linear = linear.assign(
+            vars=linear.vars1.where(linear.vars1 != -1, linear.vars2)
+        )
+        batch = objective_write_linear_terms(linear, f, [], batch_size)
 
-def constraints_to_file(m, f, log=False):
-    """
-    Write out the constraints of a model to a lp file.
-    """
-    f.write("\n\ns.t.\n\n")
-    m.constraints.sanitize_missings()
-    kwargs = dict(broadcast_like="vars", filter_missings=True)
-    vars = m.constraints.iter_ravel("vars", **kwargs)
-    coeffs = m.constraints.iter_ravel("coeffs", **kwargs)
-    labels = m.constraints.iter_ravel("labels", **kwargs)
-
-    labels_ = m.constraints.iter_ravel("labels", filter_missings=True)
-    sign_ = m.constraints.iter_ravel("sign", filter_missings=True)
-    rhs_ = m.constraints.iter_ravel("rhs", filter_missings=True)
+        if not is_linear.all():
+            batch.append("+ [\n")
+            quadratic = df[~is_linear]
+            quadratic = quadratic.assign(coeffs=2 * quadratic.coeffs)
+            batch = objective_write_cross_terms(quadratic, f, batch, batch_size)
+            batch = objective_write_quad_terms(quadratic, f, batch, batch_size)
+            batch.append("] / 2\n")
+
+    if batch:  # write the remaining lines
+        f.writelines(batch)
 
-    iterate = zip(labels, vars, coeffs, labels_, sign_, rhs_)
+
+def constraints_to_file(m, f, log=False, batch_size=50000):
+    if not len(m.constraints):
+        return
+
+    f.write("\n\ns.t.\n\n")
+    names = m.constraints
     if log:
-        iterate = tqdm(iterate, "Writing constraints.", len(m.constraints.labels))
+        names = tqdm(
+            list(names),
+            desc="Writing constraints.",
+            colour=TQDM_COLOR,
+        )
+
+    batch = []
+    for name in names:
+        df = m.constraints[name].flat
+
+        labels = df.labels.values
+        vars = df.vars.values
+        coeffs = df.coeffs.values
+        rhs = df.rhs.values
+        sign = df.sign.values
 
-    for l, v, c, l_, s_, r_ in iterate:
-        if not c.size:
+        len_df = len(df)  # compute length once
+        if not len_df:
             continue
-        # Group repeated variables in the same constraint
-        df = pd.DataFrame({"coeffs": c, "labels": l, "vars": v})
-        df = df.groupby(["labels", "vars"], as_index=False).sum()
-        c, l, v = df.coeffs.values, df.labels.values, df.vars.values
-
-        diff_con = l[:-1] != l[1:]
-        new_con_b = concatenate([asarray([True]), diff_con])
-        end_of_con_b = concatenate([diff_con, asarray([True])])
-
-        l = fill_by(v.shape, new_con_b, "\nc" + int_to_str(l_) + ":\n")
-        s = fill_by(v.shape, end_of_con_b, "\n" + s_.astype(object) + "\n")
-        r = fill_by(v.shape, end_of_con_b, float_to_str(r_, ensure_sign=False))
-        constraints = l + float_to_str(c) + " x" + int_to_str(v) + s + r
-
-        f.write("\n".join(constraints))
-        f.write("\n")
-        del l, s, r, constraints
 
+        # write out the start to enable a fast loop afterwards
+        idx = 0
+        label = labels[idx]
+        coeff = coeffs[idx]
+        var = vars[idx]
+        batch.append(f"c{label}:\n{coeff:+.12g} x{var}\n")
+        prev_label = label
+        prev_sign = sign[idx]
+        prev_rhs = rhs[idx]
+
+        for idx in range(1, len_df):
+            label = labels[idx]
+            coeff = coeffs[idx]
+            var = vars[idx]
+
+            if label != prev_label:
+                batch.append(
+                    f"{prev_sign} {prev_rhs:+.12g}\n\nc{label}:\n{coeff:+.12g} x{var}\n"
+                )
+                prev_sign = sign[idx]
+                prev_rhs = rhs[idx]
+            else:
+                batch.append(f"{coeff:+.12g} x{var}\n")
 
-def bounds_to_file(m, f, log=False):
+            batch = handle_batch(batch, f, batch_size)
+
+            prev_label = label
+
+        batch.append(f"{prev_sign} {prev_rhs:+.12g}\n")
+
+    if batch:  # write the remaining lines
+        f.writelines(batch)
+
+
+def bounds_to_file(m, f, log=False, batch_size=10000):
     """
     Write out variables of a model to a lp file.
     """
-    f.write("\n\nbounds\n\n")
-    lower = m.non_binaries.iter_ravel("lower", filter_missings=True)
-    upper = m.non_binaries.iter_ravel("upper", filter_missings=True)
-    labels = m.non_binaries.iter_ravel("labels", filter_missings=True)
+    names = list(m.variables.continuous) + list(m.variables.integers)
+    if not len(list(names)):
+        return
 
-    iterate = zip(lower, labels, upper)
+    f.write("\n\nbounds\n\n")
     if log:
-        iterate = tqdm(iterate, "Writing variables.", len(m.non_binaries.labels))
+        names = tqdm(
+            list(names),
+            desc="Writing continuous variables.",
+            colour=TQDM_COLOR,
+        )
 
-    for lo, l, up in iterate:
-        if not l.size:
-            continue
+    batch = []  # to store batch of lines
+    for name in names:
+        df = m.variables[name].flat
+
+        labels = df.labels.values
+        lowers = df.lower.values
+        uppers = df.upper.values
+
+        for idx in range(len(df)):
+            label = labels[idx]
+            lower = lowers[idx]
+            upper = uppers[idx]
+            batch.append(f"{lower:+.12g} <= x{label} <= {upper:+.12g}\n")
+            batch = handle_batch(batch, f, batch_size)
 
-        bounds = float_to_str(lo) + " <= x" + int_to_str(l) + " <= " + float_to_str(up)
-        f.write("\n".join(bounds))
-        f.write("\n")
-        del bounds
+    if batch:  # write the remaining lines
+        f.writelines(batch)
 
 
-def binaries_to_file(m, f, log=False):
+def binaries_to_file(m, f, log=False, batch_size=1000):
     """
     Write out binaries of a model to a lp file.
     """
-    f.write("\n\nbinary\n\n")
-    labels = m.binaries.iter_ravel("labels", filter_missings=True)
-
-    if len(m.variables._binary_variables) == 0:
+    names = m.variables.binaries
+    if not len(list(names)):
         return
 
-    iterate = labels
+    f.write("\n\nbinary\n\n")
     if log:
-        iterate = tqdm(iterate, "Writing binaries.", len(m.binaries.labels))
+        names = tqdm(
+            list(names),
+            desc="Writing binary variables.",
+            colour=TQDM_COLOR,
+        )
 
-    for l in iterate:
-        if not l.size:
-            continue
+    batch = []  # to store batch of lines
+    for name in names:
+        df = m.variables[name].flat
+
+        for label in df.labels.values:
+            batch.append(f"x{label}\n")
+            batch = handle_batch(batch, f, batch_size)
 
-        bounds = "x" + int_to_str(l)
-        f.write("\n".join(bounds))
-        f.write("\n")
-        del bounds
+    if batch:  # write the remaining lines
+        f.writelines(batch)
 
 
-def integers_to_file(m, f, log=False):
+def integers_to_file(m, f, log=False, batch_size=1000):
     """
     Write out integers of a model to a lp file.
     """
-    f.write("\n\ngeneral\n\n")
-    labels = m.integers.iter_ravel("labels", filter_missings=True)
-
-    if len(m.variables._integer_variables) == 0:
+    names = m.variables.integers
+    if not len(list(names)):
         return
 
-    iterate = labels
+    f.write("\n\ninteger\n\n")
     if log:
-        iterate = tqdm(iterate, "Writing integer variables.", len(m.integers.labels))
+        names = tqdm(
+            list(names),
+            desc="Writing integer variables.",
+            colour=TQDM_COLOR,
+        )
 
-    for l in iterate:
-        if not l.size:
-            continue
+    batch = []  # to store batch of lines
+    for name in names:
+        df = m.variables[name].flat
+
+        for label in df.labels.values:
+            batch.append(f"x{label}\n")
+            batch = handle_batch(batch, f, batch_size)
 
-        bounds = "x" + int_to_str(l)
-        f.write("\n".join(bounds))
-        f.write("\n")
-        del bounds
+    if batch:  # write the remaining lines
+        f.writelines(batch)
 
 
 def to_file(m, fn):
     """
     Write out a model to a lp or mps file.
     """
     fn = Path(m.get_problem_file(fn))
-
     if fn.exists():
         fn.unlink()
 
     if fn.suffix == ".lp":
-        log = m._xCounter > 10000
+        log = m._xCounter > 10_000
+
+        batch_size = 5000
 
         with open(fn, mode="w") as f:
             start = time.time()
 
-            objective_to_file(m, f, log)
-            constraints_to_file(m, f, log)
-            bounds_to_file(m, f, log)
-            binaries_to_file(m, f, log)
-            integers_to_file(m, f, log)
+            objective_to_file(m, f, log=log)
+            constraints_to_file(m, f, log=log, batch_size=batch_size)
+            bounds_to_file(m, f, log=log, batch_size=batch_size)
+            binaries_to_file(m, f, log=log, batch_size=batch_size)
+            integers_to_file(m, f, log=log, batch_size=batch_size)
             f.write("end\n")
 
             logger.info(f" Writing time: {round(time.time()-start, 2)}s")
 
     elif fn.suffix == ".mps":
-        if "highs" in solvers.available_solvers:
-            # Use very fast highspy implementation
-            # Might be replaced by custom writer, however needs C bindings for performance
-            h = m.to_highspy()
-            h.writeModel(str(fn))
-        else:
+        if "highs" not in solvers.available_solvers:
             raise RuntimeError(
                 "Package highspy not installed. This is required to exporting to MPS file."
             )
 
+        # Use very fast highspy implementation
+        # Might be replaced by custom writer, however needs C bindings for performance
+        h = m.to_highspy()
+        h.writeModel(str(fn))
     else:
         raise ValueError(
             f"Cannot write problem to {fn}, file format `{fn.suffix}` not supported."
         )
 
     return fn
 
@@ -259,19 +344,23 @@
 
     names = "x" + M.vlabels.astype(str).astype(object)
     kwargs = {}
     if len(m.binaries.labels) + len(m.integers.labels):
         kwargs["vtype"] = M.vtypes
     x = model.addMVar(M.vlabels.shape, M.lb, M.ub, name=list(names), **kwargs)
 
-    model.setObjective(M.c @ x)
+    if m.is_quadratic:
+        model.setObjective(0.5 * x.T @ M.Q @ x + M.c @ x)
+    else:
+        model.setObjective(M.c @ x)
 
-    names = "c" + M.clabels.astype(str).astype(object)
-    c = model.addMConstr(M.A, x, M.sense, M.b)
-    c.setAttr("ConstrName", list(names))
+    if len(m.constraints):
+        names = "c" + M.clabels.astype(str).astype(object)
+        c = model.addMConstr(M.A, x, M.sense, M.b)
+        c.setAttr("ConstrName", list(names))
 
     model.update()
     return model
 
 
 def to_highspy(m):
     """
@@ -291,33 +380,50 @@
     model : highspy.Highs
     """
     import highspy
 
     M = m.matrices
     h = highspy.Highs()
     h.addVars(len(M.vlabels), M.lb, M.ub)
-    if len(m.binaries.labels) + len(m.integers.labels):
+    if len(m.binaries) + len(m.integers):
         vtypes = M.vtypes
         labels = np.arange(len(vtypes))[(vtypes == "B") | (vtypes == "I")]
         n = len(labels)
         h.changeColsIntegrality(n, labels, ones_like(labels))
-        if len(m.binaries.labels):
+        if len(m.binaries):
             labels = np.arange(len(vtypes))[vtypes == "B"]
             n = len(labels)
             h.changeColsBounds(n, labels, zeros_like(labels), ones_like(labels))
+
+    # linear objective
     h.changeColsCost(len(M.c), np.arange(len(M.c), dtype=np.int32), M.c)
-    A = M.A.tocsr()
-    num_cons = A.shape[0]
-    lower = np.where(M.sense != "<", M.b, -np.inf)
-    upper = np.where(M.sense != ">", M.b, np.inf)
-    h.addRows(num_cons, lower, upper, A.nnz, A.indptr, A.indices, A.data)
+
+    # linear constraints
+    A = M.A
+    if A is not None:
+        A = A.tocsr()
+        num_cons = A.shape[0]
+        lower = np.where(M.sense != "<", M.b, -np.inf)
+        upper = np.where(M.sense != ">", M.b, np.inf)
+        h.addRows(num_cons, lower, upper, A.nnz, A.indptr, A.indices, A.data)
+
     lp = h.getLp()
-    lp.row_names_ = "c" + M.clabels.astype(str).astype(object)
     lp.col_names_ = "x" + M.vlabels.astype(str).astype(object)
+    if len(M.clabels):
+        lp.row_names_ = "c" + M.clabels.astype(str).astype(object)
     h.passModel(lp)
+
+    # quadrative objective
+    Q = M.Q
+    if Q is not None:
+        Q = triu(Q)
+        Q = Q.tocsr()
+        num_vars = Q.shape[0]
+        h.passHessian(num_vars, Q.nnz, 1, Q.indptr, Q.indices, Q.data)
+
     return h
 
 
 def to_block_files(m, fn):
     """
     Write out the linopy model to a block structured output.
 
@@ -390,17 +496,15 @@
     def filtered(arr, mask, key):
         """
         Set coefficients to zero where mask is False, keep others unchanged.
 
         PIPS requires this information to set the shape of sub-matrices.
         """
         assert key in keys
-        if key == "coeffs":
-            return np.where(mask, arr, 0)
-        return arr
+        return np.where(mask, arr, 0) if key == "coeffs" else arr
 
     for key, suffix in zip(keys, ["row", "data", "col"]):
         arr = cons.ravel(key, "vars", filter_missings=True)
         for n in tqdm(range(N + 1), desc=f"Write constraint {key}"):
             is_conblock_n = conblocks == n
             is_varblock_n = varblocks == n
 
@@ -433,15 +537,15 @@
                 )
 
 
 def non_bool_dict(d):
     """
     Convert bool to int for netCDF4 storing.
     """
-    return {k: v if not isinstance(v, bool) else int(v) for k, v in d.items()}
+    return {k: int(v) if isinstance(v, bool) else v for k, v in d.items()}
 
 
 def to_netcdf(m, *args, **kwargs):
     """
     Write out the model to a netcdf file.
 
     Parameters
@@ -449,33 +553,34 @@
     m : linopy.Model
         Model to write out.
     *args
         Arguments passed to ``xarray.Dataset.to_netcdf``.
     **kwargs : TYPE
         Keyword arguments passed to ``xarray.Dataset.to_netcdf``.
     """
-    from linopy.expressions import LinearExpression
 
-    def get_and_rename(m, attr, prefix=""):
-        ds = getattr(m, attr)
-        if isinstance(ds, LinearExpression):
-            ds = ds.data
-        return ds.rename({v: prefix + attr + "-" + v for v in ds})
+    def with_prefix(ds, prefix):
+        ds = ds.rename({d: f"{prefix}-{d}" for d in [*ds.dims, *ds]})
+        ds.attrs = {f"{prefix}-{k}": v for k, v in ds.attrs.items()}
+        return ds
 
     vars = [
-        get_and_rename(m.variables, attr, "variables_")
-        for attr in m.variables.dataset_attrs
+        with_prefix(var.data, f"variables-{name}") for name, var in m.variables.items()
     ]
     cons = [
-        get_and_rename(m.constraints, attr, "constraints_")
-        for attr in m.constraints.dataset_attrs
+        with_prefix(con.data, f"constraints-{name}")
+        for name, con in m.constraints.items()
     ]
-    others = [get_and_rename(m, d) for d in m.dataset_attrs + ["objective"]]
+    obj = [with_prefix(m.objective.data, "objective")]
+    params = [with_prefix(m.parameters, "params")]
+
     scalars = {k: getattr(m, k) for k in m.scalar_attrs}
-    ds = xr.merge(vars + cons + others).assign_attrs(non_bool_dict(scalars))
+    ds = xr.merge(vars + cons + obj + params)
+    ds = ds.assign_attrs(scalars)
+    ds.attrs = non_bool_dict(ds.attrs)
 
     for k in ds:
         ds[k].attrs = non_bool_dict(ds[k].attrs)
 
     ds.to_netcdf(*args, **kwargs)
 
 
@@ -490,32 +595,48 @@
     **kwargs
         Keyword arguments passed to ``xarray.load_dataset``.
 
     Returns
     -------
     m : linopy.Model
     """
-    from linopy.model import Constraints, LinearExpression, Model, Variables
+    from linopy.model import (
+        Constraint,
+        Constraints,
+        LinearExpression,
+        Model,
+        Variable,
+        Variables,
+    )
 
     m = Model()
-    all_ds = xr.load_dataset(path, **kwargs)
+    ds = xr.load_dataset(path, **kwargs)
+
+    def get_prefix(ds, prefix):
+        ds = ds[[k for k in ds if k.startswith(prefix)]]
+        ds = ds.rename({d: d.split(prefix + "-", 1)[1] for d in [*ds.dims, *ds]})
+        ds.attrs = {
+            k.split(prefix + "-", 1)[1]: v
+            for k, v in ds.attrs.items()
+            if k.startswith(prefix + "-")
+        }
+        return ds
+
+    vars = get_prefix(ds, "variables")
+    var_names = list({k.split("-", 1)[0] for k in vars})
+    variables = {k: Variable(get_prefix(vars, k), m, k) for k in var_names}
+    m._variables = Variables(variables, m)
+
+    cons = get_prefix(ds, "constraints")
+    con_names = list({k.split("-", 1)[0] for k in cons})
+    constraints = {k: Constraint(get_prefix(cons, k), m, k) for k in con_names}
+    m._constraints = Constraints(constraints, m)
+
+    objective = get_prefix(ds, "objective")
+    m._objective = LinearExpression(objective, m)
 
-    def get_and_rename(ds, attr, prefix=""):
-        keys = [k for k in ds if k.startswith(prefix + attr + "-")]
-        return ds[keys].rename({k: k[len(prefix + attr) + 1 :] for k in keys})
-
-    attrs = Variables.dataset_attrs
-    kwargs = {attr: get_and_rename(all_ds, attr, "variables_") for attr in attrs}
-    m._variables = Variables(**kwargs, model=m)
-
-    attrs = Constraints.dataset_attrs
-    kwargs = {attr: get_and_rename(all_ds, attr, "constraints_") for attr in attrs}
-    m._constraints = Constraints(**kwargs, model=m)
-
-    for attr in m.dataset_attrs:
-        setattr(m, attr, get_and_rename(all_ds, attr))
-    m._objective = LinearExpression(get_and_rename(all_ds, "objective"), m)
+    m._parameters = get_prefix(ds, "parameter")
 
     for k in m.scalar_attrs:
-        setattr(m, k, all_ds.attrs.pop(k))
+        setattr(m, k, ds.attrs.get(k))
 
     return m
```

### Comparing `linopy-0.1.5/linopy/model.py` & `linopy-0.2/linopy/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numpy import inf, nan
 from xarray import DataArray, Dataset
 
 from linopy import solvers
-from linopy.common import best_int, maybe_replace_signs, replace_by_map
-from linopy.constants import ModelStatus, TerminationCondition
-from linopy.constraints import (
-    AnonymousConstraint,
-    AnonymousScalarConstraint,
-    Constraints,
+from linopy.common import (
+    as_dataarray,
+    best_int,
+    maybe_replace_signs,
+    replace_by_map,
+    save_join,
+)
+from linopy.constants import TERM_DIM, ModelStatus, TerminationCondition
+from linopy.constraints import AnonymousScalarConstraint, Constraint, Constraints
+from linopy.expressions import (
+    LinearExpression,
+    QuadraticExpression,
+    ScalarLinearExpression,
 )
-from linopy.expressions import LinearExpression, ScalarLinearExpression
 from linopy.io import to_block_files, to_file, to_gurobipy, to_highspy, to_netcdf
 from linopy.matrices import MatrixAccessor
-from linopy.solvers import available_solvers
+from linopy.solvers import available_solvers, quadratic_solvers
 from linopy.variables import ScalarVariable, Variable, Variables
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     """
@@ -58,14 +64,15 @@
         "_objective",
         "_parameters",
         "_solution",
         "_dual",
         # hidden attributes
         "_status",
         "_termination_condition",
+        # TODO: move counters to Variables and Constraints class
         "_xCounter",
         "_cCounter",
         "_varnameCounter",
         "_connameCounter",
         "_blocks",
         "_objective_value",
         # TODO: check if these should not be mutable
@@ -101,16 +108,14 @@
         linopy.Model
         """
         self._variables = Variables(model=self)
         self._constraints = Constraints(model=self)
         self._objective = LinearExpression(None, self)
         self._parameters = Dataset()
 
-        self._solution = Dataset()
-        self._dual = Dataset()
         self._objective_value = nan
 
         self._status = "initialized"
         self._termination_condition = ""
         self._xCounter = 0
         self._cCounter = 0
         self._varnameCounter = 0
@@ -163,30 +168,22 @@
         self._parameters = Dataset(value)
 
     @property
     def solution(self):
         """
         Solution calculated by the optimization.
         """
-        return self._solution
-
-    @solution.setter
-    def solution(self, value):
-        self._solution = Dataset(value)
+        return self.variables.solution
 
     @property
     def dual(self):
         """
         Dual values calculated by the optimization.
         """
-        return self._dual
-
-    @dual.setter
-    def dual(self, value):
-        self._dual = Dataset(value)
+        return self.constraints.dual
 
     @property
     def status(self):
         """
         Status of the model.
         """
         return self._status
@@ -269,15 +266,15 @@
     def solver_dir(self, value):
         if not isinstance(value, [str, Path]):
             raise TypeError("'solver_dir' must path-like.")
         self._solver_dir = Path(value)
 
     @property
     def dataset_attrs(self):
-        return ["parameters", "solution", "dual"]
+        return ["parameters"]
 
     @property
     def scalar_attrs(self):
         return [
             "objective_value",
             "status",
             "_xCounter",
@@ -287,22 +284,22 @@
             "force_dim_names",
         ]
 
     def __repr__(self):
         """
         Return a string representation of the linopy model.
         """
-        var_string = self.variables.labels.__repr__().split("\n", 1)[1]
-        var_string = var_string.replace("Data variables:\n", "Data:\n")
-        con_string = self.constraints.labels.__repr__().split("\n", 1)[1]
-        con_string = con_string.replace("Data variables:\n", "Data:\n")
+        var_string = self.variables.__repr__().split("\n", 2)[2]
+        con_string = self.constraints.__repr__().split("\n", 2)[2]
+        model_string = f"Linopy {self.type} model"
+
         return (
-            f"Linopy model\n============\n\n"
-            f"Variables:\n----------\n{var_string}\n\n"
-            f"Constraints:\n------------\n{con_string}\n\n"
+            f"{model_string}\n{'=' * len(model_string)}\n\n"
+            f"Variables:\n----------\n{var_string}\n"
+            f"Constraints:\n------------\n{con_string}\n"
             f"Status:\n-------\n{self.status}"
         )
 
     def __getitem__(self, key):
         """
         Get a model variable by the name.
         """
@@ -417,93 +414,61 @@
         [5]: x[5] ∈ [0, inf]
         [6]: x[6] ∈ [0, inf]
         [7]: x[7] ∈ [0, inf]
         [8]: x[8] ∈ [0, inf]
         [9]: x[9] ∈ [0, inf]
         """
         if name is None:
-            name = "var" + str(self._varnameCounter)
+            name = f"var{self._varnameCounter}"
             self._varnameCounter += 1
 
         if name in self.variables:
             raise ValueError(f"Variable '{name}' already assigned to model")
 
         if binary and integer:
             raise ValueError("Variable cannot be both binary and integer.")
 
-        if not binary:
-            lower = DataArray(lower, coords=coords, **kwargs)
-            upper = DataArray(upper, coords=coords, **kwargs)
-            if coords is None:
-                # only a lazy calculation for extracting coords, shape and size
-                broadcasted = lower.chunk() + upper.chunk()
-                coords = broadcasted.coords
-                if not coords and broadcasted.size > 1:
-                    raise ValueError(
-                        "Both `lower` and `upper` have missing coordinates"
-                        " while the broadcasted array is of size > 1."
-                    )
-        else:
-            # check if lower and upper and non-defaults
+        if binary:
             if (lower != -inf) or (upper != inf):
-                raise ValueError(
-                    "Argument lower and upper not valid for binary variables."
-                )
-            # for general compatibility when ravelling all values set non-nan
-            lower = DataArray(-inf, coords=coords, **kwargs)
-            upper = DataArray(inf, coords=coords, **kwargs)
+                raise ValueError("Binary variables cannot have lower or upper bounds.")
+            else:
+                lower, upper = 0, 1
 
-        labels = DataArray(-2, coords=coords).assign_attrs(
-            binary=binary, integer=integer
+        data = Dataset(
+            {
+                "lower": as_dataarray(lower, coords, **kwargs),
+                "upper": as_dataarray(upper, coords, **kwargs),
+            }
         )
 
-        # ensure order of dims is the same
-        lower = lower.transpose(*[d for d in labels.dims if d in lower.dims])
-        upper = upper.transpose(*[d for d in labels.dims if d in upper.dims])
-
         if mask is not None:
-            mask = DataArray(mask).astype(bool)
-            mask, _ = xr.align(mask, labels, join="right")
-            assert set(mask.dims).issubset(
-                labels.dims
-            ), "Dimensions of mask not a subset of resulting labels dimensions."
+            mask = as_dataarray(mask, coords=data.coords, dims=data.dims).astype(bool)
 
-        # It is important to end up with monotonically increasing labels in the
-        # model's variables container as we use it for indirect indexing.
-        labels_reindexed = labels.reindex_like(self.variables.labels, fill_value=-1)
-        if not labels.equals(labels_reindexed):
-            warnings.warn(
-                f"Reindexing variable `{name}` to match existing coordinates.",
-                UserWarning,
-            )
-            labels = labels_reindexed
-            lower = lower.reindex_like(labels)
-            upper = upper.reindex_like(labels)
-            if mask is None:
-                mask = labels != -1
-            else:
-                mask = mask.reindex_like(labels_reindexed, fill_value=False)
+        labels = DataArray(-2, coords=data.coords)
 
         self.check_force_dim_names(labels)
 
         start = self._xCounter
         end = start + labels.size
         labels.data = np.arange(start, end).reshape(labels.shape)
         self._xCounter += labels.size
 
         if mask is not None:
             labels = labels.where(mask, -1)
 
+        data = data.assign(labels=labels).assign_attrs(
+            label_range=(start, end), name=name, binary=binary, integer=integer
+        )
+
         if self.chunk:
-            labels = labels.chunk(self.chunk)
-            lower = lower.chunk(self.chunk)
-            upper = upper.chunk(self.chunk)
+            data = data.chunk(self.chunk)
 
-        self.variables.add(name, labels, lower, upper, start=start, end=end)
-        return self.variables[name]
+        variable = Variable(data, name=name, model=self)
+        self.variables.add(variable)
+        return variable
 
     def add_constraints(
         self, lhs, sign=None, rhs=None, name=None, coords=None, mask=None
     ):
         """
         Assign a new, possibly multi-dimensional array of constraints to the
         model.
@@ -511,15 +476,15 @@
         Constraints are added by defining a left hand side (lhs), the sign and
         the right hand side (rhs). The lhs has to be a linopy.LinearExpression
         and the rhs a constant (array of constants). The function return the
         an array with the constraint labels (integers).
 
         Parameters
         ----------
-        lhs : linopy.LinearExpression/linopy.AnonymousConstraint/callable
+        lhs : linopy.LinearExpression/linopy.Constraint/callable
             Left hand side of the constraint(s) or optionally full constraint.
             In case a linear expression is passed, `sign` and `rhs` must not be
             None.
             If a function is passed, it is called for every combination of
             coordinates given in `coords`. It's first argument has to be the
             model, followed by scalar argument for each coordinate given in
             coordinates.
@@ -540,106 +505,89 @@
 
 
         Returns
         -------
         labels : linopy.model.Constraint
             Array containing the labels of the added constraints.
         """
-        labels = None
 
-        if name is None:
-            name = "con" + str(self._connameCounter)
-            self._connameCounter += 1
+        def assert_sign_rhs_are_None(lhs, sign, rhs):
+            if sign is not None or rhs is not None:
+                msg = f"Passing arguments `sign` and `rhs` together with a {type(lhs)} is ambiguous."
+                raise ValueError(msg)
+
+        def assert_sign_rhs_not_None(lhs, sign, rhs):
+            if sign is None or rhs is None:
+                msg = f"Arguments `sign` and `rhs` cannot be None when passing along with a {type(lhs)}."
+                raise ValueError(msg)
 
         if name in self.constraints:
             raise ValueError(f"Constraint '{name}' already assigned to model")
-
-        if callable(lhs):
+        elif name is None:
+            name = f"con{self._connameCounter}"
+            self._connameCounter += 1
+        if sign is not None:
+            sign = maybe_replace_signs(as_dataarray(sign))
+        if rhs is not None:
+            rhs = as_dataarray(rhs)
+
+        if isinstance(lhs, LinearExpression):
+            assert_sign_rhs_not_None(lhs, sign, rhs)
+            data = lhs.data.assign(sign=sign, rhs=rhs)
+        elif callable(lhs):
             assert coords is not None, "`coords` must be given when lhs is a function"
             rule = lhs
-            lhs = AnonymousConstraint.from_rule(self, rule, coords)
-
-        if isinstance(lhs, AnonymousScalarConstraint):
-            lhs = lhs.to_anonymous_constraint()
-
-        if isinstance(lhs, AnonymousConstraint):
-            if sign is not None or rhs is not None:
-                raise ValueError(
-                    "Passing arguments `sign` and `rhs` together with a constraint"
-                    " is ambiguous."
-                )
-            labels = lhs.labels  # returns an empty data array of correct shape
-            sign = lhs.sign
-            rhs = lhs.rhs
-            lhs = lhs.lhs
-        else:
-            if sign is None or rhs is None:
-                raise ValueError(
-                    "Argument `sign` and `rhs` must not be None if first argument "
-                    " is an expression."
-                )
-        if isinstance(lhs, (list, tuple)):
-            lhs = self.linexpr(*lhs)
+            assert_sign_rhs_are_None(lhs, sign, rhs)
+            data = Constraint.from_rule(self, rule, coords).data
+        elif isinstance(lhs, AnonymousScalarConstraint):
+            assert_sign_rhs_are_None(lhs, sign, rhs)
+            data = lhs.to_constraint().data
+        elif isinstance(lhs, Constraint):
+            assert_sign_rhs_are_None(lhs, sign, rhs)
+            data = lhs.data
+        elif isinstance(lhs, (list, tuple)):
+            assert_sign_rhs_not_None(lhs, sign, rhs)
+            data = self.linexpr(*lhs).to_constraint(sign, rhs).data
         elif isinstance(lhs, (Variable, ScalarVariable, ScalarLinearExpression)):
-            lhs = lhs.to_linexpr()
-        assert isinstance(lhs, LinearExpression)
-
-        if isinstance(rhs, (Variable, LinearExpression)):
-            raise TypeError(f"Assigned rhs must be a constant, got {type(rhs)}).")
-
-        lhs = lhs.sanitize()
-        sign = maybe_replace_signs(DataArray(sign))
-        rhs = DataArray(rhs)
-
-        if labels is None:
-            labels = (lhs.vars.chunk() + rhs).sum("_term")
+            assert_sign_rhs_not_None(lhs, sign, rhs)
+            data = lhs.to_linexpr().to_constraint(sign, rhs).data
+        else:
+            raise ValueError(
+                f"Invalid type of `lhs` ({type(lhs)}) or invalid combination of `lhs`, `sign` and `rhs`."
+            )
 
         if mask is not None:
-            mask = DataArray(mask).astype(bool)
-            mask, _ = xr.align(mask, labels, join="right")
+            mask = as_dataarray(mask).astype(bool)
+            # TODO: simplify
             assert set(mask.dims).issubset(
-                labels.dims
+                data.dims
             ), "Dimensions of mask not a subset of resulting labels dimensions."
 
-        # It is important to end up with monotonically increasing labels in the
-        # model's constraints container as we use it for indirect indexing.
-        labels_reindexed = labels.reindex_like(self.constraints.labels, fill_value=-1)
-        if not labels.equals(labels_reindexed):
-            warnings.warn(
-                f"Reindexing constraint `{name}` to match existing coordinates.",
-                UserWarning,
-            )
-            labels = labels_reindexed
-            lhs = lhs.reindex_like(labels)
-            rhs = rhs.reindex_like(labels)
-            if mask is None:
-                mask = labels != -1
-            else:
-                mask = mask.reindex_like(labels_reindexed, fill_value=False)
+        labels = DataArray(-1, coords=data.indexes)
 
         self.check_force_dim_names(labels)
 
         start = self._cCounter
-        labels.data = np.arange(start, start + labels.size).reshape(labels.shape)
+        end = start + labels.size
+        labels.data = np.arange(start, end).reshape(labels.shape)
         self._cCounter += labels.size
 
         if mask is not None:
             labels = labels.where(mask, -1)
 
-        lhs = lhs.data.rename({"_term": f"{name}_term"})
+        data = data.assign(labels=labels).assign_attrs(
+            label_range=(start, end), name=name
+        )
 
         if self.chunk:
-            lhs = lhs.chunk(self.chunk)
-            sign = sign.chunk(self.chunk)
-            rhs = rhs.chunk(self.chunk)
-            labels = labels.chunk(self.chunk)
-
-        self.constraints.add(name, labels, lhs.coeffs, lhs.vars, sign, rhs)
+            data = data.chunk(self.chunk)
 
-        return self.constraints[name]
+        constraint = Constraint(data, name=name, model=self)
+        self.constraints.add(constraint)
+        return constraint
 
     def add_objective(self, expr, overwrite=False):
         """
         Add a linear objective function to the model.
 
         Parameters
         ----------
@@ -657,21 +605,30 @@
             assert self.objective.empty(), (
                 "Objective already defined."
                 " Set `overwrite` to True to force overwriting."
             )
 
         if isinstance(expr, (list, tuple)):
             expr = self.linexpr(*expr)
-        assert isinstance(expr, LinearExpression)
+
+        if not isinstance(expr, (LinearExpression, QuadraticExpression)):
+            raise ValueError(
+                f"Invalid type of `expr` ({type(expr)})."
+                " Must be a LinearExpression or QuadraticExpression."
+            )
 
         if self.chunk is not None:
             expr = expr.chunk(self.chunk)
 
-        if expr.vars.ndim > 1:
+        if len(expr.coord_dims):
             expr = expr.sum()
+
+        if expr.const != 0:
+            raise ValueError("Constant values in objective function not supported.")
+
         self._objective = expr
         return self._objective
 
     def remove_variables(self, name):
         """
         Remove all variables stored under reference name `name` from the model.
 
@@ -683,22 +640,25 @@
             Reference name of the variables which to remove, same as used in
             `model.add_variables`.
 
         Returns
         -------
         None.
         """
-        labels = self.variables.labels[name]
+        labels = self.variables[name].labels
         self.variables.remove(name)
 
-        remove_b = self.constraints.vars.isin(labels).any()
-        names = [name for name, remove in remove_b.items() if remove.item()]
-        self.constraints.remove(names)
+        for k in self.constraints:
+            vars = self.constraints[k].data["vars"]
+            vars = vars.where(~vars.isin(labels), -1)
+            self.constraints[k].data["vars"] = vars
 
-        self.objective = self.objective.sel(_term=~self.objective.vars.isin(labels))
+        self.objective = self.objective.sel(
+            {TERM_DIM: ~self.objective.vars.isin(labels)}
+        )
 
     def remove_constraints(self, name):
         """
         Remove all constraints stored under reference name `name` from the
         model.
 
         Parameters
@@ -710,49 +670,83 @@
         Returns
         -------
         None.
         """
         self.constraints.remove(name)
 
     @property
+    def continuous(self):
+        """
+        Get all continuous variables.
+        """
+        return self.variables.continuous
+
+    @property
     def binaries(self):
         """
         Get all binary variables.
         """
         return self.variables.binaries
 
     @property
     def integers(self):
         """
         Get all integer variables.
         """
         return self.variables.integers
 
     @property
-    def non_binaries(self):
-        """
-        Get all non-binary variables.
-        """
-        return self.variables.non_binaries
+    def is_linear(self):
+        return type(self.objective) is LinearExpression
+
+    @property
+    def is_quadratic(self):
+        return type(self.objective) is QuadraticExpression
+
+    @property
+    def type(self):
+        if (len(self.binaries) or len(self.integers)) and len(self.continuous):
+            variable_type = "MI"
+        elif len(self.binaries) or len(self.integers):
+            variable_type = "I"
+        else:
+            variable_type = ""
+
+        objective_type = "Q" if self.is_quadratic else "L"
+
+        return f"{variable_type}{objective_type}P"
 
     @property
     def nvars(self):
         """
         Get the total number of variables.
+
+        This excludes all variables which are not active.
         """
         return self.variables.nvars
 
     @property
     def ncons(self):
         """
         Get the total number of constraints.
+
+        This excludes all constraints which are not active.
         """
         return self.constraints.ncons
 
     @property
+    def shape(self):
+        """
+        Get the shape of the non-filtered constraint matrix.
+
+        This includes all constraints and variables which are not active.
+        """
+        return (self._cCounter, self._xCounter)
+
+    @property
     def blocks(self):
         """
         Blocks used as a basis to split the variables and constraint matrix.
         """
         return self._blocks
 
     @blocks.setter
@@ -772,18 +766,17 @@
     def calculate_block_maps(self):
         """
         Calculate the matrix block mappings based on dimensional blocks.
         """
         assert self.blocks is not None, "Blocks are not defined."
 
         dtype = self.blocks.dtype
-        self.variables.blocks = self.variables.get_blocks(self.blocks)
-        block_map = self.variables.blocks_to_blockmap(self.variables.blocks, dtype)
-
-        self.constraints.blocks = self.constraints.get_blocks(block_map)
+        self.variables.set_blocks(self.blocks)
+        block_map = self.variables.get_blockmap(dtype)
+        self.constraints.set_blocks(block_map)
 
         blocks = replace_by_map(self.objective.vars, block_map)
         self.objective = self.objective.assign(blocks=blocks)
 
     def linexpr(self, *args):
         """
         Create a linopy.LinearExpression from argument list.
@@ -854,38 +847,20 @@
         if callable(args[0]):
             assert len(args) == 2, (
                 "When first argument is a function, only one second argument "
                 "containing a tuple or a single set of coords must be given."
             )
             rule, coords = args
             return LinearExpression.from_rule(self, rule, coords)
-        if isinstance(args, tuple):
-            tuples = [
-                (c, self.variables[v]) if isinstance(v, str) else (c, v)
-                for (c, v) in args
-            ]
-            return LinearExpression.from_tuples(*tuples, chunk=self.chunk)
-        else:
+        if not isinstance(args, tuple):
             raise TypeError(f"Not supported type {args}.")
-
-    def vareval(self, expr: str, eval_kw=None, **kwargs):
-        raise NotImplementedError(
-            "vareval was removed in version `v0.1.0`. Please use m.add_variables() instead."
-        )
-
-    def lineval(self, expr: str, eval_kw=None, **kwargs):
-        raise NotImplementedError(
-            "lineval was removed in version `v0.1.0`. Please use arithmetic expressions instead."
-        )
-
-    def coneval(self, expr: str, eval_kw=None, **kwargs):
-        raise NotImplementedError(
-            "coneval was removed in version `v0.1.0`. Please use arithmetic "
-            "expressions and m.add_constraints() instead."
-        )
+        tuples = [
+            (c, self.variables[v]) if isinstance(v, str) else (c, v) for (c, v) in args
+        ]
+        return LinearExpression.from_tuples(*tuples, chunk=self.chunk)
 
     @property
     def coefficientrange(self):
         """
         Coefficient range of the constraints in the model.
         """
         return self.constraints.coefficientrange
@@ -900,52 +875,48 @@
             index=["min", "max"],
         )
 
     def get_solution_file(self, solution_fn=None):
         """
         Get a fresh created solution file if solution file is None.
         """
-        if solution_fn is None:
-            kwargs = dict(
-                prefix="linopy-solve-",
-                suffix=".sol",
-                mode="w",
-                dir=self.solver_dir,
-                delete=False,
-            )
-            with NamedTemporaryFile(**kwargs) as f:
-                return f.name
-        else:
+        if solution_fn is not None:
             return solution_fn
 
+        kwargs = dict(
+            prefix="linopy-solve-",
+            suffix=".sol",
+            mode="w",
+            dir=self.solver_dir,
+            delete=False,
+        )
+        with NamedTemporaryFile(**kwargs) as f:
+            return f.name
+
     def get_problem_file(self, problem_fn=None, io_api=None):
         """
         Get a fresh created problem file if problem file is None.
         """
-        if problem_fn is None:
-            if io_api == "mps":
-                suffix = ".mps"
-            else:
-                suffix = ".lp"
-
-            kwargs = dict(
-                prefix="linopy-problem-",
-                suffix=suffix,
-                mode="w",
-                dir=self.solver_dir,
-                delete=False,
-            )
-            with NamedTemporaryFile(**kwargs) as f:
-                return f.name
-        else:
+        if problem_fn is not None:
             return problem_fn
 
+        suffix = ".mps" if io_api == "mps" else ".lp"
+        kwargs = dict(
+            prefix="linopy-problem-",
+            suffix=suffix,
+            mode="w",
+            dir=self.solver_dir,
+            delete=False,
+        )
+        with NamedTemporaryFile(**kwargs) as f:
+            return f.name
+
     def solve(
         self,
-        solver_name="gurobi",
+        solver_name=None,
         io_api=None,
         problem_fn=None,
         solution_fn=None,
         log_fn=None,
         basis_fn=None,
         warmstart_fn=None,
         keep_files=False,
@@ -959,15 +930,15 @@
         The optimal values of the variables are stored in `model.solution`.
         The optimal dual variables are stored in `model.dual`.
 
         Parameters
         ----------
         solver_name : str, optional
             Name of the solver to use, this must be in `linopy.available_solvers`.
-            The default is 'gurobi'.
+            Default to the first entry in `linopy.available_solvers`.
         io_api : str, optional
             Api to use for communicating with the solver, must be one of
             {'lp', 'mps', 'direct'}. If set to 'lp'/'mps' the problem is written to an
             LP/MPS file which is then read by the solver. If set to
             'direct' the problem is communicated to the solver via the solver
             specific API, e.g. gurobipy. This may lead to faster run times.
             The default is set to 'lp' if available.
@@ -1022,24 +993,32 @@
                 sanitize_zeros=sanitize_zeros,
                 **solver_options,
             )
 
             self.objective_value = solved.objective_value
             self.status = solved.status
             self.termination_condition = solved.termination_condition
-            self.solution = solved.solution
-            self.dual = solved.dual
+            for k, v in self.variables.items():
+                v.solution = solved.variables[k].solution
+            for k, c in self.constraints.items():
+                if "dual" in solved.constraints[k]:
+                    c.dual = solved.constraints[k].dual
             return self.status, self.termination_condition
 
+        if len(available_solvers) == 0:
+            raise RuntimeError("No solver installed.")
+
+        if solver_name is None:
+            solver_name = available_solvers[0]
+
         logger.info(f" Solve linear problem using {solver_name.title()} solver")
         assert solver_name in available_solvers, f"Solver {solver_name} not installed"
 
         # reset result
-        self.solution = xr.Dataset()
-        self.dual = xr.Dataset()
+        self.reset_solution()
 
         if log_fn is not None:
             logger.info(f"Solver logs written to `{log_fn}`.")
 
         if solver_options:
             options_string = "\n".join(
                 f" - {k}: {v}" for k, v in solver_options.items()
@@ -1048,14 +1027,19 @@
 
         problem_fn = self.get_problem_file(problem_fn, io_api=io_api)
         solution_fn = self.get_solution_file(solution_fn)
 
         if sanitize_zeros:
             self.constraints.sanitize_zeros()
 
+        if self.is_quadratic and solver_name not in quadratic_solvers:
+            raise ValueError(
+                f"Solver {solver_name} does not support quadratic problems."
+            )
+
         try:
             func = getattr(solvers, f"run_{solver_name}")
             result = func(
                 self,
                 io_api,
                 problem_fn,
                 solution_fn,
@@ -1063,17 +1047,16 @@
                 warmstart_fn,
                 basis_fn,
                 keep_files,
                 **solver_options,
             )
         finally:
             for fn in (problem_fn, solution_fn):
-                if fn is not None:
-                    if os.path.exists(fn) and not keep_files:
-                        os.remove(fn)
+                if fn is not None and (os.path.exists(fn) and not keep_files):
+                    os.remove(fn)
 
         result.info()
 
         self.objective_value = result.solution.objective
         self.status = result.status.status.value
         self.termination_condition = result.status.termination_condition.value
         self.solver_model = result.solver_model
@@ -1081,44 +1064,50 @@
         if not result.status.is_ok:
             return result.status.status.value, result.status.termination_condition.value
 
         # map solution and dual to original shape which includes missing values
         sol = result.solution.primal.copy()
         sol.loc[-1] = nan
 
-        for name, labels in self.variables.labels.items():
-            idx = np.ravel(labels)
-            vals = sol[idx].values.reshape(labels.shape)
-            self.solution[name] = xr.DataArray(vals, labels.coords)
+        for name, var in self.variables.items():
+            idx = np.ravel(var.labels)
+            try:
+                vals = sol[idx].values.reshape(var.labels.shape)
+            except KeyError:
+                vals = sol.reindex(idx).values.reshape(var.labels.shape)
+            var.solution = xr.DataArray(vals, var.coords)
 
         if not result.solution.dual.empty:
             dual = result.solution.dual.copy()
             dual.loc[-1] = nan
 
-            for name, labels in self.constraints.labels.items():
-                idx = np.ravel(labels)
+            for name, con in self.constraints.items():
+                idx = np.ravel(con.labels)
                 try:
-                    vals = dual[idx].values.reshape(labels.shape)
+                    vals = dual[idx].values.reshape(con.labels.shape)
                 except KeyError:
-                    vals = dual.reindex(idx).values.reshape(labels.shape)
-                self.dual[name] = xr.DataArray(vals, labels.coords)
+                    vals = dual.reindex(idx).values.reshape(con.labels.shape)
+                con.dual = xr.DataArray(vals, con.labels.coords)
 
         return result.status.status.value, result.status.termination_condition.value
 
     def compute_set_of_infeasible_constraints(self):
         """
         Compute a set of infeasible constraints.
 
         This method requires gurobipy to be running.
 
         Returns
         -------
         labels : xr.DataArray
             Labels of the infeasible constraints. Labels with value -1 are not in the set.
         """
+        if "gurobi" not in available_solvers:
+            raise ImportError("Gurobi is required for this method.")
+
         import gurobipy
 
         solver_model = getattr(self, "solver_model")
 
         if not isinstance(solver_model, gurobipy.Model):
             raise NotImplementedError("Solver model must be a Gurobi Model.")
 
@@ -1133,14 +1122,21 @@
         cons = self.constraints.labels.isin(np.array(labels))
         subset = self.constraints.labels.where(cons, -1)
         subset = subset.drop_vars(
             [k for (k, v) in (subset == -1).all().items() if v.item()]
         )
         return subset
 
+    def reset_solution(self):
+        """
+        Reset the solution and dual values if available of the model.
+        """
+        self.variables.reset_solution()
+        self.constraints.reset_dual()
+
     to_netcdf = to_netcdf
 
     to_file = to_file
 
     to_gurobipy = to_gurobipy
 
     to_highspy = to_highspy
```

### Comparing `linopy-0.1.5/linopy/monkey_patch_xarray.py` & `linopy-0.2/linopy/monkey_patch_xarray.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/linopy/remote.py` & `linopy-0.2/linopy/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sun Feb 13 21:34:55 2022.
 
 @author: fabian
 """
 
+
 import logging
 import tempfile
 from dataclasses import dataclass
 
 from linopy.io import read_netcdf
 
 paramiko_present = True
 try:
     import paramiko
 except ImportError:
     paramiko_present = False
-    pass
-
 logger = logging.getLogger(__name__)
 
 command = """
 import linopy
 
 m = linopy.read_netcdf("{model_unsolved_file}")
 m.solve({solve_kwargs})
@@ -151,15 +150,15 @@
         """
         Write the python file of the RemoteHandler on the remote machine under
         `self.python_file`.
         """
         logger.info(f"Saving python script at {self.python_file} on remote")
         script_kwargs = dict(
             model_unsolved_file=self.model_unsolved_file,
-            solve_kwargs="**" + str(solve_kwargs),
+            solve_kwargs=f"**{solve_kwargs}",
             model_solved_file=self.model_solved_file,
         )
         with self.sftp_client.open(self.python_file, "w") as fn:
             fn.write(self.python_script(**script_kwargs))
 
     def write_model_on_remote(self, model):
         """
@@ -173,29 +172,29 @@
     def execute(self, cmd):
         """
         Execute a shell command on the remote machine.
         """
         cmd = cmd.strip("\n")
         self.stdin.write(cmd + "\n")
         finish = "End of stdout. Exit Status"
-        echo_cmd = "echo {} $?".format(finish)
+        echo_cmd = f"echo {finish} $?"
         self.stdin.write(echo_cmd + "\n")
         self.stdin.flush()
 
         print_stdout = False
         exit_status = 0
         for line in self.stdout:
             line = str(line).strip("\n").strip()
             if line.endswith(cmd):
                 # up to now everything was login and stdin
                 print_stdout = True
-            elif str(line).startswith(finish):
-                exit_status = int(str(line).rsplit(maxsplit=1)[1])
+            elif line.startswith(finish):
+                exit_status = int(line.rsplit(maxsplit=1)[1])
                 break
-            elif not finish in line and print_stdout:
+            elif finish not in line and print_stdout:
                 print(line)
 
         if exit_status:
             raise OSError("Execution on remote raised an error, see above.")
 
     def solve_on_remote(self, model, **kwargs):
         """
@@ -219,15 +218,15 @@
         -------
         linopy.model.Model
             Solved model.
         """
         self.write_python_file_on_remote(**kwargs)
         self.write_model_on_remote(model)
 
-        command = self.python_executable + " " + self.python_file
+        command = f"{self.python_executable} {self.python_file}"
 
         logger.info("Solving model on remote.")
         self.execute(command)
 
         logger.info("Retrieve solved model from remote.")
         with tempfile.NamedTemporaryFile(prefix="linopy", suffix=".nc") as fn:
             self.sftp_client.get(self.model_solved_file, fn.name)
```

### Comparing `linopy-0.1.5/linopy/solvers.py` & `linopy-0.2/linopy/solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Linopy module for solving lp files with different solvers.
 """
+
 import io
 import logging
 import os
 import re
 import subprocess as sub
 from pathlib import Path
 
+import numpy as np
 import pandas as pd
 
 from linopy.constants import (
     Result,
     Solution,
     SolverStatus,
     Status,
     TerminationCondition,
 )
 
-available_solvers = []
-
-if os.name == "nt":
-    which = "where"
-else:
-    which = "which"
+quadratic_solvers = ["gurobi", "xpress", "cplex", "highs"]
 
-if sub.run([which, "glpsol"], stdout=sub.DEVNULL, stderr=sub.STDOUT).returncode == 0:
-    available_solvers.append("glpk")
+available_solvers = []
 
-if sub.run([which, "cbc"], stdout=sub.DEVNULL, stderr=sub.STDOUT).returncode == 0:
-    available_solvers.append("cbc")
+which = "where" if os.name == "nt" else "which"
 
+# the first available solver will be the default solver
 try:
     import gurobipy
 
     available_solvers.append("gurobi")
 except (ModuleNotFoundError, ImportError):
     pass
 
 try:
     import highspy
 
     available_solvers.append("highs")
 except (ModuleNotFoundError, ImportError):
     pass
 
+if sub.run([which, "glpsol"], stdout=sub.DEVNULL, stderr=sub.STDOUT).returncode == 0:
+    available_solvers.append("glpk")
+
+
+if sub.run([which, "cbc"], stdout=sub.DEVNULL, stderr=sub.STDOUT).returncode == 0:
+    available_solvers.append("cbc")
 
 try:
     import cplex
 
     available_solvers.append("cplex")
 except (ModuleNotFoundError, ImportError):
     pass
@@ -253,21 +255,25 @@
         for line in iter(p.stdout.readline, b""):
             print(line.decode(), end="")
         p.stdout.close()
         p.wait()
     else:
         p.wait()
 
+    if not os.path.exists(solution_fn):
+        status = Status(SolverStatus.warning, TerminationCondition.unknown)
+        return Result(status, Solution())
+
     f = open(solution_fn)
 
     def read_until_break(f):
-        linebreak = False
-        while not linebreak:
+        while True:
             line = f.readline()
-            linebreak = line == "\n"
+            if line == "\n" or line == "":
+                break
             yield line
 
     info = io.StringIO("".join(read_until_break(f))[:-2])
     info = pd.read_csv(info, sep=":", index_col=0, header=None)[1]
     condition = info.Status.lower().strip()
     objective = float(re.sub(r"[^0-9\.\+\-e]+", "", info.Objective))
 
@@ -444,25 +450,30 @@
                 param = getattr(param, key_layer)
             param.set(value)
 
     m.read(problem_fn)
 
     if warmstart_fn:
         m.start.read_basis(warmstart_fn)
-    m.solve()
+
     is_lp = m.problem_type[m.get_problem_type()] == "LP"
 
-    if log_fn is not None:
-        log_f.close()
+    try:
+        m.solve()
+    except cplex.exceptions.errors.CplexSolverError as e:
+        pass
 
     condition = m.solution.get_status_string()
     termination_condition = CONDITION_MAP.get(condition, condition)
     status = Status.from_termination_condition(termination_condition)
     status.legacy_status = condition
 
+    if log_fn is not None:
+        log_f.close()
+
     def get_solver_solution() -> Solution:
         if basis_fn and is_lp:
             try:
                 m.solution.basis.write(basis_fn)
             except cplex.exceptions.errors.CplexSolverError:
                 logger.info("No model basis stored")
```

### Comparing `linopy-0.1.5/linopy/variables.py` & `linopy-0.2/linopy/variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,75 +2,78 @@
 """
 Linopy variables module.
 
 This module contains variable related definitions of the package.
 """
 
 import functools
-import re
+import logging
 from collections.abc import Iterable
 from dataclasses import dataclass, field
-from typing import Any, Mapping, Sequence, Union
+from typing import Any, Dict, Mapping, Sequence, Union
+from warnings import warn
 
 import dask
 import numpy as np
 import pandas as pd
 from deprecation import deprecated
 from numpy import floating, inf, issubdtype
-from xarray import DataArray, Dataset, zeros_like
-from xarray.core import indexing, utils
+from xarray import DataArray, Dataset, align, broadcast, zeros_like
 
 import linopy.expressions as expressions
 from linopy.common import (
-    _merge_inplace,
-    dictsel,
+    LocIndexer,
+    as_dataarray,
+    fill_missing_coords,
     forward_as_properties,
+    generate_indices_for_printout,
     has_optimized_model,
-    head_tail_range,
     is_constant,
     print_coord,
     print_single_variable,
+    save_join,
 )
 from linopy.config import options
+from linopy.constants import TERM_DIM
+
+logger = logging.getLogger(__name__)
 
 
 def varwrap(method, *default_args, **new_default_kwargs):
     @functools.wraps(method)
     def _varwrap(var, *args, **kwargs):
         for k, v in new_default_kwargs.items():
             kwargs.setdefault(k, v)
         return var.__class__(
-            method(var.labels, *default_args, *args, **kwargs), var.model
+            method(var.data, *default_args, *args, **kwargs), var.model, var.name
         )
 
     _varwrap.__doc__ = f"Wrapper for the xarray {method} function for linopy.Variable"
     if new_default_kwargs:
         _varwrap.__doc__ += f" with default arguments: {new_default_kwargs}"
 
     return _varwrap
 
 
 def _var_unwrap(var):
-    if isinstance(var, Variable):
-        return var.labels
-    return var
+    return var.data if isinstance(var, Variable) else var
 
 
 @forward_as_properties(
-    labels=[
+    data=[
         "attrs",
         "coords",
         "indexes",
-        "name",
+    ],
+    labels=[
         "shape",
         "size",
-        "values",
         "dims",
         "ndim",
-    ]
+    ],
 )
 class Variable:
     """
     Variable container for storing variable labels.
 
     The Variable class is a subclass of xr.DataArray hence most xarray functions
     can be applied to it. However most arithmetic operations are overwritten.
@@ -113,43 +116,60 @@
         coeffs   (dim_0, _term) int64 3 3
         vars     (dim_0, _term) int64 0 1
 
 
     Further operations like taking the negative and subtracting are supported.
     """
 
-    __slots__ = ("_labels", "_model")
+    __slots__ = ("_data", "_model")
     __array_ufunc__ = None
 
-    _fill_value = -1
+    _fill_value = {"labels": -1, "lower": np.nan, "upper": np.nan}
 
-    def __init__(self, labels: DataArray, model: Any):
+    def __init__(self, data: Dataset, model: Any, name: str):
         """
-        Initialize the Constraint.
+        Initialize the Variable.
 
         Parameters
         ----------
-        labels : xarray.DataArray
-            labels of the constraint.
+        labels : xarray.Dataset
+            data of the variable.
         model : linopy.Model
             Underlying model.
         """
         from linopy.model import Model
 
-        if not isinstance(labels, DataArray):
-            raise ValueError(f"labels must be a DataArray, got {type(labels)}")
+        if not isinstance(data, Dataset):
+            raise ValueError(f"data must be a Dataset, got {type(data)}")
 
         if not isinstance(model, Model):
             raise ValueError(f"model must be a Model, got {type(model)}")
 
-        self._labels = labels
+        # check that `labels`, `lower` and `upper`, `sign` and `mask` are in data
+        for attr in ("labels", "lower", "upper"):
+            if attr not in data:
+                raise ValueError(f"missing '{attr}' in data")
+
+        data = data.assign_attrs(name=name)
+        (data,) = broadcast(data)
+        for attr in (
+            "lower",
+            "upper",
+        ):  # convert to float, important for  operations like "shift"
+            if not issubdtype(data[attr].dtype, floating):
+                data[attr] = data[attr].astype(float)
+
+        if "label_range" not in data.attrs:
+            data.assign_attrs(label_range=(data.labels.min(), data.labels.max()))
+
+        self._data = data
         self._model = model
 
     def __getitem__(self, keys) -> "ScalarVariable":
-        keys = (keys,) if not isinstance(keys, tuple) else keys
+        keys = keys if isinstance(keys, tuple) else (keys,)
         assert all(map(pd.api.types.is_scalar, keys)), (
             "The get function of Variable is different as of xarray.DataArray. "
             "Set single values for each dimension in order to obtain a "
             "ScalarVariable. For all other purposes, use `.sel` and `.isel`."
         )
         if not self.labels.ndim:
             return ScalarVariable(self.labels.item(), self.model)
@@ -158,140 +178,98 @@
         ), f"expected {self.labels.ndim} keys, got {len(keys)}."
         key = dict(zip(self.labels.dims, keys))
         selector = [self.labels.get_index(k).get_loc(v) for k, v in key.items()]
         return ScalarVariable(self.labels.data[tuple(selector)], self.model)
 
     @property
     def loc(self):
-        return _LocIndexer(self)
-
-    @deprecated(details="Use `labels` instead of `to_array()`")
-    def to_array(self):
-        """
-        Convert the variable array to a xarray.DataArray.
-        """
-        return self.labels
+        return LocIndexer(self)
 
     def to_pandas(self):
         return self.labels.to_pandas()
 
-    def to_linexpr(self, coefficient=1):
+    def to_linexpr(
+        self,
+        coefficient: Union[
+            np.number, pd.Series, pd.DataFrame, np.ndarray, DataArray
+        ] = 1,
+    ) -> "expressions.LinearExpression":
         """
-        Create a linear exprssion from the variables.
+        Create a linear expression from the variables.
+
+        Parameters
+        ----------
+        coefficient : array-like, optional
+                Coefficient for the linear expression. This can be a numeric value, numpy array,
+                pandas series/dataframe or a DataArray. Default is 1.
+        Returns
+        -------
+        linopy.LinearExpression
+            Linear expression with the variables and coefficients.
         """
-        if isinstance(coefficient, (expressions.LinearExpression, Variable)):
-            raise TypeError(f"unsupported type of coefficient: {type(coefficient)}")
-        return expressions.LinearExpression.from_tuples((coefficient, self))
+        coefficient = as_dataarray(coefficient, coords=self.coords, dims=self.dims)
+        ds = Dataset({"coeffs": coefficient, "vars": self.labels}).expand_dims(
+            TERM_DIM, -1
+        )
+        return expressions.LinearExpression(ds, self.model)
 
     def __repr__(self):
         """
         Print the variable arrays.
         """
-        # don't loop over all values if not necessary
-        if not self.coords:
-            header = f"Variable\n{'-' * len('Variable')}"
-            lower = self.lower.item()
-            upper = self.upper.item()
-            coord = []
-            var_string, bound_string = print_single_variable(
-                self, self.name, coord, lower, upper
-            )
-            return f"{header}\n{var_string} {bound_string}"
-
-        # create header string
-        if self.shape:
-            shape_string = ", ".join(
-                [f"{self.dims[i]}: {self.shape[i]}" for i in range(self.ndim)]
+        max_lines = options["display_max_rows"]
+        dims = list(self.dims)
+        dim_sizes = list(self.data.sizes.values())
+        masked_entries = (~self.mask).sum().values
+        lines = []
+
+        if dims:
+            for indices in generate_indices_for_printout(dim_sizes, max_lines):
+                if indices is None:
+                    lines.append("\t\t...")
+                else:
+                    coord = [
+                        self.data[dims[i]].values[ind] for i, ind in enumerate(indices)
+                    ]
+                    label = self.labels.values[indices]
+                    line = (
+                        print_coord(coord)
+                        + ": "
+                        + print_single_variable(self.model, label)
+                    )
+                    lines.append(line)
+            # lines = align_lines_by_delimiter(lines, "∈")
+
+            shape_str = ", ".join(f"{d}: {s}" for d, s in zip(dims, dim_sizes))
+            mask_str = f" - {masked_entries} masked entries" if masked_entries else ""
+            lines.insert(
+                0,
+                f"Variable ({shape_str}){mask_str}\n{'-'* (len(shape_str) + len(mask_str) + 11)}",
             )
-            shape_string = f"({shape_string})"
         else:
-            shape_string = ""
-        n_masked = (~self.mask).sum().item()
-        mask_string = f" - {n_masked} masked entries" if n_masked else ""
-        header = f"Variable {shape_string}{mask_string}\n" + "-" * (
-            len("Variable") + len(shape_string) + len(mask_string) + 1
-        )
-
-        # create data string, print only a few values
-        max_print = options["display_max_rows"]
-        split_at = max_print // 2
-        to_print = head_tail_range(self.size, max_print)
-        truncate = self.size > max_print
-
-        # create string, we use numpy to get the indexes
-        if self.shape:
-            idx = np.unravel_index(to_print, self.shape)
-            labels = np.ravel(self.labels.values)[to_print]
-            coords = [self.indexes[self.dims[i]][idx[i]] for i in range(len(self.dims))]
-            coords = list(zip(*coords))
-        else:
-            # case a single variable was selected
-            idx = [0]
-            labels = np.ravel(self.labels.values)
-            coords = [[c.item() for c in self.coords.values()]]
-
-        if not self.size:
-            return f"{header}\nNone"
-
-        coord_strings = []
-        var_strings = []
-        bound_strings = []
-        trunc_strings = []
-        for i, coord in enumerate(coords):
-            label = labels[i]
-            variables = self.model.variables
-
-            coord_string = print_coord(coord) + ":"
-            trunc_string = "\n\t\t..." if i == split_at - 1 and truncate else ""
-
-            if label != -1:
-                vname, vcoord = self.model.variables.get_label_position(label)
-                lower = variables[vname].lower
-                lower = lower.sel(dictsel(vcoord, lower.dims)).item()
-                upper = variables[vname].upper
-                upper = upper.sel(dictsel(vcoord, upper.dims)).item()
-                var_string, bound_string = print_single_variable(
-                    self, vname, vcoord, lower, upper
-                )
-
-            else:
-                var_string = "None"
-                bound_string = ""
-
-            coord_strings.append(coord_string)
-            var_strings.append(var_string)
-            bound_strings.append(bound_string)
-            trunc_strings.append(trunc_string)
-
-        coord_width = max(len(c) for c in coord_strings)
-        var_width = max(len(v) for v in var_strings)
-
-        data_string = ""
-        for c, v, b, t in zip(coord_strings, var_strings, bound_strings, trunc_strings):
-            data_string += f"\n{c:<{coord_width}} {v:<{var_width}} {b}{t}"
+            lines.append(
+                f"Variable\n{'-'*8}\n{print_single_variable(self.model, self.labels.item())}"
+            )
 
-        return f"{header}{data_string}"
+        return "\n".join(lines)
 
     def __neg__(self):
         """
         Calculate the negative of the variables (converts coefficients only).
         """
         return self.to_linexpr(-1)
 
     def __mul__(self, other):
         """
         Multiply variables with a coefficient.
         """
-        if isinstance(other, (expressions.LinearExpression, Variable)):
-            raise TypeError(
-                "unsupported operand type(s) for *: "
-                f"{type(self)} and {type(other)}. "
-                "Non-linear expressions are not yet supported."
-            )
-        return self.to_linexpr(other)
+        if isinstance(other, (expressions.LinearExpression, Variable, ScalarVariable)):
+            return self.to_linexpr() * other
+        else:
+            return self.to_linexpr(other)
 
     def __rmul__(self, other):
         """
         Right-multiply variables with a coefficient.
         """
         return self.to_linexpr(other)
 
@@ -313,42 +291,25 @@
         """
         return self.__div__(coefficient)
 
     def __add__(self, other):
         """
         Add variables to linear expressions or other variables.
         """
-        if isinstance(other, Variable):
-            return expressions.LinearExpression.from_tuples((1, self), (1, other))
-        elif isinstance(other, expressions.LinearExpression):
-            return self.to_linexpr() + other
-        else:
-            raise TypeError(
-                "unsupported operand type(s) for +: " f"{type(self)} and {type(other)}"
-            )
+        return self.to_linexpr() + other
 
     def __radd__(self, other):
         # This is needed for using python's sum function
-        if other == 0:
-            return self
-        else:
-            return NotImplemented
+        return self if other == 0 else NotImplemented
 
     def __sub__(self, other):
         """
         Subtract linear expressions or other variables from the variables.
         """
-        if isinstance(other, Variable):
-            return expressions.LinearExpression.from_tuples((1, self), (-1, other))
-        elif isinstance(other, expressions.LinearExpression):
-            return self.to_linexpr() - other
-        else:
-            raise TypeError(
-                "unsupported operand type(s) for -: " f"{type(self)} and {type(other)}"
-            )
+        return self.to_linexpr() - other
 
     def __le__(self, other):
         return self.to_linexpr().__le__(other)
 
     def __ge__(self, other):
         return self.to_linexpr().__ge__(other)
 
@@ -361,14 +322,17 @@
         )
 
     def __lt__(self, other):
         raise NotImplementedError(
             "Inequalities only ever defined for >= rather than >."
         )
 
+    def __contains__(self, value):
+        return self.data.__contains__(value)
+
     def groupby(
         self,
         group,
         squeeze: "bool" = True,
         restore_coord_dims: "bool" = None,
     ):
         """
@@ -396,32 +360,14 @@
             A `LinearExpressionGroupBy` containing the xarray groups and ensuring
             the correct return type.
         """
         return self.to_linexpr().groupby(
             group=group, squeeze=squeeze, restore_coord_dims=restore_coord_dims
         )
 
-    def groupby_sum(self, group):
-        """
-        Sum variable over groups.
-
-        The function works in the same manner as the xarray.Dataset.groupby
-        function, but automatically sums over all terms.
-
-        Parameters
-        ----------
-        group : DataArray or IndexVariable
-            Array whose unique values should be used to group the expressions.
-
-        Returns
-        -------
-        Grouped linear expression.
-        """
-        return self.to_linexpr().groupby_sum(group)
-
     def rolling(
         self,
         dim: "Mapping[Any, int]" = None,
         min_periods: "int" = None,
         center: "bool | Mapping[Any, bool]" = False,
         **window_kwargs: "int",
     ) -> "expressions.LinearExpressionRolling":
@@ -449,43 +395,35 @@
         -------
         linopy.expression.LinearExpressionRolling
         """
         return self.to_linexpr().rolling(
             dim=dim, min_periods=min_periods, center=center, **window_kwargs
         )
 
-    def rolling_sum(self, **kwargs):
+    @property
+    def name(self):
         """
-        Rolling sum of variable.
-
-        Parameters
-        ----------
-        **kwargs :
-            Keyword arguments passed to xarray.DataArray.rolling.
-
-        Returns
-        -------
-        Rolling sum of variable.
+        Return the name of the variable.
         """
-        return self.to_linexpr().rolling_sum(**kwargs)
+        return self.attrs["name"]
 
     @property
     def labels(self):
         """
         Return the labels of the variable.
         """
-        return self._labels
+        return self.data.labels
 
     @property
     def data(self):
         """
         Get the data of the variable.
         """
         # Needed for compatibility with linopy.merge
-        return self.labels
+        return self._data
 
     @property
     def model(self):
         """
         Return the model of the variable.
         """
         return self._model
@@ -503,96 +441,152 @@
         if self.attrs["integer"]:
             return "Integer Variable"
         elif self.attrs["binary"]:
             return "Binary Variable"
         else:
             return "Continuous Variable"
 
+    @property
+    def range(self):
+        """
+        Return the range of the variable.
+        """
+        return self.data.attrs["label_range"]
+
     @classmethod
     @property
-    def fill_value(self):
+    def fill_value(cls):
         """
         Return the fill value of the variable.
         """
-        return self._fill_value
+        return cls._fill_value
 
     @property
     def mask(self):
         """
         Get the mask of the variable.
 
         The mask indicates on which coordinates the variable array is enabled
         (True) and disabled (False).
 
         Returns
         -------
         xr.DataArray
         """
-        return (self.labels != self._fill_value).astype(bool)
+        return (self.labels != self.fill_value["labels"]).astype(bool)
 
     @property
     def upper(self):
         """
         Get the upper bounds of the variables.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.variables.upper[self.name]
+        return self.data.upper
 
     @upper.setter
     @is_constant
     def upper(self, value):
         """
         Set the upper bounds of the variables.
 
         The function raises an error in case no model is set as a
         reference.
         """
         value = DataArray(value).broadcast_like(self.upper)
         if not set(value.dims).issubset(self.model.variables[self.name].dims):
             raise ValueError("Cannot assign new dimensions to existing variable.")
-        self.model.variables.upper[self.name] = value
+        self.data["upper"] = value
 
     @property
     def lower(self):
         """
         Get the lower bounds of the variables.
 
         The function raises an error in case no model is set as a
         reference.
         """
-        return self.model.variables.lower[self.name]
+        return self.data.lower
 
     @lower.setter
     @is_constant
     def lower(self, value):
         """
         Set the lower bounds of the variables.
 
         The function raises an error in case no model is set as a
         reference.
         """
         value = DataArray(value).broadcast_like(self.lower)
         if not set(value.dims).issubset(self.model.variables[self.name].dims):
             raise ValueError("Cannot assign new dimensions to existing variable.")
-        self.model.variables.lower[self.name] = value
+        self.data["lower"] = value
+
+    @property
+    @has_optimized_model
+    def solution(self):
+        """
+        Get the optimal values of the variable.
+
+        The function raises an error in case no model is set as a
+        reference or the model is not optimized.
+        """
+        return self.data["solution"]
+
+    @solution.setter
+    def solution(self, value):
+        """
+        Set the optimal values of the variable.
+        """
+        value = DataArray(value).broadcast_like(self.labels)
+        self.data["solution"] = value
 
     @property
     @has_optimized_model
     def sol(self):
         """
         Get the optimal values of the variable.
 
         The function raises an error in case no model is set as a
         reference or the model is not optimized.
         """
-        if self.model.status != "ok":
-            raise AttributeError("Underlying model not optimized.")
-        return self.model.solution[self.name]
+        warn(
+            "`Variable.sol` is deprecated. Use `Variable.solution` instead.",
+            DeprecationWarning,
+        )
+        return self.solution
+
+    @property
+    def flat(self):
+        """
+        Convert the variable to a pandas DataFrame.
+
+        The resulting DataFrame represents a long table format of the variable
+        with columns `labels`, `lower`, `upper` which are not masked.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+        """
+        ds = self.data
+        if not ds.sizes:
+            # fallback for weird error raised due to missing index
+            df = pd.DataFrame({k: ds[k].item() for k in ds}, index=[0])
+        else:
+            df = ds.to_dataframe()
+        df = df[df.labels != -1]
+
+        any_nan = df.isna().any()
+        if any_nan.any():
+            fields = ", ".join("`" + df.columns[any_nan] + "`")
+            raise ValueError(
+                f"Variable `{self.name}` contains nan's in field(s) {fields}"
+            )
+        return df
 
     def sum(self, dims=None):
         """
         Sum the variables over all or a subset of dimensions.
 
         This stack all terms of the dimensions, that are summed over, together.
         The function works exactly in the same way as ``LinearExpression.sum()``.
@@ -649,18 +643,20 @@
             Keyword arguments passed to ``xarray.DataArray.where``
 
         Returns
         -------
         linopy.Variable
         """
         if isinstance(other, Variable):
-            other = other.labels
+            other = other.data
         elif isinstance(other, ScalarVariable):
-            other = other.label
-        return self.__class__(self.labels.where(cond, other, **kwargs), self.model)
+            other = {"labels": other.label, "lower": other.lower, "upper": other.upper}
+        return self.__class__(
+            self.data.where(cond, other, **kwargs), self.model, self.name
+        )
 
     def ffill(self, dim, limit=None):
         """
         Forward fill the variable along a dimension.
 
         This operation call ``xarray.DataArray.ffill`` but ensures preserving
         the linopy.Variable type.
@@ -672,21 +668,22 @@
         limit : int, optional
             Maximum number of consecutive NaN values to forward fill. Must be greater than or equal to 0.
 
         Returns
         -------
         linopy.Variable
         """
-        labels = (
-            self.labels.where(self.labels != -1)
-            .ffill(dim, limit=limit)
-            .fillna(-1)
-            .astype(int)
+        data = (
+            self.data.where(self.labels != -1)
+            # .ffill(dim, limit=limit)
+            # breaks with Dataset.ffill, use map instead
+            .map(DataArray.ffill, dim=dim, limit=limit).fillna(self.fill_value)
         )
-        return self.__class__(labels, self.model)
+        data = data.assign(labels=data.labels.astype(int))
+        return self.__class__(data, self.model, self.name)
 
     def bfill(self, dim, limit=None):
         """
         Backward fill the variable along a dimension.
 
         This operation call ``xarray.DataArray.bfill`` but ensures preserving
         the linopy.Variable type.
@@ -698,77 +695,65 @@
         limit : int, optional
             Maximum number of consecutive NaN values to backward fill. Must be greater than or equal to 0.
 
         Returns
         -------
         linopy.Variable
         """
-        labels = (
-            self.labels.where(self.labels != -1)
-            .bfill(dim, limit=limit)
-            .fillna(-1)
-            .astype(int)
+        data = (
+            self.data.where(self.labels != -1)
+            # .bfill(dim, limit=limit)
+            # breaks with Dataset.bfill, use map instead
+            .map(DataArray.bfill, dim=dim, limit=limit).fillna(self.fill_value)
         )
-        return self.__class__(labels, self.model)
+        data = data.assign(labels=data.labels.astype(int))
+        return self.__class__(data, self.model, self.name)
 
     def sanitize(self):
         """
         Sanitize variable by ensuring int dtype with fill value of -1.
 
         Returns
         -------
         linopy.Variable
         """
         if issubdtype(self.labels.dtype, floating):
-            return self.__class__(self.labels.fillna(-1).astype(int), self.model)
+            data = self.data.assign(labels=self.labels.fillna(-1).astype(int))
+            return self.__class__(data, self.model, self.name)
         return self
 
     def equals(self, other):
         return self.labels.equals(_var_unwrap(other))
 
     # Wrapped function which would convert variable to dataarray
-    assign_attrs = varwrap(DataArray.assign_attrs)
-
-    assign_coords = varwrap(DataArray.assign_coords)
-
-    broadcast_like = varwrap(DataArray.broadcast_like)
-
-    compute = varwrap(DataArray.compute)
+    assign_attrs = varwrap(Dataset.assign_attrs)
 
-    drop = varwrap(DataArray.drop)
+    assign_coords = varwrap(Dataset.assign_coords)
 
-    drop_sel = varwrap(DataArray.drop_sel)
+    broadcast_like = varwrap(Dataset.broadcast_like)
 
-    drop_isel = varwrap(DataArray.drop_isel)
+    compute = varwrap(Dataset.compute)
 
-    fillna = varwrap(DataArray.fillna)
+    # drop = varwrap(Dataset.drop)
 
-    sel = varwrap(DataArray.sel)
+    drop_sel = varwrap(Dataset.drop_sel)
 
-    isel = varwrap(DataArray.isel)
+    drop_isel = varwrap(Dataset.drop_isel)
 
-    shift = varwrap(DataArray.shift, fill_value=-1)
+    fillna = varwrap(Dataset.fillna)
 
-    rename = varwrap(DataArray.rename)
+    sel = varwrap(Dataset.sel)
 
-    roll = varwrap(DataArray.roll)
+    isel = varwrap(Dataset.isel)
 
+    shift = varwrap(Dataset.shift, fill_value=_fill_value)
 
-class _LocIndexer:
-    __slots__ = ("variable",)
+    rename = varwrap(Dataset.rename)
 
-    def __init__(self, variable: Variable):
-        self.variable = variable
-
-    def __getitem__(self, key) -> DataArray:
-        if not utils.is_dict_like(key):
-            # expand the indexer so we can handle Ellipsis
-            labels = indexing.expanded_indexer(key, self.variable.ndim)
-            key = dict(zip(self.variable.dims, labels))
-        return self.variable.sel(key)
+    roll = varwrap(Dataset.roll)
 
 
 @dataclass(repr=False)
 @forward_as_properties(
     labels=[
         "attrs",
         "coords",
@@ -777,135 +762,147 @@
     ]
 )
 class Variables:
     """
     A variables container used for storing multiple variable arrays.
     """
 
-    labels: Dataset = field(default_factory=Dataset)
-    lower: Dataset = field(default_factory=Dataset)
-    upper: Dataset = field(default_factory=Dataset)
-    blocks: Dataset = field(default_factory=Dataset)
-    ranges: Dataset = field(default_factory=Dataset)
+    data: Dict[str, Variable] = field(default_factory=dict)
     model: Any = None  # Model is not defined due to circular imports
 
     dataset_attrs = ["labels", "lower", "upper"]
     dataset_names = ["Labels", "Lower bounds", "Upper bounds"]
 
     def __getitem__(
         self, names: Union[str, Sequence[str]]
     ) -> Union[Variable, "Variables"]:
         if isinstance(names, str):
-            return Variable(self.labels[names], self.model)
+            return self.data[names]
 
-        return self.__class__(
-            self.labels[names], self.lower[names], self.upper[names], self.model
-        )
+        return self.__class__({name: self.data[name] for name in names}, self.model)
+
+    def __getattr__(self, name: str):
+        # If name is an attribute of self (including methods and properties), return that
+        if name in self.data:
+            return self.data[name]
+        else:
+            raise AttributeError(
+                f"Variables has no attribute `{name}` or the attribute is not accessible / raises an error."
+            )
 
     def __repr__(self):
         """
         Return a string representation of the linopy model.
         """
         r = "linopy.model.Variables"
         line = "-" * len(r)
-        r += f"\n{line}\n\n"
+        r += f"\n{line}\n"
 
-        labelprint = self.labels.__repr__()
-        coordspattern = r"(?s)(?<=\<xarray\.Dataset\>\n).*?(?=Data variables:)"
-        r += re.search(coordspattern, labelprint).group()
-        r += "Variables:\n"
-        for name in self.labels:
-            r += f"  *  {name} ({', '.join(self.labels[name].coords)})\n"
+        for name, ds in self.items():
+            coords = " (" + ", ".join(ds.coords) + ")" if ds.coords else ""
+            r += f" * {name}{coords}\n"
+        if not len(list(self)):
+            r += "<empty>\n"
         return r
 
+    def __len__(self):
+        return self.data.__len__()
+
     def __iter__(self):
-        return self.labels.__iter__()
+        return self.data.__iter__()
 
-    _merge_inplace = _merge_inplace
+    def items(self):
+        return self.data.items()
 
     def _ipython_key_completions_(self):
         """
         Provide method for the key-autocompletions in IPython.
 
         See
         http://ipython.readthedocs.io/en/stable/config/integrating.html#tab-completion
         For the details.
         """
         return list(self)
 
-    def add(
-        self,
-        name,
-        labels: DataArray,
-        lower: DataArray,
-        upper: DataArray,
-        start=None,
-        end=None,
-    ):
+    def add(self, variable):
         """
-        Add variable `name`.
+        Add a variable to the variables container.
         """
-        self._merge_inplace("labels", labels, name, fill_value=-1)
-        self._merge_inplace("lower", lower, name, fill_value=-inf)
-        self._merge_inplace("upper", upper, name, fill_value=inf)
-        start = start or int(labels.min())
-        end = end or int(labels.max())
-        self.ranges[name] = DataArray([start, end], dims=["_start_stop"])
+        self.data[variable.name] = variable
 
     def remove(self, name):
         """
         Remove variable `name` from the variables.
         """
-        for attr in self.dataset_attrs:
-            ds = getattr(self, attr)
-            if name in ds:
-                setattr(self, attr, ds.drop_vars(name))
+        self.data.pop(name)
 
     @property
-    def nvars(self):
+    def labels(self):
+        """
+        Get the labels of all variables.
         """
-        Get the number all variables which were at some point added to the
-        model.
+        return save_join(*[v.labels.rename(k) for k, v in self.items()])
 
-        These also include variables with missing labels.
+    @property
+    def lower(self):
+        """
+        Get the lower bounds of all variables.
         """
-        return self.ravel("labels", filter_missings=True).shape[0]
+        return save_join(*[v.lower.rename(k) for k, v in self.items()])
 
     @property
-    def _binary_variables(self):
-        return [v for v in self if self[v].attrs["binary"]]
+    def upper(self):
+        """
+        Get the upper bounds of all variables.
+        """
+        return save_join(*[v.upper.rename(k) for k, v in self.items()])
 
     @property
-    def _non_binary_variables(self):
-        return [v for v in self if not self[v].attrs["binary"]]
+    def nvars(self):
+        """
+        Get the number all variables effectively used by the model.
+
+        These excludes variables with missing labels.
+        """
+        return len(self.flat.labels.unique())
 
     @property
     def binaries(self):
         """
         Get all binary variables.
         """
-        return self[self._binary_variables]
+        keys = [v for v in self if self[v].attrs["binary"]]
+        return self[keys]
 
     @property
-    def non_binaries(self):
+    def integers(self):
         """
-        Get all non-binary variables.
+        Get all integers variables.
         """
-        return self[self._non_binary_variables]
+        keys = [v for v in self if self[v].attrs["integer"]]
+        return self[keys]
 
     @property
-    def _integer_variables(self):
-        return [v for v in self if self[v].attrs["integer"]]
+    def continuous(self):
+        """
+        Get all continuous variables.
+        """
+        keys = [
+            v
+            for v in self
+            if not self[v].attrs["integer"] and not self[v].attrs["binary"]
+        ]
+        return self[keys]
 
     @property
-    def integers(self):
+    def solution(self):
         """
-        Get all integers variables.
+        Get the solution of variables.
         """
-        return self[self._integer_variables]
+        return save_join(*[v.solution.rename(k) for k, v in self.items()])
 
     def get_name_by_label(self, label):
         """
         Get the variable name of the variable containing the passed label.
 
         Parameters
         ----------
@@ -919,55 +916,62 @@
             If label is not contained by any variable.
 
         Returns
         -------
         name : str
             Name of the containing variable.
         """
-        if not isinstance(label, (float, int)) or label < 0:
+        if not isinstance(label, (float, int, np.integer)) or label < 0:
             raise ValueError("Label must be a positive number.")
         for name, labels in self.labels.items():
             if label in labels:
                 return name
         raise ValueError(f"No variable found containing the label {label}.")
 
     def get_label_range(self, name: str):
         """
         Get starting and ending label for a variable.
         """
-        return list(self.ranges[name].values)
+        return self[name].range
 
     def get_label_position(self, values):
         """
         Get tuple of name and coordinate for variable labels.
         """
-        coords = []
-        return_list = True
-        if not isinstance(values, Iterable):
-            values = [values]
-            return_list = False
-
-        for value in values:
-            for name, labels in self.labels.items():
-                start, stop = self.get_label_range(name)
+
+        def find_single(value):
+            if value == -1:
+                return None, None
+            for name, var in self.items():
+                labels = var.labels
+                start, stop = var.range
 
                 if value >= start and value < stop:
                     index = np.unravel_index(value - start, labels.shape)
 
                     # Extract the coordinates from the indices
                     coord = {
                         dim: labels.indexes[dim][i]
                         for dim, i in zip(labels.dims, index)
                     }
 
                     # Add the name of the DataArray and the coordinates to the result list
-                    coords.append((name, coord))
+                    return name, coord
 
-        return coords if return_list else coords[0]
+        ndim = np.array(values).ndim
+        if ndim == 0:
+            return find_single(values)
+        elif ndim == 1:
+            return [find_single(v) for v in values]
+        elif ndim == 2:
+            return [[find_single(v) for v in _] for _ in values.T]
+        else:
+            raise ValueError("Array's with more than two dimensions is not supported")
 
+    @deprecated("0.2", details="Use `to_dataframe` or `flat` instead.")
     def iter_ravel(self, key, filter_missings=False):
         """
         Create an generator which iterates over all arrays in `key` and
         flattens them.
 
         Parameters
         ----------
@@ -980,37 +984,34 @@
             When enabled, the data is loaded into memory. The default is False.
 
 
         Yields
         ------
         flat : np.array/dask.array
         """
-        if isinstance(key, str):
-            ds = getattr(self, key)
-        elif isinstance(key, Dataset):
-            ds = key
-        else:
-            raise TypeError("Argument `key` must be of type string or xarray.Dataset")
 
-        for name, labels in self.labels.items():
-            broadcasted = ds[name].broadcast_like(labels)
+        for name, variable in self.items():
+            labels = variable.labels
+            ds = variable.data[key]
+            broadcasted = ds.broadcast_like(labels)
             if labels.chunks is not None:
                 broadcasted = broadcasted.chunk(labels.chunks)
 
             if filter_missings:
                 flat = np.ravel(broadcasted)
                 flat = flat[np.ravel(labels) != -1]
                 if pd.isna(flat).any():
                     ds_name = self.dataset_names[self.dataset_attrs.index(key)]
                     err = f"{ds_name} of variable '{name}' contains nan's."
                     raise ValueError(err)
             else:
                 flat = broadcasted.data.ravel()
             yield flat
 
+    @deprecated("0.2", details="Use `to_dataframe` or `flat` instead.")
     def ravel(self, key, filter_missings=False, compute=True):
         """
         Ravel and concate all arrays in `key` while aligning to
         `broadcast_like`.
 
         Parameters
         ----------
@@ -1028,41 +1029,60 @@
 
         Returns
         -------
         flat
             One dimensional data with all values in `key`.
         """
         res = np.concatenate(list(self.iter_ravel(key, filter_missings)))
-        if compute:
-            return dask.compute(res)[0]
-        else:
-            return res
+        return dask.compute(res)[0] if compute else res
 
-    def get_blocks(self, blocks: DataArray):
+    @property
+    def flat(self) -> pd.DataFrame:
+        """
+        Convert all variables to a single pandas Dataframe.
+
+        The resulting dataframe is a long format of the variables
+        with columns `labels`, `lower`, 'upper` and `mask`.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        df = pd.concat([self[k].flat for k in self], ignore_index=True)
+        unique_labels = df.labels.unique()
+        map_labels = pd.Series(np.arange(len(unique_labels)), index=unique_labels)
+        df["key"] = df.labels.map(map_labels)
+        return df
+
+    def reset_solution(self):
+        """
+        Reset the stored solution of variables.
+        """
+        for k, v in self.items():
+            if "solution" in v:
+                v._data = v.data.drop_vars("solution")
+
+    def set_blocks(self, blocks: DataArray):
         """
         Get a dataset of same shape as variables.labels indicating the blocks.
         """
         dim = blocks.dims[0]
         assert dim in self.labels.dims, "Block dimension not in variables."
 
-        block_map = zeros_like(self.labels, dtype=blocks.dtype)
-        for name, variable in self.labels.items():
+        for name, variable in self.items():
             if dim in variable.dims:
-                block_map[name] = blocks.broadcast_like(variable)
-        return block_map.where(self.labels != -1, -1)
+                variable.data["blocks"] = blocks.broadcast_like(variable.labels)
 
-    def blocks_to_blockmap(self, block_map, dtype=np.int8):
+    def get_blockmap(self, dtype=np.int8):
         """
         Get a one-dimensional array mapping the variables to blocks.
         """
-        # non-assigned variables are assumed to be masked, insert -1
+        df = self.flat
         res = np.full(self.model._xCounter + 1, -1, dtype=dtype)
-        for name, labels in self.labels.items():
-            res[np.ravel(labels)] = np.ravel(block_map[name])
-        res[-1] = -1
+        res[df.labels] = df.blocks
         return res
 
 
 class ScalarVariable:
     """
     A scalar variable container.
 
@@ -1088,14 +1108,30 @@
     def label(self):
         """
         Get the label of the variable.
         """
         return self._label
 
     @property
+    def lower(self):
+        """
+        Get the lower bound of the variable.
+        """
+        name, position = self.model.variables.get_label_position(self.label)
+        return self.model.variables[name].lower.sel(position).item()
+
+    @property
+    def upper(self):
+        """
+        Get the upper bound of the variable.
+        """
+        name, position = self.model.variables.get_label_position(self.label)
+        return self.model.variables[name].upper.sel(position).item()
+
+    @property
     def model(self):
         """
         Get the model to which the variable belongs.
         """
         return self._model
 
     def to_scalar_linexpr(self, coeff=1):
@@ -1110,18 +1146,15 @@
         return self.to_scalar_linexpr(-1)
 
     def __add__(self, other):
         return self.to_scalar_linexpr(1) + other
 
     def __radd__(self, other):
         # This is needed for using python's sum function
-        if other == 0:
-            return self
-        else:
-            return NotImplemented
+        return self if other == 0 else NotImplemented
 
     def __sub__(self, other):
         return self.to_scalar_linexpr(1) - other
 
     def __mul__(self, coeff):
         return self.to_scalar_linexpr(coeff)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linopy-0.1.5/linopy.egg-info/PKG-INFO` & `linopy-0.2/linopy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.1.5
+Version: 0.2
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
-License: GPLv3
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: solvers
 License-File: LICENSE.txt
 
-# linopy: Linear optimization with N-D labeled variables
+# linopy: Linear optimization with N-dimensional labeled variables
 
-[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
+[![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License](https://img.shields.io/pypi/l/linopy.svg)](LICENSE.txt) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
 
-**linopy** is an open-source python package that facilitates **linear or mixed-integer optimisation** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and linear problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). The project aims to make linear programming in python easy, highly-flexible and performant.
+**linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) contnuous or binary variables with **coordinates**, e.g. time, consumers, etc.
@@ -45,14 +45,21 @@
 
 So far **linopy** is available on the PyPI repository
 
 ```bash
 pip install linopy
 ```
 
+or on conda-forge
+
+```bash
+conda install -c conda-forge linopy
+```
+
+
 ## Supported solvers
 
 **linopy** supports the following solvers
 
 * [Cbc](https://projects.coin-or.org/Cbc)
 * [GLPK](https://www.gnu.org/software/glpk/)
 * [HiGHS](https://www.maths.ed.ac.uk/hall/HiGHS/)
@@ -65,8 +72,8 @@
 
 # License
 
 Copyright 2021 Fabian Hofmann
 
 
 
-This package is published under license GNU Public License GPLv3
+This package is published under MIT license. See [LICENSE.txt](LICENSE.txt) for details.
```

### Comparing `linopy-0.1.5/linopy.egg-info/SOURCES.txt` & `linopy-0.2/linopy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.coverage
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CONTRIBUTING.md
 LICENSE.txt
 README.md
@@ -106,22 +107,24 @@
 linopy/variables.py
 linopy/version.py
 linopy.egg-info/PKG-INFO
 linopy.egg-info/SOURCES.txt
 linopy.egg-info/dependency_links.txt
 linopy.egg-info/requires.txt
 linopy.egg-info/top_level.txt
+test/test_common.py
 test/test_constraint.py
 test/test_constraints.py
 test/test_inconsistency_checks.py
 test/test_io.py
 test/test_linear_expression.py
 test/test_matrices.py
 test/test_model.py
 test/test_optimization.py
 test/test_options.py
+test/test_quadratic_expression.py
 test/test_repr.py
 test/test_scalar_constraint.py
 test/test_scalar_linear_expression.py
 test/test_variable.py
 test/test_variable_assignment.py
 test/test_variables.py
```

### Comparing `linopy-0.1.5/setup.py` & `linopy-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     name="linopy",
     author="Fabian Hofmann",
     author_email="hofmann@fias.uni-frankfurt.de",
     description="Linear optimization with N-D labeled arrays in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PyPSA/linopy",
-    license="GPLv3",
+    license="MIT",
     packages=find_packages(exclude=["doc", "test"]),
     include_package_data=True,
     python_requires="~=3.8",
     install_requires=[
         "numpy",
         "scipy",
         "bottleneck",
```

### Comparing `linopy-0.1.5/test/test_constraint.py` & `linopy-0.2/test/test_constraint.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from linopy import EQUAL, GREATER_EQUAL, LESS_EQUAL, LinearExpression, Model
 from linopy.constants import (
     long_EQUAL,
     short_GREATER_EQUAL,
     short_LESS_EQUAL,
     sign_replace_dict,
 )
-from linopy.constraints import AnonymousConstraint
+from linopy.constraints import Constraint
 
 
 @pytest.fixture
 def m():
     m = Model()
     x = m.add_variables(coords=[pd.RangeIndex(10, name="first")], name="x")
     m.add_variables(coords=[pd.Index([1, 2, 3], name="second")], name="y")
@@ -69,95 +69,127 @@
     assert isinstance(m.constraints[["c"]], linopy.constraints.Constraints)
 
 
 def test_anonymous_constraint_from_linear_expression_le(x, y):
     expr = 10 * x + y
     con = expr <= 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == LESS_EQUAL
+    assert (con.sign == LESS_EQUAL).all()
     assert (con.rhs == 10).all()
 
 
 def test_anonymous_constraint_from_linear_expression_ge(x, y):
     expr = 10 * x + y
     con = expr >= 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == GREATER_EQUAL
+    assert (con.sign == GREATER_EQUAL).all()
     assert (con.rhs == 10).all()
 
 
 def test_anonymous_constraint_from_linear_expression_eq(x, y):
     expr = 10 * x + y
     con = expr == 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == EQUAL
+    assert (con.sign == EQUAL).all()
     assert (con.rhs == 10).all()
 
 
 def test_anonymous_constraint_from_variable_le(x):
     con = x <= 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == LESS_EQUAL
+    assert (con.sign == LESS_EQUAL).all()
     assert (con.rhs == 10).all()
 
 
 def test_anonymous_constraint_from_variable_ge(x):
     con = x >= 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == GREATER_EQUAL
+    assert (con.sign == GREATER_EQUAL).all()
     assert (con.rhs == 10).all()
 
 
 def test_anonymous_constraint_from_variable_eq(x):
     con = x == 10
     assert isinstance(con.lhs, LinearExpression)
-    assert con.sign.item() == EQUAL
+    assert (con.sign == EQUAL).all()
     assert (con.rhs == 10).all()
 
 
-def test_anonymous_constraint_from_linear_expression_fail(x, y):
+def test_anonymous_constraint_with_variable_on_rhs(x, y):
     expr = 10 * x + y
-    with pytest.raises(TypeError):
-        expr == x
+    con = expr == x
+    assert isinstance(con.lhs, LinearExpression)
+    assert (con.sign == EQUAL).all()
+    assert (con.rhs == 0).all()
+
+
+def test_anonymous_constraint_with_constant_on_lhs(x, y):
+    expr = 10 * x + y + 10
+    con = expr == 0
+    assert isinstance(con.lhs, LinearExpression)
+    assert (con.lhs.const == 0).all()
+    assert (con.sign == EQUAL).all()
+    assert (con.rhs == -10).all()
+
+
+def test_anonymous_constraint_with_constant_on_rhs(x, y):
+    expr = 10 * x + y
+    con = expr == 10
+    assert isinstance(con.lhs, LinearExpression)
+    assert (con.sign == EQUAL).all()
+    assert (con.rhs == 10).all()
+
+
+def test_anonymous_constraint_with_expression_on_both_sides(x, y):
+    expr = 10 * x + y + 10
+    con = expr == expr
+    assert isinstance(con.lhs, LinearExpression)
+    assert con.lhs.nterm == 4  # are stacked on top of each other
+    assert (con.coeffs.sum(con.term_dim) == 0).all()
+    assert (con.sign == EQUAL).all()
+    assert (con.rhs == 0).all()
 
 
-def test_anonymous_scalar_constraint_from_linear_expression_fail(x, y):
+def test_anonymous_scalar_constraint_with_scalar_variable_on_rhs(x, y):
     expr = 10 * x[0] + y[1]
     with pytest.raises(TypeError):
-        expr == x[0]
+        con = expr == x[0]
+        # assert isinstance(con.lhs, LinearExpression)
+        # assert (con.sign == EQUAL).all()
+        # assert (con.rhs == 0).all()
 
 
 def test_anonymous_constraint_sel(x, y):
     expr = 10 * x + y
     con = expr <= 10
-    assert isinstance(con.sel(first=[1, 2]), AnonymousConstraint)
+    assert isinstance(con.sel(first=[1, 2]), Constraint)
 
 
 def test_constraint_from_rule(m, x, y):
     def bound(m, i, j):
         if i % 2:
             return (i - 1) * x[i - 1] + y[j] >= 0
         else:
             return i * x[i] >= 0
 
     coords = [x.coords["first"], y.coords["second"]]
-    con = AnonymousConstraint.from_rule(m, bound, coords)
-    assert isinstance(con, AnonymousConstraint)
+    con = Constraint.from_rule(m, bound, coords)
+    assert isinstance(con, Constraint)
     assert con.lhs.nterm == 2
     repr(con)  # test repr
 
 
 def test_constraint_from_rule_with_none_return(m, x, y):
     def bound(m, i, j):
         if i % 2:
             return i * x[i] + y[j] >= 0
 
     coords = [x.coords["first"], y.coords["second"]]
-    con = AnonymousConstraint.from_rule(m, bound, coords)
-    assert isinstance(con, AnonymousConstraint)
+    con = Constraint.from_rule(m, bound, coords)
+    assert isinstance(con, Constraint)
     assert con.lhs.nterm == 2
     assert (con.lhs.vars.loc[0, :] == -1).all()
     assert (con.lhs.vars.loc[1, :] != -1).all()
     repr(con)  # test repr
 
 
 def test_constraint_vars_getter(c, x):
@@ -165,19 +197,19 @@
 
 
 def test_constraint_coeffs_getter(c):
     assert (c.coeffs == 1).all()
 
 
 def test_constraint_sign_getter(c):
-    assert c.sign.item() == GREATER_EQUAL
+    assert (c.sign == GREATER_EQUAL).all()
 
 
 def test_constraint_rhs_getter(c):
-    assert c.rhs.item() == 0
+    assert (c.rhs == 0).all()
 
 
 def test_constraint_vars_setter(c, x):
     c.vars = x
     assert_equal(c.vars, x.labels)
 
 
@@ -199,61 +231,82 @@
 def test_constraint_lhs_setter(c, x, y):
     c.lhs = x + y
     assert c.lhs.nterm == 2
     assert c.vars.notnull().all().item()
     assert c.coeffs.notnull().all().item()
 
 
-def test_constraint_lhs_setter_invalid(c):
-    # Test that assigning lhs with other type that LinearExpression raises TypeError
-    with pytest.raises(TypeError):
-        c.lhs = x
+def test_constraint_lhs_setter_with_variable(c, x):
+    c.lhs = x
+    assert c.lhs.nterm == 1
+
+
+def test_constraint_lhs_setter_with_constant(c):
+    c.lhs = 10
+    assert (c.rhs == -10).all()
+    assert c.lhs.nterm == 0
 
 
 def test_constraint_sign_setter(c):
     c.sign = EQUAL
-    assert c.sign.item() == EQUAL
+    assert (c.sign == EQUAL).all()
 
 
 def test_constraint_sign_setter_alternative(c):
     c.sign = long_EQUAL
-    assert c.sign.item() == EQUAL
+    assert (c.sign == EQUAL).all()
 
 
 def test_constraint_sign_setter_invalid(c):
     # Test that assigning lhs with other type that LinearExpression raises TypeError
     with pytest.raises(ValueError):
         c.sign = "asd"
 
 
 def test_constraint_rhs_setter(c):
     c.rhs = 2
-    assert c.rhs.item() == 2
+    assert (c.rhs == 2).all()
 
 
-def test_constraint_rhs_setter_invalid(c, x):
-    # Test that assigning a variable or linear expression to the rhs property raises a TypeError
-    with pytest.raises(TypeError):
-        c.rhs = x
+def test_constraint_rhs_setter_with_variable(c, x):
+    c.rhs = x
+    assert (c.rhs == 0).all()
+    assert (c.coeffs.isel({c.term_dim: -1}) == -1).all()
+    assert c.lhs.nterm == 2
 
-    with pytest.raises(TypeError):
-        c.rhs = x + y
+
+def test_constraint_rhs_setter_with_expression(c, x, y):
+    c.rhs = x + y
+    assert (c.rhs == 0).all()
+    assert (c.coeffs.isel({c.term_dim: -1}) == -1).all()
+    assert c.lhs.nterm == 3
+
+
+def test_constraint_rhs_setter_with_expression_and_constant(c, x):
+    c.rhs = x + 1
+    assert (c.rhs == 1).all()
+    assert (c.coeffs.sum(c.term_dim) == 0).all()
+    assert c.lhs.nterm == 2
 
 
 def test_constraint_labels_setter_invalid(c):
     # Test that assigning labels raises FrozenInstanceError
     with pytest.raises(AttributeError):
         c.labels = c.labels
 
 
 def test_constraint_sel(c):
     assert isinstance(c.sel(first=[1, 2]), linopy.constraints.Constraint)
     assert isinstance(c.isel(first=[1, 2]), linopy.constraints.Constraint)
 
 
+def test_constraint_flat(c):
+    assert isinstance(c.flat, pd.DataFrame)
+
+
 def test_constraint_assignment_with_anonymous_constraints(m, x, y):
     m.add_constraints(x + y == 0, name="c2")
     assert m.constraints["c2"].vars.notnull().all()
     assert m.constraints["c2"].coeffs.notnull().all()
 
 
 def test_constraint_assignment_sanitize_zeros(m, x, y):
@@ -264,37 +317,37 @@
 
 
 def test_constraint_assignment_with_args(m, x, y):
     lhs = x + y
     m.add_constraints(lhs, EQUAL, 0, name="c2")
     assert m.constraints["c2"].vars.notnull().all()
     assert m.constraints["c2"].coeffs.notnull().all()
-    assert m.constraints["c2"].sign == EQUAL
-    assert m.constraints["c2"].rhs == 0
+    assert (m.constraints["c2"].sign == EQUAL).all()
+    assert (m.constraints["c2"].rhs == 0).all()
 
 
 def test_constraint_assignment_with_args_valid_sign(m, x, y):
     lhs = x + y
     for i, sign in enumerate([EQUAL, GREATER_EQUAL, LESS_EQUAL]):
         m.add_constraints(lhs, sign, 0, name=f"c{i}")
         assert m.constraints[f"c{i}"].vars.notnull().all()
         assert m.constraints[f"c{i}"].coeffs.notnull().all()
-        assert m.constraints[f"c{i}"].sign == sign
-        assert m.constraints[f"c{i}"].rhs == 0
+        assert (m.constraints[f"c{i}"].sign == sign).all()
+        assert (m.constraints[f"c{i}"].rhs == 0).all()
 
 
 def test_constraint_assignment_with_args_alternative_sign(m, x, y):
     lhs = x + y
 
     for i, sign in enumerate([long_EQUAL, short_GREATER_EQUAL, short_LESS_EQUAL]):
         m.add_constraints(lhs, sign, 0, name=f"c{i}")
         assert m.constraints[f"c{i}"].vars.notnull().all()
         assert m.constraints[f"c{i}"].coeffs.notnull().all()
-        assert m.constraints[f"c{i}"].sign == sign_replace_dict[sign]
-        assert m.constraints[f"c{i}"].rhs == 0
+        assert (m.constraints[f"c{i}"].sign == sign_replace_dict[sign]).all()
+        assert (m.constraints[f"c{i}"].rhs == 0).all()
 
 
 def test_constraint_assignment_with_args_invalid_sign(m, x, y):
     lhs = x + y
     with pytest.raises(ValueError):
         m.add_constraints(lhs, ",", 0)
 
@@ -319,15 +372,15 @@
     m.add_variables()
     m.add_constraints(x, EQUAL, 0)
     A = m.constraints.to_matrix(filter_missings=True)
     assert A.shape == (5, 6)
     assert A.shape == (m.ncons, m.nvars)
 
     A = m.constraints.to_matrix(filter_missings=False)
-    assert A.shape == (m._cCounter, m._xCounter)
+    assert A.shape == m.shape
 
 
 def test_constraint_matrix_masked_constraints():
     """
     Test constraint matrix with missing constraints.
     """
     # now with missing variables
@@ -337,15 +390,15 @@
     m.add_variables()
     m.add_constraints(x, EQUAL, 0, mask=mask)
     A = m.constraints.to_matrix(filter_missings=True)
     assert A.shape == (5, 11)
     assert A.shape == (m.ncons, m.nvars)
 
     A = m.constraints.to_matrix(filter_missings=False)
-    assert A.shape == (m._cCounter, m._xCounter)
+    assert A.shape == m.shape
 
 
 def test_constraint_matrix_masked_constraints_and_variables():
     """
     Test constraint matrix with missing constraints.
     """
     # now with missing variables
@@ -355,15 +408,15 @@
     m.add_variables()
     m.add_constraints(x, EQUAL, 0, mask=mask)
     A = m.constraints.to_matrix(filter_missings=True)
     assert A.shape == (5, 6)
     assert A.shape == (m.ncons, m.nvars)
 
     A = m.constraints.to_matrix(filter_missings=False)
-    assert A.shape == (m._cCounter, m._xCounter)
+    assert A.shape == m.shape
 
 
 def test_get_name_by_label():
     m = Model()
     x = m.add_variables(coords=[range(10)])
     y = m.add_variables(coords=[range(10)])
```

### Comparing `linopy-0.1.5/test/test_constraints.py` & `linopy-0.2/test/test_constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,40 @@
 import dask
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
 
 from linopy import EQUAL, GREATER_EQUAL, LESS_EQUAL, Model
+from linopy.testing import assert_conequal
 
 # Test model functions
 
 
 def test_constraint_assignment():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
     x = m.add_variables(lower, upper, name="x")
     y = m.add_variables(name="y")
 
-    m.add_constraints(1 * x + 10 * y, EQUAL, 0)
+    con0 = m.add_constraints(1 * x + 10 * y, EQUAL, 0)
 
     for attr in m.constraints.dataset_attrs:
         assert "con0" in getattr(m.constraints, attr)
 
     assert m.constraints.labels.con0.shape == (10, 10)
     assert m.constraints.labels.con0.dtype == int
     assert m.constraints.coeffs.con0.dtype in (int, float)
     assert m.constraints.vars.con0.dtype in (int, float)
     assert m.constraints.rhs.con0.dtype in (int, float)
 
+    assert_conequal(m.constraints.con0, con0)
+
 
 def test_anonymous_constraint_assignment():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
     x = m.add_variables(lower, upper, name="x")
@@ -92,22 +95,18 @@
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
     x = m.add_variables(lower, upper, name="x")
     y = m.add_variables(name="y")
 
     m.add_constraints(1 * x + 10 * y, EQUAL, 0)
 
-    shuffled_coords = pd.Index([2, 1, 3, 4, 6, 5, 7, 9, 8, 0], name="first")
-    con = m.variables["x"].loc[shuffled_coords] <= 10
-    with pytest.warns(UserWarning):
-        con_shuffled = m.add_constraints(con, name="con_shuffled")
-
-    assert con_shuffled.indexes["dim_0"].equals(m.constraints["con0"].indexes["dim_0"])
-    # check if labels are monotonically increasing
-    assert np.all(np.diff(np.ravel(con_shuffled.labels)) > 0)
+    shuffled_coords = [2, 1, 3, 4, 6, 5, 7, 9, 8, 0]
+
+    con = x.loc[shuffled_coords] + y >= 10
+    assert (con.coords["dim_0"].values == shuffled_coords).all()
 
 
 def test_wrong_constraint_assignment_repeated():
     # repeated variable assignment is forbidden
     m = Model()
     x = m.add_variables()
     m.add_constraints(x, LESS_EQUAL, 0, name="con")
@@ -123,7 +122,27 @@
     x = m.add_variables(lower, upper)
     y = m.add_variables()
 
     mask = pd.Series([True] * 5 + [False] * 5)
     m.add_constraints(1 * x + 10 * y, EQUAL, 0, mask=mask)
     assert (m.constraints.labels.con0[0:5, :] != -1).all()
     assert (m.constraints.labels.con0[5:10, :] == -1).all()
+
+
+def test_constraints_flat():
+    m = Model()
+
+    lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
+    upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
+    x = m.add_variables(lower, upper)
+    y = m.add_variables()
+
+    assert isinstance(m.constraints.flat, pd.DataFrame)
+    assert m.constraints.flat.empty
+    assert m.constraints.to_matrix() is None
+
+    m.add_constraints(1 * x + 10 * y, EQUAL, 0)
+    m.add_constraints(1 * x + 10 * y, LESS_EQUAL, 0)
+    m.add_constraints(1 * x + 10 * y, GREATER_EQUAL, 0)
+
+    assert isinstance(m.constraints.flat, pd.DataFrame)
+    assert not m.constraints.flat.empty
```

### Comparing `linopy-0.1.5/test/test_inconsistency_checks.py` & `linopy-0.2/test/test_inconsistency_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     x = m.add_variables(lower=np.nan, name="x")
     y = m.add_variables(name="y")
 
     m.add_constraints(2 * x + 6 * y, GREATER_EQUAL, 10)
     m.add_constraints(4 * x + 2 * y, GREATER_EQUAL, 3)
 
     m.add_objective(2 * y + x)
+
     with pytest.raises(ValueError):
         m.solve()
 
 
 def test_nan_in_variable_upper():
     m = Model()
```

### Comparing `linopy-0.1.5/test/test_io.py` & `linopy-0.2/test/test_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import pandas as pd
 import pytest
 import xarray as xr
 from xarray.testing import assert_equal
 
 from linopy import LESS_EQUAL, Model, available_solvers, read_netcdf
-from linopy.io import int_to_str
 
 
 @pytest.fixture
 def m():
     m = Model()
 
     x = m.add_variables(4, pd.Series([8, 10]), name="x")
@@ -25,55 +24,37 @@
     m.add_constraints(x + y, LESS_EQUAL, 10)
 
     m.add_objective(2 * x + 3 * y)
 
     return m
 
 
-def test_str_arrays(m):
-    da = int_to_str(m.variables["x"].values)
-    assert da.dtype == object
-
-
-def test_str_arrays_chunked():
-    m = Model(chunk="auto")
-
-    m.add_variables(4, pd.Series([8, 10]))
-    y = m.add_variables(0, pd.DataFrame([[1, 2], [3, 4], [5, 6]]).T)
-
-    da = int_to_str(y.compute().values)
-    assert da.dtype == object
-
-
-def test_str_arrays_with_nans():
-    m = Model()
-
-    m.add_variables(4, pd.Series([8, 10]), name="x")
-    # now expand the second dimension, expanded values of x will be nan
-
-    with pytest.warns(UserWarning):
-        m.add_variables(0, pd.DataFrame([[1, 2]]), name="y")
-
-    assert m["y"].values[-1, -1] == -1
-
-    da = int_to_str(m["y"].values)
-    assert da.dtype == object
-
-
 def test_to_netcdf(m, tmp_path):
     fn = tmp_path / "test.nc"
     m.to_netcdf(fn)
     p = read_netcdf(fn)
 
     for k in m.scalar_attrs:
         if k != "objective_value":
             assert getattr(m, k) == getattr(p, k)
+
     for k in m.dataset_attrs:
         assert_equal(getattr(m, k), getattr(p, k))
 
+    assert set(m.variables) == set(p.variables)
+    assert set(m.constraints) == set(p.constraints)
+
+    for v in m.variables:
+        assert_equal(m.variables[v].data, p.variables[v].data)
+
+    for c in m.constraints:
+        assert_equal(m.constraints[c].data, p.constraints[c].data)
+
+    assert_equal(m.objective.data, p.objective.data)
+
 
 @pytest.mark.skipif("gurobi" not in available_solvers, reason="Gurobipy not installed")
 def test_to_file_lp(m, tmp_path):
     import gurobipy
 
     fn = tmp_path / "test.lp"
     m.to_file(fn)
@@ -108,21 +89,23 @@
 
 @pytest.mark.skipif("highs" not in available_solvers, reason="Highspy not installed")
 def test_to_highspy(m):
     m.to_highspy()
 
 
 def test_to_blocks(tmp_path):
+    # This is currently broken and due to time-constraints not possible to fix
     m = Model()
 
     lower = pd.Series(range(20))
     upper = pd.Series(range(30, 50))
     x = m.add_variables(lower, upper)
     y = m.add_variables(lower, upper)
 
     m.add_constraints(x + y, LESS_EQUAL, 10)
 
     m.add_objective(2 * x + 3 * y)
 
     m.blocks = xr.DataArray([1] * 10 + [2] * 10)
 
-    m.to_block_files(tmp_path)
+    with pytest.raises(ValueError):
+        m.to_block_files(tmp_path)
```

### Comparing `linopy-0.1.5/test/test_linear_expression.py` & `linopy-0.2/test/test_linear_expression.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
 from xarray.testing import assert_equal
 
 from linopy import LinearExpression, Model, merge
+from linopy.constants import TERM_DIM
 from linopy.testing import assert_linequal
 
 
 @pytest.fixture
 def m():
     m = Model()
 
@@ -69,43 +70,44 @@
 
     coeffs = xr.DataArray([1, 2], dims=["a"])
     vars = xr.DataArray([1, 2], dims=["a"])
     data = xr.Dataset({"coeffs": coeffs, "vars": vars})
     with pytest.raises(ValueError):
         LinearExpression(data, m)
 
-    coords = [pd.Index([0], name="a"), pd.Index([1, 2], name="_term")]
+    coords = [pd.Index([0], name="a"), pd.Index([1, 2], name=TERM_DIM)]
     coeffs = xr.DataArray(np.array([[1, 2]]), coords=coords)
     vars = xr.DataArray(np.array([[1, 2]]), coords=coords)
     data = xr.Dataset({"coeffs": coeffs, "vars": vars})
     with pytest.raises(ValueError):
         LinearExpression(data, None)
 
+
+def test_linexpr_with_data_without_coords(m):
     lhs = 1 * m["x"]
-    vars = xr.DataArray(lhs.vars.values, dims=["dim_0", "_term"])
-    coeffs = xr.DataArray(lhs.coeffs.values, dims=["dim_0", "_term"])
+    vars = xr.DataArray(lhs.vars.values, dims=["dim_0", TERM_DIM])
+    coeffs = xr.DataArray(lhs.coeffs.values, dims=["dim_0", TERM_DIM])
     data = xr.Dataset({"vars": vars, "coeffs": coeffs})
-    with pytest.raises(ValueError):
-        # test missing coords
-        LinearExpression(data, m)
+    expr = LinearExpression(data, m)
+    assert_linequal(expr, lhs)
 
 
 def test_repr(m):
     expr = m.linexpr((10, "x"), (1, "y"))
     expr.__repr__()
 
 
 def test_fill_value():
     isinstance(LinearExpression.fill_value, dict)
 
 
 def test_linexpr_with_scalars(m):
     expr = m.linexpr((10, "x"), (1, "y"))
     target = xr.DataArray(
-        [[10, 1], [10, 1]], coords={"dim_0": [0, 1]}, dims=["dim_0", "_term"]
+        [[10, 1], [10, 1]], coords={"dim_0": [0, 1]}, dims=["dim_0", TERM_DIM]
     )
     assert_equal(expr.coeffs, target)
 
 
 def test_linexpr_with_series(m, v):
     lhs = pd.Series(np.arange(20)), v
     expr = m.linexpr(lhs)
@@ -165,39 +167,35 @@
     assert_linequal(expr, m.linexpr((1, "x"), (-1, "y")))
 
     expr = -x - 8 * y
     assert isinstance(expr, LinearExpression)
     assert_linequal(expr, m.linexpr((-1, "x"), (-8, "y")))
 
 
-def test_linear_expression_multi_indexed(u):
-    expr = 3 * u + 1 * u
+def test_linear_expression_with_constant(m, x, y):
+    expr = x + 1
     assert isinstance(expr, LinearExpression)
+    assert (expr.const == 1).all()
 
+    expr = -x - 8 * y - 10
+    assert isinstance(expr, LinearExpression)
+    assert (expr.const == -10).all()
+    assert expr.nterm == 2
 
-def test_linear_expression_with_errors(m, x):
-    with pytest.raises(TypeError):
-        x.to_linexpr(x)
-
-    with pytest.raises(TypeError):
-        x + 10
 
-    with pytest.raises(TypeError):
-        x - 10
+def test_linear_expression_multi_indexed(u):
+    expr = 3 * u + 1 * u
+    assert isinstance(expr, LinearExpression)
 
-    with pytest.raises(TypeError):
-        x * x
 
+def test_linear_expression_with_errors(m, x):
     with pytest.raises(TypeError):
         x / x
 
     with pytest.raises(TypeError):
-        x * (1 * x)
-
-    with pytest.raises(TypeError):
         x / (1 * x)
 
     with pytest.raises(TypeError):
         m.linexpr((10, x.labels), (1, "y"))
 
 
 def test_linear_expression_from_rule(m, x, y):
@@ -238,21 +236,34 @@
     assert (res.coords["dim_1"] == other.coords["dim_1"]).all()
     assert res.data.notnull().all().to_array().all()
 
     assert isinstance(x - expr, LinearExpression)
     assert isinstance(x + expr, LinearExpression)
 
 
-def test_linear_expression_addition_invalid(x, y, z):
-    expr = 10 * x + y
+def test_linear_expression_addition_with_constant(x, y, z):
+    expr = 10 * x + y + 10
+    assert (expr.const == 10).all()
+
+    expr = 10 * x + y + np.array([2, 3])
+    assert list(expr.const) == [2, 3]
+
+    expr = 10 * x + y + pd.Series([2, 3])
+    assert list(expr.const) == [2, 3]
 
-    with pytest.raises(TypeError):
-        expr + 10
-    with pytest.raises(TypeError):
-        expr - 10
+
+def test_linear_expression_subtraction(x, y, z):
+    expr = 10 * x + y - 10
+    assert (expr.const == -10).all()
+
+    expr = 10 * x + y - np.array([2, 3])
+    assert list(expr.const) == [-2, -3]
+
+    expr = 10 * x + y - pd.Series([2, 3])
+    assert list(expr.const) == [-2, -3]
 
 
 def test_linear_expression_substraction(x, y, z, v):
     expr = 10 * x + y
     other = 2 * y - z
     res = expr - other
 
@@ -270,15 +281,37 @@
     assert res.nterm == expr.nterm * len(expr.data.dim_0)
 
     res = expr.sum()
     assert res.size == expr.size
     assert res.nterm == expr.size
     assert res.data.notnull().all().to_array().all()
 
-    assert_linequal(expr.sum(["dim_0", "_term"]), expr.sum("dim_0"))
+    assert_linequal(expr.sum(["dim_0", TERM_DIM]), expr.sum("dim_0"))
+
+    # test special case otherride coords
+    expr = v.loc[:9] + v.loc[10:]
+    assert expr.nterm == 2
+    assert len(expr.coords["dim_2"]) == 10
+
+
+def test_linear_expression_sum_with_const(x, y, z, v):
+    expr = 10 * x + y + z + 10
+    res = expr.sum("dim_0")
+
+    assert res.size == expr.size
+    assert res.nterm == expr.nterm * len(expr.data.dim_0)
+    assert (res.const == 20).all()
+
+    res = expr.sum()
+    assert res.size == expr.size
+    assert res.nterm == expr.size
+    assert res.data.notnull().all().to_array().all()
+    assert (res.const == 60).item()
+
+    assert_linequal(expr.sum(["dim_0", TERM_DIM]), expr.sum("dim_0"))
 
     # test special case otherride coords
     expr = v.loc[:9] + v.loc[10:]
     assert expr.nterm == 2
     assert len(expr.coords["dim_2"]) == 10
 
 
@@ -321,93 +354,196 @@
 
 
 def test_linear_expression_multiplication_invalid(x, y, z):
     expr = 10 * x + y + z
 
     with pytest.raises(TypeError):
         expr = 10 * x + y + z
-        expr * x
+        expr * expr
 
     with pytest.raises(TypeError):
         expr = 10 * x + y + z
         expr / x
 
 
+def test_linear_expression_loc(x, y):
+    expr = x + y
+    assert expr.loc[0].size < expr.loc[:5].size
+
+
 def test_linear_expression_where(v):
     expr = np.arange(20) * v
     expr = expr.where(expr.coeffs >= 10)
     assert isinstance(expr, LinearExpression)
     assert expr.nterm == 1
 
     expr = np.arange(20) * v
     expr = expr.where(expr.coeffs >= 10, drop=True).sum()
     assert isinstance(expr, LinearExpression)
     assert expr.nterm == 10
 
 
+def test_linear_expression_where_with_const(v):
+    expr = np.arange(20) * v + 10
+    expr = expr.where(expr.coeffs >= 10)
+    assert isinstance(expr, LinearExpression)
+    assert expr.nterm == 1
+    assert (expr.const[:10] == 0).all()
+    assert (expr.const[10:] == 10).all()
+
+    expr = np.arange(20) * v + 10
+    expr = expr.where(expr.coeffs >= 10, drop=True).sum()
+    assert isinstance(expr, LinearExpression)
+    assert expr.nterm == 10
+    assert expr.const == 100
+
+
 def test_linear_expression_shift(v):
     shifted = v.to_linexpr().shift(dim_2=2)
     assert shifted.nterm == 1
     assert shifted.coeffs.loc[:1].isnull().all()
     assert (shifted.vars.loc[:1] == -1).all()
 
 
 def test_linear_expression_diff(v):
     diff = v.to_linexpr().diff("dim_2")
     assert diff.nterm == 2
 
 
-def test_linear_expression_groupby(v):
+@pytest.mark.parametrize("use_fallback", [True, False])
+def test_linear_expression_groupby(v, use_fallback):
     expr = 1 * v
     groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
+    grouped = expr.groupby(groups).sum(use_fallback=use_fallback)
+    assert "group" in grouped.dims
+    assert (grouped.data.group == [1, 2]).all()
+    assert grouped.nterm == 10
+
+
+@pytest.mark.parametrize("use_fallback", [True, False])
+def test_linear_expression_groupby_with_name(v, use_fallback):
+    expr = 1 * v
+    groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords, name="my_group")
+    grouped = expr.groupby(groups).sum(use_fallback=use_fallback)
+    assert "my_group" in grouped.dims
+    assert (grouped.data.my_group == [1, 2]).all()
+    assert grouped.nterm == 10
+
+
+def test_linear_expression_groupby_with_series(v):
+    expr = 1 * v
+    groups = pd.Series([1] * 10 + [2] * 10, index=v.indexes["dim_2"])
     grouped = expr.groupby(groups).sum()
     assert "group" in grouped.dims
     assert (grouped.data.group == [1, 2]).all()
-    assert grouped.data._term.size == 10
+    assert grouped.nterm == 10
+
+
+def test_linear_expression_groupby_with_dataframe(v):
+    expr = 1 * v
+    groups = pd.DataFrame(
+        {"a": [1] * 10 + [2] * 10, "b": list(range(4)) * 5}, index=v.indexes["dim_2"]
+    )
+    grouped = expr.groupby(xr.DataArray(groups)).sum()
+    index = pd.MultiIndex.from_frame(groups)
+    assert "group" in grouped.dims
+    assert set(grouped.data.group.values) == set(index.values)
+    assert grouped.nterm == 3
+
+
+@pytest.mark.parametrize("use_fallback", [True, False])
+def test_linear_expression_groupby_with_const(v, use_fallback):
+    expr = 1 * v + 15
+    groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
+    grouped = expr.groupby(groups).sum(use_fallback=use_fallback)
+    assert "group" in grouped.dims
+    assert (grouped.data.group == [1, 2]).all()
+    assert grouped.nterm == 10
+    assert (grouped.const == 150).all()
 
 
-def test_linear_expression_groupby_asymmetric(v):
+@pytest.mark.parametrize("use_fallback", [True, False])
+def test_linear_expression_groupby_asymmetric(v, use_fallback):
     expr = 1 * v
     # now asymetric groups which result in different nterms
     groups = xr.DataArray([1] * 12 + [2] * 8, coords=v.coords)
-    grouped = expr.groupby(groups).sum()
+    grouped = expr.groupby(groups).sum(use_fallback=use_fallback)
+    assert "group" in grouped.dims
+    # first group must be full with vars
+    assert (grouped.data.sel(group=1) > 0).all()
+    # the last 4 entries of the second group must be empty, i.e. -1
+    assert (grouped.data.sel(group=2).isel(_term=slice(None, -4)).vars >= 0).all()
+    assert (grouped.data.sel(group=2).isel(_term=slice(-4, None)).vars == -1).all()
+    assert grouped.nterm == 12
+
+
+@pytest.mark.parametrize("use_fallback", [True, False])
+def test_linear_expression_groupby_asymmetric_with_const(v, use_fallback):
+    expr = 1 * v + 15
+    # now asymetric groups which result in different nterms
+    groups = xr.DataArray([1] * 12 + [2] * 8, coords=v.coords)
+    grouped = expr.groupby(groups).sum(use_fallback=use_fallback)
     assert "group" in grouped.dims
     # first group must be full with vars
     assert (grouped.data.sel(group=1) > 0).all()
     # the last 4 entries of the second group must be empty, i.e. -1
     assert (grouped.data.sel(group=2).isel(_term=slice(None, -4)).vars >= 0).all()
     assert (grouped.data.sel(group=2).isel(_term=slice(-4, None)).vars == -1).all()
-    assert grouped.data._term.size == 12
+    assert grouped.nterm == 12
+    assert list(grouped.const) == [180, 120]
 
 
 def test_linear_expression_groupby_roll(v):
     expr = 1 * v
     groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
     grouped = expr.groupby(groups).roll(dim_2=1)
     assert grouped.nterm == 1
     assert grouped.vars[0].item() == 19
 
 
+def test_linear_expression_groupby_roll_with_const(v):
+    expr = 1 * v + np.arange(20)
+    groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
+    grouped = expr.groupby(groups).roll(dim_2=1)
+    assert grouped.nterm == 1
+    assert grouped.vars[0].item() == 19
+    assert grouped.const[0].item() == 9
+
+
 def test_linear_expression_groupby_from_variable(v):
     groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
     grouped = v.groupby(groups).sum()
     assert "group" in grouped.dims
     assert (grouped.data.group == [1, 2]).all()
-    assert grouped.data._term.size == 10
+    assert grouped.nterm == 10
 
 
 def test_linear_expression_rolling(v):
     expr = 1 * v
     rolled = expr.rolling(dim_2=2).sum()
     assert rolled.nterm == 2
 
     rolled = expr.rolling(dim_2=3).sum()
     assert rolled.nterm == 3
 
 
+def test_linear_expression_rolling_with_const(v):
+    expr = 1 * v + 15
+    rolled = expr.rolling(dim_2=2).sum()
+    assert rolled.nterm == 2
+    assert rolled.const[0].item() == 15
+    assert (rolled.const[1:] == 30).all()
+
+    rolled = expr.rolling(dim_2=3).sum()
+    assert rolled.nterm == 3
+    assert rolled.const[0].item() == 15
+    assert rolled.const[1].item() == 30
+    assert (rolled.const[2:] == 45).all()
+
+
 def test_linear_expression_rolling_from_variable(v):
     rolled = v.rolling(dim_2=2).sum()
     assert rolled.nterm == 2
 
 
 def test_linear_expression_sanitize(x, y, z):
     expr = 10 * x + y + z
@@ -449,64 +585,13 @@
     expr2 = sum([1 * x, 2 * y])
     assert_linequal(expr, expr2)
 
 
 def test_rename(x, y, z):
     expr = 10 * x + y + z
     renamed = expr.rename({"dim_0": "dim_5"})
-    assert set(renamed.dims) == {"dim_1", "dim_5", "_term"}
+    assert set(renamed.dims) == {"dim_1", "dim_5", TERM_DIM}
     assert renamed.nterm == 3
 
     renamed = expr.rename({"dim_0": "dim_1", "dim_1": "dim_2"})
-    assert set(renamed.dims) == {"dim_1", "dim_2", "_term"}
+    assert set(renamed.dims) == {"dim_1", "dim_2", TERM_DIM}
     assert renamed.nterm == 3
-
-
-# -------------------------------- deprecated -------------------------------- #
-
-
-def test_rolling_sum_variable_deprecated(v):
-    with pytest.warns(DeprecationWarning):
-        rolled = v.rolling_sum(dim_2=2)
-    assert rolled.nterm == 2
-
-
-def test_linear_expression_rolling_sum_deprecated(x, v):
-    with pytest.warns(DeprecationWarning):
-        rolled = v.to_linexpr().rolling_sum(dim_2=2)
-    assert rolled.nterm == 2
-
-    # multi-dimensional rolling with non-scalar _term dimension
-    expr = 10 * x + v
-    with pytest.warns(DeprecationWarning):
-        rolled = expr.rolling_sum(dim_2=3)
-    assert rolled.nterm == 6
-
-
-def test_variable_groupby_sum_deprecated(v):
-    groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
-    with pytest.warns(DeprecationWarning):
-        grouped = v.groupby_sum(groups)
-    assert "group" in grouped.dims
-    assert (grouped.data.group == [1, 2]).all()
-    assert grouped.data._term.size == 10
-
-
-def test_linear_expression_groupby_sum_deprecated(v):
-    groups = xr.DataArray([1] * 10 + [2] * 10, coords=v.coords)
-    with pytest.warns(DeprecationWarning):
-        grouped = v.to_linexpr().groupby_sum(groups)
-    assert "group" in grouped.dims
-    assert (grouped.data.group == [1, 2]).all()
-    assert grouped.data._term.size == 10
-
-    # now asymetric groups which result in different nterms
-    groups = xr.DataArray([1] * 12 + [2] * 8, coords=v.coords)
-    with pytest.warns(DeprecationWarning):
-        grouped = v.to_linexpr().groupby_sum(groups)
-    assert "group" in grouped.dims
-    # first group must be full with vars
-    assert (grouped.data.sel(group=1) > 0).all()
-    # the last 4 entries of the second group must be empty, i.e. -1
-    assert (grouped.data.sel(group=2).isel(_term=slice(None, -4)).vars >= 0).all()
-    assert (grouped.data.sel(group=2).isel(_term=slice(-4, None)).vars == -1).all()
-    assert grouped.data._term.size == 12
```

### Comparing `linopy-0.1.5/test/test_matrices.py` & `linopy-0.2/test/test_matrices.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     x = m.add_variables(pd.Series([0, 0]), 1, name="x")
     y = m.add_variables(4, pd.Series([8, 10]), name="y")
     z = m.add_variables(0, pd.DataFrame([[1, 2], [3, 4], [5, 6]]).T, name="z")
     m.add_constraints(x + x + y + y + z + z == 0)
 
     A = m.matrices.A.todense()
     assert A[0, 0] == 2
-    assert np.isin(np.unique(A), [0, 2]).all()
+    assert np.isin(np.unique(np.array(A)), [0.0, 2.0]).all()
```

### Comparing `linopy-0.1.5/test/test_model.py` & `linopy-0.2/test/test_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     m = Model(solver_dir=d)
     assert m.solver_dir == Path(d)
 
 
 def test_model_variable_getitem():
     m = Model()
     x = m.add_variables(name="x")
-    assert m["x"].values == x.values
+    assert m["x"].labels == x.labels
 
 
 def test_coefficient_range():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
@@ -72,50 +72,42 @@
     obj = [(2, x)]
     m.add_objective(obj, overwrite=True)
 
     # test objective range
     assert m.objectiverange.min() == 2
     assert m.objectiverange.max() == 2
 
+    # test objective with constant which is not supported
+    with pytest.raises(ValueError):
+        m.objective = m.objective + 3
+
 
 def test_remove_variable():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
     x = m.add_variables(lower, upper, name="x")
     y = m.add_variables(name="y")
 
     m.add_constraints(1 * x + 10 * y, EQUAL, 0)
 
     obj = (10 * x + 5 * y).sum()
     m.add_objective(obj)
 
+    assert "x" in m.variables
+
     m.remove_variables("x")
-    for attr in m.constraints.dataset_attrs:
-        assert "x" not in getattr(m.constraints, attr)
+    assert "x" not in m.variables
 
-    assert "con0" not in m.constraints.labels
+    assert not m.constraints.con0.vars.isin(x.labels).any()
 
     assert not m.objective.vars.isin(x.labels).any()
 
 
 def test_remove_constraint():
     m = Model()
 
     x = m.add_variables()
     m.add_constraints(x, EQUAL, 0, name="x")
     m.remove_constraints("x")
     assert not len(m.constraints.labels)
-
-
-def test_removed_eval_funcs():
-    m = Model()
-
-    with pytest.raises(NotImplementedError):
-        m.vareval("")
-
-    with pytest.raises(NotImplementedError):
-        m.lineval("")
-
-    with pytest.raises(NotImplementedError):
-        m.coneval("")
```

### Comparing `linopy-0.1.5/test/test_optimization.py` & `linopy-0.2/test/test_optimization.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from xarray.testing import assert_equal
 
 from linopy import GREATER_EQUAL, Model
-from linopy.solvers import available_solvers
+from linopy.constants import SolverStatus, Status, TerminationCondition
+from linopy.solvers import available_solvers, quadratic_solvers
 
 params = [(name, "lp") for name in available_solvers]
 # mps io is only supported via highspy
 if "highs" in available_solvers:
     params += [(name, "mps") for name in available_solvers]
 
 if "gurobi" in available_solvers:
@@ -149,14 +150,42 @@
     m.add_constraints(x + y, GREATER_EQUAL, 10.99)
 
     m.add_objective(x + 2 * y)
     return m
 
 
 @pytest.fixture
+def quadratic_model():
+    m = Model()
+
+    lower = pd.Series(0, range(10))
+    x = m.add_variables(lower, name="x")
+    y = m.add_variables(lower, name="y")
+
+    m.add_constraints(x + y, GREATER_EQUAL, 10)
+
+    m.add_objective(x * x)
+    return m
+
+
+@pytest.fixture
+def quadratic_model_cross_terms():
+    m = Model()
+
+    lower = pd.Series(0, range(10))
+    x = m.add_variables(lower, name="x")
+    y = m.add_variables(lower, name="y")
+
+    m.add_constraints(x + y >= 10)
+
+    m.add_objective(-2 * x + y + x * x)
+    return m
+
+
+@pytest.fixture
 def modified_model():
     m = Model()
 
     lower = pd.Series(0, range(10))
     x = m.add_variables(coords=[lower.index], name="x", binary=True)
     y = m.add_variables(lower, name="y")
 
@@ -199,27 +228,53 @@
     # for the last two entries only the following constraint will be active
     m.add_constraints(x + y, GREATER_EQUAL, 5)
 
     m.add_objective(2 * x + y)
     return m
 
 
+def test_model_types(
+    model,
+    model_with_duplicated_variables,
+    milp_binary_model,
+    milp_binary_model_r,
+    milp_model,
+    milp_model_r,
+    quadratic_model,
+    quadratic_model_cross_terms,
+    modified_model,
+    masked_variable_model,
+    masked_constraint_model,
+):
+    assert model.type == "LP"
+    assert model_with_duplicated_variables.type == "LP"
+    assert milp_binary_model.type == "MILP"
+    assert milp_binary_model_r.type == "MILP"
+    assert milp_model.type == "MILP"
+    assert milp_model_r.type == "MILP"
+    assert quadratic_model.type == "QP"
+    assert quadratic_model_cross_terms.type == "QP"
+    assert modified_model.type == "MILP"
+    assert masked_variable_model.type == "LP"
+    assert masked_constraint_model.type == "LP"
+
+
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_setting(model, solver, io_api):
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "ok"
     assert np.isclose(model.objective_value, 3.3)
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_setting_sol_and_dual_accessor(model, solver, io_api):
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "ok"
     x = model["x"]
-    assert_equal(x.sol, model.solution["x"])
+    assert_equal(x.solution, model.solution["x"])
     c = model.constraints["con1"]
     assert_equal(c.dual, model.dual["con1"])
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_anonymous_constraint(model, model_anonymous_constraint, solver, io_api):
     status, condition = model_anonymous_constraint.solve(solver, io_api=io_api)
@@ -292,15 +347,15 @@
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "warning"
     assert "infeasible" in condition
 
     if solver == "gurobi":
         model.compute_set_of_infeasible_constraints()
     else:
-        with pytest.raises(NotImplementedError):
+        with pytest.raises((NotImplementedError, ImportError)):
             model.compute_set_of_infeasible_constraints()
 
 
 @pytest.mark.parametrize(
     "solver,io_api", [p for p in params if p[0] not in ["glpk", "cplex"]]
 )
 def test_model_with_inf(model_with_inf, solver, io_api):
@@ -333,17 +388,70 @@
     status, condition = milp_model.solve(solver, io_api=io_api)
     assert condition == "optimal"
     assert ((milp_model.solution.y == 9) | (milp_model.solution.x == 0.5)).all()
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_milp_model_r(milp_model_r, solver, io_api):
-    status, condition = milp_model_r.solve(solver, io_api=io_api)
-    assert condition == "optimal"
-    assert ((milp_model_r.solution.x == 11) | (milp_model_r.solution.y == 0)).all()
+    # MPS format by Highs wrong, see https://github.com/ERGO-Code/HiGHS/issues/1325
+    # skip it
+    if io_api != "mps":
+        status, condition = milp_model_r.solve(solver, io_api=io_api)
+        assert condition == "optimal"
+        assert ((milp_model_r.solution.x == 11) | (milp_model_r.solution.y == 0)).all()
+
+
+@pytest.mark.parametrize("solver,io_api", params)
+def test_quadratic_model(quadratic_model, solver, io_api):
+    if solver in quadratic_solvers:
+        status, condition = quadratic_model.solve(solver, io_api=io_api)
+        assert condition == "optimal"
+        assert (quadratic_model.solution.x.round(3) == 0).all()
+        assert (quadratic_model.solution.y.round(3) == 10).all()
+        assert round(quadratic_model.objective_value, 3) == 0
+    else:
+        with pytest.raises(ValueError):
+            quadratic_model.solve(solver, io_api=io_api)
+
+
+@pytest.mark.parametrize("solver,io_api", params)
+def test_quadratic_model_cross_terms(quadratic_model_cross_terms, solver, io_api):
+    if solver in quadratic_solvers:
+        status, condition = quadratic_model_cross_terms.solve(solver, io_api=io_api)
+        assert condition == "optimal"
+        assert (quadratic_model_cross_terms.solution.x.round(3) == 1.5).all()
+        assert (quadratic_model_cross_terms.solution.y.round(3) == 8.5).all()
+        assert round(quadratic_model_cross_terms.objective_value, 3) == 77.5
+    else:
+        with pytest.raises(ValueError):
+            quadratic_model_cross_terms.solve(solver, io_api=io_api)
+
+
+@pytest.mark.parametrize("solver,io_api", params)
+def test_quadratic_model_wo_constraint(quadratic_model, solver, io_api):
+    quadratic_model.constraints.remove("con0")
+    if solver in quadratic_solvers:
+        status, condition = quadratic_model.solve(solver, io_api=io_api)
+        assert condition == "optimal"
+        assert (quadratic_model.solution.x.round(3) == 0).all()
+        assert round(quadratic_model.objective_value, 3) == 0
+    else:
+        with pytest.raises(ValueError):
+            quadratic_model.solve(solver, io_api=io_api)
+
+
+@pytest.mark.parametrize("solver,io_api", params)
+def test_quadratic_model_unbounded(quadratic_model, solver, io_api):
+    quadratic_model.objective = -quadratic_model.objective
+    if solver in quadratic_solvers:
+        status, condition = quadratic_model.solve(solver, io_api=io_api)
+        assert condition in ["unbounded", "unknown", "infeasible_or_unbounded"]
+    else:
+        with pytest.raises(ValueError):
+            quadratic_model.solve(solver, io_api=io_api)
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_modified_model(modified_model, solver, io_api):
     status, condition = modified_model.solve(solver, io_api=io_api)
     assert condition == "optimal"
     assert (modified_model.solution.x == 0).all()
```

### Comparing `linopy-0.1.5/test/test_options.py` & `linopy-0.2/test/test_options.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/test/test_repr.py` & `linopy-0.2/test/test_repr.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,61 +19,65 @@
 a = m.add_variables(coords=[lower.index], name="a", binary=True)
 b = m.add_variables(coords=[lower.index], name="b", integer=True)
 c_mask = xr.DataArray(False, coords=upper.axes)
 c_mask[:, 5:] = True
 c = m.add_variables(lower, upper, name="c", mask=c_mask)
 d = m.add_variables(0, 10, coords=[types], name="d")
 
-# add variable with indexes to reindex
-with pytest.warns(UserWarning):
-    e = m.add_variables(0, upper[5:], name="e")
-
-    f_mask = np.full_like(upper[:5], True, dtype=bool)
-    f_mask[:3] = False
-    f = m.add_variables(0, upper[5:], name="f", mask=f_mask)
+# new behavior in v0.2, variable with dimension name and other
+# coordinates are added without a warning
+e = m.add_variables(0, upper[5:], name="e")
+
+f_mask = np.full_like(upper[:5], True, dtype=bool)
+f_mask[:3] = False
+f = m.add_variables(0, upper[5:], name="f", mask=f_mask)
 
 
 # create linear expression for each variable
 lu = 1 * u
 lv = 1 * v
 lx = 1 * x
 ly = 1 * y
 lz = 1 * z
 la = 1 * a
 lb = 1 * b
 lc = 1 * c
 ld = 1 * d
 lav = 1 * a + 1 * v
-
+luc = 1 * v + 10
+lq = x * x
+lq2 = x * x + 1 * x
+lq3 = x * x + 1 * x + 1 + 1 * y + 1 * z
 
 # create anonymous constraint for linear expression
 cu_ = lu >= 0
 cv_ = lv >= 0
 cx_ = lx >= 0
 cy_ = ly >= 0
 cz_ = lz >= 0
 ca_ = la >= 0
 cb_ = lb >= 0
 cc_ = lc >= 0
 cd_ = ld >= 0
 cav_ = lav >= 0
-
+cuc_ = luc >= 0
 
 # add constraint for each variable
 cu = m.add_constraints(cu_, name="cu")
 cv = m.add_constraints(cv_, name="cv")
 cx = m.add_constraints(cx_, name="cx")
 cy = m.add_constraints(cy_, name="cy")
 cz = m.add_constraints(cz_, name="cz")
 ca = m.add_constraints(ca_, name="ca")
 cb = m.add_constraints(cb_, name="cb")
 cc = m.add_constraints(cc_, name="cc")
 cd = m.add_constraints(cd_, name="cd")
 cav = m.add_constraints(cav_, name="cav")
-cu_masked = m.add_constraints(cu_, name="cu_masked", mask=xr.full_like(u.data, False))
+cuc = m.add_constraints(cuc_, name="cuc")
+cu_masked = m.add_constraints(cu_, name="cu_masked", mask=xr.full_like(u.labels, False))
 
 
 def test_variable_repr():
     for var in [u, v, x, y, z, a, b, c, d, e, f]:
         repr(var)
 
 
@@ -86,15 +90,15 @@
 def test_single_variable_repr():
     for var in [u, v, x, y, z, a, b, c, d]:
         coord = tuple([var.indexes[c][0] for c in var.dims])
         repr(var.loc[coord])
 
 
 def test_linear_expression_repr():
-    for expr in [lu, lv, lx, ly, lz, la, lb, lc, ld, lav]:
+    for expr in [lu, lv, lx, ly, lz, la, lb, lc, ld, lav, luc, lq, lq2, lq3]:
         repr(expr)
 
 
 def test_linear_expression_long():
     repr(x.sum())
 
 
@@ -107,15 +111,15 @@
 def test_single_linear_repr():
     for var in [u, v, x, y, z, a, b, c, d]:
         coord = tuple([var.indexes[c][0] for c in var.dims])
         repr(1 * var.loc[coord])
 
 
 def test_anonymous_constraint_repr():
-    for con in [cu_, cv_, cx_, cy_, cz_, ca_, cb_, cc_, cd_, cav_]:
+    for con in [cu_, cv_, cx_, cy_, cz_, ca_, cb_, cc_, cd_, cav_, cuc_]:
         repr(con)
 
 
 def test_scalar_constraint_repr():
     repr(1 * u[0, 0] >= 0)
 
 
@@ -123,15 +127,15 @@
     for var in [u, v, x, y, z, a, b, c, d]:
         coord = tuple([var.indexes[c][0] for c in var.dims])
         repr(1 * var.loc[coord] == 0)
         repr(1 * var.loc[coord] - var.loc[coord] == 0)
 
 
 def test_constraint_repr():
-    for con in [cu, cv, cx, cy, cz, ca, cb, cc, cd, cav, cu_masked]:
+    for con in [cu, cv, cx, cy, cz, ca, cb, cc, cd, cav, cuc, cu_masked]:
         repr(con)
 
 
 def test_empty_repr():
     repr(u.loc[[]])
     repr(lu.sel(dim_0=[]))
     repr(lu.sel(dim_0=[]) >= 0)
```

### Comparing `linopy-0.1.5/test/test_scalar_constraint.py` & `linopy-0.2/test/test_scalar_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/test/test_scalar_linear_expression.py` & `linopy-0.2/test/test_scalar_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.1.5/test/test_variable.py` & `linopy-0.2/test/test_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,19 +44,25 @@
 
 
 def test_variable_data(x):
     isinstance(x.data, xr.DataArray)
 
 
 def test_wrong_variable_init(m, x):
+    # without explicit name
+    with pytest.raises(TypeError):
+        linopy.Variable(x.data, m)
+
+    # wrong data type
     with pytest.raises(ValueError):
-        linopy.Variable(x.labels.values, m)
+        linopy.Variable(x.labels.values, m, "")
 
+    # no model
     with pytest.raises(ValueError):
-        linopy.Variable(x.labels, None)
+        linopy.Variable(x.labels, None, "")
 
 
 def test_variable_getter(x, z):
     assert isinstance(x[0], linopy.variables.ScalarVariable)
 
     assert isinstance(z[0], linopy.variables.ScalarVariable)
 
@@ -136,56 +142,56 @@
     res = x.sum()
     assert res.nterm == 10
 
 
 def test_variable_where(x):
     x = x.where([True] * 4 + [False] * 6)
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[9] == x.fill_value
+    assert x.labels[9] == x.fill_value["labels"]
 
     x = x.where([True] * 4 + [False] * 6, x[0])
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[9] == x[0].label
+    assert x.labels[9] == x[0].label
 
     x = x.where([True] * 4 + [False] * 6, x.loc[0])
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[9] == x[0].label
+    assert x.labels[9] == x[0].label
 
 
 def test_variable_shift(x):
     x = x.shift(first=3)
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[0] == -1
+    assert x.labels[0] == -1
 
 
 def test_variable_bfill(x):
     x = x.where([False] * 4 + [True] * 6)
     x = x.bfill("first")
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[2] == x.values[4]
-    assert x.values[2] != x.values[5]
+    assert x.labels[2] == x.labels[4]
+    assert x.labels[2] != x.labels[5]
 
 
 def test_variable_broadcast_like(x):
     result = x.broadcast_like(x.labels)
     assert isinstance(result, linopy.variables.Variable)
 
 
 def test_variable_ffill(x):
     x = x.where([True] * 4 + [False] * 6)
     x = x.ffill("first")
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[9] == x.values[3]
-    assert x.values[3] != x.values[2]
+    assert x.labels[9] == x.labels[3]
+    assert x.labels[3] != x.labels[2]
 
 
 def test_variable_fillna(x):
     result = x.fillna(-1)
     assert isinstance(result, linopy.variables.Variable)
 
 
 def test_variable_sanitize(x):
     # convert intentionally to float with nans
     x = x.where([True] * 4 + [False] * 6, np.nan)
     x = x.sanitize()
     assert isinstance(x, linopy.variables.Variable)
-    assert x.values[9] == -1
+    assert x.labels[9] == -1
```

### Comparing `linopy-0.1.5/test/test_variable_assignment.py` & `linopy-0.2/test/test_variable_assignment.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,107 +31,173 @@
 
 
 def test_variable_assignment():
     m = Model()
 
     lower = xr.DataArray(np.zeros((10, 10)), coords=[range(10), range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_broadcasted():
     m = Model()
     # setting only one dimension, the other has to be broadcasted
     lower = xr.DataArray(np.zeros((10)), coords=[range(10)])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_no_coords():
     # setting bounds without explicit coords
     m = Model()
     lower = xr.DataArray(np.zeros((10)))
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_pd_index():
     # setting bounds with pandas index
     m = Model()
     lower = xr.DataArray(np.zeros((10)), coords=[pd.Index(range(10))])
     upper = xr.DataArray(np.ones((10, 10)), coords=[range(10), range(10)])
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_by_coords():
     # setting bounds with scalar and coords
     m = Model()
     lower = 0
     upper = 1
     coords = [pd.Index(range(10)), pd.Index(range(10))]
-    m.add_variables(lower, upper, coords=coords, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, coords=coords, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_with_dataframes():
     # setting bounds with pd.DataFrames
     m = Model()
     lower = pd.DataFrame(np.zeros((10, 10)))
     upper = pd.DataFrame(np.ones((10, 10)))
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_with_dataframe_and_series():
     # setting bounds with one pd.DataFrame and one pd.Series
     m = Model()
     lower = pd.DataFrame(np.zeros((10, 10)))
     upper = pd.Series(np.ones((10)))
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
 
 
 def test_variable_assignment_chunked():
     # setting bounds with one pd.DataFrame and one pd.Series
     m = Model(chunk=5)
     lower = pd.DataFrame(np.zeros((10, 10)))
     upper = pd.Series(np.ones((10)))
-    m.add_variables(lower, upper, name="x")
-    assert m.variables.labels.x.shape == target_shape
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
     assert isinstance(m.variables.labels.x.data, dask.array.core.Array)
 
 
+def test_variable_assignment_different_shapes():
+    # setting bounds with different shapes
+    m = Model()
+    lower = pd.DataFrame(np.zeros((10, 10)))
+    upper = pd.Series(np.ones((10)))
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
+
+
+def test_variable_assignment_without_coords():
+    # setting bounds without explicit coords
+    m = Model()
+    lower = np.zeros((10, 10))
+    upper = np.ones((10))
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
+
+
+def test_variable_assignment_without_coords_and_dims_names():
+    # setting bounds without explicit coords
+    m = Model()
+    lower = np.zeros((10, 10))
+    upper = np.ones((10, 10))
+    x = m.add_variables(lower, upper, name="x", dims=["i", "j"])
+    assert x.shape == target_shape
+    assert x.dims == ("i", "j")
+
+
+def test_variable_assignment_without_coords_in_bounds():
+    # setting bounds without explicit coords
+    m = Model()
+    lower = xr.DataArray(np.zeros((10, 10)), dims=["i", "j"])
+    upper = xr.DataArray(np.ones((10, 10)), dims=["i", "j"])
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
+    assert x.dims == ("i", "j")
+
+
+def test_variable_assignment_without_coords_pandas_types():
+    # setting bounds without explicit coords
+    m = Model()
+    lower = pd.DataFrame(np.zeros((10, 10)))
+    upper = pd.DataFrame(np.ones((10, 10)))
+    x = m.add_variables(lower, upper, name="x", dims=["i", "j"])
+    assert x.shape == target_shape
+    assert x.dims == ("i", "j")
+
+
+def test_variable_assignment_without_coords_mixed_types():
+    # setting bounds without explicit coords
+    m = Model()
+    lower = pd.DataFrame(np.zeros((10, 10)))
+    upper = 1
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
+
+    m = Model()
+    lower = xr.DataArray(np.zeros((10, 10)), dims=["i", "j"])
+    upper = 1
+    x = m.add_variables(lower, upper, name="x")
+    assert x.shape == target_shape
+    assert x.dims == ("i", "j")
+
+
 def test_variable_assignment_different_coords():
     # set a variable with different set of coordinates
     # since v0.1 new coordinates are reindexed to the old ones
     m = Model()
     lower = pd.DataFrame(np.zeros((10, 10)))
     upper = pd.Series(np.ones((10)))
     m.add_variables(lower, upper, name="x")
 
     lower = pd.DataFrame(np.zeros((20, 10)))
     upper = pd.Series(np.ones((20)))
-    with pytest.warns(UserWarning):
-        m.add_variables(lower, upper, name="y")
+    m.add_variables(lower, upper, name="y")
 
-    assert m.variables.labels.y.shape == (10, 10)
-    # x should now be aligned to new coords and contain 100 nans
-    assert m.variables.labels.x.shape == (10, 10)
-    assert (m.variables.labels.x != -1).sum() == 100
+    with pytest.warns(UserWarning):
+        assert m.variables.labels.y.shape == (20, 10)
+        # x should now be aligned to new coords and contain 100 nans
+        assert m.variables.labels.x.shape == (20, 10)
+        assert (m.variables.labels.x != -1).sum() == 100
 
 
-def test_variable_assignment_non_broadcastable():
+def test_variable_assignment_with_broadcast():
     # setting with scalar and list
     m = Model()
+    m.add_variables(lower=0, upper=[1, 2])
+
     with pytest.raises(ValueError):
-        m.add_variables(0, [1, 2])
+        m.add_variables(lower=0, upper=[1, 2], dims=["i"])
 
 
 def test_variable_assignment_repeated():
     # repeated variable assignment is forbidden
     m = Model()
     m.add_variables(name="x")
     with pytest.raises(ValueError):
```

### Comparing `linopy-0.1.5/test/test_variables.py` & `linopy-0.2/test/test_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import linopy
 from linopy import Model
+from linopy.testing import assert_varequal
 
 
 @pytest.fixture
 def m():
     m = Model()
     m.add_variables(coords=[pd.RangeIndex(10, name="first")], name="x")
     m.add_variables(coords=[pd.Index([1, 2, 3], name="second")], name="y")
@@ -32,30 +33,32 @@
 
     New coordinates are aligned to the existing ones. Thus this should
     raise a warning.
     """
     m = Model()
 
     upper = pd.Series(np.ones((10)))
-    m.add_variables(upper)
+    var0 = m.add_variables(upper)
 
     upper = pd.Series(np.ones((12)))
+    var1 = m.add_variables(upper)
+
     with pytest.warns(UserWarning):
-        m.add_variables(upper)
+        assert m.variables.labels.var0[-1].item() == -1
 
-    assert m.variables.labels.var0[-1].item() != -1
+    assert_varequal(var0, m.variables.var0)
+    assert_varequal(var1, m.variables.var1)
 
 
 def test_variables_assignment_with_reindex(m):
     shuffled_coords = [pd.Index([2, 1, 3, 4, 6, 5, 7, 9, 8, 0], name="first")]
+    m.add_variables(coords=shuffled_coords, name="a")
+
     with pytest.warns(UserWarning):
-        a = m.add_variables(coords=shuffled_coords, name="a")
-    assert a.indexes["first"].equals(m["x"].indexes["first"])
-    # check if labels are monotonically increasing
-    assert np.all(np.diff(np.ravel(a.labels)) > 0)
+        m.variables.labels
 
 
 def test_scalar_variables_name_counter():
     m = Model()
     m.add_variables()
     m.add_variables()
     assert "var0" in m.variables
```

