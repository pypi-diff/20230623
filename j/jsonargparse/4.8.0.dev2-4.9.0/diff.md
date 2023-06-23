# Comparing `tmp/jsonargparse-4.8.0.dev2.tar.gz` & `tmp/jsonargparse-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonargparse-4.8.0.dev2.tar", last modified: Wed May 25 13:21:39 2022, max compression
+gzip compressed data, was "jsonargparse-4.9.0.tar", last modified: Wed Jun  1 07:14:55 2022, max compression
```

## Comparing `jsonargparse-4.8.0.dev2.tar` & `jsonargparse-4.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-25 13:21:39.798621 jsonargparse-4.8.0.dev2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1115 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/LICENSE.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    65481 2022-05-25 13:21:39.802621 jsonargparse-4.8.0.dev2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69209 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-25 13:21:39.798621 jsonargparse-4.8.0.dev2/jsonargparse/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42482 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5687 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    57544 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8941 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/deprecated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9390 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/formatters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6490 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/jsonnet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5388 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/jsonschema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6222 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/loaders_dumpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10879 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/namespace.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6294 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/optionals.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26885 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/signatures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/type_checking.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37341 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/typehints.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12943 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/typing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      190 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/typing.pyi
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20576 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse/util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-25 13:21:39.798621 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    65481 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1298 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1083 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-25 13:21:39.798621 jsonargparse-4.8.0.dev2/jsonargparse_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1305 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/__main__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    14539 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/actions_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11834 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/argcomplete_tests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1647 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/base.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    10798 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/cli_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    48692 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/core_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11551 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/deprecated_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4246 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/formatters_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7702 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/jsonnet_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4346 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/jsonschema_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4725 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/loaders_dumpers_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6664 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/namespace_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7141 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/optionals_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    63856 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/signatures_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    44172 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/typehints_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9806 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/typing_tests.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11671 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/jsonargparse_tests/util_tests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3103 2022-05-25 13:21:39.802621 jsonargparse-4.8.0.dev2/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1695 2022-05-25 13:21:39.000000 jsonargparse-4.8.0.dev2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:14:55.618012 jsonargparse-4.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1115 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/LICENSE.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    65860 2022-06-01 07:14:55.622012 jsonargparse-4.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    69571 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:14:55.618012 jsonargparse-4.9.0/jsonargparse/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    42526 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5679 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    57666 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8941 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/deprecated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9857 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/formatters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6490 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/jsonnet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5357 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/jsonschema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6216 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/loaders_dumpers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10879 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/namespace.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6294 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/optionals.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26900 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/signatures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/type_checking.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37771 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/typehints.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12943 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/typing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      190 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/typing.pyi
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20635 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse/util.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:14:55.618012 jsonargparse-4.9.0/jsonargparse.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    65860 2022-06-01 07:14:55.000000 jsonargparse-4.9.0/jsonargparse.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1298 2022-06-01 07:14:55.000000 jsonargparse-4.9.0/jsonargparse.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-01 07:14:55.000000 jsonargparse-4.9.0/jsonargparse.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1232 2022-06-01 07:14:55.000000 jsonargparse-4.9.0/jsonargparse.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2022-06-01 07:14:55.000000 jsonargparse-4.9.0/jsonargparse.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-01 07:14:55.618012 jsonargparse-4.9.0/jsonargparse_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1305 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/__main__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    14539 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/actions_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11834 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/argcomplete_tests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1647 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/base.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    10798 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/cli_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    48824 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/core_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11551 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/deprecated_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4246 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/formatters_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7702 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/jsonnet_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4346 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/jsonschema_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4725 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/loaders_dumpers_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6662 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/namespace_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7141 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/optionals_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    63997 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/signatures_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    46461 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/typehints_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9806 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/typing_tests.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    11671 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/jsonargparse_tests/util_tests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3221 2022-06-01 07:14:55.622012 jsonargparse-4.9.0/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1613 2022-06-01 07:14:54.000000 jsonargparse-4.9.0/setup.py
```

### Comparing `jsonargparse-4.8.0.dev2/LICENSE.rst` & `jsonargparse-4.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/PKG-INFO` & `jsonargparse-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonargparse
-Version: 4.8.0.dev2
+Version: 4.9.0
 Summary: Parsing of command line options, yaml/jsonnet config files and/or environment variables based on argparse.
 Home-page: https://github.com/omni-us/jsonargparse
 Author: Mauricio Villegas
 Author-email: mauricio@omnius.com
 License: MIT
 Project-URL: Documentation-stable, https://jsonargparse.readthedocs.io/en/stable/
 Project-URL: Documentation-latest, https://jsonargparse.readthedocs.io/en/latest/
@@ -42,14 +42,15 @@
 Provides-Extra: omegaconf
 Provides-Extra: typing_extensions
 Provides-Extra: reconplogger
 Provides-Extra: test
 Provides-Extra: test_no_urls
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: maintainer
 License-File: LICENSE.rst
 
 .. image:: https://readthedocs.org/projects/jsonargparse/badge/?version=stable
     :target: https://jsonargparse.readthedocs.io/en/stable/
 .. image:: https://github.com/omni-us/jsonargparse/actions/workflows/ci_test.yml/badge.svg
     :target: https://github.com/omni-us/jsonargparse/actions/workflows/ci_test.yml
 .. image:: https://codecov.io/gh/omni-us/jsonargparse/branch/master/graph/badge.svg
@@ -256,21 +257,36 @@
 functions are not automatically printed. `.CLI` returns its value and it
 is up to the developer to decide what to do with it. Finally, jsonargparse has
 many features designed to help in creating convenient argument parsers such as:
 `nested-namespaces`, `configuration-files`, additional type hints
 (`parsing-paths`, `restricted-numbers`, `restricted-strings`) and
 much more.
 
-The next section explains how to create an argument parser in a low level
+Section `parsers` explains how to create an argument parser in a low level
 argparse-style. However, as parsers get more complex, being able to define them
 in a modular way becomes important. Three mechanisms are available for
 modularity, see respective sections `classes-methods-functions`,
 `sub-commands` and `parser-arguments`.
 
 
+.. _tutorials:
+
+Tutorials
+=========
+
+- `"jsonargparse - Say goodbye to configuration hassles"
+  <https://2022.pycon.de/program/XK73C3/>`__  by Marianne Stecklina at PyCon DE
+  & PyData Berlin 2022
+
+    - Presentation video: https://youtu.be/2gDf2S0nHKg
+    - GitHub repository: https://github.com/stecklin/pycon22-jsonargparse
+
+
+.. _parsers:
+
 Parsers
 =======
 
 An argument parser is created just like it is done with python's `argparse
 <https://docs.python.org/3/library/argparse.html>`__. You import the module,
 create a parser object and then add arguments to it. A simple example would be:
 
@@ -840,18 +856,18 @@
 - ``Tuple``, ``Set`` and ``MutableSet`` are supported even though they can't be
   represented in json distinguishable from a list. Each ``Tuple`` element
   position can have its own type and will be validated as such. ``Tuple`` with
   ellipsis (``Tuple[type, ...]``) is also supported. In command line arguments,
   config files and environment variables, tuples and sets are represented as an
   array.
 
-- ``dataclasses`` are supported as a type but without any nesting and for pure
-  data classes. By pure it is meant that it only inherits from data classes. Not
-  a mixture of normal classes and data classes. Data classes as fields of other
-  data classes is supported.
+- ``dataclasses`` are supported as a type but only for pure data classes and not
+  nested in a type. By pure it is meant that the class only inherits from data
+  classes. Not a mixture of normal classes and data classes. Data classes as
+  fields of other data classes is supported.
 
 - To set a value to ``None`` it is required to use ``null`` since this is how
   json/yaml defines it. To avoid confusion in the help, ``NoneType`` is
   displayed as ``null``. For example a function argument with type and default
   ``Optional[str] = None`` would be shown in the help as ``type: Union[str,
   null], default: null``.
