# Comparing `tmp/pytodotxt-1.4.3.tar.gz` & `tmp/pytodotxt-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytodotxt-1.4.3.tar", last modified: Sun Oct 30 08:08:51 2022, max compression
+gzip compressed data, was "pytodotxt-1.5.0.tar", last modified: Fri Jun 23 08:45:19 2023, max compression
```

## Comparing `pytodotxt-1.4.3.tar` & `pytodotxt-1.5.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/
--rw-r--r--   0 robert    (1000) robert    (1000)      430 2022-10-29 12:19:15.000000 pytodotxt-1.4.3/AUTHORS.md
--rw-r--r--   0 robert    (1000) robert    (1000)     2562 2022-10-30 08:07:47.000000 pytodotxt-1.4.3/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1112 2022-02-19 09:36:45.000000 pytodotxt-1.4.3/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 17:10:56.000000 pytodotxt-1.4.3/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     1520 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     1006 2022-02-20 07:20:38.000000 pytodotxt-1.4.3/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.143469 pytodotxt-1.4.3/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-19 08:58:46.000000 pytodotxt-1.4.3/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.143469 pytodotxt-1.4.3/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.146802 pytodotxt-1.4.3/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    23409 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5716 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/contributors.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    37674 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)     6898 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6056 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     3994 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6137 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   114149 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/doctrees/reference.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.146802 pytodotxt-1.4.3/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.146802 pytodotxt-1.4.3/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-19 09:57:34.000000 pytodotxt-1.4.3/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       82 2022-02-19 09:55:18.000000 pytodotxt-1.4.3/doc/build/html/_sources/contributors.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      679 2022-02-19 15:53:57.000000 pytodotxt-1.4.3/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      789 2022-02-19 17:15:11.000000 pytodotxt-1.4.3/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      315 2022-02-19 09:51:32.000000 pytodotxt-1.4.3/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-19 09:10:46.000000 pytodotxt-1.4.3/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      322 2022-02-19 17:15:56.000000 pytodotxt-1.4.3/doc/build/html/_sources/reference.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.146802 pytodotxt-1.4.3/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 15:37:56.000000 pytodotxt-1.4.3/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    13633 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4625 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/contributors.html
--rw-r--r--   0 robert    (1000) robert    (1000)    11206 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    10300 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6067 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4679 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5353 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)      678 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    44342 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6600 2022-02-23 15:38:26.000000 pytodotxt-1.4.3/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-19 08:58:46.000000 pytodotxt-1.4.3/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-19 15:06:58.000000 pytodotxt-1.4.3/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-19 09:57:34.000000 pytodotxt-1.4.3/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1869 2022-02-19 17:13:07.000000 pytodotxt-1.4.3/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)       82 2022-02-19 09:55:18.000000 pytodotxt-1.4.3/doc/source/contributors.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      679 2022-02-19 15:53:57.000000 pytodotxt-1.4.3/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      789 2022-02-19 17:15:11.000000 pytodotxt-1.4.3/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      315 2022-02-19 09:51:32.000000 pytodotxt-1.4.3/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-19 09:10:46.000000 pytodotxt-1.4.3/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      322 2022-02-19 17:15:56.000000 pytodotxt-1.4.3/doc/source/reference.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)      227 2022-02-19 15:51:58.000000 pytodotxt-1.4.3/examples/adding_task.py
--rw-r--r--   0 robert    (1000) robert    (1000)      297 2022-02-19 15:54:24.000000 pytodotxt-1.4.3/examples/complete_tasks.py
--rw-r--r--   0 robert    (1000) robert    (1000)      279 2022-02-19 15:53:11.000000 pytodotxt-1.4.3/examples/custom_task.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/pytodotxt/
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-19 13:33:49.000000 pytodotxt-1.4.3/pytodotxt/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    13395 2022-10-29 12:12:37.000000 pytodotxt-1.4.3/pytodotxt/task.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8111 2022-04-24 09:16:54.000000 pytodotxt-1.4.3/pytodotxt/todotxt.py
--rw-r--r--   0 robert    (1000) robert    (1000)       22 2022-10-30 08:07:56.000000 pytodotxt-1.4.3/pytodotxt/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/pytodotxt.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     1520 2022-10-30 08:08:51.000000 pytodotxt-1.4.3/pytodotxt.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     2046 2022-10-30 08:08:51.000000 pytodotxt-1.4.3/pytodotxt.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2022-10-30 08:08:51.000000 pytodotxt-1.4.3/pytodotxt.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       10 2022-10-30 08:08:51.000000 pytodotxt-1.4.3/pytodotxt.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     1614 2022-02-19 17:35:33.000000 pytodotxt-1.4.3/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-10-30 08:08:51.150136 pytodotxt-1.4.3/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)    13312 2022-10-29 11:58:01.000000 pytodotxt-1.4.3/tests/test_pytodotxt.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)      430 2022-10-29 12:19:15.000000 pytodotxt-1.5.0/AUTHORS.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     2679 2023-06-23 08:35:14.000000 pytodotxt-1.5.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1112 2022-02-19 09:36:45.000000 pytodotxt-1.5.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 17:10:56.000000 pytodotxt-1.5.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     1520 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     1006 2022-02-20 07:20:38.000000 pytodotxt-1.5.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-19 08:58:46.000000 pytodotxt-1.5.0/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.196800 pytodotxt-1.5.0/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    23409 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5716 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/contributors.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    37674 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)     6898 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6056 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     3994 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6137 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   114149 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/doctrees/reference.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-19 09:57:34.000000 pytodotxt-1.5.0/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       82 2022-02-19 09:55:18.000000 pytodotxt-1.5.0/doc/build/html/_sources/contributors.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      679 2022-02-19 15:53:57.000000 pytodotxt-1.5.0/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      789 2022-02-19 17:15:11.000000 pytodotxt-1.5.0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      315 2022-02-19 09:51:32.000000 pytodotxt-1.5.0/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-19 09:10:46.000000 pytodotxt-1.5.0/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      322 2022-02-19 17:15:56.000000 pytodotxt-1.5.0/doc/build/html/_sources/reference.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 15:37:56.000000 pytodotxt-1.5.0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    13633 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4625 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/contributors.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    11206 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    10300 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6067 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4679 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5353 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)      678 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    44342 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6600 2022-02-23 15:38:26.000000 pytodotxt-1.5.0/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-19 08:58:46.000000 pytodotxt-1.5.0/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-19 15:06:58.000000 pytodotxt-1.5.0/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.200133 pytodotxt-1.5.0/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-19 09:57:34.000000 pytodotxt-1.5.0/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1869 2022-02-19 17:13:07.000000 pytodotxt-1.5.0/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       82 2022-02-19 09:55:18.000000 pytodotxt-1.5.0/doc/source/contributors.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      679 2022-02-19 15:53:57.000000 pytodotxt-1.5.0/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      789 2022-02-19 17:15:11.000000 pytodotxt-1.5.0/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      315 2022-02-19 09:51:32.000000 pytodotxt-1.5.0/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-19 09:10:46.000000 pytodotxt-1.5.0/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      322 2022-02-19 17:15:56.000000 pytodotxt-1.5.0/doc/source/reference.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)      227 2022-02-19 15:51:58.000000 pytodotxt-1.5.0/examples/adding_task.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      297 2022-02-19 15:54:24.000000 pytodotxt-1.5.0/examples/complete_tasks.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      279 2022-02-19 15:53:11.000000 pytodotxt-1.5.0/examples/custom_task.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-06-23 08:37:32.000000 pytodotxt-1.5.0/pyproject.toml
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/pytodotxt/
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-19 13:33:49.000000 pytodotxt-1.5.0/pytodotxt/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    13395 2022-10-29 12:12:37.000000 pytodotxt-1.5.0/pytodotxt/task.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8151 2023-06-23 08:43:15.000000 pytodotxt-1.5.0/pytodotxt/todotxt.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       21 2023-06-23 08:35:24.000000 pytodotxt-1.5.0/pytodotxt/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/pytodotxt.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1520 2023-06-23 08:45:19.000000 pytodotxt-1.5.0/pytodotxt.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     2061 2023-06-23 08:45:19.000000 pytodotxt-1.5.0/pytodotxt.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-23 08:45:19.000000 pytodotxt-1.5.0/pytodotxt.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       10 2023-06-23 08:45:19.000000 pytodotxt-1.5.0/pytodotxt.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     1614 2022-02-19 17:35:33.000000 pytodotxt-1.5.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 08:45:19.203467 pytodotxt-1.5.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13359 2023-06-23 08:43:03.000000 pytodotxt-1.5.0/tests/test_pytodotxt.py
```

### Comparing `pytodotxt-1.4.3/CHANGELOG.md` & `pytodotxt-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+
+## 1.5.0
+### Fixed
+- Blank lines in a `todo.txt` file are ignored (they used to create a completely empty `Task`)
+
+
 ## 1.4.3
 ### Fixed
 - `Task.remove_attribute` used to remove everything after the first occurrence of a matching attribute name (thanks to [Gal](https://github.com/gal064))
 
 
 ## 1.4.2
 ### Fixed
```

### Comparing `pytodotxt-1.4.3/LICENSE` & `pytodotxt-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/PKG-INFO` & `pytodotxt-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytodotxt
-Version: 1.4.3
+Version: 1.5.0
 Summary: Library to access todo.txt-like task lists
 Home-page: https://vonshednob.cc/pytodotxt
 Author: R
 Author-email: contact+pytodotxt@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytodotxt-1.4.3/README.md` & `pytodotxt-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/Makefile` & `pytodotxt-1.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/changelog.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/contributors.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/contributors.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/environment.pickle` & `pytodotxt-1.5.0/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/examples.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/index.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/install.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/license.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/doctrees/reference.doctree` & `pytodotxt-1.5.0/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_sources/examples.rst.txt` & `pytodotxt-1.5.0/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_sources/index.rst.txt` & `pytodotxt-1.5.0/doc/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/basic.css` & `pytodotxt-1.5.0/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/doctools.js` & `pytodotxt-1.5.0/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/jquery-3.5.1.js` & `pytodotxt-1.5.0/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/jquery.js` & `pytodotxt-1.5.0/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/language_data.js` & `pytodotxt-1.5.0/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/nature.css` & `pytodotxt-1.5.0/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/pygments.css` & `pytodotxt-1.5.0/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/searchtools.js` & `pytodotxt-1.5.0/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/underscore-1.13.1.js` & `pytodotxt-1.5.0/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/_static/underscore.js` & `pytodotxt-1.5.0/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/changelog.html` & `pytodotxt-1.5.0/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/contributors.html` & `pytodotxt-1.5.0/doc/build/html/contributors.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/examples.html` & `pytodotxt-1.5.0/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/genindex.html` & `pytodotxt-1.5.0/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/index.html` & `pytodotxt-1.5.0/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/install.html` & `pytodotxt-1.5.0/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/license.html` & `pytodotxt-1.5.0/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/objects.inv` & `pytodotxt-1.5.0/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/reference.html` & `pytodotxt-1.5.0/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/search.html` & `pytodotxt-1.5.0/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/build/html/searchindex.js` & `pytodotxt-1.5.0/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/make.bat` & `pytodotxt-1.5.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/source/conf.py` & `pytodotxt-1.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/source/examples.rst` & `pytodotxt-1.5.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/doc/source/index.rst` & `pytodotxt-1.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/pytodotxt/task.py` & `pytodotxt-1.5.0/pytodotxt/task.py`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/pytodotxt/todotxt.py` & `pytodotxt-1.5.0/pytodotxt/todotxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,16 @@
         # determine line separator
         for ch in ['\r\n', '\n', '\r']:
             if ch in text:
                 self.linesep = ch
                 break
 
         return [self.task_type(line, linenr)
-                for linenr, line in enumerate(text.rstrip().split(self.linesep))]
+                for linenr, line in enumerate(text.rstrip().split(self.linesep))
+                if len(line.strip()) > 0]
 
     def parse_file(self, path):
         """Parse the content of the file at ``path``
 
         :param path: The file to parse
         :return: a list of tasks found in ``file``.
         """
@@ -221,8 +222,8 @@
         :return: a list of tasks found in ``stream``
         """
         # get the text from the stream
         blob = stream.read()
         if not isinstance(blob, str):
             blob = str(blob, self.encoding)
 
-        return self.parse_str(blob)
+        return self.parse_str(blob)
```

### Comparing `pytodotxt-1.4.3/pytodotxt.egg-info/PKG-INFO` & `pytodotxt-1.5.0/pytodotxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytodotxt
-Version: 1.4.3
+Version: 1.5.0
 Summary: Library to access todo.txt-like task lists
 Home-page: https://vonshednob.cc/pytodotxt
 Author: R
 Author-email: contact+pytodotxt@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytodotxt-1.4.3/pytodotxt.egg-info/SOURCES.txt` & `pytodotxt-1.5.0/pytodotxt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 doc/Makefile
 doc/make.bat
 doc/requirements.txt
 doc/build/doctrees/changelog.doctree
 doc/build/doctrees/contributors.doctree
 doc/build/doctrees/environment.pickle
```

### Comparing `pytodotxt-1.4.3/setup.py` & `pytodotxt-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytodotxt-1.4.3/tests/test_pytodotxt.py` & `pytodotxt-1.5.0/tests/test_pytodotxt.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,19 +311,21 @@
     def test_add_first(self):
         todotxt = pytodotxt.TodoTxt(self.tmpfile.name)
         self.assertEqual(len(todotxt.tasks), 0)
 
         task = pytodotxt.Task("Some task")
         todotxt.add(task)
         todotxt.save()
+        todotxt.parse()
 
         self.assertEqual(Path(self.tmpfile.name).read_text(encoding="utf-8"),
                          "Some task" + os.linesep)
 
     def test_blank_newlines(self):
         Path(self.tmpfile.name).write_text("\n\n", encoding='utf-8')
         todotxt = pytodotxt.TodoTxt(self.tmpfile.name)
+        todotxt.parse()
         self.assertEqual(len(todotxt.tasks), 0)
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

