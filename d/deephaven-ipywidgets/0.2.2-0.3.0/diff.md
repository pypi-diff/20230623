# Comparing `tmp/deephaven_ipywidgets-0.2.2.tar.gz` & `tmp/deephaven_ipywidgets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven_ipywidgets-0.2.2.tar", last modified: Fri Apr 14 19:25:57 2023, max compression
+gzip compressed data, was "deephaven_ipywidgets-0.3.0.tar", last modified: Fri Jun 23 16:01:56 2023, max compression
```

## Comparing `deephaven_ipywidgets-0.2.2.tar` & `deephaven_ipywidgets-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/css/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/css/widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/deephaven.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-14 19:24:24.497498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/480.26bcd834ece40109d1df.js
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/568.8c7c3ea60a12c60e6eb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/remoteEntry.6443de594d4e2715e64f.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-14 19:24:21.909489 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    15446 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    25901 2023-04-14 19:24:18.705479 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-04-14 19:24:18.705479 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-14 19:24:18.589478 deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)    94888 2023-04-14 19:24:18.589478 deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/_static/helper.js
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/develop-install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/examples/introduction.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/__tests__/index.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/__tests__/utils.ts
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/extension.ts
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/widget.ts
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/css/widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/deephaven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-23 16:00:42.396814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/421.1465f517f2d0e9eda410.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 16:00:39.376806 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52136 2023-06-23 16:00:42.392814 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.485008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    75326 2023-06-23 16:00:37.524802 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   274308 2023-06-23 16:00:37.524802 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 15:59:20.680584 deephaven_ipywidgets-0.3.0/deephaven_ipywidgets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    74803 2023-06-23 16:00:37.432802 deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   273409 2023-06-23 16:00:37.432802 deephaven_ipywidgets-0.3.0/docs/source/_static/embed-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/_static/helper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/develop-install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/examples/introduction.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/docs/source/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:01:56.489008 deephaven_ipywidgets-0.3.0/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/__tests__/index.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/__tests__/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/extension.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/src/widget.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-23 15:59:20.684584 deephaven_ipywidgets-0.3.0/webpack.config.js
```

### Comparing `deephaven_ipywidgets-0.2.2/LICENSE.txt` & `deephaven_ipywidgets-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/PKG-INFO` & `deephaven_ipywidgets-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven_ipywidgets
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com/deephaven/deephaven-ipywidgets
 Author: Deephaven Data Labs LLC
 Author-email: operations@deephaven.io
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
@@ -74,14 +74,20 @@
 You can also pass in the size you would like the widget to be:
 
 ```python
 # Specify a size for the table
 display(DeephavenWidget(t, width=100, height=250))
 ```
 
+### Alternate Deephaven Server URL
+By default, the Deephaven server is located at `http://localhost:{port}`, where `{port}` is the port set in the Deephaven server creation call. If the server is not there, such as when running a Jupyter notebook in a Docker container, modify the `DEEPHAVEN_IPY_URL` environmental variable to the correct URL before creating a `DeephavenWidget`. 
+```python
+import os 
+os.environ["DEEPHAVEN_IPY_URL"] = "http://localhost:1234"
+```
 ## Development Installation
 
 Before starting, you will need [python3](https://www.python.org/downloads/), [node](https://nodejs.org/en/download/), and [yarn](https://classic.yarnpkg.com/lang/en/docs/install/) installed.
 
 Create and source a dev python venv environment:
 
 ```bash
```

### Comparing `deephaven_ipywidgets-0.2.2/README.md` & `deephaven_ipywidgets-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 You can also pass in the size you would like the widget to be:
 
 ```python
 # Specify a size for the table
 display(DeephavenWidget(t, width=100, height=250))
 ```
 
+### Alternate Deephaven Server URL
+By default, the Deephaven server is located at `http://localhost:{port}`, where `{port}` is the port set in the Deephaven server creation call. If the server is not there, such as when running a Jupyter notebook in a Docker container, modify the `DEEPHAVEN_IPY_URL` environmental variable to the correct URL before creating a `DeephavenWidget`. 
+```python
+import os 
+os.environ["DEEPHAVEN_IPY_URL"] = "http://localhost:1234"
+```
 ## Development Installation
 
 Before starting, you will need [python3](https://www.python.org/downloads/), [node](https://nodejs.org/en/download/), and [yarn](https://classic.yarnpkg.com/lang/en/docs/install/) installed.
 
 Create and source a dev python venv environment:
 
 ```bash
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/__init__.py` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/deephaven.py` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/deephaven.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 
 """
 Module for displaying Deephaven widgets within interactive python environments.
 """
 
 import __main__
 from ipywidgets import DOMWidget
-from traitlets import Unicode, Integer
+from traitlets import Unicode, Integer, Bytes
 from deephaven_server import Server
 from uuid import uuid4
 from ._frontend import module_name, module_version
 import os
+import base64
+import json
+
 
 def _str_object_type(obj):
     """Returns the object type as a string value"""
     return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
 
 
 def _path_for_object(obj):
     """Return the iframe path for the specified object. Inspects the class name to determine."""
     name = _str_object_type(obj)
 
-    if name in ('deephaven.table.Table', 'pandas.core.frame.DataFrame'):
+    if name in ('deephaven.table.Table', 'pandas.core.frame.DataFrame', 'pydeephaven.table.Table'):
         return 'table'
     if name == 'deephaven.plot.figure.Figure':
         return 'chart'
     raise TypeError(f"Unknown object type: {name}")
 
 
+
 class DeephavenWidget(DOMWidget):
     """A wrapper for viewing DeephavenWidgets in IPython
     """
     _model_name = Unicode('DeephavenModel').tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
     _view_name = Unicode('DeephavenView').tag(sync=True)
@@ -44,49 +48,78 @@
 
     object_id = Unicode().tag(sync=True)
     object_type = Unicode().tag(sync=True)
     server_url = Unicode().tag(sync=True)
     iframe_url = Unicode().tag(sync=True)
     width = Integer().tag(sync=True)
     height = Integer().tag(sync=True)
+    token = Unicode().tag(sync=True)
 
     def __init__(self, deephaven_object, height=600, width=0):
         """Create a Deephaven widget for displaying in an interactive Python console.
 
         Args:
             deephaven_object (Table): the Deephaven object to display
             height (int): the height of the table
             width (int): the width of the table. Set to 0 to take up full width of notebook.
         """
         super(DeephavenWidget, self).__init__()
 
         # Generate a new table ID using a UUID prepended with a `t_` prefix
         object_id = f"t_{str(uuid4()).replace('-', '_')}"
 
-        port = Server.instance.port
+        params = {
+            "name": object_id
+        }
+
+        token = ''
+
+        if _str_object_type(deephaven_object) == 'pydeephaven.table.Table':
+            session = deephaven_object.session
+
+            envoy_prefix = session._extra_headers[
+                b'envoy-prefix'].decode('ascii')
 
-        server_url = f"http://localhost:{Server.instance.port}/"
+            token = base64.b64encode(
+                session.session_manager.auth_client.get_token("RemoteQueryProcessor").SerializeToString()
+            ).decode('us-ascii')
+
+            params.update({
+                "authProvider": "parent",
+                "envoyPrefix": envoy_prefix
+            })
+
+            port = deephaven_object.session.port
+            server_url = f"https://{deephaven_object.session.host}:{port}"
+
+            session.bind_table(object_id, deephaven_object)
+        else:
+            port = Server.instance.port
+            server_url = f"http://localhost:{port}/"
+
+        param_values = [f"{k}={v}" for k, v in params.items()]
+        param_string = "?" + "&".join(param_values)
 
         if "DEEPHAVEN_IPY_URL" in os.environ:
             server_url = os.environ["DEEPHAVEN_IPY_URL"]
 
         try:
             from google.colab.output import eval_js
             server_url = eval_js(f"google.colab.kernel.proxyPort({port})")
         except ImportError:
             pass
 
         if not server_url.endswith("/"):
             server_url = f"{server_url}/"
 
         # Generate the iframe_url from the object type
-        iframe_url = f"{server_url}iframe/{_path_for_object(deephaven_object)}/?name={object_id}"
-
+        iframe_url = f"{server_url}iframe/{_path_for_object(deephaven_object)}/{param_string}"
         # Add the table to the main modules globals list so it can be retrieved by the iframe
         __main__.__dict__[object_id] = deephaven_object
 
         self.set_trait('server_url', server_url)
         self.set_trait('iframe_url', iframe_url)
         self.set_trait('object_id', object_id)
         self.set_trait('object_type', _str_object_type(deephaven_object))
         self.set_trait('width', width)
         self.set_trait('height', height)
+        self.set_trait('token', token)
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/package.json` & `deephaven_ipywidgets-0.3.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9506944444444445%*

 * *Differences: {"'dependencies'": "{'@deephaven/jsapi-shim': '^0.41.0', '@deephaven/log': '^0.41.0', "*

 * *                   "'@deephaven/jsapi-utils': '^0.41.3'}",*

 * * "'devDependencies'": "{'@deephaven/eslint-config': '^0.41.0', '@deephaven/prettier-config': "*

 * *                      "'^0.41.0', '@jupyterlab/builder': '^3.6.4', "*

 * *                      "'@typescript-eslint/eslint-plugin': '^5.46.0', '@typescript-eslint/parser': "*

 * *                      "'^5.46.0', 'eslint': '^8.29.0', 'eslint-import-resolver-typescript': "*

 * *       […]*

```diff
@@ -3,46 +3,48 @@
         "email": "operations@deephaven.io",
         "name": "Deephaven Data Labs LLC"
     },
     "bugs": {
         "url": "https://github.com/deephaven/deephaven-ipywidgets/issues"
     },
     "dependencies": {
-        "@deephaven/jsapi-shim": "0.15.0",
-        "@deephaven/log": "0.15.0",
+        "@deephaven/jsapi-shim": "^0.41.0",
+        "@deephaven/jsapi-utils": "^0.41.3",
+        "@deephaven/log": "^0.41.0",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "uuid": "8.3.2"
     },
     "description": "Deephaven ipython widget library",
     "devDependencies": {
         "@babel/core": "^7.5.0",
         "@babel/preset-env": "^7.5.0",
-        "@deephaven/eslint-config": "0.15.0",
-        "@deephaven/prettier-config": "0.15.0",
-        "@jupyterlab/builder": "^3.0.0",
+        "@deephaven/eslint-config": "^0.41.0",
+        "@deephaven/prettier-config": "^0.41.0",
+        "@jupyterlab/builder": "^3.6.4",
         "@phosphor/application": "^1.6.0",
         "@phosphor/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
         "@types/uuid": "8.3.4",
         "@types/webpack-env": "^1.13.6",
-        "@typescript-eslint/eslint-plugin": "^4.28.0",
-        "@typescript-eslint/parser": "^4.28.0",
+        "@typescript-eslint/eslint-plugin": "^5.46.0",
+        "@typescript-eslint/parser": "^5.46.0",
         "acorn": "^7.2.0",
         "babel-eslint": "^10.1.0",
         "css-loader": "^3.2.0",
-        "eslint": "^7.22.0",
+        "eslint": "^8.29.0",
         "eslint-config-prettier": "^6.11.0",
-        "eslint-import-resolver-typescript": "^2.5.0",
+        "eslint-import-resolver-typescript": "^3.5.0",
         "eslint-plugin-es": "^4.1.0",
-        "eslint-plugin-flowtype": "^5.2.0",
+        "eslint-plugin-flowtype": "^8.0.3",
         "eslint-plugin-import": "^2.26.0",
         "eslint-plugin-jsx-a11y": "^6.6.0",
         "eslint-plugin-prettier": "^3.3.1",
         "eslint-plugin-react": "7.30.1",
         "eslint-plugin-react-hooks": "4.6.0",
+        "eslint-plugin-react-refresh": "0.3.4",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
         "prettier": "^2.0.5",
         "rimraf": "^2.6.2",
@@ -57,18 +59,14 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/deephaven/deephaven-ipywidgets",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.6443de594d4e2715e64f.js"
-        },
         "extension": "lib/plugin",
         "outputDir": "deephaven_ipywidgets/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -109,9 +107,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/480.26bcd834ece40109d1df.js` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/480.a275f597035bbcf259ca.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -16,30 +16,30 @@
                     Object.defineProperty(e, "default", {
                         enumerable: !0,
                         value: t
                     })
                 } : function(e, t) {
                     e.default = t
                 }),