```

### Comparing `jsonargparse-4.8.0.dev2/README.rst` & `jsonargparse-4.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -216,21 +216,36 @@
 functions are not automatically printed. :func:`.CLI` returns its value and it
 is up to the developer to decide what to do with it. Finally, jsonargparse has
 many features designed to help in creating convenient argument parsers such as:
 :ref:`nested-namespaces`, :ref:`configuration-files`, additional type hints
 (:ref:`parsing-paths`, :ref:`restricted-numbers`, :ref:`restricted-strings`) and
 much more.
 
-The next section explains how to create an argument parser in a low level
+Section :ref:`parsers` explains how to create an argument parser in a low level
 argparse-style. However, as parsers get more complex, being able to define them
 in a modular way becomes important. Three mechanisms are available for
 modularity, see respective sections :ref:`classes-methods-functions`,
 :ref:`sub-commands` and :ref:`parser-arguments`.
 
 
+.. _tutorials:
+
+Tutorials
+=========
+
+- `"jsonargparse - Say goodbye to configuration hassles"
+  <https://2022.pycon.de/program/XK73C3/>`__  by Marianne Stecklina at PyCon DE
+  & PyData Berlin 2022
+
+    - Presentation video: https://youtu.be/2gDf2S0nHKg
+    - GitHub repository: https://github.com/stecklin/pycon22-jsonargparse
+
+
+.. _parsers:
+
 Parsers
 =======
 
 An argument parser is created just like it is done with python's `argparse
 <https://docs.python.org/3/library/argparse.html>`__. You import the module,
 create a parser object and then add arguments to it. A simple example would be:
 
@@ -835,18 +850,18 @@
 - ``Tuple``, ``Set`` and ``MutableSet`` are supported even though they can't be
   represented in json distinguishable from a list. Each ``Tuple`` element
   position can have its own type and will be validated as such. ``Tuple`` with
   ellipsis (``Tuple[type, ...]``) is also supported. In command line arguments,
   config files and environment variables, tuples and sets are represented as an
   array.
 
-- ``dataclasses`` are supported as a type but without any nesting and for pure
-  data classes. By pure it is meant that it only inherits from data classes. Not
-  a mixture of normal classes and data classes. Data classes as fields of other
-  data classes is supported.
+- ``dataclasses`` are supported as a type but only for pure data classes and not
+  nested in a type. By pure it is meant that the class only inherits from data
+  classes. Not a mixture of normal classes and data classes. Data classes as
+  fields of other data classes is supported.
 
 - To set a value to ``None`` it is required to use ``null`` since this is how
   json/yaml defines it. To avoid confusion in the help, ``NoneType`` is
   displayed as ``null``. For example a function argument with type and default
   ``Optional[str] = None`` would be shown in the help as ``type: Union[str,
   null], default: null``.
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/__init__.py` & `jsonargparse-4.9.0/jsonargparse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 __all__ += formatters.__all__
 __all__ += optionals.__all__
 __all__ += loaders_dumpers.__all__
 __all__ += util.__all__
 __all__ += deprecated.__all__
 
 
-__version__ = '4.8.0.dev2'
+__version__ = '4.9.0'
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/actions.py` & `jsonargparse-4.9.0/jsonargparse/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ParserError,
     import_object,
     change_to_path_dir,
     NoneType,
     indent_text,
     Path,
     _parse_value_or_config,
-    _issubclass,
+    is_subclass,
 )
 
 
 __all__ = [
     'ActionConfigFile',
     'ActionYesNo',
     'ActionParser',
@@ -241,15 +241,15 @@
                  dest=SUPPRESS,
                  default=SUPPRESS):
         super().__init__(option_strings=option_strings,
                          dest=dest,
                          default=default,
                          nargs=1,
                          metavar='[={comments,skip_null,skip_default}+]',
-                         help='Print configuration and exit.')
+                         help='Print the configuration after applying all other arguments and exit.')
 
     def __call__(self, parser, namespace, value, option_string=None):
         kwargs = {'subparser': parser, 'key': None, 'skip_none': False, 'skip_check': True}
         valid_flags = {'': None, 'comments': 'yaml_comments', 'skip_default': 'skip_default', 'skip_null': 'skip_none'}
         if value is not None:
             flags = value[0].split(',')
             invalid_flags = [f for f in flags if f not in valid_flags]
@@ -345,15 +345,15 @@
 
     def update_init_kwargs(self, kwargs):
         if getattr(self._baseclass, '__origin__', None) == Union:
             self._basename = '{'+', '.join(c.__name__ for c in self._baseclass.__args__ if c != NoneType)+'}'
         else:
             self._basename = self._baseclass.__name__
         kwargs.update({
-            'metavar': 'CLASS',
+            'metavar': 'CLASS_NAME_OR_PATH',
             'default': SUPPRESS,
             'help': f'Show the help for the given subclass of {self._basename} and exit.',
         })
 
     def __call__(self, *args, **kwargs):
         if len(args) == 0:
             kwargs['_baseclass'] = self._baseclass
@@ -367,15 +367,15 @@
             val_class = import_object(resolve_class_path_by_name(baseclass, call_args[2]))
         except Exception as ex:
             raise TypeError(f'{call_args[3]}: {ex}')
         if getattr(self._baseclass, '__origin__', None) == Union:
             baseclasses = self._baseclass.__args__
         else:
             baseclasses = [baseclass]
-        if not any(_issubclass(val_class, b) for b in baseclasses):
+        if not any(is_subclass(val_class, b) for b in baseclasses):
             raise TypeError(f'{call_args[3]}: Class "{call_args[2]}" is not a subclass of {self._basename}')
         dest += '.init_args'
         subparser = import_object('jsonargparse.ArgumentParser')()
         subparser.add_class_arguments(val_class, dest, **self.sub_add_kwargs)
         _remove_actions(subparser, (_HelpAction, _ActionPrintConfig, _ActionConfigLoad))
         args = self.get_extra_args(call_args[0].args)
         if args:
@@ -737,15 +737,15 @@
         if not (len(args) == 1 and args[0][:2] == '--'):
             raise ValueError(f'ActionParser only accepts a single optional key but got {args}')
         prefix = args[0][2:]
 
         def add_prefix(key):
             return re.sub('^--', '--'+prefix+'.', key)
 
-        required_args = set(prefix+'.'+x for x in subparser.required_args)
+        required_args = {prefix+'.'+x for x in subparser.required_args}
 
         option_string_actions = {}
         for key, action in filter_default_actions(subparser._option_string_actions).items():
             option_string_actions[add_prefix(key)] = action
 
         isect = set(option_string_actions.keys()).intersection(set(parser._option_string_actions.keys()))
         if len(isect) > 0:
@@ -1017,15 +1017,15 @@
         if not islist and not isinstance(value, list):
             value = [value]
         if isinstance(value, list) and all(not isinstance(v, self._type) for v in value):
             path_list_files = value
             value = []
             for path_list_file in path_list_files:
                 try:
-                    with sys.stdin if path_list_file == '-' else open(path_list_file, 'r') as f:
+                    with sys.stdin if path_list_file == '-' else open(path_list_file) as f:
                         path_list = [x.strip() for x in f.readlines()]
                 except FileNotFoundError as ex:
                     raise TypeError(f'Problems reading path list: {path_list_file} :: {ex}') from ex
                 cwd = os.getcwd()
                 if self._rel == 'list' and path_list_file != '-':
                     os.chdir(os.path.abspath(os.path.join(path_list_file, os.pardir)))
                 try:
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/cli.py` & `jsonargparse-4.9.0/jsonargparse/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,22 +91,22 @@
     component = comp_dict[subcommand]
     return _run_component(component, cfg_init.get(subcommand))
 
 
 def _get_help_str(component):
     help_str = str(component)
     if docstring_parser_support:
-        docstring_parse, DocstringParseError = import_docstring_parse('_get_help_str', True)
+        docstring_parse, docstring_error = import_docstring_parse('_get_help_str', True)
         description = None
         try:
             if inspect.isclass(component):
                 description = docstring_parse(component.__init__.__doc__).short_description
             if description is None:
                 description = docstring_parse(component.__doc__).short_description
-        except (ValueError, DocstringParseError):
+        except (ValueError, docstring_error):
             pass
         if description is not None:
             help_str = description
     return help_str
 
 
 def _add_component_to_parser(component, parser, as_positional, config_help):
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/core.py` & `jsonargparse-4.9.0/jsonargparse/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     return_parser_if_captured,
 )
 
 
 __all__ = ['ActionsContainer', 'ArgumentParser']
 
 
-class ActionsContainer(SignatureArguments, argparse._ActionsContainer, LoggerProperty):
+class ActionsContainer(SignatureArguments, LoggerProperty, argparse._ActionsContainer):
     """Extension of argparse._ActionsContainer to support additional functionalities."""
 
     _action_groups: Sequence['_ArgumentGroup']  # type: ignore
 
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -122,15 +122,15 @@
         """Adds a group to the parser.
 
         All the arguments from `argparse.ArgumentParser.add_argument_group
         <https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_argument_group>`_
         are supported. Additionally it accepts:
 
         Args:
-            name: Name of the group. If set the group object will be included in the parser.groups dict.
+            name: Name of the group. If set, the group object will be included in the parser.groups dict.
 
         Returns:
             The group object.
 
         Raises:
             ValueError: If group with the same name already exists.
         """
@@ -179,18 +179,18 @@
 
         All the arguments from the initializer of `argparse.ArgumentParser
         <https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser>`_
         are supported. Additionally it accepts:
 
         Args:
             env_prefix: Prefix for environment variables.
-            error_handler: Handler for parsing errors, set to None to simply raise exception.
+            error_handler: Handler for parsing errors, if None raises :class:`.ParserError` exception.
             formatter_class: Class for printing help messages.
             logger: Configures the logger, see :class:`.LoggerProperty`.
-            version: Program version string to add --version argument.
+            version: Program version which will be printed by the --version argument.
             print_config: Add this as argument to print config, set None to disable.
             parser_mode: Mode for parsing configuration files: ``'yaml'``, ``'jsonnet'`` or ones added via :func:`.set_loader`.
             dump_header: Header to include as comment when dumping a config object.
             default_config_files: Default config file locations, e.g. :code:`['~/.config/myapp/*.yaml']`.
             default_env: Set the default value on whether to parse environment variables.
             default_meta: Set the default value on whether to include metadata in config objects.
         """
@@ -648,15 +648,16 @@
         Args:
             required: Whether the subcommand must be provided.
             dest: Destination key where the chosen subcommand name is stored.
             **kwargs: All options that `argparse.ArgumentParser.add_subparsers` accepts.
         """
         if 'description' not in kwargs:
             kwargs['description'] = 'For more details of each subcommand add it as argument followed by --help.'
-        subcommands: _ActionSubCommands = super().add_subparsers(dest=dest, **kwargs)  # type: ignore
+        with formatter_context(self):
+            subcommands: _ActionSubCommands = super().add_subparsers(dest=dest, **kwargs)  # type: ignore
         if required:
             self.required_args.add(dest)
         subcommands._required = required  # type: ignore
         subcommands.required = False
         subcommands.parent_parser = self  # type: ignore
         subcommands._env_prefix = self.env_prefix
         self._subcommands_action = subcommands
@@ -900,15 +901,15 @@
         Args:
             dest: Destination key from which to get the default.
 
         Raises:
             KeyError: If key or its default not defined in the parser.
         """
         action, _ = _find_parent_action_and_subcommand(self, dest)
-        if action is None or dest != action.dest or action.dest == argparse.SUPPRESS:
+        if action is None or dest != action.dest:
             raise KeyError(f'No action for destination key "{dest}" to get its default.')
 
         def check_suppressed_default():
             if action.default == argparse.SUPPRESS:
                 raise KeyError(f'Action for destination key "{dest}" does not specify a default.')
 
         if not self._get_default_config_files():
@@ -1072,15 +1073,15 @@
         components: List[Union[ActionTypeHint, _ActionConfigLoad, _ArgumentGroup]] = []
         for action in filter_default_actions(self._actions):
             if isinstance(action, ActionTypeHint) or \
                (isinstance(action, _ActionConfigLoad) and is_pure_dataclass(action.basetype)):
                 components.append(action)
 
         if instantiate_groups:
-            skip = set(c.dest for c in components)
+            skip = {c.dest for c in components}
             groups = [g for g in self._action_groups if hasattr(g, 'instantiate_class') and g.dest not in skip]
             components.extend(groups)
 
         components.sort(key=lambda x: -len(split_key(x.dest)))  # type: ignore
         order = _ActionLink.instantiation_order(self)
         components = _ActionLink.reorder(order, components)
 
@@ -1164,14 +1165,19 @@
             group = self._default_config_files_group
             group.description = f'{self._default_config_files}, Note: {note}'
         with formatter_context(self, defaults):
             help_str = super().format_help()
         return help_str
 
 
+    def print_usage(self, file=None):
+        with formatter_context(self):
+            return super().print_usage(file)
+
+
     def _apply_actions(self, cfg: Union[Namespace, Dict[str, Any]], parent_key: str = '') -> Namespace:
         """Runs _check_value_key on actions present in config."""
         if isinstance(cfg, dict):
             cfg = Namespace(cfg)
         if parent_key:
             cfg_branch = cfg
             cfg = Namespace()
@@ -1192,18 +1198,17 @@
                     value = Namespace(value)
                 if isinstance(value, Namespace):
                     new_keys = value.__dict__.keys()
                     keys += [key+'.'+k for k in new_keys if key+'.'+k not in keys]
                 cfg[key] = value
                 continue
             action_dest = action.dest if subcommand is None else subcommand+'.'+action.dest
-            with _lenient_check_context():
-                value = cfg[action_dest]
-                with load_value_context(self.parser_mode):
-                    value = self._check_value_key(action, value, action_dest, cfg)
+            value = cfg[action_dest]
+            with _lenient_check_context(), load_value_context(self.parser_mode):
+                value = self._check_value_key(action, value, action_dest, cfg)
             if isinstance(action, _ActionConfigLoad):
                 config_keys.add(action_dest)
                 keys.append(action_dest)
             cfg[action_dest] = value
         return cfg[parent_key] if parent_key else cfg
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/deprecated.py` & `jsonargparse-4.9.0/jsonargparse/deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from enum import Enum
 from typing import Any, Dict, Set
 from .namespace import Namespace
 from .optionals import get_config_read_mode, set_config_read_mode
 from .typehints import ActionTypeHint
 from .typing import path_type, restricted_number_type, registered_types
-from .util import _issubclass, warning
+from .util import is_subclass, warning
 
 
 __all__ = [
     'ActionEnum',
     'ActionOperators',
     'ActionPath',
     'set_url_support',
@@ -174,15 +174,15 @@
     should be given directly as a type as explained in :ref:`enums`.
 """)
 class ActionEnum:
     """An action based on an Enum that maps to-from strings and enum values."""
 
     def __init__(self, **kwargs):
         if 'enum' in kwargs:
-            if not _issubclass(kwargs['enum'], Enum):
+            if not is_subclass(kwargs['enum'], Enum):
                 raise ValueError('Expected enum to be an subclass of Enum.')
             self._type = kwargs['enum']
         else:
             raise ValueError('Expected enum keyword argument.')
 
     def __call__(self, *args, **kwargs):
         return ActionTypeHint(typehint=self._type)(**kwargs)
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/formatters.py` & `jsonargparse-4.9.0/jsonargparse/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,27 @@
            (action.option_strings or action.nargs in {OPTIONAL, ZERO_OR_MORE}):
             help_str += (', ' if help_str else '') + 'default: %(default)s'
         if isinstance(action, ActionTypeHint):
             help_str += action.extra_help()
         return action_help + (' ('+help_str+')' if help_str else '')
 
 
+    def _format_usage(self, *args, **kwargs):
+        usage = super()._format_usage(*args, **kwargs)
+        parser = formatter_parser.get()
+        for key in parser.required_args:
+            try:
+                default = parser.get_default(key)
+            except KeyError:
+                default = None
+            if default is None and f'[--{key} ' in usage:
+                usage = re.sub(f'\\[(--{key} [^\\]]+)]', r'\1', usage, count=1)
+        return usage
+
+
     def _format_action_invocation(self, action):
         parser = formatter_parser.get()
         if action.option_strings == [] or action.default == SUPPRESS or not parser.default_env:
             return super()._format_action_invocation(action)
         extr = ''
         if parser.default_env:
             extr += '\n  ENV:   ' + get_env_var(self, action)
@@ -163,15 +176,15 @@
 
         group_titles = {}
         for parser_key, parser in parsers.items():
             prefix = '' if parser_key is None else parser_key + '.'
             for group in parser._action_groups:
                 actions = filter_default_actions(group._group_actions)
                 actions = [a for a in actions if not isinstance(a, (_ActionConfigLoad, ActionConfigFile, _ActionSubCommands))]
-                keys = set(re.sub(r'\.?[^.]+$', '', a.dest) for a in actions)
+                keys = {re.sub(r'\.?[^.]+$', '', a.dest) for a in actions}
                 for key in keys:
                     full_key = prefix + key if key != '' else parser_key
                     group_titles[full_key] = group.title
 
         def set_comments(cfg, prefix='', depth=0):
             for key in cfg.keys():
                 full_key = (prefix+'.' if prefix else '')+key
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/jsonnet.py` & `jsonargparse-4.9.0/jsonargparse/jsonnet.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/jsonschema.py` & `jsonargparse-4.9.0/jsonargparse/jsonschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,15 @@
         validate_properties = validator_class.VALIDATORS['properties']
 
         def set_defaults(validator, properties, instance, schema):
             for prop, subschema in properties.items():
                 if 'default' in subschema:
                     instance.setdefault(prop, subschema['default'])
 
