# Comparing `tmp/ipylivebash-0.1.2.tar.gz` & `tmp/ipylivebash-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipylivebash-0.1.2.tar", last modified: Thu Jan 27 15:26:11 2022, max compression
+gzip compressed data, was "ipylivebash-0.2.0a0.tar", last modified: Fri Jun 23 09:58:25 2023, max compression
```

## Comparing `ipylivebash-0.1.2.tar` & `ipylivebash-0.2.0a0.tar`

### file list

```diff
@@ -1,80 +1,86 @@
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.231974 ipylivebash-0.1.2/
--rw-r--r--   0 benlau     (501) staff       (20)     1492 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/LICENSE.txt
--rw-r--r--   0 benlau     (501) staff       (20)      648 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/MANIFEST.in
--rw-r--r--   0 benlau     (501) staff       (20)     5198 2022-01-27 15:26:11.232313 ipylivebash-0.1.2/PKG-INFO
--rw-r--r--   0 benlau     (501) staff       (20)     4264 2022-01-06 17:47:38.000000 ipylivebash-0.1.2/README.md
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.156377 ipylivebash-0.1.2/css/
--rw-r--r--   0 benlau     (501) staff       (20)     1369 2022-01-08 09:48:19.000000 ipylivebash-0.1.2/css/widget.css
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.159181 ipylivebash-0.1.2/docs/
--rw-r--r--   0 benlau     (501) staff       (20)      613 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/Makefile
--rw-r--r--   0 benlau     (501) staff       (20)      172 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/environment.yml
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.163819 ipylivebash-0.1.2/docs/img/
--rw-r--r--   0 benlau     (501) staff       (20)     6964 2022-01-02 11:07:56.000000 ipylivebash-0.1.2/docs/img/ask_confirm.png
--rw-r--r--   0 benlau     (501) staff       (20)      783 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/make.bat
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.172141 ipylivebash-0.1.2/docs/source/
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.176111 ipylivebash-0.1.2/docs/source/_static/
--rw-r--r--   0 benlau     (501) staff       (20)    12128 2022-01-27 15:25:58.000000 ipylivebash-0.1.2/docs/source/_static/embed-bundle.js
--rw-r--r--   0 benlau     (501) staff       (20)    30084 2022-01-27 15:25:58.000000 ipylivebash-0.1.2/docs/source/_static/embed-bundle.js.map
--rw-r--r--   0 benlau     (501) staff       (20)      120 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/_static/helper.js
--rw-r--r--   0 benlau     (501) staff       (20)     6314 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/conf.py
--rw-r--r--   0 benlau     (501) staff       (20)      825 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/develop-install.rst
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.181467 ipylivebash-0.1.2/docs/source/examples/
--rw-r--r--   0 benlau     (501) staff       (20)      385 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/examples/index.rst
--rw-r--r--   0 benlau     (501) staff       (20)       53 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/examples/introduction.nblink
--rw-r--r--   0 benlau     (501) staff       (20)      636 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/index.rst
--rw-r--r--   0 benlau     (501) staff       (20)     1023 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/installing.rst
--rw-r--r--   0 benlau     (501) staff       (20)      109 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/docs/source/introduction.rst
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.182457 ipylivebash-0.1.2/examples/
--rw-r--r--   0 benlau     (501) staff       (20)     7360 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/examples/introduction.ipynb
--rw-r--r--   0 benlau     (501) staff       (20)      183 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/install.json
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.190643 ipylivebash-0.1.2/ipylivebash/
--rw-r--r--   0 benlau     (501) staff       (20)     2433 2022-01-21 14:12:12.000000 ipylivebash-0.1.2/ipylivebash/__init__.py
--rw-r--r--   0 benlau     (501) staff       (20)      242 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/_frontend.py
--rw-r--r--   0 benlau     (501) staff       (20)      196 2022-01-27 15:24:42.000000 ipylivebash-0.1.2/ipylivebash/_version.py
--rw-r--r--   0 benlau     (501) staff       (20)      536 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/debounce.py
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.198966 ipylivebash-0.1.2/ipylivebash/labextension/
--rw-r--r--   0 benlau     (501) staff       (20)     2989 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/package.json
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.205544 ipylivebash-0.1.2/ipylivebash/labextension/static/
--rw-r--r--   0 benlau     (501) staff       (20)    11475 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/367.21ed93376ff16371416b.js
--rw-r--r--   0 benlau     (501) staff       (20)      927 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/480.e6446a30d6b6a16ad121.js
--rw-r--r--   0 benlau     (501) staff       (20)      516 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/568.fb1e61d7b0a27a69428e.js
--rw-r--r--   0 benlau     (501) staff       (20)     6198 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/remoteEntry.c307d6dfc35834975a6a.js
--rw-r--r--   0 benlau     (501) staff       (20)      118 2022-01-27 15:26:04.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/style.js
--rw-r--r--   0 benlau     (501) staff       (20)     2452 2022-01-27 15:26:08.000000 ipylivebash-0.1.2/ipylivebash/labextension/static/third-party-licenses.json
--rw-r--r--   0 benlau     (501) staff       (20)     1393 2022-01-22 12:21:54.000000 ipylivebash-0.1.2/ipylivebash/logfile.py
--rw-r--r--   0 benlau     (501) staff       (20)     2263 2022-01-22 12:21:54.000000 ipylivebash-0.1.2/ipylivebash/logview.py
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.209066 ipylivebash-0.1.2/ipylivebash/nbextension/
--rw-r--r--   0 benlau     (501) staff       (20)      412 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/nbextension/extension.js
--rw-r--r--   0 benlau     (501) staff       (20)    12650 2022-01-27 15:25:58.000000 ipylivebash-0.1.2/ipylivebash/nbextension/index.js
--rw-r--r--   0 benlau     (501) staff       (20)    30860 2022-01-27 15:25:58.000000 ipylivebash-0.1.2/ipylivebash/nbextension/index.js.map
--rw-r--r--   0 benlau     (501) staff       (20)     7729 2022-01-22 12:21:54.000000 ipylivebash-0.1.2/ipylivebash/runner.py
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.217858 ipylivebash-0.1.2/ipylivebash/tests/
--rw-r--r--   0 benlau     (501) staff       (20)        0 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/tests/__init__.py
--rw-r--r--   0 benlau     (501) staff       (20)     1417 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/tests/conftest.py
--rw-r--r--   0 benlau     (501) staff       (20)      732 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/tests/test_logfile.py
--rw-r--r--   0 benlau     (501) staff       (20)      113 2022-01-07 05:44:36.000000 ipylivebash-0.1.2/ipylivebash/tests/test_logview.py
--rw-r--r--   0 benlau     (501) staff       (20)      333 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash/tests/test_nbextension_path.py
--rw-r--r--   0 benlau     (501) staff       (20)     1564 2022-01-22 12:21:54.000000 ipylivebash-0.1.2/ipylivebash/tests/test_runner.py
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.198174 ipylivebash-0.1.2/ipylivebash.egg-info/
--rw-r--r--   0 benlau     (501) staff       (20)     5198 2022-01-27 15:26:11.000000 ipylivebash-0.1.2/ipylivebash.egg-info/PKG-INFO
--rw-r--r--   0 benlau     (501) staff       (20)     1737 2022-01-27 15:26:11.000000 ipylivebash-0.1.2/ipylivebash.egg-info/SOURCES.txt
--rw-r--r--   0 benlau     (501) staff       (20)        1 2022-01-27 15:26:11.000000 ipylivebash-0.1.2/ipylivebash.egg-info/dependency_links.txt
--rw-r--r--   0 benlau     (501) staff       (20)      183 2022-01-27 15:26:11.000000 ipylivebash-0.1.2/ipylivebash.egg-info/requires.txt
--rw-r--r--   0 benlau     (501) staff       (20)       12 2022-01-27 15:26:11.000000 ipylivebash-0.1.2/ipylivebash.egg-info/top_level.txt
--rw-r--r--   0 benlau     (501) staff       (20)       65 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/ipylivebash.json
--rw-r--r--   0 benlau     (501) staff       (20)     2873 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/package.json
--rw-r--r--   0 benlau     (501) staff       (20)      439 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/pyproject.toml
--rw-r--r--   0 benlau     (501) staff       (20)      107 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/pytest.ini
--rw-r--r--   0 benlau     (501) staff       (20)      187 2022-01-27 15:26:11.234303 ipylivebash-0.1.2/setup.cfg
--rw-r--r--   0 benlau     (501) staff       (20)     3122 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/setup.py
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.223879 ipylivebash-0.1.2/src/
-drwxr-xr-x   0 benlau     (501) staff       (20)        0 2022-01-27 15:26:11.230826 ipylivebash-0.1.2/src/__tests__/
--rw-r--r--   0 benlau     (501) staff       (20)      842 2022-01-08 05:42:56.000000 ipylivebash-0.1.2/src/__tests__/index.spec.ts
--rw-r--r--   0 benlau     (501) staff       (20)     2856 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/src/__tests__/utils.ts
--rw-r--r--   0 benlau     (501) staff       (20)      619 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/src/extension.ts
--rw-r--r--   0 benlau     (501) staff       (20)      139 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/src/index.ts
--rw-r--r--   0 benlau     (501) staff       (20)     1114 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/src/plugin.ts
--rw-r--r--   0 benlau     (501) staff       (20)      567 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/src/version.ts
--rw-r--r--   0 benlau     (501) staff       (20)     5207 2022-01-08 12:56:52.000000 ipylivebash-0.1.2/src/widget.ts
--rw-r--r--   0 benlau     (501) staff       (20)      553 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/tsconfig.json
--rw-r--r--   0 benlau     (501) staff       (20)     2127 2022-01-02 09:38:46.000000 ipylivebash-0.1.2/webpack.config.js
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.107733 ipylivebash-0.2.0a0/
+-rw-r--r--   0 benlau     (501) staff       (20)     1492 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/LICENSE.txt
+-rw-r--r--   0 benlau     (501) staff       (20)      648 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/MANIFEST.in
+-rw-r--r--   0 benlau     (501) staff       (20)     5198 2023-06-23 09:58:25.107859 ipylivebash-0.2.0a0/PKG-INFO
+-rw-r--r--   0 benlau     (501) staff       (20)     4264 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/README.md
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.099136 ipylivebash-0.2.0a0/css/
+-rw-r--r--   0 benlau     (501) staff       (20)        0 2023-04-21 12:50:42.000000 ipylivebash-0.2.0a0/css/widget.css
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.099572 ipylivebash-0.2.0a0/docs/
+-rw-r--r--   0 benlau     (501) staff       (20)      613 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/Makefile
+-rw-r--r--   0 benlau     (501) staff       (20)      172 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/environment.yml
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.099734 ipylivebash-0.2.0a0/docs/img/
+-rw-r--r--   0 benlau     (501) staff       (20)     6964 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/img/ask_confirm.png
+-rw-r--r--   0 benlau     (501) staff       (20)      783 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/make.bat
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.100507 ipylivebash-0.2.0a0/docs/source/
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.101316 ipylivebash-0.2.0a0/docs/source/_static/
+-rw-r--r--   0 benlau     (501) staff       (20)   215203 2023-05-14 08:47:41.000000 ipylivebash-0.2.0a0/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 benlau     (501) staff       (20)     1540 2023-04-19 14:38:10.000000 ipylivebash-0.2.0a0/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0 benlau     (501) staff       (20)   522479 2023-05-14 08:47:41.000000 ipylivebash-0.2.0a0/docs/source/_static/embed-bundle.js.map
+-rw-r--r--   0 benlau     (501) staff       (20)      120 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/_static/helper.js
+-rw-r--r--   0 benlau     (501) staff       (20)     6314 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/conf.py
+-rw-r--r--   0 benlau     (501) staff       (20)      825 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/develop-install.rst
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.101624 ipylivebash-0.2.0a0/docs/source/examples/
+-rw-r--r--   0 benlau     (501) staff       (20)      385 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/examples/index.rst
+-rw-r--r--   0 benlau     (501) staff       (20)       53 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/examples/introduction.nblink
+-rw-r--r--   0 benlau     (501) staff       (20)      636 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/index.rst
+-rw-r--r--   0 benlau     (501) staff       (20)     1023 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/installing.rst
+-rw-r--r--   0 benlau     (501) staff       (20)      109 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/docs/source/introduction.rst
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.101755 ipylivebash-0.2.0a0/examples/
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.101862 ipylivebash-0.2.0a0/examples/.ipynb_checkpoints/
+-rw-r--r--   0 benlau     (501) staff       (20)     7360 2023-04-15 17:14:13.000000 ipylivebash-0.2.0a0/examples/.ipynb_checkpoints/introduction-checkpoint.ipynb
+-rw-r--r--   0 benlau     (501) staff       (20)     7360 2023-06-16 11:40:46.000000 ipylivebash-0.2.0a0/examples/introduction.ipynb
+-rw-r--r--   0 benlau     (501) staff       (20)      183 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/install.json
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.103000 ipylivebash-0.2.0a0/ipylivebash/
+-rw-r--r--   0 benlau     (501) staff       (20)     2433 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/__init__.py
+-rw-r--r--   0 benlau     (501) staff       (20)      249 2023-05-08 00:53:13.000000 ipylivebash-0.2.0a0/ipylivebash/_frontend.py
+-rw-r--r--   0 benlau     (501) staff       (20)      148 2023-05-08 00:51:54.000000 ipylivebash-0.2.0a0/ipylivebash/_version.py
+-rw-r--r--   0 benlau     (501) staff       (20)      536 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/debounce.py
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.103655 ipylivebash-0.2.0a0/ipylivebash/labextension/
+-rw-r--r--   0 benlau     (501) staff       (20)     2996 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/package.json
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.104545 ipylivebash-0.2.0a0/ipylivebash/labextension/static/
+-rw-r--r--   0 benlau     (501) staff       (20)   214392 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/367.7672911d17cc2c4b7cb0.js
+-rw-r--r--   0 benlau     (501) staff       (20)     1540 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/367.7672911d17cc2c4b7cb0.js.LICENSE.txt
+-rw-r--r--   0 benlau     (501) staff       (20)      927 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/480.e6446a30d6b6a16ad121.js
+-rw-r--r--   0 benlau     (501) staff       (20)      516 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/568.fb1e61d7b0a27a69428e.js
+-rw-r--r--   0 benlau     (501) staff       (20)     6206 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/remoteEntry.0287ca83ae9ac6168426.js
+-rw-r--r--   0 benlau     (501) staff       (20)      118 2023-06-23 09:58:23.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/style.js
+-rw-r--r--   0 benlau     (501) staff       (20)     2452 2023-06-23 09:58:24.000000 ipylivebash-0.2.0a0/ipylivebash/labextension/static/third-party-licenses.json
+-rw-r--r--   0 benlau     (501) staff       (20)     1393 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/logfile.py
+-rw-r--r--   0 benlau     (501) staff       (20)     3014 2023-04-24 16:08:31.000000 ipylivebash-0.2.0a0/ipylivebash/logview.py
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.105149 ipylivebash-0.2.0a0/ipylivebash/nbextension/
+-rw-r--r--   0 benlau     (501) staff       (20)      412 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/nbextension/extension.js
+-rw-r--r--   0 benlau     (501) staff       (20)   215718 2023-05-14 08:47:41.000000 ipylivebash-0.2.0a0/ipylivebash/nbextension/index.js
+-rw-r--r--   0 benlau     (501) staff       (20)     1540 2023-04-19 14:38:10.000000 ipylivebash-0.2.0a0/ipylivebash/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 benlau     (501) staff       (20)   523241 2023-05-14 08:47:41.000000 ipylivebash-0.2.0a0/ipylivebash/nbextension/index.js.map
+-rw-r--r--   0 benlau     (501) staff       (20)     7370 2023-06-16 11:43:28.000000 ipylivebash-0.2.0a0/ipylivebash/runner.py
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.106184 ipylivebash-0.2.0a0/ipylivebash/tests/
+-rw-r--r--   0 benlau     (501) staff       (20)        0 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/tests/__init__.py
+-rw-r--r--   0 benlau     (501) staff       (20)     1417 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/tests/conftest.py
+-rw-r--r--   0 benlau     (501) staff       (20)      732 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/tests/test_logfile.py
+-rw-r--r--   0 benlau     (501) staff       (20)      113 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/tests/test_logview.py
+-rw-r--r--   0 benlau     (501) staff       (20)      333 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash/tests/test_nbextension_path.py
+-rw-r--r--   0 benlau     (501) staff       (20)      361 2023-04-27 22:54:14.000000 ipylivebash-0.2.0a0/ipylivebash/tests/test_runner.py
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.103552 ipylivebash-0.2.0a0/ipylivebash.egg-info/
+-rw-r--r--   0 benlau     (501) staff       (20)     5198 2023-06-23 09:58:25.000000 ipylivebash-0.2.0a0/ipylivebash.egg-info/PKG-INFO
+-rw-r--r--   0 benlau     (501) staff       (20)     1975 2023-06-23 09:58:25.000000 ipylivebash-0.2.0a0/ipylivebash.egg-info/SOURCES.txt
+-rw-r--r--   0 benlau     (501) staff       (20)        1 2023-06-23 09:58:25.000000 ipylivebash-0.2.0a0/ipylivebash.egg-info/dependency_links.txt
+-rw-r--r--   0 benlau     (501) staff       (20)      183 2023-06-23 09:58:25.000000 ipylivebash-0.2.0a0/ipylivebash.egg-info/requires.txt
+-rw-r--r--   0 benlau     (501) staff       (20)       12 2023-06-23 09:58:25.000000 ipylivebash-0.2.0a0/ipylivebash.egg-info/top_level.txt
+-rw-r--r--   0 benlau     (501) staff       (20)       65 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/ipylivebash.json
+-rw-r--r--   0 benlau     (501) staff       (20)     2879 2023-05-08 00:53:22.000000 ipylivebash-0.2.0a0/package.json
+-rw-r--r--   0 benlau     (501) staff       (20)      439 2023-05-06 05:47:45.000000 ipylivebash-0.2.0a0/pyproject.toml
+-rw-r--r--   0 benlau     (501) staff       (20)      107 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/pytest.ini
+-rw-r--r--   0 benlau     (501) staff       (20)      187 2023-06-23 09:58:25.108183 ipylivebash-0.2.0a0/setup.cfg
+-rw-r--r--   0 benlau     (501) staff       (20)     3122 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/setup.py
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.107321 ipylivebash-0.2.0a0/src/
+drwxr-xr-x   0 benlau     (501) staff       (20)        0 2023-06-23 09:58:25.107606 ipylivebash-0.2.0a0/src/__tests__/
+-rw-r--r--   0 benlau     (501) staff       (20)      783 2023-04-27 23:26:21.000000 ipylivebash-0.2.0a0/src/__tests__/index.spec.ts
+-rw-r--r--   0 benlau     (501) staff       (20)     2856 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/src/__tests__/utils.ts
+-rw-r--r--   0 benlau     (501) staff       (20)      619 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/src/extension.ts
+-rw-r--r--   0 benlau     (501) staff       (20)      139 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/src/index.ts
+-rw-r--r--   0 benlau     (501) staff       (20)     1114 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/src/plugin.ts
+-rw-r--r--   0 benlau     (501) staff       (20)      567 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/src/version.ts
+-rw-r--r--   0 benlau     (501) staff       (20)   211035 2023-06-23 09:58:11.000000 ipylivebash-0.2.0a0/src/webcomp.ts
+-rw-r--r--   0 benlau     (501) staff       (20)     4741 2023-05-09 03:28:47.000000 ipylivebash-0.2.0a0/src/widget.ts
+-rw-r--r--   0 benlau     (501) staff       (20)      678 2023-04-27 23:23:50.000000 ipylivebash-0.2.0a0/tsconfig.json
+-rw-r--r--   0 benlau     (501) staff       (20)     2127 2022-11-28 04:48:08.000000 ipylivebash-0.2.0a0/webpack.config.js
```

### Comparing `ipylivebash-0.1.2/LICENSE.txt` & `ipylivebash-0.2.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/MANIFEST.in` & `ipylivebash-0.2.0a0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/PKG-INFO` & `ipylivebash-0.2.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylivebash
-Version: 0.1.2
+Version: 0.2.0a0
 Summary: Run shell script in Jupyter with live output
 Home-page: https://github.com/benlau/ipylivebash
 Author: Ben lau
 Author-email: xbenlau@gmail.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