-                a = this && this.__importStar || function(e) {
+                s = this && this.__importStar || function(e) {
                     if (e && e.__esModule) return e;
                     var t = {};
                     if (null != e)
                         for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && i(t, e, n);
                     return r(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             });
-            const s = n(565),
-                o = a(n(367)),
+            const a = n(565),
+                o = s(n(367)),
                 l = n(657),
                 d = {
                     id: "@deephaven/ipywidgets:plugin",
-                    requires: [s.IJupyterWidgetRegistry],
+                    requires: [a.IJupyterWidgetRegistry],
                     activate: function(e, t) {
                         t.registerWidget({
                             name: l.MODULE_NAME,
                             version: l.MODULE_VERSION,
                             exports: o
                         })
                     },
@@ -48,88 +48,109 @@
             t.default = d
         },
         657: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const i = n(598);
+            const i = n(147);
             t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
         },
         367: function(e, t, n) {
             "use strict";
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.DeephavenView = t.DeephavenModel = void 0;
             const r = n(565),
-                a = i(n(969)),
-                s = n(657);
+                s = n(429),
+                a = i(n(939)),
+                o = n(657);
             n(204);
-            const o = a.default.module("deephaven-ipywidgets.widget");
-            class l extends r.DOMWidgetModel {
+            const l = a.default.module("deephaven-ipywidgets.widget");
+            class d extends r.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: l.model_name,
-                        _model_module: l.model_module,
-                        _model_module_version: l.model_module_version,
-                        _view_name: l.view_name,
-                        _view_module: l.view_module,
-                        _view_module_version: l.view_module_version
+                        _model_name: d.model_name,
+                        _model_module: d.model_module,
+                        _model_module_version: d.model_module_version,
+                        _view_name: d.view_name,
+                        _view_module: d.view_module,
+                        _view_module_version: d.view_module_version
                     })
                 }
             }
-            t.DeephavenModel = l, l.serializers = Object.assign({}, r.DOMWidgetModel.serializers), l.model_name = "DeephavenModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "DeephavenView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
-            class d extends r.DOMWidgetView {
+            t.DeephavenModel = d, d.serializers = Object.assign({}, r.DOMWidgetModel.serializers), d.model_name = "DeephavenModel", d.model_module = o.MODULE_NAME, d.model_module_version = o.MODULE_VERSION, d.view_name = "DeephavenView", d.view_module = o.MODULE_NAME, d.view_module_version = o.MODULE_VERSION;
+            class u extends r.DOMWidgetView {
+                constructor() {
+                    super(...arguments), this.sendAuthenticationResponse = (e, t, n) => {
+                        const i = {
+                            type: "io.deephaven.proto.auth.Token",
+                            token: this.model.get("token")
+                        };
+                        try {
+                            l.info("Sending login options to iframe", n), t.postMessage(s.makeResponse(e, i), n)
+                        } catch (e) {
+                            l.error(e)
+                        }
+                    }, this.handleAuthentication = e => {
+                        const {
+                            data: t,
+                            source: n,
+                            origin: i
+                        } = e;
+                        null == n || n instanceof MessagePort || n instanceof ServiceWorker || n !== this.iframe.contentWindow ? l.debug("Ignore message, invalid event source", n) : s.isMessage(t) ? t.message === s.LOGIN_OPTIONS_REQUEST ? this.sendAuthenticationResponse(t.id, n, i) : l.debug("Ignore unsupported message", t.message) : l.debug("Ignore unsupported message", t)
+                    }
+                }
                 render() {
                     const e = this.model.get("iframe_url"),
                         t = this.model.get("width"),
                         n = this.model.get("height");
-                    o.info("init_element for widget", e, t, n), this.iframe = document.createElement("iframe"), this.iframe.src = e, t > 0 && (this.iframe.width = t, this.iframe.style.width = `${t}px`), n > 0 && (this.iframe.height = n, this.iframe.style.height = `${n}px`), this.el.className = "deephaven-ipywidgets-widget", this.el.appendChild(this.iframe)
+                    window.addEventListener("message", this.handleAuthentication), l.info("init_element for widget", e, t, n), this.iframe = document.createElement("iframe"), this.iframe.src = e, t > 0 && (this.iframe.width = t, this.iframe.style.width = `${t}px`), n > 0 && (this.iframe.height = n, this.iframe.style.height = `${n}px`), this.el.className = "deephaven-ipywidgets-widget", this.el.appendChild(this.iframe)
                 }
             }
-            t.DeephavenView = d
+            t.DeephavenView = u
         },
         889: (e, t, n) => {
             (t = n(645)(!1)).push([e.id, ".deephaven-ipywidgets-widget {\n  padding: 0;\n  margin: 0;\n}\n\n.deephaven-ipywidgets-widget iframe {\n  border: none;\n  width: 100%;\n}\n\n/** \n * ipywidgets has a white background for objects always, even on a dark theme. \n * Set it to transparent so it looks better in dark themes (like VS Code) \n */\n.cell-output-ipywidget-background {\n  background-color: transparent !important;\n}\n.jp-OutputArea-output {\n  background-color: transparent;\n}", ""]), e.exports = t
         },
         645: e => {
             "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = function(e, t) {
-                            var n, i, r, a = e[1] || "",
-                                s = e[3];
-                            if (!s) return a;
+                            var n, i, r, s = e[1] || "",
+                                a = e[3];
+                            if (!a) return s;
                             if (t && "function" == typeof btoa) {
-                                var o = (n = s, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), r = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(r, " */")),
-                                    l = s.sources.map((function(e) {
-                                        return "/*# sourceURL=".concat(s.sourceRoot || "").concat(e, " */")
+                                var o = (n = a, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), r = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(r, " */")),
+                                    l = a.sources.map((function(e) {
+                                        return "/*# sourceURL=".concat(a.sourceRoot || "").concat(e, " */")
                                     }));
-                                return [a].concat(l).concat([o]).join("\n")
+                                return [s].concat(l).concat([o]).join("\n")
                             }
-                            return [a].join("\n")
+                            return [s].join("\n")
                         }(t, e);
                         return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                     })).join("")
                 }, t.i = function(e, n, i) {
                     "string" == typeof e && (e = [
                         [null, e, ""]
                     ]);
                     var r = {};
                     if (i)
-                        for (var a = 0; a < this.length; a++) {
-                            var s = this[a][0];
-                            null != s && (r[s] = !0)
+                        for (var s = 0; s < this.length; s++) {
+                            var a = this[s][0];
+                            null != a && (r[a] = !0)
                         }
                     for (var o = 0; o < e.length; o++) {
                         var l = [].concat(e[o]);
                         i && r[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
                     }
                 }, t
             }
@@ -158,94 +179,94 @@
                                 n = null
                             }
                             e[t] = n
                         }
                         return e[t]
                     }
                 }(),
-                a = [];
+                s = [];
 
