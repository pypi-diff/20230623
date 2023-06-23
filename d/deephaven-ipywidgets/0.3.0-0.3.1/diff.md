# Comparing `tmp/deephaven_ipywidgets-0.3.0.tar.gz` & `tmp/deephaven_ipywidgets-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven_ipywidgets-0.3.0.tar", last modified: Fri Jun 23 16:01:56 2023, max compression
+gzip compressed data, was "deephaven_ipywidgets-0.3.1.tar", last modified: Fri Jun 23 20:16:31 2023, max compression
```

## Comparing `deephaven_ipywidgets-0.3.0.tar` & `deephaven_ipywidgets-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/css/widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/deephaven.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-23 16:00:42.396814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/421.1465f517f2d0e9eda410.js
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 16:00:39.376806 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    52136 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    75326 2023-06-23 16:00:37.524802 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   274308 2023-06-23 16:00:37.524802 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    74803 2023-06-23 16:00:37.432802 deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   273409 2023-06-23 16:00:37.432802 deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/_static/helper.js
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/develop-install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/examples/introduction.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/__tests__/index.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/__tests__/utils.ts
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/extension.ts
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/widget.ts
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/css/widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/deephaven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-23 20:15:18.574201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/421.1465f517f2d0e9eda410.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 20:15:15.442176 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52136 2023-06-23 20:15:18.570201 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    75326 2023-06-23 20:15:13.414161 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   274308 2023-06-23 20:15:13.414161 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/deephaven_ipywidgets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    74803 2023-06-23 20:15:13.366160 deephaven_ipywidgets-0.3.1/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   273409 2023-06-23 20:15:13.366160 deephaven_ipywidgets-0.3.1/docs/source/_static/embed-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/_static/helper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/develop-install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/examples/introduction.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/docs/source/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:16:31.254880 deephaven_ipywidgets-0.3.1/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/__tests__/index.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/__tests__/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/extension.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/src/widget.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-23 20:13:56.705519 deephaven_ipywidgets-0.3.1/webpack.config.js
```

### Comparing `deephaven_ipywidgets-0.3.0/LICENSE.txt` & `deephaven_ipywidgets-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/PKG-INFO` & `deephaven_ipywidgets-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven_ipywidgets
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com/deephaven/deephaven-ipywidgets
 Author: Deephaven Data Labs LLC
 Author-email: operations@deephaven.io
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `deephaven_ipywidgets-0.3.0/README.md` & `deephaven_ipywidgets-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/__init__.py` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/deephaven.py` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/deephaven.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/package.json` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/package.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/421.1465f517f2d0e9eda410.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/421.1465f517f2d0e9eda410.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/third-party-licenses.json` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js.map` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/conftest.py` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_table.py` & `deephaven_ipywidgets-0.3.1/deephaven_ipywidgets/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/Makefile` & `deephaven_ipywidgets-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/make.bat` & `deephaven_ipywidgets-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js` & `deephaven_ipywidgets-0.3.1/docs/source/_static/embed-bundle.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js.map` & `deephaven_ipywidgets-0.3.1/docs/source/_static/embed-bundle.js.map`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/conf.py` & `deephaven_ipywidgets-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/develop-install.rst` & `deephaven_ipywidgets-0.3.1/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/index.rst` & `deephaven_ipywidgets-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/docs/source/installing.rst` & `deephaven_ipywidgets-0.3.1/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/examples/introduction.ipynb` & `deephaven_ipywidgets-0.3.1/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/package.json` & `deephaven_ipywidgets-0.3.1/package.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/setup.py` & `deephaven_ipywidgets-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/__tests__/index.spec.ts` & `deephaven_ipywidgets-0.3.1/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/__tests__/utils.ts` & `deephaven_ipywidgets-0.3.1/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/extension.ts` & `deephaven_ipywidgets-0.3.1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/plugin.ts` & `deephaven_ipywidgets-0.3.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/version.ts` & `deephaven_ipywidgets-0.3.1/src/version.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/src/widget.ts` & `deephaven_ipywidgets-0.3.1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/tsconfig.json` & `deephaven_ipywidgets-0.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.3.0/webpack.config.js` & `deephaven_ipywidgets-0.3.1/webpack.config.js`

 * *Files identical despite different names*