@@ -172,9 +172,7 @@
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
 
 #### Python:
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
-
-
```

### Comparing `ipylivebash-0.1.2/README.md` & `ipylivebash-0.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/Makefile` & `ipylivebash-0.2.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/img/ask_confirm.png` & `ipylivebash-0.2.0a0/docs/img/ask_confirm.png`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/make.bat` & `ipylivebash-0.2.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/source/conf.py` & `ipylivebash-0.2.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/source/develop-install.rst` & `ipylivebash-0.2.0a0/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/source/index.rst` & `ipylivebash-0.2.0a0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/docs/source/installing.rst` & `ipylivebash-0.2.0a0/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/examples/introduction.ipynb` & `ipylivebash-0.2.0a0/examples/.ipynb_checkpoints/introduction-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994318181818181%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(2, 'echo It will send a notification when the script "*

 * *            "finished')], delete: [2]}}}"}*

```diff
@@ -236,15 +236,15 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "%%livebash --notify\n",
                 "\n",
-                "echo It will send a notification when the script finishes"
+                "echo It will send a notification when the script finished"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
```

### Comparing `ipylivebash-0.1.2/ipylivebash/__init__.py` & `ipylivebash-0.2.0a0/ipylivebash/__init__.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/debounce.py` & `ipylivebash-0.2.0a0/ipylivebash/debounce.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/labextension/package.json` & `ipylivebash-0.2.0a0/ipylivebash/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672154017857143%*

 * *Differences: {"'devDependencies'": "{'eslint': '7.4.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0287ca83ae9ac6168426.js'}}",*

 * * "'version'": "'0.2.0-alpha.0'"}*