-            function s(e) {
-                for (var t = -1, n = 0; n < a.length; n++)
-                    if (a[n].identifier === e) {
+            function a(e) {
+                for (var t = -1, n = 0; n < s.length; n++)
+                    if (s[n].identifier === e) {
                         t = n;
                         break
                     } return t
             }
 
             function o(e, t) {
                 for (var n = {}, i = [], r = 0; r < e.length; r++) {
                     var o = e[r],
                         l = t.base ? o[0] + t.base : o[0],
                         d = n[l] || 0,
                         u = "".concat(l, " ").concat(d);
                     n[l] = d + 1;
-                    var c = s(u),
+                    var c = a(u),
                         p = {
                             css: o[1],
                             media: o[2],
                             sourceMap: o[3]
-                        }; - 1 !== c ? (a[c].references++, a[c].updater(p)) : a.push({
+                        }; - 1 !== c ? (s[c].references++, s[c].updater(p)) : s.push({
                         identifier: u,
                         updater: b(p, t),
                         references: 1
                     }), i.push(u)
                 }
                 return i
             }
 
             function l(e) {
                 var t = document.createElement("style"),
                     i = e.attributes || {};
                 if (void 0 === i.nonce) {
-                    var a = n.nc;
-                    a && (i.nonce = a)
+                    var s = n.nc;
+                    s && (i.nonce = s)
                 }
                 if (Object.keys(i).forEach((function(e) {
                         t.setAttribute(e, i[e])
                     })), "function" == typeof e.insert) e.insert(t);
                 else {
-                    var s = r(e.insert || "head");
-                    if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    s.appendChild(t)
+                    var a = r(e.insert || "head");
+                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    a.appendChild(t)
                 }
                 return t
             }
             var d, u = (d = [], function(e, t) {
                 return d[e] = t, d.filter(Boolean).join("\n")
             });
 
             function c(e, t, n, i) {
                 var r = n ? "" : i.media ? "@media ".concat(i.media, " {").concat(i.css, "}") : i.css;
                 if (e.styleSheet) e.styleSheet.cssText = u(t, r);
                 else {
-                    var a = document.createTextNode(r),
-                        s = e.childNodes;
-                    s[t] && e.removeChild(s[t]), s.length ? e.insertBefore(a, s[t]) : e.appendChild(a)
+                    var s = document.createTextNode(r),
+                        a = e.childNodes;
+                    a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(s, a[t]) : e.appendChild(s)
                 }
             }
 
             function p(e, t, n) {
                 var i = n.css,
                     r = n.media,
-                    a = n.sourceMap;
-                if (r ? e.setAttribute("media", r) : e.removeAttribute("media"), a && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
+                    s = n.sourceMap;
+                if (r ? e.setAttribute("media", r) : e.removeAttribute("media"), s && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(s)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
                 else {
                     for (; e.firstChild;) e.removeChild(e.firstChild);
                     e.appendChild(document.createTextNode(i))
                 }
             }
             var h = null,
                 f = 0;
 
             function b(e, t) {
                 var n, i, r;
                 if (t.singleton) {
-                    var a = f++;
-                    n = h || (h = l(t)), i = c.bind(null, n, a, !1), r = c.bind(null, n, a, !0)
+                    var s = f++;
+                    n = h || (h = l(t)), i = c.bind(null, n, s, !1), r = c.bind(null, n, s, !0)
                 } else n = l(t), i = p.bind(null, n, t), r = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(n)
                 };
                 return i(e),
@@ -258,25 +279,25 @@
             }
             e.exports = function(e, t) {
                 (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === i && (i = Boolean(window && document && document.all && !window.atob)), i));
                 var n = o(e = e || [], t);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var i = 0; i < n.length; i++) {
-                            var r = s(n[i]);
-                            a[r].references--
+                            var r = a(n[i]);
+                            s[r].references--
                         }
                         for (var l = o(e, t), d = 0; d < n.length; d++) {
-                            var u = s(n[d]);
-                            0 === a[u].references && (a[u].updater(), a.splice(u, 1))
+                            var u = a(n[d]);
+                            0 === s[u].references && (s[u].updater(), s.splice(u, 1))
                         }
                         n = l
                     }
                 }
             }
         },