-            for error in validate_properties(validator, properties, instance, schema):
-                yield error
+            yield from validate_properties(validator, properties, instance, schema)
 
         jsonschema = import_jsonschema('ActionJsonSchema')[0]
         return jsonschema.validators.extend(validator_class, {'properties': set_defaults})
 
 
     def completer(self, prefix, **kwargs):
         """Used by argcomplete, validates value and shows expected type."""
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/loaders_dumpers.py` & `jsonargparse-4.9.0/jsonargparse/loaders_dumpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,30 +47,30 @@
 
 
 remove_implicit_resolver(DefaultLoader, 'tag:yaml.org,2002:timestamp')
 remove_implicit_resolver(DefaultLoader, 'tag:yaml.org,2002:float')
 
 
 DefaultLoader.add_implicit_resolver(
-    u'tag:yaml.org,2002:float',
-    re.compile(u'''^(?:
+    'tag:yaml.org,2002:float',
+    re.compile('''^(?:
      [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
     |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
     |\\.[0-9_]+(?:[eE][-+][0-9]+)?
     |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
     |[-+]?\\.(?:inf|Inf|INF)
     |\\.(?:nan|NaN|NAN))$''', re.X),
-    list(u'-+0123456789.'),
+    list('-+0123456789.'),
 )
 
 
 def yaml_load(stream):
     value = yaml.load(stream, Loader=DefaultLoader)
     if isinstance(value, dict) and all(v is None for v in value.values()):
-        keys = set(k for k in regex_curly_comma.split(stream) if k)
+        keys = {k for k in regex_curly_comma.split(stream) if k}
         if len(keys) > 0 and keys == set(value.keys()):
             value = stream
     return value
 
 
 def jsonnet_load(stream, path='', ext_vars=None):
     from .jsonnet import ActionJsonnet
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/namespace.py` & `jsonargparse-4.9.0/jsonargparse/namespace.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/optionals.py` & `jsonargparse-4.9.0/jsonargparse/optionals.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/signatures.py` & `jsonargparse-4.9.0/jsonargparse/signatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import wraps
 from typing import Any, Callable, List, Optional, Set, Tuple, Type, Union
 
 from .actions import _ActionConfigLoad
 from .namespace import Namespace
 from .typehints import ActionTypeHint, ClassType, is_optional, LazyInitBaseClass
 from .typing import is_final_class
-from .util import get_import_path, _issubclass
+from .util import get_import_path, is_subclass
 from .optionals import (
     dataclasses_support,
     docstring_parser_support,
     import_dataclasses,
     import_docstring_parse,
 )
 
@@ -69,15 +69,15 @@
             ValueError: When there are required parameters without at least one valid type.
         """
         if not inspect.isclass(theclass):
             raise ValueError(f'Expected "theclass" parameter to be a class type, got: {theclass}.')
         if default and not (isinstance(default, LazyInitBaseClass) and isinstance(default, theclass)):
             raise ValueError(f'Expected "default" parameter to be a lazy instance of the class, got: {default}.')
 
-        skip_first = not _issubclass(theclass, ClassFromFunctionBase)
+        skip_first = not is_subclass(theclass, ClassFromFunctionBase)
 
         added_args = self._add_signature_arguments(
             inspect.getmro(theclass),
             nested_key,
             as_group,
             as_positional,
             skip,
@@ -339,15 +339,15 @@
         elif not as_positional:
             kwargs['required'] = True
         is_subclass_typehint = False
         is_final_class_typehint = is_final_class(annotation)
         dest = (nested_key+'.' if nested_key else '') + name
         args = [dest if is_required and as_positional else '--'+dest]
         if annotation in {str, int, float, bool} or \
-           _issubclass(annotation, (str, int, float)) or \
+           is_subclass(annotation, (str, int, float)) or \
            is_final_class_typehint or \
            is_pure_dataclass(annotation):
             kwargs['type'] = annotation
         elif annotation != inspect_empty:
             try:
                 is_subclass_typehint = ActionTypeHint.is_subclass_typehint(annotation)
                 kwargs['type'] = annotation
@@ -451,16 +451,16 @@
         self,
         baseclass: Union[Type, Tuple[Type, ...]],
         nested_key: str,
         as_group: bool = True,
         skip: Optional[Set[str]] = None,
         instantiate: bool = True,
         required: bool = False,
-        metavar: str = '{"class_path":...[,"init_args":...]}',
-        help: str = 'Dictionary with "class_path" and "init_args" for any subclass of %(baseclass_name)s.',
+        metavar: str = 'CONFIG | CLASS_NAME_OR_PATH | .ARG_NAME VALUE',
+        help: str = 'One or more arguments specifying "class_path" and "init_args" for any subclass of %(baseclass_name)s.',
         **kwargs
     ):
         """Adds arguments to allow specifying any subclass of the given base class.
 
         This adds an argument that requires a dictionary with a "class_path"
         entry which must be a import dot notation expression. Optionally any
         init arguments for the class can be given in the "init_args" entry.
@@ -499,15 +499,15 @@
             instantiate=False,
         )
 
         added_args: List[str] = []
         if skip is None:
             skip = set()
         else:
-            skip = set(nested_key+'.init_args.'+s for s in skip)
+            skip = {nested_key+'.init_args.'+s for s in skip}
         param = Namespace(name=nested_key, _kind=None, annotation=Union[baseclass])
         str_baseclass = '{' + ', '.join(get_import_path(x) for x in baseclass) + '}'
         kwargs.update({
             'metavar': metavar,
             'help': (help % {'baseclass_name': str_baseclass}),
         })
         if 'default' not in kwargs:
@@ -526,20 +526,20 @@
         )
 
 
     def _gather_docstrings(self, objects, docs_func):
         doc_group = None
         doc_params = {}
         if docstring_parser_support:
-            docstring_parse, DocstringParseError = import_docstring_parse('_gather_docstrings', True)
+            docstring_parse, docstring_error = import_docstring_parse('_gather_docstrings', True)
             for base in objects:
                 for doc in docs_func(base):
                     try:
                         docstring = docstring_parse(doc)
-                    except (ValueError, DocstringParseError) as ex:
+                    except (ValueError, docstring_error) as ex:
                         self.logger.debug(f'Failed parsing docstring for {base}: {ex}')
                     else:
                         if docstring.short_description and not doc_group:
                             doc_group = docstring.short_description
                         for param in docstring.params:
                             if param.arg_name not in doc_params:
                                 doc_params[param.arg_name] = param.description
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/typehints.py` & `jsonargparse-4.9.0/jsonargparse/typehints.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     get_import_path,
     import_object,
     object_path_serializer,
     ParserError,
     Path,
     NoneType,
     indent_text,
-    _issubclass,
+    is_subclass,
     _parse_value_or_config,
     warning,
     lenient_check,
 )
 
 
 __all__ = ['lazy_instance']
@@ -162,15 +162,15 @@
     @staticmethod
     def is_supported_typehint(typehint, full=False):
         """Whether the given type hint is supported."""
         supported = \
             typehint in root_types or \
             get_typehint_origin(typehint) in root_types or \
             typehint in registered_types or \
-            _issubclass(typehint, Enum) or \
+            is_subclass(typehint, Enum) or \
             ActionTypeHint.is_subclass_typehint(typehint)
         if full and supported:
             typehint_origin = get_typehint_origin(typehint) or typehint
             if typehint not in root_types and typehint_origin in root_types and typehint_origin != Literal:
                 for typehint in getattr(typehint, '__args__', []):
                     if not (
                         typehint == Ellipsis or
@@ -192,15 +192,15 @@
             subtypes = [a for a in typehint.__args__ if a != NoneType]
             test = all if all_subtypes else any
             return test(ActionTypeHint.is_subclass_typehint(s) for s in subtypes)
         return inspect.isclass(typehint) and \
             typehint not in leaf_or_root_types and \
             typehint not in registered_types and \
             typehint_origin is None and \
-            not _issubclass(typehint, (Path, Enum))
+            not is_subclass(typehint, (Path, Enum))
 
 
     @staticmethod
     def is_mapping_typehint(typehint):
         typehint_origin = get_typehint_origin(typehint) or typehint
         if typehint in mapping_origin_types or typehint_origin in mapping_origin_types or is_optional(typehint, tuple(mapping_origin_types)):
             return True
@@ -417,15 +417,15 @@
 
     def completer(self, prefix, **kwargs):
         """Used by argcomplete, validates value and shows expected type."""
         if self._typehint == bool:
             return ['true', 'false']
         elif is_optional(self._typehint, bool):
             return ['true', 'false', 'null']
-        elif _issubclass(self._typehint, Enum):
+        elif is_subclass(self._typehint, Enum):
             enum = self._typehint
             return list(enum.__members__.keys())
         elif is_optional(self._typehint, Enum):
             enum = self._typehint.__args__[0]
             return list(enum.__members__.keys())+['null']
         elif is_optional(self._typehint, Path):
             return ['null'] + sorted(files_completer(prefix, **kwargs))
@@ -452,15 +452,15 @@
     }
     subtypehints = get_typehint_subtypes(typehint, append=append)
     typehint_origin = get_typehint_origin(typehint) or typehint
 
     # Any
     if typehint == Any:
         type_val = type(val)
-        if type_val in registered_types or _issubclass(type_val, Enum):
+        if type_val in registered_types or is_subclass(type_val, Enum):
             val = adapt_typehints(val, type_val, **adapt_kwargs)
         elif isinstance(val, str):
             try:
                 val, _ = _parse_value_or_config(val, enable_path=False)
             except get_loader_exceptions():
                 pass
 
@@ -485,15 +485,15 @@
                 val = registered_type.serializer(val)
             else:
                 registered_type.deserializer(val)
         elif not serialize and not registered_type.is_value_of_type(val):
             val = registered_type.deserializer(val)
 
     # Enum
-    elif _issubclass(typehint, Enum):
+    elif is_subclass(typehint, Enum):
         if serialize:
             if isinstance(val, typehint):
                 val = val.name
             else:
                 if val not in typehint.__members__:
                     raise ValueError(f'Value "{val}" is not a valid member name for the enum "{typehint}"')
         elif not serialize and not isinstance(val, typehint):
@@ -503,15 +503,15 @@
     elif typehint in {Type, type} or typehint_origin in {Type, type}:
         if serialize:
             val = object_path_serializer(val)
         elif not serialize and not isinstance(val, type):
             path = val
             val = import_object(val)
             if (typehint in {Type, type} and not isinstance(val, type)) or \
-               (typehint not in {Type, type} and not _issubclass(val, subtypehints[0])):
+               (typehint not in {Type, type} and not is_subclass(val, subtypehints[0])):
                 raise ValueError(f'Value "{path}" is not a {typehint}.')
 
     # Union
     elif typehint_origin == Union:
         vals = []
         for subtypehint in subtypehints:
             try:
@@ -540,23 +540,24 @@
             if is_tuple and len(val) == 0:
                 raise ValueError('Expected a non-empty tuple')
         if not serialize:
             val = tuple(val) if typehint_origin in {Tuple, tuple} else set(val)
 
     # List, Iterable or Sequence
     elif typehint_origin in sequence_origin_types:
-        if append and prev_val is not None:
-            if not isinstance(prev_val, list):
+        if append:
+            if prev_val is None:
+                prev_val = []
+            elif not isinstance(prev_val, list):
                 try:
                     prev_val = [adapt_typehints(prev_val, subtypehints[0], **adapt_kwargs)]
                 except Exception:
-                    pass
-            if isinstance(prev_val, list):
-                val = prev_val + (val if isinstance(val, list) else [val])
-                prev_val = prev_val + [None] * (len(val) if isinstance(val, list) else 1)
+                    prev_val = []
+            val = prev_val + (val if isinstance(val, list) else [val])
+            prev_val = prev_val + [None] * (len(val) if isinstance(val, list) else 1)
         if not isinstance(val, list):
             raise ValueError(f'Expected a List but got "{val}"')
         if subtypehints is not None:
             for n, v in enumerate(val):
                 adapt_kwargs_n = {**adapt_kwargs, 'prev_val': prev_val[n]} if isinstance(prev_val, list) else adapt_kwargs
                 val[n] = adapt_typehints(v, subtypehints[0], **adapt_kwargs_n)
 
@@ -628,15 +629,15 @@
             raise ValueError(f'Type {typehint} expects an str or a Dict/Namespace with a class_path entry but got "{val}"')
         try:
             if isinstance(val, str):
                 val = Namespace(class_path=val)
             elif isinstance(val, dict):
                 val = Namespace(val)
             val_class = import_object(resolve_class_path_by_name(typehint, val['class_path']))
-            if not _issubclass(val_class, typehint):
+            if not is_subclass(val_class, typehint):
                 raise ValueError(f'"{val["class_path"]}" is not a subclass of {typehint}')
             val['class_path'] = class_path = get_import_path(val_class)
             if isinstance(prev_val, Namespace) and 'class_path' in prev_val and 'init_args' not in val:
                 prev_class_path = prev_val['class_path']
                 prev_init_args = prev_val.get('init_args')
                 if prev_class_path != class_path and not (prev_init_args is None or is_empty_namespace(prev_init_args)):
                     warnings.warn(
@@ -787,21 +788,21 @@
 
 
 def is_optional(annotation, ref_type):
     """Checks whether a type annotation is an optional for one type class."""
     return get_typehint_origin(annotation) == Union and \
         len(annotation.__args__) == 2 and \
         any(NoneType == a for a in annotation.__args__) and \
-        any(_issubclass(a, ref_type) for a in annotation.__args__)
+        any(is_subclass(a, ref_type) for a in annotation.__args__)
 
 
 def is_enum_type(annotation):
-    return _issubclass(annotation, Enum) or \
+    return is_subclass(annotation, Enum) or \
         (get_typehint_origin(annotation) == Union and
-         any(_issubclass(a, Enum) for a in annotation.__args__))
+         any(is_subclass(a, Enum) for a in annotation.__args__))
 
 
 def is_callable_type(annotation):
     def is_callable(a):
         return (get_typehint_origin(a) or a) in callable_origin_types or a in callable_origin_types
     return is_callable(annotation) or \
         (get_typehint_origin(annotation) == Union and
@@ -811,33 +812,43 @@
 def typehint_from_action(action_or_typehint):
     if isinstance(action_or_typehint, Action):
         action_or_typehint = getattr(action_or_typehint, '_typehint', None)
     return action_or_typehint
 
 
 def type_to_str(obj):
-    if _issubclass(obj, (bool, int, float, str, Enum)):
+    if obj in {bool, tuple} or is_subclass(obj, (int, float, str, Enum)):
         return obj.__name__
     elif obj is not None:
-        return re.sub(r'[a-z_.]+\.', '', str(obj)).replace('NoneType', 'null')
+        return re.sub(r'[A-Za-z0-9_<>.]+\.', '', str(obj)).replace('NoneType', 'null')
+
+
+def literal_to_str(val):
+    return 'null' if val is None else str(val)
 
 
 def typehint_metavar(typehint):
     """Generates a metavar for some types."""
     metavar = None
+    typehint_origin = get_typehint_origin(typehint) or typehint
     if typehint == bool:
         metavar = '{true,false}'
     elif is_optional(typehint, bool):
         metavar = '{true,false,null}'
-    elif _issubclass(typehint, Enum):
+    elif typehint_origin == Literal:
+        args = typehint.__args__
+        metavar = literal_to_str(args[0]) if len(args) == 1 else '{'+','.join(literal_to_str(a) for a in args)+'}'
+    elif is_subclass(typehint, Enum):
         enum = typehint
         metavar = '{'+','.join(list(enum.__members__.keys()))+'}'
     elif is_optional(typehint, Enum):
         enum = typehint.__args__[0]
         metavar = '{'+','.join(list(enum.__members__.keys())+['null'])+'}'
+    elif typehint_origin in tuple_set_origin_types:
+        metavar = '[ITEM,...]'
     return metavar
 
 
 def serialize_class_instance(val):
     type_val = type(val)
     val = str(val)
     warning(f"""
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/typing.py` & `jsonargparse-4.9.0/jsonargparse/typing.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse/util.py` & `jsonargparse-4.9.0/jsonargparse/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     sys.stderr.write('%(prog)s: error: %(message)s\n' % args)
     if 'JSONARGPARSE_DEBUG' in os.environ:
         raise DebugException('jsonargparse debug enabled, thus raising exception instead of exit.')
     else:
         parser.exit(2)
 
 
-def _issubclass(cls, class_or_tuple):
+def is_subclass(cls, class_or_tuple):
     """Extension of issubclass that supports non-class argument."""
     return inspect.isclass(cls) and issubclass(cls, class_or_tuple)
 
 
 def import_object(name: str):
     """Returns an object in a module given its dot import path."""
     if not isinstance(name, str) or '.' not in name:
@@ -479,18 +479,19 @@
         if 's' in mode and 'd' in mode:
             raise ValueError('Both modes "d" and "s" not possible.')
 
 
 class LoggerProperty:
     """Class designed to be inherited by other classes to add a logger property."""
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         """Initializer for LoggerProperty class."""
         if not hasattr(self, '_logger'):
             self.logger = None
+        super().__init__(*args, **kwargs)
 
 
     @property
     def logger(self):
         """The logger property for the class.
 
         :getter: Returns the current logger.
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse.egg-info/PKG-INFO` & `jsonargparse-4.9.0/jsonargparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonargparse
-Version: 4.8.0.dev2
+Version: 4.9.0
 Summary: Parsing of command line options, yaml/jsonnet config files and/or environment variables based on argparse.
 Home-page: https://github.com/omni-us/jsonargparse
 Author: Mauricio Villegas
 Author-email: mauricio@omnius.com
 License: MIT
 Project-URL: Documentation-stable, https://jsonargparse.readthedocs.io/en/stable/
 Project-URL: Documentation-latest, https://jsonargparse.readthedocs.io/en/latest/
@@ -42,14 +42,15 @@
 Provides-Extra: omegaconf
 Provides-Extra: typing_extensions
 Provides-Extra: reconplogger
 Provides-Extra: test
 Provides-Extra: test_no_urls
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: maintainer
 License-File: LICENSE.rst
 
 .. image:: https://readthedocs.org/projects/jsonargparse/badge/?version=stable
     :target: https://jsonargparse.readthedocs.io/en/stable/
 .. image:: https://github.com/omni-us/jsonargparse/actions/workflows/ci_test.yml/badge.svg
     :target: https://github.com/omni-us/jsonargparse/actions/workflows/ci_test.yml
 .. image:: https://codecov.io/gh/omni-us/jsonargparse/branch/master/graph/badge.svg
@@ -256,21 +257,36 @@
 functions are not automatically printed. `.CLI` returns its value and it
 is up to the developer to decide what to do with it. Finally, jsonargparse has
 many features designed to help in creating convenient argument parsers such as:
 `nested-namespaces`, `configuration-files`, additional type hints
 (`parsing-paths`, `restricted-numbers`, `restricted-strings`) and
 much more.
 
-The next section explains how to create an argument parser in a low level
+Section `parsers` explains how to create an argument parser in a low level
 argparse-style. However, as parsers get more complex, being able to define them
 in a modular way becomes important. Three mechanisms are available for
 modularity, see respective sections `classes-methods-functions`,
 `sub-commands` and `parser-arguments`.
 
 
+.. _tutorials:
+
+Tutorials
+=========
+
+- `"jsonargparse - Say goodbye to configuration hassles"
+  <https://2022.pycon.de/program/XK73C3/>`__  by Marianne Stecklina at PyCon DE
+  & PyData Berlin 2022
+
+    - Presentation video: https://youtu.be/2gDf2S0nHKg
+    - GitHub repository: https://github.com/stecklin/pycon22-jsonargparse
+
+
+.. _parsers:
+
 Parsers
 =======
 
 An argument parser is created just like it is done with python's `argparse
 <https://docs.python.org/3/library/argparse.html>`__. You import the module,
 create a parser object and then add arguments to it. A simple example would be:
 
@@ -840,18 +856,18 @@
 - ``Tuple``, ``Set`` and ``MutableSet`` are supported even though they can't be
   represented in json distinguishable from a list. Each ``Tuple`` element
   position can have its own type and will be validated as such. ``Tuple`` with
   ellipsis (``Tuple[type, ...]``) is also supported. In command line arguments,
   config files and environment variables, tuples and sets are represented as an
   array.
 
-- ``dataclasses`` are supported as a type but without any nesting and for pure
-  data classes. By pure it is meant that it only inherits from data classes. Not
-  a mixture of normal classes and data classes. Data classes as fields of other
-  data classes is supported.
+- ``dataclasses`` are supported as a type but only for pure data classes and not
+  nested in a type. By pure it is meant that the class only inherits from data
+  classes. Not a mixture of normal classes and data classes. Data classes as
+  fields of other data classes is supported.
 
 - To set a value to ``None`` it is required to use ``null`` since this is how
   json/yaml defines it. To avoid confusion in the help, ``NoneType`` is
   displayed as ``null``. For example a function argument with type and default
   ``Optional[str] = None`` would be shown in the help as ``type: Union[str,
   null], default: null``.
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse.egg-info/SOURCES.txt` & `jsonargparse-4.9.0/jsonargparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse.egg-info/requires.txt` & `jsonargparse-4.9.0/jsonargparse.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,18 +28,23 @@
 
 [dataclasses:python_version == "3.6"]
 dataclasses>=0.8
 
 [dev]
 coverage>=4.5.1
 responses>=0.12.0
+Sphinx>=1.7.9
+sphinx-rtd-theme>=0.4.3
+autodocsumm>=0.1.10
+sphinx-autodoc-typehints>=1.11.1
+pre-commit>=2.19.0
 pylint>=1.8.3
 pycodestyle>=2.5.0
 mypy>=0.701
-bump2version>=0.5.11
+tox>=3.25.0
 
 [doc]
 Sphinx>=1.7.9
 sphinx-rtd-theme>=0.4.3
 autodocsumm>=0.1.10
 sphinx-autodoc-typehints>=1.11.1
 
@@ -48,14 +53,18 @@
 
 [jsonnet]
 jsonnet>=0.13.0
 
 [jsonschema]
 jsonschema>=3.2.0
 
+[maintainer]
+bump2version>=0.5.11
+twine>=4.0.0
+
 [omegaconf]
 omegaconf>=2.1.1
 
 [reconplogger]
 reconplogger>=4.4.0
 
 [ruyaml]
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/__main__.py` & `jsonargparse-4.9.0/jsonargparse_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/actions_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/actions_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/argcomplete_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/argcomplete_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/base.py` & `jsonargparse-4.9.0/jsonargparse_tests/base.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/cli_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/cli_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/core_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/core_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,18 @@
         cfg = parser.parse_env({'APP_REQ1': 'val5', 'APP_LEV1__REQ2': 'val6'})
         self.assertEqual('val5', cfg.req1)
         self.assertEqual('val6', cfg.lev1.req2)
         self.assertRaises(ParserError, lambda: parser.parse_args(['--req1', 'val1']))
         self.assertRaises(ParserError, lambda: parser.parse_string('{"lev1":{"req2":"val4"}}'))
         self.assertRaises(ParserError, lambda: parser.parse_env({}))
 
+        out = StringIO()
+        parser.print_help(out)
+        self.assertIn('[-h] --req1 REQ1 --lev1.req2 REQ2', out.getvalue())
+
         parser = ArgumentParser(default_env=True)
         parser.add_argument('--req1', required=True)
         parser.add_argument('--cfg', action=ActionConfigFile)
         cfg = parser.parse_args(['--cfg', '{"req1": "val1"}'])
         self.assertEqual('val1', cfg.req1)
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/deprecated_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/deprecated_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/formatters_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/formatters_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/jsonnet_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/jsonnet_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/jsonschema_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/jsonschema_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/loaders_dumpers_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/loaders_dumpers_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/namespace_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/namespace_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         ns['d.b'] = 2
         self.assertEqual(2, ns['d']['b'])
 
     def test_contains_non_str_key(self):
         ns = Namespace()
         for key in [None, True, False, 1, 2.3]:
             with self.subTest(str(key)):
-                self.assertFalse(key in ns)
+                self.assertNotIn(key, ns)
 
     def test_pop(self):
         ns = Namespace()
         ns['x.y.z'] = 1
         self.assertEqual(1, ns.pop('x.y.z'))
         self.assertEqual(ns, Namespace(x=Namespace(y=Namespace())))
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/optionals_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/optionals_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/signatures_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/signatures_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,14 +467,17 @@
 
 
     def test_required_group(self):
         parser = ArgumentParser(error_handler=None)
         self.assertRaises(ValueError, lambda: parser.add_subclass_arguments(calendar.Calendar, None, required=True))
         parser.add_subclass_arguments(calendar.Calendar, 'cal', required=True)
         self.assertRaises(ParserError, lambda: parser.parse_args([]))
+        out = StringIO()
+        parser.print_help(out)
+        self.assertIn('[-h] [--cal.help CLASS_NAME_OR_PATH] --cal ', out.getvalue())
 
 
     def test_not_required_group(self):
         parser = ArgumentParser(error_handler=None)
         parser.add_subclass_arguments(calendar.Calendar, 'cal', required=False)
         cfg = parser.parse_args([])
         self.assertEqual(cfg, Namespace())
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/typehints_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/typehints_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import sys
 import unittest
 import uuid
 import warnings
 import yaml
 from calendar import Calendar
 from contextlib import redirect_stderr, redirect_stdout
+from copy import deepcopy
 from datetime import datetime
 from enum import Enum
 from gzip import GzipFile
 from io import StringIO
 from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Type, Union
 from jsonargparse import ActionConfigFile, ArgumentParser, CLI, lazy_instance, Namespace, ParserError, Path
 from jsonargparse.typehints import ActionTypeHint, is_optional, Literal
@@ -185,14 +186,27 @@
         self.assertEqual((2, 'a', 'b'), cfg.tuple)
         self.assertIsInstance(cfg.tuple[1], Path)
         self.assertRaises(ParserError, lambda: parser.parse_args(['--tuple=[]']))
         self.assertRaises(ParserError, lambda: parser.parse_args(['--tuple=[2, "a", "b", 5]']))
         self.assertRaises(ParserError, lambda: parser.parse_args(['--tuple=[2, "a"]']))
         self.assertRaises(ParserError, lambda: parser.parse_args(['--tuple=["2", "a", "b"]']))
         self.assertRaises(ParserError, lambda: parser.parse_args(['--tuple={"a":1, "b":"2"}']))
+        out = StringIO()
+        parser.print_help(out)
+        self.assertIn('--tuple [ITEM,...]  (type: Tuple[Union[int, MyEnum], Path_fc, NotEmptyStr], default: null)', out.getvalue())
+
+
+    def test_tuple_untyped(self):
+        parser = ArgumentParser(error_handler=None)
+        parser.add_argument('--tuple', type=tuple)
+        cfg = parser.parse_args(['--tuple=[1, "a", True]'])
+        self.assertEqual((1, 'a', True), cfg.tuple)
+        out = StringIO()
+        parser.print_help(out)
+        self.assertIn('--tuple [ITEM,...]  (type: tuple, default: null)', out.getvalue())
 
 
     def test_nested_tuples(self):
         parser = ArgumentParser(error_handler=None)
         parser.add_argument('--tuple', type=Tuple[Tuple[str, str], Tuple[Tuple[int, float], Tuple[int, float]]])
         cfg = parser.parse_args(['--tuple=[["foo", "bar"], [[1, 2.02], [3, 3.09]]]'])
         self.assertEqual((('foo', 'bar'), ((1, 2.02), (3, 3.09))), cfg.tuple)
@@ -226,18 +240,19 @@
         self.assertEqual(cfg.complex, 2+3j)
         self.assertEqual(parser.dump(cfg), 'complex: (2+3j)\n')
 
 
     def test_list_append(self):
         parser = ArgumentParser(error_handler=None)
         parser.add_argument('--val', type=Union[int, str, List[int]])
-        self.assertEqual(0, parser.parse_args(['--val+=0']).val)
-        self.assertEqual([1, 2, 3], parser.parse_args(['--val+=1', '--val+=2', '--val+=3']).val)
+        self.assertEqual(0, parser.parse_args(['--val=0']).val)
+        self.assertEqual([0], parser.parse_args(['--val+=0']).val)
+        self.assertEqual([1, 2, 3], parser.parse_args(['--val=1', '--val+=2', '--val+=3']).val)
         self.assertEqual([1, 2, 3], parser.parse_args(['--val=[1,2]', '--val+=3']).val)
-        self.assertEqual(1, parser.parse_args(['--val=a', '--val+=1']).val)
+        self.assertEqual([1], parser.parse_args(['--val=a', '--val+=1']).val)
         with warnings.catch_warnings(record=True) as w:
             self.assertEqual(3, parser.parse_args(['--val=[1,2]', '--val=3']).val)
             self.assertIn('Replacing list value "[1, 2]" with "3"', str(w[0].message))
 
 
     def test_list_append_config(self):
         parser = ArgumentParser(error_handler=None)
@@ -302,24 +317,32 @@
         self.assertEqual(' xyz ', parser.parse_args(['--any= xyz '])['any'])
         self.assertEqual('[[[', parser.parse_args(['--any=[[['])['any'])
 
 
     @unittest.skipIf(not Literal, 'Literal introduced in python 3.8 or backported in typing_extensions')
     def test_Literal(self):
         parser = ArgumentParser(error_handler=None)
-        parser.add_argument('--str', type=Literal['a', 'b'])
+        parser.add_argument('--str', type=Literal['a', 'b', None])
+        parser.add_argument('--int', type=Literal[3, 4])
         parser.add_argument('--true', type=Literal[True])
         parser.add_argument('--false', type=Literal[False])
         self.assertEqual('a', parser.parse_args(['--str=a']).str)
         self.assertEqual('b', parser.parse_args(['--str=b']).str)
         self.assertRaises(ParserError, lambda: parser.parse_args(['--str=x']))
+        self.assertIsNone(parser.parse_args(['--str=null']).str)
+        self.assertEqual(4, parser.parse_args(['--int=4']).int)
+        self.assertRaises(ParserError, lambda: parser.parse_args(['--int=5']))
         self.assertIs(True, parser.parse_args(['--true=true']).true)
         self.assertRaises(ParserError, lambda: parser.parse_args(['--true=false']))
         self.assertIs(False, parser.parse_args(['--false=false']).false)
         self.assertRaises(ParserError, lambda: parser.parse_args(['--false=true']))
+        out = StringIO()
+        parser.print_help(out)
+        for value in ['--str {a,b,null}', '--int {3,4}', '--true True', '--false False']:
+            self.assertIn(value, out.getvalue())
 
 
     def test_nested_mapping_without_args(self):
         parser = ArgumentParser()
         parser.add_argument('--map', type=Mapping[str, Union[int, Mapping]])
         self.assertEqual(parser.parse_args(['--map={"a": 1}']).map, {"a": 1})
         self.assertEqual(parser.parse_args(['--map={"b": {"c": 2}}']).map, {"b": {"c": 2}})
@@ -555,14 +578,45 @@
         parser = ArgumentParser()
         parser.add_argument('--op', type=Calendar)
         cfg = parser.parse_args(['--op=TextCalendar', '--op.firstweekday=2'])
         self.assertEqual(cfg.op.class_path, 'calendar.TextCalendar')
         self.assertEqual(cfg.op.init_args, Namespace(firstweekday=2))
 
 
+    def test_class_type_config_merge_init_args(self):
+        class MyCal(Calendar):
+            def __init__(self, param_a: int = 1, param_b: str = 'x', **kwargs):
+                super().__init__(**kwargs)
+
+        parser = ArgumentParser(error_handler=None)
+        parser.add_argument('--cfg', action=ActionConfigFile)
+        parser.add_argument('--cal', type=Calendar)
+
+        with mock_module(MyCal) as module:
+            config1 = {
+                'cal': {
+                    'class_path': f'{module}.MyCal',
+                    'init_args': {
+                        'firstweekday': 2,
+                        'param_b': 'y',
+                    }
+                }
+            }
+            config2 = deepcopy(config1)
+            config2['cal']['init_args'] = {
+                'param_a': 2,
+                'firstweekday': 3,
+            }
+            expected = deepcopy(config1['cal'])
+            expected['init_args'].update(config2['cal']['init_args'])
+
+            cfg = parser.parse_args([f'--cfg={yaml.safe_dump(config1)}', f'--cfg={yaml.safe_dump(config2)}'])
+            self.assertEqual(cfg.cal.as_dict(), expected)
+
+
     def test_class_type_subclass_nested_init_args(self):
         class Class:
             def __init__(self, cal: Calendar, p1: int = 0):
                 self.cal = cal
 
         for full in ['init_args.', '']:
             with self.subTest('full' if full else 'short'), mock_module(Class) as module:
```

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/typing_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/typing_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/jsonargparse_tests/util_tests.py` & `jsonargparse-4.9.0/jsonargparse_tests/util_tests.py`

 * *Files identical despite different names*

### Comparing `jsonargparse-4.8.0.dev2/setup.cfg` & `jsonargparse-4.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -45,31 +45,36 @@
 test = 
 	%(test_no_urls)s
 	responses>=0.12.0
 test_no_urls = 
 	coverage>=4.5.1
 dev = 
 	%(test)s
+	%(doc)s
+	pre-commit>=2.19.0
 	pylint>=1.8.3
 	pycodestyle>=2.5.0
 	mypy>=0.701
-	bump2version>=0.5.11
+	tox>=3.25.0
 doc = 
 	Sphinx>=1.7.9
 	sphinx-rtd-theme>=0.4.3
 	autodocsumm>=0.1.10
 	sphinx-autodoc-typehints>=1.11.1
+maintainer = 
+	bump2version>=0.5.11
+	twine>=4.0.0
 
 [options.package_data]
 jsonargparse = 
 	*.pyi
 
 [metadata]
 name = jsonargparse
-version = 4.8.0.dev2
+version = 4.9.0
 description = Parsing of command line options, yaml/jsonnet config files and/or environment variables based on argparse.
 long_description_content_type = text/x-rst
 author = Mauricio Villegas
 author_email = mauricio@omnius.com
 license = MIT
 url = https://github.com/omni-us/jsonargparse
 project_urls = 
@@ -110,15 +115,15 @@
 
 [mypy]
 ignore_missing_imports = true
 allow_redefinition = true
 warn_unused_ignores = true
 
 [tox:tox]
-envlist = py{36,37,38,39,310},pypy3
+envlist = py{36,37,38,39,310},pypy3,no-extras
 
 [testenv]
 extras = 
 	test
 	signatures
 	dataclasses
 	jsonschema
@@ -128,11 +133,14 @@
 	ruyaml
 	omegaconf
 changedir = jsonargparse_tests
 commands = discover --pattern='*_tests.py'
 deps = discover
 passenv = JSONARGPARSE_*
 
+[testenv:no-extras]
+extras = test_no_urls
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jsonargparse-4.8.0.dev2/setup.py` & `jsonargparse-4.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 
 
 ## build_sphinx target ##
 try:
     from sphinx.setup_command import BuildDoc
     CMDCLASS['build_sphinx'] = BuildDoc  # type: ignore
 except ImportError:
-    print('warning: sphinx package not found, build_sphinx target will not be available.')
+    pass
 
 
 ## Run setuptools setup ##
 setup(long_description=LONG_DESCRIPTION, cmdclass=CMDCLASS)
```