```diff
@@ -18,15 +18,15 @@
         "@phosphor/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
-        "eslint": "^7.4.0",
+        "eslint": "7.4.0",
         "eslint-config-prettier": "^6.11.0",
         "eslint-plugin-prettier": "^3.1.4",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
@@ -45,15 +45,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com//ipylivebash",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c307d6dfc35834975a6a.js"
+            "load": "static/remoteEntry.0287ca83ae9ac6168426.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipylivebash/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -90,9 +90,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0-alpha.0"
 }
```

### Comparing `ipylivebash-0.1.2/ipylivebash/labextension/static/480.e6446a30d6b6a16ad121.js` & `ipylivebash-0.2.0a0/ipylivebash/labextension/static/480.e6446a30d6b6a16ad121.js`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/labextension/static/568.fb1e61d7b0a27a69428e.js` & `ipylivebash-0.2.0a0/ipylivebash/labextension/static/568.fb1e61d7b0a27a69428e.js`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/labextension/static/remoteEntry.c307d6dfc35834975a6a.js` & `ipylivebash-0.2.0a0/ipylivebash/labextension/static/remoteEntry.0287ca83ae9ac6168426.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, s, u, f, p, c, d, h, v = {
+    var e, r, t, n, a, o, i, l, s, u, f, p, d, h, c, v = {
             49: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(367), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(367), t.e(480)]).then((() => () => t(480)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         b = {};
 
     function g(e) {
         var r = b[e];
@@ -37,74 +37,74 @@
     }
     g.m = v, g.c = b, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        367: "21ed93376ff16371416b",
+        367: "7672911d17cc2c4b7cb0",
         480: "e6446a30d6b6a16ad121",
         568: "fb1e61d7b0a27a69428e"
     } [e] + ".js?v=" + {
-        367: "21ed93376ff16371416b",
+        367: "7672911d17cc2c4b7cb0",
         480: "e6446a30d6b6a16ad121",
         568: "fb1e61d7b0a27a69428e"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipylivebash:", g.l = (t, n, o, a) => {
+    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipylivebash:", g.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== o)
+            if (void 0 !== a)
                 for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
                     var f = s[u];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    i.onerror = i.onload = null, clearTimeout(d);
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(p.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, (() => {
         g.S = {};
         var e = {},
             r = {};
         g.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
+                var o = g.S[t],
                     i = "ipylivebash",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = a[e] = a[e] || {},
-                        l = o[r];
-                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (o[r] = {
+                    var a = o[e] = o[e] || {},
+                        l = a[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
                         get: () => Promise.all([g.e(367), g.e(568)]).then((() => () => g(568))),
                         from: i,
                         eager: !1
                     })
-                })("ipylivebash", "0.1.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("ipylivebash", "0.2.0-alpha.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -118,148 +118,148 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + s() + ")" : 1 === l ? "(" + s() + " || " + s() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+        for (o = 1; o < e.length; o++) {
+            var l = e[o];
+            i.push(0 === l ? "not(" + s() + ")" : 1 === l ? "(" + s() + " || " + s() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return s();
 
         function s() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, l = 1, s = !0;; l++, i++) {
                 var u, f, p = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(u = r[i]))[0])) return !s || ("u" == p ? l > n && !o : "" == p != o);
+                if (i >= r.length || "o" == (f = (typeof(u = r[i]))[0])) return !s || ("u" == p ? l > n && !a : "" == p != a);
                 if ("u" == f) {
                     if (!s || "u" != p) return !1
                 } else if (s)
                     if (p == f)
                         if (l <= n) {
                             if (u != e[l]) return !1
                         } else {
-                            if (o ? u > e[l] : u < e[l]) return !1;
+                            if (a ? u > e[l] : u < e[l]) return !1;
                             u != e[l] && (s = !1)
                         }
                 else if ("s" != p && "n" != p) {
-                    if (o || l <= n) return !1;
+                    if (a || l <= n) return !1;
                     s = !1, l--
                 } else {
-                    if (l <= n || f < p != o) return !1;
+                    if (l <= n || f < p != a) return !1;
                     s = !1
                 } else "s" != p && "n" != p && (s = !1, l--)
             }
         }
-        var c = [],
-            d = c.pop.bind(c);
+        var d = [],
+            h = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
+            var c = e[i];
+            d.push(1 == c ? h() | h() : 2 == c ? h() & h() : c ? o(c, r) : !h())
         }
-        return !!d()
+        return !!h()
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
-        var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), c = {}, d = {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", u = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(e, t, a, n)), f(e[t][a])
+    }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
+        var o = g.I(r);
+        return o && o.then ? o.then(e.bind(e, r, g.S[r], t, n, a)) : e(r, g.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), d = {}, h = {
         565: () => p("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ])
-    }, h = {
+    }, c = {
         367: [565]
     }, g.f.consumes = (e, r) => {
-        g.o(h, e) && h[e].forEach((e => {
-            if (g.o(c, e)) return r.push(c[e]);
+        g.o(c, e) && c[e].forEach((e => {
+            if (g.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    c[e] = 0, g.m[e] = t => {
+                    d[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], g.m[e] = t => {
+                    delete d[e], g.m[e] = t => {
                         throw delete g.c[e], r
                     }
                 };
             try {
-                var o = d[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                var a = h[e]();
+                a.then ? r.push(d[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             74: 0
         };
         g.f.j = (r, t) => {
             var n = g.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                    t.push(n[2] = o);
-                    var a = g.p + g.u(r),
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
+                    var o = g.p + g.u(r),
                         i = new Error;
-                    g.l(a, (t => {
+                    g.l(o, (t => {
                         if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                            var a = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, l] = t,
+                var n, a, [o, i, l] = t,
                     s = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) g.o(i, n) && (g.m[n] = i[n]);
                     l && l(g)
                 }
-                for (r && r(t); s < a.length; s++) o = a[s], g.o(e, o) && e[o] && e[o][0](), e[a[s]] = 0
+                for (r && r(t); s < o.length; s++) a = o[s], g.o(e, a) && e[a] && e[a][0](), e[o[s]] = 0
             },
             t = self.webpackChunkipylivebash = self.webpackChunkipylivebash || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var m = g(49);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipylivebash = m
 })();
```

### Comparing `ipylivebash-0.1.2/ipylivebash/labextension/static/third-party-licenses.json` & `ipylivebash-0.2.0a0/ipylivebash/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/logfile.py` & `ipylivebash-0.2.0a0/ipylivebash/logfile.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/logview.py` & `ipylivebash-0.2.0a0/ipylivebash/logview.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 LogView Widget
 """
 
 from ipywidgets import DOMWidget
 from traitlets import Unicode, Any, Int, Bool
+import json
 from ._frontend import module_name, module_version
+import string
+import random
 
 UNKNOWN = "unknown"
 STATUS_TEXT_LINE_LIMIT = 5
 
 
 class LogView(DOMWidget):
     """LogView
@@ -21,25 +24,33 @@
     _view_module_version = Unicode(module_version).tag(sync=True)
 
     messages = Any([]).tag(sync=True)
     status_header = Unicode('').tag(sync=True)
     status = Any([]).tag(sync=True)
     height = Int(0).tag(sync=True)
     running = Bool(False).tag(sync=True)
+    confirmation_required = Bool(False).tag(sync=True)
 
     notification_permission_request = Bool(False).tag(sync=True)
     notification_permission = Unicode(UNKNOWN).tag(sync=True)
 
     notification_message = Unicode('').tag(sync=True)
+    
+    response = Unicode('').tag(sync=True)
+    action = Unicode('').tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.submitted_count = 0
         self.messages_buffer = []
         self.status_buffer = []
+        self.instance_id = ''.join(random.choices(string.ascii_uppercase + string.ascii_lowercase + string.digits, k=8))
+
+    def __repr__(self):
+        return f""
 
     def write_message(self, line):
         self.messages_buffer.append(line)
 
     def write_status(self, status):
         self.status_buffer.append(status)
         if len(self.status_buffer) > STATUS_TEXT_LINE_LIMIT:
@@ -51,18 +62,32 @@
         if len(self.messages_buffer) == 0:
             return
         messages = [self.submitted_count] + self.messages_buffer
         self.submitted_count = self.submitted_count + 1
         self.messages_buffer = []
         self.messages = messages
 
+    def clear(self):
+        self.messages = []
+        self.status = []
+        self.status_header = ""
+        self.submitted_count = 0
+
     def request_notification_permission(self, callback):
         if self.notification_permission != UNKNOWN:
             callback(self.notification_permission)
 
         def getvalue(change):
             self.unobserve(getvalue, "notification_permission")
             callback(change["new"])
 
         self.observe(getvalue, "notification_permission")
         self.notification_permission_request = True
         self.notification_permission_request = False
+
+    def send_action(self, content: str):
+        self.action = ''
+        self.action = json.dumps({
+            "id": self.instance_id + f":{self.submitted_count}",
+            "content": content
+        })
+        self.submitted_count = self.submitted_count + 1
```

### Comparing `ipylivebash-0.1.2/ipylivebash/runner.py` & `ipylivebash-0.2.0a0/ipylivebash/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,27 @@
 from IPython.display import display
-import ipywidgets as widgets
 import subprocess
 import argparse
 import sys
 import time
 import threading
+import json
 from .logview import LogView
 from .logfile import LogFile
 
 
 def run_script(script):
     """
     Run script via Python API.
     It is an internal testing API.
     """
     runner = Runner("")
     runner.run(script)
 
 
-class RunScriptProxy:
-    def __init__(self):
-        self.mutex = threading.Lock()
-        self.is_finished = False
-        self.error = None
-        self.messages = []
-
-    def acquire(self):
-        self.mutex.acquire()
-
-    def release(self):
-        self.mutex.release()
-
-
-def execute_script_in_thread(script):
-    def worker(proxy, script):
-        try:
-            process = subprocess.Popen(script,
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.STDOUT,
-                                       shell=True,
-                                       universal_newlines=True,
-                                       executable='/bin/bash')
-            for line in process.stdout:
-                proxy.acquire()
-                proxy.messages.append(line)
-                proxy.release()
-        except Exception as e:
-            proxy.acquire()
-            proxy.error = e
-            proxy.release()
-
-        proxy.acquire()
-        if process.wait() != 0:
-            proxy.error = Exception("Failed!")
-
-        proxy.is_finished = True
-        proxy.release()
-
-    proxy = RunScriptProxy()
-    thread = threading.Thread(target=worker, args=(proxy, script))
-    thread.start()
-    return proxy
-
-
 def run_chain(funcs):
     if len(funcs) == 0:
         return
     remaining = funcs[1:]
     func = funcs[0]
 
     def next():
@@ -85,159 +40,184 @@
         parser.add_argument('--save-timestamp',
                             action='store_true', dest='use_timestamp',
                             help="Add timestamp to the output file name")
         parser.add_argument('--line-limit',
                             dest='line_limit', default=0, type=int,
                             help="Restrict the no. of lines to be shown")
         parser.add_argument('--height',
-                            dest='height', default=0, type=int,
+                            dest='height', default=4, type=int,
                             help="Set the height of the output cell (no. of line)")
         parser.add_argument('--ask-confirm',
                             action='store_true', dest='ask_confirm',
                             help="Ask for confirmation before execution")
         parser.add_argument('--notify',
                             action='store_true', dest='send_notification',
                             help="Send a notification when the script finished")
-        parser.add_argument('--keep-cell-output',
-                            action='store_true', dest='keep_cell_output',
-                            help="Keep the cell output")
         self.args = parser.parse_args(args)
         self.parser = parser
         self.log_view = LogView()
         self.line_printed = 0
         self.is_executed = False
+
+        self.process = None
+        self.process_finish_messages = [""]
+        
         if self.args.output_file is not None:
             self.log_file = LogFile(
                 pattern=self.args.output_file,
                 use_timestamp=self.args.use_timestamp
             )
         self.log_view.height = self.args.height
-        self.container = widgets.VBox(
-            [self.log_view]
-        )
-        self.grid_box = widgets.GridBox(
-            children=[self.container],
-            layout=widgets.Layout(
-                width="100%",
-                grid_template_rows='auto',
-                grid_template_columns='100%'
-            )
-        )
+        self.log_view.observe(self.on_response, names='response')
 
     def run(self, script):
-        display(self.grid_box)
+        self.script = script
+
+        display(self.log_view)
+
         funcs = [
             lambda next: self.execute_confirmation(next),
+            lambda _: self.run_without_confirmation(),
+        ]
+        run_chain(funcs)
+
+    def run_without_confirmation(self):
+        funcs = [
             lambda next: self.execute_notification(next),
             lambda next: self.execute_logger(next),
-            lambda next: self.execute_script(script, next)
+            lambda next: self.execute_script(self.script, next)
         ]
         run_chain(funcs)
 
     def execute_confirmation(self, next):
         if self.args.ask_confirm is not True:
             next()
             return
 
-        confirm_button = widgets.Button(description="Confirm")
-        cancel_button = widgets.Button(description="Cancel")
-        output = widgets.Output()
-        hbox = widgets.HBox([confirm_button, cancel_button])
-
-        def confirm(_):
-            hbox.layout.display = 'none'
-            output.layout.display = 'none'
-            next()
-
-        def cancel(_):
-            hbox.layout.display = 'none'
-            with output:
-                print("")
-                print("Canceled")
-
-        confirm_button.on_click(confirm)
-        cancel_button.on_click(cancel)
-        self.container.children = [output, hbox] + \
-            list(self.container.children)
-
-        with output:
-            print("Are you sure you want to run this script?")
+        self.log_view.confirmation_required = True
 
     def flush(self):
         self.log_view.flush()
         if self.args.output_file is not None:
             self.log_file.flush()
 
     def write_message(self, line):
         self.line_printed = self.line_printed + 1
         if self.args.output_file is not None:
             self.log_file.write_message(line)
 
-        if self.args.keep_cell_output is True:
-            sys.stdout.write(line)
-            return
-
         if (self.line_printed >= self.args.line_limit and
                 self.args.line_limit > 0):
             if self.log_view.status_header == "":
                 self.log_view.status_header = "=== Output exceed the line limitation. Only the latest output will be shown ==="  # noqa
             self.log_view.write_status(line)
         else:
             self.log_view.write_message(line)
 
     def execute_script(self, script, next):
         if self.is_executed:
             return
+        self.log_view.clear()
         self.is_executed = True
         self.log_view.running = True
+        self.line_printed = 0
+        self.process_finish_messages = []
 
-        try:
-            proxy = execute_script_in_thread(script)
-            while True:
+        pending_messages = []
+        running = True
+        mutex = threading.Lock()
+
+        def worker():
+            nonlocal running
+            nonlocal pending_messages
+
+            # Pause a while to make sure the frontend 
+            # could receive the property changes
+            time.sleep(0.1)
+
+            try:
+                process = subprocess.Popen(script,
+                                        stdout=subprocess.PIPE,
+                                        stderr=subprocess.STDOUT,
+                                        shell=True,
+                                        universal_newlines=True,
+                                        executable='/bin/bash')
+                self.process = process
+                for line in process.stdout:
+                    mutex.acquire()
+                    pending_messages.append(line)
+                    mutex.release()
+            except Exception as e:
+                self.process_finish_messages.append(str(e))
+
+            exit_code = process.poll()
+
+            mutex.acquire()
+
+            if self.args.send_notification:
+                self.log_view.notification_message = "The script is finished"
+
+            for message in self.process_finish_messages:
+                pending_messages.append(message)
+
+            if len(self.process_finish_messages) == 0:
+                pending_messages.append(f"Process finished with exit code {exit_code}")
+
+            self.is_executed = False
+            self.log_view.running = False
+            running = False
+            mutex.release()
+
+
+        def writer():
+            nonlocal running
+            nonlocal pending_messages
+            while running:
                 time.sleep(0.1)
-                proxy.acquire()
-                messages = proxy.messages
-                is_finished = proxy.is_finished
-                error = proxy.error
-                proxy.messages = []
-                proxy.release()
-
-                if len(messages) > 0:
-                    for message in messages:
+                mutex.acquire()
+                if len(pending_messages) > 0:
+                    for message in pending_messages:
                         self.write_message(message)
                     self.flush()
+                    pending_messages = []
+                mutex.release()
 
-                if is_finished or error is not None:
-                    break
-        except Exception as e:
-            error = e
-
-        self.log_view.flush()
-        self.log_view.running = False
+        worker_thread = threading.Thread(target=worker, args=())
+        worker_thread.start()
 
-        if error is not None:
-            raise error
+        writer_thread = threading.Thread(target=writer, args=())
+        writer_thread.start()
 
         next()
 
     def execute_notification(self, next):
         if self.args.send_notification is False:
             next()
             return
 
         def callback(permission):
             if permission != "granted":
                 self.log_view.write_message(
                     f"Request notification permission failed: {permission}")
                 return
             next()
-            self.log_view.notification_message = "The script is finished"
 
         self.log_view.request_notification_permission(callback)
 
     def execute_logger(self, next):
         if self.args.output_file is not None:
-            self.log_file.open()
-            next()
-            self.log_file.close()
-        else:
-            next()
+            try:
+                self.log_file.open()
+            except OSError as e:
+                self.log_view.write_message(str(e))
+                self.log_view.flush()
+                return
+        next()
+
+    def on_response(self, change):
+        response = json.loads(change.new)
+        content = json.loads(response['content'])
+        if content['type'] == 'requestToStop':
+            self.process_finish_messages.append("Force terminated")
+            self.process.terminate()
+        elif content['type'] == 'confirmToRun':
+            self.run_without_confirmation()
```

### Comparing `ipylivebash-0.1.2/ipylivebash/tests/conftest.py` & `ipylivebash-0.2.0a0/ipylivebash/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash/tests/test_logfile.py` & `ipylivebash-0.2.0a0/ipylivebash/tests/test_logfile.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/ipylivebash.egg-info/PKG-INFO` & `ipylivebash-0.2.0a0/ipylivebash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylivebash
-Version: 0.1.2
+Version: 0.2.0a0
 Summary: Run shell script in Jupyter with live output
 Home-page: https://github.com/benlau/ipylivebash
 Author: Ben lau
 Author-email: xbenlau@gmail.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
@@ -172,9 +172,7 @@
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
 
 #### Python:
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
-
-
```

### Comparing `ipylivebash-0.1.2/ipylivebash.egg-info/SOURCES.txt` & `ipylivebash-0.2.0a0/ipylivebash.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,47 +17,52 @@
 docs/img/ask_confirm.png
 docs/source/conf.py
 docs/source/develop-install.rst
 docs/source/index.rst
 docs/source/installing.rst
 docs/source/introduction.rst
 docs/source/_static/embed-bundle.js
+docs/source/_static/embed-bundle.js.LICENSE.txt
 docs/source/_static/embed-bundle.js.map
 docs/source/_static/helper.js
 docs/source/examples/index.rst
 docs/source/examples/introduction.nblink
 examples/introduction.ipynb
+examples/.ipynb_checkpoints/introduction-checkpoint.ipynb
 ipylivebash/__init__.py
 ipylivebash/_frontend.py
 ipylivebash/_version.py
 ipylivebash/debounce.py
 ipylivebash/logfile.py
 ipylivebash/logview.py
 ipylivebash/runner.py
 ipylivebash.egg-info/PKG-INFO
 ipylivebash.egg-info/SOURCES.txt
 ipylivebash.egg-info/dependency_links.txt
 ipylivebash.egg-info/requires.txt
 ipylivebash.egg-info/top_level.txt
 ipylivebash/labextension/package.json
-ipylivebash/labextension/static/367.21ed93376ff16371416b.js
+ipylivebash/labextension/static/367.7672911d17cc2c4b7cb0.js
+ipylivebash/labextension/static/367.7672911d17cc2c4b7cb0.js.LICENSE.txt
 ipylivebash/labextension/static/480.e6446a30d6b6a16ad121.js
 ipylivebash/labextension/static/568.fb1e61d7b0a27a69428e.js
-ipylivebash/labextension/static/remoteEntry.c307d6dfc35834975a6a.js
+ipylivebash/labextension/static/remoteEntry.0287ca83ae9ac6168426.js
 ipylivebash/labextension/static/style.js
 ipylivebash/labextension/static/third-party-licenses.json
 ipylivebash/nbextension/extension.js
 ipylivebash/nbextension/index.js
+ipylivebash/nbextension/index.js.LICENSE.txt
 ipylivebash/nbextension/index.js.map
 ipylivebash/tests/__init__.py
 ipylivebash/tests/conftest.py
 ipylivebash/tests/test_logfile.py
 ipylivebash/tests/test_logview.py
 ipylivebash/tests/test_nbextension_path.py
 ipylivebash/tests/test_runner.py
 src/extension.ts
 src/index.ts
 src/plugin.ts
 src/version.ts
+src/webcomp.ts
 src/widget.ts
 src/__tests__/index.spec.ts
 src/__tests__/utils.ts
```

### Comparing `ipylivebash-0.1.2/package.json` & `ipylivebash-0.2.0a0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9681919642857143%*

 * *Differences: {"'devDependencies'": "{'eslint': '7.4.0'}", "'version'": "'0.2.0-alpha.0'"}*

```diff
@@ -18,15 +18,15 @@
         "@phosphor/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
-        "eslint": "^7.4.0",
+        "eslint": "7.4.0",
         "eslint-config-prettier": "^6.11.0",
         "eslint-plugin-prettier": "^3.1.4",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
@@ -86,9 +86,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0-alpha.0"
 }
```

### Comparing `ipylivebash-0.1.2/setup.py` & `ipylivebash-0.2.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/src/__tests__/index.spec.ts` & `ipylivebash-0.2.0a0/src/__tests__/index.spec.ts`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 // import {} from '@jupyter-widgets/base';
 
 import { createTestModel } from './utils';
 
 import { LogViewModel } from '..';
 
 describe('LogViewModel', () => {
-  describe('LogViewModel', () => {
-    it('should be createable', () => {
-      const model = createTestModel(LogViewModel);
-      expect(model).toBeInstanceOf(LogViewModel);
-      expect(model.get('messages')).toEqual([]);
-    });
+  test('should be createable', () => {
+    const model = createTestModel(LogViewModel);
+    expect(model).toBeInstanceOf(LogViewModel);
+    expect(model.get('messages')).toEqual([]);
+  });
 
-    it('should be createable with a value', () => {
-      const state = { messages: [0, 'Foo Bar!'] };
-      const model = createTestModel(LogViewModel, state);
-      expect(model).toBeInstanceOf(LogViewModel);
-      expect(model.get('messages')).toEqual([0, 'Foo Bar!']);
-    });
+  test('should be createable with a value', () => {
+    const state = { messages: [0, 'Foo Bar!'] };
+    const model = createTestModel(LogViewModel, state);
+    expect(model).toBeInstanceOf(LogViewModel);
+    expect(model.get('messages')).toEqual([0, 'Foo Bar!']);
   });
 });
```

### Comparing `ipylivebash-0.1.2/src/__tests__/utils.ts` & `ipylivebash-0.2.0a0/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/src/extension.ts` & `ipylivebash-0.2.0a0/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/src/plugin.ts` & `ipylivebash-0.2.0a0/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/src/version.ts` & `ipylivebash-0.2.0a0/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipylivebash-0.1.2/src/widget.ts` & `ipylivebash-0.2.0a0/src/widget.ts`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
   DOMWidgetModel,
   DOMWidgetView,
   ISerializers,
 } from '@jupyter-widgets/base';
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
 import '../css/widget.css';
+import './webcomp';
 
 export class LogViewModel extends DOMWidgetModel {
   defaults() {
     return {
       ...super.defaults(),
       _model_name: LogViewModel.model_name,
       _model_module: LogViewModel.model_module,
@@ -21,14 +22,17 @@
       divider_text: '',
       height: 0,
       status: [],
       running: false,
       notification_permission_request: false,
       notification_permission: '',
       notification_message: '',
+      response: '',
+      action: '',
+      confirmation_required: false,
     };
   }
 
   static serializers: ISerializers = {
     ...DOMWidgetModel.serializers,
   };
 
@@ -36,56 +40,33 @@
   static model_module = MODULE_NAME;
   static model_module_version = MODULE_VERSION;
   static view_name = 'LogView';
   static view_module = MODULE_NAME;
   static view_module_version = MODULE_VERSION;
 }
 
+let responseId = 0;
+
 export class LogView extends DOMWidgetView {
   views: any = {};
   status = '';
+  panel: HTMLElement;
 
   render() {
-    const container = document.createElement('div');
-    const content = document.createElement('div');
-    const messageView = document.createElement('div');
-    const statusHeader = document.createElement('div');
-
-    const statusView = document.createElement('div');
-
-    const loadingSpinner = document.createElement('div');
-
-    this.el.classList.add('livebash-log-view');
-
-    container.classList.add('livebash-log-view-container');
-    this.el.appendChild(container);
-
-    loadingSpinner.innerHTML = '<div></div><div></div><div></div><div></div>';
-    this.el.appendChild(loadingSpinner);
-
-    content.setAttribute('tabIndex', '1');
-    container.appendChild(content);
-
-    content.appendChild(messageView);
-    content.appendChild(statusHeader);
-
-    statusHeader.classList.add('livebash-log-view-divider');
-    content.appendChild(statusView);
-
-    this.views = {
-      messageView,
-      statusHeader,
-      statusView,
-      container,
-      loadingSpinner,
-      content,
-    };
+    const panel = document.createElement('live-bash-panel');
+    this.el.appendChild(panel);
+    this.panel = panel;
+    this.panel.setAttribute('tabIndex', '1');
+    this.panel.addEventListener('response', (e: any) => {
+      this.onPanelResponse(JSON.stringify(e.detail));
+    });
 
     this.heightChanged();
     this.runningChanged();
+    this.onConfirmationRequiredChanged();
 
     this.model.on('change:messages', this.messagesChanged, this);
     this.model.on('change:status_header', this.statusHeaderChanged, this);
     this.model.on('change:status', this.statusChanged, this);
     this.model.on('change:height', this.heightChanged, this);
     this.model.on('change:running', this.runningChanged, this);
     this.model.on(
@@ -94,65 +75,48 @@
       this
     );
     this.model.on(
       'change:notification_message',
       this.onNotificationMessageChanged,
       this
     );
+    this.model.on('change:action', this.onActionChanged, this);
+    this.model.on(
+      'change:confirmation_required',
+      this.onConfirmationRequiredChanged,
+      this
+    );
   }
 
   messagesChanged() {
     const value = this.model.get('messages');
-    const messages = value.slice(1);
-    messages.forEach((line: any) => {
-      const elem = document.createElement('p');
-      const text = document.createTextNode(line);
-      elem.appendChild(text);
-      this.views.messageView.appendChild(elem);
-    });
-
-    this.scrollToEnd();
+    this.panel.setAttribute(
+      'messages',
+      value
+        .map((v: string) => {
+          const str = Number.isInteger(v) ? v.toString() : v;
+          return str.replace(/^\s+|\s+$/gm, '');
+        })
+        .join('\n')
+    );
   }
 
   statusHeaderChanged() {
     const value = this.model.get('status_header');
-    this.views.statusHeader.textContent = value;
-  }
-
-  scrollToEnd() {
-    const { container, content } = this.views;
-    container.scrollTop = content.scrollHeight;
+    this.panel.setAttribute('status-header', value);
   }
 
   statusChanged() {
     const value = this.model.get('status');
-    this.views.statusView.textContent = '';
-
-    value
-      .map((line: any) => {
-        const item = document.createElement('div');
-        const text = document.createTextNode(line);
-        item.appendChild(text);
-        return item;
-      })
-      .forEach((item: any) => {
-        this.views.statusView.appendChild(item);
-      });
+    this.panel.setAttribute('status', value.join('\n'));
   }
 
   heightChanged() {
     const value = this.model.get('height');
-    if (value > 0) {
-      const height = `${value * 1.2}em`;
-      const styles = {
-        maxHeight: height,
-        height,
-      };
-      Object.assign(this.views.container.style, styles);
-    }
+    this.panel.setAttribute('height-in-lines', value);
   }
 
   onNotificationPermissionRequestChanged() {
     const value = this.model.get('notification_permission_request');
     if (!value) {
       return;
     }
@@ -171,23 +135,42 @@
       this.model.set('notification_permission', Notification.permission);
       this.model.save_changes();
     });
   }
 
   onNotificationMessageChanged() {
     const value = this.model.get('notification_message');
-    new Notification('livebash', {
+    const notification = new Notification('livebash', {
       body: value,
+      requireInteraction: true
     });
+    notification.onclick = (e) => {
+      notification.close();
+    };
   }
 
   runningChanged() {
     const value = this.model.get('running');
-    const className = 'livebash-lds';
+    this.panel.setAttribute('is-running', value);
+  }
 
-    if (value) {
-      this.views.loadingSpinner.classList.add(className);
-    } else {
-      this.views.loadingSpinner.classList.remove(className);
-    }
+  onPanelResponse(content: string) {
+    const value = {
+      id: responseId++,
+      content,
+    };
+
+    this.model.set('response', JSON.stringify(value));
+    this.model.save_changes();
+    this.touch();
+  }
+
+  onConfirmationRequiredChanged() {
+    const value = this.model.get('confirmation_required');
+    this.panel.setAttribute('confirmation-required', value);
+  }
+
+  onActionChanged() {
+    const value = this.model.get('action');
+    this.panel.setAttribute('action', value);
   }
 }
```

### Comparing `ipylivebash-0.1.2/tsconfig.json` & `ipylivebash-0.2.0a0/tsconfig.json`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,19 @@
     "resolveJsonModule": true,
     "rootDir": "src",
     "skipLibCheck": true,
     "sourceMap": true,
     "strict": true,
     "strictPropertyInitialization": false,
     "target": "es2015",
-    "types": ["jest"]
+    "types": ["jest", "node", "@types/jest"],
+    "typeRoots": [      
+      "./node_modules/@types/",
+      "./src/@types/"
+    ],
   },
   "include": [
     "src/**/*.ts",
     "src/**/*.tsx",
   ],
-  "exclude": ["src/**/__tests__"]
+  "exclude": ["node_modules", "dest", "webcomp"]
 }
```

### Comparing `ipylivebash-0.1.2/webpack.config.js` & `ipylivebash-0.2.0a0/webpack.config.js`

 * *Files identical despite different names*