-        598: e => {
+        147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.1.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"0.15.0","@deephaven/log":"0.15.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"0.15.0","@deephaven/prettier-config":"0.15.0","@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^4.28.0","@typescript-eslint/parser":"^4.28.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^7.22.0","eslint-import-resolver-typescript":"^2.5.0","eslint-config-prettier":"^6.11.0","eslint-plugin-import":"^2.26.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^5.2.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
+            e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.2.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"^0.41.0","@deephaven/jsapi-utils":"^0.41.3","@deephaven/log":"^0.41.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"^0.41.0","@deephaven/prettier-config":"^0.41.0","@jupyterlab/builder":"^3.6.4","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.46.0","@typescript-eslint/parser":"^5.46.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^8.29.0","eslint-config-prettier":"^6.11.0","eslint-import-resolver-typescript":"^3.5.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^8.0.3","eslint-plugin-import":"^2.26.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","eslint-plugin-react-refresh":"0.3.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
         }
     }
 ]);
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/568.8c7c3ea60a12c60e6eb1.js` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/568.7551298c61415e9b2969.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -8,247 +8,268 @@
                         get: function() {
                             return t[n]
                         }
                     })
                 } : function(e, t, n, i) {
                     void 0 === i && (i = n), e[i] = t[n]
                 }),
-                r = this && this.__exportStar || function(e, t) {
+                s = this && this.__exportStar || function(e, t) {
                     for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || i(t, e, n)
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), r(n(657), t), r(n(367), t)
+            }), s(n(657), t), s(n(367), t)
         },
         657: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const i = n(598);
+            const i = n(147);
             t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
         },
         367: function(e, t, n) {
             "use strict";
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.DeephavenView = t.DeephavenModel = void 0;
-            const r = n(565),
-                a = i(n(969)),
-                s = n(657);
+            const s = n(565),
+                r = n(429),
+                a = i(n(939)),
+                o = n(657);
             n(204);
-            const o = a.default.module("deephaven-ipywidgets.widget");
-            class l extends r.DOMWidgetModel {
+            const l = a.default.module("deephaven-ipywidgets.widget");
+            class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: l.model_name,
-                        _model_module: l.model_module,
-                        _model_module_version: l.model_module_version,
-                        _view_name: l.view_name,
-                        _view_module: l.view_module,
-                        _view_module_version: l.view_module_version
+                        _model_name: d.model_name,
+                        _model_module: d.model_module,
+                        _model_module_version: d.model_module_version,
+                        _view_name: d.view_name,
+                        _view_module: d.view_module,
+                        _view_module_version: d.view_module_version
                     })
                 }
             }
-            t.DeephavenModel = l, l.serializers = Object.assign({}, r.DOMWidgetModel.serializers), l.model_name = "DeephavenModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "DeephavenView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
-            class d extends r.DOMWidgetView {
+            t.DeephavenModel = d, d.serializers = Object.assign({}, s.DOMWidgetModel.serializers), d.model_name = "DeephavenModel", d.model_module = o.MODULE_NAME, d.model_module_version = o.MODULE_VERSION, d.view_name = "DeephavenView", d.view_module = o.MODULE_NAME, d.view_module_version = o.MODULE_VERSION;
+            class u extends s.DOMWidgetView {
+                constructor() {
+                    super(...arguments), this.sendAuthenticationResponse = (e, t, n) => {
+                        const i = {
+                            type: "io.deephaven.proto.auth.Token",
+                            token: this.model.get("token")
+                        };
+                        try {
+                            l.info("Sending login options to iframe", n), t.postMessage(r.makeResponse(e, i), n)
+                        } catch (e) {
+                            l.error(e)
+                        }
+                    }, this.handleAuthentication = e => {
+                        const {
+                            data: t,
+                            source: n,
+                            origin: i
+                        } = e;
+                        null == n || n instanceof MessagePort || n instanceof ServiceWorker || n !== this.iframe.contentWindow ? l.debug("Ignore message, invalid event source", n) : r.isMessage(t) ? t.message === r.LOGIN_OPTIONS_REQUEST ? this.sendAuthenticationResponse(t.id, n, i) : l.debug("Ignore unsupported message", t.message) : l.debug("Ignore unsupported message", t)
+                    }
+                }
                 render() {
                     const e = this.model.get("iframe_url"),
                         t = this.model.get("width"),
                         n = this.model.get("height");
-                    o.info("init_element for widget", e, t, n), this.iframe = document.createElement("iframe"), this.iframe.src = e, t > 0 && (this.iframe.width = t, this.iframe.style.width = `${t}px`), n > 0 && (this.iframe.height = n, this.iframe.style.height = `${n}px`), this.el.className = "deephaven-ipywidgets-widget", this.el.appendChild(this.iframe)
+                    window.addEventListener("message", this.handleAuthentication), l.info("init_element for widget", e, t, n), this.iframe = document.createElement("iframe"), this.iframe.src = e, t > 0 && (this.iframe.width = t, this.iframe.style.width = `${t}px`), n > 0 && (this.iframe.height = n, this.iframe.style.height = `${n}px`), this.el.className = "deephaven-ipywidgets-widget", this.el.appendChild(this.iframe)
                 }
             }
-            t.DeephavenView = d
+            t.DeephavenView = u
         },
         889: (e, t, n) => {
             (t = n(645)(!1)).push([e.id, ".deephaven-ipywidgets-widget {\n  padding: 0;\n  margin: 0;\n}\n\n.deephaven-ipywidgets-widget iframe {\n  border: none;\n  width: 100%;\n}\n\n/** \n * ipywidgets has a white background for objects always, even on a dark theme. \n * Set it to transparent so it looks better in dark themes (like VS Code) \n */\n.cell-output-ipywidget-background {\n  background-color: transparent !important;\n}\n.jp-OutputArea-output {\n  background-color: transparent;\n}", ""]), e.exports = t
         },
         645: e => {
             "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = function(e, t) {
-                            var n, i, r, a = e[1] || "",
-                                s = e[3];
-                            if (!s) return a;
+                            var n, i, s, r = e[1] || "",
+                                a = e[3];
+                            if (!a) return r;
                             if (t && "function" == typeof btoa) {
-                                var o = (n = s, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), r = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(r, " */")),
-                                    l = s.sources.map((function(e) {
-                                        return "/*# sourceURL=".concat(s.sourceRoot || "").concat(e, " */")
+                                var o = (n = a, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(s, " */")),
+                                    l = a.sources.map((function(e) {
+                                        return "/*# sourceURL=".concat(a.sourceRoot || "").concat(e, " */")
                                     }));
-                                return [a].concat(l).concat([o]).join("\n")
+                                return [r].concat(l).concat([o]).join("\n")
                             }
-                            return [a].join("\n")
+                            return [r].join("\n")
                         }(t, e);
                         return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                     })).join("")
                 }, t.i = function(e, n, i) {
                     "string" == typeof e && (e = [
                         [null, e, ""]
                     ]);
-                    var r = {};
+                    var s = {};
                     if (i)
-                        for (var a = 0; a < this.length; a++) {
-                            var s = this[a][0];
-                            null != s && (r[s] = !0)
+                        for (var r = 0; r < this.length; r++) {
+                            var a = this[r][0];
+                            null != a && (s[a] = !0)
                         }
                     for (var o = 0; o < e.length; o++) {
                         var l = [].concat(e[o]);
-                        i && r[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
+                        i && s[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
                     }
                 }, t
             }
         },
         204: (e, t, n) => {
             var i = n(379),
-                r = n(889);
-            "string" == typeof(r = r.__esModule ? r.default : r) && (r = [
-                [e.id, r, ""]
+                s = n(889);
+            "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
+                [e.id, s, ""]
             ]);
-            i(r, {
+            i(s, {
                 insert: "head",
                 singleton: !1
-            }), e.exports = r.locals || {}
+            }), e.exports = s.locals || {}
         },
         379: (e, t, n) => {
             "use strict";
-            var i, r = function() {
+            var i, s = function() {
                     var e = {};
                     return function(t) {
                         if (void 0 === e[t]) {
                             var n = document.querySelector(t);
                             if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                                 n = n.contentDocument.head
                             } catch (e) {
                                 n = null
                             }
                             e[t] = n
                         }
                         return e[t]
                     }
                 }(),
-                a = [];
+                r = [];
 
-            function s(e) {
-                for (var t = -1, n = 0; n < a.length; n++)
-                    if (a[n].identifier === e) {
+            function a(e) {
+                for (var t = -1, n = 0; n < r.length; n++)
+                    if (r[n].identifier === e) {
                         t = n;
                         break
                     } return t
             }
 
             function o(e, t) {
-                for (var n = {}, i = [], r = 0; r < e.length; r++) {
-                    var o = e[r],
+                for (var n = {}, i = [], s = 0; s < e.length; s++) {
+                    var o = e[s],
                         l = t.base ? o[0] + t.base : o[0],
                         d = n[l] || 0,
                         u = "".concat(l, " ").concat(d);
                     n[l] = d + 1;
-                    var c = s(u),
+                    var c = a(u),
                         p = {
                             css: o[1],
                             media: o[2],
                             sourceMap: o[3]
-                        }; - 1 !== c ? (a[c].references++, a[c].updater(p)) : a.push({
+                        }; - 1 !== c ? (r[c].references++, r[c].updater(p)) : r.push({
                         identifier: u,
                         updater: b(p, t),
                         references: 1
                     }), i.push(u)
                 }
                 return i
             }
 
             function l(e) {
                 var t = document.createElement("style"),
                     i = e.attributes || {};
                 if (void 0 === i.nonce) {
-                    var a = n.nc;
-                    a && (i.nonce = a)
+                    var r = n.nc;
+                    r && (i.nonce = r)
                 }
                 if (Object.keys(i).forEach((function(e) {
                         t.setAttribute(e, i[e])
                     })), "function" == typeof e.insert) e.insert(t);
                 else {
-                    var s = r(e.insert || "head");
-                    if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    s.appendChild(t)
+                    var a = s(e.insert || "head");
+                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    a.appendChild(t)
                 }
                 return t
             }
             var d, u = (d = [], function(e, t) {
                 return d[e] = t, d.filter(Boolean).join("\n")
             });
 
             function c(e, t, n, i) {
-                var r = n ? "" : i.media ? "@media ".concat(i.media, " {").concat(i.css, "}") : i.css;
-                if (e.styleSheet) e.styleSheet.cssText = u(t, r);
+                var s = n ? "" : i.media ? "@media ".concat(i.media, " {").concat(i.css, "}") : i.css;
+                if (e.styleSheet) e.styleSheet.cssText = u(t, s);
                 else {
-                    var a = document.createTextNode(r),
-                        s = e.childNodes;
-                    s[t] && e.removeChild(s[t]), s.length ? e.insertBefore(a, s[t]) : e.appendChild(a)
+                    var r = document.createTextNode(s),
+                        a = e.childNodes;
+                    a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(r, a[t]) : e.appendChild(r)
                 }
             }
 
             function p(e, t, n) {
                 var i = n.css,
-                    r = n.media,
-                    a = n.sourceMap;
-                if (r ? e.setAttribute("media", r) : e.removeAttribute("media"), a && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
+                    s = n.media,
+                    r = n.sourceMap;
+                if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
                 else {
                     for (; e.firstChild;) e.removeChild(e.firstChild);
                     e.appendChild(document.createTextNode(i))
                 }
             }
             var h = null,
                 f = 0;
 
             function b(e, t) {
-                var n, i, r;
+                var n, i, s;
                 if (t.singleton) {
-                    var a = f++;
-                    n = h || (h = l(t)), i = c.bind(null, n, a, !1), r = c.bind(null, n, a, !0)
-                } else n = l(t), i = p.bind(null, n, t), r = function() {
+                    var r = f++;
+                    n = h || (h = l(t)), i = c.bind(null, n, r, !1), s = c.bind(null, n, r, !0)
+                } else n = l(t), i = p.bind(null, n, t), s = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(n)
                 };
                 return i(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
                             i(e = t)
-                        } else r()
+                        } else s()
                     }
             }
             e.exports = function(e, t) {
                 (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === i && (i = Boolean(window && document && document.all && !window.atob)), i));
                 var n = o(e = e || [], t);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var i = 0; i < n.length; i++) {
-                            var r = s(n[i]);
-                            a[r].references--
+                            var s = a(n[i]);
+                            r[s].references--
                         }
                         for (var l = o(e, t), d = 0; d < n.length; d++) {
-                            var u = s(n[d]);
-                            0 === a[u].references && (a[u].updater(), a.splice(u, 1))
+                            var u = a(n[d]);
+                            0 === r[u].references && (r[u].updater(), r.splice(u, 1))
                         }
                         n = l
                     }
                 }
             }
         },
-        598: e => {
+        147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.1.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"0.15.0","@deephaven/log":"0.15.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"0.15.0","@deephaven/prettier-config":"0.15.0","@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^4.28.0","@typescript-eslint/parser":"^4.28.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^7.22.0","eslint-import-resolver-typescript":"^2.5.0","eslint-config-prettier":"^6.11.0","eslint-plugin-import":"^2.26.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^5.2.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
+            e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.2.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"^0.41.0","@deephaven/jsapi-utils":"^0.41.3","@deephaven/log":"^0.41.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"^0.41.0","@deephaven/prettier-config":"^0.41.0","@jupyterlab/builder":"^3.6.4","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.46.0","@typescript-eslint/parser":"^5.46.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^8.29.0","eslint-config-prettier":"^6.11.0","eslint-import-resolver-typescript":"^3.5.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^8.0.3","eslint-plugin-import":"^2.26.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","eslint-plugin-react-refresh":"0.3.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
         }
     }
 ]);
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/701.6f39578fffe6bd3cfc48.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,54 +1,84 @@
 (self.webpackChunk_deephaven_ipywidgets = self.webpackChunk_deephaven_ipywidgets || []).push([
     [701], {
         701: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Log: () => a,
-                LogHistory: () => ie,
+                LogHistory: () => se,
                 LogProxy: () => re,
                 Logger: () => s,
                 LoggerLevel: () => r,
-                default: () => a
+                default: () => ae
             });
             const r = Object.freeze({
                 SILENT: -1,
                 ERROR: 0,
                 WARN: 1,
                 INFO: 2,
                 DEBUG: 3,
                 DEBUG2: 4
             });
-            var o = () => {};
+
+            function o(e, t, n) {
+                return (t = function(e) {
+                    var t = function(e, t) {
+                        if ("object" != typeof e || null === e) return e;
+                        var n = e[Symbol.toPrimitive];
+                        if (void 0 !== n) {
+                            var r = n.call(e, "string");
+                            if ("object" != typeof r) return r;
+                            throw new TypeError("@@toPrimitive must return a primitive value.")
+                        }
+                        return String(e)
+                    }(e);
+                    return "symbol" == typeof t ? t : String(t)
+                }(t)) in e ? Object.defineProperty(e, t, {
+                    value: n,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : e[t] = n, e
+            }
+            var i = () => {};
             const s = class {
                 constructor(e, t) {
-                    this.name = e, this.prefix = e ? "[".concat(e, "]") : "", this.setLogLevel(t)
+                    o(this, "name", void 0), o(this, "prefix", void 0), o(this, "level", void 0), o(this, "error", void 0), o(this, "warn", void 0), o(this, "log", void 0), o(this, "info", void 0), o(this, "debug", void 0), o(this, "debug2", void 0), this.name = e, this.prefix = null != e ? "[".concat(e, "]") : "", this.error = i, this.warn = i, this.log = i, this.info = i, this.debug = i, this.debug2 = i, this.level = t, this.setLogLevel(t)
                 }
                 setLogLevel(e) {
-                    this.level = e, this.error = 0 <= e ? console.error.bind(console, this.prefix) : o, this.warn = 1 <= e ? console.warn.bind(console, this.prefix) : o, this.log = 2 <= e ? console.log.bind(console, this.prefix) : o, this.info = this.log, this.debug = 3 <= e ? console.debug.bind(console, this.prefix) : o, this.debug2 = 4 <= e ? console.debug.bind(console, this.prefix) : o
+                    Number.isFinite(e) ? (this.level = e, this.error = e >= 0 ? console.error.bind(console, this.prefix) : i, this.warn = e >= 1 ? console.warn.bind(console, this.prefix) : i, this.log = e >= 2 ? console.log.bind(console, this.prefix) : i, this.info = this.log, this.debug = e >= 3 ? console.debug.bind(console, this.prefix) : i, this.debug2 = e >= 4 ? console.debug.bind(console, this.prefix) : i) : console.warn("Expected a number for log level. Received: ".concat(e, ". Ignoring"))
                 }
             };
-            var i = n(155);
             const a = new class extends s {
                 constructor() {
-                    super(null, arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : function() {
-                        var e, t = "";
-                        try {
-                            t = i.env.DEEPHAVEN_LOG_LEVEL
-                        } catch (e) {}
-                        if (t && r[t]) return r[t];
-                        var n = parseInt(null !== (e = t) && void 0 !== e ? e : "", 10);
-                        return Number.isNaN(n) ? 2 : n
-                    }()), this.modules = {}
+                    var e, t, n;
+                    super(null, arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 2), e = this, n = void 0, (t = function(e) {
+                        var t = function(e, t) {
+                            if ("object" != typeof e || null === e) return e;
+                            var n = e[Symbol.toPrimitive];
+                            if (void 0 !== n) {
+                                var r = n.call(e, "string");
+                                if ("object" != typeof r) return r;
+                                throw new TypeError("@@toPrimitive must return a primitive value.")
+                            }
+                            return String(e)
+                        }(e);
+                        return "symbol" == typeof t ? t : String(t)
+                    }(t = "modules")) in e ? Object.defineProperty(e, t, {
+                        value: n,
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0
+                    }) : e[t] = n, this.modules = {}
                 }
                 module(e) {
-                    return this.modules[e] || (this.modules[e] = new s(e, this.level)), this.modules[e]
+                    return null == this.modules[e] && (this.modules[e] = new s(e, this.level)), this.modules[e]
                 }
                 setLogLevel(e) {
-                    if (super.setLogLevel(e), this.modules)
+                    if (super.setLogLevel(e), null != this.modules)
                         for (var t = Object.keys(this.modules), n = 0; n < t.length; n += 1) this.modules[t[n]].setLogLevel(e)
                 }
             };
             var l = n(155);
 
             function c(e, t, ...n) {
                 if (!e) throw new TypeError(u(t, n))
@@ -59,46 +89,46 @@
                 return e.replace(/%[os]/gu, (() => p(t[n++])))
             }
 
             function p(e) {
                 return "object" != typeof e || null === e ? String(e) : Object.prototype.toString.call(e)
             }
             const h = "undefined" != typeof window ? window : "undefined" != typeof self ? self : void 0 !== n.g ? n.g : "undefined" != typeof globalThis ? globalThis : void 0;
-            let g;
-            class d {
+            let d;
+            class g {
                 constructor(e, t) {
                     this.code = e, this.message = t
                 }
                 warn(...e) {
                     var t;
                     try {
-                        g;
+                        d;
                         const n = (null !== (t = (new Error).stack) && void 0 !== t ? t : "").replace(/^(?:.+?\n){2}/gu, "\n");
                         console.warn(this.message, ...e, n)
                     } catch (e) {}
                 }
             }
-            const f = new d("W01", "Unable to initialize event under dispatching."),
-                b = new d("W02", "Assigning any falsy value to 'cancelBubble' property has no effect."),
-                v = new d("W03", "Assigning any truthy value to 'returnValue' property has no effect."),
-                E = new d("W04", "Unable to preventDefault on non-cancelable events."),
-                y = new d("W05", "Unable to preventDefault inside passive event listener invocation."),
-                m = new d("W06", "An event listener wasn't added because it has been added already: %o, %o"),
-                R = new d("W07", "The %o option value was abandoned because the event listener wasn't added as duplicated."),
-                w = new d("W08", "The 'callback' argument must be a function or an object that has 'handleEvent' method: %o");
-            new d("W09", "Event attribute handler must be a function: %o");
+            const f = new g("W01", "Unable to initialize event under dispatching."),
+                v = new g("W02", "Assigning any falsy value to 'cancelBubble' property has no effect."),
+                b = new g("W03", "Assigning any truthy value to 'returnValue' property has no effect."),
+                E = new g("W04", "Unable to preventDefault on non-cancelable events."),
+                y = new g("W05", "Unable to preventDefault inside passive event listener invocation."),
+                m = new g("W06", "An event listener wasn't added because it has been added already: %o, %o"),
+                R = new g("W07", "The %o option value was abandoned because the event listener wasn't added as duplicated."),
+                w = new g("W08", "The 'callback' argument must be a function or an object that has 'handleEvent' method: %o");
+            new g("W09", "Event attribute handler must be a function: %o");
             class T {
                 static get NONE() {
                     return O
                 }
                 static get CAPTURING_PHASE() {
-                    return L
+                    return P
                 }
                 static get AT_TARGET() {
-                    return P
+                    return L
                 }
                 static get BUBBLING_PHASE() {
                     return _
                 }
                 constructor(e, t) {
                     Object.defineProperty(this, "isTrusted", {
                         value: !1,
@@ -117,127 +147,127 @@
                         canceledFlag: !1,
                         inPassiveListenerFlag: !1,
                         dispatchFlag: !1,
                         timeStamp: Date.now()
                     })
                 }
                 get type() {
-                    return N(this).type
+                    return S(this).type
                 }
                 get target() {
-                    return N(this).target
+                    return S(this).target
                 }
                 get srcElement() {
-                    return N(this).target
+                    return S(this).target
                 }
                 get currentTarget() {
-                    return N(this).currentTarget
+                    return S(this).currentTarget
                 }
                 composedPath() {
-                    const e = N(this).currentTarget;
+                    const e = S(this).currentTarget;
                     return e ? [e] : []
                 }
                 get NONE() {
                     return O
                 }
                 get CAPTURING_PHASE() {
-                    return L
+                    return P
                 }
                 get AT_TARGET() {
-                    return P
+                    return L
                 }
                 get BUBBLING_PHASE() {
                     return _
                 }
                 get eventPhase() {
-                    return N(this).dispatchFlag ? 2 : 0
+                    return S(this).dispatchFlag ? 2 : 0
                 }
                 stopPropagation() {
-                    N(this).stopPropagationFlag = !0
+                    S(this).stopPropagationFlag = !0
                 }
                 get cancelBubble() {
-                    return N(this).stopPropagationFlag
+                    return S(this).stopPropagationFlag
                 }
                 set cancelBubble(e) {
-                    e ? N(this).stopPropagationFlag = !0 : b.warn()
+                    e ? S(this).stopPropagationFlag = !0 : v.warn()
                 }
                 stopImmediatePropagation() {
-                    const e = N(this);
+                    const e = S(this);
                     e.stopPropagationFlag = e.stopImmediatePropagationFlag = !0
                 }
                 get bubbles() {
-                    return N(this).bubbles
+                    return S(this).bubbles
                 }
                 get cancelable() {
-                    return N(this).cancelable
+                    return S(this).cancelable
                 }
                 get returnValue() {
-                    return !N(this).canceledFlag
+                    return !S(this).canceledFlag
                 }
                 set returnValue(e) {
-                    e ? v.warn() : I(N(this))
+                    e ? b.warn() : j(S(this))
                 }
                 preventDefault() {
-                    I(N(this))
+                    j(S(this))
                 }
                 get defaultPrevented() {
-                    return N(this).canceledFlag
+                    return S(this).canceledFlag
                 }
                 get composed() {
-                    return N(this).composed
+                    return S(this).composed
                 }
                 get isTrusted() {
                     return !1
                 }
                 get timeStamp() {
-                    return N(this).timeStamp
+                    return S(this).timeStamp
                 }
                 initEvent(e, t = !1, n = !1) {
-                    const r = N(this);
+                    const r = S(this);
                     r.dispatchFlag ? f.warn() : A.set(this, {
                         ...r,
                         type: String(e),
                         bubbles: Boolean(t),
                         cancelable: Boolean(n),
                         target: null,
                         currentTarget: null,
                         stopPropagationFlag: !1,
                         stopImmediatePropagationFlag: !1,
                         canceledFlag: !1
                     })
                 }
             }
             const O = 0,
-                L = 1,
-                P = 2,
+                P = 1,
+                L = 2,
                 _ = 3,
                 A = new WeakMap;
 
-            function N(e, t = "this") {
+            function S(e, t = "this") {
                 const n = A.get(e);
                 return c(null != n, "'%s' must be an object that Event constructor created, but got another one: %o", t, e), n
             }
 
-            function I(e) {
+            function j(e) {
                 e.inPassiveListenerFlag ? y.warn() : e.cancelable ? e.canceledFlag = !0 : E.warn()
             }
             Object.defineProperty(T, "NONE", {
                 enumerable: !0
             }), Object.defineProperty(T, "CAPTURING_PHASE", {
                 enumerable: !0
             }), Object.defineProperty(T, "AT_TARGET", {
                 enumerable: !0
             }), Object.defineProperty(T, "BUBBLING_PHASE", {
                 enumerable: !0
             });
-            const S = Object.getOwnPropertyNames(T.prototype);
-            for (let e = 0; e < S.length; ++e) "constructor" !== S[e] && Object.defineProperty(T.prototype, S[e], {
+            const N = Object.getOwnPropertyNames(T.prototype);
+            for (let e = 0; e < N.length; ++e) "constructor" !== N[e] && Object.defineProperty(T.prototype, N[e], {
                 enumerable: !0
             });
-            let D;
+            let I;
             void 0 !== h && void 0 !== h.Event && Object.setPrototypeOf(T.prototype, h.Event.prototype);
             const U = {
                 INDEX_SIZE_ERR: 1,
                 DOMSTRING_SIZE_ERR: 2,
                 HIERARCHY_REQUEST_ERR: 3,
                 WRONG_DOCUMENT_ERR: 4,
                 INVALID_CHARACTER_ERR: 5,
@@ -259,15 +289,15 @@
                 URL_MISMATCH_ERR: 21,
                 QUOTA_EXCEEDED_ERR: 22,
                 TIMEOUT_ERR: 23,
                 INVALID_NODE_TYPE_ERR: 24,
                 DATA_CLONE_ERR: 25
             };
 
-            function j(e) {
+            function D(e) {
                 const t = Object.keys(U);
                 for (let n = 0; n < t.length; ++n) {
                     const r = t[n],
                         o = U[r];
                     Object.defineProperty(e, r, {
                         get: () => o,
                         configurable: !0,
@@ -286,102 +316,102 @@
                         composed: e.composed
                     }), e.cancelBubble && super.stopPropagation(), e.defaultPrevented && super.preventDefault(), k.set(this, {
                         original: e
                     });
                     const t = Object.keys(e);
                     for (let n = 0; n < t.length; ++n) {
                         const r = t[n];
-                        r in this || Object.defineProperty(this, r, G(e, r))
+                        r in this || Object.defineProperty(this, r, C(e, r))
                     }
                 }
                 stopPropagation() {
                     super.stopPropagation();
                     const {
                         original: e
-                    } = H(this);
+                    } = F(this);
                     "stopPropagation" in e && e.stopPropagation()
                 }
                 get cancelBubble() {
                     return super.cancelBubble
                 }
                 set cancelBubble(e) {
                     super.cancelBubble = e;
                     const {
                         original: t
-                    } = H(this);
+                    } = F(this);
                     "cancelBubble" in t && (t.cancelBubble = e)
                 }
                 stopImmediatePropagation() {
                     super.stopImmediatePropagation();
                     const {
                         original: e
-                    } = H(this);
+                    } = F(this);
                     "stopImmediatePropagation" in e && e.stopImmediatePropagation()
                 }
                 get returnValue() {
                     return super.returnValue
                 }
                 set returnValue(e) {
                     super.returnValue = e;
                     const {
                         original: t
-                    } = H(this);
+                    } = F(this);
                     "returnValue" in t && (t.returnValue = e)
                 }
                 preventDefault() {
                     super.preventDefault();
                     const {
                         original: e
-                    } = H(this);
+                    } = F(this);
                     "preventDefault" in e && e.preventDefault()
                 }
                 get timeStamp() {
                     const {
                         original: e
-                    } = H(this);
+                    } = F(this);
                     return "timeStamp" in e ? e.timeStamp : super.timeStamp
                 }
             }
             const k = new WeakMap;
 
-            function H(e) {
+            function F(e) {
                 const t = k.get(e);
                 return c(null != t, "'this' is expected an Event object, but got", e), t
             }
-            const F = new WeakMap;
+            const H = new WeakMap;
 
             function x(e) {
                 const t = Object.getPrototypeOf(e);
                 if (null == t) return B;
-                let n = F.get(t);
+                let n = H.get(t);
                 return null == n && (n = function(e, t) {
                     class n extends e {}
                     const r = Object.keys(t);
-                    for (let e = 0; e < r.length; ++e) Object.defineProperty(n.prototype, r[e], G(t, r[e]));
+                    for (let e = 0; e < r.length; ++e) Object.defineProperty(n.prototype, r[e], C(t, r[e]));
                     return n
-                }(x(t), t), F.set(t, n)), n
+                }(x(t), t), H.set(t, n)), n
             }
 
-            function G(e, t) {
+            function C(e, t) {
                 const n = Object.getOwnPropertyDescriptor(e, t);
                 return {
                     get() {
-                        const e = H(this).original,
+                        const e = F(this).original,
                             n = e[t];
                         return "function" == typeof n ? n.bind(e) : n
                     },
                     set(e) {
-                        H(this).original[t] = e
+                        F(this).original[t] = e
                     },
                     configurable: n.configurable,
                     enumerable: n.enumerable
                 }
             }
 
-            function C(e) {
+            function G(e) {
                 return 1 == (1 & e.flags)
             }
 
             function W(e) {
                 return 2 == (2 & e.flags)
             }
 
@@ -413,40 +443,40 @@
                 }
             }
 
             function X({
                 listeners: e
             }, t, n) {
                 for (let r = 0; r < e.length; ++r)
-                    if (e[r].callback === t && C(e[r]) === n) return r;
+                    if (e[r].callback === t && G(e[r]) === n) return r;
                 return -1
             }
 
             function z(e, t, n) {
                 const r = X(e, t, n);
                 return -1 !== r && Q(e, r)
             }
 
             function Q(e, t, n = !1) {
                 const r = e.listeners[t];
                 return function(e) {
                     e.flags |= 8
                 }(r), r.signal && r.signal.removeEventListener("abort", r.signalListener), e.cow && !n ? (e.cow = !1, e.listeners = e.listeners.filter(((e, n) => n !== t)), !1) : (e.listeners.splice(t, 1), !0)
             }
-            F.set(Object.prototype, B), void 0 !== h && void 0 !== h.Event && F.set(h.Event.prototype, B);
+            H.set(Object.prototype, B), void 0 !== h && void 0 !== h.Event && H.set(h.Event.prototype, B);
             class Z {
                 constructor() {
                     J.set(this, Object.create(null))
                 }
                 addEventListener(e, t, n) {
                     const r = K(this),
                         {
                             callback: o,
-                            capture: s,
-                            once: i,
+                            capture: i,
+                            once: s,
                             passive: a,
                             signal: l,
                             type: c
                         } = function(e, t, n) {
                             var r;
                             return q(t), "object" == typeof n && null !== n ? {
                                 type: String(e),
@@ -470,83 +500,83 @@
                             return null !== (n = e[t]) && void 0 !== n ? n : e[t] = {
                                 attrCallback: void 0,
                                 attrListener: void 0,
                                 cow: !1,
                                 listeners: []
                             }
                         }(r, c),
-                        p = X(u, o, s); - 1 === p ? function(e, t, n, r, o, s) {
-                        let i;
-                        s && (i = z.bind(null, e, t, n), s.addEventListener("abort", i));
-                        const a = function(e, t, n, r, o, s) {
+                        p = X(u, o, i); - 1 === p ? function(e, t, n, r, o, i) {
+                        let s;
+                        i && (s = z.bind(null, e, t, n), i.addEventListener("abort", s));
+                        const a = function(e, t, n, r, o, i) {
                             return {
                                 callback: e,
                                 flags: (t ? 1 : 0) | (n ? 2 : 0) | (r ? 4 : 0),
                                 signal: o,
-                                signalListener: s
+                                signalListener: i
                             }
-                        }(t, n, r, o, s, i);
+                        }(t, n, r, o, i, s);
                         e.cow ? (e.cow = !1, e.listeners = [...e.listeners, a]) : e.listeners.push(a)
-                    }(u, o, s, a, i, l) : function(e, t, n, r) {
-                        m.warn(C(e) ? "capture" : "bubble", e.callback), W(e) !== t && R.warn("passive"), M(e) !== n && R.warn("once"), e.signal !== r && R.warn("signal")
-                    }(u.listeners[p], a, i, l)
+                    }(u, o, i, a, s, l) : function(e, t, n, r) {
+                        m.warn(G(e) ? "capture" : "bubble", e.callback), W(e) !== t && R.warn("passive"), M(e) !== n && R.warn("once"), e.signal !== r && R.warn("signal")
+                    }(u.listeners[p], a, s, l)
                 }
                 removeEventListener(e, t, n) {
                     const r = K(this),
                         {
                             callback: o,
-                            capture: s,
-                            type: i
+                            capture: i,
+                            type: s
                         } = function(e, t, n) {
                             return q(t), "object" == typeof n && null !== n ? {
                                 type: String(e),
                                 callback: null != t ? t : void 0,
                                 capture: Boolean(n.capture)
                             } : {
                                 type: String(e),
                                 callback: null != t ? t : void 0,
                                 capture: Boolean(n)
                             }
                         }(e, t, n),
-                        a = r[i];
-                    null != o && a && z(a, o, s)
+                        a = r[s];
+                    null != o && a && z(a, o, i)
                 }
                 dispatchEvent(e) {
                     const t = K(this)[String(e.type)];
                     if (null == t) return !0;
                     const n = e instanceof T ? e : B.wrap(e),
-                        r = N(n, "event");
-                    if (r.dispatchFlag) throw o = "This event has been in dispatching.", h.DOMException ? new h.DOMException(o, "InvalidStateError") : (null == D && (D = class e extends Error {
+                        r = S(n, "event");
+                    if (r.dispatchFlag) throw o = "This event has been in dispatching.", h.DOMException ? new h.DOMException(o, "InvalidStateError") : (null == I && (I = class e extends Error {
                         constructor(t) {
                             super(t), Error.captureStackTrace && Error.captureStackTrace(this, e)
                         }
                         get code() {
                             return 11
                         }
                         get name() {
                             return "InvalidStateError"
                         }
-                    }, Object.defineProperties(D.prototype, {
+                    }, Object.defineProperties(I.prototype, {
                         code: {
                             enumerable: !0
                         },
                         name: {
                             enumerable: !0
                         }
-                    }), j(D), j(D.prototype)), new D(o));
+                    }), D(I), D(I.prototype)), new I(o));
                     var o;
                     if (r.dispatchFlag = !0, r.target = r.currentTarget = this, !r.stopPropagationFlag) {
                         const {
                             cow: e,
                             listeners: o
                         } = t;
                         t.cow = !0;
-                        for (let s = 0; s < o.length; ++s) {
-                            const i = o[s];
-                            if (!V(i) && (M(i) && Q(t, s, !e) && (s -= 1), r.inPassiveListenerFlag = W(i), Y(i, this, n), r.inPassiveListenerFlag = !1, r.stopImmediatePropagationFlag)) break
+                        for (let i = 0; i < o.length; ++i) {
+                            const s = o[i];
+                            if (!V(s) && (M(s) && Q(t, i, !e) && (i -= 1), r.inPassiveListenerFlag = W(s), Y(s, this, n), r.inPassiveListenerFlag = !1, r.stopImmediatePropagationFlag)) break
                         }
                         e || (t.cow = !1)
                     }
                     return r.target = null, r.currentTarget = null, r.stopImmediatePropagationFlag = !1, r.stopPropagationFlag = !1, r.dispatchFlag = !1, !r.canceledFlag
                 }
             }
             const J = new WeakMap;
@@ -564,15 +594,27 @@
             }
             const $ = Object.getOwnPropertyNames(Z.prototype);
             for (let e = 0; e < $.length; ++e) "constructor" !== $[e] && Object.defineProperty(Z.prototype, $[e], {
                 enumerable: !0
             });
 
             function ee(e, t, n) {
-                return t in e ? Object.defineProperty(e, t, {
+                return (t = function(e) {
+                    var t = function(e, t) {
+                        if ("object" != typeof e || null === e) return e;
+                        var n = e[Symbol.toPrimitive];
+                        if (void 0 !== n) {
+                            var r = n.call(e, "string");
+                            if ("object" != typeof r) return r;
+                            throw new TypeError("@@toPrimitive must return a primitive value.")
+                        }
+                        return String(e)
+                    }(e);
+                    return "symbol" == typeof t ? t : String(t)
+                }(t)) in e ? Object.defineProperty(e, t, {
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = n, e
             }
             var te;
@@ -586,15 +628,18 @@
                 function(e) {
                     e.DEBUG = "D", e.LOG = "L", e.WARN = "W", e.ERROR = "E", e.UNCAUGHT_ERROR = "U"
                 }(te || (te = {}));
             const re = class {
                 constructor() {
                     ee(this, "isEnabled", !1), ee(this, "debug", void 0), ee(this, "log", void 0), ee(this, "warn", void 0), ee(this, "error", void 0), ee(this, "eventTarget", void 0), ee(this, "handleUncaughtError", (e => {
                         var t = [];
-                        e.error && t.push(e.error), e.message && t.push(e.message), this.eventTarget.dispatchEvent(ne(te.UNCAUGHT_ERROR, t))
+                        null != e.error && t.push(e.error), e.message && t.push(e.message), this.eventTarget.dispatchEvent(ne(te.UNCAUGHT_ERROR, t))
+                    })), ee(this, "handleUncaughtRejection", (e => {
+                        var t = [];
+                        null != e.promise && t.push(e.promise.toString()), e.reason && t.push(e.reason), this.eventTarget.dispatchEvent(ne(te.UNCAUGHT_ERROR, t))
                     })), this.debug = console.debug, this.log = console.log, this.warn = console.warn, this.error = console.error, this.eventTarget = new Z
                 }
                 enable() {
                     var e = this;
                     this.isEnabled || (console.debug = function() {
                         for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                         e.eventTarget.dispatchEvent(ne(te.DEBUG, n)), e.debug.apply(console, n)
@@ -603,61 +648,71 @@
                         e.eventTarget.dispatchEvent(ne(te.LOG, n)), e.log.apply(console, n)
                     }, console.warn = function() {
                         for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                         e.eventTarget.dispatchEvent(ne(te.WARN, n)), e.warn.apply(console, n)
                     }, console.error = function() {
                         for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                         e.eventTarget.dispatchEvent(ne(te.ERROR, n)), e.error.apply(console, n)
-                    }, window.addEventListener("error", this.handleUncaughtError), a.setLogLevel(a.level), this.isEnabled = !0)
+                    }, window.addEventListener("error", this.handleUncaughtError), window.addEventListener("unhandledrejection", this.handleUncaughtRejection), a.setLogLevel(a.level), this.isEnabled = !0)
                 }
                 disable() {
-                    this.isEnabled && (console.debug = this.debug, console.log = this.log, console.warn = this.warn, console.error = this.error, window.removeEventListener("error", this.handleUncaughtError), a.setLogLevel(a.level), this.isEnabled = !1)
+                    this.isEnabled && (console.debug = this.debug, console.log = this.log, console.warn = this.warn, console.error = this.error, window.removeEventListener("error", this.handleUncaughtError), window.removeEventListener("unhandledrejection", this.handleUncaughtRejection), a.setLogLevel(a.level), this.isEnabled = !1)
                 }
                 addEventListener(e, t) {
                     this.eventTarget.addEventListener(e, t)
                 }
                 removeEventListener(e, t) {
                     this.eventTarget.removeEventListener(e, t)
                 }
             };
 
             function oe(e, t, n) {
-                return t in e ? Object.defineProperty(e, t, {
+                return (t = function(e) {
+                    var t = function(e, t) {
+                        if ("object" != typeof e || null === e) return e;
+                        var n = e[Symbol.toPrimitive];
+                        if (void 0 !== n) {
+                            var r = n.call(e, "string");
+                            if ("object" != typeof r) return r;
+                            throw new TypeError("@@toPrimitive must return a primitive value.")
+                        }
+                        return String(e)
+                    }(e);
+                    return "symbol" == typeof t ? t : String(t)
+                }(t)) in e ? Object.defineProperty(e, t, {
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = n, e
             }
-            class se {
+            class ie {
                 static formatMessages(e) {
                     return e.map((e => {
                         if ("string" == typeof e) return e;
                         var t = "";
                         try {
                             t = JSON.stringify(e)
                         } catch (n) {
                             t = e.toString()
                         }
                         return "{}" === t ? e.toString() : t
                     })).join("\t")
                 }
-                static formatStack() {
-                    var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "",
-                        t = arguments.length > 1 ? arguments[1] : void 0;
+                static formatStack(e, t) {
                     if ("" === e) return "";
                     var n = e.split("\n").map((e => e.trim()));
                     switch (t) {
                         case te.ERROR:
                             n = n.splice("Error" === e[0] ? 4 : 3);
                             break;
                         case te.UNCAUGHT_ERROR:
                             n = n.splice("Error" === e[0] ? 3 : 2)
                     }
-                    return n ? "\t".concat(n.join("\n\t")) : ""
+                    return null != n ? "\t".concat(n.join("\n\t")) : ""
                 }
                 constructor(e) {
                     oe(this, "history", void 0), oe(this, "offset", void 0), oe(this, "limit", void 0), oe(this, "isEnabled", void 0), oe(this, "proxy", void 0), this.history = [], this.offset = 0, this.limit = 1e4, this.isEnabled = !1, this.proxy = e, this.addHistory = this.addHistory.bind(this)
                 }
                 enable() {
                     this.isEnabled || (this.proxy.addEventListener(te.DEBUG, this.addHistory), this.proxy.addEventListener(te.LOG, this.addHistory), this.proxy.addEventListener(te.WARN, this.addHistory), this.proxy.addEventListener(te.ERROR, this.addHistory), this.proxy.addEventListener(te.UNCAUGHT_ERROR, this.addHistory), this.isEnabled = !0)
                 }
@@ -684,31 +739,32 @@
                     if (this.offset > this.limit) {
                         var e = this.offset % this.limit;
                         this.history = this.history.slice(e).concat(this.history.slice(0, e)), this.offset = this.limit
                     }
                     return this.history
                 }
                 getFormattedHistory() {
-                    return this.getHistory().map((e => "".concat(e.time.toISOString(), " ").concat(e.type, "\t") + "".concat(se.formatMessages(e.messages)) + (e.stack ? "\n".concat(se.formatStack(e.stack, e.type)) : ""))).join("\n")
+                    return this.getHistory().map((e => "".concat(e.time.toISOString(), " ").concat(e.type, "\t") + "".concat(ie.formatMessages(e.messages)) + (null != e.stack ? "\n".concat(ie.formatStack(e.stack, e.type)) : ""))).join("\n")
                 }
             }
-            const ie = se
+            const se = ie,
+                ae = a
         },
         155: e => {
             var t, n, r = e.exports = {};
 
             function o() {
                 throw new Error("setTimeout has not been defined")
             }
 
-            function s() {
+            function i() {
                 throw new Error("clearTimeout has not been defined")
             }
 
-            function i(e) {
+            function s(e) {
                 if (t === setTimeout) return setTimeout(e, 0);
                 if ((t === o || !t) && setTimeout) return t = setTimeout, setTimeout(e, 0);
                 try {
                     return t(e, 0)
                 } catch (n) {
                     try {
                         return t.call(null, e, 0)
@@ -719,65 +775,65 @@
             }! function() {
                 try {
                     t = "function" == typeof setTimeout ? setTimeout : o
                 } catch (e) {
                     t = o
                 }
                 try {
-                    n = "function" == typeof clearTimeout ? clearTimeout : s
+                    n = "function" == typeof clearTimeout ? clearTimeout : i
                 } catch (e) {
-                    n = s
+                    n = i
                 }
             }();
             var a, l = [],
                 c = !1,
                 u = -1;
 
             function p() {
                 c && a && (c = !1, a.length ? l = a.concat(l) : u = -1, l.length && h())
             }
 
             function h() {
                 if (!c) {
-                    var e = i(p);
+                    var e = s(p);
                     c = !0;
                     for (var t = l.length; t;) {
                         for (a = l, l = []; ++u < t;) a && a[u].run();
                         u = -1, t = l.length
                     }
                     a = null, c = !1,
                         function(e) {
                             if (n === clearTimeout) return clearTimeout(e);
-                            if ((n === s || !n) && clearTimeout) return n = clearTimeout, clearTimeout(e);
+                            if ((n === i || !n) && clearTimeout) return n = clearTimeout, clearTimeout(e);
                             try {
-                                n(e)
+                                return n(e)
                             } catch (t) {
                                 try {
                                     return n.call(null, e)
                                 } catch (t) {
                                     return n.call(this, e)
                                 }
                             }
                         }(e)
                 }
             }
 
-            function g(e, t) {
+            function d(e, t) {
                 this.fun = e, this.array = t
             }
 
-            function d() {}
+            function g() {}
             r.nextTick = function(e) {
                 var t = new Array(arguments.length - 1);
                 if (arguments.length > 1)
                     for (var n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
-                l.push(new g(e, t)), 1 !== l.length || c || i(h)
-            }, g.prototype.run = function() {
+                l.push(new d(e, t)), 1 !== l.length || c || s(h)
+            }, d.prototype.run = function() {
                 this.fun.apply(null, this.array)
-            }, r.title = "browser", r.browser = !0, r.env = {}, r.argv = [], r.version = "", r.versions = {}, r.on = d, r.addListener = d, r.once = d, r.off = d, r.removeListener = d, r.removeAllListeners = d, r.emit = d, r.prependListener = d, r.prependOnceListener = d, r.listeners = function(e) {
+            }, r.title = "browser", r.browser = !0, r.env = {}, r.argv = [], r.version = "", r.versions = {}, r.on = g, r.addListener = g, r.once = g, r.off = g, r.removeListener = g, r.removeAllListeners = g, r.emit = g, r.prependListener = g, r.prependOnceListener = g, r.listeners = function(e) {
                 return []
             }, r.binding = function(e) {
                 throw new Error("process.binding is not supported")
             }, r.cwd = function() {
                 return "/"
             }, r.chdir = function(e) {
                 throw new Error("process.chdir is not supported")
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/remoteEntry.6443de594d4e2715e64f.js` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/static/remoteEntry.c8e537d8b4d0739199bb.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,281 +1,303 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, l, s, d, f, p, c, h, v, g, b, m = {
+    var e, r, t, n, o, a, i, u, d, l, s, f, c, p, h, v, b, g, m, y, w, S = {
             690: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(790), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(790), t.e(480)]).then((() => () => t(480)))
