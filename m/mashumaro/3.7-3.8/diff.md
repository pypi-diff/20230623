# Comparing `tmp/mashumaro-3.7.tar.gz` & `tmp/mashumaro-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mashumaro-3.7.tar", last modified: Thu Apr 13 17:38:55 2023, max compression
+gzip compressed data, was "mashumaro-3.8.tar", last modified: Thu Jun 22 18:41:44 2023, max compression
```

## Comparing `mashumaro-3.7.tar` & `mashumaro-3.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.211377 mashumaro-3.7/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-13 17:38:38.000000 mashumaro-3.7/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78949 2023-04-13 17:38:55.211162 mashumaro-3.7/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78030 2023-04-13 17:38:38.000000 mashumaro-3.7/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.205196 mashumaro-3.7/mashumaro/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      258 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1452 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/config.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.206520 mashumaro-3.7/mashumaro/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1013 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      825 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/core/helpers.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.207249 mashumaro-3.7/mashumaro/core/meta/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.208148 mashumaro-3.7/mashumaro/core/meta/code/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/code/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    37703 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/core/meta/code/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      707 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/code/lines.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    20883 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/helpers.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1366 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/mixin.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.208781 mashumaro-3.7/mashumaro/core/meta/types/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/core/meta/types/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4109 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/common.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25319 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/pack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    32058 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/core/meta/types/unpack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      469 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/dialect.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4548 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/exceptions.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1472 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/helper.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.209840 mashumaro-3.7/mashumaro/jsonschema/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      214 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2170 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/annotations.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2837 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      746 2023-04-07 09:26:24.000000 mashumaro-3.7/mashumaro/jsonschema/dialects.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5818 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    25682 2023-04-13 17:38:38.000000 mashumaro-3.7/mashumaro/jsonschema/schema.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.210887 mashumaro-3.7/mashumaro/mixins/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1673 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/dict.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      790 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/json.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1558 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/msgpack.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1731 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/orjson.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1000 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/orjson.pyi
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1392 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/toml.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1108 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/mixins/yaml.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-02-06 08:24:36.000000 mashumaro-3.7/mashumaro/py.typed
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2249 2023-02-13 10:27:04.000000 mashumaro-3.7/mashumaro/types.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 17:38:55.206105 mashumaro-3.7/mashumaro.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    78949 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1210 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-02-06 08:27:56.000000 mashumaro-3.7/mashumaro.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      155 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-13 17:38:55.000000 mashumaro-3.7/mashumaro.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      689 2023-04-07 09:26:24.000000 mashumaro-3.7/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-13 17:38:55.211416 mashumaro-3.7/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1463 2023-04-13 17:38:38.000000 mashumaro-3.7/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.345355 mashumaro-3.8/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-06-22 18:41:04.000000 mashumaro-3.8/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    97542 2023-06-22 18:41:44.345219 mashumaro-3.8/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    96623 2023-06-22 18:41:04.000000 mashumaro-3.8/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.341240 mashumaro-3.8/mashumaro/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      258 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1674 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/config.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.342269 mashumaro-3.8/mashumaro/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1013 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      825 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/helpers.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.342585 mashumaro-3.8/mashumaro/core/meta/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.342903 mashumaro-3.8/mashumaro/core/meta/code/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/code/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    41929 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/code/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      815 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/code/lines.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    22129 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/helpers.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1366 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/mixin.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.343354 mashumaro-3.8/mashumaro/core/meta/types/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/types/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4882 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/types/common.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    25094 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/types/pack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    42599 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/core/meta/types/unpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      469 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/dialect.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5491 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/exceptions.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1472 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/helper.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.344184 mashumaro-3.8/mashumaro/jsonschema/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      214 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2151 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/annotations.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2837 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      746 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/dialects.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5946 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    25698 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/jsonschema/schema.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.344984 mashumaro-3.8/mashumaro/mixins/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1867 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/dict.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      790 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/json.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1558 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/msgpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1731 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/orjson.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1000 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1392 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/toml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1108 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/mixins/yaml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/py.typed
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2715 2023-06-22 18:41:04.000000 mashumaro-3.8/mashumaro/types.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:44.341990 mashumaro-3.8/mashumaro.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    97542 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1210 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      155 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-06-22 18:41:44.000000 mashumaro-3.8/mashumaro.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      689 2023-06-22 18:41:04.000000 mashumaro-3.8/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-06-22 18:41:44.345389 mashumaro-3.8/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1463 2023-06-22 18:41:04.000000 mashumaro-3.8/setup.py
```

### Comparing `mashumaro-3.7/LICENSE` & `mashumaro-3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/PKG-INFO` & `mashumaro-3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.7
+Version: 3.8
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,23 +20,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: orjson
 Provides-Extra: msgpack
 Provides-Extra: yaml
 Provides-Extra: toml
 License-File: LICENSE
 
-# mashumaro
+<div align="center">
+
+<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+</div>
 
 When using dataclasses, you often need to dump and load objects based on the
 schema you have. Mashumaro not only lets you save and load things in different
 ways, but it also does it _super quick_.
 
 **Key features**
 * 🚀 One of the fastest libraries
@@ -82,23 +85,32 @@
         * [`aliases` config option](#aliases-config-option)
         * [`serialize_by_alias` config option](#serialize_by_alias-config-option)
         * [`omit_none` config option](#omit_none-config-option)
         * [`namedtuple_as_dict` config option](#namedtuple_as_dict-config-option)
         * [`allow_postponed_evaluation` config option](#allow_postponed_evaluation-config-option)
         * [`dialect` config option](#dialect-config-option)
         * [`orjson_options`](#orjson_options-config-option)
+        * [`discriminator` config option](#discriminator-config-option)
+        * [`lazy_compilation` config option](#lazy_compilation-config-option)
     * [Passing field values as is](#passing-field-values-as-is)
+    * [Extending existing types](#extending-existing-types)
     * [Dialects](#dialects)
       * [`serialization_strategy` dialect option](#serialization_strategy-dialect-option)
       * [`omit_none` dialect option](#omit_none-dialect-option)
       * [Changing the default dialect](#changing-the-default-dialect)
+    * [Discriminator](#discriminator)
+      * [Subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+      * [Subclasses without a common field](#subclasses-without-a-common-field)
+      * [Class level discriminator](#class-level-discriminator)
+      * [Working with union of classes](#working-with-union-of-classes)
     * [Code generation options](#code-generation-options)
         * [Add `omit_none` keyword argument](#add-omit_none-keyword-argument)
         * [Add `by_alias` keyword argument](#add-by_alias-keyword-argument)
         * [Add `dialect` keyword argument](#add-dialect-keyword-argument)
+        * [Add `context` keyword argument](#add-context-keyword-argument)
     * [Generic dataclasses](#generic-dataclasses)
       * [Generic dataclass inheritance](#generic-dataclass-inheritance)
       * [Generic dataclass in a field type](#generic-dataclass-in-a-field-type)
     * [`GenericSerializableType` interface](#genericserializabletype-interface)
     * [Serialization hooks](#serialization-hooks)
         * [Before deserialization](#before-deserialization)
         * [After deserialization](#after-deserialization)
@@ -188,14 +200,15 @@
 * [`Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)
 * [`Union`](https://docs.python.org/3/library/typing.html#typing.Union)
 * [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar)
 * [`TypeVarTuple`](https://docs.python.org/3/library/typing.html#typing.TypeVarTuple)
 * [`NewType`](https://docs.python.org/3/library/typing.html#newtype)
 * [`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
 * [`Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)
+* [`Final`](https://docs.python.org/3/library/typing.html#typing.Final)
 * [`Self`](https://docs.python.org/3/library/typing.html#typing.Self)
 * [`Unpack`](https://docs.python.org/3/library/typing.html#typing.Unpack)
 
 for standard interpreter types from [`types`](https://docs.python.org/3/library/types.html#standard-interpreter-types) module:
 * [`NoneType`](https://docs.python.org/3/library/types.html#types.NoneType)
 * [`UnionType`](https://docs.python.org/3/library/types.html#types.UnionType)
 
@@ -308,27 +321,40 @@
 specific parser and builder for exactly that schema, taking into account the
 specifics of the serialization format. This is much faster than inspection of
 field types on every call of parsing or building at runtime.
 
 These specific parsers and builders are presented by the corresponding
 `from_*` and `to_*` methods. They are compiled during import time (or at
 runtime in some cases) and are set as attributes to your dataclasses.
+To minimize the import time, you can explicitly enable
+[lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
 * macOS 13.0.1 Ventura
 * Apple M1
 * 8GB RAM
 * Python 3.11.0
 
 Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
 The following figures show the best overall time in each case.
 
-<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump.png" width="400">
+[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
+
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
+</picture>
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
+</picture>
 
 <table>
   <col>
   <colgroup span="2"></colgroup>
   <colgroup span="2"></colgroup>
   <tr>
     <th rowspan="2">Library</th>
@@ -339,51 +365,51 @@
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14791</td>
+    <td align="right">0.14724</td>
     <td align="left">1x</td>
-    <td align="right">0.10294</td>
+    <td align="right">0.10128</td>
     <td align="left">1x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18913</td>
+    <td align="right">0.18906</td>
     <td align="left">1.28x</td>
-    <td align="right">0.13879</td>
-    <td align="left">1.35x</td>
+    <td align="right">0.14072</td>
+    <td align="left">1.39x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">0.92652</td>
-    <td align="left">6.26x</td>
-    <td align="right">0.81281</td>
-    <td align="left">7.9x</td>
+    <td align="right">1.02666</td>
+    <td align="left">6.97x</td>
+    <td align="right">0.81932</td>
+    <td align="left">8.09x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38964</td>
-    <td align="left">9.39x</td>
-    <td align="right">0.45987</td>
-    <td align="left">4.47x</td>
+    <td align="right">1.38348</td>
+    <td align="left">9.4x</td>
+    <td align="right">0.45695</td>
+    <td align="left">4.51x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
     <td align="left">—</td>
     <td align="left">—</td>
-    <td align="right">0.68592</td>
-    <td align="left">6.66x</td>
+    <td align="right">0.68057</td>
+    <td align="left">6.72x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.40445</td>
-    <td align="left">16.26x</td>
+    <td align="right">2.37315</td>
+    <td align="left">16.12x</td>
     <td align="left">—</td>
     <td align="left">—</td>
 </tr>
 </table>
 
 To run benchmark in your environment:
 ```bash
@@ -584,15 +610,15 @@
 assert my_flight == Flight(JFK, LAX)
 assert my_flight.to_dict() == input_data
 ```
 
 You can see how `Airport` instances are seamlessly created from lists of two
 strings and serialized into them.
 
-By default `_deserialize` method will get raw input data without any 
+By default `_deserialize` method will get raw input data without any
 transformations before. This should be enough in many cases, especially when
 you need to perform non-standard transformations yourself, but let's extend
 our example:
 
 ```python
 class Itinerary(SerializableType):
     def __init__(self, flights):
@@ -1079,14 +1105,15 @@
 described below.
 
 | Constant                                                        | Description                                                          |
 |:----------------------------------------------------------------|:---------------------------------------------------------------------|
 | [`TO_DICT_ADD_OMIT_NONE_FLAG`](#add-omit_none-keyword-argument) | Adds `omit_none` keyword-only argument to `to_*` methods.            |
 | [`TO_DICT_ADD_BY_ALIAS_FLAG`](#add-by_alias-keyword-argument)   | Adds `by_alias` keyword-only argument to `to_*` methods.             |
 | [`ADD_DIALECT_SUPPORT`](#add-dialect-keyword-argument)          | Adds `dialect` keyword-only argument to `from_*` and `to_*` methods. |
+| [`ADD_SERIALIZATION_CONTEXT`](#add-context-keyword-argument)    | Adds `context` keyword-only argument to `to_*` methods.              |
 
 #### `serialization_strategy` config option
 
 You can register custom [`SerializationStrategy`](#serializationstrategy), `serialize` and `deserialize`
 methods for specific types just in one place. It could be configured using
 a dictionary with types as keys. The value could be either a
 [`SerializationStrategy`](#serializationstrategy) instance or a dictionary with `serialize` and
@@ -1128,14 +1155,18 @@
 
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
+Note that you can register different methods for multiple logical types which
+are based on the same type using `NewType` and `Annotated`.
+See [Extending existing types](#extending-existing-types) for details.
+
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
 ```python
@@ -1335,14 +1366,36 @@
 
     class Config(BaseConfig):
         orjson_options = orjson.OPT_NON_STR_KEYS
 
 assert MyClass({1: 2}).to_json() == {"1": 2}
 ```
 
+#### `discriminator` config option
+
+This option is described in the
+[Class level discriminator](#class-level-discriminator) section.
+
+#### `lazy_compilation` config option
+
+By using this option, the compilation of the `from_*` and `to_*` methods will
+be deferred until they are called first time. This will reduce the import time
+and, in certain instances, may enhance the speed of deserialization
+by leveraging the data that is accessible after the class has been created.
+
+> **Warning**
+>
+> If you need to save a reference to `from_*` or `to_*` method, you should
+> do it after the method is compiled. To be safe, you can always use lambda
+> function:
+> ```python
+> from_dict = lambda x: MyModel.from_dict(x)
+> to_dict = lambda x: x.to_dict()
+> ```
+
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
 [`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
@@ -1404,20 +1457,74 @@
 a2_dict = A2(my_class_instance).to_dict()
 a3_dict = A3(my_class_instance).to_dict()
 a4_dict = A4(my_class_instance).to_dict()
 
 assert a1_dict == a2_dict == a3_dict == a4_dict == {"x": my_class_instance}
 ```
 
+### Extending existing types
+
+There are situations where you might want some values of the same type to be
+treated as their own type. You can create new logical types with
+[`NewType`](https://docs.python.org/3/library/typing.html#newtype) or
+[`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
+and register serialization strategies for them:
+
+```python
+from typing import Mapping, NewType, Annotated
+from dataclasses import dataclass
+from mashumaro import DataClassDictMixin
+
+SessionID = NewType("SessionID", str)
+AccountID = Annotated[str, "AccountID"]
+
+@dataclass
+class Context(DataClassDictMixin):
+    account_sessions: Mapping[AccountID, SessionID]
+
+    class Config:
+        serialization_strategy = {
+            AccountID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            },
+            SessionID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            }
+        }
+```
+
+Although using `NewType` is usually the most reliable way to avoid logical
+errors, you have to pay for it with notable overhead. If you are creating
+dataclass instances manually, then you know that type checkers will
+enforce you to enclose a value in your `"NewType"` callable, which leads
+to performance degradation:
+
+```python
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "MyInt(42)"
+10000000 loops, best of 5: 31.1 nsec per loop
+
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "42"
+50000000 loops, best of 5: 4.35 nsec per loop
+```
+
+However, when you create dataclass instances using the `from_*` method, there
+will be no performance degradation, because the value won't be enclosed in the
+callable in the generated code. Therefore, if performance is more important
+to you than catching logical errors by type checkers, and you are actively
+creating or changing dataclasses manually, then you should take a closer look
+at using `Annotated`.
+
 ### Dialects
 
 Sometimes it's needed to have different serialization and deserialization
 methods depending on the data source where entities of the dataclass are
 stored or on the API to which the entities are being sent or received from.
-There is a special Dialect type that may contain all the differences from the
+There is a special `Dialect` type that may contain all the differences from the
 default serialization and deserialization methods. You can create different
 dialects and use each of them for the same dataclass depending on
 the situation.
 
 Suppose we have the following dataclass with a field of type `date`:
 ```python
 @dataclass
@@ -1501,14 +1608,406 @@
         dialect = JapaneseDialect
 
 entity = Entity(date(2021, 12, 31))
 entity.to_dict()  # {'dt': '2021年12月31日'}
 assert Entity.from_dict({'dt': '2021年12月31日'}) == entity
 ```
 
+### Discriminator
+
+There is a special `Discriminator` class that allows you to customize how
+a union of dataclasses or their hierarchy will be deserialized.
+It has the following parameters that affects class selection rules:
+
+* `field` — optional name of the input dictionary key by which all the variants
+  can be distinguished
+* `include_subtypes` — allow to deserialize subclasses
+* `include_supertypes` — allow to deserialize superclasses
+
+Parameter `field` coule be in the following forms:
+
+* without annotations: `type = 42`
+* annotated as ClassVar: `type: ClassVar[int] = 42`
+* annotated as Final: `type: Final[int] = 42`
+* annotated as Literal: `type: Literal[42] = 42`
+* annotated as StrEnum: `type: ResponseType = ResponseType.OK`
+
+> **Note**
+>
+> Keep in mind that by default only Final, Literal and StrEnum fields are
+> processed during serialization.
+
+Next, we will look at different use cases, as well as their pros and cons.
+
+#### Subclasses distinguishable by a field
+
+Often you have a base dataclass and multiple subclasses that are easily
+distinguishable from each other by the value of a particular field.
+For example, there may be different events, messages or requests with
+a discriminator field "event_type", "message_type" or just "type". You could've
+listed all of them within `Union` type, but it would be too verbose and
+impractical. Moreover, deserialization of the union would be slow, since we
+need to iterate over each variant in the list until we find the right one.
+
+We can improve subclass deserialization using `Discriminator` as annotation
+within `Annotated` type. We will use `field` parameter and set
+`include_subtypes` to `True`.
+
+> **Note**
+>
+> The discriminator field should be accessible from the `__dict__` attribute
+> of a specific descendant, i.e. defined at the level of that descendant.
+> A descendant class without a discriminator field will be ignored, but
+> its descendants won't.
+
+Suppose we have a hierarchy of client events distinguishable by a class
+attribute "type":
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from mashumaro import DataClassDictMixin
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    pass
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+```
+
+We use base dataclass `ClientEvent` for a field of another dataclass:
+
+```python
+from typing import Annotated, List
+# or from typing_extensions import Annotated
+from mashumaro.types import Discriminator
+
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[
+        Annotated[
+            ClientEvent, Discriminator(field="type", include_subtypes=True)
+        ]
+    ]
+```
+
+Now we can deserialize events based on "type" value:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+#### Subclasses without a common field
+
+In rare cases you have to deal with subclasses that don't have a common field
+name which they can be distinguished by. Since `Discriminator` can be
+initialized without "field" parameter you can use it with only
+`include_subclasses` enabled. The drawback is that we will have to go through all
+the subclasses until we find the suitable one. It's almost like using `Union`
+type but with subclasses support.
+
+Suppose we're making a brunch. We have some ingredients:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+@dataclass
+class Hummus(Ingredient):
+    made_of: Literal["chickpeas", "beet", "artichoke"]
+    grams: int
+
+@dataclass
+class Celery(Ingredient):
+    pieces: int
+```
+
+Let's create a plate:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[Ingredient, Discriminator(include_subtypes=True)]
+    ]
+```
+
+And now we can put our ingredients on the plate:
+
+```python
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+    ]
+)
+```
+
+In some cases it's necessary to fall back to the base class if there is no
+suitable subclass. We can set `include_supertypes` to `True`:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Ingredient,
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+            {"name": "cumin"}  # <- new unknown ingredient
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+        Ingredient(name="cumin"),  # <- unknown ingredient added
+    ]
+)
+```
+
+#### Class level discriminator
+
+It may often be more convenient to specify a `Discriminator` once at the class
+level and use that class without `Annotated` type for subclass deserialization.
+Depending on the `Discriminator` parameters, it can be used as a replacement for
+[subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+as well as for [subclasses without a common field](#subclasses-without-a-common-field).
+The only difference is that you can't use `include_supertypes=True` because
+it would lead to a recursion error.
+
+Reworked example will look like this:
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from typing import List
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig
+from mashumaro.types import Discriminator
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    class Config(BaseConfig):
+        discriminator = Discriminator(  # <- add discriminator
+            field="type",
+            include_subtypes=True,
+        )
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[ClientEvent]  # <- use base class here
+```
+
+And now we can deserialize events based on "type" value as we did earlier:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+What's more interesting is that you can now deserialize subclasses simply by
+calling the superclass `from_*` method, which is very useful:
+```python
+disconnected_event = ClientEvent.from_dict(
+    {"type": "disconnected", "client_ip": "10.0.0.42"}
+)
+assert disconnected_event == ClientDisconnectedEvent(IPv4Address("10.0.0.42"))
+```
+
+The same is applicable for subclasses without a common field:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+    class Config:
+        discriminator = Discriminator(include_subtypes=True)
+
+...
+
+celery = Ingredient.from_dict({"name": "celery from my garden", "pieces": 5})
+assert celery == Celery(name="celery from my garden", pieces=5)
+```
+
+#### Working with union of classes
+
+Deserialization of union of types distinguishable by a particular field will
+be much faster using `Discriminator` because there will be no traversal
+of all classes and an attempt to deserialize each of them.
+Usually this approach can be used when you have multiple classes without a
+common superclass or when you only need to deserialize some of the subclasses.
+In the following example we will use `include_supertypes=True` to
+deserialize two subclasses out of three:
+
+```python
+from dataclasses import dataclass
+from typing import Annotated, Literal, Union
+# or from typing_extensions import Annotated
+from mashumaro import DataClassDictMixin
+from mashumaro.types import Discriminator
+
+@dataclass
+class Event(DataClassDictMixin):
+    pass
+
+@dataclass
+class Event1(Event):
+    code: Literal[1] = 1
+    ...
+
+@dataclass
+class Event2(Event):
+    code: Literal[2] = 2
+    ...
+
+@dataclass
+class Event3(Event):
+    code: Literal[3] = 3
+    ...
+
+@dataclass
+class Message(DataClassDictMixin):
+    event: Annotated[
+        Union[Event1, Event2],
+        Discriminator(field="code", include_supertypes=True),
+    ]
+
+event1_msg = Message.from_dict({"event": {"code": 1, ...}})
+event2_msg = Message.from_dict({"event": {"code": 2, ...}})
+assert isinstance(event1_msg.event, Event1)
+assert isinstance(event2_msg.event, Event2)
+
+# raises InvalidFieldValue:
+Message.from_dict({"event": {"code": 3, ...}})
+```
+
+Again, it's not necessary to have a common superclass. If you have a union of
+dataclasses without a field that they can be distinguishable by, you can still
+use `Discriminator`, but deserialization will almost be the same as for `Union`
+type without `Discriminator` except that it could be possible to deserialize
+subclasses with `include_subtypes=True`.
+
+> **Note**
+>
+> When both `include_subtypes` and `include_supertypes` are enabled,
+> all subclasses will be attempted to be deserialized first,
+> superclasses — at the end.
+
+```python
+@dataclass
+class Hummus(DataClassDictMixin):
+    made_of: Literal["chickpeas", "artichoke"]
+    grams: int
+
+@dataclass
+class ChickpeaHummus(Hummus):
+    made_of: Literal["chickpeas"]
+
+@dataclass
+class Celery(DataClassDictMixin):
+    pieces: int
+
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Union[Hummus, Celery],
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {"made_of": "chickpeas", "grams": 100},
+            {"made_of": "artichoke", "grams": 50},
+            {"pieces": 4},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        ChickpeaHummus(made_of='chickpeas', grams=100),  # <- subclass
+        Hummus(made_of='artichoke', grams=50),  # <- superclass
+        Celery(pieces=4),
+    ]
+)
+```
+
 ### Code generation options
 
 #### Add `omit_none` keyword argument
 
 If you want to have control over whether to skip `None` values on serialization
 you can add `omit_none` parameter to `to_*` methods using the
 `code_generation_options` list. The default value of `omit_none`
@@ -1575,14 +2074,94 @@
 class Entity(DataClassDictMixin):
     dt: date
 
     class Config(BaseConfig):
         code_generation_options = [ADD_DIALECT_SUPPORT]
 ```
 
+#### Add `context` keyword argument
+
+Sometimes it's needed to pass a "context" object to the serialization hooks
+that will take it into account. For example, you could want to have an option
+to remove sensitive data from the serialization result if you need to.
+You can add `context` parameter to `to_*` methods that will be passed to
+[`__pre_serialize__`](#before-serialization) and
+[`__post_serialize__`](#after-serialization) hooks. The type of this context
+as well as its mutability is up to you.
+
+```python
+from dataclasses import dataclass
+from typing import Dict, Optional
+from uuid import UUID
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig, ADD_SERIALIZATION_CONTEXT
+
+class BaseModel(DataClassDictMixin):
+    class Config(BaseConfig):
+        code_generation_options = [ADD_SERIALIZATION_CONTEXT]
+
+@dataclass
+class Account(BaseModel):
+    id: UUID
+    username: str
+    name: str
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["username"] = "***"
+            d["name"] = "***"
+        return d
+
+@dataclass
+class Session(BaseModel):
+    id: UUID
+    key: str
+    account: Account
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["key"] = "***"
+        return d
+
+
+foo = Session(
+    id=UUID('03321c9f-6a97-421e-9869-918ff2867a71'),
+    key="VQ6Q9bX4c8s",
+    account=Account(
+        id=UUID('4ef2baa7-edef-4d6a-b496-71e6d72c58fb'),
+        username="john_doe",
+        name="John"
+    )
+)
+assert foo.to_dict() == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': 'VQ6Q9bX4c8s',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': 'john_doe',
+        'name': 'John'
+    }
+}
+assert foo.to_dict(context={"remove_sensitive_data": True}) == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': '***',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': '***',
+        'name': '***'
+    }
+}
+```
+
 ### Generic dataclasses
 
 Along with [user-defined generic types](#user-defined-generic-types)
 implementing `SerializableType` interface, generic and variadic
 generic dataclasses can also be used. There are two applicable scenarios
 for them.
 
@@ -1765,14 +2344,17 @@
 
 obj = DataClass(abc=123)
 obj.to_dict()
 obj.to_json()
 print(obj.counter)  # 2
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 #### After serialization
 
 For doing something with a dictionary that was created as a result of
 serialization you can use `__post_serialize__` method:
 
 ```python
 @dataclass
@@ -1785,14 +2367,17 @@
         return d
 
 obj = DataClass(user="name", password="secret")
 print(obj.to_dict())  # {"user": "name"}
 print(obj.to_json())  # '{"user": "name"}'
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 JSON Schema
 --------------------------------------------------------------------------------
 
 You can build JSON Schema not only for dataclasses but also for any other
 [supported](#supported-data-types) data
 types. There is support for the following standards:
 * [Draft 2022-12](https://json-schema.org/specification.html)
```

### Comparing `mashumaro-3.7/README.md` & `mashumaro-3.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# mashumaro
+<div align="center">
+
+<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+</div>
 
 When using dataclasses, you often need to dump and load objects based on the
 schema you have. Mashumaro not only lets you save and load things in different
 ways, but it also does it _super quick_.
 
 **Key features**
 * 🚀 One of the fastest libraries
@@ -56,23 +59,32 @@
         * [`aliases` config option](#aliases-config-option)
         * [`serialize_by_alias` config option](#serialize_by_alias-config-option)
         * [`omit_none` config option](#omit_none-config-option)
         * [`namedtuple_as_dict` config option](#namedtuple_as_dict-config-option)
         * [`allow_postponed_evaluation` config option](#allow_postponed_evaluation-config-option)
         * [`dialect` config option](#dialect-config-option)
         * [`orjson_options`](#orjson_options-config-option)
+        * [`discriminator` config option](#discriminator-config-option)
+        * [`lazy_compilation` config option](#lazy_compilation-config-option)
     * [Passing field values as is](#passing-field-values-as-is)
+    * [Extending existing types](#extending-existing-types)
     * [Dialects](#dialects)
       * [`serialization_strategy` dialect option](#serialization_strategy-dialect-option)
       * [`omit_none` dialect option](#omit_none-dialect-option)
       * [Changing the default dialect](#changing-the-default-dialect)
+    * [Discriminator](#discriminator)
+      * [Subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+      * [Subclasses without a common field](#subclasses-without-a-common-field)
+      * [Class level discriminator](#class-level-discriminator)
+      * [Working with union of classes](#working-with-union-of-classes)
     * [Code generation options](#code-generation-options)
         * [Add `omit_none` keyword argument](#add-omit_none-keyword-argument)
         * [Add `by_alias` keyword argument](#add-by_alias-keyword-argument)
         * [Add `dialect` keyword argument](#add-dialect-keyword-argument)
+        * [Add `context` keyword argument](#add-context-keyword-argument)
     * [Generic dataclasses](#generic-dataclasses)
       * [Generic dataclass inheritance](#generic-dataclass-inheritance)
       * [Generic dataclass in a field type](#generic-dataclass-in-a-field-type)
     * [`GenericSerializableType` interface](#genericserializabletype-interface)
     * [Serialization hooks](#serialization-hooks)
         * [Before deserialization](#before-deserialization)
         * [After deserialization](#after-deserialization)
@@ -162,14 +174,15 @@
 * [`Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)
 * [`Union`](https://docs.python.org/3/library/typing.html#typing.Union)
 * [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar)
 * [`TypeVarTuple`](https://docs.python.org/3/library/typing.html#typing.TypeVarTuple)
 * [`NewType`](https://docs.python.org/3/library/typing.html#newtype)
 * [`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
 * [`Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)
+* [`Final`](https://docs.python.org/3/library/typing.html#typing.Final)
 * [`Self`](https://docs.python.org/3/library/typing.html#typing.Self)
 * [`Unpack`](https://docs.python.org/3/library/typing.html#typing.Unpack)
 
 for standard interpreter types from [`types`](https://docs.python.org/3/library/types.html#standard-interpreter-types) module:
 * [`NoneType`](https://docs.python.org/3/library/types.html#types.NoneType)
 * [`UnionType`](https://docs.python.org/3/library/types.html#types.UnionType)
 
@@ -282,27 +295,40 @@
 specific parser and builder for exactly that schema, taking into account the
 specifics of the serialization format. This is much faster than inspection of
 field types on every call of parsing or building at runtime.
 
 These specific parsers and builders are presented by the corresponding
 `from_*` and `to_*` methods. They are compiled during import time (or at
 runtime in some cases) and are set as attributes to your dataclasses.
+To minimize the import time, you can explicitly enable
+[lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
 * macOS 13.0.1 Ventura
 * Apple M1
 * 8GB RAM
 * Python 3.11.0
 
 Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
 The following figures show the best overall time in each case.
 
-<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump.png" width="400">
+[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
+
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
+</picture>
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
+</picture>
 
 <table>
   <col>
   <colgroup span="2"></colgroup>
   <colgroup span="2"></colgroup>
   <tr>
     <th rowspan="2">Library</th>
@@ -313,51 +339,51 @@
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14791</td>
+    <td align="right">0.14724</td>
     <td align="left">1x</td>
-    <td align="right">0.10294</td>
+    <td align="right">0.10128</td>
     <td align="left">1x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18913</td>
+    <td align="right">0.18906</td>
     <td align="left">1.28x</td>
-    <td align="right">0.13879</td>
-    <td align="left">1.35x</td>
+    <td align="right">0.14072</td>
+    <td align="left">1.39x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">0.92652</td>
-    <td align="left">6.26x</td>
-    <td align="right">0.81281</td>
-    <td align="left">7.9x</td>
+    <td align="right">1.02666</td>
+    <td align="left">6.97x</td>
+    <td align="right">0.81932</td>
+    <td align="left">8.09x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38964</td>
-    <td align="left">9.39x</td>
-    <td align="right">0.45987</td>
-    <td align="left">4.47x</td>
+    <td align="right">1.38348</td>
+    <td align="left">9.4x</td>
+    <td align="right">0.45695</td>
+    <td align="left">4.51x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
     <td align="left">—</td>
     <td align="left">—</td>
-    <td align="right">0.68592</td>
-    <td align="left">6.66x</td>
+    <td align="right">0.68057</td>
+    <td align="left">6.72x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.40445</td>
-    <td align="left">16.26x</td>
+    <td align="right">2.37315</td>
+    <td align="left">16.12x</td>
     <td align="left">—</td>
     <td align="left">—</td>
 </tr>
 </table>
 
 To run benchmark in your environment:
 ```bash
@@ -558,15 +584,15 @@
 assert my_flight == Flight(JFK, LAX)
 assert my_flight.to_dict() == input_data
 ```
 
 You can see how `Airport` instances are seamlessly created from lists of two
 strings and serialized into them.
 
-By default `_deserialize` method will get raw input data without any 
+By default `_deserialize` method will get raw input data without any
 transformations before. This should be enough in many cases, especially when
 you need to perform non-standard transformations yourself, but let's extend
 our example:
 
 ```python
 class Itinerary(SerializableType):
     def __init__(self, flights):
@@ -1053,14 +1079,15 @@
 described below.
 
 | Constant                                                        | Description                                                          |
 |:----------------------------------------------------------------|:---------------------------------------------------------------------|
 | [`TO_DICT_ADD_OMIT_NONE_FLAG`](#add-omit_none-keyword-argument) | Adds `omit_none` keyword-only argument to `to_*` methods.            |
 | [`TO_DICT_ADD_BY_ALIAS_FLAG`](#add-by_alias-keyword-argument)   | Adds `by_alias` keyword-only argument to `to_*` methods.             |
 | [`ADD_DIALECT_SUPPORT`](#add-dialect-keyword-argument)          | Adds `dialect` keyword-only argument to `from_*` and `to_*` methods. |
+| [`ADD_SERIALIZATION_CONTEXT`](#add-context-keyword-argument)    | Adds `context` keyword-only argument to `to_*` methods.              |
 
 #### `serialization_strategy` config option
 
 You can register custom [`SerializationStrategy`](#serializationstrategy), `serialize` and `deserialize`
 methods for specific types just in one place. It could be configured using
 a dictionary with types as keys. The value could be either a
 [`SerializationStrategy`](#serializationstrategy) instance or a dictionary with `serialize` and
@@ -1102,14 +1129,18 @@
 
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
+Note that you can register different methods for multiple logical types which
+are based on the same type using `NewType` and `Annotated`.
+See [Extending existing types](#extending-existing-types) for details.
+
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
 ```python
@@ -1309,14 +1340,36 @@
 
     class Config(BaseConfig):
         orjson_options = orjson.OPT_NON_STR_KEYS
 
 assert MyClass({1: 2}).to_json() == {"1": 2}
 ```
 
+#### `discriminator` config option
+
+This option is described in the
+[Class level discriminator](#class-level-discriminator) section.
+
+#### `lazy_compilation` config option
+
+By using this option, the compilation of the `from_*` and `to_*` methods will
+be deferred until they are called first time. This will reduce the import time
+and, in certain instances, may enhance the speed of deserialization
+by leveraging the data that is accessible after the class has been created.
+
+> **Warning**
+>
+> If you need to save a reference to `from_*` or `to_*` method, you should
+> do it after the method is compiled. To be safe, you can always use lambda
+> function:
+> ```python
+> from_dict = lambda x: MyModel.from_dict(x)
+> to_dict = lambda x: x.to_dict()
+> ```
+
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
 [`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
@@ -1378,20 +1431,74 @@
 a2_dict = A2(my_class_instance).to_dict()
 a3_dict = A3(my_class_instance).to_dict()
 a4_dict = A4(my_class_instance).to_dict()
 
 assert a1_dict == a2_dict == a3_dict == a4_dict == {"x": my_class_instance}
 ```
 
+### Extending existing types
+
+There are situations where you might want some values of the same type to be
+treated as their own type. You can create new logical types with
+[`NewType`](https://docs.python.org/3/library/typing.html#newtype) or
+[`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
+and register serialization strategies for them:
+
+```python
+from typing import Mapping, NewType, Annotated
+from dataclasses import dataclass
+from mashumaro import DataClassDictMixin
+
+SessionID = NewType("SessionID", str)
+AccountID = Annotated[str, "AccountID"]
+
+@dataclass
+class Context(DataClassDictMixin):
+    account_sessions: Mapping[AccountID, SessionID]
+
+    class Config:
+        serialization_strategy = {
+            AccountID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            },
+            SessionID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            }
+        }
+```
+
+Although using `NewType` is usually the most reliable way to avoid logical
+errors, you have to pay for it with notable overhead. If you are creating
+dataclass instances manually, then you know that type checkers will
+enforce you to enclose a value in your `"NewType"` callable, which leads
+to performance degradation:
+
+```python
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "MyInt(42)"
+10000000 loops, best of 5: 31.1 nsec per loop
+
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "42"
+50000000 loops, best of 5: 4.35 nsec per loop
+```
+
+However, when you create dataclass instances using the `from_*` method, there
+will be no performance degradation, because the value won't be enclosed in the
+callable in the generated code. Therefore, if performance is more important
+to you than catching logical errors by type checkers, and you are actively
+creating or changing dataclasses manually, then you should take a closer look
+at using `Annotated`.
+
 ### Dialects
 
 Sometimes it's needed to have different serialization and deserialization
 methods depending on the data source where entities of the dataclass are
 stored or on the API to which the entities are being sent or received from.
-There is a special Dialect type that may contain all the differences from the
+There is a special `Dialect` type that may contain all the differences from the
 default serialization and deserialization methods. You can create different
 dialects and use each of them for the same dataclass depending on
 the situation.
 
 Suppose we have the following dataclass with a field of type `date`:
 ```python
 @dataclass
@@ -1475,14 +1582,406 @@
         dialect = JapaneseDialect
 
 entity = Entity(date(2021, 12, 31))
 entity.to_dict()  # {'dt': '2021年12月31日'}
 assert Entity.from_dict({'dt': '2021年12月31日'}) == entity
 ```
 
+### Discriminator
+
+There is a special `Discriminator` class that allows you to customize how
+a union of dataclasses or their hierarchy will be deserialized.
+It has the following parameters that affects class selection rules:
+
+* `field` — optional name of the input dictionary key by which all the variants
+  can be distinguished
+* `include_subtypes` — allow to deserialize subclasses
+* `include_supertypes` — allow to deserialize superclasses
+
+Parameter `field` coule be in the following forms:
+
+* without annotations: `type = 42`
+* annotated as ClassVar: `type: ClassVar[int] = 42`
+* annotated as Final: `type: Final[int] = 42`
+* annotated as Literal: `type: Literal[42] = 42`
+* annotated as StrEnum: `type: ResponseType = ResponseType.OK`
+
+> **Note**
+>
+> Keep in mind that by default only Final, Literal and StrEnum fields are
+> processed during serialization.
+
+Next, we will look at different use cases, as well as their pros and cons.
+
+#### Subclasses distinguishable by a field
+
+Often you have a base dataclass and multiple subclasses that are easily
+distinguishable from each other by the value of a particular field.
+For example, there may be different events, messages or requests with
+a discriminator field "event_type", "message_type" or just "type". You could've
+listed all of them within `Union` type, but it would be too verbose and
+impractical. Moreover, deserialization of the union would be slow, since we
+need to iterate over each variant in the list until we find the right one.
+
+We can improve subclass deserialization using `Discriminator` as annotation
+within `Annotated` type. We will use `field` parameter and set
+`include_subtypes` to `True`.
+
+> **Note**
+>
+> The discriminator field should be accessible from the `__dict__` attribute
+> of a specific descendant, i.e. defined at the level of that descendant.
+> A descendant class without a discriminator field will be ignored, but
+> its descendants won't.
+
+Suppose we have a hierarchy of client events distinguishable by a class
+attribute "type":
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from mashumaro import DataClassDictMixin
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    pass
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+```
+
+We use base dataclass `ClientEvent` for a field of another dataclass:
+
+```python
+from typing import Annotated, List
+# or from typing_extensions import Annotated
+from mashumaro.types import Discriminator
+
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[
+        Annotated[
+            ClientEvent, Discriminator(field="type", include_subtypes=True)
+        ]
+    ]
+```
+
+Now we can deserialize events based on "type" value:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+#### Subclasses without a common field
+
+In rare cases you have to deal with subclasses that don't have a common field
+name which they can be distinguished by. Since `Discriminator` can be
+initialized without "field" parameter you can use it with only
+`include_subclasses` enabled. The drawback is that we will have to go through all
+the subclasses until we find the suitable one. It's almost like using `Union`
+type but with subclasses support.
+
+Suppose we're making a brunch. We have some ingredients:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+@dataclass
+class Hummus(Ingredient):
+    made_of: Literal["chickpeas", "beet", "artichoke"]
+    grams: int
+
+@dataclass
+class Celery(Ingredient):
+    pieces: int
+```
+
+Let's create a plate:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[Ingredient, Discriminator(include_subtypes=True)]
+    ]
+```
+
+And now we can put our ingredients on the plate:
+
+```python
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+    ]
+)
+```
+
+In some cases it's necessary to fall back to the base class if there is no
+suitable subclass. We can set `include_supertypes` to `True`:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Ingredient,
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+            {"name": "cumin"}  # <- new unknown ingredient
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+        Ingredient(name="cumin"),  # <- unknown ingredient added
+    ]
+)
+```
+
+#### Class level discriminator
+
+It may often be more convenient to specify a `Discriminator` once at the class
+level and use that class without `Annotated` type for subclass deserialization.
+Depending on the `Discriminator` parameters, it can be used as a replacement for
+[subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+as well as for [subclasses without a common field](#subclasses-without-a-common-field).
+The only difference is that you can't use `include_supertypes=True` because
+it would lead to a recursion error.
+
+Reworked example will look like this:
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from typing import List
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig
+from mashumaro.types import Discriminator
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    class Config(BaseConfig):
+        discriminator = Discriminator(  # <- add discriminator
+            field="type",
+            include_subtypes=True,
+        )
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[ClientEvent]  # <- use base class here
+```
+
+And now we can deserialize events based on "type" value as we did earlier:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+What's more interesting is that you can now deserialize subclasses simply by
+calling the superclass `from_*` method, which is very useful:
+```python
+disconnected_event = ClientEvent.from_dict(
+    {"type": "disconnected", "client_ip": "10.0.0.42"}
+)
+assert disconnected_event == ClientDisconnectedEvent(IPv4Address("10.0.0.42"))
+```
+
+The same is applicable for subclasses without a common field:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+    class Config:
+        discriminator = Discriminator(include_subtypes=True)
+
+...
+
+celery = Ingredient.from_dict({"name": "celery from my garden", "pieces": 5})
+assert celery == Celery(name="celery from my garden", pieces=5)
+```
+
+#### Working with union of classes
+
+Deserialization of union of types distinguishable by a particular field will
+be much faster using `Discriminator` because there will be no traversal
+of all classes and an attempt to deserialize each of them.
+Usually this approach can be used when you have multiple classes without a
+common superclass or when you only need to deserialize some of the subclasses.
+In the following example we will use `include_supertypes=True` to
+deserialize two subclasses out of three:
+
+```python
+from dataclasses import dataclass
+from typing import Annotated, Literal, Union
+# or from typing_extensions import Annotated
+from mashumaro import DataClassDictMixin
+from mashumaro.types import Discriminator
+
+@dataclass
+class Event(DataClassDictMixin):
+    pass
+
+@dataclass
+class Event1(Event):
+    code: Literal[1] = 1
+    ...
+
+@dataclass
+class Event2(Event):
+    code: Literal[2] = 2
+    ...
+
+@dataclass
+class Event3(Event):
+    code: Literal[3] = 3
+    ...
+
+@dataclass
+class Message(DataClassDictMixin):
+    event: Annotated[
+        Union[Event1, Event2],
+        Discriminator(field="code", include_supertypes=True),
+    ]
+
+event1_msg = Message.from_dict({"event": {"code": 1, ...}})
+event2_msg = Message.from_dict({"event": {"code": 2, ...}})
+assert isinstance(event1_msg.event, Event1)
+assert isinstance(event2_msg.event, Event2)
+
+# raises InvalidFieldValue:
+Message.from_dict({"event": {"code": 3, ...}})
+```
+
+Again, it's not necessary to have a common superclass. If you have a union of
+dataclasses without a field that they can be distinguishable by, you can still
+use `Discriminator`, but deserialization will almost be the same as for `Union`
+type without `Discriminator` except that it could be possible to deserialize
+subclasses with `include_subtypes=True`.
+
+> **Note**
+>
+> When both `include_subtypes` and `include_supertypes` are enabled,
+> all subclasses will be attempted to be deserialized first,
+> superclasses — at the end.
+
+```python
+@dataclass
+class Hummus(DataClassDictMixin):
+    made_of: Literal["chickpeas", "artichoke"]
+    grams: int
+
+@dataclass
+class ChickpeaHummus(Hummus):
+    made_of: Literal["chickpeas"]
+
+@dataclass
+class Celery(DataClassDictMixin):
+    pieces: int
+
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Union[Hummus, Celery],
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {"made_of": "chickpeas", "grams": 100},
+            {"made_of": "artichoke", "grams": 50},
+            {"pieces": 4},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        ChickpeaHummus(made_of='chickpeas', grams=100),  # <- subclass
+        Hummus(made_of='artichoke', grams=50),  # <- superclass
+        Celery(pieces=4),
+    ]
+)
+```
+
 ### Code generation options
 
 #### Add `omit_none` keyword argument
 
 If you want to have control over whether to skip `None` values on serialization
 you can add `omit_none` parameter to `to_*` methods using the
 `code_generation_options` list. The default value of `omit_none`
@@ -1549,14 +2048,94 @@
 class Entity(DataClassDictMixin):
     dt: date
 
     class Config(BaseConfig):
         code_generation_options = [ADD_DIALECT_SUPPORT]
 ```
 
+#### Add `context` keyword argument
+
+Sometimes it's needed to pass a "context" object to the serialization hooks
+that will take it into account. For example, you could want to have an option
+to remove sensitive data from the serialization result if you need to.
+You can add `context` parameter to `to_*` methods that will be passed to
+[`__pre_serialize__`](#before-serialization) and
+[`__post_serialize__`](#after-serialization) hooks. The type of this context
+as well as its mutability is up to you.
+
+```python
+from dataclasses import dataclass
+from typing import Dict, Optional
+from uuid import UUID
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig, ADD_SERIALIZATION_CONTEXT
+
+class BaseModel(DataClassDictMixin):
+    class Config(BaseConfig):
+        code_generation_options = [ADD_SERIALIZATION_CONTEXT]
+
+@dataclass
+class Account(BaseModel):
+    id: UUID
+    username: str
+    name: str
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["username"] = "***"
+            d["name"] = "***"
+        return d
+
+@dataclass
+class Session(BaseModel):
+    id: UUID
+    key: str
+    account: Account
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["key"] = "***"
+        return d
+
+
+foo = Session(
+    id=UUID('03321c9f-6a97-421e-9869-918ff2867a71'),
+    key="VQ6Q9bX4c8s",
+    account=Account(
+        id=UUID('4ef2baa7-edef-4d6a-b496-71e6d72c58fb'),
+        username="john_doe",
+        name="John"
+    )
+)
+assert foo.to_dict() == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': 'VQ6Q9bX4c8s',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': 'john_doe',
+        'name': 'John'
+    }
+}
+assert foo.to_dict(context={"remove_sensitive_data": True}) == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': '***',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': '***',
+        'name': '***'
+    }
+}
+```
+
 ### Generic dataclasses
 
 Along with [user-defined generic types](#user-defined-generic-types)
 implementing `SerializableType` interface, generic and variadic
 generic dataclasses can also be used. There are two applicable scenarios
 for them.
 
@@ -1739,14 +2318,17 @@
 
 obj = DataClass(abc=123)
 obj.to_dict()
 obj.to_json()
 print(obj.counter)  # 2
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 #### After serialization
 
 For doing something with a dictionary that was created as a result of
 serialization you can use `__post_serialize__` method:
 
 ```python
 @dataclass
@@ -1759,14 +2341,17 @@
         return d
 
 obj = DataClass(user="name", password="secret")
 print(obj.to_dict())  # {"user": "name"}
 print(obj.to_json())  # '{"user": "name"}'
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 JSON Schema
 --------------------------------------------------------------------------------
 
 You can build JSON Schema not only for dataclasses but also for any other
 [supported](#supported-data-types) data
 types. There is support for the following standards:
 * [Draft 2022-12](https://json-schema.org/specification.html)
```

### Comparing `mashumaro-3.7/mashumaro/config.py` & `mashumaro-3.8/mashumaro/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 from mashumaro.core.const import PEP_586_COMPATIBLE, Sentinel
 from mashumaro.dialect import Dialect
-from mashumaro.types import SerializationStrategy
+from mashumaro.types import Discriminator, SerializationStrategy
 
 if PEP_586_COMPATIBLE:
     from typing import Literal  # type: ignore
 else:
     from typing_extensions import Literal  # type: ignore
 
 
 __all__ = [
     "BaseConfig",
     "TO_DICT_ADD_BY_ALIAS_FLAG",
     "TO_DICT_ADD_OMIT_NONE_FLAG",
     "ADD_DIALECT_SUPPORT",
+    "ADD_SERIALIZATION_CONTEXT",
     "SerializationStrategyValueType",
 ]
 
 
 TO_DICT_ADD_BY_ALIAS_FLAG = "TO_DICT_ADD_BY_ALIAS_FLAG"
 TO_DICT_ADD_OMIT_NONE_FLAG = "TO_DICT_ADD_OMIT_NONE_FLAG"
 ADD_DIALECT_SUPPORT = "ADD_DIALECT_SUPPORT"
+ADD_SERIALIZATION_CONTEXT = "ADD_SERIALIZATION_CONTEXT"
 
 
 CodeGenerationOption = Literal[
     "TO_DICT_ADD_BY_ALIAS_FLAG",
     "TO_DICT_ADD_OMIT_NONE_FLAG",
     "ADD_DIALECT_SUPPORT",
+    "ADD_SERIALIZATION_CONTEXT",
 ]
 
 
 SerializationStrategyValueType = Union[
     SerializationStrategy, Dict[str, Union[str, Callable]]
 ]
 
@@ -44,7 +47,9 @@
     serialize_by_alias: bool = False
     namedtuple_as_dict: bool = False
     allow_postponed_evaluation: bool = True
     dialect: Optional[Type[Dialect]] = None
     omit_none: Union[bool, Literal[Sentinel.MISSING]] = Sentinel.MISSING
     orjson_options: Optional[int] = 0
     json_schema: Dict[str, Any] = {}
+    discriminator: Optional[Discriminator] = None
+    lazy_compilation: bool = False
```

### Comparing `mashumaro-3.7/mashumaro/core/const.py` & `mashumaro-3.8/mashumaro/core/const.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/core/helpers.py` & `mashumaro-3.8/mashumaro/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/core/meta/code/builder.py` & `mashumaro-3.8/mashumaro/core/meta/code/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import importlib
 import inspect
 import types
 import typing
 from contextlib import contextmanager
 
 # noinspection PyProtectedMember
-from dataclasses import _FIELDS, MISSING, Field, is_dataclass  # type: ignore
+from dataclasses import _FIELDS  # type: ignore
+from dataclasses import MISSING, Field, is_dataclass
 from functools import lru_cache
 
+try:
+    from dataclasses import KW_ONLY  # type: ignore
+except ImportError:
+    KW_ONLY = object()  # type: ignore
+
 import typing_extensions
 
 from mashumaro.config import (
     ADD_DIALECT_SUPPORT,
+    ADD_SERIALIZATION_CONTEXT,
     TO_DICT_ADD_BY_ALIAS_FLAG,
     TO_DICT_ADD_OMIT_NONE_FLAG,
     BaseConfig,
     SerializationStrategyValueType,
 )
 from mashumaro.core.const import Sentinel
 from mashumaro.core.helpers import ConfigValue
@@ -28,36 +35,42 @@
     get_name_error_name,
     hash_type_args,
     is_class_var,
     is_dataclass_dict_mixin,
     is_dialect_subclass,
     is_init_var,
     is_literal,
-    is_named_tuple,
     is_optional,
     is_type_var_any,
     resolve_type_params,
+    substitute_type_params,
     type_name,
 )
 from mashumaro.core.meta.types.common import FieldContext, ValueSpec
 from mashumaro.core.meta.types.pack import PackerRegistry
-from mashumaro.core.meta.types.unpack import UnpackerRegistry
+from mashumaro.core.meta.types.unpack import (
+    SubtypeUnpackerBuilder,
+    UnpackerRegistry,
+)
 from mashumaro.dialect import Dialect
 from mashumaro.exceptions import (  # noqa
     BadDialect,
     BadHookSignature,
     InvalidFieldValue,
+    MissingDiscriminatorError,
     MissingField,
+    SuitableVariantNotFoundError,
     ThirdPartyModuleNotFoundError,
     UnresolvedTypeReferenceError,
     UnserializableDataError,
     UnserializableField,
     UnsupportedDeserializationEngine,
     UnsupportedSerializationEngine,
 )
+from mashumaro.types import Discriminator
 
 __PRE_SERIALIZE__ = "__pre_serialize__"
 __PRE_DESERIALIZE__ = "__pre_deserialize__"
 __POST_SERIALIZE__ = "__post_serialize__"
 __POST_DESERIALIZE__ = "__post_deserialize__"
 
 
@@ -120,15 +133,15 @@
             field_type_hints = typing_extensions.get_type_hints(
                 self.cls, include_extras=include_extras
             )
         except NameError as e:
             name = get_name_error_name(e)
             raise UnresolvedTypeReferenceError(self.cls, name) from None
         for fname, ftype in field_type_hints.items():
-            if is_class_var(ftype) or is_init_var(ftype):
+            if is_class_var(ftype) or is_init_var(ftype) or ftype is KW_ONLY:
                 continue
             if recursive or fname in self.annotations:
                 fields[fname] = ftype
         return fields
 
     def _get_field_class(self, field_name: str) -> typing.Any:
         try:
@@ -138,26 +151,24 @@
             self.field_classes[field_name] = cls
         return cls
 
     def _get_real_type(
         self, field_name: str, field_type: typing.Type
     ) -> typing.Type:
         cls = self._get_field_class(field_name)
-        return self.resolved_type_params[cls].get(field_type, field_type)
+        return substitute_type_params(
+            field_type, self.resolved_type_params[cls]
+        )
 
     def get_field_resolved_type_params(
         self, field_name: str
     ) -> typing.Dict[typing.Type, typing.Type]:
         cls = self._get_field_class(field_name)
         return self.resolved_type_params[cls]
 
-    @property
-    def field_types(self) -> typing.Dict[str, typing.Any]:
-        return self.__get_field_types()
-
     def get_field_types(
         self, include_extras: bool = False
     ) -> typing.Dict[str, typing.Any]:
         return self.__get_field_types(include_extras=include_extras)
 
     @property  # type: ignore
     @lru_cache()
@@ -230,16 +241,19 @@
     ) -> None:
         self.globals.setdefault(name or obj.__name__, obj)
 
     def add_line(self, line: str) -> None:
         self.lines.append(line)
 
     @contextmanager
-    def indent(self) -> typing.Generator[None, None, None]:
-        with self.lines.indent():
+    def indent(
+        self,
+        expr: typing.Optional[str] = None,
+    ) -> typing.Generator[None, None, None]:
+        with self.lines.indent(expr):
             yield
 
     def compile(self) -> None:
         code = self.lines.as_text()
         if self.get_config().debug:
             if self.dialect is not None:
                 print(f"{type_name(self.cls)}[{type_name(self.dialect)}]:")
@@ -249,113 +263,158 @@
         exec(code, self.globals, self.__dict__)
 
     def get_declared_hook(self, method_name: str) -> typing.Any:
         cls = get_class_that_defines_method(method_name, self.cls)
         if cls is not None and not is_dataclass_dict_mixin(cls):
             return cls.__dict__[method_name]
 
+    def _add_unpack_method_lines_lazy(self, method_name: str) -> None:
+        if self.default_dialect is not None:
+            self.add_type_modules(self.default_dialect)
+        self.add_line(
+            f"CodeBuilder("
+            f"cls,"
+            f"first_method='{method_name}',"
+            f"allow_postponed_evaluation=False,"
+            f"format_name='{self.format_name}',"
+            f"decoder={type_name(self.decoder)},"  # type: ignore
+            f"default_dialect={type_name(self.default_dialect)}"
+            f").add_unpack_method()"
+        )
+        unpacker_args = [
+            "d",
+            self.get_unpack_method_flags(pass_decoder=True),
+        ]
+        unpacker_args_s = ", ".join(filter(None, unpacker_args))
+        self.add_line(f"return cls.{method_name}({unpacker_args_s})")
+
     def _add_unpack_method_lines(self, method_name: str) -> None:
         config = self.get_config()
+        if config.lazy_compilation and self.allow_postponed_evaluation:
+            self._add_unpack_method_lines_lazy(method_name)
+            return
         try:
-            field_types = self.field_types
+            field_types = self.get_field_types(include_extras=True)
         except UnresolvedTypeReferenceError:
             if (
                 not self.allow_postponed_evaluation
                 or not config.allow_postponed_evaluation
             ):
                 raise
-            if self.default_dialect is not None:
-                self.add_type_modules(self.default_dialect)
-            self.add_line(
-                f"CodeBuilder("
-                f"cls,"
-                f"first_method='{method_name}',"
-                f"allow_postponed_evaluation=False,"
-                f"format_name='{self.format_name}',"
-                f"decoder={type_name(self.decoder)},"  # type: ignore
-                f"default_dialect={type_name(self.default_dialect)}"
-                f").add_unpack_method()"
-            )
-            unpacker_args = [
-                "d",
-                self.get_unpack_method_flags(pass_decoder=True),
-            ]
-            unpacker_args_s = ", ".join(filter(None, unpacker_args))
-            self.add_line(f"return cls.{method_name}({unpacker_args_s})")
+            self._add_unpack_method_lines_lazy(method_name)
         else:
             if self.decoder is not None:
                 self.add_line("d = decoder(d)")
+            discr = self.get_discriminator()
+            if discr:
+                if not discr.include_subtypes:
+                    raise ValueError(
+                        "Config based discriminator must have "
+                        "'include_subtypes' enabled"
+                    )
+                discr = Discriminator(
+                    # prevent RecursionError
+                    field=discr.field,
+                    include_subtypes=discr.include_subtypes,
+                )
+                self.add_type_modules(self.cls)
+                method = SubtypeUnpackerBuilder(discr).build(
+                    spec=ValueSpec(
+                        type=self.cls,
+                        expression="d",
+                        builder=self,
+                        field_ctx=FieldContext("", {}),
+                    )
+                )
+                self.add_line(f"return {method}")
+                return
             pre_deserialize = self.get_declared_hook(__PRE_DESERIALIZE__)
             if pre_deserialize:
                 if not isinstance(pre_deserialize, classmethod):
                     raise BadHookSignature(
                         f"`{__PRE_DESERIALIZE__}` must be a class method with "
                         f"Callable[[Dict[Any, Any]], Dict[Any, Any]] signature"
                     )
                 else:
                     self.add_line(f"d = cls.{__PRE_DESERIALIZE__}(d)")
+            post_deserialize = self.get_declared_hook(__POST_DESERIALIZE__)
+            if post_deserialize:
+                if not isinstance(post_deserialize, classmethod):
+                    raise BadHookSignature(
+                        f"`{__POST_DESERIALIZE__}` must be a class method "
+                        f"with Callable[[{type_name(self.cls)}], "
+                        f"{type_name(self.cls)}] signature"
+                    )
             filtered_fields = []
+            kwargs_only = post_deserialize is not None
+            pos_args = []
+            kw_args = []
+            can_be_kwargs = False
             for fname, ftype in field_types.items():
                 field = self.dataclass_fields.get(fname)  # type: ignore
                 # https://github.com/python/mypy/issues/1362
                 if field and not field.init:
                     continue
+                if self.get_field_default(fname) is MISSING:
+                    if field and not getattr(field, "kw_only", True):
+                        pos_args.append(fname)
+                    else:
+                        kw_args.append(fname)
+                else:
+                    can_be_kwargs = True
                 filtered_fields.append((fname, ftype))
             if filtered_fields:
-                self.add_line("try:")
-                with self.indent():
-                    self.add_line("kwargs = {}")
+                with self.indent("try:"):
+                    if kwargs_only or can_be_kwargs:
+                        self.add_line("kwargs = {}")
                     for fname, ftype in filtered_fields:
                         self.add_type_modules(ftype)
                         metadata = self.metadatas.get(fname, {})
                         alias = metadata.get("alias")
                         if alias is None:
                             alias = config.aliases.get(fname)
                         self._unpack_method_set_value(
-                            fname, ftype, metadata, alias
+                            fname,
+                            ftype,
+                            metadata,
+                            alias=alias,
+                            kwargs_only=kwargs_only,
                         )
-                self.add_line("except TypeError:")
-                with self.indent():
-                    self.add_line("if not isinstance(d, dict):")
-                    with self.indent():
+                with self.indent("except TypeError:"):
+                    with self.indent("if not isinstance(d, dict):"):
                         self.add_line(
                             f"raise ValueError('Argument for "
                             f"{type_name(self.cls)}.{method_name} method "
                             f"should be a dict instance') from None"
                         )
-                    self.add_line("else:")
-                    with self.indent():
+                    with self.indent("else:"):
                         self.add_line("raise")
             else:
                 self.add_line("kwargs = {}")
-            post_deserialize = self.get_declared_hook(__POST_DESERIALIZE__)
             if post_deserialize:
-                if not isinstance(post_deserialize, classmethod):
-                    raise BadHookSignature(
-                        f"`{__POST_DESERIALIZE__}` must be a class method "
-                        f"with Callable[[{type_name(self.cls)}], "
-                        f"{type_name(self.cls)}] signature"
-                    )
-                else:
-                    self.add_line(
-                        f"return cls.{__POST_DESERIALIZE__}(cls(**kwargs))"
-                    )
+                self.add_line(
+                    f"return cls.{__POST_DESERIALIZE__}(cls(**kwargs))"
+                )
             else:
-                self.add_line("return cls(**kwargs)")
+                args = [f"__{f}" for f in pos_args]
+                for kw_arg in kw_args:
+                    args.append(f"{kw_arg}=__{kw_arg}")
+                if can_be_kwargs:
+                    args.append("**kwargs")
+                self.add_line(f"return cls({', '.join(args)})")
 
     def _add_unpack_method_with_dialect_lines(self, method_name: str) -> None:
         if self.decoder is not None:
             self.add_line("d = decoder(d)")
         unpacker_args = ", ".join(
             filter(None, ("cls", "d", self.get_unpack_method_flags()))
         )
         cache_name = f"__dialect_{self.format_name}_unpacker_cache__"
         self.add_line(f"unpacker = cls.{cache_name}.get(dialect)")
-        self.add_line("if unpacker is not None:")
-        with self.indent():
+        with self.indent("if unpacker is not None:"):
             self.add_line(f"return unpacker({unpacker_args})")
         if self.default_dialect:
             self.add_type_modules(self.default_dialect)
         self.add_line(
             f"CodeBuilder("
             f"cls,dialect=dialect,"
             f"first_method='{method_name}',"
@@ -375,28 +434,25 @@
         if self.decoder is not None:
             self.add_type_modules(self.decoder)
         dialects_feature = self.is_code_generation_option_enabled(
             ADD_DIALECT_SUPPORT
         )
         cache_name = f"__dialect_{self.format_name}_unpacker_cache__"
         if dialects_feature:
-            self.add_line(f"if not '{cache_name}' in cls.__dict__:")
-            with self.indent():
+            with self.indent(f"if not '{cache_name}' in cls.__dict__:"):
                 self.add_line(f"cls.{cache_name} = {{}}")
 
         if self.dialect is None:
             self.add_line("@classmethod")
         self._add_unpack_method_definition(method_name)
         with self.indent():
             if dialects_feature and self.dialect is None:
-                self.add_line("if dialect is None:")
-                with self.indent():
+                with self.indent("if dialect is None:"):
                     self._add_unpack_method_lines(method_name)
-                self.add_line("else:")
-                with self.indent():
+                with self.indent("else:"):
                     self._add_unpack_method_with_dialect_lines(method_name)
             else:
                 self._add_unpack_method_lines(method_name)
         if self.dialect is None:
             self.add_line(f"setattr(cls, '{method_name}', {method_name})")
         else:
             self.add_line(f"cls.{cache_name}[dialect] = {method_name}")
@@ -412,107 +468,155 @@
         self.add_line(f"def {method_name}(cls, d{kwargs}):")
 
     def _unpack_method_set_value(
         self,
         fname: str,
         ftype: typing.Type,
         metadata: typing.Mapping,
+        *,
         alias: typing.Optional[str] = None,
+        kwargs_only: bool = False,
     ) -> None:
-        self.add_line("try:")
-        with self.indent():
-            could_be_none = False
-            if is_named_tuple(ftype):
-                self.add_line(f"value = d['{alias or fname}']")
-                packed_value = "value"
-            else:
-                packed_value = f"d['{alias or fname}']"
-                could_be_none = (
-                    ftype in (typing.Any, type(None), None)
-                    or is_type_var_any(self._get_real_type(fname, ftype))
-                    or is_optional(
-                        ftype, self.get_field_resolved_type_params(fname)
-                    )
-                    or self.get_field_default(fname) is None
-                )
-                if could_be_none:
-                    self.add_line(f"value = {packed_value}")
-                    packed_value = "value"
-            unpacked_value = UnpackerRegistry.get(
-                ValueSpec(
-                    type=ftype,
-                    expression=packed_value,
-                    builder=self,
-                    field_ctx=FieldContext(
-                        name=fname,
-                        metadata=metadata,
-                    ),
-                    could_be_none=False if could_be_none else True,
-                )
-            )
-            if could_be_none:
-                self.add_line("if value is not None:")
-                with self.indent():
-                    self.add_line(f"kwargs['{fname}'] = {unpacked_value}")
-                self.add_line("else:")
-                with self.indent():
-                    self.add_line(f"kwargs['{fname}'] = None")
-            else:
-                self.add_line(f"kwargs['{fname}'] = {unpacked_value}")
-        self.add_line("except KeyError as e:")
-        with self.indent():
-            field_type = type_name(
-                ftype,
-                resolved_type_params=self.get_field_resolved_type_params(
-                    fname
+        default = self.get_field_default(fname)
+        has_default = default is not MISSING
+        field_type = type_name(
+            ftype,
+            resolved_type_params=self.get_field_resolved_type_params(fname),
+        )
+        could_be_none = (
+            ftype in (typing.Any, type(None), None)
+            or is_type_var_any(self._get_real_type(fname, ftype))
+            or is_optional(ftype, self.get_field_resolved_type_params(fname))
+            or default is None
+        )
+        unpacked_value = UnpackerRegistry.get(
+            ValueSpec(
+                type=ftype,
+                expression="value",
+                builder=self,
+                field_ctx=FieldContext(
+                    name=fname,
+                    metadata=metadata,
                 ),
+                could_be_none=False if could_be_none else True,
             )
-            if self.get_field_default(fname) is MISSING:
-                self.add_line("if e.__traceback__.tb_next is None:")
-                with self.indent():
-                    self.add_line(
-                        f"raise MissingField('{fname}',{field_type},cls) "
-                        f"from None"
-                    )
-                self.add_line("else:")
-                with self.indent():
-                    self.add_line(
-                        f"raise InvalidFieldValue("
-                        f"'{fname}',{field_type},{packed_value},cls)"
+        )
+        if unpacked_value != "value":
+            self.add_line(f"value = d.get('{alias or fname}', MISSING)")
+            packed_value = "value"
+        elif has_default:
+            self.add_line(f"value = d.get('{alias or fname}', MISSING)")
+            packed_value = "value"
+        else:
+            self.add_line(f"__{fname} = d.get('{alias or fname}', MISSING)")
+            packed_value = f"__{fname}"
+            unpacked_value = packed_value
+        if not has_default:
+            with self.indent(f"if {packed_value} is MISSING:"):
+                self.add_line(
+                    f"raise MissingField('{fname}',{field_type},cls) "
+                    f"from None"
+                )
+            if packed_value != unpacked_value:
+                if could_be_none:
+                    with self.indent(f"if {packed_value} is not None:"):
+                        self.__unpack_try_set_value(
+                            fname,
+                            field_type,
+                            unpacked_value,
+                            kwargs_only,
+                            has_default,
+                        )
+                    with self.indent("else:"):
+                        self.__unpack_set_value(
+                            fname, "None", kwargs_only or has_default
+                        )
+                else:
+                    self.__unpack_try_set_value(
+                        fname,
+                        field_type,
+                        unpacked_value,
+                        kwargs_only,
+                        has_default,
                     )
-            else:
-                self.add_line("if e.__traceback__.tb_next is not None:")
-                with self.indent():
-                    self.add_line(
-                        f"raise InvalidFieldValue("
-                        f"'{fname}',{field_type},{packed_value},cls)"
+        else:
+            with self.indent(f"if {packed_value} is not MISSING:"):
+                if could_be_none:
+                    with self.indent(f"if {packed_value} is not None:"):
+                        self.__unpack_try_set_value(
+                            fname,
+                            field_type,
+                            unpacked_value,
+                            kwargs_only,
+                            has_default,
+                        )
+                    if default is not None:
+                        with self.indent("else:"):
+                            self.__unpack_set_value(
+                                fname, "None", kwargs_only or has_default
+                            )
+                else:
+                    self.__unpack_try_set_value(
+                        fname,
+                        field_type,
+                        unpacked_value,
+                        kwargs_only,
+                        has_default,
                     )
-        self.add_line("except Exception:")
-        with self.indent():
+
+    def __unpack_try_set_value(
+        self,
+        field_name: str,
+        field_type_name: str,
+        unpacked_value: str,
+        kwargs_only: bool,
+        has_default: bool,
+    ) -> None:
+        with self.indent("try:"):
+            self.__unpack_set_value(
+                field_name, unpacked_value, kwargs_only or has_default
+            )
+        with self.indent("except:"):
             self.add_line(
                 f"raise InvalidFieldValue("
-                f"'{fname}',{field_type},{packed_value},cls)"
+                f"'{field_name}',{field_type_name},value,cls)"
             )
 
+    def __unpack_set_value(
+        self, fname: str, unpacked_value: str, kwargs_only: bool
+    ) -> None:
+        if kwargs_only:
+            self.add_line(f"kwargs['{fname}'] = {unpacked_value}")
+        else:
+            self.add_line(f"__{fname} = {unpacked_value}")
+
     @lru_cache()
     @typing.no_type_check
     def get_config(
-        self, cls: typing.Optional[typing.Type] = None
+        self,
+        cls: typing.Optional[typing.Type] = None,
+        look_in_parents: bool = True,
     ) -> typing.Type[BaseConfig]:
         if cls is None:
             cls = self.cls
-        config_cls = getattr(cls, "Config", BaseConfig)
+        if look_in_parents:
+            config_cls = getattr(cls, "Config", BaseConfig)
+        else:
+            config_cls = self.namespace.get("Config", BaseConfig)
         if not issubclass(config_cls, BaseConfig):
             config_cls = type(
                 "Config",
                 (BaseConfig, config_cls),
                 {**BaseConfig.__dict__, **config_cls.__dict__},
             )
         return config_cls
 
+    def get_discriminator(self) -> typing.Optional[Discriminator]:
+        return self.get_config(look_in_parents=False).discriminator
+
     def get_pack_method_flags(
         self,
         cls: typing.Optional[typing.Type] = None,
         pass_encoder: bool = False,
     ) -> str:
         pluggable_flags = []
         if pass_encoder and self.encoder is not None:
@@ -520,14 +624,15 @@
             for value in self._get_encoder_kwargs(cls).values():
                 pluggable_flags.append(f"{value[0]}={value[0]}")
 
         for option, flag in (
             (TO_DICT_ADD_OMIT_NONE_FLAG, "omit_none"),
             (TO_DICT_ADD_BY_ALIAS_FLAG, "by_alias"),
             (ADD_DIALECT_SUPPORT, "dialect"),
+            (ADD_SERIALIZATION_CONTEXT, "context"),
         ):
             if self.is_code_generation_option_enabled(option, cls):
                 if self.is_code_generation_option_enabled(option):
                     pluggable_flags.append(f"{flag}={flag}")
         return ", ".join(pluggable_flags)
 
     def get_unpack_method_flags(
@@ -555,36 +660,47 @@
         kw_param_values = []
         if pass_encoder and self.encoder is not None:
             pos_param_names.append("encoder")
             pos_param_values.append(type_name(self.encoder))
             for value in self._get_encoder_kwargs(cls).values():
                 kw_param_names.append(value[0])
                 kw_param_values.append(value[1])
+
         omit_none_feature = self.is_code_generation_option_enabled(
             TO_DICT_ADD_OMIT_NONE_FLAG, cls
         )
         if omit_none_feature:
             omit_none = self._get_dialect_or_config_option(
                 "omit_none", False, None
             )
             kw_param_names.append("omit_none")
             kw_param_values.append("True" if omit_none else "False")
+
         by_alias_feature = self.is_code_generation_option_enabled(
             TO_DICT_ADD_BY_ALIAS_FLAG, cls
         )
         if by_alias_feature:
             serialize_by_alias = self.get_config(cls).serialize_by_alias
             kw_param_names.append("by_alias")
             kw_param_values.append("True" if serialize_by_alias else "False")
+
         dialects_feature = self.is_code_generation_option_enabled(
             ADD_DIALECT_SUPPORT, cls
         )
         if dialects_feature:
             kw_param_names.append("dialect")
             kw_param_values.append("None")
+
+        context_feature = self.is_code_generation_option_enabled(
+            ADD_SERIALIZATION_CONTEXT, cls
+        )
+        if context_feature:
+            kw_param_names.append("context")
+            kw_param_values.append("None")
+
         if pos_param_names:
             pluggable_flags_str = ", ".join(
                 [f"{n}={v}" for n, v in zip(pos_param_names, pos_param_values)]
             )
         else:
             pluggable_flags_str = ""
         if kw_param_names:
@@ -592,43 +708,42 @@
                 pluggable_flags_str += ", "
             pluggable_flags_str += "*, " + ", ".join(
                 [f"{n}={v}" for n, v in zip(kw_param_names, kw_param_values)]
             )
         return pluggable_flags_str
 
     def get_unpack_method_default_flag_values(
-        self,
-        cls: typing.Optional[typing.Type] = None,
-        pass_decoder: bool = False,
+        self, pass_decoder: bool = False
     ) -> str:
         pos_param_names = []
         pos_param_values = []
         kw_param_names = []
         kw_param_values = []
+
         if pass_decoder and self.decoder is not None:
             pos_param_names.append("decoder")
             pos_param_values.append(type_name(self.decoder))
-        dialects_feature = self.is_code_generation_option_enabled(
-            ADD_DIALECT_SUPPORT, cls
-        )
-        if dialects_feature:
-            kw_param_names.append("dialect")
-            kw_param_values.append("None")
+
+        kw_param_names.append("dialect")
+        kw_param_values.append("None")
+
         if pos_param_names:
             pluggable_flags_str = ", ".join(
                 [f"{n}={v}" for n, v in zip(pos_param_names, pos_param_values)]
             )
         else:
             pluggable_flags_str = ""
+
         if kw_param_names:
             if pos_param_names:
                 pluggable_flags_str += ", "
             pluggable_flags_str += "*, " + ", ".join(
                 [f"{n}={v}" for n, v in zip(kw_param_names, kw_param_values)]
             )
+
         return pluggable_flags_str
 
     def is_code_generation_option_enabled(
         self, option: str, cls: typing.Optional[typing.Type] = None
     ) -> bool:
         if cls is None:
             cls = self.cls
@@ -664,43 +779,57 @@
             method_name = "to_dict"
             if format_name != "dict":
                 method_name += f"_{format_name}"
             if type_args:
                 method_name += f"_{hash_type_args(type_args)}"
             return method_name
 
+    def _add_pack_method_lines_lazy(self, method_name: str) -> None:
+        if self.default_dialect is not None:
+            self.add_type_modules(self.default_dialect)
+        self.add_line(
+            f"CodeBuilder("
+            f"self.__class__,"
+            f"first_method='{method_name}',"
+            f"allow_postponed_evaluation=False,"
+            f"format_name='{self.format_name}',"
+            f"encoder={type_name(self.encoder)},"
+            f"encoder_kwargs={self._get_encoder_kwargs()},"
+            f"default_dialect={type_name(self.default_dialect)}"
+            f").add_pack_method()"
+        )
+        packer_args = self.get_pack_method_flags(pass_encoder=True)
+        self.add_line(f"return self.{method_name}({packer_args})")
+
     def _add_pack_method_lines(self, method_name: str) -> None:
         config = self.get_config()
+        if config.lazy_compilation and self.allow_postponed_evaluation:
+            self._add_pack_method_lines_lazy(method_name)
+            return
         try:
-            field_types = self.field_types
+            field_types = self.get_field_types(include_extras=True)
         except UnresolvedTypeReferenceError:
             if (
                 not self.allow_postponed_evaluation
                 or not config.allow_postponed_evaluation
             ):
                 raise
-            if self.default_dialect is not None:
-                self.add_type_modules(self.default_dialect)
-            self.add_line(
-                f"CodeBuilder("
-                f"self.__class__,"
-                f"first_method='{method_name}',"
-                f"allow_postponed_evaluation=False,"
-                f"format_name='{self.format_name}',"
-                f"encoder={type_name(self.encoder)},"
-                f"encoder_kwargs={self._get_encoder_kwargs()},"
-                f"default_dialect={type_name(self.default_dialect)}"
-                f").add_pack_method()"
-            )
-            packer_args = self.get_pack_method_flags(pass_encoder=True)
-            self.add_line(f"return self.{method_name}({packer_args})")
+            self._add_pack_method_lines_lazy(method_name)
         else:
             pre_serialize = self.get_declared_hook(__PRE_SERIALIZE__)
             if pre_serialize:
-                self.add_line(f"self = self.{__PRE_SERIALIZE__}()")
+                if self.is_code_generation_option_enabled(
+                    ADD_SERIALIZATION_CONTEXT
+                ):
+                    pre_serialize_args = "context=context"
+                else:
+                    pre_serialize_args = ""
+                self.add_line(
+                    f"self = self.{__PRE_SERIALIZE__}({pre_serialize_args})"
+                )
             by_alias_feature = self.is_code_generation_option_enabled(
                 TO_DICT_ADD_BY_ALIAS_FLAG
             )
             omit_none_feature = self.is_code_generation_option_enabled(
                 TO_DICT_ADD_OMIT_NONE_FLAG
             )
             serialize_by_alias = self.get_config().serialize_by_alias
@@ -722,26 +851,23 @@
             if fields_could_be_none or by_alias_feature and aliases:
                 kwargs = "kwargs"
                 self.add_line("kwargs = {}")
                 for fname, packer in packers.items():
                     alias = aliases.get(fname)
                     if fname in fields_could_be_none:
                         self.add_line(f"value = self.{fname}")
-                        self.add_line("if value is not None:")
-                        with self.indent():
+                        with self.indent("if value is not None:"):
                             self._pack_method_set_value(
                                 fname, alias, by_alias_feature, packer
                             )
                         if omit_none and not omit_none_feature:
                             continue
-                        self.add_line("else:")
-                        with self.indent():
+                        with self.indent("else:"):
                             if omit_none_feature:
-                                self.add_line("if not omit_none:")
-                                with self.indent():
+                                with self.indent("if not omit_none:"):
                                     self._pack_method_set_value(
                                         fname, alias, by_alias_feature, "None"
                                     )
                             else:
                                 self._pack_method_set_value(
                                     fname, alias, by_alias_feature, "None"
                                 )
@@ -769,14 +895,18 @@
                         f"return encoder({{}}, {encoder_options})"
                     )
                 else:
                     return_statement = "return encoder({})"
             else:
                 return_statement = "return {}"
             if post_serialize:
+                if self.is_code_generation_option_enabled(
+                    ADD_SERIALIZATION_CONTEXT
+                ):
+                    kwargs = f"{kwargs}, context=context"
                 self.add_line(
                     return_statement.format(
                         f"self.{__POST_SERIALIZE__}({kwargs})"
                     )
                 )
             else:
                 self.add_line(return_statement.format(kwargs))
@@ -785,19 +915,17 @@
         self,
         fname: str,
         alias: typing.Optional[str],
         by_alias_feature: bool,
         packed_value: str,
     ) -> None:
         if by_alias_feature and alias is not None:
-            self.add_line("if by_alias:")
-            with self.indent():
+            with self.indent("if by_alias:"):
                 self.add_line(f"kwargs['{alias}'] = {packed_value}")
-            self.add_line("else:")
-            with self.indent():
+            with self.indent("else:"):
                 self.add_line(f"kwargs['{fname}'] = {packed_value}")
         else:
             serialize_by_alias = self.get_config().serialize_by_alias
             if serialize_by_alias and alias is not None:
                 fname_or_alias = alias
             else:
                 fname_or_alias = fname
@@ -863,26 +991,23 @@
         if self.encoder is not None:
             self.add_type_modules(self.encoder)
         dialects_feature = self.is_code_generation_option_enabled(
             ADD_DIALECT_SUPPORT
         )
         cache_name = f"__dialect_{self.format_name}_packer_cache__"
         if dialects_feature:
-            self.add_line(f"if not '{cache_name}' in cls.__dict__:")
-            with self.indent():
+            with self.indent(f"if not '{cache_name}' in cls.__dict__:"):
                 self.add_line(f"cls.{cache_name} = {{}}")
 
         self._add_pack_method_definition(method_name)
         with self.indent():
             if dialects_feature and self.dialect is None:
-                self.add_line("if dialect is None:")
-                with self.indent():
+                with self.indent("if dialect is None:"):
                     self._add_pack_method_lines(method_name)
-                self.add_line("else:")
-                with self.indent():
+                with self.indent("else:"):
                     self._add_pack_method_with_dialect_lines(method_name)
             else:
                 self._add_pack_method_lines(method_name)
         if self.dialect is None:
             self.add_line(f"setattr(cls, '{method_name}', {method_name})")
         else:
             self.add_line(f"cls.{cache_name}[dialect] = {method_name}")
```

### Comparing `mashumaro-3.7/mashumaro/core/meta/helpers.py` & `mashumaro-3.8/mashumaro/core/meta/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,27 @@
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
+try:
+    from typing import Unpack  # type: ignore[attr-defined]
+except ImportError:
+    from typing_extensions import Unpack
+
 import typing_extensions
-from typing_extensions import Unpack
 
 from mashumaro.core.const import (
     PEP_585_COMPATIBLE,
     PY_37,
     PY_38,
     PY_38_MIN,
+    PY_39,
     PY_39_MIN,
     PY_310_MIN,
     PY_311_MIN,
 )
 from mashumaro.dialect import Dialect
 
 __all__ = [
@@ -45,36 +50,40 @@
     "is_named_tuple",
     "is_optional",
     "is_union",
     "not_none_type_arg",
     "is_type_var",
     "is_type_var_any",
     "is_class_var",
+    "is_final",
     "is_init_var",
     "get_class_that_defines_method",
     "get_class_that_defines_field",
     "is_dataclass_dict_mixin",
     "is_dataclass_dict_mixin_subclass",
     "collect_type_params",
     "resolve_type_params",
+    "substitute_type_params",
     "get_generic_name",
     "get_name_error_name",
     "is_dialect_subclass",
     "is_new_type",
     "is_annotated",
+    "get_type_annotations",
     "is_literal",
     "get_literal_values",
     "is_self",
     "is_required",
     "is_not_required",
     "get_function_arg_annotation",
     "get_function_return_annotation",
     "is_unpack",
     "is_type_var_tuple",
     "hash_type_args",
+    "iter_all_subclasses",
 ]
 
 
 NoneType = type(None)
 DataClassDictMixinPath = (
     f"{__name__.rsplit('.', 3)[:-3][0]}" f".mixins.dict.DataClassDictMixin"
 )
@@ -357,19 +366,23 @@
     for module in (typing, typing_extensions):
         with suppress(AttributeError):
             if type(typ) is getattr(module, "_AnnotatedAlias"):
                 return True
     return False
 
 
+def get_type_annotations(typ: Type) -> Sequence[Any]:
+    return getattr(typ, "__metadata__", [])
+
+
 def is_literal(typ: Type) -> bool:
-    if PY_37 or PY_38:
+    if PY_37 or PY_38 or PY_39:
         with suppress(AttributeError):
             return is_generic(typ) and get_generic_name(typ, True) == "Literal"
-    elif PY_39_MIN:
+    elif PY_310_MIN:
         with suppress(AttributeError):
             # noinspection PyProtectedMember
             # noinspection PyUnresolvedReferences
             return type(typ) is typing._LiteralGenericAlias  # type: ignore
     return False
 
 
@@ -400,14 +413,18 @@
         return True
 
 
 def is_class_var(typ: Type) -> bool:
     return get_type_origin(typ) is ClassVar
 
 
+def is_final(typ: Type) -> bool:
+    return get_type_origin(typ) is typing_extensions.Final
+
+
 def is_init_var(typ: Type) -> bool:
     if PY_37:
         return get_type_origin(typ) is dataclasses.InitVar
     elif PY_38_MIN:
         return isinstance(typ, dataclasses.InitVar)
     else:
         raise NotImplementedError
@@ -600,14 +617,31 @@
                 [resolved_type_params.get(a, a) for a in base_type_params]
             )
             result.update(resolve_type_params(base, base_type_args))
 
     return result
 
 
+def substitute_type_params(typ: Type, substitutions: Dict[Type, Type]) -> Type:
+    if is_annotated(typ):
+        origin = get_type_origin(typ)
+        subst = substitutions.get(origin, origin)
+        return typing_extensions.Annotated.__class_getitem__(  # type: ignore
+            (subst, *get_type_annotations(typ))
+        )
+    else:
+        new_type_args = []
+        for type_param in collect_type_params(typ):
+            new_type_args.append(substitutions.get(type_param, type_param))
+        if new_type_args:
+            with suppress(TypeError, KeyError):
+                return typ[tuple(new_type_args)]
+        return substitutions.get(typ, typ)
+
+
 def get_name_error_name(e: NameError) -> str:
     if PY_310_MIN:
         return e.name  # type: ignore
     else:
         match = re.search("'(.*)'", e.args[0])
         return match.group(1) if match else ""
 
@@ -678,7 +712,13 @@
 def is_variable_length_tuple(typ: Type) -> bool:
     type_args = get_args(typ)
     return len(type_args) == 2 and type_args[1] is Ellipsis
 
 
 def hash_type_args(type_args: typing.Iterable[typing.Type]) -> str:
     return md5(",".join(map(type_name, type_args)).encode()).hexdigest()
+
+
+def iter_all_subclasses(cls: Type) -> typing.Iterator[Type]:
+    for subclass in cls.__subclasses__():
+        yield subclass
+        yield from iter_all_subclasses(subclass)
```

### Comparing `mashumaro-3.7/mashumaro/core/meta/mixin.py` & `mashumaro-3.8/mashumaro/core/meta/mixin.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/core/meta/types/common.py` & `mashumaro-3.8/mashumaro/core/meta/types/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 import collections.abc
+import uuid
 from dataclasses import dataclass, field, is_dataclass, replace
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Mapping,
     Optional,
     Sequence,
     Type,
+    TypeVar,
 )
 
-from typing_extensions import TypeAlias
+try:
+    from functools import cached_property  # type: ignore
+except ImportError:
+    # for python 3.7
+    cached_property = property  # type: ignore
+
+from typing_extensions import ParamSpec, TypeAlias
 
 from mashumaro.core.const import PEP_585_COMPATIBLE
-from mashumaro.core.meta.helpers import get_type_origin, is_generic, type_name
+from mashumaro.core.meta.helpers import (
+    get_type_origin,
+    is_annotated,
+    is_generic,
+    type_name,
+)
 from mashumaro.exceptions import UnserializableDataError, UnserializableField
 
 if TYPE_CHECKING:  # pragma no cover
     from mashumaro.core.meta.code.builder import CodeBuilder
 else:
     CodeBuilder = Any
 
 
 NoneType = type(None)
 Expression: TypeAlias = str
 
+P = ParamSpec("P")
+T = TypeVar("T")
+
 
 class ExpressionWrapper:
     def __init__(self, expression: str):
         self.expression = expression
 
 
 PROPER_COLLECTION_TYPES: Dict[Type, str] = {
@@ -60,36 +76,46 @@
 class ValueSpec:
     type: Type
     origin_type: Type = field(init=False)
     expression: Expression
     builder: CodeBuilder
     field_ctx: FieldContext
     could_be_none: bool = True
+    annotated_type: Optional[Type] = None
 
     def __setattr__(self, key: str, value: Any) -> None:
         if key == "type":
             self.origin_type = get_type_origin(value)
         super().__setattr__(key, value)
 
     def copy(self, **changes: Any) -> "ValueSpec":
         return replace(self, **changes)
 
+    @cached_property
+    def annotations(self) -> Sequence[str]:
+        return getattr(self.annotated_type, "__metadata__", [])
+
 
 ValueSpecExprCreator: TypeAlias = Callable[[ValueSpec], Optional[Expression]]
 
 
 @dataclass
 class Registry:
     _registry: List[ValueSpecExprCreator] = field(default_factory=list)
 
     def register(self, function: ValueSpecExprCreator) -> ValueSpecExprCreator:
         self._registry.append(function)
         return function
 
     def get(self, spec: ValueSpec) -> Expression:
+        if is_annotated(spec.type):
+            spec.annotated_type = spec.builder._get_real_type(
+                spec.field_ctx.name, spec.type
+            )
+            spec.type = get_type_origin(spec.type)
         spec.type = spec.builder._get_real_type(spec.field_ctx.name, spec.type)
         spec.builder.add_type_modules(spec.type)
         for packer in self._registry:
             expr = packer(spec)
             if expr is not None:
                 return expr
         raise UnserializableField(
@@ -141,7 +167,15 @@
 
 
 def expr_or_maybe_none(spec: ValueSpec, new_expr: Expression) -> Expression:
     if spec.could_be_none:
         return f"{new_expr} if {spec.expression} is not None else None"
     else:
         return new_expr
+
+
+def random_hex() -> str:
+    return str(uuid.uuid4().hex)
+
+
+def clean_id(value: str) -> str:
+    return value.replace(".", "_")
```

### Comparing `mashumaro-3.7/mashumaro/core/meta/types/pack.py` & `mashumaro-3.8/mashumaro/core/meta/types/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 from typing import Any, Callable, List, Optional, Tuple, Type, Union
 
 import typing_extensions
 
 from mashumaro.core.const import PY_39_MIN, PY_311_MIN
 from mashumaro.core.meta.code.lines import CodeLines
 from mashumaro.core.meta.helpers import (
-    collect_type_params,
     get_args,
     get_class_that_defines_method,
     get_function_return_annotation,
     get_literal_values,
     is_dataclass_dict_mixin_subclass,
+    is_final,
     is_generic,
     is_literal,
     is_named_tuple,
     is_new_type,
     is_not_required,
     is_optional,
     is_required,
@@ -34,26 +34,28 @@
     is_type_var_any,
     is_type_var_tuple,
     is_typed_dict,
     is_union,
     is_unpack,
     not_none_type_arg,
     resolve_type_params,
+    substitute_type_params,
     type_name,
 )
 from mashumaro.core.meta.types.common import (
     Expression,
     ExpressionWrapper,
     NoneType,
     Registry,
     ValueSpec,
     ensure_generic_collection,
     ensure_generic_collection_subclass,
     ensure_generic_mapping,
     expr_or_maybe_none,
+    random_hex,
 )
 from mashumaro.exceptions import (
     UnserializableDataError,
     UnserializableField,
     UnsupportedSerializationEngine,
 )
 from mashumaro.helper import pass_through
@@ -81,23 +83,19 @@
     strategy_type = type(strategy)
     try:
         value_type: Union[Type, Any] = get_function_return_annotation(
             strategy.serialize
         )
     except (KeyError, ValueError):
         value_type = Any
-    resolved = resolve_type_params(strategy_type, get_args(spec.type))[
-        strategy_type
-    ]
-    new_type_args = []
-    for type_param in collect_type_params(value_type):
-        new_type_args.append(resolved.get(type_param, type_param))
-    with suppress(TypeError):
-        value_type = value_type[tuple(new_type_args)]
-    overridden_fn = f"__{spec.field_ctx.name}_serialize_{uuid.uuid4().hex}"
+    value_type = substitute_type_params(
+        value_type,
+        resolve_type_params(strategy_type, get_args(spec.type))[strategy_type],
+    )
+    overridden_fn = f"__{spec.field_ctx.name}_serialize_{random_hex()}"
     setattr(spec.builder.cls, overridden_fn, strategy.serialize)
     return PackerRegistry.get(
         spec.copy(
             type=value_type,
             expression=f"self.{overridden_fn}({spec.expression})",
         )
     )
@@ -105,15 +103,18 @@
 
 def get_overridden_serialization_method(
     spec: ValueSpec,
 ) -> Optional[Union[Callable, str, ExpressionWrapper]]:
     serialize_option = spec.field_ctx.metadata.get("serialize")
     if serialize_option is not None:
         return serialize_option
-    for typ in (spec.type, spec.origin_type):
+    checking_types = [spec.type, spec.origin_type]
+    if spec.annotated_type:
+        checking_types.insert(0, spec.annotated_type)
+    for typ in checking_types:
         for strategy in spec.builder.iter_serialization_strategies(
             spec.field_ctx.metadata, typ
         ):
             if strategy is pass_through:
                 return pass_through
             elif isinstance(strategy, dict):
                 serialize_option = strategy.get("serialize")
@@ -137,15 +138,15 @@
 ) -> Optional[Expression]:
     serialization_method = get_overridden_serialization_method(spec)
     if serialization_method is pass_through:
         return spec.expression
     elif isinstance(serialization_method, ExpressionWrapper):
         return serialization_method.expression
     elif callable(serialization_method):
-        overridden_fn = f"__{spec.field_ctx.name}_serialize_{uuid.uuid4().hex}"
+        overridden_fn = f"__{spec.field_ctx.name}_serialize_{random_hex()}"
         setattr(
             spec.builder.cls, overridden_fn, staticmethod(serialization_method)
         )
         return f"self.{overridden_fn}({spec.expression})"
 
 
 def _pack_annotated_serializable_type(
@@ -162,24 +163,20 @@
             field_name=spec.field_ctx.name,
             field_type=spec.type,
             holder_class=spec.builder.cls,
             msg="Method _serialize must have return annotation",
         ) from None
     if is_self(value_type):
         return f"{spec.expression}._serialize()"
-    args = get_args(value_type)
-    resolved = resolve_type_params(spec.origin_type, get_args(spec.type))[
-        spec.origin_type
-    ]
-    new_args = []
-    for arg in args:
-        new_args.append(resolved.get(arg, arg))
-    with suppress(TypeError):
-        # noinspection PyUnresolvedReferences
-        value_type = value_type[tuple(new_args)]
+    value_type = substitute_type_params(
+        value_type,
+        resolve_type_params(spec.origin_type, get_args(spec.type))[
+            spec.origin_type
+        ],
+    )
     return PackerRegistry.get(
         spec.copy(
             type=value_type,
             expression=f"{spec.expression}._serialize()",
         )
     )
 
@@ -236,43 +233,46 @@
             )
             builder.add_pack_method()
         flags = spec.builder.get_pack_method_flags(spec.type)
         return f"{spec.expression}.{method_name}({flags})"
 
 
 @register
+def pack_final(spec: ValueSpec) -> Optional[Expression]:
+    if is_final(spec.type):
+        return PackerRegistry.get(spec.copy(type=get_args(spec.type)[0]))
+
+
+@register
 def pack_any(spec: ValueSpec) -> Optional[Expression]:
     if spec.type is Any:
         return spec.expression
 
 
 def pack_union(
     spec: ValueSpec, args: Tuple[Type, ...], prefix: str = "union"
 ) -> Expression:
     lines = CodeLines()
     method_name = (
         f"__pack_{prefix}_{spec.builder.cls.__name__}_{spec.field_ctx.name}__"
-        f"{str(uuid.uuid4().hex)}"
+        f"{random_hex()}"
     )
     default_kwargs = spec.builder.get_pack_method_default_flag_values()
     if default_kwargs:
         lines.append(f"def {method_name}(self, value, {default_kwargs}):")
     else:
         lines.append(f"def {method_name}(self, value):")
     with lines.indent():
         for packer in (
             PackerRegistry.get(spec.copy(type=type_arg, expression="value"))
             for type_arg in args
         ):
-            lines.append("try:")
-            with lines.indent():
+            with lines.indent("try:"):
                 lines.append(f"return {packer}")
-            lines.append("except:")
-            with lines.indent():
-                lines.append("pass")
+            lines.append("except Exception: pass")
         field_type = type_name(
             spec.type,
             resolved_type_params=spec.builder.get_field_resolved_type_params(
                 spec.field_ctx.name
             ),
         )
         lines.append(
@@ -291,15 +291,15 @@
 
 
 def pack_literal(spec: ValueSpec) -> Expression:
     spec.builder.add_type_modules(spec.type)
     lines = CodeLines()
     method_name = (
         f"__pack_literal_{spec.builder.cls.__name__}_{spec.field_ctx.name}__"
-        f"{str(uuid.uuid4().hex)}"
+        f"{random_hex()}"
     )
     default_kwargs = spec.builder.get_pack_method_default_flag_values()
     if default_kwargs:
         lines.append(f"def {method_name}(self, value, {default_kwargs}):")
     else:
         lines.append(f"def {method_name}(self, value):")
     resolved_type_params = spec.builder.get_field_resolved_type_params(
@@ -312,25 +312,23 @@
                 spec.copy(type=value_type, expression="value")
             )
             if isinstance(literal_value, enum.Enum):
                 enum_type_name = type_name(
                     typ=value_type,
                     resolved_type_params=resolved_type_params,
                 )
-                lines.append(
+                with lines.indent(
                     f"if value == {enum_type_name}.{literal_value.name}:"
-                )
-                with lines.indent():
+                ):
                     lines.append(f"return {packer}")
             elif isinstance(  # type: ignore
                 literal_value,
                 (int, str, bytes, bool, NoneType),  # type: ignore
             ):
-                lines.append(f"if value == {literal_value!r}:")
-                with lines.indent():
+                with lines.indent(f"if value == {literal_value!r}:"):
                     lines.append(f"return {packer}")
         field_type = type_name(
             typ=spec.type,
             resolved_type_params=resolved_type_params,
         )
         lines.append(
             f"raise InvalidFieldValue('{spec.field_ctx.name}',"
@@ -588,15 +586,15 @@
     }
     all_keys = list(annotations.keys())
     required_keys = getattr(spec.type, "__required_keys__", all_keys)
     optional_keys = getattr(spec.type, "__optional_keys__", [])
     lines = CodeLines()
     method_name = (
         f"__pack_typed_dict_{spec.builder.cls.__name__}_"
-        f"{spec.field_ctx.name}__{str(uuid.uuid4().hex)}"
+        f"{spec.field_ctx.name}__{random_hex()}"
     )
     default_kwargs = spec.builder.get_pack_method_default_flag_values()
     if default_kwargs:
         lines.append(f"def {method_name}(self, value, {default_kwargs}):")
     else:
         lines.append(f"def {method_name}(self, value):")
     with lines.indent():
@@ -608,16 +606,15 @@
                     expression=f"value['{key}']",
                     could_be_none=True,
                 )
             )
             lines.append(f"d['{key}'] = {packer}")
         for key in sorted(optional_keys, key=all_keys.index):
             lines.append(f"key_value = value.get('{key}', MISSING)")
-            lines.append("if key_value is not MISSING:")
-            with lines.indent():
+            with lines.indent("if key_value is not MISSING:"):
                 packer = PackerRegistry.get(
                     spec.copy(
                         type=annotations[key],
                         expression="key_value",
                         could_be_none=True,
                     )
                 )
@@ -660,15 +657,15 @@
                     type=type_arg,
                     expression=v_name,
                     could_be_none=True,
                     field_ctx=spec.field_ctx.copy(metadata={}),
                 )
             )
 
-    if issubclass(spec.origin_type, typing.ByteString):
+    if issubclass(spec.origin_type, typing.ByteString):  # type: ignore
         spec.builder.ensure_object_imported(encodebytes)
         return f"encodebytes({spec.expression}).decode()"
     elif issubclass(spec.origin_type, str):
         return spec.expression
     elif issubclass(spec.origin_type, Tuple):  # type: ignore
         if is_named_tuple(spec.origin_type):
             return pack_named_tuple(spec)
```

### Comparing `mashumaro-3.7/mashumaro/core/meta/types/unpack.py` & `mashumaro-3.8/mashumaro/core/meta/types/unpack.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 import enum
 import ipaddress
 import os
 import pathlib
 import types
 import typing
 import uuid
+from abc import ABC, abstractmethod
 from base64 import decodebytes
 from contextlib import suppress
 from decimal import Decimal
 from fractions import Fraction
 from typing import Any, Callable, Iterable, List, Optional, Tuple, Type, Union
 
 import typing_extensions
 
 from mashumaro.core.const import PY_39_MIN, PY_311_MIN
 from mashumaro.core.helpers import parse_timezone
 from mashumaro.core.meta.code.lines import CodeLines
 from mashumaro.core.meta.helpers import (
-    collect_type_params,
     get_args,
     get_class_that_defines_method,
     get_function_arg_annotation,
     get_literal_values,
     is_dataclass_dict_mixin_subclass,
+    is_final,
     is_generic,
     is_literal,
     is_named_tuple,
     is_new_type,
     is_not_required,
     is_optional,
     is_required,
@@ -37,37 +38,42 @@
     is_special_typing_primitive,
     is_type_var,
     is_type_var_any,
     is_type_var_tuple,
     is_typed_dict,
     is_union,
     is_unpack,
+    iter_all_subclasses,
     not_none_type_arg,
     resolve_type_params,
+    substitute_type_params,
     type_name,
 )
 from mashumaro.core.meta.types.common import (
     Expression,
     ExpressionWrapper,
     NoneType,
     Registry,
     ValueSpec,
+    clean_id,
     ensure_generic_collection,
     ensure_generic_collection_subclass,
     ensure_generic_mapping,
     expr_or_maybe_none,
+    random_hex,
 )
 from mashumaro.exceptions import (
     ThirdPartyModuleNotFoundError,
     UnserializableDataError,
     UnserializableField,
     UnsupportedDeserializationEngine,
 )
 from mashumaro.helper import pass_through
 from mashumaro.types import (
+    Discriminator,
     GenericSerializableType,
     SerializableType,
     SerializationStrategy,
 )
 
 if PY_39_MIN:
     import zoneinfo
@@ -78,54 +84,398 @@
     ciso8601: Optional[types.ModuleType] = None  # type: ignore
 try:
     import pendulum
 except ImportError:  # pragma no cover
     pendulum: Optional[types.ModuleType] = None  # type: ignore
 
 
-__all__ = ["UnpackerRegistry"]
+__all__ = ["UnpackerRegistry", "SubtypeUnpackerBuilder"]
 
 
 UnpackerRegistry = Registry()
 register = UnpackerRegistry.register
 
 
+class AbstractUnpackerBuilder(ABC):
+    @abstractmethod
+    def get_method_prefix(self) -> str:  # pragma: no cover
+        raise NotImplementedError
+
+    def _generate_method_name(self, spec: ValueSpec) -> str:
+        prefix = self.get_method_prefix()
+        if prefix:
+            prefix = f"{prefix}_"
+        if spec.field_ctx.name:
+            suffix = f"_{spec.field_ctx.name}"
+        else:
+            suffix = ""
+        return (
+            f"__unpack_{prefix}{spec.builder.cls.__name__}{suffix}"
+            f"__{random_hex()}"
+        )
+
+    def _add_definition(self, spec: ValueSpec, lines: CodeLines) -> str:
+        method_name = self._generate_method_name(spec)
+        method_args = self._generate_method_args(spec)
+        lines.append("@classmethod")
+        lines.append(f"def {method_name}({method_args}):")
+        return method_name
+
+    def _get_extra_method_args(self) -> List[str]:
+        return []
+
+    def _generate_method_args(self, spec: ValueSpec) -> str:
+        default_kwargs = spec.builder.get_unpack_method_default_flag_values()
+        extra_args = self._get_extra_method_args()
+        if extra_args:
+            extra_args_str = f", {', '.join(extra_args)}"
+        else:
+            extra_args_str = ""
+        if default_kwargs:
+            return f"cls, value{extra_args_str}, {default_kwargs}"
+        else:  # pragma: no cover
+            # we shouldn't be here because there will be default_kwargs
+            return f"cls, value{extra_args_str}"
+
+    @abstractmethod
+    def _add_body(
+        self, spec: ValueSpec, lines: CodeLines
+    ) -> None:  # pragma: no cover
+        raise NotImplementedError
+
+    def _add_setattr(self, method_name: str, lines: CodeLines) -> None:
+        lines.append(f"setattr(cls, '{method_name}', {method_name})")
+
+    def _compile(self, spec: ValueSpec, lines: CodeLines) -> None:
+        if spec.builder.get_config().debug:
+            print(f"{type_name(spec.builder.cls)}:")
+            print(lines.as_text())
+        exec(lines.as_text(), spec.builder.globals, spec.builder.__dict__)
+
+    def _get_call_expr(self, spec: ValueSpec, method_name: str) -> str:
+        method_args = ", ".join(
+            filter(
+                None, (spec.expression, spec.builder.get_unpack_method_flags())
+            )
+        )
+        return f"cls.{method_name}({method_args})"
+
+    def _before_build(self, spec: ValueSpec) -> None:
+        pass
+
+    def build(self, spec: ValueSpec) -> str:
+        self._before_build(spec)
+        lines = CodeLines()
+        method_name = self._add_definition(spec, lines)
+        with lines.indent():
+            self._add_body(spec, lines)
+        self._add_setattr(method_name, lines)
+        self._compile(spec, lines)
+        return self._get_call_expr(spec, method_name)
+
+
+class UnionUnpackerBuilder(AbstractUnpackerBuilder):
+    def __init__(self, args: Tuple[Type, ...]):
+        self.union_args = args
+
+    def get_method_prefix(self) -> str:
+        return "union"
+
+    def _add_body(self, spec: ValueSpec, lines: CodeLines) -> None:
+        for unpacker in (
+            UnpackerRegistry.get(spec.copy(type=type_arg, expression="value"))
+            for type_arg in self.union_args
+        ):
+            with lines.indent("try:"):
+                lines.append(f"return {unpacker}")
+            lines.append("except Exception: pass")
+        field_type = type_name(
+            spec.type,
+            resolved_type_params=spec.builder.get_field_resolved_type_params(
+                spec.field_ctx.name
+            ),
+        )
+        lines.append(
+            f"raise InvalidFieldValue('{spec.field_ctx.name}',{field_type},"
+            f"value,cls)"
+        )
+
+
+class TypeVarUnpackerBuilder(UnionUnpackerBuilder):
+    def get_method_prefix(self) -> str:
+        return "type_var"
+
+
+class LiteralUnpackerBuilder(AbstractUnpackerBuilder):
+    def _before_build(self, spec: ValueSpec) -> None:
+        spec.builder.add_type_modules(spec.type)
+
+    def get_method_prefix(self) -> str:
+        return "literal"
+
+    def _add_body(self, spec: ValueSpec, lines: CodeLines) -> None:
+        for literal_value in get_literal_values(spec.type):
+            if isinstance(literal_value, enum.Enum):
+                enum_type_name = type_name(type(literal_value))
+                with lines.indent(
+                    f"if value == {enum_type_name}.{literal_value.name}.value:"
+                ):
+                    lines.append(
+                        f"return {enum_type_name}.{literal_value.name}"
+                    )
+            elif isinstance(literal_value, bytes):
+                unpacker = UnpackerRegistry.get(
+                    spec.copy(type=bytes, expression="value")
+                )
+                with lines.indent("try:"):
+                    with lines.indent(f"if {unpacker} == {literal_value!r}:"):
+                        lines.append(f"return {literal_value!r}")
+                lines.append("except Exception: pass")
+            elif isinstance(  # type: ignore
+                literal_value,
+                (int, str, bool, NoneType),  # type: ignore
+            ):
+                with lines.indent(f"if value == {literal_value!r}:"):
+                    lines.append(f"return {literal_value!r}")
+        lines.append("raise ValueError(value)")
+
+
+class DiscriminatedUnionUnpackerBuilder(AbstractUnpackerBuilder):
+    def __init__(
+        self,
+        discriminator: Discriminator,
+        base_variants: Optional[Tuple[Type, ...]] = None,
+    ):
+        self.discriminator = discriminator
+        self.base_variants = base_variants or tuple()
+        self._variants_attr: Optional[str] = None
+
+    def get_method_prefix(self) -> str:
+        return ""
+
+    def _get_extra_method_args(self) -> List[str]:
+        return ["_dialect", "_default_dialect"]
+
+    def _get_variants_attr(self, spec: ValueSpec) -> str:
+        if self._variants_attr is None:
+            self._variants_attr = (
+                f"__mashumaro_{spec.field_ctx.name}_variants_{random_hex()}__"
+            )
+        return self._variants_attr
+
+    def _get_variants_map(self, spec: ValueSpec) -> str:
+        variants_attr = self._get_variants_attr(spec)
+        return f"{type_name(spec.builder.cls)}.{variants_attr}"
+
+    def _get_variant_names(self, spec: ValueSpec) -> List[str]:
+        base_variants = self.base_variants or (spec.origin_type,)
+        variant_names: List[str] = []
+        if self.discriminator.include_subtypes:
+            spec.builder.ensure_object_imported(iter_all_subclasses)
+            variant_names.extend(
+                f"*iter_all_subclasses({type_name(base_variant)})"
+                for base_variant in base_variants
+            )
+        if self.discriminator.include_supertypes:
+            variant_names.extend(map(type_name, base_variants))
+        return variant_names
+
+    def _get_variant_names_iterable(self, spec: ValueSpec) -> str:
+        variant_names = self._get_variant_names(spec)
+        if len(variant_names) == 1:
+            if variant_names[0].startswith("*"):
+                return variant_names[0][1:]
+            else:
+                return f"[{variant_names[0]}]"
+        return f'({", ".join(variant_names)})'
+
+    @staticmethod
+    def _get_variants_attr_holder(spec: ValueSpec) -> Type:
+        return spec.builder.cls
+
+    @staticmethod
+    def _get_variant_method_call(method_name: str, spec: ValueSpec) -> str:
+        method_flags = spec.builder.get_unpack_method_flags()
+        if method_flags:
+            return f"{method_name}(value, {method_flags})"
+        else:
+            return f"{method_name}(value)"
+
+    def _add_body(self, spec: ValueSpec, lines: CodeLines) -> None:
+        discriminator = self.discriminator
+
+        variants_attr = self._get_variants_attr(spec)
+        variants_map = self._get_variants_map(spec)
+        variants_attr_holder = self._get_variants_attr_holder(spec)
+        variants = self._get_variant_names_iterable(spec)
+        variants_type_expr = type_name(spec.type)
+
+        if variants_attr not in variants_attr_holder.__dict__:
+            setattr(variants_attr_holder, variants_attr, {})
+        variant_method_name = spec.builder.get_unpack_method_name(
+            format_name=spec.builder.format_name
+        )
+        variant_method_call = self._get_variant_method_call(
+            variant_method_name, spec
+        )
+
+        if spec.builder.dialect:
+            spec.builder.ensure_object_imported(
+                spec.builder.dialect,
+                clean_id(type_name(spec.builder.dialect)),
+            )
+        if spec.builder.default_dialect:
+            spec.builder.ensure_object_imported(
+                spec.builder.default_dialect,
+                clean_id(type_name(spec.builder.default_dialect)),
+            )
+
+        if discriminator.field:
+            chosen_cls = f"{variants_map}[discriminator]"
+            with lines.indent("try:"):
+                lines.append(f"discriminator = value['{discriminator.field}']")
+            with lines.indent("except KeyError:"):
+                lines.append(
+                    f"raise MissingDiscriminatorError('{discriminator.field}')"
+                    f" from None"
+                )
+            with lines.indent("try:"):
+                lines.append(f"return {chosen_cls}.{variant_method_call}")
+            with lines.indent("except (KeyError, AttributeError):"):
+                lines.append(f"variants_map = {variants_map}")
+                with lines.indent(f"for variant in {variants}:"):
+                    with lines.indent("try:"):
+                        lines.append(
+                            f"variants_map[variant.__dict__["
+                            f"'{discriminator.field}']] = variant"
+                        )
+                    with lines.indent("except KeyError:"):
+                        lines.append("continue")
+                    spec.builder.ensure_object_imported(
+                        get_class_that_defines_method
+                    )
+                    lines.append(
+                        f"if get_class_that_defines_method("
+                        f"'{variant_method_name}',variant) != variant:"
+                    )
+                    with lines.indent():
+                        spec.builder.ensure_object_imported(
+                            spec.builder.__class__
+                        )
+                        lines.append(
+                            f"CodeBuilder(variant, "
+                            f"dialect=_dialect, "
+                            f"format_name={repr(spec.builder.format_name)}, "
+                            f"default_dialect=_default_dialect)"
+                            f".add_unpack_method()"
+                        )
+                with lines.indent("try:"):
+                    lines.append(
+                        f"return variants_map[discriminator]"
+                        f".{variant_method_call}"
+                    )
+                with lines.indent("except KeyError:"):
+                    lines.append(
+                        f"raise SuitableVariantNotFoundError("
+                        f"{variants_type_expr}, '{discriminator.field}', "
+                        f"discriminator) from None"
+                    )
+        else:
+            with lines.indent(f"for variant in {variants}:"):
+                with lines.indent("try:"):
+                    lines.append(f"return variant.{variant_method_call}")
+                with lines.indent("except AttributeError:"):
+                    spec.builder.ensure_object_imported(
+                        get_class_that_defines_method
+                    )
+                    lines.append(
+                        f"if get_class_that_defines_method("
+                        f"'{variant_method_name}',variant) != variant:"
+                    )
+                    with lines.indent():
+                        spec.builder.ensure_object_imported(
+                            spec.builder.__class__
+                        )
+                        lines.append(
+                            f"CodeBuilder(variant, "
+                            f"dialect=_dialect, "
+                            f"format_name={repr(spec.builder.format_name)}, "
+                            f"default_dialect=_default_dialect)"
+                            f".add_unpack_method()"
+                        )
+                        with lines.indent("try:"):
+                            lines.append(
+                                f"return variant.{variant_method_call}"
+                            )
+                        lines.append("except Exception: pass")
+                lines.append("except Exception: pass")
+            lines.append(
+                f"raise SuitableVariantNotFoundError({variants_type_expr}) "
+                f"from None"
+            )
+
+    def _get_call_expr(self, spec: ValueSpec, method_name: str) -> str:
+        method_args = ", ".join(
+            filter(
+                None,
+                (
+                    spec.expression,
+                    clean_id(type_name(spec.builder.dialect)),
+                    clean_id(type_name(spec.builder.default_dialect)),
+                    spec.builder.get_unpack_method_flags(),
+                ),
+            )
+        )
+        return f"cls.{method_name}({method_args})"
+
+
+class SubtypeUnpackerBuilder(DiscriminatedUnionUnpackerBuilder):
+    def _get_variants_attr(self, spec: ValueSpec) -> str:
+        if self._variants_attr is None:
+            assert self.discriminator.include_subtypes
+            self._variants_attr = "__mashumaro_subtype_variants__"
+        return self._variants_attr
+
+    def _get_variants_map(self, spec: ValueSpec) -> str:
+        variants_attr = self._get_variants_attr(spec)
+        return f"{type_name(spec.origin_type)}.{variants_attr}"
+
+
 def _unpack_with_annotated_serialization_strategy(
     spec: ValueSpec,
     strategy: SerializationStrategy,
 ) -> Expression:
     strategy_type = type(strategy)
     try:
         value_type: Union[Type, Any] = get_function_arg_annotation(
             strategy.deserialize,
             arg_pos=0,
         )
     except (KeyError, ValueError):
         value_type = Any
-    resolved = resolve_type_params(strategy_type, get_args(spec.type))[
-        strategy_type
-    ]
-    new_type_args = []
-    for type_param in collect_type_params(value_type):
-        new_type_args.append(resolved.get(type_param, type_param))
-    with suppress(TypeError):
-        value_type = value_type[tuple(new_type_args)]
-    overridden_fn = f"__{spec.field_ctx.name}_deserialize_{uuid.uuid4().hex}"
+    value_type = substitute_type_params(
+        value_type,
+        resolve_type_params(strategy_type, get_args(spec.type))[strategy_type],
+    )
+    overridden_fn = f"__{spec.field_ctx.name}_deserialize_{random_hex()}"
     setattr(spec.builder.cls, overridden_fn, strategy.deserialize)
     unpacker = UnpackerRegistry.get(spec.copy(type=value_type))
     return f"cls.{overridden_fn}({unpacker})"
 
 
 def get_overridden_deserialization_method(
     spec: ValueSpec,
 ) -> Optional[Union[Callable, str, ExpressionWrapper]]:
     deserialize_option = spec.field_ctx.metadata.get("deserialize")
     if deserialize_option is not None:
         return deserialize_option
-    for typ in (spec.type, spec.origin_type):
+    checking_types = [spec.type, spec.origin_type]
+    if spec.annotated_type:
+        checking_types.insert(0, spec.annotated_type)
+    for typ in checking_types:
         for strategy in spec.builder.iter_serialization_strategies(
             spec.field_ctx.metadata, typ
         ):
             if strategy is pass_through:
                 return pass_through
             elif isinstance(strategy, dict):
                 deserialize_option = strategy.get("deserialize")
@@ -148,17 +498,15 @@
 ) -> Optional[Expression]:
     deserialization_method = get_overridden_deserialization_method(spec)
     if deserialization_method is pass_through:
         return spec.expression
     elif isinstance(deserialization_method, ExpressionWrapper):
         return deserialization_method.expression
     elif callable(deserialization_method):
-        overridden_fn = (
-            f"__{spec.field_ctx.name}_deserialize_{uuid.uuid4().hex}"
-        )
+        overridden_fn = f"__{spec.field_ctx.name}_deserialize_{random_hex()}"
         setattr(spec.builder.cls, overridden_fn, deserialization_method)
         return f"cls.{overridden_fn}({spec.expression})"
 
 
 def _unpack_annotated_serializable_type(
     spec: ValueSpec,
 ) -> Optional[Expression]:
@@ -174,24 +522,20 @@
             field_name=spec.field_ctx.name,
             field_type=spec.type,
             holder_class=spec.builder.cls,
             msg='Method _deserialize must have annotated "value" argument',
         ) from None
     if is_self(value_type):
         return f"{type_name(spec.type)}._deserialize({spec.expression})"
-    type_args = get_args(value_type)
-    resolved = resolve_type_params(spec.origin_type, get_args(spec.type))[
-        spec.origin_type
-    ]
-    new_type_args = []
-    for type_arg in type_args:
-        new_type_args.append(resolved.get(type_arg, type_arg))
-    with suppress(TypeError):
-        # noinspection PyUnresolvedReferences
-        value_type = value_type[tuple(new_type_args)]
+    value_type = substitute_type_params(
+        value_type,
+        resolve_type_params(spec.origin_type, get_args(spec.type))[
+            spec.origin_type
+        ],
+    )
     unpacker = UnpackerRegistry.get(spec.copy(type=value_type))
     return f"{type_name(spec.type)}._deserialize({unpacker})"
 
 
 @register
 def unpack_serializable_type(spec: ValueSpec) -> Optional[Expression]:
     try:
@@ -219,14 +563,19 @@
 
 
 @register
 def unpack_dataclass_dict_mixin_subclass(
     spec: ValueSpec,
 ) -> Optional[Expression]:
     if is_dataclass_dict_mixin_subclass(spec.origin_type):
+        for annotation in spec.annotations:
+            if isinstance(annotation, Discriminator):
+                return DiscriminatedUnionUnpackerBuilder(annotation).build(
+                    spec
+                )
         type_args = get_args(spec.type)
         method_name = spec.builder.get_unpack_method_name(
             type_args, spec.builder.format_name
         )
         if get_class_that_defines_method(
             method_name, spec.origin_type
         ) != spec.origin_type and (
@@ -251,160 +600,73 @@
                 None,
                 (
                     spec.expression,
                     spec.builder.get_unpack_method_flags(spec.type),
                 ),
             )
         )
-        return f"{type_name(spec.origin_type)}.{method_name}({method_args})"
+        cls_alias = clean_id(type_name(spec.origin_type))
+        spec.builder.ensure_object_imported(spec.origin_type, cls_alias)
+        return f"{cls_alias}.{method_name}({method_args})"
+
+
+@register
+def unpack_final(spec: ValueSpec) -> Optional[Expression]:
+    if is_final(spec.type):
+        return UnpackerRegistry.get(spec.copy(type=get_args(spec.type)[0]))
 
 
 @register
 def unpack_any(spec: ValueSpec) -> Optional[Expression]:
     if spec.type is Any:
         return spec.expression
 
 
-def unpack_union(
-    spec: ValueSpec, args: Tuple[Type, ...], prefix: str = "union"
-) -> Expression:
-    lines = CodeLines()
-    method_name = (
-        f"__unpack_{prefix}_{spec.builder.cls.__name__}_"
-        f"{spec.field_ctx.name}__{str(uuid.uuid4().hex)}"
-    )
-    default_kwargs = spec.builder.get_unpack_method_default_flag_values()
-    lines.append("@classmethod")
-    if default_kwargs:
-        lines.append(f"def {method_name}(cls, value, {default_kwargs}):")
-    else:
-        lines.append(f"def {method_name}(cls, value):")
-    with lines.indent():
-        for unpacker in (
-            UnpackerRegistry.get(spec.copy(type=type_arg, expression="value"))
-            for type_arg in args
-        ):
-            lines.append("try:")
-            with lines.indent():
-                lines.append(f"return {unpacker}")
-            lines.append("except:")
-            with lines.indent():
-                lines.append("pass")
-        field_type = type_name(
-            spec.type,
-            resolved_type_params=spec.builder.get_field_resolved_type_params(
-                spec.field_ctx.name
-            ),
-        )
-        lines.append(
-            f"raise InvalidFieldValue('{spec.field_ctx.name}',{field_type},"
-            f"value,cls)"
-        )
-    lines.append(f"setattr(cls, '{method_name}', {method_name})")
-    if spec.builder.get_config().debug:
-        print(f"{type_name(spec.builder.cls)}:")
-        print(lines.as_text())
-    exec(lines.as_text(), spec.builder.globals, spec.builder.__dict__)
-    method_args = ", ".join(
-        filter(None, (spec.expression, spec.builder.get_unpack_method_flags()))
-    )
-    return f"cls.{method_name}({method_args})"
-
-
-def unpack_literal(spec: ValueSpec) -> Expression:
-    spec.builder.add_type_modules(spec.type)
-    lines = CodeLines()
-    method_name = (
-        f"__unpack_literal_{spec.builder.cls.__name__}_{spec.field_ctx.name}__"
-        f"{str(uuid.uuid4().hex)}"
-    )
-    default_kwargs = spec.builder.get_unpack_method_default_flag_values()
-    lines.append("@classmethod")
-    if default_kwargs:
-        lines.append(f"def {method_name}(cls, value, {default_kwargs}):")
-    else:
-        lines.append(f"def {method_name}(cls, value):")
-    with lines.indent():
-        for literal_value in get_literal_values(spec.type):
-            if isinstance(literal_value, enum.Enum):
-                enum_type_name = type_name(type(literal_value))
-                lines.append(
-                    f"if value == {enum_type_name}.{literal_value.name}.value:"
-                )
-                with lines.indent():
-                    lines.append(
-                        f"return {enum_type_name}.{literal_value.name}"
-                    )
-            elif isinstance(literal_value, bytes):
-                unpacker = UnpackerRegistry.get(
-                    spec.copy(type=bytes, expression="value")
-                )
-                lines.append("try:")
-                with lines.indent():
-                    lines.append(f"if {unpacker} == {literal_value!r}:")
-                    with lines.indent():
-                        lines.append(f"return {literal_value!r}")
-                lines.append("except:")
-                with lines.indent():
-                    lines.append("pass")
-            elif isinstance(  # type: ignore
-                literal_value,
-                (int, str, bool, NoneType),  # type: ignore
-            ):
-                lines.append(f"if value == {literal_value!r}:")
-                with lines.indent():
-                    lines.append(f"return {literal_value!r}")
-        lines.append("raise ValueError(value)")
-    lines.append(f"setattr(cls, '{method_name}', {method_name})")
-    if spec.builder.get_config().debug:
-        print(f"{type_name(spec.builder.cls)}:")
-        print(lines.as_text())
-    exec(lines.as_text(), spec.builder.globals, spec.builder.__dict__)
-    method_args = ", ".join(
-        filter(None, (spec.expression, spec.builder.get_unpack_method_flags()))
-    )
-    return f"cls.{method_name}({method_args})"
-
-
 @register
 def unpack_special_typing_primitive(spec: ValueSpec) -> Optional[Expression]:
     if is_special_typing_primitive(spec.origin_type):
         if is_union(spec.type):
             resolved_type_params = spec.builder.get_field_resolved_type_params(
                 spec.field_ctx.name
             )
             if is_optional(spec.type, resolved_type_params):
                 arg = not_none_type_arg(
                     get_args(spec.type), resolved_type_params
                 )
                 uv = UnpackerRegistry.get(spec.copy(type=arg))
                 return expr_or_maybe_none(spec, uv)
             else:
-                return unpack_union(spec, get_args(spec.type))
+                union_args = get_args(spec.type)
+                for annotation in spec.annotations:
+                    if isinstance(annotation, Discriminator):
+                        return DiscriminatedUnionUnpackerBuilder(
+                            annotation, union_args
+                        ).build(spec)
+                return UnionUnpackerBuilder(union_args).build(spec)
         elif spec.origin_type is typing.AnyStr:
             raise UnserializableDataError(
                 "AnyStr is not supported by mashumaro"
             )
         elif is_type_var_any(spec.type):
             return spec.expression
         elif is_type_var(spec.type):
             constraints = getattr(spec.type, "__constraints__")
             if constraints:
-                return unpack_union(spec, constraints, "type_var")
+                return TypeVarUnpackerBuilder(constraints).build(spec)
             else:
                 bound = getattr(spec.type, "__bound__")
                 # act as if it was Optional[bound]
                 uv = UnpackerRegistry.get(spec.copy(type=bound))
                 return expr_or_maybe_none(spec, uv)
         elif is_new_type(spec.type):
             return UnpackerRegistry.get(
                 spec.copy(type=spec.type.__supertype__)
             )
         elif is_literal(spec.type):
-            return unpack_literal(spec)
+            return LiteralUnpackerBuilder().build(spec)
         elif is_self(spec.type):
             method_name = spec.builder.get_unpack_method_name(
                 format_name=spec.builder.format_name
             )
             if (
                 get_class_that_defines_method(method_name, spec.builder.cls)
                 != spec.builder.cls
@@ -664,30 +926,29 @@
 
     if not defaults:
         return f"{type_name(spec.type)}({', '.join(unpackers)})"
 
     lines = CodeLines()
     method_name = (
         f"__unpack_named_tuple_{spec.builder.cls.__name__}_"
-        f"{spec.field_ctx.name}__{str(uuid.uuid4().hex)}"
+        f"{spec.field_ctx.name}__{random_hex()}"
     )
     lines.append("@classmethod")
     default_kwargs = spec.builder.get_unpack_method_default_flag_values()
     if default_kwargs:
         lines.append(f"def {method_name}(cls, value, {default_kwargs}):")
-    else:
+    else:  # pragma: no cover
+        # we shouldn't be here because there will be default_kwargs
         lines.append(f"def {method_name}(cls, value):")
     with lines.indent():
         lines.append("fields = []")
-        lines.append("try:")
-        with lines.indent():
+        with lines.indent("try:"):
             for unpacker in unpackers:
                 lines.append(f"fields.append({unpacker})")
-        lines.append("except IndexError:")
-        with lines.indent():
+        with lines.indent("except IndexError:"):
             lines.append("pass")
         lines.append(f"return {type_name(spec.type)}(*fields)")
     lines.append(f"setattr(cls, '{method_name}', {method_name})")
     if spec.builder.get_config().debug:
         print(f"{type_name(spec.builder.cls)}:")
         print(lines.as_text())
     exec(lines.as_text(), spec.builder.globals, spec.builder.__dict__)
@@ -707,37 +968,37 @@
     }
     all_keys = list(annotations.keys())
     required_keys = getattr(spec.type, "__required_keys__", all_keys)
     optional_keys = getattr(spec.type, "__optional_keys__", [])
     lines = CodeLines()
     method_name = (
         f"__unpack_typed_dict_{spec.builder.cls.__name__}_"
-        f"{spec.field_ctx.name}__{str(uuid.uuid4().hex)}"
+        f"{spec.field_ctx.name}__{random_hex()}"
     )
     default_kwargs = spec.builder.get_unpack_method_default_flag_values()
     lines.append("@classmethod")
     if default_kwargs:
         lines.append(f"def {method_name}(cls, value, {default_kwargs}):")
-    else:
+    else:  # pragma: no cover
+        # we shouldn't be here because there will be default_kwargs
         lines.append(f"def {method_name}(cls, value):")
     with lines.indent():
         lines.append("d = {}")
         for key in sorted(required_keys, key=all_keys.index):
             unpacker = UnpackerRegistry.get(
                 spec.copy(
                     type=annotations[key],
                     expression=f"value['{key}']",
                     could_be_none=True,
                 )
             )
             lines.append(f"d['{key}'] = {unpacker}")
         for key in sorted(optional_keys, key=all_keys.index):
             lines.append(f"key_value = value.get('{key}', MISSING)")
-            lines.append("if key_value is not MISSING:")
-            with lines.indent():
+            with lines.indent("if key_value is not MISSING:"):
                 unpacker = UnpackerRegistry.get(
                     spec.copy(
                         type=annotations[key],
                         expression="key_value",
                         could_be_none=True,
                     )
                 )
@@ -780,15 +1041,15 @@
                     type=type_arg,
                     expression=v_name,
                     could_be_none=True,
                     field_ctx=spec.field_ctx.copy(metadata={}),
                 )
             )
 
-    if issubclass(spec.origin_type, typing.ByteString):
+    if issubclass(spec.origin_type, typing.ByteString):  # type: ignore
         if spec.origin_type is bytes:
             spec.builder.ensure_object_imported(decodebytes)
             return f"decodebytes({spec.expression}.encode())"
         elif spec.origin_type is bytearray:
             spec.builder.ensure_object_imported(decodebytes)
             return f"bytearray(decodebytes({spec.expression}.encode()))"
     elif issubclass(spec.origin_type, str):
```

### Comparing `mashumaro-3.7/mashumaro/exceptions.py` & `mashumaro-3.8/mashumaro/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -121,14 +121,45 @@
             f"{repr(self.field_value)}"
         )
         if self.msg:
             s += f": {self.msg}"
         return s
 
 
+class MissingDiscriminatorError(LookupError):
+    def __init__(self, field_name: str):
+        self.field_name = field_name
+
+    def __str__(self) -> str:
+        return f"Discriminator '{self.field_name}' is missing"
+
+
+class SuitableVariantNotFoundError(ValueError):
+    def __init__(
+        self,
+        variants_type: Type,
+        discriminator_name: Optional[str] = None,
+        discriminator_value: Any = None,
+    ):
+        self.variants_type = variants_type
+        self.discriminator_name = discriminator_name
+        self.discriminator_value = discriminator_value
+
+    def __str__(self) -> str:
+        s = f"{type_name(self.variants_type)} has no "
+        if self.discriminator_value is not None:
+            s += (
+                f"subtype with attribute '{self.discriminator_name}' "
+                f"equal to {self.discriminator_value!r}"
+            )
+        else:
+            s += "suitable subtype"
+        return s
+
+
 class BadHookSignature(TypeError):
     pass
 
 
 class ThirdPartyModuleNotFoundError(ModuleNotFoundError):
     def __init__(self, module_name: str, field_name: str, holder_class: Type):
         self.module_name = module_name
```

### Comparing `mashumaro-3.7/mashumaro/helper.py` & `mashumaro-3.8/mashumaro/helper.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/jsonschema/annotations.py` & `mashumaro-3.8/mashumaro/jsonschema/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
-from numbers import Number
 from typing import Dict, Set
 
-from mashumaro.jsonschema.models import JSONSchema
+from mashumaro.jsonschema.models import JSONSchema, Number
 
 
 class Annotation:
     pass
 
 
 class Constraint(Annotation):
```

### Comparing `mashumaro-3.7/mashumaro/jsonschema/builder.py` & `mashumaro-3.8/mashumaro/jsonschema/builder.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/jsonschema/dialects.py` & `mashumaro-3.8/mashumaro/jsonschema/dialects.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/jsonschema/models.py` & `mashumaro-3.8/mashumaro/jsonschema/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import datetime
 import ipaddress
 from dataclasses import MISSING, dataclass, field
 from enum import Enum
-from numbers import Number
 from typing import Any, Dict, List, Optional, Set, Union
 
+from typing_extensions import TypeAlias
+
 from mashumaro.config import BaseConfig
 from mashumaro.helper import pass_through
 from mashumaro.jsonschema.dialects import DRAFT_2020_12, JSONSchemaDialect
 
 try:
     from mashumaro.mixins.orjson import (
         DataClassORJSONMixin as DataClassJSONMixin,
     )
 except ImportError:  # pragma no cover
     from mashumaro.mixins.json import DataClassJSONMixin  # type: ignore
 
 
+# https://github.com/python/mypy/issues/3186
+Number: TypeAlias = Union[int, float]
+
 Null = object()
 
 
 class JSONSchemaInstanceType(Enum):
     NULL = "null"
     BOOLEAN = "boolean"
     OBJECT = "object"
@@ -144,15 +148,16 @@
         serialize_by_alias = True
         aliases = {
             "schema": "$schema",
             "reference": "$ref",
             "definitions": "$defs",
         }
         serialization_strategy = {
-            Number: pass_through,
+            int: pass_through,
+            float: pass_through,
             Null: pass_through,
         }
 
     def __pre_serialize__(self) -> "JSONSchema":
         if self.const is None:
             self.const = Null
         if self.default is None:
```

### Comparing `mashumaro-3.7/mashumaro/jsonschema/schema.py` & `mashumaro-3.8/mashumaro/jsonschema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,15 @@
     if not issubclass(instance.origin_type, typing.Collection):
         return None
     elif issubclass(instance.origin_type, Enum):
         return None
 
     args = get_args(instance.type)
 
-    if issubclass(instance.origin_type, typing.ByteString):
+    if issubclass(instance.origin_type, typing.ByteString):  # type: ignore
         return JSONSchema(
             type=JSONSchemaInstanceType.STRING,
             format=JSONSchemaInstanceFormatExtension.BASE64,
         )
     elif issubclass(instance.origin_type, str):
         schema = JSONSchema(type=JSONSchemaInstanceType.STRING)
         for annotation in instance.annotations:
```

### Comparing `mashumaro-3.7/mashumaro/mixins/dict.py` & `mashumaro-3.8/mashumaro/mixins/dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,12 +50,19 @@
     def __pre_deserialize__(cls: Type[T], d: Dict[Any, Any]) -> Dict[Any, Any]:
         ...
 
     @classmethod
     def __post_deserialize__(cls: Type[T], obj: T) -> T:
         ...
 
-    def __pre_serialize__(self: T) -> T:
+    def __pre_serialize__(
+        self: T,
+        # context: Any = None,  # added with ADD_SERIALIZATION_CONTEXT option
+    ) -> T:
         ...
 
-    def __post_serialize__(self: T, d: Dict[Any, Any]) -> Dict[Any, Any]:
+    def __post_serialize__(
+        self: T,
+        d: Dict[Any, Any],
+        # context: Any = None,  # added with ADD_SERIALIZATION_CONTEXT option
+    ) -> Dict[Any, Any]:
         ...
```

### Comparing `mashumaro-3.7/mashumaro/mixins/json.py` & `mashumaro-3.8/mashumaro/mixins/json.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/mixins/msgpack.py` & `mashumaro-3.8/mashumaro/mixins/msgpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/mixins/orjson.py` & `mashumaro-3.8/mashumaro/mixins/orjson.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/mixins/orjson.pyi` & `mashumaro-3.8/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/mixins/toml.py` & `mashumaro-3.8/mashumaro/mixins/toml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/mixins/yaml.py` & `mashumaro-3.8/mashumaro/mixins/yaml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/mashumaro/types.py` & `mashumaro-3.8/mashumaro/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import decimal
+from dataclasses import dataclass
 from typing import Any, List, Optional, Type, Union
 
 from typing_extensions import Literal
 
 from mashumaro.core.const import Sentinel
 
 __all__ = [
     "SerializableType",
     "GenericSerializableType",
     "SerializationStrategy",
     "RoundedDecimal",
+    "Discriminator",
 ]
 
 
 class SerializableType:
     __use_annotations__ = False
 
     def __init_subclass__(
@@ -80,7 +82,21 @@
             else:
                 return str(value.quantize(self.exp))
         else:
             return str(value)
 
     def deserialize(self, value: str) -> decimal.Decimal:
         return decimal.Decimal(str(value))
+
+
+@dataclass(unsafe_hash=True)
+class Discriminator:
+    field: Optional[str] = None
+    include_supertypes: bool = False
+    include_subtypes: bool = False
+
+    def __post_init__(self) -> None:
+        if not self.include_supertypes and not self.include_subtypes:
+            raise ValueError(
+                "Either 'include_supertypes' or 'include_subtypes' "
+                "must be enabled"
+            )
```

### Comparing `mashumaro-3.7/mashumaro.egg-info/PKG-INFO` & `mashumaro-3.8/mashumaro.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.7
+Version: 3.8
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,23 +20,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: orjson
 Provides-Extra: msgpack
 Provides-Extra: yaml
 Provides-Extra: toml
 License-File: LICENSE
 
-# mashumaro
+<div align="center">
+
+<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+</div>
 
 When using dataclasses, you often need to dump and load objects based on the
 schema you have. Mashumaro not only lets you save and load things in different
 ways, but it also does it _super quick_.
 
 **Key features**
 * 🚀 One of the fastest libraries
@@ -82,23 +85,32 @@
         * [`aliases` config option](#aliases-config-option)
         * [`serialize_by_alias` config option](#serialize_by_alias-config-option)
         * [`omit_none` config option](#omit_none-config-option)
         * [`namedtuple_as_dict` config option](#namedtuple_as_dict-config-option)
         * [`allow_postponed_evaluation` config option](#allow_postponed_evaluation-config-option)
         * [`dialect` config option](#dialect-config-option)
         * [`orjson_options`](#orjson_options-config-option)
+        * [`discriminator` config option](#discriminator-config-option)
+        * [`lazy_compilation` config option](#lazy_compilation-config-option)
     * [Passing field values as is](#passing-field-values-as-is)
+    * [Extending existing types](#extending-existing-types)
     * [Dialects](#dialects)
       * [`serialization_strategy` dialect option](#serialization_strategy-dialect-option)
       * [`omit_none` dialect option](#omit_none-dialect-option)
       * [Changing the default dialect](#changing-the-default-dialect)
+    * [Discriminator](#discriminator)
+      * [Subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+      * [Subclasses without a common field](#subclasses-without-a-common-field)
+      * [Class level discriminator](#class-level-discriminator)
+      * [Working with union of classes](#working-with-union-of-classes)
     * [Code generation options](#code-generation-options)
         * [Add `omit_none` keyword argument](#add-omit_none-keyword-argument)
         * [Add `by_alias` keyword argument](#add-by_alias-keyword-argument)
         * [Add `dialect` keyword argument](#add-dialect-keyword-argument)
+        * [Add `context` keyword argument](#add-context-keyword-argument)
     * [Generic dataclasses](#generic-dataclasses)
       * [Generic dataclass inheritance](#generic-dataclass-inheritance)
       * [Generic dataclass in a field type](#generic-dataclass-in-a-field-type)
     * [`GenericSerializableType` interface](#genericserializabletype-interface)
     * [Serialization hooks](#serialization-hooks)
         * [Before deserialization](#before-deserialization)
         * [After deserialization](#after-deserialization)
@@ -188,14 +200,15 @@
 * [`Optional`](https://docs.python.org/3/library/typing.html#typing.Optional)
 * [`Union`](https://docs.python.org/3/library/typing.html#typing.Union)
 * [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar)
 * [`TypeVarTuple`](https://docs.python.org/3/library/typing.html#typing.TypeVarTuple)
 * [`NewType`](https://docs.python.org/3/library/typing.html#newtype)
 * [`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
 * [`Literal`](https://docs.python.org/3/library/typing.html#typing.Literal)
+* [`Final`](https://docs.python.org/3/library/typing.html#typing.Final)
 * [`Self`](https://docs.python.org/3/library/typing.html#typing.Self)
 * [`Unpack`](https://docs.python.org/3/library/typing.html#typing.Unpack)
 
 for standard interpreter types from [`types`](https://docs.python.org/3/library/types.html#standard-interpreter-types) module:
 * [`NoneType`](https://docs.python.org/3/library/types.html#types.NoneType)
 * [`UnionType`](https://docs.python.org/3/library/types.html#types.UnionType)
 
@@ -308,27 +321,40 @@
 specific parser and builder for exactly that schema, taking into account the
 specifics of the serialization format. This is much faster than inspection of
 field types on every call of parsing or building at runtime.
 
 These specific parsers and builders are presented by the corresponding
 `from_*` and `to_*` methods. They are compiled during import time (or at
 runtime in some cases) and are set as attributes to your dataclasses.
+To minimize the import time, you can explicitly enable
+[lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
 * macOS 13.0.1 Ventura
 * Apple M1
 * 8GB RAM
 * Python 3.11.0
 
 Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
 The following figures show the best overall time in each case.
 
-<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump.png" width="400">
+[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
+
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
+</picture>
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
+  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
+</picture>
 
 <table>
   <col>
   <colgroup span="2"></colgroup>
   <colgroup span="2"></colgroup>
   <tr>
     <th rowspan="2">Library</th>
@@ -339,51 +365,51 @@
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
     <th scope="col">Time</th>
     <th scope="col">Slowdown factor</th>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14791</td>
+    <td align="right">0.14724</td>
     <td align="left">1x</td>
-    <td align="right">0.10294</td>
+    <td align="right">0.10128</td>
     <td align="left">1x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18913</td>
+    <td align="right">0.18906</td>
     <td align="left">1.28x</td>
-    <td align="right">0.13879</td>
-    <td align="left">1.35x</td>
+    <td align="right">0.14072</td>
+    <td align="left">1.39x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">0.92652</td>
-    <td align="left">6.26x</td>
-    <td align="right">0.81281</td>
-    <td align="left">7.9x</td>
+    <td align="right">1.02666</td>
+    <td align="left">6.97x</td>
+    <td align="right">0.81932</td>
+    <td align="left">8.09x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38964</td>
-    <td align="left">9.39x</td>
-    <td align="right">0.45987</td>
-    <td align="left">4.47x</td>
+    <td align="right">1.38348</td>
+    <td align="left">9.4x</td>
+    <td align="right">0.45695</td>
+    <td align="left">4.51x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
     <td align="left">—</td>
     <td align="left">—</td>
-    <td align="right">0.68592</td>
-    <td align="left">6.66x</td>
+    <td align="right">0.68057</td>
+    <td align="left">6.72x</td>
 </tr>
 <tr>
     <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.40445</td>
-    <td align="left">16.26x</td>
+    <td align="right">2.37315</td>
+    <td align="left">16.12x</td>
     <td align="left">—</td>
     <td align="left">—</td>
 </tr>
 </table>
 
 To run benchmark in your environment:
 ```bash
@@ -584,15 +610,15 @@
 assert my_flight == Flight(JFK, LAX)
 assert my_flight.to_dict() == input_data
 ```
 
 You can see how `Airport` instances are seamlessly created from lists of two
 strings and serialized into them.
 
-By default `_deserialize` method will get raw input data without any 
+By default `_deserialize` method will get raw input data without any
 transformations before. This should be enough in many cases, especially when
 you need to perform non-standard transformations yourself, but let's extend
 our example:
 
 ```python
 class Itinerary(SerializableType):
     def __init__(self, flights):
@@ -1079,14 +1105,15 @@
 described below.
 
 | Constant                                                        | Description                                                          |
 |:----------------------------------------------------------------|:---------------------------------------------------------------------|
 | [`TO_DICT_ADD_OMIT_NONE_FLAG`](#add-omit_none-keyword-argument) | Adds `omit_none` keyword-only argument to `to_*` methods.            |
 | [`TO_DICT_ADD_BY_ALIAS_FLAG`](#add-by_alias-keyword-argument)   | Adds `by_alias` keyword-only argument to `to_*` methods.             |
 | [`ADD_DIALECT_SUPPORT`](#add-dialect-keyword-argument)          | Adds `dialect` keyword-only argument to `from_*` and `to_*` methods. |
+| [`ADD_SERIALIZATION_CONTEXT`](#add-context-keyword-argument)    | Adds `context` keyword-only argument to `to_*` methods.              |
 
 #### `serialization_strategy` config option
 
 You can register custom [`SerializationStrategy`](#serializationstrategy), `serialize` and `deserialize`
 methods for specific types just in one place. It could be configured using
 a dictionary with types as keys. The value could be either a
 [`SerializationStrategy`](#serializationstrategy) instance or a dictionary with `serialize` and
@@ -1128,14 +1155,18 @@
 
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
+Note that you can register different methods for multiple logical types which
+are based on the same type using `NewType` and `Annotated`.
+See [Extending existing types](#extending-existing-types) for details.
+
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
 ```python
@@ -1335,14 +1366,36 @@
 
     class Config(BaseConfig):
         orjson_options = orjson.OPT_NON_STR_KEYS
 
 assert MyClass({1: 2}).to_json() == {"1": 2}
 ```
 
+#### `discriminator` config option
+
+This option is described in the
+[Class level discriminator](#class-level-discriminator) section.
+
+#### `lazy_compilation` config option
+
+By using this option, the compilation of the `from_*` and `to_*` methods will
+be deferred until they are called first time. This will reduce the import time
+and, in certain instances, may enhance the speed of deserialization
+by leveraging the data that is accessible after the class has been created.
+
+> **Warning**
+>
+> If you need to save a reference to `from_*` or `to_*` method, you should
+> do it after the method is compiled. To be safe, you can always use lambda
+> function:
+> ```python
+> from_dict = lambda x: MyModel.from_dict(x)
+> to_dict = lambda x: x.to_dict()
+> ```
+
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
 [`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
@@ -1404,20 +1457,74 @@
 a2_dict = A2(my_class_instance).to_dict()
 a3_dict = A3(my_class_instance).to_dict()
 a4_dict = A4(my_class_instance).to_dict()
 
 assert a1_dict == a2_dict == a3_dict == a4_dict == {"x": my_class_instance}
 ```
 
+### Extending existing types
+
+There are situations where you might want some values of the same type to be
+treated as their own type. You can create new logical types with
+[`NewType`](https://docs.python.org/3/library/typing.html#newtype) or
+[`Annotated`](https://docs.python.org/3/library/typing.html#typing.Annotated)
+and register serialization strategies for them:
+
+```python
+from typing import Mapping, NewType, Annotated
+from dataclasses import dataclass
+from mashumaro import DataClassDictMixin
+
+SessionID = NewType("SessionID", str)
+AccountID = Annotated[str, "AccountID"]
+
+@dataclass
+class Context(DataClassDictMixin):
+    account_sessions: Mapping[AccountID, SessionID]
+
+    class Config:
+        serialization_strategy = {
+            AccountID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            },
+            SessionID: {
+                "deserialize": lambda x: ...,
+                "serialize": lambda x: ...,
+            }
+        }
+```
+
+Although using `NewType` is usually the most reliable way to avoid logical
+errors, you have to pay for it with notable overhead. If you are creating
+dataclass instances manually, then you know that type checkers will
+enforce you to enclose a value in your `"NewType"` callable, which leads
+to performance degradation:
+
+```python
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "MyInt(42)"
+10000000 loops, best of 5: 31.1 nsec per loop
+
+python -m timeit -s "from typing import NewType; MyInt = NewType('MyInt', int)" "42"
+50000000 loops, best of 5: 4.35 nsec per loop
+```
+
+However, when you create dataclass instances using the `from_*` method, there
+will be no performance degradation, because the value won't be enclosed in the
+callable in the generated code. Therefore, if performance is more important
+to you than catching logical errors by type checkers, and you are actively
+creating or changing dataclasses manually, then you should take a closer look
+at using `Annotated`.
+
 ### Dialects
 
 Sometimes it's needed to have different serialization and deserialization
 methods depending on the data source where entities of the dataclass are
 stored or on the API to which the entities are being sent or received from.
-There is a special Dialect type that may contain all the differences from the
+There is a special `Dialect` type that may contain all the differences from the
 default serialization and deserialization methods. You can create different
 dialects and use each of them for the same dataclass depending on
 the situation.
 
 Suppose we have the following dataclass with a field of type `date`:
 ```python
 @dataclass
@@ -1501,14 +1608,406 @@
         dialect = JapaneseDialect
 
 entity = Entity(date(2021, 12, 31))
 entity.to_dict()  # {'dt': '2021年12月31日'}
 assert Entity.from_dict({'dt': '2021年12月31日'}) == entity
 ```
 
+### Discriminator
+
+There is a special `Discriminator` class that allows you to customize how
+a union of dataclasses or their hierarchy will be deserialized.
+It has the following parameters that affects class selection rules:
+
+* `field` — optional name of the input dictionary key by which all the variants
+  can be distinguished
+* `include_subtypes` — allow to deserialize subclasses
+* `include_supertypes` — allow to deserialize superclasses
+
+Parameter `field` coule be in the following forms:
+
+* without annotations: `type = 42`
+* annotated as ClassVar: `type: ClassVar[int] = 42`
+* annotated as Final: `type: Final[int] = 42`
+* annotated as Literal: `type: Literal[42] = 42`
+* annotated as StrEnum: `type: ResponseType = ResponseType.OK`
+
+> **Note**
+>
+> Keep in mind that by default only Final, Literal and StrEnum fields are
+> processed during serialization.
+
+Next, we will look at different use cases, as well as their pros and cons.
+
+#### Subclasses distinguishable by a field
+
+Often you have a base dataclass and multiple subclasses that are easily
+distinguishable from each other by the value of a particular field.
+For example, there may be different events, messages or requests with
+a discriminator field "event_type", "message_type" or just "type". You could've
+listed all of them within `Union` type, but it would be too verbose and
+impractical. Moreover, deserialization of the union would be slow, since we
+need to iterate over each variant in the list until we find the right one.
+
+We can improve subclass deserialization using `Discriminator` as annotation
+within `Annotated` type. We will use `field` parameter and set
+`include_subtypes` to `True`.
+
+> **Note**
+>
+> The discriminator field should be accessible from the `__dict__` attribute
+> of a specific descendant, i.e. defined at the level of that descendant.
+> A descendant class without a discriminator field will be ignored, but
+> its descendants won't.
+
+Suppose we have a hierarchy of client events distinguishable by a class
+attribute "type":
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from mashumaro import DataClassDictMixin
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    pass
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+```
+
+We use base dataclass `ClientEvent` for a field of another dataclass:
+
+```python
+from typing import Annotated, List
+# or from typing_extensions import Annotated
+from mashumaro.types import Discriminator
+
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[
+        Annotated[
+            ClientEvent, Discriminator(field="type", include_subtypes=True)
+        ]
+    ]
+```
+
+Now we can deserialize events based on "type" value:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+#### Subclasses without a common field
+
+In rare cases you have to deal with subclasses that don't have a common field
+name which they can be distinguished by. Since `Discriminator` can be
+initialized without "field" parameter you can use it with only
+`include_subclasses` enabled. The drawback is that we will have to go through all
+the subclasses until we find the suitable one. It's almost like using `Union`
+type but with subclasses support.
+
+Suppose we're making a brunch. We have some ingredients:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+@dataclass
+class Hummus(Ingredient):
+    made_of: Literal["chickpeas", "beet", "artichoke"]
+    grams: int
+
+@dataclass
+class Celery(Ingredient):
+    pieces: int
+```
+
+Let's create a plate:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[Ingredient, Discriminator(include_subtypes=True)]
+    ]
+```
+
+And now we can put our ingredients on the plate:
+
+```python
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+    ]
+)
+```
+
+In some cases it's necessary to fall back to the base class if there is no
+suitable subclass. We can set `include_supertypes` to `True`:
+
+```python
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Ingredient,
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {
+                "name": "hummus from the shop",
+                "made_of": "chickpeas",
+                "grams": 150,
+            },
+            {"name": "celery from my garden", "pieces": 5},
+            {"name": "cumin"}  # <- new unknown ingredient
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        Hummus(name="hummus from the shop", made_of="chickpeas", grams=150),
+        Celery(name="celery from my garden", pieces=5),
+        Ingredient(name="cumin"),  # <- unknown ingredient added
+    ]
+)
+```
+
+#### Class level discriminator
+
+It may often be more convenient to specify a `Discriminator` once at the class
+level and use that class without `Annotated` type for subclass deserialization.
+Depending on the `Discriminator` parameters, it can be used as a replacement for
+[subclasses distinguishable by a field](#subclasses-distinguishable-by-a-field)
+as well as for [subclasses without a common field](#subclasses-without-a-common-field).
+The only difference is that you can't use `include_supertypes=True` because
+it would lead to a recursion error.
+
+Reworked example will look like this:
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from typing import List
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig
+from mashumaro.types import Discriminator
+
+@dataclass
+class ClientEvent(DataClassDictMixin):
+    class Config(BaseConfig):
+        discriminator = Discriminator(  # <- add discriminator
+            field="type",
+            include_subtypes=True,
+        )
+
+@dataclass
+class ClientConnectedEvent(ClientEvent):
+    type = "connected"
+    client_ip: IPv4Address
+
+@dataclass
+class ClientDisconnectedEvent(ClientEvent):
+    type = "disconnected"
+    client_ip: IPv4Address
+
+@dataclass
+class AggregatedEvents(DataClassDictMixin):
+    list: List[ClientEvent]  # <- use base class here
+```
+
+And now we can deserialize events based on "type" value as we did earlier:
+
+```python
+events = AggregatedEvents.from_dict(
+    {
+        "list": [
+            {"type": "connected", "client_ip": "10.0.0.42"},
+            {"type": "disconnected", "client_ip": "10.0.0.42"},
+        ]
+    }
+)
+assert events == AggregatedEvents(
+    list=[
+        ClientConnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+        ClientDisconnectedEvent(client_ip=IPv4Address("10.0.0.42")),
+    ]
+)
+```
+
+What's more interesting is that you can now deserialize subclasses simply by
+calling the superclass `from_*` method, which is very useful:
+```python
+disconnected_event = ClientEvent.from_dict(
+    {"type": "disconnected", "client_ip": "10.0.0.42"}
+)
+assert disconnected_event == ClientDisconnectedEvent(IPv4Address("10.0.0.42"))
+```
+
+The same is applicable for subclasses without a common field:
+
+```python
+@dataclass
+class Ingredient(DataClassDictMixin):
+    name: str
+
+    class Config:
+        discriminator = Discriminator(include_subtypes=True)
+
+...
+
+celery = Ingredient.from_dict({"name": "celery from my garden", "pieces": 5})
+assert celery == Celery(name="celery from my garden", pieces=5)
+```
+
+#### Working with union of classes
+
+Deserialization of union of types distinguishable by a particular field will
+be much faster using `Discriminator` because there will be no traversal
+of all classes and an attempt to deserialize each of them.
+Usually this approach can be used when you have multiple classes without a
+common superclass or when you only need to deserialize some of the subclasses.
+In the following example we will use `include_supertypes=True` to
+deserialize two subclasses out of three:
+
+```python
+from dataclasses import dataclass
+from typing import Annotated, Literal, Union
+# or from typing_extensions import Annotated
+from mashumaro import DataClassDictMixin
+from mashumaro.types import Discriminator
+
+@dataclass
+class Event(DataClassDictMixin):
+    pass
+
+@dataclass
+class Event1(Event):
+    code: Literal[1] = 1
+    ...
+
+@dataclass
+class Event2(Event):
+    code: Literal[2] = 2
+    ...
+
+@dataclass
+class Event3(Event):
+    code: Literal[3] = 3
+    ...
+
+@dataclass
+class Message(DataClassDictMixin):
+    event: Annotated[
+        Union[Event1, Event2],
+        Discriminator(field="code", include_supertypes=True),
+    ]
+
+event1_msg = Message.from_dict({"event": {"code": 1, ...}})
+event2_msg = Message.from_dict({"event": {"code": 2, ...}})
+assert isinstance(event1_msg.event, Event1)
+assert isinstance(event2_msg.event, Event2)
+
+# raises InvalidFieldValue:
+Message.from_dict({"event": {"code": 3, ...}})
+```
+
+Again, it's not necessary to have a common superclass. If you have a union of
+dataclasses without a field that they can be distinguishable by, you can still
+use `Discriminator`, but deserialization will almost be the same as for `Union`
+type without `Discriminator` except that it could be possible to deserialize
+subclasses with `include_subtypes=True`.
+
+> **Note**
+>
+> When both `include_subtypes` and `include_supertypes` are enabled,
+> all subclasses will be attempted to be deserialized first,
+> superclasses — at the end.
+
+```python
+@dataclass
+class Hummus(DataClassDictMixin):
+    made_of: Literal["chickpeas", "artichoke"]
+    grams: int
+
+@dataclass
+class ChickpeaHummus(Hummus):
+    made_of: Literal["chickpeas"]
+
+@dataclass
+class Celery(DataClassDictMixin):
+    pieces: int
+
+@dataclass
+class Plate(DataClassDictMixin):
+    ingredients: List[
+        Annotated[
+            Union[Hummus, Celery],
+            Discriminator(include_subtypes=True, include_supertypes=True),
+        ]
+    ]
+
+plate = Plate.from_dict(
+    {
+        "ingredients": [
+            {"made_of": "chickpeas", "grams": 100},
+            {"made_of": "artichoke", "grams": 50},
+            {"pieces": 4},
+        ]
+    }
+)
+assert plate == Plate(
+    ingredients=[
+        ChickpeaHummus(made_of='chickpeas', grams=100),  # <- subclass
+        Hummus(made_of='artichoke', grams=50),  # <- superclass
+        Celery(pieces=4),
+    ]
+)
+```
+
 ### Code generation options
 
 #### Add `omit_none` keyword argument
 
 If you want to have control over whether to skip `None` values on serialization
 you can add `omit_none` parameter to `to_*` methods using the
 `code_generation_options` list. The default value of `omit_none`
@@ -1575,14 +2074,94 @@
 class Entity(DataClassDictMixin):
     dt: date
 
     class Config(BaseConfig):
         code_generation_options = [ADD_DIALECT_SUPPORT]
 ```
 
+#### Add `context` keyword argument
+
+Sometimes it's needed to pass a "context" object to the serialization hooks
+that will take it into account. For example, you could want to have an option
+to remove sensitive data from the serialization result if you need to.
+You can add `context` parameter to `to_*` methods that will be passed to
+[`__pre_serialize__`](#before-serialization) and
+[`__post_serialize__`](#after-serialization) hooks. The type of this context
+as well as its mutability is up to you.
+
+```python
+from dataclasses import dataclass
+from typing import Dict, Optional
+from uuid import UUID
+from mashumaro import DataClassDictMixin
+from mashumaro.config import BaseConfig, ADD_SERIALIZATION_CONTEXT
+
+class BaseModel(DataClassDictMixin):
+    class Config(BaseConfig):
+        code_generation_options = [ADD_SERIALIZATION_CONTEXT]
+
+@dataclass
+class Account(BaseModel):
+    id: UUID
+    username: str
+    name: str
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["username"] = "***"
+            d["name"] = "***"
+        return d
+
+@dataclass
+class Session(BaseModel):
+    id: UUID
+    key: str
+    account: Account
+
+    def __pre_serialize__(self, context: Optional[Dict] = None):
+        return self
+
+    def __post_serialize__(self, d: Dict, context: Optional[Dict] = None):
+        if context and context.get("remove_sensitive_data"):
+            d["key"] = "***"
+        return d
+
+
+foo = Session(
+    id=UUID('03321c9f-6a97-421e-9869-918ff2867a71'),
+    key="VQ6Q9bX4c8s",
+    account=Account(
+        id=UUID('4ef2baa7-edef-4d6a-b496-71e6d72c58fb'),
+        username="john_doe",
+        name="John"
+    )
+)
+assert foo.to_dict() == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': 'VQ6Q9bX4c8s',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': 'john_doe',
+        'name': 'John'
+    }
+}
+assert foo.to_dict(context={"remove_sensitive_data": True}) == {
+    'id': '03321c9f-6a97-421e-9869-918ff2867a71',
+    'key': '***',
+    'account': {
+        'id': '4ef2baa7-edef-4d6a-b496-71e6d72c58fb',
+        'username': '***',
+        'name': '***'
+    }
+}
+```
+
 ### Generic dataclasses
 
 Along with [user-defined generic types](#user-defined-generic-types)
 implementing `SerializableType` interface, generic and variadic
 generic dataclasses can also be used. There are two applicable scenarios
 for them.
 
@@ -1765,14 +2344,17 @@
 
 obj = DataClass(abc=123)
 obj.to_dict()
 obj.to_json()
 print(obj.counter)  # 2
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 #### After serialization
 
 For doing something with a dictionary that was created as a result of
 serialization you can use `__post_serialize__` method:
 
 ```python
 @dataclass
@@ -1785,14 +2367,17 @@
         return d
 
 obj = DataClass(user="name", password="secret")
 print(obj.to_dict())  # {"user": "name"}
 print(obj.to_json())  # '{"user": "name"}'
 ```
 
+Note that you can add an additional `context` argument using the
+[corresponding](#add-context-keyword-argument) code generation option.
+
 JSON Schema
 --------------------------------------------------------------------------------
 
 You can build JSON Schema not only for dataclasses but also for any other
 [supported](#supported-data-types) data
 types. There is support for the following standards:
 * [Draft 2022-12](https://json-schema.org/specification.html)
```

### Comparing `mashumaro-3.7/mashumaro.egg-info/SOURCES.txt` & `mashumaro-3.8/mashumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/pyproject.toml` & `mashumaro-3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mashumaro-3.7/setup.py` & `mashumaro-3.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="mashumaro",
-    version="3.7",
+    version="3.8",
     description="Fast serialization library on top of dataclasses",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
```