+                        "./index": () => Promise.all([t.e(939), t.e(646), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(939), t.e(646), t.e(480)]).then((() => () => t(480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => i
+                    init: () => a
                 })
             }
         },
-        y = {};
+        P = {};
 
-    function w(e) {
-        var r = y[e];
+    function j(e) {
+        var r = P[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = P[e] = {
             id: e,
             exports: {}
         };
-        return m[e].call(t.exports, t, t.exports, w), t.exports
+        return S[e].call(t.exports, t, t.exports, j), t.exports
     }
-    w.m = m, w.c = y, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    j.m = S, j.c = P, j.n = e => {
+        var r = e && e.__esModule ? () => e.default : () => e;
+        return j.d(r, {
+            a: r
+        }), r
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        480: "26bcd834ece40109d1df",
-        568: "8c7c3ea60a12c60e6eb1",
-        701: "c67db7c3d6d969fcf22b",
-        790: "b21bef9f80316178ddf0"
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        421: "1465f517f2d0e9eda410",
+        480: "a275f597035bbcf259ca",
+        568: "7551298c61415e9b2969",
+        646: "9f6ce530718b1dd2e63f",
+        701: "6f39578fffe6bd3cfc48",
+        748: "2b10c134bb09150dc4a9",
+        939: "8209c75376606b79555f"
     } [e] + ".js?v=" + {
-        480: "26bcd834ece40109d1df",
-        568: "8c7c3ea60a12c60e6eb1",
-        701: "c67db7c3d6d969fcf22b",
-        790: "b21bef9f80316178ddf0"
-    } [e], w.g = function() {
+        421: "1465f517f2d0e9eda410",
+        480: "a275f597035bbcf259ca",
+        568: "7551298c61415e9b2969",
+        646: "9f6ce530718b1dd2e63f",
+        701: "6f39578fffe6bd3cfc48",
+        748: "2b10c134bb09150dc4a9",
+        939: "8209c75376606b79555f"
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deephaven/ipywidgets:", w.l = (t, n, o, i) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deephaven/ipywidgets:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
+            var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        a = d;
+                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
+                    var s = d[l];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, w.nc && a.setAttribute("nonce", w.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        j.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        j.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var i = w.S[t],
-                    a = "@deephaven/ipywidgets",
+                j.o(j.S, t) || (j.S[t] = {});
+                var a = j.S[t],
+                    i = "@deephaven/ipywidgets",
                     u = (e, r, t, n) => {
-                        var o = i[e] = i[e] || {},
+                        var o = a[e] = a[e] || {},
                             u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
-                            from: a,
+                            from: i,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("@deephaven/ipywidgets", "0.1.0", (() => Promise.all([w.e(790), w.e(568)]).then((() => () => w(568))))), u("@deephaven/log", "0.15.0", (() => w.e(701).then((() => () => w(701)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (u("@deephaven/ipywidgets", "0.2.0", (() => Promise.all([j.e(939), j.e(646), j.e(568)]).then((() => () => j(568))))), u("@deephaven/jsapi-utils", "0.41.3", (() => Promise.all([j.e(421), j.e(939), j.e(748)]).then((() => () => j(421))))), u("@deephaven/log", "0.41.0", (() => j.e(701).then((() => () => j(701)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
-            var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                u = (typeof i)[0];
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return d();
 
-        function l() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+        function d() {
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, l = !0;; u++, a++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (d = (typeof(s = r[a]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
-                } else if (l)
-                    if (f == d)
+            for (var i = 0, u = 1, d = !0;; u++, i++) {
+                var l, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !d || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
+                    if (!d || "u" != f) return !1
+                } else if (d)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (d = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    d = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
-                    l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                    if (u <= n || s < f != o) return !1;
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        var c = [],
+            p = c.pop.bind(c);
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
-    }, a = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        return !!p()
+    }, i = (e, r) => {
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
+        return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
+    }, d = (e, r) => {
+        var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
-        var o = u(e, t);
-        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
-    }, d = (e, r, t) => {
+        var o = d(e, t);
+        return a(n, o) || c(l(e, t, o, n)), p(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
-        var i = w.I(r);
-        return i && i.then ? i.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var i = r && w.o(r, t) && d(r, t, n);
-        return i ? f(i) : o()
-    })), v = {}, g = {
-        565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, p = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => r && j.o(r, t) ? p(u(r, t)) : n())), b = h(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), g = h(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && f(r, t, n);
+        return a ? p(a) : o()
+    })), m = {}, y = {
+        939: () => g("default", "@deephaven/log", [2, 0, 41, 0], (() => j.e(701).then((() => () => j(701))))),
+        429: () => g("default", "@deephaven/jsapi-utils", [2, 0, 41, 3], (() => Promise.all([j.e(421), j.e(748)]).then((() => () => j(421))))),
+        565: () => b("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ]),
-        969: () => h("default", "@deephaven/log", [4, 0, 15, 0], (() => w.e(701).then((() => () => w(701)))))
-    }, b = {
-        790: [565, 969]
-    }, w.f.consumes = (e, r) => {
-        w.o(b, e) && b[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+        748: () => v("default", "@deephaven/jsapi-utils", (() => () => j(421)))
+    }, w = {
+        646: [429, 565],
+        748: [748],
+        939: [939]
+    }, j.f.consumes = (e, r) => {
+        j.o(w, e) && w[e].forEach((e => {
+            if (j.o(m, e)) return r.push(m[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    m[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete m[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
-                var o = g[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var o = y[e]();
+                o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             552: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (790 != r) {
+                else if (/^(646|748|939)$/.test(r)) e[r] = 0;
+            else {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var i = w.p + w.u(r),
-                    a = new Error;
-                w.l(i, (t => {
-                    if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                var a = j.p + j.u(r),
+                    i = new Error;
+                j.l(a, (t => {
+                    if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
-                            i = t && t.target && t.target.src;
-                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
-            } else e[r] = 0
+            }
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
-                    l = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) w.o(a, n) && (w.m[n] = a[n]);
-                    u && u(w)
+                var n, o, [a, i, u] = t,
+                    d = 0;
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    u && u(j)
                 }
-                for (r && r(t); l < i.length; l++) o = i[l], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); d < a.length; d++) o = a[d], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_deephaven_ipywidgets = self.webpackChunk_deephaven_ipywidgets || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), w.nc = void 0;
-    var S = w(690);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deephaven/ipywidgets"] = S
+    })(), j.nc = void 0;
+    var E = j(690);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deephaven/ipywidgets"] = E
 })();
```

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/conftest.py` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_table.py` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/Makefile` & `deephaven_ipywidgets-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/make.bat` & `deephaven_ipywidgets-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/source/conf.py` & `deephaven_ipywidgets-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/source/develop-install.rst` & `deephaven_ipywidgets-0.3.0/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/source/index.rst` & `deephaven_ipywidgets-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/docs/source/installing.rst` & `deephaven_ipywidgets-0.3.0/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/examples/introduction.ipynb` & `deephaven_ipywidgets-0.3.0/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/package.json` & `deephaven_ipywidgets-0.3.0/deephaven_ipywidgets/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9506944444444445%*

 * *Differences: {"'dependencies'": "{'@deephaven/jsapi-shim': '^0.41.0', '@deephaven/log': '^0.41.0', "*

 * *                   "'@deephaven/jsapi-utils': '^0.41.3'}",*

 * * "'devDependencies'": "{'@deephaven/eslint-config': '^0.41.0', '@deephaven/prettier-config': "*

 * *                      "'^0.41.0', '@jupyterlab/builder': '^3.6.4', "*

 * *                      "'@typescript-eslint/eslint-plugin': '^5.46.0', '@typescript-eslint/parser': "*

 * *                      "'^5.46.0', 'eslint': '^8.29.0', 'eslint-import-resolver-typescript': "*

 * *       […]*

```diff
@@ -3,46 +3,48 @@
         "email": "operations@deephaven.io",
         "name": "Deephaven Data Labs LLC"
     },
     "bugs": {
         "url": "https://github.com/deephaven/deephaven-ipywidgets/issues"
     },
     "dependencies": {
-        "@deephaven/jsapi-shim": "0.15.0",
-        "@deephaven/log": "0.15.0",
+        "@deephaven/jsapi-shim": "^0.41.0",
+        "@deephaven/jsapi-utils": "^0.41.3",
+        "@deephaven/log": "^0.41.0",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "uuid": "8.3.2"
     },
     "description": "Deephaven ipython widget library",
     "devDependencies": {
         "@babel/core": "^7.5.0",
         "@babel/preset-env": "^7.5.0",
-        "@deephaven/eslint-config": "0.15.0",
-        "@deephaven/prettier-config": "0.15.0",
-        "@jupyterlab/builder": "^3.0.0",
+        "@deephaven/eslint-config": "^0.41.0",
+        "@deephaven/prettier-config": "^0.41.0",
+        "@jupyterlab/builder": "^3.6.4",
         "@phosphor/application": "^1.6.0",
         "@phosphor/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
         "@types/uuid": "8.3.4",
         "@types/webpack-env": "^1.13.6",
-        "@typescript-eslint/eslint-plugin": "^4.28.0",
-        "@typescript-eslint/parser": "^4.28.0",
+        "@typescript-eslint/eslint-plugin": "^5.46.0",
+        "@typescript-eslint/parser": "^5.46.0",
         "acorn": "^7.2.0",
         "babel-eslint": "^10.1.0",
         "css-loader": "^3.2.0",
-        "eslint": "^7.22.0",
+        "eslint": "^8.29.0",
         "eslint-config-prettier": "^6.11.0",
-        "eslint-import-resolver-typescript": "^2.5.0",
+        "eslint-import-resolver-typescript": "^3.5.0",
         "eslint-plugin-es": "^4.1.0",
-        "eslint-plugin-flowtype": "^5.2.0",
+        "eslint-plugin-flowtype": "^8.0.3",
         "eslint-plugin-import": "^2.26.0",
         "eslint-plugin-jsx-a11y": "^6.6.0",
         "eslint-plugin-prettier": "^3.3.1",
         "eslint-plugin-react": "7.30.1",
         "eslint-plugin-react-hooks": "4.6.0",
+        "eslint-plugin-react-refresh": "0.3.4",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
         "prettier": "^2.0.5",
         "rimraf": "^2.6.2",
@@ -57,14 +59,18 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/deephaven/deephaven-ipywidgets",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.c8e537d8b4d0739199bb.js"
+        },
         "extension": "lib/plugin",
         "outputDir": "deephaven_ipywidgets/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -105,9 +111,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `deephaven_ipywidgets-0.2.2/setup.py` & `deephaven_ipywidgets-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/src/__tests__/index.spec.ts` & `deephaven_ipywidgets-0.3.0/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/src/__tests__/utils.ts` & `deephaven_ipywidgets-0.3.0/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/src/extension.ts` & `deephaven_ipywidgets-0.3.0/src/extension.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/src/plugin.ts` & `deephaven_ipywidgets-0.3.0/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/src/version.ts` & `deephaven_ipywidgets-0.3.0/src/version.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/tsconfig.json` & `deephaven_ipywidgets-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.2/webpack.config.js` & `deephaven_ipywidgets-0.3.0/webpack.config.js`

 * *Files identical despite different names*

