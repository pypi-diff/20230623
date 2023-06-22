# Comparing `tmp/tensorstore-0.1.8.tar.gz` & `tmp/tensorstore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorstore-0.1.8.tar", last modified: Mon Nov 30 23:09:33 2020, max compression
+gzip compressed data, was "dist/tensorstore-0.1.9.tar", last modified: Wed Jan 13 22:04:08 2021, max compression
```

## Comparing `tensorstore-0.1.8.tar` & `tensorstore-0.1.9.tar`

### file list

```diff
@@ -1,1106 +1,973 @@
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      888 2020-04-29 01:47:28.000000 tensorstore-0.1.8/.bazelrc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)        6 2020-08-25 23:48:07.000000 tensorstore-0.1.8/.bazelversion
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       76 2020-04-18 03:06:59.000000 tensorstore-0.1.8/.clang-format
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      244 2020-04-18 03:06:59.000000 tensorstore-0.1.8/.gitignore
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       33 2020-04-18 03:06:59.000000 tensorstore-0.1.8/.style.yapf
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      303 2020-04-18 03:06:59.000000 tensorstore-0.1.8/AUTHORS
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      153 2020-04-29 01:47:28.000000 tensorstore-0.1.8/BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1097 2020-04-18 03:06:59.000000 tensorstore-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12627 2020-04-18 03:06:59.000000 tensorstore-0.1.8/LICENSE
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      300 2020-11-30 23:09:33.024689 tensorstore-0.1.8/PKG-INFO
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      803 2020-04-18 03:06:59.000000 tensorstore-0.1.8/README.md
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      191 2020-04-18 03:06:59.000000 tensorstore-0.1.8/WORKSPACE
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)    11342 2020-04-18 03:06:59.000000 tensorstore-0.1.8/bazelisk.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.920689 tensorstore-0.1.8/docs/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.924689 tensorstore-0.1.8/docs/_static/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1097 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/_static/sphinx_rtd_theme_table_word_wrap_fix.css
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.924689 tensorstore-0.1.8/docs/_templates/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.924689 tensorstore-0.1.8/docs/_templates/autosummary/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      106 2020-04-18 03:07:00.000000 tensorstore-0.1.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      539 2020-04-18 03:07:00.000000 tensorstore-0.1.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      693 2020-04-18 03:07:00.000000 tensorstore-0.1.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      678 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/_templates/autosummary_root_module.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2944 2020-04-29 01:47:28.000000 tensorstore-0.1.8/docs/conf.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      640 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/context.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4482 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/context_schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      132 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/docutils.conf
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4528 2020-08-25 23:48:07.000000 tensorstore-0.1.8/docs/environment.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      323 2020-08-25 23:48:07.000000 tensorstore-0.1.8/docs/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10559 2020-11-30 23:09:09.000000 tensorstore-0.1.8/docs/index_space.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6485 2020-04-29 01:47:28.000000 tensorstore-0.1.8/docs/index_transform_schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6207 2020-08-25 23:48:07.000000 tensorstore-0.1.8/docs/installation.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      699 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/overview.rst
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.924689 tensorstore-0.1.8/docs/python/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.924689 tensorstore-0.1.8/docs/python/api/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      169 2020-04-18 03:07:00.000000 tensorstore-0.1.8/docs/python/api/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      107 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/python/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    41153 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/python/indexing.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7705 2020-08-25 23:48:07.000000 tensorstore-0.1.8/docs/python/tutorial.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      310 2020-04-29 01:47:28.000000 tensorstore-0.1.8/docs/spec.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1553 2020-04-18 03:06:59.000000 tensorstore-0.1.8/docs/tensorstore_schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4651 2020-06-29 03:39:51.000000 tensorstore-0.1.8/external.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.912689 tensorstore-0.1.8/python/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.928689 tensorstore-0.1.8/python/tensorstore/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12693 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11418 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/LICENSE
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1278 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/__init__.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13652 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/array_type_caster.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11060 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/array_type_caster.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1313 2020-04-29 01:47:28.000000 tensorstore-0.1.8/python/tensorstore/bazel_pytest_main.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17088 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/context.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4724 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/context.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6650 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/data_type.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7225 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/data_type.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20053 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/dim_expression.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5777 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/dim_expression.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8025 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/future.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10441 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/future.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2502 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/index.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5903 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/index.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    47335 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/index_space.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11850 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/index_space.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4502 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/index_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    45208 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/indexing_spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13625 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/indexing_spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1414 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/intrusive_ptr_holder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6417 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/json_type_caster.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2237 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/json_type_caster.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4178 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/pybind11.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1331 2020-05-28 22:28:53.000000 tensorstore-0.1.8/python/tensorstore/pytest.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3774 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/result_type_caster.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      853 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/shell.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5657 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1564 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2243 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/status.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2113 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/status.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4378 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/subscript_method.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2251 2020-10-10 00:09:50.000000 tensorstore-0.1.8/python/tensorstore/tensorstore.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12750 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tensorstore_class.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1098 2020-04-18 03:06:59.000000 tensorstore-0.1.8/python/tensorstore/tensorstore_class.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.928689 tensorstore-0.1.8/python/tensorstore/tests/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3690 2020-07-29 01:03:09.000000 tensorstore-0.1.8/python/tensorstore/tests/context_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3758 2020-04-29 01:47:28.000000 tensorstore-0.1.8/python/tensorstore/tests/data_type_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21043 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tests/dim_expression_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1636 2020-04-29 01:47:28.000000 tensorstore-0.1.8/python/tensorstore/tests/future_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5671 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tests/index_domain_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2859 2020-04-29 01:47:28.000000 tensorstore-0.1.8/python/tensorstore/tests/index_interval_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4491 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tests/index_transform_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6101 2020-04-29 01:47:28.000000 tensorstore-0.1.8/python/tensorstore/tests/indexing_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2959 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tests/spec_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7262 2020-11-30 23:09:09.000000 tensorstore-0.1.8/python/tensorstore/tests/tensorstore_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4811 2020-10-10 00:09:50.000000 tensorstore-0.1.8/python/tensorstore/tests/transaction_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8466 2020-10-10 00:09:50.000000 tensorstore-0.1.8/python/tensorstore/transaction.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1697 2020-10-10 00:09:50.000000 tensorstore-0.1.8/python/tensorstore/transaction.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2493 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/write_futures.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2055 2020-06-29 03:39:52.000000 tensorstore-0.1.8/python/tensorstore/write_futures.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.928689 tensorstore-0.1.8/python/tensorstore.egg-info/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      300 2020-11-30 23:09:32.000000 tensorstore-0.1.8/python/tensorstore.egg-info/PKG-INFO
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    38285 2020-11-30 23:09:32.000000 tensorstore-0.1.8/python/tensorstore.egg-info/SOURCES.txt
--rw-r--r--   0 jbms     (297878) primarygroup (89939)        1 2020-11-30 23:09:32.000000 tensorstore-0.1.8/python/tensorstore.egg-info/dependency_links.txt
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       14 2020-11-30 23:09:32.000000 tensorstore-0.1.8/python/tensorstore.egg-info/requires.txt
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       37 2020-11-30 23:09:32.000000 tensorstore-0.1.8/python/tensorstore.egg-info/top_level.txt
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       38 2020-11-30 23:09:33.024689 tensorstore-0.1.8/setup.cfg
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3250 2020-04-29 01:47:28.000000 tensorstore-0.1.8/setup.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.936689 tensorstore-0.1.8/tensorstore/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16338 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7448 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    77732 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2050 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/array_nc_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    65319 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7580 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/array_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8782 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/array_testutil_matches_array.inc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6493 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/array_testutil_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1399 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/box.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    30651 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/box.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    25021 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/box_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3933 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/cast.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      935 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/container_kind.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20451 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/context.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11365 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/context.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6638 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/context_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10720 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/context_impl_base.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8060 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/context_resource_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17491 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/context_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1491 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/contiguous_layout.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2145 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/contiguous_layout.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1991 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/contiguous_layout_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14673 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/data_type.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    38274 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/data_type.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19708 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/data_type_conversion.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    36812 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/data_type_conversion_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15163 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/data_type_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.940689 tensorstore-0.1.8/tensorstore/driver/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6233 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/BUILD
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.940689 tensorstore-0.1.8/tensorstore/driver/array/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1647 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/array/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14569 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/array/array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2976 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/array/array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    35884 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/array/array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      371 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/array/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      714 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/array/schema.yml
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.940689 tensorstore-0.1.8/tensorstore/driver/cast/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1326 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/cast/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12304 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/cast/cast.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4667 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/cast/cast.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21276 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/cast/cast_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      610 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/cast/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      761 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/cast/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9213 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/chunk.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    45328 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    25715 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/driver.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3032 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/driver_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    29405 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/driver_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6418 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/driver_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      490 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/index.rst
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.940689 tensorstore-0.1.8/tensorstore/driver/json/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2436 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19524 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15041 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/driver_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      817 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6227 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/json_change_map.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3921 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/json_change_map.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7822 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/json_change_map_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3548 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/json/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    56918 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    32534 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6241 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5051 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6641 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7460 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2009 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/blosc_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7021 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/n5/blosc_compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1524 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/bzip2_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3996 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/n5/bzip2_compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1881 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1214 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1231 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/compressor_registry.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14334 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    38892 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/driver_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2513 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/golden_file_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2114 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/gzip_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4663 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/n5/gzip_compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      898 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19766 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/metadata.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5229 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/metadata.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12405 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/metadata_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6138 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/n5/schema.yml
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/0/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/0/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/0/1
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/1/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/1/1
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      266 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/blosc/attributes.json
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/0/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       54 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/0/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       55 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/0/1
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       56 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/1/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       56 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/1/1
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      199 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/bzip2/attributes.json
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1548 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/generate.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/0/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/0/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/0/1
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/1/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/1/1
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      220 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/gzip/attributes.json
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/0/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/0/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/0/1
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.944689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/1/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/1/1
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      173 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/raw/attributes.json
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.948689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.948689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/0/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/0/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/0/1
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.948689 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/1/0
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/1/1
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      193 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/testdata/xz/attributes.json
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1541 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/n5/xz_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4138 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/n5/xz_compressor_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.948689 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9435 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13058 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2582 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3906 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    26138 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    67149 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/driver_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3446 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    41729 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11277 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    77881 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2184 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1434 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3171 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9457 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8508 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6580 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8493 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3553 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3719 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6444 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7209 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8237 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    43962 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5262 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    67224 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14203 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13611 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/registry.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.952689 tensorstore-0.1.8/tensorstore/driver/zarr/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8723 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/zarr/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2473 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/blosc_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12385 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/zarr/blosc_compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1548 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/bzip2_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4544 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/zarr/bzip2_compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1787 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1225 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1243 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/compressor_registry.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2387 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/compressor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17590 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/driver/zarr/driver.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1579 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/driver/zarr/driver_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16799 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/zarr/driver_impl_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    84001 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/driver/zarr/driver_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10656 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/dtype.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5080 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/dtype.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12994 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/dtype_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1238 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19055 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/zarr/metadata.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8948 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/zarr/metadata.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    29898 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tensorstore/driver/zarr/metadata_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2640 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/metadata_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1646 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/metadata_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6380 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10014 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5646 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16807 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/spec_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2003 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/driver/zarr/zlib_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4220 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/driver/zarr/zlib_compressor_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.952689 tensorstore-0.1.8/tensorstore/examples/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2939 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/examples/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17267 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/examples/compute_percentiles.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8983 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/examples/create_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5861 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/examples/image_convolution.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3891 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/examples/map_apply.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.912689 tensorstore-0.1.8/tensorstore/examples/python/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.956689 tensorstore-0.1.8/tensorstore/examples/python/beam/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1131 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      153 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/README.md
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3314 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/compute_dfbyf.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3885 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/compute_percentiles.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1509 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/example.gin
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5501 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/pipeline_test.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       54 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/requirements.txt
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6370 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/reshard_tensor.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1567 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/run_pipeline.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      467 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/examples/python/beam/setup.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4194 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/examples/status_result.cc
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     9827 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/generate_interval_slice_overloads.py
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     6687 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/generate_make_array_overloads.py
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     4187 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/generate_matches_array_overloads.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1934 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17923 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_interval.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    36088 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_interval.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    57627 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_interval_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.960689 tensorstore-0.1.8/tensorstore/index_space/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    25637 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8594 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/add_new_dims_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6869 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/alignment.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8136 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/alignment.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19374 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/alignment_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13815 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/compose_transforms_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5388 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/deep_copy_transform_rep_ptr_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14645 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/diagonal_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    84002 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/dim_expression.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2098 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/dim_expression_nc_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6145 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/dimension_identifier.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9920 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/dimension_identifier.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11428 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/dimension_identifier_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1281 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/dimension_index_buffer.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16540 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/dimension_selection_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11564 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/get_output_range_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6984 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/identity_transform_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    32007 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_array_slice_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13331 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_domain_builder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16176 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    57634 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6795 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_builder.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    35316 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_builder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23808 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_builder_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2402 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4935 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8437 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_spec_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    25719 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7129 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2129 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/index_transform_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1230 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3390 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3608 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.968689 tensorstore-0.1.8/tensorstore/index_space/internal/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6746 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/add_new_dims_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2982 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/add_new_dims_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11724 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/compose_transforms.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2866 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/compose_transforms.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3562 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/deep_copy_transform_rep_ptr.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8226 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/diagonal_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3204 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/diagonal_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9903 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/dim_expression_helper.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11025 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/dim_expression_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6784 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/dimension_selection.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5564 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/dimension_selection.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3486 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/identity_transform.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2338 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/identity_transform.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    18082 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/index_array_slice_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8119 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/index_array_slice_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10602 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/interval_slice_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8940 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/interval_slice_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5499 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/inverse_transform.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1180 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/inverse_transform.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19996 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/iterate.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17048 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/iterate_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1878 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/label_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3617 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/label_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1334 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/mark_explicit_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3164 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/mark_explicit_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13881 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/propagate_bounds.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3032 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/propagate_bounds.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12680 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/single_index_slice_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3915 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/single_index_slice_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10100 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transform_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6105 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transform_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20845 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23735 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3818 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    31782 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transformed_array_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4544 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/translate_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5079 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/translate_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12316 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transpose_op.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7718 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/index_space/internal/transpose_op.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    41774 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/interval_slice_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15212 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/inverse_transform_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6679 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/iterate_benchmark_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1327 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/iterate_nc_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14085 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/iterate_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21963 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/json.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9599 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/json.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    22494 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/json_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4177 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/label_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10309 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/mark_explicit_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10533 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/move_to_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10512 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/output_index_map.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9432 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/output_index_map_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1067 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/output_index_method.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    27557 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/propagate_bounds_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    24852 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/propagate_input_domain_resize_to_output_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17309 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/single_index_slice_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13385 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/index_space/slice_by_index_domain_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5680 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/transform_array_constraints.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3771 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space/transform_array_constraints_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16396 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/transform_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17750 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/transform_rep_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9249 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/transformed_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    60604 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/index_space/transformed_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    33909 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/index_space/transformed_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21167 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/translate_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9185 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/transpose_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5294 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/index_space/transpose_to_op_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7782 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/index_space.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.988689 tensorstore-0.1.8/tensorstore/internal/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    58460 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3537 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/aggregate_writeback_cache.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5220 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/arena.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3525 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/arena_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    32220 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/async_cache.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    40848 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/async_cache.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    36956 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/async_cache_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3547 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/async_initialized_cache_mixin.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11607 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/async_write_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12897 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/async_write_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    18483 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/async_write_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      945 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/attributes.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3975 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/bit_operations.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1587 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/bit_operations_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5530 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/box_difference.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2621 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/box_difference.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6839 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/box_difference_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20320 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/cache.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17786 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/cache.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7411 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/cache_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1783 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/cache_key.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1040 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/cache_pool_limits.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2775 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/cache_pool_resource.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1069 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/cache_pool_resource.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3445 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/cache_pool_resource_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    41441 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/cache_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    33045 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/chunk_cache.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17326 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/chunk_cache.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13568 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/chunk_cache_benchmark_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    57456 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/chunk_cache_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3388 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/compressed_pair.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3585 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/compressed_pair_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.992689 tensorstore-0.1.8/tensorstore/internal/compression/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6092 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2847 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/blosc.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2996 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/blosc.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2318 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/blosc_compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9178 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/blosc_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3400 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/bzip2.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1894 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/bzip2.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1731 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/bzip2_compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4604 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/bzip2_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3087 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/cord_stream_manager.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10994 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/jpeg.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2798 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/jpeg.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9462 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/jpeg_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1524 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/json_specified_compressor.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3225 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/json_specified_compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3563 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/lzma.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2161 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/lzma.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5273 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/lzma_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16759 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8837 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15320 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1635 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/xz_compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4258 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/zlib.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2244 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/zlib.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1742 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/zlib_compressor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5348 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/compression/zlib_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2453 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/concurrency_resource.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2374 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/concurrency_resource.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2256 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/concurrency_resource_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      669 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/concurrent_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3768 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/concurrent_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1453 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/container_to_shared.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1542 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/container_to_shared_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8794 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tensorstore/internal/context_binding.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1329 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/cord_util.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/cord_util.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1712 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/data_copy_concurrency_resource.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1186 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/data_copy_concurrency_resource.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8925 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5753 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10757 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2828 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/data_type_json_binder.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1228 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/data_type_json_binder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2700 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/data_type_json_binder_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5246 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/data_type_random_generator.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1667 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/data_type_random_generator.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2094 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/decoded_matches.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1633 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/decoded_matches.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2487 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/decoded_matches_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1855 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/element_copy_function.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    24593 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/elementwise_function.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9424 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/elementwise_function_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4880 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/endian_elementwise_conversion.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1725 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/env.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1158 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/env.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1191 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/env_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2237 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/estimate_heap_usage.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1007 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/exception_macros.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1404 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/file_io_concurrency_resource.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1067 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/file_io_concurrency_resource.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2831 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/flat_cord_builder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      838 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/gdb_scripting.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2235 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/global_initializer.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1036 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/global_initializer_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17261 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6867 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    40249 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition_impl.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7949 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20798 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition_impl_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20725 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/grid_partition_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1069 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/half_gtest.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.992689 tensorstore-0.1.8/tensorstore/internal/http/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3178 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/internal/http/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5648 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_handle.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3331 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_handle.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      964 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_handle_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      321 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_request_initialize.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15994 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_transport.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2293 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_transport.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23360 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/internal/http/curl_transport_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2584 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_request.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3147 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_request.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1495 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_request_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7589 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_response.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1922 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_response.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4152 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/http/http_response_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1515 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/http/http_transport.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      273 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/init_tensorstore.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      468 2020-06-29 03:39:51.000000 tensorstore-0.1.8/tensorstore/internal/init_tensorstore.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4992 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/integer_overflow.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4582 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/integer_overflow_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1716 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/integer_types.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3200 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_linked_list.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1835 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_linked_list_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15395 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_ptr.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9650 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_ptr_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19888 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    22500 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11184 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13299 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    44960 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11425 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/json_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5671 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/json_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9475 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/json_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15178 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_bindable.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1887 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json_fwd.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1850 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/json_gtest.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10660 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pointer.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5812 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pointer.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14164 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pointer_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5387 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pprint_python.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2303 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pprint_python.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3335 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/json_pprint_python_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9038 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_registry.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      990 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_registry_fwd.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4235 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_registry_impl.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8372 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_registry_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4108 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/json_registry_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    38086 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/json_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13866 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    31163 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    28565 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7432 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2194 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/lock_collection.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5400 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/lock_collection.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7545 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/lock_collection_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1056 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/log_message.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1300 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/log_message.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1606 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/logging.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14140 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/masked_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4654 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/masked_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    34052 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/masked_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4517 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/masked_array_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3058 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/masked_array_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5168 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/memory.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1483 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/meta.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1316 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/meta_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12446 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/multi_vector.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4777 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/multi_vector_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11741 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/multi_vector_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7706 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/multi_vector_view.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5978 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/multi_vector_view_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5630 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/mutex.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1472 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17654 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/nditerable.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7603 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1658 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21766 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3912 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_array_util.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17379 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_buffer_management.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9316 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_copy.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7836 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_copy.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7246 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_copy_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5291 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1989 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4615 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4858 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2290 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5910 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4087 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2364 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4271 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    21561 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2234 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19749 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6734 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_util.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    18985 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_util.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12610 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/nditerable_util_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1668 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/no_destructor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/no_destructor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      959 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/non_compile_bypass.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.996689 tensorstore-0.1.8/tensorstore/internal/oauth2/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6653 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1002 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1566 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2976 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/fake_private_key.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      989 2020-06-29 03:39:51.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/fake_private_key.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1095 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1400 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1081 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6240 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2633 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4507 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8596 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1918 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6998 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4245 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2760 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5112 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3785 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2635 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4127 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9540 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3523 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10327 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3771 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/open_mode_spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2292 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/open_mode_spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3585 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/os_error_code.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1991 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tensorstore/internal/os_error_code.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1887 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/parse_json_matches.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1490 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/parse_json_matches.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1922 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/parse_json_matches_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3567 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/path.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2364 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/path.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4627 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/path_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      793 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/poly.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14678 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/poly.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    22161 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/poly_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14943 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/poly_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1559 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/preprocessor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2203 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/queue_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3046 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/retry.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1500 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/retry.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2860 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/retry_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1218 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/source_location.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2102 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1407 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3411 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2606 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/string_like.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1581 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/string_like_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7245 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/tagged_ptr.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5875 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/tagged_ptr_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7032 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/test_util.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2067 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/internal/test_util.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9371 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/internal/thread_pool.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1166 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/thread_pool.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3558 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/internal/thread_pool_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    17835 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/type_traits.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8155 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/type_traits_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6238 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/unique_with_intrusive_allocator.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2395 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/unique_with_intrusive_allocator_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1369 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/unowned_to_shared.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4184 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/utf8.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/utf8.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2981 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/utf8_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3462 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/void_wrapper.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3125 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/internal/void_wrapper_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3377 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/json_serialization_options.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.000689 tensorstore-0.1.8/tensorstore/kvstore/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5460 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1725 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/byte_range.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3643 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/byte_range.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5235 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/byte_range_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.000689 tensorstore-0.1.8/tensorstore/kvstore/file/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2674 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    32642 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/file/file_key_value_store.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20758 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/file_key_value_store_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      736 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/file/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4754 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/posix_file_util.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10976 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/posix_file_util.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      694 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/file/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2039 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/file/unique_handle.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12462 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/windows_file_util.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4843 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/file/windows_file_util.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.000689 tensorstore-0.1.8/tensorstore/kvstore/gcs/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3279 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    32888 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_key_value_store.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20408 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_key_value_store_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16010 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_mock.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4390 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_mock.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2428 2020-08-25 23:48:07.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6190 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2641 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7032 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3700 2020-07-29 01:03:09.000000 tensorstore-0.1.8/tensorstore/kvstore/gcs/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4331 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/generation.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11197 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/generation.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2554 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/generation_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3760 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/generation_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      490 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5056 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_range.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4518 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_range.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7351 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_range_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8776 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_value_store.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    33164 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_value_store.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1456 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/key_value_store_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20189 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/key_value_store_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8419 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/key_value_store_testutil.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.000689 tensorstore-0.1.8/tensorstore/kvstore/memory/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1784 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      385 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/index.rst
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20737 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1348 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10714 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1666 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/memory/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13669 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/registry.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      680 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/kvstore/schema.yml
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    60416 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/transaction.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    27920 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/kvstore/transaction.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    35341 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/make_array.inc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1860 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/non_compile.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1800 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/open.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4138 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/open.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1658 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/open_mode.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5344 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/open_mode.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4599 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/open_mode_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2381 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/progress.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3647 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/progress.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2268 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/progress_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      895 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/rank.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13500 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/rank.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6942 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/rank_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3595 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/read_write_options.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1596 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/resize_options.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4148 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/resize_options.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/resize_options_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2098 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/spec.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3717 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/spec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1178 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/spec_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2473 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/spec_request_options.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5658 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/spec_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3334 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/staleness_bound.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1017 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/static_cast.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12240 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/static_cast.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7779 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/static_cast_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1688 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/strided_layout.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    41764 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/strided_layout.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    42899 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/strided_layout_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1134 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/tensorstore.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2270 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/tensorstore.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23012 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/tensorstore.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13458 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/tensorstore_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19541 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/transaction.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10813 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/transaction.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    39108 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/transaction_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    22625 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/transaction_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2843 2020-04-18 03:06:59.000000 tensorstore-0.1.8/tensorstore/update_generated_source_code.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.008689 tensorstore-0.1.8/tensorstore/util/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16168 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/BUILD
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2053 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/assert_macros.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      818 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/assert_macros_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15174 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/bit_span.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    14756 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/bit_span_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8144 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/bit_vec.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2118 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/bit_vec_impl.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3611 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/bit_vec_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    12255 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/bit_vec_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5774 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/byte_strided_pointer.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5599 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/byte_strided_pointer_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3010 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/collecting_sender.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1921 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/collecting_sender_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1902 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/constant_bit_vector.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2113 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/constant_bit_vector_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2602 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/constant_vector.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7892 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/constant_vector.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3754 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/constant_vector_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1636 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/default_iteration_result.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      917 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/default_iteration_result_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5267 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/division.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1019 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/division_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1025 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/element_pointer.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19732 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/util/element_pointer.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    18292 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/element_pointer_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3772 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/element_traits.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3574 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/element_traits_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2664 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/endian.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4862 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/execution.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3053 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/executor.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2154 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/executor_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7194 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/extents.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6028 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/extents_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3441 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/function_view.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2801 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/function_view_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16267 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/util/future.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    48151 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/util/future.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    59289 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/future_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     7017 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/future_sender_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    57197 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tensorstore/util/future_test.cc
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.008689 tensorstore-0.1.8/tensorstore/util/internal/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4502 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/internal/iterate.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11913 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/internal/iterate_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8659 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/iterate.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10246 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/util/iterate.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     8762 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/iterate_over_index_range.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5271 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/iterate_over_index_range_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23132 2020-11-30 23:09:09.000000 tensorstore-0.1.8/tensorstore/util/iterate_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      884 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/quote_string.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1106 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/quote_string.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      918 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/quote_string_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    29458 2020-07-31 18:37:28.000000 tensorstore-0.1.8/tensorstore/util/result.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10934 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/result_impl.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/result_nc_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2772 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/result_sender_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    28679 2020-05-28 22:28:53.000000 tensorstore-0.1.8/tensorstore/util/result_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    16093 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/sender.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    11163 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/sender_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2464 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/sender_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    15027 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/span.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1062 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/span_json.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      967 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/span_json_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    20313 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/span_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1557 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/status.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6408 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/status.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2979 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/status_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2371 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/status_testutil.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3468 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/status_testutil.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3429 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/str_cat.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1858 2020-06-29 03:39:52.000000 tensorstore-0.1.8/tensorstore/util/str_cat_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3600 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/sync_flow_sender.h
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3091 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/sync_flow_sender_test.cc
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1706 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tensorstore/util/utf8_string.h
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.008689 tensorstore-0.1.8/third_party/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       54 2020-04-18 03:06:59.000000 tensorstore-0.1.8/third_party/BUILD.bazel
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.008689 tensorstore-0.1.8/third_party/com_facebook_zstd/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2305 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_facebook_zstd/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_facebook_zstd/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1211 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_facebook_zstd/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.008689 tensorstore-0.1.8/third_party/com_github_nlohmann_json/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      333 2020-11-30 23:09:09.000000 tensorstore-0.1.8/third_party/com_github_nlohmann_json/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1117 2020-11-30 23:09:09.000000 tensorstore-0.1.8/third_party/com_github_nlohmann_json/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_github_pybind_pybind11/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      423 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_github_pybind_pybind11/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1138 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_github_pybind_pybind11/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_google_absl/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1133 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/com_google_absl/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_google_benchmark/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1041 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_benchmark/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_google_boringssl/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      261 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_boringssl/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1306 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_boringssl/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_google_googletest/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1113 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_googletest/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/com_google_snappy/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3928 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_snappy/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      106 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_snappy/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1189 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/com_google_snappy/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/jpeg/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    23571 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/jpeg/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/jpeg/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1379 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/jpeg/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/nasm/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4102 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/nasm/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       53 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/nasm/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1183 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/nasm/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/net_sourceforge_half/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      318 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/net_sourceforge_half/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1108 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/net_sourceforge_half/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/net_zlib/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/net_zlib/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)       99 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/net_zlib/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1169 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/net_zlib/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/org_blosc_cblosc/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4175 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_blosc_cblosc/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      104 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_blosc_cblosc/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1213 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_blosc_cblosc/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/org_lz4/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      961 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_lz4/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      100 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_lz4/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1174 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_lz4/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/org_nghttp2/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     6962 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/org_nghttp2/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      108 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/org_nghttp2/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1228 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/org_nghttp2/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/org_sourceware_bzip2/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      513 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_sourceware_bzip2/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_sourceware_bzip2/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1221 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_sourceware_bzip2/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/org_tukaani_xz/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    24299 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_tukaani_xz/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      100 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_tukaani_xz/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1176 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/org_tukaani_xz/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/pypa/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/pypa/absl_py/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1110 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/absl_py/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.012689 tensorstore-0.1.8/third_party/pypa/alabaster/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      971 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/alabaster/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/apache_beam/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3587 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/apache_beam/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/argh/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      951 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/argh/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/atomicwrites/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      982 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/atomicwrites/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/attrs/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      955 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/attrs/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/avro_python3/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      984 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/avro_python3/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/babel/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1107 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/babel/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/backcall/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      966 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/backcall/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/certifi/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      967 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/certifi/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/chardet/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      962 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/chardet/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/crcmod/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      956 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/crcmod/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/decorator/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      970 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/decorator/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/dill/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      952 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/dill/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/docopt/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      958 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/docopt/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/docutils/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      965 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/docutils/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/fastavro/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      968 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/fastavro/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/future/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      959 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/future/workspace.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5187 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/generate_pypa_directory.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/gin_config/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1122 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/gin_config/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/grpcio/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1107 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/grpcio/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/hdfs/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1378 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/hdfs/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/httplib2/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      967 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/httplib2/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/idna/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      948 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/idna/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/imagesize/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      970 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/imagesize/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/importlib_metadata/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1158 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/importlib_metadata/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/ipython/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2335 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/ipython/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/ipython_genutils/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      998 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/ipython_genutils/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/jedi/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1109 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/jedi/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/jinja2/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1142 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/jinja2/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/jsonpointer/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      976 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/jsonpointer/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/jsonschema/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1757 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/jsonschema/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/livereload/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1262 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/livereload/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/markupsafe/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      974 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/markupsafe/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/mock/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1218 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/mock/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/more_itertools/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      990 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/more_itertools/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/numpy/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      955 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/numpy/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/oauth2client/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1705 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/oauth2client/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/packaging/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1267 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/packaging/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/parso/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      954 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/parso/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/pathtools/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      970 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pathtools/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/pbr/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      946 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pbr/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.016689 tensorstore-0.1.8/third_party/pypa/pexpect/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1145 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pexpect/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pickleshare/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      978 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pickleshare/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pluggy/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1182 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pluggy/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/port_for/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      966 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/port_for/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/prompt_toolkit/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1279 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/prompt_toolkit/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/protobuf/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1270 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/protobuf/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/ptyprocess/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      974 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/ptyprocess/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/py/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      942 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/py/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyarrow/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1241 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pyarrow/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyasn1/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      958 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pyasn1/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyasn1_modules/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1153 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pyasn1_modules/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pydot/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1132 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pydot/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pygments/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      966 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pygments/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pymongo/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      963 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/pymongo/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyparsing/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      970 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pyparsing/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyrsistent/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1123 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pyrsistent/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pytest/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2191 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pytest/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pytest_asyncio/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1154 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pytest_asyncio/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/python_dateutil/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1142 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/python_dateutil/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pytz/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      951 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pytz/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/pyyaml/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      956 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/pyyaml/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/requests/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1540 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/requests/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/rsa/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1107 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/rsa/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/setuptools/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      975 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/setuptools/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/six/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      947 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/six/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/snowballstemmer/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      994 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/snowballstemmer/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinx/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     3776 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinx/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinx_autobuild/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     2021 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinx_autobuild/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinx_rtd_theme/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1161 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinx_rtd_theme/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_applehelp/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1026 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_applehelp/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_devhelp/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1018 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_devhelp/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_htmlhelp/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1022 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_htmlhelp/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_jsmath/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1014 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_jsmath/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_qthelp/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1014 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_qthelp/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_serializinghtml/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1050 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/sphinxcontrib_serializinghtml/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/tornado/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      962 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/tornado/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/traitlets/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1453 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/traitlets/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/typing_extensions/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1004 2020-05-09 00:00:44.000000 tensorstore-0.1.8/third_party/pypa/typing_extensions/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/urllib3/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      963 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/urllib3/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.020689 tensorstore-0.1.8/third_party/pypa/watchdog/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1145 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/watchdog/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/third_party/pypa/wcwidth/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      962 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/wcwidth/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/third_party/pypa/wheel/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      955 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/wheel/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/third_party/pypa/zipp/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1153 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/pypa/zipp/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/third_party/python/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1899 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/python/BUILD.tpl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    10317 2020-04-29 01:47:28.000000 tensorstore-0.1.8/third_party/python/python_configure.bzl
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5264 2020-04-18 03:06:59.000000 tensorstore-0.1.8/third_party/repo.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/third_party/se_haxx_curl/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    19573 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/se_haxx_curl/bundled.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.8/third_party/se_haxx_curl/system.BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     1194 2020-06-29 03:39:52.000000 tensorstore-0.1.8/third_party/se_haxx_curl/workspace.bzl
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:32.920689 tensorstore-0.1.8/tools/
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/tools/docs/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      937 2020-05-09 00:00:44.000000 tensorstore-0.1.8/tools/docs/BUILD.bazel
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4714 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tools/docs/build_docs.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4125 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tools/docs/json_pprint.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     9430 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tools/docs/tensorstore_autosummary.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)    13955 2020-04-18 03:07:00.000000 tensorstore-0.1.8/tools/docs/tensorstore_jsonschema_sphinx.py
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     5155 2020-10-10 00:09:50.000000 tensorstore-0.1.8/tools/docs/update_doctests.py
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/tools/python-manylinux/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      239 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tools/python-manylinux/README.md
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)      635 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tools/python-manylinux/build_wheels_inside_container.sh
--rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     1372 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tools/python-manylinux/build_wheels_manylinux2014_x86_64.sh
-drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2020-11-30 23:09:33.024689 tensorstore-0.1.8/tools/python-manylinux/manylinux2014_x86_64/
--rw-r--r--   0 jbms     (297878) primarygroup (89939)      331 2020-04-29 01:47:28.000000 tensorstore-0.1.8/tools/python-manylinux/manylinux2014_x86_64/Dockerfile
--rw-r--r--   0 jbms     (297878) primarygroup (89939)     4419 2020-04-18 03:06:59.000000 tensorstore-0.1.8/utils.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1225 2021-01-13 22:02:59.000000 tensorstore-0.1.9/.bazelrc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)        6 2020-08-25 23:48:07.000000 tensorstore-0.1.9/.bazelversion
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       76 2020-04-18 03:06:59.000000 tensorstore-0.1.9/.clang-format
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      244 2020-04-18 03:06:59.000000 tensorstore-0.1.9/.gitignore
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       33 2020-04-18 03:06:59.000000 tensorstore-0.1.9/.style.yapf
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      303 2020-04-18 03:06:59.000000 tensorstore-0.1.9/AUTHORS
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      153 2020-04-29 01:47:28.000000 tensorstore-0.1.9/BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1097 2020-04-18 03:06:59.000000 tensorstore-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12627 2020-04-18 03:06:59.000000 tensorstore-0.1.9/LICENSE
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      300 2021-01-13 22:04:08.141687 tensorstore-0.1.9/PKG-INFO
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      803 2020-04-18 03:06:59.000000 tensorstore-0.1.9/README.md
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      191 2020-04-18 03:06:59.000000 tensorstore-0.1.9/WORKSPACE
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)    11342 2020-04-18 03:06:59.000000 tensorstore-0.1.9/bazelisk.py
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1632 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/BUILD
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/_static/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1097 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/_static/sphinx_rtd_theme_table_word_wrap_fix.css
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/_templates/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/_templates/autosummary/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      106 2020-04-18 03:07:00.000000 tensorstore-0.1.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      539 2020-04-18 03:07:00.000000 tensorstore-0.1.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      693 2020-04-18 03:07:00.000000 tensorstore-0.1.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      678 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/_templates/autosummary_root_module.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5152 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/build_docs.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3468 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/conf.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      640 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/context.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4482 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/context_schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      132 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/docutils.conf
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4523 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/environment.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      323 2020-08-25 23:48:07.000000 tensorstore-0.1.9/docs/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4220 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/index_domain_schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10856 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/index_space.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7816 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/index_transform_schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6202 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/installation.rst
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/intersphinx_inv/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9632 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/intersphinx_inv/dask.inv
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    62911 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/intersphinx_inv/numpy.inv
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)   109510 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/intersphinx_inv/python3.inv
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2093 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/intersphinx_inv/zarr.inv
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4125 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/json_pprint.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      699 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/overview.rst
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/python/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.049687 tensorstore-0.1.9/docs/python/api/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      169 2020-04-18 03:07:00.000000 tensorstore-0.1.9/docs/python/api/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      107 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/python/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    41109 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/python/indexing.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7705 2020-08-25 23:48:07.000000 tensorstore-0.1.9/docs/python/tutorial.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      310 2020-04-29 01:47:28.000000 tensorstore-0.1.9/docs/spec.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9431 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/tensorstore_autosummary.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13955 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/tensorstore_jsonschema_sphinx.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1553 2020-04-18 03:06:59.000000 tensorstore-0.1.9/docs/tensorstore_schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5155 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/update_doctests.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1452 2021-01-13 22:01:20.000000 tensorstore-0.1.9/docs/update_intersphinx_inventories.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3652 2021-01-13 22:01:20.000000 tensorstore-0.1.9/external.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.041687 tensorstore-0.1.9/python/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.053687 tensorstore-0.1.9/python/tensorstore/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13355 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11418 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/LICENSE
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1278 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/__init__.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13652 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/array_type_caster.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11060 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/array_type_caster.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1313 2020-04-29 01:47:28.000000 tensorstore-0.1.9/python/tensorstore/bazel_pytest_main.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17088 2020-07-29 01:03:09.000000 tensorstore-0.1.9/python/tensorstore/context.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4724 2020-07-29 01:03:09.000000 tensorstore-0.1.9/python/tensorstore/context.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6650 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/data_type.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7225 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/data_type.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21241 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/dim_expression.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5777 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/dim_expression.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3132 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/downsample.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1566 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/downsample.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8025 2020-07-29 01:03:09.000000 tensorstore-0.1.9/python/tensorstore/future.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10647 2021-01-13 22:02:59.000000 tensorstore-0.1.9/python/tensorstore/future.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2502 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/index.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5903 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/index.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    47813 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/index_space.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11850 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/index_space.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4502 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/index_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    45258 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/indexing_spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13625 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/indexing_spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1414 2020-07-29 01:03:09.000000 tensorstore-0.1.9/python/tensorstore/intrusive_ptr_holder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6417 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/json_type_caster.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2237 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/json_type_caster.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4178 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/pybind11.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1337 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/pytest.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3774 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/result_type_caster.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      853 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/shell.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5657 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1564 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2243 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/status.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2113 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/status.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4378 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/subscript_method.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2327 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/tensorstore.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13298 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/tensorstore_class.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1098 2020-04-18 03:06:59.000000 tensorstore-0.1.9/python/tensorstore/tensorstore_class.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.057687 tensorstore-0.1.9/python/tensorstore/tests/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3690 2020-07-29 01:03:09.000000 tensorstore-0.1.9/python/tensorstore/tests/context_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3758 2020-04-29 01:47:28.000000 tensorstore-0.1.9/python/tensorstore/tests/data_type_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21225 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/tests/dim_expression_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1627 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/tests/downsample_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1824 2021-01-13 22:02:59.000000 tensorstore-0.1.9/python/tensorstore/tests/future_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5812 2021-01-13 22:01:20.000000 tensorstore-0.1.9/python/tensorstore/tests/index_domain_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2859 2020-04-29 01:47:28.000000 tensorstore-0.1.9/python/tensorstore/tests/index_interval_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4491 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/tests/index_transform_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6101 2020-04-29 01:47:28.000000 tensorstore-0.1.9/python/tensorstore/tests/indexing_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2959 2020-11-30 23:09:09.000000 tensorstore-0.1.9/python/tensorstore/tests/spec_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8954 2021-01-13 22:02:59.000000 tensorstore-0.1.9/python/tensorstore/tests/tensorstore_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4811 2020-10-10 00:09:50.000000 tensorstore-0.1.9/python/tensorstore/tests/transaction_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8466 2020-10-10 00:09:50.000000 tensorstore-0.1.9/python/tensorstore/transaction.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1697 2020-10-10 00:09:50.000000 tensorstore-0.1.9/python/tensorstore/transaction.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2493 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/write_futures.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2055 2020-06-29 03:39:52.000000 tensorstore-0.1.9/python/tensorstore/write_futures.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.053687 tensorstore-0.1.9/python/tensorstore.egg-info/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      300 2021-01-13 22:04:07.000000 tensorstore-0.1.9/python/tensorstore.egg-info/PKG-INFO
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    36194 2021-01-13 22:04:07.000000 tensorstore-0.1.9/python/tensorstore.egg-info/SOURCES.txt
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)        1 2021-01-13 22:04:07.000000 tensorstore-0.1.9/python/tensorstore.egg-info/dependency_links.txt
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       14 2021-01-13 22:04:07.000000 tensorstore-0.1.9/python/tensorstore.egg-info/requires.txt
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       37 2021-01-13 22:04:07.000000 tensorstore-0.1.9/python/tensorstore.egg-info/top_level.txt
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       38 2021-01-13 22:04:08.141687 tensorstore-0.1.9/setup.cfg
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3422 2021-01-13 22:01:20.000000 tensorstore-0.1.9/setup.py
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.065687 tensorstore-0.1.9/tensorstore/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16969 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7448 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    77772 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2050 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/array_nc_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    65319 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7580 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/array_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8782 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/array_testutil_matches_array.inc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6493 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/array_testutil_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1399 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/box.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    32289 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/box.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    25021 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/box_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3933 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/cast.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      935 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/container_kind.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21056 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/context.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13166 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/context.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6638 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/context_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10720 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/context_impl_base.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8060 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/context_resource_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18808 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/context_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1491 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/contiguous_layout.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2145 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/contiguous_layout.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1991 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/contiguous_layout_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14673 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/data_type.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    38274 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/data_type.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19708 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/data_type_conversion.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    36812 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/data_type_conversion_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15163 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/data_type_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4180 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/downsample.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1248 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/downsample_method.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1082 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/downsample_method.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.065687 tensorstore-0.1.9/tensorstore/driver/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6727 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/BUILD
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.065687 tensorstore-0.1.9/tensorstore/driver/array/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1753 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/array/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14569 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/array/array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2976 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/array/array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    35884 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/array/array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      371 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/array/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      714 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/array/schema.yml
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.069687 tensorstore-0.1.9/tensorstore/driver/cast/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1432 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/cast/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12304 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/cast/cast.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4667 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/cast/cast.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21276 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/cast/cast_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      610 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/cast/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      761 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/cast/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9213 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/chunk.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.069687 tensorstore-0.1.9/tensorstore/driver/downsample/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7404 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    34412 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1185 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8291 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2974 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16820 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3996 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_benchmark_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1864 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_method_json_binder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    51337 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_nditerable.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3023 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_nditerable.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    28834 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    33627 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9647 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23931 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/downsample_util_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5509 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/grid_occupancy_map.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3359 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/grid_occupancy_map.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3529 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/grid_occupancy_map_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      258 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6352 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/downsample/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    45328 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    25715 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/driver.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3032 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/driver_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    29405 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/driver_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6418 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/driver_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      510 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/index.rst
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.069687 tensorstore-0.1.9/tensorstore/driver/json/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2542 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/json/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19524 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15041 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/driver_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      817 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6227 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/json_change_map.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3921 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/json_change_map.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7822 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/json_change_map_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3548 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/json/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    56642 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    32534 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6241 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5051 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6641 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7566 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/n5/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2009 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/blosc_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7021 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/n5/blosc_compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1524 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/bzip2_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3996 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/n5/bzip2_compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1881 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1214 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1231 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/compressor_registry.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14334 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/n5/driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    38892 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/n5/driver_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2513 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/golden_file_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2114 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/gzip_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4663 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/n5/gzip_compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      898 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19884 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/n5/metadata.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5229 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/n5/metadata.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12759 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/n5/metadata_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6138 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/n5/schema.yml
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/0/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/0/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/0/1
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/1/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/1/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       40 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/1/1
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      266 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/blosc/attributes.json
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/0/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       54 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/0/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       55 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/0/1
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/1/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       56 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/1/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       56 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/1/1
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      199 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/bzip2/attributes.json
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1548 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/generate.py
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/0/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/0/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/0/1
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/1/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/1/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       44 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/1/1
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      220 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/gzip/attributes.json
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/0/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/0/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/0/1
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/1/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/1/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       24 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/1/1
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      173 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/raw/attributes.json
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/0/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/0/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/0/1
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.073687 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/1/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/1/0
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       80 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/1/1
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      193 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/testdata/xz/attributes.json
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1541 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/n5/xz_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4138 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/n5/xz_compressor_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.077687 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9541 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13058 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2582 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3906 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    26138 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    67149 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/driver_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3446 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    41729 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11277 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    77881 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2184 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1434 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3171 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9457 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8508 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6580 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8493 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3553 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3719 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6444 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7209 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8237 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    43962 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5262 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    67224 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14203 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13611 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/registry.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.081687 tensorstore-0.1.9/tensorstore/driver/zarr/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8829 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/zarr/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2473 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/blosc_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12385 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/zarr/blosc_compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1548 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/bzip2_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4544 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/zarr/bzip2_compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1787 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1225 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1243 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/compressor_registry.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2387 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/compressor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17590 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/driver/zarr/driver.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1579 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/driver/zarr/driver_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16799 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/driver/zarr/driver_impl_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    82824 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/zarr/driver_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10656 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/dtype.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5080 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/dtype.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12994 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/dtype_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1238 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19114 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/zarr/metadata.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8948 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/zarr/metadata.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    30661 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/driver/zarr/metadata_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2640 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/metadata_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1646 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/metadata_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6380 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10014 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5646 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16807 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/spec_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2003 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/driver/zarr/zlib_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4220 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/driver/zarr/zlib_compressor_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.081687 tensorstore-0.1.9/tensorstore/examples/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2939 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/examples/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17267 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/examples/compute_percentiles.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8983 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/examples/create_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5861 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/examples/image_convolution.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3891 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/examples/map_apply.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.041687 tensorstore-0.1.9/tensorstore/examples/python/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.081687 tensorstore-0.1.9/tensorstore/examples/python/beam/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1232 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      153 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/README.md
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3314 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/compute_dfbyf.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3885 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/compute_percentiles.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1509 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/example.gin
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5501 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/pipeline_test.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       54 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/requirements.txt
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6370 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/reshard_tensor.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1567 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/run_pipeline.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      467 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/examples/python/beam/setup.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4194 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/examples/status_result.cc
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     9827 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/generate_interval_slice_overloads.py
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     6687 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/generate_make_array_overloads.py
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     4187 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/generate_matches_array_overloads.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1934 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17898 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_interval.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    36088 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_interval.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    57627 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_interval_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.089686 tensorstore-0.1.9/tensorstore/index_space/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    26004 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8936 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/add_new_dims_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6869 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/alignment.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8136 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/alignment.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19374 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/alignment_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14537 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/index_space/compose_transforms_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5388 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/deep_copy_transform_rep_ptr_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14645 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/diagonal_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    86594 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/dim_expression.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2098 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/dim_expression_nc_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6145 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/dimension_identifier.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9924 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/dimension_identifier.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11428 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/dimension_identifier_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1281 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/dimension_index_buffer.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16540 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/dimension_selection_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11564 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/get_output_range_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6984 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/identity_transform_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    33551 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/index_array_slice_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13374 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/index_domain_builder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17447 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    60781 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6795 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_builder.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    35412 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_builder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23808 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_builder_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2402 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4935 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8437 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_spec_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    25719 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7129 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2129 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/index_transform_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1230 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3390 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3608 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.093687 tensorstore-0.1.9/tensorstore/index_space/internal/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6807 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/add_new_dims_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2982 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/add_new_dims_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11746 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/index_space/internal/compose_transforms.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2866 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/compose_transforms.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3562 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/deep_copy_transform_rep_ptr.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8226 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/diagonal_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3204 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/diagonal_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9903 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/internal/dim_expression_helper.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11025 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/dim_expression_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6784 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/internal/dimension_selection.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5564 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/dimension_selection.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3486 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/identity_transform.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2338 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/identity_transform.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18090 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/index_array_slice_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8119 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/index_array_slice_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10602 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/internal/interval_slice_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10302 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/interval_slice_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5499 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/internal/inverse_transform.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1180 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/inverse_transform.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20044 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/index_space/internal/iterate.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17048 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/iterate_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1878 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/label_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3617 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/label_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1334 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/mark_explicit_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3164 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/mark_explicit_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13554 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/propagate_bounds.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3032 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/propagate_bounds.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12680 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/internal/single_index_slice_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3915 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/single_index_slice_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10100 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transform_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6105 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transform_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20766 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23291 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3818 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    31782 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transformed_array_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4544 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/translate_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5079 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/translate_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12316 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transpose_op.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7718 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/index_space/internal/transpose_op.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    45344 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/interval_slice_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15212 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/inverse_transform_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6679 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/iterate_benchmark_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1327 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/iterate_nc_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14085 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/iterate_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    26779 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/json.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15823 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/json.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    29005 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/json_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4177 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/label_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10309 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/mark_explicit_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10533 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/move_to_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10512 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/output_index_map.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9432 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/output_index_map_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1067 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/output_index_method.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    27557 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/propagate_bounds_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    24852 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/propagate_input_domain_resize_to_output_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17309 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/single_index_slice_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5609 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/index_space/slice_by_box_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13385 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/index_space/slice_by_index_domain_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5680 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/transform_array_constraints.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3771 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space/transform_array_constraints_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18357 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/index_space/transform_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17750 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/transform_rep_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9249 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/transformed_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    60604 2020-07-31 18:37:28.000000 tensorstore-0.1.9/tensorstore/index_space/transformed_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    33909 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/index_space/transformed_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21167 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/translate_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9185 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/transpose_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5294 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/index_space/transpose_to_op_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7782 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/index_space.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.117687 tensorstore-0.1.9/tensorstore/internal/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    58460 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3537 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/aggregate_writeback_cache.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5220 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/arena.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3525 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/arena_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    32220 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/async_cache.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    40848 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/async_cache.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    36956 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/async_cache_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3547 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/async_initialized_cache_mixin.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11607 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/async_write_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12897 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/async_write_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18483 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/async_write_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      945 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/attributes.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3975 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/bit_operations.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1587 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/bit_operations_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5519 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/box_difference.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2252 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/box_difference.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6839 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/box_difference_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20320 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/cache.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17786 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/cache.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7411 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/cache_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1783 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/cache_key.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1040 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/cache_pool_limits.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2775 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/cache_pool_resource.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1069 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/cache_pool_resource.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3445 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/cache_pool_resource_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    41441 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/cache_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    33045 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/chunk_cache.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17326 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/chunk_cache.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13568 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/chunk_cache_benchmark_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    57456 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/chunk_cache_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3388 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/compressed_pair.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3585 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/compressed_pair_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.117687 tensorstore-0.1.9/tensorstore/internal/compression/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6092 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2847 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/blosc.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2996 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/blosc.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2318 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/blosc_compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9178 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/blosc_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3400 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/bzip2.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1894 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/bzip2.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1731 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/bzip2_compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4604 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/bzip2_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3087 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/cord_stream_manager.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10994 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/jpeg.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2798 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/jpeg.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9462 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/jpeg_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1524 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/json_specified_compressor.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3225 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/json_specified_compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3563 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/lzma.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2161 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/lzma.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5273 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/lzma_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16759 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8837 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15320 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1635 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/xz_compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4258 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/zlib.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2244 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/zlib.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1742 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/zlib_compressor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5348 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/compression/zlib_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2453 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/concurrency_resource.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2374 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/concurrency_resource.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2256 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/concurrency_resource_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      669 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/concurrent_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3768 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/concurrent_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1453 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/container_to_shared.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1542 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/container_to_shared_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8794 2020-05-09 00:00:44.000000 tensorstore-0.1.9/tensorstore/internal/context_binding.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1329 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/cord_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/cord_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1712 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/data_copy_concurrency_resource.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1186 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/data_copy_concurrency_resource.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8925 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5753 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10757 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2828 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/data_type_json_binder.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1228 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/data_type_json_binder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2700 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/data_type_json_binder_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5246 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/data_type_random_generator.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1667 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/data_type_random_generator.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2094 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/decoded_matches.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1633 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/decoded_matches.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2487 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/decoded_matches_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1855 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/element_copy_function.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    24747 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/elementwise_function.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9424 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/elementwise_function_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4880 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/endian_elementwise_conversion.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1725 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/env.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1158 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/env.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1191 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/env_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2237 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/estimate_heap_usage.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1007 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/exception_macros.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1404 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/file_io_concurrency_resource.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1067 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/file_io_concurrency_resource.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2831 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/flat_cord_builder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      838 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/gdb_scripting.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2235 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/global_initializer.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1036 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/global_initializer_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17261 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6867 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    40249 2020-08-25 23:48:07.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition_impl.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7949 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20798 2020-08-25 23:48:07.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition_impl_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20725 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/grid_partition_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1069 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/half_gtest.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.121687 tensorstore-0.1.9/tensorstore/internal/http/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3168 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/http/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5648 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_handle.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3331 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_handle.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      964 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_handle_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      321 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_request_initialize.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15994 2020-08-25 23:48:07.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_transport.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2293 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_transport.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23360 2020-08-25 23:48:07.000000 tensorstore-0.1.9/tensorstore/internal/http/curl_transport_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2584 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_request.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3147 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_request.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1495 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_request_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7589 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_response.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1922 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_response.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4152 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/http/http_response_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1515 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/http/http_transport.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      273 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/init_tensorstore.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      468 2020-06-29 03:39:51.000000 tensorstore-0.1.9/tensorstore/internal/init_tensorstore.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4992 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/integer_overflow.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4582 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/integer_overflow_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1716 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/integer_types.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3200 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_linked_list.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1835 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_linked_list_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15908 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_ptr.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11481 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_ptr_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19888 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    22500 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11184 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13299 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    44960 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11619 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/json_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5671 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/json_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9855 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/json_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15178 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_bindable.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1887 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json_fwd.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5219 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/json_gtest.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10660 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pointer.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5812 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pointer.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14164 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pointer_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5387 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pprint_python.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2303 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pprint_python.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3335 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/json_pprint_python_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9038 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_registry.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      990 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_registry_fwd.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4235 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_registry_impl.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8372 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_registry_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4108 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/json_registry_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    36010 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/json_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13866 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    31163 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    28565 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7432 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2194 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/lock_collection.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5400 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/lock_collection.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7545 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/lock_collection_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1056 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/log_message.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1300 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/log_message.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1606 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/logging.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14140 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/masked_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4654 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/masked_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    34052 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/masked_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4517 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/masked_array_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3058 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/masked_array_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5168 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/memory.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1483 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/meta.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1316 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/meta_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12446 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/multi_vector.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4777 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/multi_vector_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11741 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/multi_vector_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7706 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/multi_vector_view.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5978 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/multi_vector_view_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5630 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/mutex.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1472 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17654 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/nditerable.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7603 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1658 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21766 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3912 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_array_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    17379 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_buffer_management.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9316 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_copy.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7836 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_copy.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7246 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_copy_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5291 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1989 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4615 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4858 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2290 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5910 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4087 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2364 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4271 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    21561 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2234 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19749 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6734 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18985 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12610 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/nditerable_util_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1668 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/no_destructor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/no_destructor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      959 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/non_compile_bypass.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.121687 tensorstore-0.1.9/tensorstore/internal/oauth2/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6653 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1002 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1566 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2976 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/fake_private_key.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      989 2020-06-29 03:39:51.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/fake_private_key.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1095 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1400 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1081 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6240 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2633 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4507 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8596 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1918 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6998 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4245 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2760 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5112 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3785 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2635 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4127 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9540 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3523 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10327 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3771 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/open_mode_spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2292 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/open_mode_spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3585 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/os_error_code.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1991 2020-04-29 01:47:28.000000 tensorstore-0.1.9/tensorstore/internal/os_error_code.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1887 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/parse_json_matches.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1490 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/parse_json_matches.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1922 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/parse_json_matches_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3567 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/path.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2364 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/path.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4627 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/path_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      793 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/poly.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14678 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/poly.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    22161 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/poly_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14943 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/poly_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1559 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/preprocessor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2203 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/queue_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3046 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/retry.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1500 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/retry.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2860 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/retry_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1218 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/source_location.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2102 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1407 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3411 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2606 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/string_like.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1581 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/string_like_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7245 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/tagged_ptr.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5875 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/tagged_ptr_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7032 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/test_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2067 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/internal/test_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     9371 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/internal/thread_pool.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1260 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/thread_pool.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3558 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/internal/thread_pool_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18427 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/type_traits.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8473 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/internal/type_traits_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6238 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/unique_with_intrusive_allocator.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2395 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/unique_with_intrusive_allocator_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1369 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/unowned_to_shared.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4184 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/utf8.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/utf8.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2981 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/utf8_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3462 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/void_wrapper.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3125 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/internal/void_wrapper_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3377 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/json_serialization_options.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.125687 tensorstore-0.1.9/tensorstore/kvstore/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5737 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1725 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/byte_range.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3643 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/byte_range.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5235 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/byte_range_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.125687 tensorstore-0.1.9/tensorstore/kvstore/file/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2780 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/file/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    32642 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/file/file_key_value_store.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20758 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/file/file_key_value_store_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      736 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/file/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4754 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/file/posix_file_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10976 2021-01-13 22:02:59.000000 tensorstore-0.1.9/tensorstore/kvstore/file/posix_file_util.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      694 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/file/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2039 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/file/unique_handle.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12462 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/file/windows_file_util.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4843 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/file/windows_file_util.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.125687 tensorstore-0.1.9/tensorstore/kvstore/gcs/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3385 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    32967 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_key_value_store.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20408 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_key_value_store_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16010 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_mock.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4390 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_mock.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2428 2020-08-25 23:48:07.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6190 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2641 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7032 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3700 2020-07-29 01:03:09.000000 tensorstore-0.1.9/tensorstore/kvstore/gcs/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4331 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/generation.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11197 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/generation.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2554 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/generation_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3760 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/generation_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      490 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5056 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/key_range.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4518 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/key_range.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7351 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/key_range_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8776 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/key_value_store.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    33186 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/key_value_store.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1456 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/key_value_store_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20189 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/key_value_store_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8419 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/key_value_store_testutil.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.129686 tensorstore-0.1.9/tensorstore/kvstore/memory/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1890 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      385 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/index.rst
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20737 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1348 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10714 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1666 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/memory/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13669 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/registry.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      680 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/kvstore/schema.yml
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    60416 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/transaction.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    27920 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/kvstore/transaction.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    35341 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/make_array.inc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1860 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/non_compile.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1800 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/open.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4138 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/open.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1658 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/open_mode.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5344 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/open_mode.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4599 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/open_mode_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2381 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/progress.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3647 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/progress.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2268 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/progress_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1137 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/rank.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14053 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/rank.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6942 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/rank_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3595 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/read_write_options.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1596 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/resize_options.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4148 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/resize_options.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/resize_options_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2098 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/spec.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4202 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/spec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1178 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/spec_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2473 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/spec_request_options.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7503 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/spec_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3334 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/staleness_bound.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1017 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/static_cast.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12240 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/static_cast.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7779 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/static_cast_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1688 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/strided_layout.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    41904 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/strided_layout.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    42899 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/strided_layout_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1134 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/tensorstore.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2270 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/tensorstore.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23286 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/tensorstore.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    13458 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/tensorstore_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19541 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/transaction.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10813 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/transaction.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    39108 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/transaction_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    22625 2020-10-10 00:09:50.000000 tensorstore-0.1.9/tensorstore/transaction_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2843 2020-04-18 03:06:59.000000 tensorstore-0.1.9/tensorstore/update_generated_source_code.py
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.133686 tensorstore-0.1.9/tensorstore/util/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16168 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/BUILD
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2053 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/assert_macros.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      818 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/assert_macros_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15174 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/bit_span.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    14756 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/bit_span_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8144 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/bit_vec.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2118 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/bit_vec_impl.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3611 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/bit_vec_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    12255 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/bit_vec_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5774 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/byte_strided_pointer.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5599 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/byte_strided_pointer_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3010 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/collecting_sender.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1921 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/collecting_sender_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1902 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/constant_bit_vector.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2113 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/constant_bit_vector_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2602 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/constant_vector.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7892 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/constant_vector.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3754 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/constant_vector_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1636 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/default_iteration_result.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      917 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/default_iteration_result_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5267 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/division.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1019 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/division_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1025 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/element_pointer.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19732 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/util/element_pointer.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    18292 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/element_pointer_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3772 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/element_traits.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3574 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/element_traits_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2664 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/endian.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4862 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/execution.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3053 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/executor.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2154 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/executor_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7194 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/extents.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6028 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/extents_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3441 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/function_view.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2801 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/function_view_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16267 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/util/future.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    48971 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/util/future.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    59713 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/util/future_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7017 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/future_sender_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    57639 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/util/future_test.cc
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/tensorstore/util/internal/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4502 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/internal/iterate.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11913 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/internal/iterate_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8659 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/iterate.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10246 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/util/iterate.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     8762 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/iterate_over_index_range.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5271 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/iterate_over_index_range_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23132 2020-11-30 23:09:09.000000 tensorstore-0.1.9/tensorstore/util/iterate_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      884 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/quote_string.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1106 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/quote_string.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      918 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/quote_string_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    29465 2021-01-13 22:01:20.000000 tensorstore-0.1.9/tensorstore/util/result.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10934 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/result_impl.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1920 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/result_nc_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2772 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/result_sender_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    28679 2020-05-28 22:28:53.000000 tensorstore-0.1.9/tensorstore/util/result_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    16093 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/sender.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    11163 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/sender_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2464 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/sender_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    15027 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/span.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1062 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/span_json.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      967 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/span_json_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    20313 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/span_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1557 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/status.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     6408 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/status.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2979 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/status_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     2371 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/status_testutil.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3468 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/status_testutil.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3429 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/str_cat.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1858 2020-06-29 03:39:52.000000 tensorstore-0.1.9/tensorstore/util/str_cat_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3600 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/sync_flow_sender.h
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3091 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/sync_flow_sender_test.cc
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1706 2020-04-18 03:07:00.000000 tensorstore-0.1.9/tensorstore/util/utf8_string.h
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      203 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/BUILD
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_facebook_zstd/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      589 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_facebook_zstd/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/com_facebook_zstd/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1211 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_facebook_zstd/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_github_nlohmann_json/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      333 2020-11-30 23:09:09.000000 tensorstore-0.1.9/third_party/com_github_nlohmann_json/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1117 2020-11-30 23:09:09.000000 tensorstore-0.1.9/third_party/com_github_nlohmann_json/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_github_pybind_pybind11/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      423 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/com_github_pybind_pybind11/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1138 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_github_pybind_pybind11/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_google_absl/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1141 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_google_absl/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_google_benchmark/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1027 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_google_benchmark/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_google_boringssl/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      261 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/com_google_boringssl/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1247 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_google_boringssl/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_google_googletest/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1121 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_google_googletest/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/com_google_snappy/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     3928 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/com_google_snappy/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      106 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/com_google_snappy/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1189 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/com_google_snappy/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/jpeg/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23707 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/jpeg/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/jpeg/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1379 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/jpeg/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/nasm/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4102 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/nasm/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       53 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/nasm/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1183 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/nasm/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/net_sourceforge_half/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      318 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/net_sourceforge_half/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1109 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/net_sourceforge_half/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/net_zlib/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1259 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/net_zlib/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)       99 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/net_zlib/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1169 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/net_zlib/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/org_blosc_cblosc/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4141 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_blosc_cblosc/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      104 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_blosc_cblosc/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1213 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_blosc_cblosc/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/org_lz4/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      961 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_lz4/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      100 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_lz4/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1174 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_lz4/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.137687 tensorstore-0.1.9/third_party/org_nghttp2/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5616 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_nghttp2/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      108 2020-06-29 03:39:52.000000 tensorstore-0.1.9/third_party/org_nghttp2/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1228 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_nghttp2/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/third_party/org_sourceware_bzip2/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      513 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_sourceware_bzip2/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_sourceware_bzip2/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1221 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_sourceware_bzip2/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/third_party/org_tukaani_xz/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    24299 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_tukaani_xz/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      100 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/org_tukaani_xz/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1176 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/org_tukaani_xz/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/third_party/pypa/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5942 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/pypa/generate_workspace.py
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    23990 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/pypa/workspace.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/third_party/python/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1899 2020-04-18 03:07:00.000000 tensorstore-0.1.9/third_party/python/BUILD.tpl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    10317 2020-04-29 01:47:28.000000 tensorstore-0.1.9/third_party/python/python_configure.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     5259 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/repo.bzl
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/third_party/se_curl/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)    19573 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/se_curl/bundled.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      102 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/se_curl/system.BUILD.bazel
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     1174 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/se_curl/workspace.bzl
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     7765 2021-01-13 22:01:20.000000 tensorstore-0.1.9/third_party/update_versions.py
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.045687 tensorstore-0.1.9/tools/
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/tools/python-manylinux/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      239 2020-04-29 01:47:28.000000 tensorstore-0.1.9/tools/python-manylinux/README.md
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)      635 2020-04-29 01:47:28.000000 tensorstore-0.1.9/tools/python-manylinux/build_wheels_inside_container.sh
+-rwxr-xr-x   0 jbms     (297878) primarygroup (89939)     1372 2020-04-29 01:47:28.000000 tensorstore-0.1.9/tools/python-manylinux/build_wheels_manylinux2014_x86_64.sh
+drwxr-xr-x   0 jbms     (297878) primarygroup (89939)        0 2021-01-13 22:04:08.141687 tensorstore-0.1.9/tools/python-manylinux/manylinux2014_x86_64/
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)      331 2020-04-29 01:47:28.000000 tensorstore-0.1.9/tools/python-manylinux/manylinux2014_x86_64/Dockerfile
+-rw-r--r--   0 jbms     (297878) primarygroup (89939)     4419 2020-04-18 03:06:59.000000 tensorstore-0.1.9/utils.bzl
```

### Comparing `tensorstore-0.1.8/CONTRIBUTING.md` & `tensorstore-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/LICENSE` & `tensorstore-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/README.md` & `tensorstore-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/bazelisk.py` & `tensorstore-0.1.9/bazelisk.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/_static/sphinx_rtd_theme_table_word_wrap_fix.css` & `tensorstore-0.1.9/docs/_static/sphinx_rtd_theme_table_word_wrap_fix.css`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/_templates/autosummary/class.rst` & `tensorstore-0.1.9/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/_templates/autosummary/module.rst` & `tensorstore-0.1.9/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/_templates/autosummary_root_module.rst` & `tensorstore-0.1.9/docs/_templates/autosummary_root_module.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/conf.py` & `tensorstore-0.1.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 copyright = '2020 The TensorStore Authors'  # pylint: disable=redefined-builtin
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
 release = ''
 
+# Override default of `utf-8-sig` which can cause problems with autosummary due
+# to the extra Unicode Byte Order Mark that gets inserted.
+source_encoding = 'utf-8'
+
+# Don't include "View page source" links, since they aren't very helpful,
+# especially for generated pages.
+html_show_sourcelink = False
+
 extensions = [
     'sphinx_rtd_theme',
     'tensorstore_jsonschema_sphinx',
     'sphinx.ext.intersphinx',
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
     'sphinx.ext.autosummary',
@@ -34,14 +42,15 @@
     'sphinx.ext.mathjax',
 ]
 
 exclude_patterns = [
     # This is included directly by `python/api/index.rst`, so we don't want to
     # generate a separate page for it.
     'python/api/tensorstore.rst',
+    '_templates/**',
 ]
 
 source_suffix = '.rst'
 master_doc = 'index'
 language = None
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -52,18 +61,22 @@
 html_static_path = ['_static']
 templates_path = ['_templates']
 html_context = {
     'css_files': ['_static/sphinx_rtd_theme_table_word_wrap_fix.css',],
 }
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3', None),
-    'zarr': ('https://zarr.readthedocs.io/en/stable', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
-    'dask': ('https://docs.dask.org/en/latest/', None),
+    'python':
+        ('https://docs.python.org/3', ('intersphinx_inv/python3.inv', None)),
+    'zarr': ('https://zarr.readthedocs.io/en/stable',
+             ('intersphinx_inv/zarr.inv', None)),
+    'numpy':
+        ('https://numpy.org/doc/stable/', ('intersphinx_inv/numpy.inv', None)),
+    'dask': ('https://docs.dask.org/en/latest/', ('intersphinx_inv/dask.inv',
+                                                  None)),
 }
 
 rst_prolog = """
 .. role:: python(code)
    :language: python
    :class: highlight
```

### Comparing `tensorstore-0.1.8/docs/context.rst` & `tensorstore-0.1.9/docs/context.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/context_schema.yml` & `tensorstore-0.1.9/docs/context_schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/environment.rst` & `tensorstore-0.1.9/docs/environment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
    store.  In most cases, the system CA certificate store should instead be
    specified using :envvar:`TENSORSTORE_CA_BUNDLE`.
 
 .. note::
 
    On Linux and BSD, TensoprStore may optionally be built to dynamically link to
    a system-provided version of libcurl by specifying
-   :envvar:`TENSORSTORE_SYSTEM_LIBS=se_haxx_curl<TENSORSTORE_SYSTEM_LIBS>`.  In
+   :envvar:`TENSORSTORE_SYSTEM_LIBS=se_curl<TENSORSTORE_SYSTEM_LIBS>`.  In
    this case, the default CA bundle path of
    :file:`/etc/ssl/certs/ca-certificates.crt` does not apply; instead, the
    default depends on how the system-provided libcurl was built, and most likely
    no additional configuration will be necessary.
 
 Proxy configuration
 ^^^^^^^^^^^^^^^^^^^
```

### Comparing `tensorstore-0.1.8/docs/index_space.rst` & `tensorstore-0.1.9/docs/index_space.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 .. note::
 
    The limits of :math:`\pm (2^{62}-2)` permit :math:`\pm (2^{62}-1)` to be
    reserved to represent :math:`\pm \infty` and still allow the
    difference between any two bounds to be represented as a signed
    64-bit integer.
 
+TensorStore currently supports ranks :math:`n` less than or equal to 32, which
+is the same constraint imposed by NumPy.
+
 .. _dimension-labels:
 
 Each of the :math:`n` dimensions may optionally be identified by a unique
 string *label*, such as ``"x"``, ``"y"``, or ``"z"``.  Unlabeled
 dimensions are indicated by an empty string as the label.
 
 .. _implicit-bounds:
@@ -51,14 +54,17 @@
    :math:`[-(2^{62}-2, +(2^{62}-2)]`, in that in both cases the domain
    contains the full range of possible indices.  The difference is
    that translating a dimension with infinite bounds has no effect,
    while translating a dimension with bounds :math:`[-(2^{62}-2,
    +(2^{62}-2)]` by any non-zero offset results in an out-of-bounds
    error.
 
+.. json-schema:: index_domain_schema.yml
+   :title: JSON Schema
+
 .. _index-transform:
 
 Index transform
 ---------------
 
 An *index transform* from rank :math:`m` to rank :math:`n` maps every
 :math:`m`-dimensional index vector in a rank-:math:`m` :ref:`index
@@ -111,14 +117,17 @@
 copying any index arrays.  Only when composing two index array maps is
 it necessary to write a new index array, and in some cases this can
 result in index array with a larger representation size.
 
 .. json-schema:: index_transform_schema.yml
    :title: JSON Schema
 
+.. json-schema:: index_transform_schema.yml#/definitions/index-interval
+   :title: Index interval JSON Schema
+
 .. _index-domain-alignment:
 
 Alignment and broadcasting
 --------------------------
 
 Many operations in TensorStore involving two :ref:`index domains<index-domain>`,
 such as read, write, and copy operations, automatically *align* the ``source``
```

### Comparing `tensorstore-0.1.8/docs/index_transform_schema.yml` & `tensorstore-0.1.9/docs/index_transform_schema.yml`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   bound of :math:`+\infty`.
 
 type: object
 properties:
   input_rank:
     type: integer
     minimum: 0
+    maximum: 32
     title: Number of input dimensions.
     description: |
       The input rank must be specified either directly, or implicitly by the
       number of dimensions specified for :json-member:`input_inclusive_min`,
       :json-member:`input_inclusive_max`, :json-member:`input_exclusive_max`,
       :json-member:`input_shape`, or :json-member:`input_labels`.
   input_inclusive_min:
@@ -40,31 +41,33 @@
         - type: integer
         - type: array
           items:
             - type: integer
     title: |
       Inclusive lower bounds of the input domain.
     description: |
-      Length must equal the :json-member:`input_rank`.  Bounds specified as :samp:`{n}` indicate normal, explicit bounds, while
-      bounds specified as :samp:`[{n}]` indicate `implicit
-      bounds<implicit-bounds>`.  For example, :json:`[1, [2]]` specifies an
-      explicit bound of :math:`1 \leq x` for the first dimension and an implicit
-      bound of :math:`2 \leq x` for the second dimension.
+      Length must equal the :json-member:`input_rank`.  Bounds specified as
+      :samp:`{n}` indicate normal, explicit bounds, while bounds specified as
+      :samp:`[{n}]` indicate `implicit bounds<implicit-bounds>`.  For example,
+      :json:`[1, [2]]` specifies an explicit bound of :math:`1 \leq x` for the
+      first dimension and an implicit bound of :math:`2 \leq x` for the second
+      dimension.
   input_exclusive_max:
     type: array
     items:
       oneOf:
         - type: integer
         - type: array
           items:
             - type: integer
     title: |
       Exclusive upper bounds of the input domain.
     description: |
-      Length must equal the :json-member:`input_rank`.  As for :json-member:`input_inclusive_min`, bounds specified as :samp:`{n}`
+      Length must equal the :json-member:`input_rank`.  As for
+      :json-member:`input_inclusive_min`, bounds specified as :samp:`{n}`
       indicate normal, explicit bounds, while bounds specified as :samp:`[{n}]`
       indicate `implicit bounds<implicit-bounds>`.  For example, :json:`[5,
       [7]]` specifies an explicit bound of :math:`x < 5` for the first dimension
       and an implicit bound of :math:`x < 7` for the second dimension.
   input_inclusive_max:
     type: array
     items:
@@ -151,7 +154,38 @@
             - type: integer
           title: |
             If present, indicates that this output dimension uses an **index
             array** map, with the index array specified as a nested list of rank
             equal to :json-member:`input_rank`.
           description: |
             If the input rank is 0, must be a numeric value.
+        index_array_bounds:
+          $ref: https://github.com/google/tensorstore/json-schema/index-interval
+          description: |
+            If present, specifies constraints on the values within
+            :json-member:`index_array` (which must also be specified).  If
+            :json-member:`index_array` contains an out-of-bounds index, an error
+            may not be returned immediately but will be returned if the
+            corresponding position within the domain is accessed.  If the
+            indices in :json-member:`index_array` have already been validated,
+            this need not be specified.  This allows transforms containing
+            out-of-bounds index array indices to correctly round trip through
+            JSON, but normally need not be specified manually.
+          default: ["-inf", "+inf"]
+          examples:
+            - [5, 100]
+            - ["-inf", 10]
+            - [-20, "+inf"]
+definitions:
+  index-interval:
+    $id: https://github.com/google/tensorstore/json-schema/index-interval
+    title: Index interval
+    description: >-
+      Specifies a closed interval of integer index values.
+    type: array
+    items:
+      - oneOf:
+          - type: integer
+          - const: "-inf"
+      - oneOf:
+          - type: integer
+          - const: "+inf"
```

### Comparing `tensorstore-0.1.8/docs/installation.rst` & `tensorstore-0.1.9/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -189,9 +189,9 @@
 .. include:: third_party_libraries.rst
 
 For example, to run the tests using the system-provided curl, jpeg, and SSL
 libraries:
 
 .. code-block:: shell
 
-   export TENSORSTORE_SYSTEM_LIBS=se_haxx_curl,jpeg,com_google_boringssl
+   export TENSORSTORE_SYSTEM_LIBS=se_curl,jpeg,com_google_boringssl
    python bazelisk.py test //...
```

### Comparing `tensorstore-0.1.8/docs/overview.rst` & `tensorstore-0.1.9/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/python/indexing.rst` & `tensorstore-0.1.9/docs/python/indexing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -994,19 +994,19 @@
 
 - a non-empty `str`, specifying an existing dimension by label;
 
 - a `slice` object, :python:`start:stop:step`, where :python:`start`,
   :python:`stop`, and :python:`step` are either integers or `None`,
   specifying a range of existing or new dimensions by index (as for built-in sequence types, negative numbers specify a dimension index relative to the end);
 
-- any sequence (including a `tuple`, `list`, or another `tensorstore.DimensionSelection` object) of any of the above.
+- any sequence (including a `tuple`, `list`, or another `tensorstore.d` object) of any of the above.
 
-The result is a `tensorstore.DimensionSelection`, which is simply a
-lightweight, immutable container representing the flattened sequence
-of `int`, `str`, or `slice` objects:
+The result is a `tensorstore.d` object, which is simply a lightweight, immutable
+container representing the flattened sequence of `int`, `str`, or `slice`
+objects:
 
 .. doctest::
 
    >>> ts.d[0, 1, 2]
    d[0,1,2]
    >>> ts.d[0:1, 2, "x"]
    d[0:1,2,'x']
@@ -1170,17 +1170,16 @@
 
 .. _python-dim-expression-numpy-indexing:
 
 NumPy-style dimension expression indexing
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The syntax :python:`dexpr[iexpr]`, :python:`dexpr.vindex[iexpr]`, and
-:python:`dexpr.oindex[iexpr]` chains a NumPy-style indexing operation
-to an existing `tensorstore.DimensionSelection` or
-`tensorstore.DimExpression`.
+:python:`dexpr.oindex[iexpr]` chains a NumPy-style indexing operation to an
+existing `tensorstore.d` or `tensorstore.DimExpression`.
 
 The behavior is similar to that of regular `NumPy-style
 indexing<python-numpy-style-indexing>` applied directly to a
 `tensorstore.Indexable` object, with the following differences:
 
 - The terms of the indexing expression :python:`iexpr` consume
   dimensions in order from the dimension selection rather than
```

### Comparing `tensorstore-0.1.8/docs/python/tutorial.rst` & `tensorstore-0.1.9/docs/python/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/docs/tensorstore_schema.yml` & `tensorstore-0.1.9/docs/tensorstore_schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/external.bzl` & `tensorstore-0.1.9/external.bzl`

 * *Files 27% similar despite different names*

```diff
@@ -22,33 +22,24 @@
 load("//third_party:com_google_benchmark/workspace.bzl", repo_com_google_benchmark = "repo")
 load("//third_party:net_zlib/workspace.bzl", repo_net_zlib = "repo")
 load("//third_party:org_sourceware_bzip2/workspace.bzl", repo_org_sourceware_bzip2 = "repo")
 load("//third_party:com_google_snappy/workspace.bzl", repo_com_google_snappy = "repo")
 load("//third_party:com_github_nlohmann_json/workspace.bzl", repo_com_github_nlohmann_json = "repo")
 load("//third_party:net_sourceforge_half/workspace.bzl", repo_net_sourceforge_half = "repo")
 load("//third_party:org_nghttp2/workspace.bzl", repo_org_nghttp2 = "repo")
-load("//third_party:se_haxx_curl/workspace.bzl", repo_se_haxx_curl = "repo")
+load("//third_party:se_curl/workspace.bzl", repo_se_curl = "repo")
 load("//third_party:com_google_boringssl/workspace.bzl", repo_com_google_boringssl = "repo")
 load("//third_party:org_lz4/workspace.bzl", repo_org_lz4 = "repo")
 load("//third_party:com_facebook_zstd/workspace.bzl", repo_com_facebook_zstd = "repo")
 load("//third_party:org_blosc_cblosc/workspace.bzl", repo_org_blosc_cblosc = "repo")
 load("//third_party:nasm/workspace.bzl", repo_nasm = "repo")
 load("//third_party:org_tukaani_xz/workspace.bzl", repo_org_tukaani_xz = "repo")
 load("//third_party:python/python_configure.bzl", "python_configure")
 load("//third_party:com_github_pybind_pybind11/workspace.bzl", repo_com_github_pybind_pybind11 = "repo")
-load("//third_party:pypa/numpy/workspace.bzl", repo_pypa_numpy = "repo")
-load("//third_party:pypa/pytest/workspace.bzl", repo_pypa_pytest = "repo")
-load("//third_party:pypa/absl_py/workspace.bzl", repo_pypa_absl_py = "repo")
-load("//third_party:pypa/pytest_asyncio/workspace.bzl", repo_pypa_pytest_asyncio = "repo")
-load("//third_party:pypa/ipython/workspace.bzl", repo_pypa_ipython = "repo")
-load("//third_party:pypa/wheel/workspace.bzl", repo_pypa_wheel = "repo")
-load("//third_party:pypa/sphinx/workspace.bzl", repo_pypa_sphinx = "repo")
-load("//third_party:pypa/sphinx_autobuild/workspace.bzl", repo_pypa_sphinx_autobuild = "repo")
-load("//third_party:pypa/apache_beam/workspace.bzl", repo_pypa_apache_beam = "repo")
-load("//third_party:pypa/gin_config/workspace.bzl", repo_pypa_gin_config = "repo")
+load("//third_party:pypa/workspace.bzl", repo_pypa = "repo")
 
 def _bazel_dependencies():
     maybe(
         http_archive,
         name = "bazel_skylib",
         url = "https://github.com/bazelbuild/bazel-skylib/releases/download/0.9.0/bazel_skylib-0.9.0.tar.gz",
         sha256 = "1dde365491125a3db70731e25658dfdd3bc5dbdfd11b840b3e987ecf043c7ca0",
@@ -60,39 +51,30 @@
         url = "https://github.com/bazelbuild/rules_python/releases/download/0.0.1/rules_python-0.0.1.tar.gz",
         sha256 = "aa96a691d3a8177f3215b14b0edc9641787abaaa30363a080165d06ab65e1161",
     )
 
 def _python_dependencies():
     python_configure(name = "local_config_python")
     repo_com_github_pybind_pybind11()
-    repo_pypa_numpy()
-    repo_pypa_absl_py()
-    repo_pypa_pytest()
-    repo_pypa_pytest_asyncio()
-    repo_pypa_ipython()
-    repo_pypa_wheel()
-    repo_pypa_sphinx()
-    repo_pypa_sphinx_autobuild()
-    repo_pypa_apache_beam()
-    repo_pypa_gin_config()
+    repo_pypa()
 
 def _cc_dependencies():
     repo_com_google_absl()
     repo_com_google_googletest()
     repo_com_google_benchmark()
     repo_nasm()
     repo_jpeg()
     repo_com_google_boringssl()
     repo_net_zlib()
     repo_org_sourceware_bzip2()
     repo_com_google_snappy()
     repo_com_github_nlohmann_json()
     repo_net_sourceforge_half()
     repo_org_nghttp2()
-    repo_se_haxx_curl()
+    repo_se_curl()
     repo_org_lz4()
     repo_com_facebook_zstd()
     repo_org_blosc_cblosc()
     repo_org_tukaani_xz()
 
 def tensorstore_dependencies():
     _bazel_dependencies()
```

### Comparing `tensorstore-0.1.8/python/tensorstore/BUILD` & `tensorstore-0.1.9/python/tensorstore/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pybind11_py_extension(
     name = "_tensorstore",
     srcs = ["tensorstore.cc"],
     imports = [".."],
     deps = [
         ":context",
         ":data_type",
+        ":downsample",
         ":future",
         ":index_space",
         ":spec",
         ":tensorstore_class",
         ":transaction",
         ":write_futures",
         "//tensorstore:all_drivers",
@@ -95,14 +96,24 @@
     srcs = ["tests/index_transform_test.py"],
     deps = [
         ":tensorstore",
         "@pypa_numpy//:numpy",
     ],
 )
 
+tensorstore_pytest_test(
+    name = "downsample_test",
+    size = "small",
+    srcs = ["tests/downsample_test.py"],
+    deps = [
+        ":tensorstore",
+        "@pypa_numpy//:numpy",
+    ],
+)
+
 pybind11_cc_library(
     name = "subscript_method",
     hdrs = ["subscript_method.h"],
     deps = [
         "//tensorstore/internal:type_traits",
         "//tensorstore/util:str_cat",
         "@com_github_pybind_pybind11//:pybind11",
@@ -481,7 +492,24 @@
     hdrs = ["transaction.h"],
     deps = [
         ":future",
         "//tensorstore:transaction",
         "@com_github_pybind_pybind11//:pybind11",
     ],
 )
+
+pybind11_cc_library(
+    name = "downsample",
+    srcs = ["downsample.cc"],
+    hdrs = ["downsample.h"],
+    deps = [
+        ":index",
+        ":result_type_caster",
+        ":spec",
+        ":status",
+        "//tensorstore:downsample",
+        "//tensorstore:downsample_method",
+        "//tensorstore:spec",
+        "//tensorstore/driver/downsample:downsample_method_json_binder",
+        "@com_github_pybind_pybind11//:pybind11",
+    ],
+)
```

### Comparing `tensorstore-0.1.8/python/tensorstore/LICENSE` & `tensorstore-0.1.9/python/tensorstore/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/__init__.py` & `tensorstore-0.1.9/python/tensorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/array_type_caster.cc` & `tensorstore-0.1.9/python/tensorstore/array_type_caster.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/array_type_caster.h` & `tensorstore-0.1.9/python/tensorstore/array_type_caster.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/bazel_pytest_main.py` & `tensorstore-0.1.9/python/tensorstore/bazel_pytest_main.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/context.cc` & `tensorstore-0.1.9/python/tensorstore/context.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/context.h` & `tensorstore-0.1.9/python/tensorstore/context.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/data_type.cc` & `tensorstore-0.1.9/python/tensorstore/data_type.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/data_type.h` & `tensorstore-0.1.9/python/tensorstore/data_type.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/dim_expression.cc` & `tensorstore-0.1.9/python/tensorstore/dim_expression.cc`

 * *Files 4% similar despite different names*

```diff
@@ -301,44 +301,81 @@
   }
 
  private:
   std::shared_ptr<const DimensionSelection> parent_;
   IndexingSpec spec_;
 };
 
+namespace {
+
+PyTypeObject* GetClassGetitemMetaclass() {
+#if PY_VERSION_HEX < 0x030700000
+  // Polyfill __class_getitem__ support for Python < 3.7
+  static auto* metaclass = [] {
+    PyTypeObject* base_metaclass =
+        pybind11::detail::get_internals().default_metaclass;
+    PyType_Slot slots[] = {
+        {Py_tp_base, base_metaclass},
+        {Py_mp_subscript,
+         (void*)+[](PyObject* self, PyObject* arg) -> PyObject* {
+           auto method = py::reinterpret_steal<py::object>(
+               PyObject_GetAttrString(self, "__class_getitem__"));
+           if (!method.ptr()) return nullptr;
+           return PyObject_CallFunctionObjArgs(method.ptr(), arg, nullptr);
+         }},
+        {0},
+    };
+    PyType_Spec spec = {};
+    spec.name = "tensorstore._Metaclass";
+    spec.basicsize = base_metaclass->tp_basicsize;
+    spec.flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE;
+    spec.slots = slots;
+    PyTypeObject* metaclass = (PyTypeObject*)PyType_FromSpec(&spec);
+    if (!metaclass) throw py::error_already_set();
+    return metaclass;
+  }();
+  return metaclass;
+#else  // Python version >= 3.7 supports __class_getitem__ natively.
+  return nullptr;
+#endif
+}
+}  // namespace
+
 void RegisterDimExpressionBindings(pybind11::module m) {
   py::class_<PythonDimExpressionBase, std::shared_ptr<PythonDimExpressionBase>>
       dim_expression_base(m, "_DimExpressionBase");
+
   py::class_<DimensionSelection, PythonDimExpressionBase,
              std::shared_ptr<DimensionSelection>>
       dimension_selection_class(
-          m, "DimensionSelection",
-          "Specifies a sequence of index space dimensions.");
-  dimension_selection_class.def(
-      "__eq__", [](const DimensionSelection& a, const DimensionSelection& b) {
-        return a.dims == b.dims;
-      });
+          m, "d", py::metaclass((PyObject*)GetClassGetitemMetaclass()),
+          R"(Specifies a dimension selection, a sequence of index space dimensions.
+
+:ref:`python-dim-selections` may be used as part of a
+`dimension expression<python-dim-expression-construction>` to specify the
+dimensions to which an indexing operation applies.
+)");
+  dimension_selection_class
+      .def("__eq__",
+           [](const DimensionSelection& a, const DimensionSelection& b) {
+             return a.dims == b.dims;
+           })
+      .def_static(
+          "__class_getitem__",
+          [](const DimensionSelection& selection) { return selection; },
+          py::arg("selection"));
 
   DefineIndexingMethods<IndexingSpec::Usage::kDimSelectionInitial>(
       &dimension_selection_class,
       [](std::shared_ptr<DimensionSelection> self,
          IndexingSpec spec) -> std::shared_ptr<PythonDimExpression> {
         return std::make_shared<PythonInitialIndexOp>(std::move(self),
                                                       std::move(spec));
       });
 
-  struct DimensionSelectionHelper {};
-  py::class_<DimensionSelectionHelper> cls_dimension_selection_helper(
-      m, "_DimensionSelectionHelper");
-  cls_dimension_selection_helper.def(
-      "__getitem__",
-      [](const DimensionSelectionHelper& self,
-         const DimensionSelection& selection) { return selection; });
-  cls_dimension_selection_helper.attr("__iter__") = py::none();
-  m.attr("d") = DimensionSelectionHelper{};
   m.attr("newaxis") = py::none();
 
   py::class_<PythonDimExpression, PythonDimExpressionBase,
              std::shared_ptr<PythonDimExpression>>
       dim_expression_class(m, "DimExpression");
 
   DefineIndexingMethods<IndexingSpec::Usage::kDimSelectionChained>(
```

### Comparing `tensorstore-0.1.8/python/tensorstore/dim_expression.h` & `tensorstore-0.1.9/python/tensorstore/dim_expression.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/future.cc` & `tensorstore-0.1.9/python/tensorstore/future.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/future.h` & `tensorstore-0.1.9/python/tensorstore/future.h`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,29 @@
 ///
 /// We can't simply use the normal `tensorstore::Future<T>::Wait` method, since
 /// that does not support interruption.
 template <typename T>
 typename Future<T>::result_type& InterruptibleWait(const Future<T>& future) {
   assert(future.valid());
   if (!future.ready() && _PyOS_IsMainThread()) {
+    {
+      pybind11::gil_scoped_release gil_release;
+      future.Force();
+    }
     // If on main thread and not already ready, use "interruptible" wait that
     // may throw a KeyboardInterrupt exception if SIGINT is received.
     internal_python::InterruptibleWaitImpl([&](auto signal) {
       return future.ExecuteWhenReady(
           [signal = std::move(signal)](ReadyFuture<const T> f) { signal(); });
     });
   }
-  return future.result();
+  {
+    pybind11::gil_scoped_release gil_release;
+    return future.result();
+  }
 }
 
 /// Base class that represents a Future exposed to Python.
 ///
 /// This provides an interface similar to the `concurrent.futures.Future` Python
 /// type, but also is directly compatible with asyncio (via `await`).
 ///
@@ -215,15 +222,18 @@
       callback(pybind11::cast(shared_from_this()));
       return;
     }
     callbacks_.push_back(callback);
     if (callbacks_.size() == 1) {
       registration_.Unregister();
       auto self = std::static_pointer_cast<PythonFuture<T>>(shared_from_this());
-      future_.Force();
+      {
+        pybind11::gil_scoped_release gil_release;
+        future_.Force();
+      }
       registration_ = future_.ExecuteWhenReady([self](Future<const T> future) {
         pybind11::gil_scoped_acquire gil_acquire;
         self->RunCallbacks();
       });
     }
   }
```

### Comparing `tensorstore-0.1.8/python/tensorstore/index.cc` & `tensorstore-0.1.9/python/tensorstore/index.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/index.h` & `tensorstore-0.1.9/python/tensorstore/index.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/index_space.cc` & `tensorstore-0.1.9/python/tensorstore/index_space.cc`

 * *Files 1% similar despite different names*

```diff
@@ -185,23 +185,28 @@
     const char* input_shape_field_name,
     const std::optional<std::vector<bool>>& implicit_upper_bounds,
     const std::optional<std::vector<std::optional<std::string>>>& input_labels,
     const char* input_labels_field_name,
     std::optional<DimensionIndex> output_rank) {
   const char* input_rank_field = nullptr;
   if (input_rank) {
-    if (*input_rank < 0) {
+    if (!IsValidRank(*input_rank)) {
       throw py::value_error(
           StrCat("Invalid ", input_rank_field_name, ": ", *input_rank));
     }
     input_rank_field = input_rank_field_name;
   }
 
   const auto check_rank = [&](DimensionIndex rank, const char* field_name) {
     if (!input_rank) {
+      if (!IsValidRank(rank)) {
+        throw py::value_error(StrCat("Rank specified by `", field_name, "` (",
+                                     rank, ") exceeds maximum rank of ",
+                                     kMaxRank));
+      }
       input_rank = rank;
       input_rank_field = field_name;
     } else if (*input_rank != rank) {
       throw py::value_error(StrCat("Rank specified by `", field_name, "` (",
                                    rank, ") does not match rank specified by `",
                                    input_rank_field, "` (", *input_rank, ")"));
     }
@@ -239,14 +244,19 @@
   }
   if (input_labels) {
     check_rank(input_labels->size(), input_labels_field_name);
   }
   if (!input_rank) {
     throw py::value_error(StrCat("Must specify `", input_rank_field_name, "`"));
   }
+  if (output_rank && !IsValidRank(*output_rank)) {
+    throw py::value_error(
+        tensorstore::StrCat("Number of output dimensions (", *output_rank,
+                            ") exceeds maximum rank of ", kMaxRank));
+  }
   auto builder =
       IndexTransformBuilder<>(*input_rank, output_rank.value_or(*input_rank));
   if (input_inclusive_min) {
     builder.input_origin(*input_inclusive_min);
   }
   if (implicit_lower_bounds) {
     builder.implicit_lower_bounds(*implicit_lower_bounds);
```

### Comparing `tensorstore-0.1.8/python/tensorstore/index_space.h` & `tensorstore-0.1.9/python/tensorstore/index_space.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/index_test.cc` & `tensorstore-0.1.9/python/tensorstore/index_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/indexing_spec.cc` & `tensorstore-0.1.9/python/tensorstore/indexing_spec.cc`

 * *Files 0% similar despite different names*

```diff
@@ -408,14 +408,15 @@
     const IndexingSpec& spec, IndexDomainView<> output_space,
     span<const DimensionIndex> indexed_output_dims,
     span<const DimensionIndex> indexed_input_dims,
     span<const DimensionIndex> unindexed_input_dims) {
   const DimensionIndex num_ellipsis_dims =
       indexed_output_dims.size() - spec.num_output_dims;
   const DimensionIndex input_rank = unindexed_input_dims.size();
+  ThrowStatusException(ValidateRank(input_rank));
   IndexTransformBuilder<> builder(input_rank, output_space.rank());
   DimensionIndex selected_input_dim_i = 0;
   DimensionIndex index_array_input_start_dim_i = -1;
   DimensionIndex selected_output_dim_i = 0;
   auto input_origin = builder.input_origin();
   auto input_shape = builder.input_shape();
   auto implicit_lower_bounds = builder.implicit_lower_bounds();
```

### Comparing `tensorstore-0.1.8/python/tensorstore/indexing_spec.h` & `tensorstore-0.1.9/python/tensorstore/indexing_spec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/intrusive_ptr_holder.h` & `tensorstore-0.1.9/python/tensorstore/intrusive_ptr_holder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/json_type_caster.cc` & `tensorstore-0.1.9/python/tensorstore/json_type_caster.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/json_type_caster.h` & `tensorstore-0.1.9/python/tensorstore/json_type_caster.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/pybind11.bzl` & `tensorstore-0.1.9/python/tensorstore/pybind11.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/pytest.bzl` & `tensorstore-0.1.9/python/tensorstore/pytest.bzl`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,14 @@
         args = []
     if deps == None:
         deps = []
     deps.append("@pypa_pytest//:pytest")
     deps.append("@pypa_pytest_asyncio//:pytest_asyncio")
     native.py_test(
         name = name,
-        args = args + ["-vv", "--pyargs"] + ["$(rootpath %s)" % test for test in tests],
+        args = args + ["-vv", "-s", "--pyargs"] + ["$(rootpath %s)" % test for test in tests],
         srcs = ["//python/tensorstore:bazel_pytest_main.py"] + srcs,
         main = "//python/tensorstore:bazel_pytest_main.py",
         legacy_create_init = False,
         deps = deps,
         **kwargs
     )
```

### Comparing `tensorstore-0.1.8/python/tensorstore/result_type_caster.h` & `tensorstore-0.1.9/python/tensorstore/result_type_caster.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/shell.py` & `tensorstore-0.1.9/python/tensorstore/shell.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/spec.cc` & `tensorstore-0.1.9/python/tensorstore/spec.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/spec.h` & `tensorstore-0.1.9/python/tensorstore/spec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/status.cc` & `tensorstore-0.1.9/python/tensorstore/status.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/status.h` & `tensorstore-0.1.9/python/tensorstore/status.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/subscript_method.h` & `tensorstore-0.1.9/python/tensorstore/subscript_method.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tensorstore.cc` & `tensorstore-0.1.9/python/tensorstore/tensorstore.cc`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 /// \file
 ///
 /// Defines the `tensorstore._tensorstore` module.
 
 #include "python/tensorstore/context.h"
 #include "python/tensorstore/data_type.h"
+#include "python/tensorstore/downsample.h"
 #include "python/tensorstore/future.h"
 #include "python/tensorstore/index_space.h"
 #include "python/tensorstore/spec.h"
 #include "python/tensorstore/tensorstore_class.h"
 #include "python/tensorstore/transaction.h"
 #include "python/tensorstore/write_futures.h"
 #include "pybind11/pybind11.h"
@@ -58,12 +59,13 @@
   RegisterDataTypeBindings(m);
   RegisterSpecBindings(m);
   RegisterContextBindings(m);
   RegisterTransactionBindings(m);
   RegisterTensorStoreBindings(m);
   RegisterFutureBindings(m);
   RegisterWriteFuturesBindings(m);
+  RegisterDownsampleBindings(m);
 }
 
 }  // namespace
 }  // namespace internal_python
 }  // namespace tensorstore
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tensorstore_class.cc` & `tensorstore-0.1.9/python/tensorstore/tensorstore_class.cc`

 * *Files 3% similar despite different names*

```diff
@@ -161,24 +161,33 @@
           [](const TensorStore<>& self) -> py::tuple {
             auto builder = internal::ContextSpecBuilder::Make();
             auto spec = ValueOrThrow(self.spec({}, builder));
             auto pickled_context =
                 internal_python::PickleContextSpecBuilder(std::move(builder));
             auto json_spec = ValueOrThrow(spec.ToJson());
             return py::make_tuple(py::cast(json_spec),
-                                  std::move(pickled_context));
+                                  std::move(pickled_context),
+                                  static_cast<int>(self.read_write_mode()));
           },
           [](py::tuple t) -> tensorstore::TensorStore<> {
             auto json_spec = py::cast<::nlohmann::json>(t[0]);
             auto context =
                 WrapImpl(internal_python::UnpickleContextSpecBuilder(t[1]));
+            auto read_write_mode = static_cast<ReadWriteMode>(
+                py::cast<int>(t[2]) &
+                static_cast<int>(ReadWriteMode::read_write));
+            if (read_write_mode == ReadWriteMode::dynamic) {
+              throw py::value_error(
+                  "Invalid ReadWriteMode encountered unpickling TensorStore");
+            }
             py::gil_scoped_release gil_release;
-            return ValueOrThrow(
-                tensorstore::Open(std::move(context), std::move(json_spec))
-                    .result());
+            return ValueOrThrow(tensorstore::Open(std::move(context),
+                                                  std::move(json_spec),
+                                                  {read_write_mode})
+                                    .result());
           }));
 
   cls_tensorstore.attr("__iter__") = py::none();
 
   cls_tensorstore.def_property_readonly(
       "transaction",
       [](const TensorStore<>& self) {
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tensorstore_class.h` & `tensorstore-0.1.9/python/tensorstore/tensorstore_class.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/context_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/data_type_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/data_type_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/dim_expression_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/dim_expression_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,21 @@
       output=[
           ts.OutputIndexMap(input_dimension=1),
           ts.OutputIndexMap(input_dimension=2),
       ],
   )
 
 
+def test_add_new_invalid_rank():
+  x = ts.IndexTransform(input_shape=[2, 3], input_labels=["x", "y"])
+  expr = ts.d[0:32][ts.newaxis]
+  with pytest.raises(ValueError):
+    x[expr]
+
+
 def test_diagonal():
   x = ts.IndexTransform(input_shape=[2, 3], input_labels=["x", "y"])
   expr = ts.d["x", "y"].diagonal
   assert repr(expr) == "d['x','y'].diagonal"
   assert x[expr] == ts.IndexTransform(
       input_shape=[2],
       output=[
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/future_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/future_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,23 @@
   promise, future = ts.Promise.new()
   assert future.done() == False
   promise.set_result(5)
   assert future.done()
   assert future.result() == 5
 
 
+def test_promise_result_release_gil():
+  promise, future = ts.Promise.new()
+  t = threading.Thread(target=future.result)
+  t.start()
+  time.sleep(0.1)
+  promise.set_result(5)
+  t.join()
+
+
 def test_promise_set_exception():
 
   promise, future = ts.Promise.new()
   assert future.done() == False
   promise.set_exception(RuntimeError(5))
   with pytest.raises(RuntimeError):
     future.result()
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/index_domain_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/index_domain_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,31 @@
   np.testing.assert_equal(x.inclusive_max, [+ts.inf] * 2)
   np.testing.assert_equal(x.exclusive_max, [+ts.inf + 1] * 2)
   np.testing.assert_equal(x.shape, [2 * ts.inf + 1] * 2)
   assert x.labels == ("", "")
   np.testing.assert_equal(x.implicit_lower_bounds, [1, 1])
   np.testing.assert_equal(x.implicit_upper_bounds, [1, 1])
 
+  with pytest.raises(ValueError):
+    ts.IndexDomain(rank=33)
+
 
 def test_init_inclusive_min():
   x = ts.IndexDomain(inclusive_min=[1, 2])
   assert x.rank == 2
   np.testing.assert_equal(x.inclusive_min, [1, 2])
   np.testing.assert_equal(x.inclusive_max, [+ts.inf] * 2)
   np.testing.assert_equal(x.exclusive_max, [+ts.inf + 1] * 2)
   assert x.labels == ("", "")
   np.testing.assert_equal(x.implicit_lower_bounds, [0, 0])
   np.testing.assert_equal(x.implicit_upper_bounds, [1, 1])
 
+  with pytest.raises(ValueError):
+    ts.IndexDomain(inclusive_min=[1] * 33)
+
 
 def test_init_exclusive_max():
   x = ts.IndexDomain(exclusive_max=[1, 2])
   assert x.rank == 2
   np.testing.assert_equal(x.inclusive_min, [-ts.inf] * 2)
   np.testing.assert_equal(x.exclusive_max, [1, 2])
   assert x.labels == ("", "")
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/index_interval_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/index_interval_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/index_transform_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/index_transform_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/indexing_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/indexing_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/spec_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/spec_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/tensorstore_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/tensorstore_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -134,14 +134,38 @@
         "delete_existing": True,
     }).result()
     dataset[80:82, 99:102] = [[1, 2, 3], [4, 5, 6]]
     np.testing.assert_equal([[1, 2, 3], [4, 5, 6], [0, 0, 0]],
                             dataset[80:83, 99:102].read().result())
 
 
+async def test_memory_n5_cache_open():
+  dataset = ts.open({
+      "context": {
+          "cache_pool": {
+              "total_bytes_limit": 1000000
+          }
+      },
+      "driver": "n5",
+      "kvstore": {
+          "driver": "memory",
+      },
+      "metadata": {
+          "compression": {
+              "type": "gzip"
+          },
+          "dataType": "uint32",
+          "dimensions": [1000, 20000],
+          "blockSize": [10, 10],
+      },
+      "create": True,
+      "delete_existing": True,
+  }).result()
+
+
 async def test_open_error_message():
   with pytest.raises(ValueError,
                      match=".*Error parsing object member \"driver\": .*"):
     await ts.open({"invalid": "key"})
 
   with pytest.raises(ValueError, match="Expected object, but received: 3"):
     await ts.open(3)
@@ -165,35 +189,78 @@
             "blockSize": [10, 10],
         },
         "recheck_cached_data": False,
         "recheck_cached_metadata": False,
         "create": True,
         "open": True,
     }
+    print('opening t1', flush=True)
     t1 = await ts.open(spec, context=context)
+    print('opening t2', flush=True)
     t2 = await ts.open(spec, context=context)
 
+    print('pickling', flush=True)
     pickled = pickle.dumps([t1, t2])
+    print('unpickling', flush=True)
     unpickled = pickle.loads(pickled)
     new_t1, new_t2 = unpickled
 
+    print('reading new_t1', flush=True)
     assert new_t1[0, 0].read().result() == 0
+    print('reading new_t2', flush=True)
     assert new_t2[0, 0].read().result() == 0
+    print('writing to new_t1', flush=True)
     new_t1[0, 0] = 42
 
     # Delete data
+    print('deleting data', flush=True)
     await ts.open(spec, create=True, delete_existing=True)
 
     # new_t1 still sees old data in cache
+    print('reading new_t1', flush=True)
     assert new_t1[0, 0].read().result() == 42
 
     # new_t2 shares cache with new_t1
+    print('reading new_t2', flush=True)
     assert new_t2[0, 0].read().result() == 42
 
 
+async def test_pickle_read_write_mode():
+  with tempfile.TemporaryDirectory() as dir_path:
+    spec = {
+        "driver": "n5",
+        "kvstore": {
+            "driver": "file",
+            "path": dir_path,
+        },
+        "metadata": {
+            "compression": {
+                "type": "raw",
+            },
+            "dataType": "uint32",
+            "dimensions": [100, 100],
+            "blockSize": [10, 10],
+        },
+        "recheck_cached_data": False,
+        "recheck_cached_metadata": False,
+        "create": True,
+        "open": True,
+    }
+    t1 = await ts.open(spec, write=True)
+
+    assert not t1.readable
+    assert t1.writable
+
+    pickled = pickle.dumps(t1)
+    new_t1 = pickle.loads(pickled)
+
+    assert not new_t1.readable
+    assert new_t1.writable
+
+
 async def test_write_json():
   t = await ts.open({
       "driver": "array",
       "dtype": "json",
       "array": [1, {
           "a": 2
       }, 3],
```

### Comparing `tensorstore-0.1.8/python/tensorstore/tests/transaction_test.py` & `tensorstore-0.1.9/python/tensorstore/tests/transaction_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/transaction.cc` & `tensorstore-0.1.9/python/tensorstore/transaction.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/transaction.h` & `tensorstore-0.1.9/python/tensorstore/transaction.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/write_futures.cc` & `tensorstore-0.1.9/python/tensorstore/write_futures.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/python/tensorstore/write_futures.h` & `tensorstore-0.1.9/python/tensorstore/write_futures.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/setup.py` & `tensorstore-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """setuptools script for installing the Python package.
 
 This invokes bazel via the included `bazelisk.py` wrapper script.
 """
 
+# Import setuptools before distutils because setuptools monkey patches
+# distutils:
+#
+# https://github.com/pypa/setuptools/commit/bd1102648109c85c782286787e4d5290ae280abe
+import setuptools
+
 import atexit
 import distutils.command.build
 import os
 import shutil
 import sys
 import tempfile
 
-import setuptools
 import setuptools.command.build_ext
 import setuptools.command.build_py
 import setuptools.command.install
 import setuptools.dist
 
 
 class BuildCommand(distutils.command.build.build):
```

### Comparing `tensorstore-0.1.8/tensorstore/BUILD` & `tensorstore-0.1.9/tensorstore/BUILD`

 * *Files 3% similar despite different names*

```diff
@@ -445,19 +445,17 @@
         ":data_type",
         ":index",
         ":rank",
         "//tensorstore/driver",
         "//tensorstore/index_space:index_transform",
         "//tensorstore/index_space:index_transform_spec",
         "//tensorstore/index_space:json",
-        "//tensorstore/internal:attributes",
-        "//tensorstore/internal:data_type_json_binder",
         "//tensorstore/internal:json",
+        "//tensorstore/internal:type_traits",
         "//tensorstore/util:result",
-        "//tensorstore/util:status",
         "@com_github_nlohmann_json//:nlohmann_json",
     ],
 )
 
 tensorstore_cc_library(
     name = "spec_request_options",
     hdrs = ["spec_request_options.h"],
@@ -522,14 +520,15 @@
     srcs = ["strided_layout.cc"],
     hdrs = ["strided_layout.h"],
     deps = [
         ":box",
         ":container_kind",
         ":contiguous_layout",
         ":rank",
+        "//tensorstore/internal:gdb_scripting",
         "//tensorstore/internal:multi_vector",
         "//tensorstore/internal:multi_vector_view",
         "//tensorstore/internal:type_traits",
         "//tensorstore/util:assert_macros",
         "//tensorstore/util:constant_vector",
         "//tensorstore/util:extents",
         "//tensorstore/util:span",
@@ -607,14 +606,16 @@
     ],
 )
 
 tensorstore_cc_library(
     name = "all_drivers",
     deps = [
         "//tensorstore/driver/array",
+        "//tensorstore/driver/cast",
+        "//tensorstore/driver/downsample",
         "//tensorstore/driver/json",
         "//tensorstore/driver/n5",
         "//tensorstore/driver/n5:blosc_compressor",
         "//tensorstore/driver/n5:bzip2_compressor",
         "//tensorstore/driver/n5:gzip_compressor",
         "//tensorstore/driver/n5:xz_compressor",
         "//tensorstore/driver/neuroglancer_precomputed",
@@ -623,7 +624,35 @@
         "//tensorstore/driver/zarr:bzip2_compressor",
         "//tensorstore/driver/zarr:zlib_compressor",
         "//tensorstore/kvstore/file",
         "//tensorstore/kvstore/gcs",
         "//tensorstore/kvstore/memory",
     ],
 )
+
+# Package group with visibility to internal-only targets.
+package_group(
+    name = "internal_packages",
+    packages = [
+        "//python/tensorstore/...",
+        "//tensorstore/...",
+    ],
+)
+
+tensorstore_cc_library(
+    name = "downsample_method",
+    srcs = ["downsample_method.cc"],
+    hdrs = ["downsample_method.h"],
+)
+
+cc_library(
+    name = "downsample",
+    hdrs = ["downsample.h"],
+    deps = [
+        ":downsample_method",
+        ":rank",
+        ":spec",
+        ":tensorstore",
+        "//tensorstore/driver/downsample",
+        "//tensorstore/internal:type_traits",
+    ],
+)
```

### Comparing `tensorstore-0.1.8/tensorstore/array.cc` & `tensorstore-0.1.9/tensorstore/array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/array.h` & `tensorstore-0.1.9/tensorstore/array.h`

 * *Files 0% similar despite different names*

```diff
@@ -383,14 +383,15 @@
 /// \tparam OriginKind Equal to `zero_origin` or `offset_origin`.
 /// \tparam LayoutContainerKind Equal to `container` or `view`.
 template <typename ElementTagType, DimensionIndex Rank = dynamic_rank,
           ArrayOriginKind OriginKind = zero_origin,
           ContainerKind LayoutContainerKind = container>
 class Array {
  public:
+  static_assert(IsValidRankSpec(Rank));
   static_assert(IsElementTag<ElementTagType>::value,
                 "ElementTagType must be an ElementTag type.");
   static_assert(LayoutContainerKind == container || Rank >= dynamic_rank,
                 "Rank must be dynamic_rank or >= 0.");
   using ElementTag = ElementTagType;
   using Layout = StridedLayout<Rank, OriginKind, LayoutContainerKind>;
   using MaybeConstIndex = typename Layout::MaybeConstIndex;
```

### Comparing `tensorstore-0.1.8/tensorstore/array_nc_test.cc` & `tensorstore-0.1.9/tensorstore/array_nc_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/array_test.cc` & `tensorstore-0.1.9/tensorstore/array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/array_testutil.h` & `tensorstore-0.1.9/tensorstore/array_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/array_testutil_matches_array.inc` & `tensorstore-0.1.9/tensorstore/array_testutil_matches_array.inc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/array_testutil_test.cc` & `tensorstore-0.1.9/tensorstore/array_testutil_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/box.cc` & `tensorstore-0.1.9/tensorstore/box.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/box.h` & `tensorstore-0.1.9/tensorstore/box.h`

 * *Files 5% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 ///     (equivalent to specifying `inline_size==0`), the number of dimensions
 ///     will be specified at run time.  If the number of dimensions is not
 ///     greater than `inline_size`, no heap allocation is necessary.
 template <DimensionIndex Rank = dynamic_rank>
 class Box : public internal_box::BoxStorage<Rank> {
   using Storage = internal_box::BoxStorage<Rank>;
   using Access = internal::MultiVectorAccess<Storage>;
+  static_assert(IsValidRankSpec(Rank));
 
  public:
   constexpr static DimensionIndex static_rank = NormalizeRankSpec(Rank);
   using RankType = StaticOrDynamicRank<static_rank>;
   using ConstIndexType = const Index;
   using IndexType = Index;
 
@@ -352,14 +353,44 @@
     std::fill_n(origin().begin(), rank(), interval.inclusive_min());
     std::fill_n(shape().begin(), rank(), interval.size());
   }
 
   friend std::ostream& operator<<(std::ostream& os, const Box& box) {
     return internal_box::PrintToOstream(os, box);
   }
+
+  /// Slices a supported type by a box.
+  ///
+  /// Supported types that define `ApplyIndexTransform` and the pipeline
+  /// `operator|` can be transformed using the syntax:
+  ///
+  ///     TENSORSTORE_ASSIGN_OR_RETURN(auto new_obj, obj | box);
+  ///
+  /// Supported types include `IndexTransform`, `IndexDomain`, `TensorStore`,
+  /// `Spec`, `TransformedArray`.
+  ///
+  /// To make a type `T` compatible, define in the same namespace or as a hidden
+  /// friend of `T`:
+  ///
+  ///     template <DimensionIndex Rank>
+  ///     std::enable_if_t<IsRankExplicitlyConvertible(Rank, static_rank),
+  ///                      Result<U>>
+  ///     ApplyIndexTransform(Box<Rank> rank, T t) {
+  ///       // ...
+  ///     }
+  ///
+  /// where `U` is the return type.
+  template <typename Transformable>
+  decltype(ApplyIndexTransform(
+      std::declval<BoxView<NormalizeRankSpec(Rank), false>>(),
+      std::declval<Transformable>()))
+  operator()(Transformable&& transformable) const {
+    return ApplyIndexTransform(BoxView<NormalizeRankSpec(Rank), false>(*this),
+                               std::forward<Transformable>(transformable));
+  }
 };
 
 Box(DimensionIndex rank)->Box<>;
 
 template <DimensionIndex Rank>
 Box(std::integral_constant<DimensionIndex, Rank> rank) -> Box<Rank>;
 
@@ -399,14 +430,15 @@
 ///     `dynamic_rank` to indicate that the number of dimensions will be
 ///     specified at run time.
 /// \tparam Mutable Specifies whether the view is mutable (rather than const).
 template <DimensionIndex Rank = dynamic_rank, bool Mutable = false>
 class BoxView : public internal_box::BoxViewStorage<Rank, Mutable> {
   using Storage = internal_box::BoxViewStorage<Rank, Mutable>;
   using Access = internal::MultiVectorAccess<Storage>;
+  static_assert(IsValidStaticRank(Rank));
 
  public:
   constexpr static DimensionIndex static_rank = Rank;
   using RankType = StaticOrDynamicRank<Rank>;
   using ConstIndexType = internal_box::MaybeConstIndex<!Mutable>;
   using IndexType = ConstIndexType;
   using IndexIntervalType =
@@ -563,14 +595,25 @@
     std::fill_n(origin().begin(), rank(), interval.inclusive_min());
     std::fill_n(shape().begin(), rank(), interval.size());
   }
 
   friend std::ostream& operator<<(std::ostream& os, const BoxView& view) {
     return internal_box::PrintToOstream(os, view);
   }
+
+  /// Slices a supported type by a box.
+  ///
+  /// See documentation of `Box::operator()`.
+  template <typename Transformable>
+  decltype(ApplyIndexTransform(std::declval<BoxView>(),
+                               std::declval<Transformable>()))
+  operator()(Transformable&& transformable) const {
+    return ApplyIndexTransform(*this,
+                               std::forward<Transformable>(transformable));
+  }
 };
 
 BoxView(DimensionIndex rank)->BoxView<>;
 
 template <DimensionIndex Rank>
 BoxView(std::integral_constant<DimensionIndex, Rank> rank) -> BoxView<Rank>;
```

### Comparing `tensorstore-0.1.8/tensorstore/box_test.cc` & `tensorstore-0.1.9/tensorstore/box_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/cast.h` & `tensorstore-0.1.9/tensorstore/cast.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/container_kind.h` & `tensorstore-0.1.9/tensorstore/container_kind.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/context.cc` & `tensorstore-0.1.9/tensorstore/context.cc`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,35 @@
   if (impl_->parent_) {
     impl_->root_ = impl_->parent_->root_;
   } else {
     impl_->root_ = impl_.get();
   }
 }
 
+Result<Context> Context::FromJson(::nlohmann::json json_spec, Context parent,
+                                  FromJsonOptions options) {
+  TENSORSTORE_ASSIGN_OR_RETURN(
+      auto spec, Spec::FromJson(std::move(json_spec), std::move(options)));
+  return Context(spec, std::move(parent));
+}
+
+Context::Spec Context::spec() const {
+  if (!impl_) return {};
+  Context::Spec spec;
+  internal_context::Access::impl(spec) = impl_->spec_;
+  return spec;
+}
+
+Context Context::parent() const {
+  if (!impl_) return {};
+  Context parent_context;
+  parent_context.impl_ = impl_->parent_;
+  return parent_context;
+}
+
 TENSORSTORE_DEFINE_JSON_DEFAULT_BINDER(Context::Spec, [](auto is_loading,
                                                          const auto& options,
                                                          auto* obj, auto* j) {
   if constexpr (!is_loading) {
     if (!options.include_context()) {
       *j = ::nlohmann::json(::nlohmann::json::value_t::discarded);
       return absl::OkStatus();
```

### Comparing `tensorstore-0.1.8/tensorstore/context.h` & `tensorstore-0.1.9/tensorstore/context.h`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,23 @@
     }
     element_type* operator->() const noexcept { return get(); }
     element_type& operator*() const noexcept { return *get(); }
 
     /// Returns `true` if this is a valid handle.
     explicit operator bool() const { return static_cast<bool>(impl_); }
 
+    /// Returns `true` if `a` and `b` refer to the same resource.
+    friend bool operator==(const Resource& a, const Resource& b) {
+      return a.impl_ == b.impl_;
+    }
+
+    friend bool operator!=(const Resource& a, const Resource& b) {
+      return !(a == b);
+    }
+
     friend void EncodeCacheKeyAdl(std::string* out, const Resource& resource) {
       internal::EncodeCacheKey(
           out, reinterpret_cast<std::uintptr_t>(resource.get()));
     }
 
    private:
     friend class Context;
@@ -210,31 +219,77 @@
   /// The actual resources are created lazily as needed.
   ///
   /// \param spec The context spec.
   /// \param parent The parent context to extend.  Specifying a null context is
   ///     equivalent to specifying `Default()`.
   explicit Context(const Spec& spec, Context parent = {});
 
+  /// Constructs a context from a JSON spec.
+  ///
+  /// \param json_spec The JSON spec.
+  /// \param parent The parent context to extend.  Specifying a null context is
+  ///     equivalent to specifying `Default()`.
+  /// \param options Options for parsing `json_spec`.
+  static Result<Context> FromJson(::nlohmann::json json_spec,
+                                  Context parent = {},
+                                  FromJsonOptions options = {});
+
   /// Returns a resource.
   ///
   /// \param resource_spec The resource spec.
   /// \threadsafety Thread safe.
   template <typename Provider>
   Result<Resource<Provider>> GetResource(
       const ResourceSpec<Provider>& resource_spec) const {
     Resource<Provider> resource;
     TENSORSTORE_ASSIGN_OR_RETURN(
         resource.impl_, internal_context::GetResource(
                             impl_.get(), resource_spec.impl_.get(), nullptr));
     return resource;
   }
 
+  /// Returns a resource from a JSON spec.
+  ///
+  /// \param resource_spec The JSON resource spec.
+  /// \threadsafety Thread safe.
+  template <typename Provider>
+  Result<Resource<Provider>> GetResource(
+      const ::nlohmann::json& json_spec) const {
+    TENSORSTORE_ASSIGN_OR_RETURN(auto spec,
+                                 ResourceSpec<Provider>::FromJson(json_spec));
+    return GetResource(spec);
+  }
+
+  /// Returns the default resource for a given provider.
+  ///
+  /// \threadsafety Thread safe.
+  template <typename Provider>
+  Result<Resource<Provider>> GetResource() {
+    return GetResource<Provider>(Provider::id);
+  }
+
   /// Returns `true` if this is not a null context.
   explicit operator bool() const { return static_cast<bool>(impl_); }
 
+  /// Returns `true` if the two context objects refer to the same underlying
+  /// shared state.
+  friend bool operator==(const Context& a, const Context& b) {
+    return a.impl_ == b.impl_;
+  }
+
+  friend bool operator!=(const Context& a, const Context& b) {
+    return !(a == b);
+  }
+
+  /// Returns the spec used to create this context.
+  Context::Spec spec() const;
+
+  /// Returns the parent Context, if any.
+  Context parent() const;
+
  private:
   friend class internal_context::Access;
   internal_context::ContextImplPtr impl_;
 };
 
 namespace internal {
```

### Comparing `tensorstore-0.1.8/tensorstore/context_impl.h` & `tensorstore-0.1.9/tensorstore/context_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/context_impl_base.h` & `tensorstore-0.1.9/tensorstore/context_impl_base.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/context_resource_provider.h` & `tensorstore-0.1.9/tensorstore/context_resource_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/context_test.cc` & `tensorstore-0.1.9/tensorstore/context_test.cc`

 * *Files 9% similar despite different names*

```diff
@@ -108,20 +108,37 @@
       Context::ResourceSpec<IntResource>::FromJson("foo"),
       MatchesStatus(absl::StatusCode::kInvalidArgument,
                     "Invalid reference to \"int_resource\" resource: \"foo\""));
 }
 
 TEST(IntResourceTest, Default) {
   auto context = Context::Default();
-  auto resource_spec =
-      Context::ResourceSpec<IntResource>::FromJson("int_resource");
-  ASSERT_EQ(absl::OkStatus(), GetStatus(resource_spec));
-  auto resource = context.GetResource(*resource_spec);
-  ASSERT_EQ(absl::OkStatus(), GetStatus(resource));
-  EXPECT_EQ(42, **resource);
+  EXPECT_EQ(context, context);
+  EXPECT_FALSE(context.parent());
+  auto context2 = Context::Default();
+  EXPECT_NE(context, context2);
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(
+      auto resource_spec,
+      Context::ResourceSpec<IntResource>::FromJson("int_resource"));
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto resource,
+                                   context.GetResource(resource_spec));
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto resource2,
+                                   context.GetResource(resource_spec));
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto resource3,
+                                   context2.GetResource(resource_spec));
+  EXPECT_EQ(resource, resource);
+  EXPECT_EQ(resource, resource2);
+  EXPECT_NE(resource, resource3);
+  EXPECT_THAT(context.GetResource<IntResource>(),
+              ::testing::Optional(resource));
+  EXPECT_THAT(context.GetResource<IntResource>("int_resource"),
+              ::testing::Optional(resource));
+  EXPECT_THAT(resource, ::testing::Pointee(42));
+  EXPECT_THAT(context.GetResource<IntResource>({{"value", 50}}),
+              ::testing::Optional(::testing::Pointee(50)));
 }
 
 TEST(IntResourceTest, ValidDirectSpec) {
   auto context = Context::Default();
   auto resource_spec =
       Context::ResourceSpec<IntResource>::FromJson({{"value", 7}});
   ASSERT_EQ(absl::OkStatus(), GetStatus(resource_spec));
@@ -137,14 +154,21 @@
   auto context = Context(*spec_result);
   auto resource_spec = Context::ResourceSpec<IntResource>::Default();
   auto resource = context.GetResource(resource_spec);
   ASSERT_EQ(absl::OkStatus(), GetStatus(resource));
   EXPECT_EQ(7, **resource);
 }
 
+TEST(IntResourceTest, ContextFromJson) {
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(
+      auto context, Context::FromJson({{"int_resource", {{"value", 7}}}}));
+  EXPECT_THAT(context.GetResource<IntResource>(),
+              ::testing::Optional(::testing::Pointee(7)));
+}
+
 TEST(IntResourceTest, ValidIndirectSpecDefault) {
   auto context = Context::Default();
   auto resource_spec = Context::ResourceSpec<IntResource>::Default();
   auto resource = context.GetResource(resource_spec);
   ASSERT_EQ(absl::OkStatus(), GetStatus(resource));
   EXPECT_EQ(42, **resource);
 }
@@ -220,36 +244,41 @@
 TEST(IntResourceTest, Inherit) {
   const ::nlohmann::json json_spec1{
       {"int_resource", {{"value", 7}}},
       {"int_resource#a", {{"value", 9}}},
       {"int_resource#d", {{"value", 42}}},
       {"int_resource#c", nullptr},
   };
-  auto spec1 = Context::Spec::FromJson(json_spec1).value();
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto spec1,
+                                   Context::Spec::FromJson(json_spec1));
   EXPECT_EQ(::nlohmann::json({
                 {"int_resource", {{"value", 7}}},
                 {"int_resource#a", {{"value", 9}}},
                 {"int_resource#d", ::nlohmann::json::object_t{}},
                 {"int_resource#c", nullptr},
             }),
             ::nlohmann::json(spec1.ToJson(IncludeDefaults{false}).value()));
   EXPECT_EQ(::nlohmann::json({
                 {"int_resource", {{"value", 7}}},
                 {"int_resource#a", {{"value", 9}}},
                 {"int_resource#d", {{"value", 42}}},
                 {"int_resource#c", nullptr},
             }),
             ::nlohmann::json(spec1.ToJson(IncludeDefaults{true}).value()));
-  auto spec2 = Context::Spec::FromJson({
-                                           {"int_resource", {{"value", 8}}},
-                                           {"int_resource#b", nullptr},
-                                       })
-                   .value();
+  ::nlohmann::json json_spec2{
+      {"int_resource", {{"value", 8}}},
+      {"int_resource#b", nullptr},
+  };
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto spec2,
+                                   Context::Spec::FromJson(json_spec2));
   auto context1 = Context(spec1);
   auto context2 = Context(spec2, context1);
+  EXPECT_EQ(context1, context2.parent());
+  EXPECT_THAT(context1.spec().ToJson(), ::testing::Optional(json_spec1));
+  EXPECT_THAT(context2.spec().ToJson(), ::testing::Optional(json_spec2));
   auto resource1 = context2.GetResource(
       Context::ResourceSpec<IntResource>::FromJson("int_resource").value());
   auto resource2 = context2.GetResource(
       Context::ResourceSpec<IntResource>::FromJson("int_resource#a").value());
   auto resource3 = context2.GetResource(
       Context::ResourceSpec<IntResource>::FromJson("int_resource#b").value());
   auto resource4 = context2.GetResource(
```

### Comparing `tensorstore-0.1.8/tensorstore/contiguous_layout.cc` & `tensorstore-0.1.9/tensorstore/contiguous_layout.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/contiguous_layout.h` & `tensorstore-0.1.9/tensorstore/contiguous_layout.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/contiguous_layout_test.cc` & `tensorstore-0.1.9/tensorstore/contiguous_layout_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/data_type.cc` & `tensorstore-0.1.9/tensorstore/data_type.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/data_type.h` & `tensorstore-0.1.9/tensorstore/data_type.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/data_type_conversion.h` & `tensorstore-0.1.9/tensorstore/data_type_conversion.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/data_type_conversion_test.cc` & `tensorstore-0.1.9/tensorstore/data_type_conversion_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/data_type_test.cc` & `tensorstore-0.1.9/tensorstore/data_type_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/BUILD` & `tensorstore-0.1.9/tensorstore/driver/BUILD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+    data = [
+        "//tensorstore/driver/array:doc_sources",
+        "//tensorstore/driver/cast:doc_sources",
+        "//tensorstore/driver/downsample:doc_sources",
+        "//tensorstore/driver/json:doc_sources",
+        "//tensorstore/driver/n5:doc_sources",
+        "//tensorstore/driver/neuroglancer_precomputed:doc_sources",
+        "//tensorstore/driver/zarr:doc_sources",
+    ],
+)
+
 tensorstore_cc_library(
     name = "chunk",
     hdrs = ["chunk.h"],
     deps = [
         "//tensorstore:data_type",
         "//tensorstore/index_space:index_transform",
         "//tensorstore/internal:arena",
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/array/BUILD` & `tensorstore-0.1.9/tensorstore/examples/BUILD`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,95 @@
-load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
+load("//tensorstore:tensorstore.bzl", "tensorstore_cc_binary", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
-tensorstore_cc_library(
-    name = "array",
-    srcs = ["array.cc"],
-    hdrs = ["array.h"],
+tensorstore_cc_test(
+    name = "compute_percentiles",
+    size = "small",
+    srcs = ["compute_percentiles.cc"],
+    tags = ["manual"],
     deps = [
         "//tensorstore",
         "//tensorstore:array",
         "//tensorstore:context",
+        "//tensorstore:contiguous_layout",
         "//tensorstore:data_type",
-        "//tensorstore/driver",
+        "//tensorstore:index",
+        "//tensorstore:open",
+        "//tensorstore:open_mode",
+        "//tensorstore:progress",
+        "//tensorstore:rank",
+        "//tensorstore:spec",
+        "//tensorstore:spec_request_options",
+        "//tensorstore/driver/n5",
         "//tensorstore/index_space:dim_expression",
         "//tensorstore/index_space:index_transform",
-        "//tensorstore/index_space:index_transform_builder",
         "//tensorstore/index_space:transformed_array",
-        "//tensorstore/internal:data_copy_concurrency_resource",
-        "//tensorstore/internal:json",
-        "//tensorstore/internal:json_array",
-        "//tensorstore/internal:nditerable_transformed_array",
-        "//tensorstore/internal:type_traits",
-        "@com_google_absl//absl/synchronization",
+        "//tensorstore/internal:init_tensorstore",
+        "//tensorstore/kvstore/gcs",
+        "//tensorstore/kvstore/memory",
+        "//tensorstore/util:future",
+        "//tensorstore/util:iterate_over_index_range",
+        "//tensorstore/util:result",
+        "//tensorstore/util:span",
+        "//tensorstore/util:status",
+        "//tensorstore/util:str_cat",
+        "//tensorstore/util:utf8_string",
+        "@com_github_nlohmann_json//:nlohmann_json",
+        "@com_google_absl//absl/flags:flag",
+        "@com_google_absl//absl/flags:marshalling",
+        "@com_google_absl//absl/status",
+        "@com_google_absl//absl/strings",
+        "@net_sourceforge_half//:half",
     ],
-    alwayslink = 1,
 )
 
-tensorstore_cc_test(
-    name = "array_test",
-    size = "small",
-    srcs = ["array_test.cc"],
+tensorstore_cc_binary(
+    name = "create_array",
+    srcs = ["create_array.cc"],
     deps = [
-        ":array",
-        "//tensorstore",
-        "//tensorstore:context",
-        "//tensorstore:open",
-        "//tensorstore:open_mode",
-        "//tensorstore:spec",
+        "//tensorstore:array",
+        "//tensorstore:index",
         "//tensorstore/index_space:dim_expression",
-        "//tensorstore/internal:elementwise_function",
-        "//tensorstore/internal:json_gtest",
-        "//tensorstore/util:executor",
+        "//tensorstore/index_space:index_transform",
+        "//tensorstore/index_space:transformed_array",
+        "//tensorstore/util:iterate_over_index_range",
+        "//tensorstore/util:status",
+    ],
+)
+
+tensorstore_cc_binary(
+    name = "image_convolution",
+    srcs = ["image_convolution.cc"],
+    deps = [
+        "//tensorstore:array",
+        "//tensorstore:index",
+        "//tensorstore/index_space:dim_expression",
+        "//tensorstore/index_space:transformed_array",
+        "//tensorstore/util:iterate_over_index_range",
+        "//tensorstore/util:status",
+    ],
+)
+
+tensorstore_cc_binary(
+    name = "map_apply",
+    srcs = ["map_apply.cc"],
+    deps = [
+        "//tensorstore:array",
+        "//tensorstore:index",
+        "//tensorstore/index_space:dim_expression",
+        "//tensorstore/index_space:transformed_array",
+        "//tensorstore/util:iterate_over_index_range",
+        "//tensorstore/util:status",
+    ],
+)
+
+tensorstore_cc_binary(
+    name = "status_result",
+    srcs = ["status_result.cc"],
+    deps = [
+        "//tensorstore/util:result",
         "//tensorstore/util:status",
-        "//tensorstore/util:status_testutil",
-        "@com_google_absl//absl/meta:type_traits",
-        "@com_google_googletest//:gtest_main",
     ],
 )
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/array/array.cc` & `tensorstore-0.1.9/tensorstore/driver/array/array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/array/array.h` & `tensorstore-0.1.9/tensorstore/driver/array/array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/array/array_test.cc` & `tensorstore-0.1.9/tensorstore/driver/array/array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/array/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/array/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/BUILD` & `tensorstore-0.1.9/tensorstore/driver/array/BUILD`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,59 @@
-# TensorStore driver adapter that performs data type conversion
-
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
-    name = "cast",
-    srcs = ["cast.cc"],
-    hdrs = ["cast.h"],
+    name = "array",
+    srcs = ["array.cc"],
+    hdrs = ["array.h"],
     deps = [
+        "//tensorstore",
+        "//tensorstore:array",
+        "//tensorstore:context",
         "//tensorstore:data_type",
-        "//tensorstore:open_mode",
-        "//tensorstore:spec",
         "//tensorstore/driver",
+        "//tensorstore/index_space:dim_expression",
+        "//tensorstore/index_space:index_transform",
+        "//tensorstore/index_space:index_transform_builder",
+        "//tensorstore/index_space:transformed_array",
+        "//tensorstore/internal:data_copy_concurrency_resource",
         "//tensorstore/internal:json",
-        "//tensorstore/internal:nditerable_data_type_conversion",
+        "//tensorstore/internal:json_array",
+        "//tensorstore/internal:nditerable_transformed_array",
         "//tensorstore/internal:type_traits",
-        "//tensorstore/util:result",
-        "//tensorstore/util:str_cat",
-        "@com_google_absl//absl/status",
+        "@com_google_absl//absl/synchronization",
     ],
     alwayslink = 1,
 )
 
 tensorstore_cc_test(
-    name = "cast_test",
+    name = "array_test",
     size = "small",
-    srcs = ["cast_test.cc"],
+    srcs = ["array_test.cc"],
     deps = [
-        ":cast",
-        "//tensorstore:cast",
+        ":array",
+        "//tensorstore",
         "//tensorstore:context",
         "//tensorstore:open",
+        "//tensorstore:open_mode",
         "//tensorstore:spec",
-        "//tensorstore/driver/array",
-        "//tensorstore/index_space:index_transform_builder",
-        "//tensorstore/index_space:json",
-        "//tensorstore/util:result",
+        "//tensorstore/index_space:dim_expression",
+        "//tensorstore/internal:elementwise_function",
+        "//tensorstore/internal:json_gtest",
+        "//tensorstore/util:executor",
         "//tensorstore/util:status",
         "//tensorstore/util:status_testutil",
+        "@com_google_absl//absl/meta:type_traits",
         "@com_google_googletest//:gtest_main",
     ],
 )
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/cast.cc` & `tensorstore-0.1.9/tensorstore/driver/cast/cast.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/cast.h` & `tensorstore-0.1.9/tensorstore/driver/cast/cast.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/cast_test.cc` & `tensorstore-0.1.9/tensorstore/driver/cast/cast_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/index.rst` & `tensorstore-0.1.9/tensorstore/driver/cast/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/cast/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/cast/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/chunk.h` & `tensorstore-0.1.9/tensorstore/driver/chunk.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/driver.cc` & `tensorstore-0.1.9/tensorstore/driver/driver.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/driver.h` & `tensorstore-0.1.9/tensorstore/driver/driver.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/driver_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/driver_testutil.cc` & `tensorstore-0.1.9/tensorstore/driver/driver_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/driver_testutil.h` & `tensorstore-0.1.9/tensorstore/driver/driver_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/BUILD` & `tensorstore-0.1.9/tensorstore/driver/json/BUILD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
     name = "json",
     srcs = ["driver.cc"],
     deps = [
         ":json_change_map",
         "//tensorstore/driver",
         "//tensorstore/internal:async_cache",
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/driver.cc` & `tensorstore-0.1.9/tensorstore/driver/json/driver.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/json/driver_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/index.rst` & `tensorstore-0.1.9/tensorstore/driver/json/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/json_change_map.cc` & `tensorstore-0.1.9/tensorstore/driver/json/json_change_map.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/json_change_map.h` & `tensorstore-0.1.9/tensorstore/driver/json/json_change_map.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/json_change_map_test.cc` & `tensorstore-0.1.9/tensorstore/driver/json/json_change_map_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/json/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/json/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver.cc` & `tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver.cc`

 * *Files 0% similar despite different names*

```diff
@@ -441,19 +441,14 @@
         ExplicitIndexOr(new_exclusive_max[i], cur_dim_bounds.exclusive_max()));
     const Index chunk_size = chunk_shape[i];
     current_grid_bounds[i] = DividePositiveRoundOut(cur_dim_bounds, chunk_size);
     new_grid_bounds[i] = DividePositiveRoundOut(new_dim_bounds, chunk_size);
   }
   internal::BoxDifference box_difference(current_grid_bounds, new_grid_bounds);
   Box<dynamic_rank(internal::kNumInlinedDims)> part(rank);
-  if (!box_difference.valid()) {
-    return absl::InvalidArgumentError(StrCat("Resize would require more than ",
-                                             std::numeric_limits<Index>::max(),
-                                             " chunk regions to be deleted"));
-  }
   for (Index box_i = 0; box_i < box_difference.num_sub_boxes(); ++box_i) {
     box_difference.GetSubBox(box_i, part);
     IterateOverIndexRange(part, [&](span<const Index> cell_indices) {
       auto entry = cache->GetEntryForCell(cell_indices);
       LinkError(pair.promise, entry->Delete(transaction));
     });
   }
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver.h` & `tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_impl.h` & `tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_schema.yml` & `tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/kvs_backed_chunk_driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/kvs_backed_chunk_driver_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/BUILD` & `tensorstore-0.1.9/tensorstore/driver/n5/BUILD`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
     name = "blosc_compressor",
     srcs = ["blosc_compressor.cc"],
     deps = [
         ":compressor",
         "//tensorstore/internal:json",
         "//tensorstore/internal/compression:blosc_compressor",
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/blosc_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/blosc_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/blosc_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/blosc_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/bzip2_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/bzip2_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/bzip2_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/bzip2_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/compressor.h` & `tensorstore-0.1.9/tensorstore/driver/n5/compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/compressor_registry.h` & `tensorstore-0.1.9/tensorstore/driver/n5/compressor_registry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/driver.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/driver.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/driver_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/golden_file_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/golden_file_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/gzip_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/gzip_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/gzip_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/gzip_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/index.rst` & `tensorstore-0.1.9/tensorstore/driver/n5/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/metadata.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/metadata.cc`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
   return internal::JsonParseArray(
       value,
       [&](std::ptrdiff_t size) {
         if (*rank) {
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonValidateArrayLength(size, **rank));
         } else {
+          TENSORSTORE_RETURN_IF_ERROR(ValidateRank(size));
           *rank = size;
         }
         vec->resize(size);
         return absl::OkStatus();
       },
       [&](const ::nlohmann::json& v, std::ptrdiff_t i) {
         return internal::JsonRequireInteger<Index>(
@@ -81,14 +82,15 @@
   TENSORSTORE_RETURN_IF_ERROR(internal::JsonParseArray(
       value,
       [&](std::ptrdiff_t size) {
         if (*rank) {
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonValidateArrayLength(size, **rank));
         } else {
+          TENSORSTORE_RETURN_IF_ERROR(ValidateRank(size));
           *rank = size;
         }
         axes->resize(size);
         return absl::OkStatus();
       },
       [&](const ::nlohmann::json& v, std::ptrdiff_t i) {
         return internal::JsonRequireValueAs(v, &(*axes)[i], /*strict=*/true);
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/metadata.h` & `tensorstore-0.1.9/tensorstore/driver/n5/metadata.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/metadata_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/metadata_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,21 @@
                                  {"blockSize", {1, 2, 3}},
                                  {"dataType", "uint16"},
                                  {"compression", 3}}),
               MatchesStatus(absl::StatusCode::kInvalidArgument));
 }
 
 TEST(MetadataTest, ParseInvalidDimensions) {
+  // Exceeds rank.
+  EXPECT_THAT(
+      N5Metadata::Parse({{"dimensions", ::nlohmann::json::array_t(33, 10)},
+                         {"blockSize", ::nlohmann::json::array_t(33, 1)},
+                         {"dataType", "uint16"},
+                         {"compression", {{"type", "raw"}}}}),
+      MatchesStatus(absl::StatusCode::kInvalidArgument));
   EXPECT_THAT(N5Metadata::Parse({{"dimensions", "x"},
                                  {"blockSize", {1, 2, 3}},
                                  {"dataType", "uint16"},
                                  {"compression", {{"type", "raw"}}}}),
               MatchesStatus(absl::StatusCode::kInvalidArgument));
   EXPECT_THAT(N5Metadata::Parse({{"dimensions", {"x"}},
                                  {"blockSize", {1, 2, 3}},
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/n5/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/testdata/generate.py` & `tensorstore-0.1.9/tensorstore/driver/n5/testdata/generate.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/xz_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/xz_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/n5/xz_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/n5/xz_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/BUILD` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
     name = "chunk_encoding",
     srcs = ["chunk_encoding.cc"],
     hdrs = ["chunk_encoding.h"],
     deps = [
         ":metadata",
         "//tensorstore:array",
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/chunk_encoding_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/chunk_encoding_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/driver.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/driver.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/driver_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/index.rst` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/metadata_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/metadata_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/murmurhash3_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/murmurhash3_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_decoder_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_encoder_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.h` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_key_value_store_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_test.cc` & `tensorstore-0.1.9/tensorstore/driver/neuroglancer_precomputed/uint64_sharded_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/registry.h` & `tensorstore-0.1.9/tensorstore/driver/registry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/BUILD` & `tensorstore-0.1.9/tensorstore/driver/zarr/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
     name = "blosc_compressor",
     srcs = ["blosc_compressor.cc"],
     deps = [
         ":compressor",
         "//tensorstore/internal:json",
         "//tensorstore/internal/compression:blosc_compressor",
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/blosc_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/blosc_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/blosc_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/blosc_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/bzip2_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/bzip2_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/bzip2_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/bzip2_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/compressor.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/compressor_registry.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/compressor_registry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/driver.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/driver.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/driver_impl.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/driver_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/driver_impl_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/driver_impl_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/driver_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/driver_test.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1312,40 +1312,14 @@
           .result(),
       MatchesStatus(absl::StatusCode::kFailedPrecondition,
                     "Resize operation would also affect output dimension 3 "
                     "over the interval \\[2, 3\\) but `resize_tied_bounds` was "
                     "not specified"));
 }
 
-TEST(ZarrDriverTest, InvalidResizeTooManyChunksToDelete) {
-  auto context = Context::Default();
-  // Create the store.
-  ::nlohmann::json storage_spec{{"driver", "memory"}};
-  ::nlohmann::json zarr_metadata_json = GetBasicResizeMetadata();
-  zarr_metadata_json["shape"] = ::nlohmann::json::array_t(100, 10);
-  zarr_metadata_json["chunks"] = ::nlohmann::json::array_t(100, 1);
-  ::nlohmann::json json_spec{
-      {"driver", "zarr"},
-      {"kvstore", storage_spec},
-      {"path", "prefix"},
-      {"metadata", zarr_metadata_json},
-  };
-  auto store = tensorstore::Open(context, json_spec,
-                                 {tensorstore::OpenMode::create,
-                                  tensorstore::ReadWriteMode::read_write})
-                   .value();
-  EXPECT_THAT(Resize(store, std::vector<Index>(100, kImplicit),
-                     std::vector<Index>(100, 5))
-                  .result(),
-              MatchesStatus(absl::StatusCode::kInvalidArgument,
-                            StrCat("Resize would require more than ",
-                                   std::numeric_limits<Index>::max(),
-                                   " chunk regions to be deleted")));
-}
-
 TEST(ZarrDriverTest, InvalidResizeIncompatibleMetadata) {
   auto context = Context::Default();
   // Create the store.
   ::nlohmann::json storage_spec{{"driver", "memory"}};
   ::nlohmann::json zarr_metadata_json = GetBasicResizeMetadata();
   ::nlohmann::json json_spec{
       {"driver", "zarr"},
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/dtype.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/dtype.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/dtype.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/dtype.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/dtype_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/dtype_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/index.rst` & `tensorstore-0.1.9/tensorstore/driver/zarr/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/metadata.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/metadata.cc`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,15 @@
   return internal::JsonParseArray(
       value,
       [&](std::ptrdiff_t size) {
         if (*rank) {
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonValidateArrayLength(size, **rank));
         } else {
+          TENSORSTORE_RETURN_IF_ERROR(ValidateRank(size));
           *rank = size;
         }
         vec->resize(size);
         return absl::OkStatus();
       },
       [&](const ::nlohmann::json& v, std::ptrdiff_t i) {
         return internal::JsonRequireInteger<Index>(
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/metadata.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/metadata.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/metadata_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/metadata_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -673,8 +673,24 @@
                                      {"order", "F"},
                                      {"shape", {10}},
                                      {"zarr_format", 2}},
                     &metadata),
       MatchesStatus(absl::StatusCode::kInvalidArgument, ".*\"chunks\".*"));
 }
 
+TEST(ParseMetadataTest, InvalidRank) {
+  ZarrMetadata metadata;
+  EXPECT_THAT(ParseMetadata(
+                  ::nlohmann::json{{"chunks", ::nlohmann::json::array_t(33, 1)},
+                                   {"compressor", nullptr},
+                                   {"dtype", "|i1"},
+                                   {"fill_value", 0},
+                                   {"filters", nullptr},
+                                   {"order", "F"},
+                                   {"shape", ::nlohmann::json::array_t(33, 10)},
+                                   {"zarr_format", 2}},
+                  &metadata),
+              MatchesStatus(absl::StatusCode::kInvalidArgument,
+                            ".*: Rank 33 is outside valid range \\[0, 32\\]"));
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/metadata_testutil.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/metadata_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/metadata_testutil.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/metadata_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/schema.yml` & `tensorstore-0.1.9/tensorstore/driver/zarr/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/spec.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/spec.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/spec.h` & `tensorstore-0.1.9/tensorstore/driver/zarr/spec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/spec_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/spec_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/zlib_compressor.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/zlib_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/driver/zarr/zlib_compressor_test.cc` & `tensorstore-0.1.9/tensorstore/driver/zarr/zlib_compressor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/BUILD` & `tensorstore-0.1.9/tensorstore/kvstore/file/BUILD`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,91 @@
-load("//tensorstore:tensorstore.bzl", "tensorstore_cc_binary", "tensorstore_cc_test")
+# Filesystem-backed KeyValueStore driver
+
+load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
-tensorstore_cc_test(
-    name = "compute_percentiles",
-    size = "small",
-    srcs = ["compute_percentiles.cc"],
-    tags = ["manual"],
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
+tensorstore_cc_library(
+    name = "file",
+    srcs = ["file_key_value_store.cc"],
     deps = [
-        "//tensorstore",
-        "//tensorstore:array",
+        ":file_util",
         "//tensorstore:context",
-        "//tensorstore:contiguous_layout",
-        "//tensorstore:data_type",
-        "//tensorstore:index",
-        "//tensorstore:open",
-        "//tensorstore:open_mode",
-        "//tensorstore:progress",
-        "//tensorstore:rank",
-        "//tensorstore:spec",
-        "//tensorstore:spec_request_options",
-        "//tensorstore/driver/n5",
-        "//tensorstore/index_space:dim_expression",
-        "//tensorstore/index_space:index_transform",
-        "//tensorstore/index_space:transformed_array",
-        "//tensorstore/internal:init_tensorstore",
-        "//tensorstore/kvstore/gcs",
-        "//tensorstore/kvstore/memory",
+        "//tensorstore/internal:file_io_concurrency_resource",
+        "//tensorstore/internal:flat_cord_builder",
+        "//tensorstore/internal:json",
+        "//tensorstore/internal:os_error_code",
+        "//tensorstore/internal:path",
+        "//tensorstore/kvstore:byte_range",
+        "//tensorstore/kvstore:generation",
+        "//tensorstore/kvstore:key_value_store",
+        "//tensorstore/util:execution",
+        "//tensorstore/util:executor",
+        "//tensorstore/util:function_view",
         "//tensorstore/util:future",
-        "//tensorstore/util:iterate_over_index_range",
+        "//tensorstore/util:quote_string",
         "//tensorstore/util:result",
-        "//tensorstore/util:span",
         "//tensorstore/util:status",
         "//tensorstore/util:str_cat",
-        "//tensorstore/util:utf8_string",
         "@com_github_nlohmann_json//:nlohmann_json",
-        "@com_google_absl//absl/flags:flag",
-        "@com_google_absl//absl/flags:marshalling",
+        "@com_google_absl//absl/base:core_headers",
         "@com_google_absl//absl/status",
         "@com_google_absl//absl/strings",
-        "@net_sourceforge_half//:half",
+        "@com_google_absl//absl/time",
+        "@com_google_absl//absl/utility",
     ],
+    alwayslink = 1,
 )
 
-tensorstore_cc_binary(
-    name = "create_array",
-    srcs = ["create_array.cc"],
+tensorstore_cc_test(
+    name = "file_key_value_store_test",
+    size = "small",
+    srcs = ["file_key_value_store_test.cc"],
     deps = [
-        "//tensorstore:array",
-        "//tensorstore:index",
-        "//tensorstore/index_space:dim_expression",
-        "//tensorstore/index_space:index_transform",
-        "//tensorstore/index_space:transformed_array",
-        "//tensorstore/util:iterate_over_index_range",
+        ":file",
+        "//tensorstore:context",
+        "//tensorstore/internal:file_io_concurrency_resource",
+        "//tensorstore/internal:test_util",
+        "//tensorstore/kvstore:generation",
+        "//tensorstore/kvstore:generation_testutil",
+        "//tensorstore/kvstore:key_value_store",
+        "//tensorstore/kvstore:key_value_store_testutil",
+        "//tensorstore/util:execution",
+        "//tensorstore/util:executor",
+        "//tensorstore/util:sender_testutil",
         "//tensorstore/util:status",
+        "//tensorstore/util:status_testutil",
+        "//tensorstore/util:str_cat",
+        "@com_github_nlohmann_json//:nlohmann_json",
+        "@com_google_absl//absl/status",
+        "@com_google_googletest//:gtest_main",
     ],
 )
 
-tensorstore_cc_binary(
-    name = "image_convolution",
-    srcs = ["image_convolution.cc"],
-    deps = [
-        "//tensorstore:array",
-        "//tensorstore:index",
-        "//tensorstore/index_space:dim_expression",
-        "//tensorstore/index_space:transformed_array",
-        "//tensorstore/util:iterate_over_index_range",
-        "//tensorstore/util:status",
+tensorstore_cc_library(
+    name = "file_util",
+    srcs = [
+        "posix_file_util.cc",
+        "windows_file_util.cc",
     ],
-)
-
-tensorstore_cc_binary(
-    name = "map_apply",
-    srcs = ["map_apply.cc"],
-    deps = [
-        "//tensorstore:array",
-        "//tensorstore:index",
-        "//tensorstore/index_space:dim_expression",
-        "//tensorstore/index_space:transformed_array",
-        "//tensorstore/util:iterate_over_index_range",
-        "//tensorstore/util:status",
+    hdrs = [
+        "posix_file_util.h",
+        "unique_handle.h",
+        "windows_file_util.h",
     ],
-)
-
-tensorstore_cc_binary(
-    name = "status_result",
-    srcs = ["status_result.cc"],
     deps = [
+        "//tensorstore/internal:os_error_code",
         "//tensorstore/util:result",
-        "//tensorstore/util:status",
+        "@com_google_absl//absl/status",
+        "@com_google_absl//absl/strings",
     ],
 )
```

### Comparing `tensorstore-0.1.8/tensorstore/examples/compute_percentiles.cc` & `tensorstore-0.1.9/tensorstore/examples/compute_percentiles.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/create_array.cc` & `tensorstore-0.1.9/tensorstore/examples/create_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/image_convolution.cc` & `tensorstore-0.1.9/tensorstore/examples/image_convolution.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/map_apply.cc` & `tensorstore-0.1.9/tensorstore/examples/map_apply.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/BUILD` & `tensorstore-0.1.9/tensorstore/examples/python/beam/BUILD`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 tensorstore_pytest_test(
     name = "pipeline_test",
     size = "medium",
     srcs = ["pipeline_test.py"],
     tags = ["manual"],
     deps = [
         ":pipelines_lib",
+        "//net/proto2/python/public:use_pure_python",  # Automatically added go/proto_python_default
         "//python/tensorstore",
         "@pypa_apache_beam//:apache_beam",
         "@pypa_numpy//:numpy",
     ],
 )
 
 py_library(
```

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/compute_dfbyf.py` & `tensorstore-0.1.9/tensorstore/examples/python/beam/compute_dfbyf.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/compute_percentiles.py` & `tensorstore-0.1.9/tensorstore/examples/python/beam/compute_percentiles.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/example.gin` & `tensorstore-0.1.9/tensorstore/examples/python/beam/example.gin`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/pipeline_test.py` & `tensorstore-0.1.9/tensorstore/examples/python/beam/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/reshard_tensor.py` & `tensorstore-0.1.9/tensorstore/examples/python/beam/reshard_tensor.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/python/beam/run_pipeline.py` & `tensorstore-0.1.9/tensorstore/examples/python/beam/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/examples/status_result.cc` & `tensorstore-0.1.9/tensorstore/examples/status_result.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/generate_interval_slice_overloads.py` & `tensorstore-0.1.9/tensorstore/generate_interval_slice_overloads.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/generate_make_array_overloads.py` & `tensorstore-0.1.9/tensorstore/generate_make_array_overloads.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/generate_matches_array_overloads.py` & `tensorstore-0.1.9/tensorstore/generate_matches_array_overloads.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index.h` & `tensorstore-0.1.9/tensorstore/index.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_interval.cc` & `tensorstore-0.1.9/tensorstore/index_interval.cc`

 * *Files 1% similar despite different names*

```diff
@@ -215,16 +215,16 @@
       internal::SubOverflow(origin, interval.inclusive_min(), &offset);
   ABSL_ASSERT(!overflow);
   return ShiftInterval(interval, offset);
 }
 
 Status CheckContains(IndexInterval interval, Index index) {
   if (Contains(interval, index)) return absl::OkStatus();
-  return Status(absl::StatusCode::kOutOfRange,
-                StrCat("Index ", index, " is outside valid range ", interval));
+  return absl::OutOfRangeError(
+      StrCat("Index ", index, " is outside valid range ", interval));
 }
 
 Result<std::pair<OptionallyImplicitIndexInterval, Index>> ExtractStridedSlice(
     OptionallyImplicitIndexInterval orig, IntervalForm interval_form,
     Index start, Index stop_or_size, Index stride) {
   // We define `constraint` here because `orig` is modified later.
   const IndexInterval constraint = IndexInterval::UncheckedClosed(
```

### Comparing `tensorstore-0.1.8/tensorstore/index_interval.h` & `tensorstore-0.1.9/tensorstore/index_interval.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_interval_test.cc` & `tensorstore-0.1.9/tensorstore/index_interval_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/BUILD` & `tensorstore-0.1.9/tensorstore/index_space/BUILD`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_binary", "tensorstore_cc_library", "tensorstore_cc_test")
 load("//tensorstore:non_compile.bzl", "cc_with_non_compile_test")
 
-package(default_visibility = ["//visibility:private"])
+package(default_visibility = ["//tensorstore:internal_packages"])
 
 licenses(["notice"])
 
 tensorstore_cc_library(
     name = "add_new_dims_op",
     srcs = ["internal/add_new_dims_op.cc"],
     hdrs = ["internal/add_new_dims_op.h"],
@@ -511,14 +511,15 @@
     name = "interval_slice_op_test",
     size = "small",
     srcs = ["interval_slice_op_test.cc"],
     deps = [
         ":dim_expression",
         ":dim_expression_testutil",
         ":index_transform_builder",
+        "//tensorstore:box",
         "//tensorstore/util:status",
         "@com_google_googletest//:gtest_main",
     ],
 )
 
 tensorstore_cc_test(
     name = "inverse_transform_test",
@@ -755,14 +756,27 @@
         ":index_transform_builder",
         "//tensorstore/util:status",
         "@com_google_googletest//:gtest_main",
     ],
 )
 
 tensorstore_cc_test(
+    name = "slice_by_box_test",
+    size = "small",
+    srcs = ["slice_by_box_test.cc"],
+    deps = [
+        ":index_transform",
+        ":index_transform_builder",
+        "//tensorstore/util:status",
+        "//tensorstore/util:status_testutil",
+        "@com_google_googletest//:gtest_main",
+    ],
+)
+
+tensorstore_cc_test(
     name = "slice_by_index_domain_test",
     size = "small",
     srcs = ["slice_by_index_domain_test.cc"],
     deps = [
         ":index_transform",
         ":index_transform_builder",
         "//tensorstore/util:status",
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/add_new_dims_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/add_new_dims_op_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 using tensorstore::Index;
 using tensorstore::IndexInterval;
 using tensorstore::IndexTransformBuilder;
 using tensorstore::kInfIndex;
 using tensorstore::kInfSize;
 using tensorstore::MakeArray;
 using tensorstore::internal_index_space::TestDimExpression;
+using tensorstore::internal_index_space::TestDimExpressionError;
 
 TEST(AddNewTest, Example) {
   const auto expected_new_transform =
       IndexTransformBuilder<3, 1>()
           .input_origin({-kInfIndex, 1, -kInfIndex})
           .input_shape({kInfSize, 5, kInfSize})
           .implicit_lower_bounds({1, 0, 1})
@@ -198,8 +199,15 @@
       {
           {{2}, {2}},
           {{3}, {3}},
       },
       /*can_operate_in_place=*/true);
 }
 
+TEST(AddNewTest, InvalidRank) {
+  TestDimExpressionError(tensorstore::IdentityTransform(31),
+                         Dims(0, 1).AddNew(),
+                         absl::StatusCode::kInvalidArgument,
+                         ".*Rank 33 is outside valid range \\[0, 32\\]");
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/alignment.cc` & `tensorstore-0.1.9/tensorstore/index_space/alignment.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/alignment.h` & `tensorstore-0.1.9/tensorstore/index_space/alignment.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/alignment_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/alignment_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/compose_transforms_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/compose_transforms_test.cc`

 * *Files 7% similar despite different names*

```diff
@@ -327,8 +327,24 @@
                       .input_exclusive_max({2})
                       .output_identity_transform()
                       .Finalize()
                       .value();
   EXPECT_THAT(ComposeTransforms(t0, t1), ::testing::Optional(t1));
 }
 
+TEST(ComposeTransformsTest, TransformIndexArraySkipRepeatedElements) {
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(
+      auto t0, IndexTransformBuilder(2, 2)
+                   .input_shape({5, 2})
+                   .output_index_array(
+                       0, 0, 1, MakeArray<Index>({{0}, {1}, {2}, {3}, {4}}))
+                   .output_single_input_dimension(1, 1)
+                   .Finalize());
+  EXPECT_THAT(t0.output_index_maps()[0].index_array().byte_strides(),
+              ::testing::ElementsAre(8, 0));
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(auto t1, ComposeTransforms(t0, t0));
+  EXPECT_EQ(t0, t1);
+  EXPECT_THAT(t1.output_index_maps()[0].index_array().byte_strides(),
+              ::testing::ElementsAre(8, 0));
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/deep_copy_transform_rep_ptr_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/deep_copy_transform_rep_ptr_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/diagonal_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/diagonal_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dim_expression.h` & `tensorstore-0.1.9/tensorstore/index_space/dim_expression.h`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,21 @@
       IndexVectorOpExpr<internal_index_space::SingleIndexSliceOp, IndexVector>;
 
   /// Defines the return type for the *Interval member functions.
   template <typename... IndexVector>
   using IntervalSliceOpExpr =
       IndexVectorOpExpr<internal_index_space::IntervalSliceOp, IndexVector...>;
 
+  template <typename BoxType>
+  using BoxSliceOpExpr = NewExpr<std::enable_if_t<
+      (IsBoxLike<BoxType>::value &&
+       IsRankExplicitlyConvertible(static_selection_rank::value,
+                                   BoxType::static_rank)),
+      internal_index_space::BoxSliceOp<BoxType::static_rank>>>;
+
   /// Defines the return type for IndexArraySlice with a parameter pack of index
   /// arrays.
   template <typename... IndexArray>
   using IndexArraySliceOpExpr = absl::enable_if_t<
       sizeof...(IndexArray) >= 1 &&
           IsRankExplicitlyConvertible(sizeof...(IndexArray),
                                       static_selection_rank::value) &&
@@ -412,14 +419,67 @@
   /// Overload that permits the indices vector to be specified as a braced list.
   template <DimensionIndex Rank>
   SingleIndexSliceOpExpr<const Index (&)[Rank]> IndexSlice(
       const Index (&indices)[Rank]) const {
     return {{span(indices)}, *this};
   }
 
+  /// Extracts a box from the selected dimensions.
+  ///
+  /// This is equivalent to `SizedInterval(box.origin(), box.shape())`.
+  ///
+  /// For example: `Dims(0, 2).BoxSlice(BoxView({1, 4}, {3, 4}))` has the
+  /// following effects:
+  ///
+  /// *                   | Prior                  | New
+  /// ------------------- | ---                    | ---
+  /// Dimension selection | {0, 2}                 | {0, 2}
+  /// Input domain        | [0, 6], [2, 5], [0, 9] | [1, 3], [2, 5], [4, 7]
+  /// Labels              | {"x", "y", "z"}        | {"x", "y", "z"}
+  /// Equiv. input indices| {1, 3, 4}              | {1, 3, 4}
+  /// Equiv. input indices| {x, y, z}              | {x, y, z}
+  ///
+  /// where `x` is any index in `[1, 3]`, `y` is any index in `[2, 5]`, and `z`
+  /// is any index in `[4, 7]`.
+  ///
+  /// \requires `BoxType` satisfies `IsBoxLike` and has a rank compatible with
+  ///     the static rank of the dimension selection.
+  /// \param box The box to extract.
+  template <typename BoxType>
+  BoxSliceOpExpr<BoxType> BoxSlice(const BoxType& box) const {
+    return {{box, false}, *this};
+  }
+
+  /// Extracts a box from the selected dimensions, and translates its origin to
+  /// 0.
+  ///
+  /// This is equivalent to `TranslateSizedInterval(box.origin(), box.shape())`.
+  ///
+  /// For example: `Dims(0, 2).TranslateBoxSlice(BoxView({1, 4}, {3, 4}))` has
+  /// the following effects:
+  ///
+  /// *                   | Prior                  | New
+  /// ------------------- | ---                    | ---
+  /// Dimension selection | {0, 2}                 | {0, 2}
+  /// Input domain        | [0, 6], [2, 5], [0, 9] | [0, 2], [2, 5], [0, 3]
+  /// Labels              | {"x", "y", "z"}        | {"x", "y", "z"}
+  /// Equiv. input indices| {1, 3, 2}              | {0, 3, 0}
+  /// Equiv. input indices| {x + 1, y, z + 4}      | {x, y, z}
+  ///
+  /// where `x` is any index in `[0, 2]`, `y` is any index in `[2, 5]`, and `z`
+  /// is any index in `[0, 3]`.
+  ///
+  /// \requires `BoxType` satisfies `IsBoxLike` and has a rank compatible with
+  ///     the static rank of the dimension selection.
+  /// \param box The box to extract.
+  template <typename BoxType>
+  BoxSliceOpExpr<BoxType> TranslateBoxSlice(const BoxType& box) const {
+    return {{box, true}, *this};
+  }
+
   // [BEGIN GENERATED: generate_interval_slice_overloads.py]
   // The following code is automatically generated.  Do not modify directly.
 
   /// Extracts a closed interval from the selected dimensions with optional
   /// striding.
   ///
   /// The domain of each selected dimension is transformed by
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dim_expression_nc_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/dim_expression_nc_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dimension_identifier.cc` & `tensorstore-0.1.9/tensorstore/index_space/dimension_identifier.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dimension_identifier.h` & `tensorstore-0.1.9/tensorstore/index_space/dimension_identifier.h`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
   /// Exclusive stop index.  If not specified, defaults to `rank` if `step > 0`
   /// and `-1` if `step < 0`.  A negative value `-n` is equivalent to `rank - n`
   /// (the default value of `-1` if `step < 0` is not subject to this
   /// normalization).
   absl::optional<DimensionIndex> exclusive_stop;
 
   /// Step size, must not equal 0.
-  DimensionIndex step;
+  DimensionIndex step = 1;
 
   /// Returns a Python-style `start:stop` or `start:stop:step` slice expression,
   /// where `start` and `stop` are omitted if equal to `nullopt` and `step` is
   /// omitted if equal to `1`.
   friend std::ostream& operator<<(std::ostream& os, const DimRangeSpec& spec);
 
   friend bool operator==(const DimRangeSpec& a, const DimRangeSpec& b);
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dimension_identifier_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/dimension_identifier_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dimension_index_buffer.h` & `tensorstore-0.1.9/tensorstore/index_space/dimension_index_buffer.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/dimension_selection_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/dimension_selection_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/get_output_range_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/get_output_range_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/identity_transform_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/identity_transform_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_array_slice_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_array_slice_op_test.cc`

 * *Files 4% similar despite different names*

```diff
@@ -429,14 +429,23 @@
       Dims(0, 1).IndexArraySlice(MakeArray<Index>({1, 2}),
                                  MakeArray<Index>({3, 4, 5})),
       absl::StatusCode::kInvalidArgument,
       "Index arrays with shapes \\{2\\}, \\{3\\} cannot be broadcast "
       "to a common shape");
 }
 
+TEST(IndexArraySliceTest, InvalidRank) {
+  auto index_array = tensorstore::AllocateArray<Index>(
+      std::vector<Index>(32, 1), tensorstore::c_order, tensorstore::value_init);
+  TestDimExpressionError(tensorstore::IdentityTransform(2),
+                         Dims(0).IndexArraySlice(index_array),
+                         absl::StatusCode::kInvalidArgument,
+                         "Rank 33 is outside valid range \\[0, 32\\]");
+}
+
 TEST(IndexVectorArraySliceTest, OneDOutputOneDArray) {
   TestDimExpression(/*original_transform=*/
                     IndexTransformBuilder<2, 2>()
                         .input_origin({-10, -100})
                         .input_shape({20, 200})
                         .output_single_input_dimension(0, -2, -3, 0)
                         .output_single_input_dimension(1, 10, 11, 1)
@@ -593,14 +602,29 @@
   TestDimExpressionError(
       IndexTransformBuilder<2, 0>().Finalize().value(),
       Dims(0).IndexVectorArraySlice(MakeArray<Index>({1, 2}), 1),
       absl::StatusCode::kInvalidArgument,
       "Dimension index 1 is outside valid range \\[-1, 1\\)");
 }
 
+TEST(IndexVectorArraySliceTest, InvalidRank) {
+  TestDimExpressionError(
+      tensorstore::IdentityTransform(4),
+      Dims(0, 1).IndexVectorArraySlice(
+          tensorstore::AllocateArray<Index>({1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                                             1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                                             1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                                             1, 2},
+                                            tensorstore::c_order,
+                                            tensorstore::default_init),
+          -1),
+      absl::StatusCode::kInvalidArgument,
+      "Rank 33 is outside valid range \\[0, 32\\]");
+}
+
 TEST(OuterIndexArraySliceTest, Integration) {
   TestDimExpression(/*original_transform=*/
                     IndexTransformBuilder<3, 3>()
                         .input_origin({-10, -100, -2})
                         .input_shape({21, 200, 15})
                         .output_single_input_dimension(0, -2, -3, 0)
                         .output_single_input_dimension(1, 6, 5, 1)
@@ -702,8 +726,18 @@
           .OuterIndexArraySlice(MakeArray<Index>({1, 2}),
                                 MakeArray<Index>({3, 4})),
       absl::StatusCode::kInvalidArgument,
       "Number of selected dimensions \\(1\\) does not equal number of index "
       "arrays \\(2\\)");
 }
 
+TEST(OuterIndexArraySliceTest, InvalidRank) {
+  auto index_array = tensorstore::AllocateArray<Index>(
+      std::vector<Index>(17, 1), tensorstore::c_order, tensorstore::value_init);
+  TestDimExpressionError(
+      tensorstore::IdentityTransform(2),
+      Dims(0, 1).OuterIndexArraySlice(index_array, index_array),
+      absl::StatusCode::kInvalidArgument,
+      "Rank 34 is outside valid range \\[0, 32\\]");
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_domain_builder.h` & `tensorstore-0.1.9/tensorstore/index_space/index_domain_builder.h`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 ///         .origin({1, 2, 3})
 ///         .exclusive_max({4, 5, 6})
 ///         .Finalize()
 ///         .value();
 ///
 template <DimensionIndex Rank = dynamic_rank>
 class IndexDomainBuilder {
+  static_assert(IsValidStaticRank(Rank));
+
  public:
   /// Constructs an invalid `IndexDomainBuilder`.
   ///
   /// \post `valid() == false`
   IndexDomainBuilder(std::nullptr_t) : builder_(nullptr) {}
 
   /// Constructs a valid `IndexDomainBuilder` with the specified rank.
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform.cc`

 * *Files 4% similar despite different names*

```diff
@@ -104,26 +104,53 @@
   for (DimensionIndex i = 0; i < slice_rank; ++i) {
     const DimensionIndex j = transform_dims[i];
     const internal_index_space::InputDimensionRef d = rep->input_dimension(j);
     const IndexInterval orig_domain =
         d.optionally_implicit_domain().effective_interval();
     const IndexInterval new_domain = domain[i];
     if (!Contains(orig_domain, new_domain)) {
-      return Status(
-          absl::StatusCode::kOutOfRange,
+      return absl::OutOfRangeError(
           StrCat("Cannot slice target dimension ", j, " {",
                  d.index_domain_dimension<view>(),
                  "} with index domain dimension ", i, " {", domain[i], "}"));
     }
     d.domain() = new_domain;
     d.implicit_lower_bound() = false;
     d.implicit_upper_bound() = false;
   }
   return TransformAccess::Make<IndexTransform<>>(std::move(rep));
 }
+
+Result<IndexTransform<>> SliceByBox(IndexTransform<> transform,
+                                    BoxView<> domain) {
+  using internal_index_space::TransformAccess;
+  assert(transform.valid());
+  if (transform.input_rank() != domain.rank()) {
+    return absl::InvalidArgumentError(
+        tensorstore::StrCat("Rank of index domain (", transform.input_rank(),
+                            ") must match rank of box (", domain.rank(), ")"));
+  }
+  TransformRep::Ptr<> rep =
+      MutableRep(TransformAccess::rep_ptr<container>(std::move(transform)));
+  for (DimensionIndex i = 0; i < domain.rank(); ++i) {
+    const internal_index_space::InputDimensionRef d = rep->input_dimension(i);
+    const IndexInterval orig_domain =
+        d.optionally_implicit_domain().effective_interval();
+    const IndexInterval new_domain = domain[i];
+    if (!Contains(orig_domain, new_domain)) {
+      return absl::OutOfRangeError(StrCat("Cannot slice dimension ", i, " {",
+                                          d.index_domain_dimension<view>(),
+                                          "} with interval {", domain[i], "}"));
+    }
+    d.domain() = new_domain;
+    d.implicit_lower_bound() = false;
+    d.implicit_upper_bound() = false;
+  }
+  return TransformAccess::Make<IndexTransform<>>(std::move(rep));
+}
 
 }  // namespace internal_index_space
 
 Result<bool> GetOutputRange(IndexTransformView<> transform,
                             MutableBoxView<> output_range) {
   ABSL_ASSERT(output_range.rank() == transform.output_rank());
   absl::FixedArray<bool, internal::kNumInlinedDims> input_dim_used(
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform.h` & `tensorstore-0.1.9/tensorstore/index_space/index_transform.h`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
                                   /*can_move_from_a_to_b=*/false));
   return TransformAccess::Make<IndexTransform<RankA, RankC>>(std::move(rep));
 }
 
 namespace internal_index_space {
 Result<IndexTransform<>> SliceByIndexDomain(IndexTransform<> transform,
                                             IndexDomainView<> domain);
+Result<IndexTransform<>> SliceByBox(IndexTransform<> transform,
+                                    BoxView<> domain);
 }  // namespace internal_index_space
 
 /// Transform from an input index space to an output index space.
 ///
 /// \tparam InputRank Compile-time rank of input space, or `dynamic_rank` (the
 ///     default) to indicate a run-time rank.
 /// \tparam OutputRank Compile-time rank of output space, or `dynamic_rank` (the
@@ -107,14 +109,16 @@
 ///     shared reference to the (immutable) transform.  If equal to `view`, this
 ///     object represents an unowned view of a transform.  Copy constructing a
 ///     `container` index transform from an existing `container` or `view` index
 ///     transform only incurs the cost of an atomic reference count increment.
 template <DimensionIndex InputRank, DimensionIndex OutputRank,
           ContainerKind CKind>
 class IndexTransform {
+  static_assert(IsValidStaticRank(InputRank));
+  static_assert(IsValidStaticRank(OutputRank));
   using Access = internal_index_space::TransformAccess;
 
  public:
   constexpr static DimensionIndex static_rank = InputRank;
   constexpr static DimensionIndex static_input_rank = InputRank;
   constexpr static DimensionIndex static_output_rank = OutputRank;
   constexpr static ContainerKind container_kind = CKind;
@@ -368,42 +372,67 @@
   ///
   /// In the expression  `x | y`, if
   ///   * y is a function having signature `Result<U>(T)`
   ///
   /// Then operator| applies y to the value of x, returning a
   /// Result<U>. See tensorstore::Result operator| for examples.
   template <typename Func>
-  PipelineResultType<const IndexTransform&, Func> operator|(
-      Func&& func) const& {
-    return static_cast<Func&&>(func)(*this);
-  }
-  template <typename Func>
-  PipelineResultType<IndexTransform&&, Func> operator|(Func&& func) && {
-    return static_cast<Func&&>(func)(std::move(*this));
+  friend PipelineResultType<IndexTransform&&, Func> operator|(
+      IndexTransform transform, Func&& func) {
+    return std::forward<Func>(func)(std::move(transform));
   }
 
   /// Prints a string representation of an index space transform.
   ///
   /// This function is intended primarily for tests/debugging.
   friend std::ostream& operator<<(std::ostream& os,
                                   const IndexTransform& transform) {
     internal_index_space::PrintToOstream(os, Access::rep(transform));
     return os;
   }
 
+  /// Restricts the domain of an index transform by a box of the same rank.
+  ///
+  /// This is normally invoked via the pipeline operator:
+  ///
+  ///     TENSORSTORE_ASSIGN_OR_RETURN(auto new_transform, transform | box);
+  ///
+  /// The resultant index transform has a domain with explicit bounds given by
+  /// `box`, but with the dimension labels preserved.
+  ///
+  /// \requires The static rank of `box` must be compatible with the static
+  ///     input rank of `transform`.
+  /// \param box The box to apply.
+  /// \param transform The index transform to restrict.
+  /// \error `absl::StatusCode::kInvalidArgument` if `box.rank()` is not equal
+  ///     to `transform.input_rank()`.
+  /// \error `absl::StatusCode::kInvalidArgument` if `box` is not contained
+  ///     within the explicit bounds of `transform.domain()`.
+  template <DimensionIndex OtherRank>
+  friend std::enable_if_t<
+      IsRankExplicitlyConvertible(OtherRank, InputRank),
+      Result<IndexTransform<MaxStaticRank(InputRank, OtherRank), OutputRank>>>
+  ApplyIndexTransform(BoxView<OtherRank> box, IndexTransform transform) {
+    TENSORSTORE_ASSIGN_OR_RETURN(
+        auto new_transform,
+        internal_index_space::SliceByBox(std::move(transform), box));
+    return {std::in_place, unchecked, std::move(new_transform)};
+  }
+
  private:
   friend class internal_index_space::TransformAccess;
   using Ptr = internal_index_space::TransformRep::Ptr<CKind>;
   Ptr rep_{};
 };
 
 /// Unowned view of an IndexTransform input domain.
 template <DimensionIndex Rank, ContainerKind CKind>
 class IndexDomain {
   using Access = internal_index_space::TransformAccess;
+  static_assert(IsValidStaticRank(Rank));
 
  public:
   using Transform = IndexTransform<Rank, dynamic_rank, CKind>;
   constexpr static DimensionIndex static_rank = Rank;
   using RankType = StaticOrDynamicRank<Rank>;
 
   /// Constructs an invalid index domain.
@@ -612,14 +641,55 @@
 
   template <DimensionIndex RankB, ContainerKind CKindB>
   friend bool operator!=(const IndexDomain& a,
                          const IndexDomain<RankB, CKindB>& b) {
     return !(a == b);
   }
 
+  /// "Pipeline" operator.
+  ///
+  /// In the expression  `x | y`, if
+  ///   * y is a function having signature `Result<U>(T)`
+  ///
+  /// Then operator| applies y to the value of x, returning a
+  /// Result<U>. See tensorstore::Result operator| for examples.
+  template <typename Func>
+  friend PipelineResultType<IndexDomain&&, Func> operator|(
+      IndexDomain transform, Func&& func) {
+    return std::forward<Func>(func)(std::move(transform));
+  }
+
+  /// Restricts an index domain by a box of the same rank.
+  ///
+  /// This is normally invoked via the pipeline operator:
+  ///
+  ///     TENSORSTORE_ASSIGN_OR_RETURN(auto new_domain, domain | box);
+  ///
+  /// The resultant index domain has the explicit bounds given by `box`, but
+  /// preserves the labels of `domain`.
+  ///
+  /// \requires The static rank of `box` must be compatible with the static rank
+  ///     of `domain`.
+  /// \param box The box to apply.
+  /// \param domain The existing index domain to restrict.
+  /// \error `absl::StatusCode::kInvalidArgument` if `box.rank()` is not equal
+  ///     to `domain.rank()`.
+  /// \error `absl::StatusCode::kInvalidArgument` if `box` is not contained
+  ///     within the explicit bounds of `domain`.
+  template <DimensionIndex OtherRank>
+  friend std::enable_if_t<IsRankExplicitlyConvertible(OtherRank, Rank),
+                          Result<IndexDomain<MaxStaticRank(Rank, OtherRank)>>>
+  ApplyIndexTransform(BoxView<OtherRank> box, IndexDomain domain) {
+    TENSORSTORE_ASSIGN_OR_RETURN(
+        auto transform,
+        internal_index_space::SliceByBox(std::move(domain.transform_), box));
+    return {std::in_place,
+            IndexTransform<Rank>(unchecked, std::move(transform))};
+  }
+
  private:
   Transform transform_;
   friend class internal_index_space::TransformAccess;
 };
 
 /// Specializes the HasBoxDomain metafunction for IndexTransform.
 template <DimensionIndex InputRank, DimensionIndex OutputRank,
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_builder.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_builder.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_builder.h` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_builder.h`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,17 @@
 ///     input domain or invalid output index map is not a fatal error; the
 ///     Finalize method will simply return an error `Result` if the invalid
 ///     input domain or output index map has not been overridden with a valid
 ///     one prior to the call to Finalize.
 template <DimensionIndex InputRank = dynamic_rank,
           DimensionIndex OutputRank = dynamic_rank>
 class IndexTransformBuilder {
+  static_assert(IsValidStaticRank(InputRank));
+  static_assert(IsValidStaticRank(OutputRank));
+
  public:
   /// Constructs an invalid `IndexTransformBuilder`.
   ///
   /// \post `valid() == false`
   IndexTransformBuilder(std::nullptr_t) {}
 
   /// Constructs a valid `IndexTransformBuilder` with the specified input and
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_builder_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_builder_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_spec.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_spec.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_spec.h` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_spec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_spec_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_spec_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_testutil.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_transform_testutil.h` & `tensorstore-0.1.9/tensorstore/index_space/index_transform_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar.h` & `tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/index_vector_or_scalar_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/index_vector_or_scalar_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/add_new_dims_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/add_new_dims_op.cc`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 }
 }  // namespace
 
 Result<IndexTransform<>> ApplyAddNewDims(IndexTransform<> transform,
                                          DimensionIndexBuffer* dimensions) {
   const DimensionIndex new_input_rank =
       transform.input_rank() + dimensions->size();
+  TENSORSTORE_RETURN_IF_ERROR(ValidateRank(new_input_rank));
   auto new_rep = NewOrMutableRep(TransformAccess::rep(transform),
                                  new_input_rank, transform.output_rank());
   AddNewDims(TransformAccess::rep(transform), new_rep.get(), dimensions);
   return TransformAccess::Make<IndexTransform<>>(std::move(new_rep));
 }
 
 }  // namespace internal_index_space
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/add_new_dims_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/add_new_dims_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/compose_transforms.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/compose_transforms.cc`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         auto& a_to_c_map = a_to_c_output_index_maps[c_dim];
         auto& result_array_data = a_to_c_map.SetArrayIndexing(a_rank);
         result_array_data.index_range = index_array_data.index_range;
         auto transform_result = TransformArraySubRegion(
             index_array_data.shared_array_view(b_to_c_domain), a_to_b,
             a_to_c_domain.origin().data(), a_to_c_domain.shape().data(),
             result_array_data.byte_strides,
-            /*constraints=*/{});
+            /*constraints=*/{skip_repeated_elements});
         if (!transform_result) return transform_result.status();
         auto new_index_array_origin_pointer =
             StaticDataTypeCast<const Index, unchecked>(*transform_result);
         result_array_data.element_pointer = AddByteOffset(
             new_index_array_origin_pointer,
             -IndexInnerProduct(a_rank, result_array_data.byte_strides,
                                a_to_c_domain.origin().data()));
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/compose_transforms.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/compose_transforms.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/deep_copy_transform_rep_ptr.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/deep_copy_transform_rep_ptr.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/diagonal_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/diagonal_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/diagonal_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/diagonal_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/dim_expression_helper.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/dim_expression_helper.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/dim_expression_testutil.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/dim_expression_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/dimension_selection.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/dimension_selection.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/dimension_selection.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/dimension_selection.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/identity_transform.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/identity_transform.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/identity_transform.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/identity_transform.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/index_array_slice_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/index_array_slice_op.cc`

 * *Files 1% similar despite different names*

```diff
@@ -71,34 +71,36 @@
 ///     dimension; `indexed_dim` is an index into the `*dimensions` sequence.
 /// \param get_index_array_byte_stride Function with signature: `(DimensionIndex
 ///     indexed_dim, DimensionIndex new_dim) -> Index` that returns the byte
 ///     stride for the dimension `new_dim` of the `indexed_dim` index array.
 /// \returns The transform where the output dimensions specified in
 ///     `*dimensions` are mapped using the specified index arrays, and the
 ///     remaining output dimensions are identity mapped.
+/// \error `absl::StatusCode::kInvalidArgument` if the resultant input rank is
+///     invalid.
 template <typename GetNewDimensionShapeFn, typename GetIndexArrayBasePointerFn,
           typename GetIndexArrayByteStrideFn>
-TransformRep::Ptr<> MakeTransformFromJointIndexArrays(
+Result<TransformRep::Ptr<>> MakeTransformFromJointIndexArrays(
     DimensionIndex num_new_dims, TransformRep* orig_transform,
     DimensionIndexBuffer* dimensions,
     GetNewDimensionShapeFn get_new_dimension_bounds,
     GetIndexArrayBasePointerFn get_index_array_base_pointer,
     GetIndexArrayByteStrideFn get_index_array_byte_stride) {
   const DimensionIndex num_indexed_dims = dimensions->size();
   const DimensionIndex output_rank = orig_transform->input_rank;
   const DimensionIndex input_rank =
       output_rank - dimensions->size() + num_new_dims;
+  TENSORSTORE_RETURN_IF_ERROR(ValidateRank(input_rank));
   auto result = TransformRep::Allocate(input_rank, output_rank);
   result->input_rank = input_rank;
   result->output_rank = output_rank;
-  // Set all bounds to explicit, and all labels to explicit.  These defaults are
-  // only used for dimensions corresponding to the domain of the index arrays.
-  // For identity-mapped dimensions, the defaults are overridden.
-  std::fill_n(result->implicit_bitvector_base(),
-              result->implicit_bitvector_storage().size(), 0);
+  // Set all bounds to explicit.  These defaults are only used for dimensions
+  // corresponding to the domain of the index arrays.  For identity-mapped
+  // dimensions, the defaults are overridden.
+  result->implicit_bitvector = 0;
   span<OutputIndexMap> maps = result->output_index_maps().first(output_rank);
   const DimensionIndex num_preserved_dims = output_rank - num_indexed_dims;
   // Set all output dimensions to single_input_dimension index method.  The
   // output dimensions corresponding to the index array dimensions will then be
   // set to either constant or array index method.  All output dimensions not
   // corresponding to the index array dimensions will remain set to the
   // single_input_dimension index method, which allows them to be distinguished.
@@ -227,22 +229,22 @@
         ") does not equal number of index arrays (", index_arrays.size(), ")"));
   }
   const DimensionIndex output_rank = orig_transform->input_rank;
   DimensionIndex input_rank = output_rank - num_indexed_dims;
   for (const auto& index_array : index_arrays) {
     input_rank += index_array.rank();
   }
+  TENSORSTORE_RETURN_IF_ERROR(ValidateRank(input_rank));
   auto result = TransformRep::Allocate(input_rank, output_rank);
   result->input_rank = input_rank;
   result->output_rank = output_rank;
-  // Set all bounds to explicit, and all labels to explicit.  These defaults are
-  // only used for dimensions corresponding to the domain of the index arrays.
-  // For identity-mapped dimensions, the defaults are overridden.
-  std::fill_n(result->implicit_bitvector_base(),
-              result->implicit_bitvector_storage().size(), 0);
+  // Set all bounds to explicit.  These defaults are only used for dimensions
+  // corresponding to the domain of the index arrays.  For identity-mapped
+  // dimensions, the defaults are overridden.
+  result->implicit_bitvector = 0;
   absl::FixedArray<DimensionIndex, internal::kNumInlinedDims>
       index_array_start_dim(num_indexed_dims);
   absl::FixedArray<DimensionIndex, internal::kNumInlinedDims> index_array_order(
       num_indexed_dims);
   std::iota(index_array_order.begin(), index_array_order.end(),
             static_cast<DimensionIndex>(0));
   std::sort(index_array_order.begin(), index_array_order.end(),
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/index_array_slice_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/index_array_slice_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/interval_slice_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/interval_slice_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/interval_slice_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/interval_slice_op.h`

 * *Files 10% similar despite different names*

```diff
@@ -186,11 +186,46 @@
     return ApplyStrideOp(std::move(transform), dimensions,
                          IndexVectorOrScalar(stride_vector));
   }
 
   StrideVector stride_vector;
 };
 
+/// Type representing the DimExpression::{Translate,}Slice(Box) operation.
+template <DimensionIndex Rank>
+struct BoxSliceOp {
+  static constexpr bool selected_dimensions_are_new = false;
+
+  static constexpr DimensionIndex static_selection_rank = Rank;
+
+  constexpr static DimensionIndex GetNewStaticInputRank(
+      DimensionIndex input_rank, DimensionIndex num_input_dims) {
+    TENSORSTORE_CONSTEXPR_ASSERT(
+        (input_rank == dynamic_rank || input_rank >= static_selection_rank) &&
+        "Number of dimensions must not exceed input rank.");
+    return input_rank;
+  }
+
+  constexpr static DimensionIndex GetStaticSelectionRank(
+      DimensionIndex num_input_dims) {
+    TENSORSTORE_CONSTEXPR_ASSERT(
+        IsRankExplicitlyConvertible(num_input_dims, static_selection_rank) &&
+        "Number of selected dimensions must match number of strides.");
+    return num_input_dims == dynamic_rank ? static_selection_rank
+                                          : num_input_dims;
+  }
+
+  Result<IndexTransform<>> Apply(IndexTransform<> transform,
+                                 DimensionIndexBuffer* dimensions) const {
+    return ApplyIntervalSliceOp(
+        std::move(transform), dimensions, IntervalForm::sized, translate,
+        IndexVectorOrScalar(box.origin()), IndexVectorOrScalar(box.shape()), 1);
+  }
+
+  BoxView<Rank> box;
+  bool translate;
+};
+
 }  // namespace internal_index_space
 }  // namespace tensorstore
 
 #endif  // TENSORSTORE_INDEX_SPACE_INTERNAL_INTERVAL_SLICE_OP_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/inverse_transform.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/inverse_transform.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/inverse_transform.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/inverse_transform.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/iterate.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/iterate.cc`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,16 @@
       }
     }
   }
   if (final_input_dim_byte_stride != 0) {
     for (Index j = 0; j < offsets.size(); ++j) {
       offsets[j] = internal::wrap_on_overflow::Add(
           offsets[j],
-          internal::wrap_on_overflow::Multiply(final_input_dim_byte_stride, j));
+          internal::wrap_on_overflow::Multiply(
+              final_input_dim_byte_stride, j + final_input_dim_start_position));
     }
   }
 }
 
 template <std::size_t Arity>
 ArrayIterateResult IterateUsingSimplifiedLayout(
     const SimplifiedDimensionIterationOrder& layout,
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/iterate_impl.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/iterate_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/label_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/label_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/label_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/label_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/mark_explicit_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/mark_explicit_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/mark_explicit_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/mark_explicit_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/propagate_bounds.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/propagate_bounds.cc`

 * *Files 2% similar despite different names*

```diff
@@ -239,19 +239,14 @@
   ABSL_ASSERT(b_rank == b_implicit_lower_bounds.size());
   ABSL_ASSERT(b_rank == b_implicit_upper_bounds.size());
   if (!a_to_b) {
     a_to_b = TransformRep::Allocate(b_rank, b_rank);
     a_to_b->input_rank = a_to_b->output_rank = b_rank;
     SetToIdentityTransform(a_to_b->output_index_maps().first(b_rank));
     a_to_b->input_domain(b_rank).DeepAssign(b_domain);
-    // Mark all labels as implicit (for efficiency, also mark lower/upper bounds
-    // as implicit as well, but the caller will ignore).
-    const auto implicit_bitvector = a_to_b->implicit_bitvector_storage();
-    std::fill(implicit_bitvector.begin(), implicit_bitvector.end(),
-              ~static_cast<std::uint64_t>(0));
     a_to_b->implicit_lower_bounds(b_rank).DeepAssign(b_implicit_lower_bounds);
     a_to_b->implicit_upper_bounds(b_rank).DeepAssign(b_implicit_upper_bounds);
     return a_to_b;
   }
   const DimensionIndex a_rank = a_to_b->input_rank;
   Box<dynamic_rank(internal::kNumInlinedDims)> bounds_temp(a_rank);
   TENSORSTORE_RETURN_IF_ERROR(PropagateBounds(b_domain, b_implicit_lower_bounds,
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/propagate_bounds.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/propagate_bounds.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/single_index_slice_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/single_index_slice_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/single_index_slice_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/single_index_slice_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transform_array.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/transform_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transform_array.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/transform_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep.cc`

 * *Files 1% similar despite different names*

```diff
@@ -133,33 +133,33 @@
   }
   offset_ = other.offset_;
   stride_ = other.stride_;
 }
 
 // Singleton transform instance used when the input and output rank are both
 // zero.
-static TransformRep rank_zero_transform_data{0, 0, 0, 0, 1};
+static TransformRep rank_zero_transform_data{
+    /*.input_rank=*/0,          /*.output_rank=*/0,
+    /*.input_rank_capacity=*/0, /*.output_rank_capacity=*/0,
+    /*.implicit_bitvector=*/0,  /*.reference_count=*/1,
+};
 
 TransformRep::Ptr<> TransformRep::Allocate(
     DimensionIndex input_rank_capacity, DimensionIndex output_rank_capacity) {
-  TENSORSTORE_CHECK(
-      input_rank_capacity >= 0 && output_rank_capacity >= 0 &&
-      input_rank_capacity <= std::numeric_limits<std::int32_t>::max() &&
-      output_rank_capacity <= std::numeric_limits<std::int32_t>::max());
+  TENSORSTORE_CHECK(input_rank_capacity >= 0 && output_rank_capacity >= 0 &&
+                    input_rank_capacity <= kMaxRank &&
+                    output_rank_capacity <= kMaxRank);
   if (input_rank_capacity == 0 && output_rank_capacity == 0) {
     return TransformRep::Ptr<>(&rank_zero_transform_data);
   }
   const size_t total_size =
       // header size
       sizeof(TransformRep) +
       // size of OutputIndexMap array
       sizeof(OutputIndexMap) * output_rank_capacity +
-      // size of implicit_bitvector_storage
-      sizeof(std::uint64_t) * CeilOfRatio(input_rank_capacity * 2,
-                                          static_cast<DimensionIndex>(64)) +
       // size of input_origin, input_shape, and input_labels arrays
       input_rank_capacity * (sizeof(Index) * 2 + sizeof(std::string));
   char* base_ptr = static_cast<char*>(::operator new(total_size));
   TransformRep* ptr =  // NOLINT
       new (base_ptr + sizeof(OutputIndexMap) * output_rank_capacity)
           TransformRep;
   ptr->reference_count.store(1, std::memory_order_relaxed);
@@ -470,15 +470,15 @@
   }
   *output_stride = 0;
   return absl::OkStatus();
 }
 
 TransformRep::Ptr<> GetSubDomain(TransformRep* rep,
                                  span<const DimensionIndex> dims) {
-  ABSL_ASSERT(rep);
+  assert(rep);
   const DimensionIndex old_rank = rep->input_rank;
   const DimensionIndex new_rank = dims.size();
   auto new_rep = TransformRep::Allocate(new_rank, 0);
   new_rep->output_rank = 0;
   new_rep->input_rank = new_rank;
 #ifndef NDEBUG
   absl::FixedArray<bool, internal::kNumInlinedDims> seen_dims(old_rank, false);
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep.h`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,14 @@
 /// This struct is stored in the middle of a dynamically allocated block with
 /// the following layout:
 ///
 ///     OutputIndexMap output_index_maps[output_rank_capacity];
 ///     TransformRep header;
 ///     Index input_origin[input_rank_capacity];
 ///     Index input_shape[input_rank_capacity];
-///     std::uint64_t implicit_bitvector_storage[
-///         CeilOfRatio(2 * input_rank_capacity, 64)];
 ///     std::string input_labels[input_rank_capacity];
 ///
 /// The representation is reference counted, and IndexTransform provide a safe,
 /// immutable public interface for accessing it.  However, internal functions
 /// that holds a unique reference (i.e. `reference_count == 1`) may modify the
 /// representation in place.
 ///
@@ -198,31 +196,38 @@
 /// There are numerous invariants, documented below, that the representation
 /// must satisfy while owned by an IndexTransform.  These invariants are
 /// temporarily violated when building and operating on the representation, but
 /// are always restored before returning an IndexTransform externally.
 struct TransformRep {
   /// The input rank.
   /// \invariant `0 <= input_rank && input_rank <= input_rank_capacity`.
-  std::int32_t input_rank;
+  std::int16_t input_rank;
 
   /// The output rank.
   /// \invariant `0 <= output_rank && output_rank <= output_rank_capacity`.
-  std::int32_t output_rank;
+  std::int16_t output_rank;
 
   /// The length of the `input_origin`, `input_shape`, and `input_labels` arrays
   /// that immediately follow this TransformRep header in memory.
   ///
-  /// \invariant `0 <= input_rank_capacity`.
-  std::int32_t input_rank_capacity;
+  /// \invariant `0 <= input_rank_capacity <= kMaxRank`.
+  std::int16_t input_rank_capacity;
 
   /// The length of the `output_index_maps` array that precedes this
   /// TransformRep header in memory.
   ///
-  /// \invariant `0 <= output_rank_capacity`.
-  std::int32_t output_rank_capacity;
+  /// \invariant `0 <= output_rank_capacity <= kMaxRank`.
+  std::int16_t output_rank_capacity;
+
+  /// Storage for `implicit_lower_bounds` and `implicit_upper_bounds`.  The
+  /// first `kMaxRank` bits are for `implicit_lower_bounds`, then the next
+  /// `kMaxRank` bits are for `implicit_upper_bounds`.
+  uint64_t implicit_bitvector;
+
+  static_assert(kMaxRank * 2 <= 64);
 
   /// Reference count.
   ///
   /// \invariant `0 <= ref_count`.
   std::atomic<std::uint64_t> reference_count;
 
   /// Returns `true` if there is only one reference to this representation.
@@ -263,42 +268,28 @@
   ///
   /// \dchecks `0 <= rank && rank <= input_rank_capacity`.
   MutableBoxView<> input_domain(DimensionIndex rank) {
     ABSL_ASSERT(0 <= rank && rank <= input_rank_capacity);
     return MutableBoxView<>(rank, input_origin().data(), input_shape().data());
   }
 
-  /// Returns the base pointer for the bit vector containing
-  /// `implicit_lower_bounds` and `implicit_upper_bounds`.
-  std::uint64_t* implicit_bitvector_base() {
-    return reinterpret_cast<std::uint64_t*>(input_shape().end());
-  }
-
-  /// Returns the span that stores the bit vector containing
-  /// `implicit_lower_bounds` and `implicit_upper_bounds`.
-  span<std::uint64_t> implicit_bitvector_storage() {
-    return {implicit_bitvector_base(),
-            CeilOfRatio(static_cast<DimensionIndex>(input_rank_capacity) * 2,
-                        static_cast<DimensionIndex>(64))};
-  }
-
   /// Returns the `implicit_lower_bounds` of length `rank`.
   ///
   /// \dchecks `0 <= rank && rank <= input_rank_capacity`.
   BitSpan<std::uint64_t> implicit_lower_bounds(DimensionIndex rank) {
-    ABSL_ASSERT(0 <= rank && rank <= input_rank_capacity);
-    return {implicit_bitvector_base(), 0, rank};
+    assert(0 <= rank && rank <= input_rank_capacity);
+    return {&implicit_bitvector, 0, rank};
   }
 
   /// Returns the `implicit_upper_bounds` of length `rank`.
   ///
   /// \dchecks `0 <= rank && rank <= input_rank_capacity`.
   BitSpan<std::uint64_t> implicit_upper_bounds(DimensionIndex rank) {
-    ABSL_ASSERT(0 <= rank && rank <= input_rank_capacity);
-    return {implicit_bitvector_base(), input_rank_capacity, rank};
+    assert(0 <= rank && rank <= input_rank_capacity);
+    return {&implicit_bitvector, kMaxRank, rank};
   }
 
   /// Returns the `output_index_maps` array of length `output_rank_capacity`.
   ///
   /// \invariant For `0 <= i && i < output_rank`:
   ///     If `output_index_maps()[i].method() == single_input_dimension`:
   ///        `output_index_maps()[i].single_input_dimension()` must be in the
@@ -312,17 +303,16 @@
   span<OutputIndexMap> output_index_maps() {
     return span(reinterpret_cast<OutputIndexMap*>(this) - output_rank_capacity,
                 output_rank_capacity);
   }
 
   /// Returns the `input_labels` array of length `input_rank_capacity`.
   span<std::string> input_labels() {
-    return span(
-        reinterpret_cast<std::string*>(implicit_bitvector_storage().end()),
-        input_rank_capacity);
+    return span(reinterpret_cast<std::string*>(input_shape().end()),
+                input_rank_capacity);
   }
 
   /// Free a TransformRep allocated by Allocate.
   /// \param ptr A pointer returned by `Allocate` and not previously freed.
   /// \dchecks `ptr->reference_count != 0`
   static void Free(TransformRep* ptr);
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transform_rep_impl.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/transform_rep_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transformed_array_impl.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/transformed_array_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/translate_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/translate_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/translate_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/translate_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transpose_op.cc` & `tensorstore-0.1.9/tensorstore/index_space/internal/transpose_op.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/internal/transpose_op.h` & `tensorstore-0.1.9/tensorstore/index_space/internal/transpose_op.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/interval_slice_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/interval_slice_op_test.cc`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 
 /// Tests for the
 /// DimExpression::{{Translate,}{Closed,HalfOpen,Sized}Interval,Stride}
 /// operations.
 
 #include <gmock/gmock.h>
 #include <gtest/gtest.h>
+#include "tensorstore/box.h"
 #include "tensorstore/index_space/dim_expression.h"
 #include "tensorstore/index_space/index_transform_builder.h"
 #include "tensorstore/index_space/internal/dim_expression_testutil.h"
 #include "tensorstore/util/status.h"
 
 namespace {
 
 using tensorstore::AllDims;
+using tensorstore::BoxView;
 using tensorstore::Dims;
 using tensorstore::Index;
 using tensorstore::IndexTransformBuilder;
 using tensorstore::kImplicit;
 using tensorstore::kInfIndex;
 using tensorstore::kInfSize;
 using tensorstore::MakeArray;
@@ -961,8 +963,83 @@
           .Finalize()
           .value(),
       Dims(0).Stride(std::numeric_limits<Index>::min()),
       absl::StatusCode::kInvalidArgument,
       StrCat("Integer overflow computing stride for output dimension 0"));
 }
 
+TEST(BoxSliceTest, Example) {
+  const auto original_transform = IndexTransformBuilder<3, 3>()
+                                      .input_origin({0, 2, 0})
+                                      .input_inclusive_max({6, 5, 9})
+                                      .input_labels({"x", "y", "z"})
+                                      .output_identity_transform()
+                                      .Finalize()
+                                      .value();
+  const auto expected_new_transform = IndexTransformBuilder<3, 3>()
+                                          .input_origin({1, 2, 4})
+                                          .input_inclusive_max({3, 5, 7})
+                                          .input_labels({"x", "y", "z"})
+                                          .output_identity_transform()
+                                          .Finalize()
+                                          .value();
+  const EquivalentIndices equivalent_indices = {
+      {{1, 3, 4}, {1, 3, 4}},
+  };
+  TestDimExpression(
+      /*original_transform=*/original_transform,
+      /*expression=*/Dims(0, 2).BoxSlice(BoxView({1, 4}, {3, 4})),
+      /*expected_new_dimension_selection=*/{0, 2},
+      /*expected_identity_new_transform=*/expected_new_transform,
+      /*expected_new_transform=*/expected_new_transform,
+      /*equivalent_indices=*/equivalent_indices);
+
+  // Test using labels to select dimensions.
+  TestDimExpression(
+      /*original_transform=*/original_transform,
+      /*expression=*/Dims("x", "z").BoxSlice(BoxView({1, 4}, {3, 4})),
+      /*expected_new_dimension_selection=*/{0, 2},
+      /*expected_identity_new_transform=*/expected_new_transform,
+      /*expected_new_transform=*/expected_new_transform,
+      /*equivalent_indices=*/equivalent_indices);
+}
+
+TEST(TranslateBoxSliceTest, Example) {
+  const auto original_transform = IndexTransformBuilder<3, 3>()
+                                      .input_origin({0, 2, 0})
+                                      .input_inclusive_max({6, 5, 9})
+                                      .input_labels({"x", "y", "z"})
+                                      .output_identity_transform()
+                                      .Finalize()
+                                      .value();
+  const auto expected_new_transform =
+      IndexTransformBuilder<3, 3>()
+          .input_origin({0, 2, 0})
+          .input_inclusive_max({2, 5, 3})
+          .input_labels({"x", "y", "z"})
+          .output_single_input_dimension(0, 1, 1, 0)
+          .output_single_input_dimension(1, 1)
+          .output_single_input_dimension(2, 4, 1, 2)
+          .Finalize()
+          .value();
+  const EquivalentIndices equivalent_indices = {
+      {{1, 3, 4}, {0, 3, 0}},
+  };
+  TestDimExpression(
+      /*original_transform=*/original_transform,
+      /*expression=*/Dims(0, 2).TranslateBoxSlice(BoxView({1, 4}, {3, 4})),
+      /*expected_new_dimension_selection=*/{0, 2},
+      /*expected_identity_new_transform=*/expected_new_transform,
+      /*expected_new_transform=*/expected_new_transform,
+      /*equivalent_indices=*/equivalent_indices);
+
+  // Test using labels to select dimensions.
+  TestDimExpression(
+      /*original_transform=*/original_transform,
+      /*expression=*/Dims("x", "z").TranslateBoxSlice(BoxView({1, 4}, {3, 4})),
+      /*expected_new_dimension_selection=*/{0, 2},
+      /*expected_identity_new_transform=*/expected_new_transform,
+      /*expected_new_transform=*/expected_new_transform,
+      /*equivalent_indices=*/equivalent_indices);
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/inverse_transform_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/inverse_transform_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/iterate_benchmark_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/iterate_benchmark_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/iterate_nc_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/iterate_nc_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/iterate_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/iterate_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/json.cc` & `tensorstore-0.1.9/tensorstore/index_space/json.cc`

 * *Files 16% similar despite different names*

```diff
@@ -25,69 +25,94 @@
 namespace {
 ::nlohmann::json EncodeImplicit(::nlohmann::json v, bool implicit) {
   if (!implicit) return v;
   ::nlohmann::json::array_t j;
   j.push_back(std::move(v));
   return j;
 }
-}  // namespace
 
-void to_json(::nlohmann::json& j,  // NOLINT
-             IndexTransformView<> transform) {
-  if (!transform.valid()) {
-    j = ::nlohmann::json(::nlohmann::json::value_t::discarded);
-    return;
-  }
-  ::nlohmann::json::object_t obj;
-  const DimensionIndex input_rank = transform.input_rank();
-  auto input_domain = transform.input_domain();
+struct DomainJsonKeys {
+  const char* rank;
+  const char* inclusive_min;
+  const char* inclusive_max;
+  const char* shape;
+  const char* exclusive_max;
+  const char* labels;
+};
+
+constexpr DomainJsonKeys kIndexDomainJsonKeys = {
+    "rank",  "inclusive_min", "inclusive_max",
+    "shape", "exclusive_max", "labels",
+};
+
+constexpr DomainJsonKeys kIndexTransformJsonKeys = {
+    "input_rank",  "input_inclusive_min", "input_inclusive_max",
+    "input_shape", "input_exclusive_max", "input_labels",
+};
 
-  // Compute the `"input_inclusive_min"` and `"input_exclusive_max"` members.
+void EncodeDomain(::nlohmann::json::object_t& obj, IndexDomainView<> domain,
+                  const DomainJsonKeys& keys) {
+  // Compute the `inclusive_min` and `exclusive_max` members.
+  DimensionIndex rank = domain.rank();
   {
-    auto implicit_lower_bounds = transform.implicit_lower_bounds();
-    auto implicit_upper_bounds = transform.implicit_upper_bounds();
+    auto implicit_lower_bounds = domain.implicit_lower_bounds();
+    auto implicit_upper_bounds = domain.implicit_upper_bounds();
     ::nlohmann::json::array_t j_inclusive_min, j_exclusive_max;
-    j_inclusive_min.reserve(input_rank);
-    j_exclusive_max.reserve(input_rank);
-    for (DimensionIndex i = 0; i < input_rank; ++i) {
-      const auto d = input_domain[i];
+    j_inclusive_min.reserve(rank);
+    j_exclusive_max.reserve(rank);
+    for (DimensionIndex i = 0; i < rank; ++i) {
+      const auto d = domain[i];
       const bool implicit_lower = implicit_lower_bounds[i];
       const bool implicit_upper = implicit_upper_bounds[i];
       j_inclusive_min.push_back(
           d.inclusive_min() == -kInfIndex
               ? EncodeImplicit("-inf", implicit_lower)
               : EncodeImplicit(d.inclusive_min(), implicit_lower));
       j_exclusive_max.push_back(
           d.inclusive_max() == kInfIndex
               ? EncodeImplicit("+inf", implicit_upper)
               : EncodeImplicit(d.exclusive_max(), implicit_upper));
     }
-    obj.emplace("input_inclusive_min", std::move(j_inclusive_min));
-    obj.emplace("input_exclusive_max", std::move(j_exclusive_max));
+    obj.emplace(keys.inclusive_min, std::move(j_inclusive_min));
+    obj.emplace(keys.exclusive_max, std::move(j_exclusive_max));
   }
 
-  // Compute the `"input_labels"` member.
+  // Compute the `labels` member.
   {
     ::nlohmann::json::array_t j_labels;
-    j_labels.reserve(input_rank);
-    auto input_labels = transform.input_labels();
+    j_labels.reserve(rank);
+    auto labels = domain.labels();
     bool encode_labels = false;
-    for (DimensionIndex i = 0; i < input_rank; ++i) {
-      auto const& label = input_labels[i];
+    for (DimensionIndex i = 0; i < rank; ++i) {
+      auto const& label = labels[i];
       if (!label.empty()) {
         encode_labels = true;
       }
       j_labels.push_back(label);
     }
     // If all labels are empty, skip the `"input_labels"` member to produce a
     // shorter representation.
     if (encode_labels) {
-      obj.emplace("input_labels", std::move(j_labels));
+      obj.emplace(keys.labels, std::move(j_labels));
     }
   }
+}
+
+}  // namespace
+
+void to_json(::nlohmann::json& j,  // NOLINT
+             IndexTransformView<> transform) {
+  if (!transform.valid()) {
+    j = ::nlohmann::json(::nlohmann::json::value_t::discarded);
+    return;
+  }
+  ::nlohmann::json::object_t obj;
+  EncodeDomain(obj, transform.input_domain(), kIndexTransformJsonKeys);
+  const DimensionIndex input_rank = transform.input_rank();
+  auto input_domain = transform.input_domain();
 
   // Compute the `"output"` member, which encodes the output index maps in
   // output dimension index order.
   {
     const DimensionIndex output_rank = transform.output_rank();
     ::nlohmann::json::array_t j_outputs;
     j_outputs.reserve(output_rank);
@@ -130,32 +155,91 @@
               AddByteOffset(
                   ElementPointer<const Index>(
                       index_array_data.element_pointer()),
                   IndexInnerProduct(input_rank, input_domain.origin().data(),
                                     index_array_data.byte_strides().data())),
               StridedLayoutView<>(input_rank, index_array_shape.data(),
                                   index_array_data.byte_strides().data()));
-          // TODO(jbms): check bounds
           j_output.emplace("index_array",
                            internal::JsonEncodeNestedArray(
                                index_array, [](const Index* x) { return *x; }));
+          IndexInterval index_range = index_array_data.index_range();
+          // If `index_array` contains values outside `index_range`, encode
+          // `index_range` as well to avoid expanding the range.
+          if (index_range != IndexInterval() &&  // NOLINT
+              !ValidateIndexArrayBounds(index_range, index_array).ok()) {
+            j_output.emplace("index_array_bounds", index_range);
+          }
           break;
         }
       }
       j_outputs.emplace_back(std::move(j_output));
     }
     // If the transform is actually an identity transform, skip the `"output"`
     // member to produce a shorter representation.
     if (!all_identity) {
       obj.emplace("output", std::move(j_outputs));
     }
   }
   j = std::move(obj);
 }
 
+void to_json(::nlohmann::json& j,  // NOLINT
+             IndexDomainView<> domain) {
+  if (!domain.valid()) {
+    j = ::nlohmann::json(::nlohmann::json::value_t::discarded);
+    return;
+  }
+  ::nlohmann::json::object_t obj;
+  EncodeDomain(obj, domain, kIndexDomainJsonKeys);
+  j = std::move(obj);
+}
+
+::nlohmann::json IndexToJson(Index index) {
+  switch (index) {
+    case -kInfIndex:
+      return "-inf";
+    case +kInfIndex:
+      return "+inf";
+    default:
+      return index;
+  }
+}
+
+Result<Index> ParseIndex(const ::nlohmann::json& j) {
+  if (const std::string* s = j.get_ptr<const std::string*>()) {
+    if (*s == "-inf") return -kInfIndex;
+    if (*s == "+inf") return +kInfIndex;
+  }
+  Index value;
+  TENSORSTORE_RETURN_IF_ERROR(internal::JsonRequireValueAs(
+      j, &value, [](Index i) { return tensorstore::IsValidIndex(i); }));
+  return value;
+}
+
+void to_json(::nlohmann::json& j,  // NOLINT
+             IndexInterval interval) {
+  ::nlohmann::json::array_t bounds(2);
+  bounds[0] = IndexToJson(interval.inclusive_min());
+  bounds[1] = IndexToJson(interval.inclusive_max());
+  j = std::move(bounds);
+}
+
+Result<IndexInterval> ParseIndexInterval(const ::nlohmann::json& j) {
+  Index bounds[2];
+  TENSORSTORE_RETURN_IF_ERROR(internal::JsonParseArray(
+      j,
+      [](ptrdiff_t size) { return internal::JsonValidateArrayLength(size, 2); },
+      [&](const ::nlohmann::json& j_value, ptrdiff_t index) {
+        TENSORSTORE_ASSIGN_OR_RETURN(bounds[index], ParseIndex(j_value));
+        return absl::OkStatus();
+      }));
+  return IndexInterval::Closed(bounds[0], bounds[1]);
+}
+
 namespace internal_index_space {
 namespace {
 
 template <typename T>
 using InlinedVector = absl::InlinedVector<T, internal::kNumInlinedDims>;
 
 /// Parses `j` as a 64-bit signed integer, except that `"-inf"` is optionally
@@ -205,14 +289,15 @@
   return internal::JsonParseArray(
       j_bounds,
       [&](DimensionIndex rank) {
         if (*input_rank) {
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonValidateArrayLength(rank, **input_rank));
         } else {
+          TENSORSTORE_RETURN_IF_ERROR(ValidateRank(rank));
           *input_rank = rank;
         }
         values->resize(rank);
         implicit->resize(rank);
         return absl::OkStatus();
       },
       [&](const ::nlohmann::json& j_bound, DimensionIndex i) {
@@ -241,14 +326,15 @@
   return internal::JsonParseArray(
       j_bounds,
       [&](DimensionIndex rank) {
         if (*input_rank) {
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonValidateArrayLength(rank, **input_rank));
         } else {
+          TENSORSTORE_RETURN_IF_ERROR(ValidateRank(rank));
           *input_rank = rank;
         }
         labels->resize(rank);
         return absl::OkStatus();
       },
       [&](const ::nlohmann::json& v, DimensionIndex i) {
         if (!v.is_string()) {
@@ -271,15 +357,16 @@
   return internal_json::ExpectedError(j, "64-bit signed integer");
 }
 
 Status ParseOutput(const ::nlohmann::json& j,
                    OutputOffsetAndStride* offset_and_stride,
                    OutputIndexMapInitializer* output_map) {
   TENSORSTORE_RETURN_IF_ERROR(internal::JsonValidateObjectMembers(
-      j, {"offset", "input_dimension", "index_array", "stride"}));
+      j, {"offset", "input_dimension", "index_array", "stride",
+          "index_array_bounds"}));
 
   TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
       j, "offset", [&](const ::nlohmann::json& value) {
         return internal::JsonRequireValueAs(value, &offset_and_stride->offset);
       }));
 
   TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
@@ -304,14 +391,25 @@
         TENSORSTORE_ASSIGN_OR_RETURN(
             output_map->index_array,
             internal::JsonParseNestedArray(value, &ParseInt64));
         return absl::OkStatus();
       }));
 
   TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
+      j, "index_array_bounds", [&](const ::nlohmann::json& value) {
+        if (!output_map->index_array.data()) {
+          return absl::InvalidArgumentError(
+              "\"index_array_bounds\" is only valid with \"index_array\"");
+        }
+        TENSORSTORE_ASSIGN_OR_RETURN(output_map->index_array_bounds,
+                                     tensorstore::ParseIndexInterval(value));
+        return absl::OkStatus();
+      }));
+
+  TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
       j, "stride", [&](const ::nlohmann::json& value) {
         if (!output_map->input_dimension && !output_map->index_array.data()) {
           return absl::InvalidArgumentError(
               "Either \"input_dimension\" or \"index_array\" must be "
               "specified in "
               "conjunction with \"stride\"");
         }
@@ -336,111 +434,110 @@
       },
       [&](const ::nlohmann::json& j_output, DimensionIndex i) {
         return ParseOutput(j_output, &(*output_offsets_and_strides)[i],
                            &(*output_maps)[i]);
       });
 }
 
-}  // namespace
-
-Result<TransformRep::Ptr<>> ParseIndexTransformAsJson(
-    const ::nlohmann::json& j, DimensionIndex input_rank_constraint,
-    DimensionIndex output_rank_constraint) {
-  if (j.is_discarded()) return TransformRep::Ptr<>(nullptr);
-  auto result = [&]() -> Result<TransformRep::Ptr<>> {
-    absl::optional<DimensionIndex> input_rank, output_rank;
-    IntervalForm interval_form = IntervalForm::half_open;
-    InlinedVector<Index> input_lower, input_upper;
-    InlinedVector<std::string> input_labels;
-    InlinedVector<OutputOffsetAndStride> output_offsets_and_strides;
-    InlinedVector<OutputIndexMapInitializer> output_maps;
-    InlinedVector<bool> implicit_lower_bounds, implicit_upper_bounds;
-    BuilderFlags flags = 0;
-    bool has_output = false;
-
-    TENSORSTORE_RETURN_IF_ERROR(internal::JsonValidateObjectMembers(
-        j, {"input_rank", "input_inclusive_min", "input_shape",
-            "input_inclusive_max", "input_exclusive_max", "input_labels",
-            "output"}));
-
-    const auto upper_bound_error = [] {
-      return absl::InvalidArgumentError(
-          "At most one of \"input_shape\", \"input_inclusive_max\", and "
-          "\"input_exclusive_max\" members must be specified");
+struct TransformParser {
+  absl::optional<DimensionIndex> input_rank, output_rank;
+  IntervalForm interval_form = IntervalForm::half_open;
+  InlinedVector<Index> input_lower, input_upper;
+  InlinedVector<std::string> input_labels;
+  InlinedVector<OutputOffsetAndStride> output_offsets_and_strides;
+  InlinedVector<OutputIndexMapInitializer> output_maps;
+  InlinedVector<bool> implicit_lower_bounds, implicit_upper_bounds;
+  BuilderFlags flags = 0;
+
+  absl::Status ParseDomain(const ::nlohmann::json& j,
+                           const DomainJsonKeys& keys,
+                           DimensionIndex input_rank_constraint) {
+    const auto upper_bound_error = [&] {
+      return absl::InvalidArgumentError(tensorstore::StrCat(
+          "At most one of \"", keys.shape, "\", \"", keys.inclusive_max,
+          "\", and ", "\"", keys.exclusive_max,
+          "\" members must be specified"));
     };
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_rank", [&](const ::nlohmann::json& value) {
+        j, keys.rank, [&](const ::nlohmann::json& value) {
           DimensionIndex rank;
           TENSORSTORE_RETURN_IF_ERROR(
               internal::JsonRequireInteger(value, &rank,
                                            /*strict=*/true,
-                                           /*min_value=*/0));
+                                           /*min_value=*/0,
+                                           /*max_value=*/kMaxRank));
           input_rank = rank;
           return absl::OkStatus();
         }));
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_inclusive_min", [&](const ::nlohmann::json& value) {
+        j, keys.inclusive_min, [&](const ::nlohmann::json& value) {
           flags |= (kSetLower | kSetImplicitLower);
           return ParseInputBounds(value, &input_rank, &input_lower,
                                   &implicit_lower_bounds, -kInfIndex, 0);
         }));
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_shape", [&](const ::nlohmann::json& value) {
+        j, keys.shape, [&](const ::nlohmann::json& value) {
           interval_form = IntervalForm::sized;
           flags |= (kSetUpper | kSetImplicitUpper);
           return ParseInputBounds(value, &input_rank, &input_upper,
                                   &implicit_upper_bounds, 0, +kInfSize);
         }));
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_inclusive_max", [&](const ::nlohmann::json& value) {
+        j, keys.inclusive_max, [&](const ::nlohmann::json& value) {
           if (flags & kSetUpper) return upper_bound_error();
           flags |= (kSetUpper | kSetImplicitUpper);
           interval_form = IntervalForm::closed;
           return ParseInputBounds(value, &input_rank, &input_upper,
                                   &implicit_upper_bounds, 0, +kInfIndex);
         }));
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_exclusive_max", [&](const ::nlohmann::json& value) {
+        j, keys.exclusive_max, [&](const ::nlohmann::json& value) {
           if (flags & kSetUpper) return upper_bound_error();
           flags |= (kSetUpper | kSetImplicitUpper);
           interval_form = IntervalForm::half_open;
           return ParseInputBounds(value, &input_rank, &input_upper,
                                   &implicit_upper_bounds, 0, +kInfIndex + 1);
         }));
 
     TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "input_labels", [&](const ::nlohmann::json& value) {
+        j, keys.labels, [&](const ::nlohmann::json& value) {
           return ParseInputLabels(value, &input_rank, &input_labels);
         }));
 
-    TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
-        j, "output", [&](const ::nlohmann::json& value) {
-          has_output = true;
-          return ParseOutputs(value, &output_rank, &output_offsets_and_strides,
-                              &output_maps);
-        }));
-
     if (!input_rank) {
-      return absl::InvalidArgumentError(
-          "At least one of \"input_rank\", \"input_inclusive_min\", "
-          "\"input_shape\", \"input_inclusive_max\", \"input_exclusive_max\", "
-          "or \"input_labels\" must be specified");
+      return absl::InvalidArgumentError(tensorstore::StrCat(
+          "At least one of \"", keys.rank, "\", \"", keys.inclusive_min, "\", ",
+          "\"", keys.shape, "\", \"", keys.inclusive_max, "\", \"",
+          keys.exclusive_max, "\", ", "or \"", keys.labels,
+          "\" must be specified"));
     }
 
     if (input_rank_constraint != dynamic_rank &&
         *input_rank != input_rank_constraint) {
-      return absl::InvalidArgumentError(StrCat("Expected input rank to be ",
-                                               input_rank_constraint,
-                                               ", but is: ", *input_rank));
+      return absl::InvalidArgumentError(tensorstore::StrCat(
+          "Expected ", keys.rank, " to be ", input_rank_constraint,
+          ", but is: ", *input_rank));
     }
+    return absl::OkStatus();
+  }
+
+  absl::Status ParseOutput(const ::nlohmann::json& j,
+                           DimensionIndex output_rank_constraint) {
+    bool has_output = false;
+    TENSORSTORE_RETURN_IF_ERROR(internal::JsonHandleObjectMember(  //
+        j, "output", [&](const ::nlohmann::json& value) {
+          has_output = true;
+          return ParseOutputs(value, &output_rank, &output_offsets_and_strides,
+                              &output_maps);
+        }));
 
     if (output_rank_constraint != dynamic_rank) {
       if (!output_rank) {
         output_rank = output_rank_constraint;
       } else if (*output_rank != output_rank_constraint) {
         return absl::InvalidArgumentError(StrCat("Expected output rank to be ",
                                                  output_rank_constraint,
@@ -455,14 +552,18 @@
       output_rank = *input_rank;
       output_maps.resize(*input_rank);
       output_offsets_and_strides.resize(*input_rank);
       for (DimensionIndex i = 0; i < *input_rank; ++i) {
         output_maps[i].input_dimension = i;
       }
     }
+    return absl::OkStatus();
+  }
+
+  Result<TransformRep::Ptr<>> Finalize() {
     auto transform = TransformRep::Allocate(*input_rank, *output_rank);
     transform->input_rank = *input_rank;
     transform->output_rank = *output_rank;
     if (flags & kSetLower) {
       std::copy(input_lower.begin(), input_lower.end(),
                 transform->input_origin().begin());
       std::copy(implicit_lower_bounds.begin(), implicit_lower_bounds.end(),
@@ -484,21 +585,59 @@
       auto& map = maps[output_dim];
       map.offset() = output_offsets_and_strides[output_dim].offset;
       map.stride() = output_offsets_and_strides[output_dim].stride;
     }
     TENSORSTORE_RETURN_IF_ERROR(SetOutputIndexMapsAndValidateTransformRep(
         transform.get(), output_maps, interval_form, flags));
     return transform;
+  }
+};
+
+}  // namespace
+
+Result<TransformRep::Ptr<>> ParseIndexTransformFromJson(
+    const ::nlohmann::json& j, DimensionIndex input_rank_constraint,
+    DimensionIndex output_rank_constraint) {
+  if (j.is_discarded()) return TransformRep::Ptr<>(nullptr);
+  auto result = [&]() -> Result<TransformRep::Ptr<>> {
+    TransformParser parser;
+    TENSORSTORE_RETURN_IF_ERROR(internal::JsonValidateObjectMembers(
+        j, {"input_rank", "input_inclusive_min", "input_shape",
+            "input_inclusive_max", "input_exclusive_max", "input_labels",
+            "output"}));
+    TENSORSTORE_RETURN_IF_ERROR(
+        parser.ParseDomain(j, kIndexTransformJsonKeys, input_rank_constraint));
+    TENSORSTORE_RETURN_IF_ERROR(parser.ParseOutput(j, output_rank_constraint));
+    return parser.Finalize();
   }();
 
   if (result) return result;
   return MaybeAnnotateStatus(result.status(),
                              "Error parsing index transform from JSON");
 }
 
+Result<TransformRep::Ptr<>> ParseIndexDomainFromJson(
+    const ::nlohmann::json& j, DimensionIndex rank_constraint) {
+  if (j.is_discarded()) return TransformRep::Ptr<>(nullptr);
+  auto result = [&]() -> Result<TransformRep::Ptr<>> {
+    TransformParser parser;
+    TENSORSTORE_RETURN_IF_ERROR(internal::JsonValidateObjectMembers(
+        j, {"rank", "inclusive_min", "shape", "inclusive_max", "exclusive_max",
+            "labels"}));
+    parser.output_rank = 0;
+    TENSORSTORE_RETURN_IF_ERROR(
+        parser.ParseDomain(j, kIndexDomainJsonKeys, rank_constraint));
+    return parser.Finalize();
+  }();
+
+  if (result) return result;
+  return MaybeAnnotateStatus(result.status(),
+                             "Error parsing index domain from JSON");
+}
+
 }  // namespace internal_index_space
 
 namespace jb = tensorstore::internal::json_binding;
 
 TENSORSTORE_DEFINE_JSON_BINDER(
     IndexTransformSpecBinder,
     jb::Validate(
@@ -520,15 +659,15 @@
                            },
                            jb::DefaultValue(
                                [options](DimensionIndex* r) {
                                  *r = options.rank;
                                },
                                jb::DefaultValue</*NeverIncludeDefaults=*/true>(
                                    [](DimensionIndex* r) { *r = dynamic_rank; },
-                                   jb::Integer<DimensionIndex>(0))))),
+                                   jb::Integer<DimensionIndex>(0, kMaxRank))))),
             jb::Member(
                 "transform",
                 jb::GetterSetter<IndexTransform<>>(
                     [](const IndexTransformSpec& s) -> IndexTransformView<> {
                       return s.transform();
                     },
                     [](IndexTransformSpec& s, IndexTransform<> transform) {
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/json.h` & `tensorstore-0.1.9/tensorstore/driver/downsample/downsample_util.h`

 * *Files 27% similar despite different names*

```diff
@@ -8,222 +8,196 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifndef TENSORSTORE_INDEX_SPACE_JSON_H_
-#define TENSORSTORE_INDEX_SPACE_JSON_H_
+#ifndef TENSORSTORE_DRIVER_DOWNSAMPLE_DOWNSAMPLE_UTIL_H_
+#define TENSORSTORE_DRIVER_DOWNSAMPLE_DOWNSAMPLE_UTIL_H_
 
-/// \file
-/// JSON encoding of index transforms.
-///
-/// An index transform `t` is encoded as a JSON object with the following
-/// members:
-///
-///   `input_rank`: Optional.  If present, must be a a non-negative integer
-///       specifying `t.input_rank()`.  If not present, the input rank is
-///       inferred from the other `input_*` members.
-///
-///   `input_inclusive_min`: Optional.  A list of length `t.input_rank()`
-///       specifying the inclusive lower bounds of the input domain.  Explicit
-///       finite bounds are encoded as integers, e.g. `17`, while explicit
-///       infinite bounds are encoded as the string constants `"-inf"` or
-///       `"+inf"`.  An implicit bound is encoded as a 1-element list containing
-///       the explicit encoding of the bound, e.g. `[17]`, or `["-inf"]`.  If
-///       not present, all dimensions are assumed to have an implicit lower
-///       bound of `-inf` (if `input_shape` is not specified) or an explicit
-///       lower bound of `0` (if `input_shape` is specified).
-///
-///   `input_shape`/`input_exclusive_max`/`input_inclusive_max`: Required (must
-///        specify exactly one of these properties).  A list of length
-///        `t.input_rank()` specifying the upper bounds of the input domain.
-///        The encoding is the same as for the `input_inclusive_min` member.
-///
-///   `input_labels`: Optional.  A list of length `t.input_rank()` specifying
-///       the input dimension labels as strings.  If the `input_labels` member
-///       is not specified, the input dimension labels are all set to the empty
-///       string.
-///
-///   `output`: Optional. A JSON list of length `t.output_rank()` specifying the
-///       output index maps.  If not present, indicates an identity mapping.
-///       Each output index map is encoded as an object with the following
-///       members:
-///
-///         `offset`: Optional.  Specifies the output offset value as an
-///             integer.  Defaults to `0`.
-///
-///         `stride`: Optional.  Specifies the output stride as an integer.
-///             Defaults to `1`.  Only valid to specify in conjunction with an
-///             `input_dimension` or `index_array` member.
-///
-///         `input_dimension`: Optional.  If present, indicates that the output
-///             index map is a single_input_dimension map.  The value must be an
-///             integer specifying the input dimension.  Must not be specified
-///             in conjunction with an `index_array` member.
-///
-///         `index_array`: Optional.  If present, indicates that the output
-///             index map is an array map.  The value must be a nested list of
-///             integers specifying the index array of rank `t.input_rank()`.
-///             The extent of each dimension of the index array must either
-///             equal the extent of the corresponding input dimension, or equal
-///             `1` for broadcasting.
-///
-///       Specifying neither `input_dimension` nor `index_array` indicates a
-///       constant map.
-///
-/// Example encoding:
-///
-///     {
-///         "input_inclusive_min": ["-inf", 7, ["-inf"], [8]],
-///         "input_exclusive_max": ["+inf", 10, ["+inf"], [17]],
-///         "input_labels": ["x", "y", "z", "t"],
-///         "output": [
-///             {"offset": 3},
-///             {"stride": 2, "input_dimension": 2},
-///             {"offset": 7, "index_array": [[ [[1]], [[2]], [[3]], [[4]] ]]}
-///         ]
-///     }
+#include <iosfwd>
 
-#include <type_traits>
-
-#include "absl/status/status.h"
-#include <nlohmann/json.hpp>
+#include "absl/container/inlined_vector.h"
+#include "tensorstore/box.h"
+#include "tensorstore/downsample_method.h"
+#include "tensorstore/index.h"
 #include "tensorstore/index_space/index_transform.h"
-#include "tensorstore/index_space/index_transform_spec.h"
-#include "tensorstore/internal/json_bindable.h"
-#include "tensorstore/json_serialization_options.h"
 #include "tensorstore/util/result.h"
+#include "tensorstore/util/span.h"
 
 namespace tensorstore {
+namespace internal_downsample {
 
-namespace internal_index_space {
-
-/// Converts an IndexTransform to JSON.
-::nlohmann::json EncodeIndexTransformAsJson(TransformRep* transform);
-
-/// Parses an IndexTransform from JSON.
-Result<TransformRep::Ptr<>> ParseIndexTransformAsJson(
-    const ::nlohmann::json& j, DimensionIndex input_rank_constraint,
-    DimensionIndex output_rank_constraint);
-
-/// Options for converting `IndexTransformSpec` to JSON.
-///
-/// See documentation of `IndexTransformSpecBinder` below.
-struct IndexTransformSpecToJsonOptions : public IncludeDefaults,
-                                         public RankConstraint {
-  IndexTransformSpecToJsonOptions(
-      IncludeDefaults include_defaults = IncludeDefaults{true},
-      RankConstraint rank_constraint = {})
-      : IncludeDefaults(include_defaults), RankConstraint(rank_constraint) {}
-};
-
-/// Options for parsing an `IndexTransformSpec` from JSON.
-///
-/// See documentation of `IndexTransformSpecBinder` below.
-struct IndexTransformSpecFromJsonOptions : public RankConstraint {
-  IndexTransformSpecFromJsonOptions(
-      internal::json_binding::NoOptions no_options = {},
-      RankConstraint rank_constraint = {})
-      : RankConstraint(rank_constraint) {}
-};
-
-}  // namespace internal_index_space
-
-/// Encodes an index transform as JSON.
-///
-/// The input domain is specified using the `inclusive_min` and `exclusive_max`
-/// members, and the `outputs` member is omitted if `t` is an identity
-/// transform.
-///
-/// If `!t.valid()`, sets `j` to discarded.
-///
-/// \param j[out] Set to the JSON representation.
-/// \param t Index transform.
-void to_json(::nlohmann::json& j,  // NOLINT
-             IndexTransformView<> t);
-
-/// Decodes an index transform from JSON.
-///
-/// If `j` is `discarded`, returns an invalid index transform.
-///
-/// \param j The JSON representation.
-/// \param input_rank Optional.  Constrains the input rank.
-/// \param output_rank Optional.  Constrains the output rank.
-/// \error `absl::StatusCode::kInvalidArgument` if `j` is not a valid index
-///     transform encoding.
-template <DimensionIndex InputRank = dynamic_rank,
-          DimensionIndex OutputRank = dynamic_rank>
-Result<IndexTransform<InputRank, OutputRank>> ParseIndexTransform(
-    const ::nlohmann::json& j,
-    StaticOrDynamicRank<InputRank> input_rank = GetDefaultRank<InputRank>(),
-    StaticOrDynamicRank<OutputRank> output_rank =
-        GetDefaultRank<OutputRank>()) {
-  TENSORSTORE_ASSIGN_OR_RETURN(auto transform,
-                               internal_index_space::ParseIndexTransformAsJson(
-                                   j, input_rank, output_rank));
-  return internal_index_space::TransformAccess::Make<
-      IndexTransform<InputRank, OutputRank>>(std::move(transform));
-}
-
-/// JSON object binder for `IndexTransformSpec` (for use with
-/// `tensorstore::internal::json_binding::Object`).
-///
-/// A known rank but unknown transform is represented as: `{"rank": 3}`.
-///
-/// A known transform is represented as: `{"transform": ...}`, where the
-/// transform is represented using the normal `IndexTransform` JSON
-/// representation.
-///
-/// An unknown rank is represented by an empty object.
-///
-/// When parsing a JSON object with both `"rank"` and `"transform"` specified,
-/// it is an error if `"rank"` does not match the input rank of the
-/// `"transform"`.
-///
-/// When parsing from JSON, if a `rank_constraint != dynamic_rank` is specified,
-/// composes the parsed `IndexTransformSpec` with
-/// `IndexTransformSpec(rank_constraint)`..
-///
-/// When converting to JSON, if a `rank_constraint != dynamic_rank` is specified
-/// in the options and the object is equal to
-/// `IndexTransformSpec(rank_constraint)`, no members are generated regardless
-/// of the value of `include_defaults`.
-TENSORSTORE_DECLARE_JSON_BINDER(
-    IndexTransformSpecBinder, IndexTransformSpec,
-    internal_index_space::IndexTransformSpecFromJsonOptions,
-    internal_index_space::IndexTransformSpecToJsonOptions,
-    ::nlohmann::json::object_t)
-
-namespace internal {
-namespace json_binding {
-
-// Defined in separate namespace to work around clang-cl bug
-// https://bugs.llvm.org/show_bug.cgi?id=45213
-namespace index_transform_binder {
-inline constexpr auto IndexTransformBinder = [](auto is_loading,
-                                                const auto& options, auto* obj,
-                                                auto* j) {
-  if constexpr (is_loading) {
-    using T = std::decay_t<decltype(*obj)>;
-    TENSORSTORE_ASSIGN_OR_RETURN(
-        *obj, (tensorstore::ParseIndexTransform<T::static_input_rank,
-                                                T::static_output_rank>(*j)));
-  } else {
-    tensorstore::to_json(*j, *obj);
+/// Result type for `PropagateIndexTransformDownsampling`.
+struct PropagatedIndexTransformDownsampling {
+  IndexTransform<> transform;
+  /// Downsample factors for each input dimension of `transform`.
+  absl::InlinedVector<Index, internal::kNumInlinedDims>
+      input_downsample_factors;
+
+  // Comparison and streaming operators are for testing only.
+
+  friend bool operator==(const PropagatedIndexTransformDownsampling& a,
+                         const PropagatedIndexTransformDownsampling& b) {
+    return a.transform == b.transform &&
+           a.input_downsample_factors == b.input_downsample_factors;
   }
-  return absl::OkStatus();
+  friend bool operator!=(const PropagatedIndexTransformDownsampling& a,
+                         const PropagatedIndexTransformDownsampling& b) {
+    return !(a == b);
+  }
+  friend std::ostream& operator<<(
+      std::ostream& os, const PropagatedIndexTransformDownsampling& x);
 };
-}  // namespace index_transform_binder
-
-template <DimensionIndex InputRank, DimensionIndex OutputRank,
-          ContainerKind CKind>
-constexpr auto DefaultBinder<IndexTransform<InputRank, OutputRank, CKind>> =
-    index_transform_binder::IndexTransformBinder;
 
-}  // namespace json_binding
-}  // namespace internal
+/// Propagates a downsampling operation through an index transform.
+///
+/// Given a `downsampled_transform` from index space `downsampled_a` ->
+/// `downsampled_b`, computes `propagated.transform` from index space `a` to
+/// `b`, and `propagated.input_downsample_factors`, such that:
+///
+///   downsampling `b` by `output_downsample_factors` (with bounds of
+///   `output_base_bounds`) and then transforming by `downsampled_transform`
+///
+/// is equivalent to:
+///
+///   transforming `b` by `propgated.transform` and then downsampling by
+///   `propgated.input_downsample_factors` (and possibly "squeezing" some
+///   singleton dimensions that were added).
+///
+/// Note that this function assumes downsampling is performed using a method
+/// such as `DownsampleMethod::kMean` where an output value can be computed as
+/// long as there is at least one in-bounds value.  This function is *not* for
+/// use with `DownsampleMethod::kStride`.
+///
+/// This function supports all index transforms, but some case can be handled
+/// more efficiently than others:
+///
+/// 1. For output dimensions `output_dim` for which
+///    `output_downsample_factors[output_dim] == 1`, the resultant
+///    `propagated.transform` just uses the same output index map unchanged.
+///
+/// 2. If output dimension `output_dim` has a `single_input_dimension` map with
+///    stide of +/-1 from a unique `input_dim`, then
+///    `propagated.input_downsample_factors[input_dim]` is set to
+///    `output_downsample_factors[output_dim]` and `transform` uses the same
+///    output index map, except that the output offset and input bounds for
+///    `input_dim` are adjusted.
+///
+/// 3. If output dimension `output_dim` has a `constant `map, then it is
+///    converted to a `single_input_dimension` map from an additional synthetic
+///    input dimension added to `propagated.transform`.
+///
+/// 4. Otherwise, the output map for `output_dim` is converted to an index array
+///    map that depends on an additional synthetic input dimension added to
+///    `propagated.transform` with domain `[0, downsample_factor)`, where
+///    `downsample_factor = output_downsample_factors[output_dim]`.  Note that
+///    this case applies if the output index map in `downsampled_transform` is
+///    an index array map or a `single_input_dimension` map with non-unit stride
+///    or non-unique input dimension.  It is possible that some of the
+///    `downsample_factor` indices within a given downsampling block are outside
+///    `output_base_bounds` (this function returns an error if none are in
+///    bounds, though).  In that case, since the index transform representation
+///    does not support ragged arrays, any out of bound indices are clamped to
+///    fit in `output_base_bounds`.  If the downsample factor is greater than 2,
+///    this *does* affect the result of the average computation within these
+///    boundary blocks.
+///
+/// If any synthetic input dimensions are added to `transform`, they are
+/// guaranteed to become singleton dimensions after downsampling by
+/// `propagated.input_downsample_factors`, and they must then be "squeezed"
+/// (eliminated) to maintain the equivalence with downsampling before
+/// transforming.
+///
+/// \param downsampled_transform The transform between the downsampled index
+///     domains.
+/// \param output_base_bounds Bounds on the range of the returned
+///     `propagated.transform`.  The returned transform is guaranteed to have a
+///     range contained in `output_base_bounds`.  If the downsampling block
+///     corresponding to a position within the range of `downsampled_transform`
+///     does not intersect `output_base_bounds`, an error is returned.  Note
+///     that the downsampling block must intersect, but need not be fully
+///     contained in, `output_base_bound`.
+/// \param output_downsample_factors Factors by which to downsample each
+///     dimension of `b`.
+/// \param propagated[out] The propagated result.
+/// \pre `downsampled_transform.valid()`
+/// \dchecks `output_downsample_factors.size() == output_base_bounds.rank()`
+/// \dchecks `output_base_bounds.rank() == downsampled_transform.output_rank()`
+/// \dchecks `output_downsample_factors[i] > 0` for all `i`.
+/// \error `absl::StatusCode::kOutOfRange` if downsampling would require data
+///     outside of `output_base_bounds`.
+absl::Status PropagateIndexTransformDownsampling(
+    IndexTransformView<> downsampled_transform, BoxView<> output_base_bounds,
+    span<const Index> output_downsample_factors,
+    PropagatedIndexTransformDownsampling& propagated);
+
+/// Same as above, but with `Result` return value.
+Result<PropagatedIndexTransformDownsampling>
+PropagateIndexTransformDownsampling(
+    IndexTransformView<> downsampled_transform, BoxView<> output_base_bounds,
+    span<const Index> output_downsample_factors);
+
+/// Computes the maximum downsampled interval that can be computed from the
+/// given base interval.
+///
+/// If `method == kStride`, a downsampled position `x` can be computed if
+/// `base_interval` contains `x * downsample_factor`.
+///
+/// If `method == kMean`, a downsampled position `x` can be computed if
+/// `base_interval` intersects
+/// `[x * downsample_factor, (x + 1) * downsample_factor - 1]`.
+IndexInterval DownsampleInterval(IndexInterval base_interval,
+                                 Index downsample_factor,
+                                 DownsampleMethod method);
+
+/// Computes the maximum downsampled region that can be computed from the given
+/// base region.
+///
+/// This simply calls `DownsampleInterval` for each dimension.
+///
+/// \param base_bounds The original (not downsampled) bounds.
+/// \param downsampled_bounds[out] The downsampled bounds.
+/// \param downsample_factors The downsample factors for each dimension.
+/// \param downsample_method The method to use, determines rounding.
+/// \dchecks `base_bounds.rank() == downsampled_bounds.rank()`
+/// \dchecks `base_bounds.rank() == downsample_factors.size()`
+void DownsampleBounds(BoxView<> base_bounds,
+                      MutableBoxView<> downsampled_bounds,
+                      span<const Index> downsample_factors,
+                      DownsampleMethod method);
+
+/// Returns an identity transform over the domain obtained by downsampling
+/// `base_domain`.
+///
+/// The returned transform copies `input_labels`, `implicit_lower_bounds` and
+/// `implicit_upper_bounds` from `base_domain`.  The bounds are obtained from
+/// calling `DownsampleBounds`.
+///
+/// \param base_domain The base domain to downsample.
+/// \param downsample_factors Downsample factor for each dimension of
+///     `base_domain`.  The size must match the rank of `base_domain`.  All
+///     factors must be positive.
+/// \param downsample_method The downsampling method to use.
+/// \returns The new transform.
+IndexTransform<> GetDownsampledDomainIdentityTransform(
+    IndexDomainView<> base_domain, span<const Index> downsample_factors,
+    DownsampleMethod downsample_method);
+
+/// Returns `true` if the range of `base_cell_transform` can be downsampled
+/// independently.
+///
+/// This is true if, and only if, the following conditions are satisfied:
+///
+/// 1. `base_cell_transform` can be inverted by `InverseTransform`.
+///
+/// 2. Each dimension of the domain of the inverse transform is aligned either
+///    to `base_bounds` or to a `downsample_factors` block boundary.
+bool CanDownsampleIndexTransform(IndexTransformView<> base_transform,
+                                 BoxView<> base_bounds,
+                                 span<const Index> downsample_factors);
 
+}  // namespace internal_downsample
 }  // namespace tensorstore
 
-#endif  // TENSORSTORE_INDEX_SPACE_JSON_H_
+#endif  // TENSORSTORE_DRIVER_DOWNSAMPLE_DOWNSAMPLE_UTIL_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/json_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/json_test.cc`

 * *Files 19% similar despite different names*

```diff
@@ -13,31 +13,34 @@
 // limitations under the License.
 
 #include "tensorstore/index_space/json.h"
 
 #include <gmock/gmock.h>
 #include <gtest/gtest.h>
 #include "tensorstore/index_space/dim_expression.h"
+#include "tensorstore/index_space/index_domain_builder.h"
 #include "tensorstore/index_space/index_transform_builder.h"
 #include "tensorstore/internal/json.h"
 #include "tensorstore/internal/json_gtest.h"
 #include "tensorstore/util/result.h"
 #include "tensorstore/util/status.h"
 #include "tensorstore/util/status_testutil.h"
 
 namespace {
 
 using tensorstore::DimensionIndex;
 using tensorstore::dynamic_rank;
 using tensorstore::Index;
+using tensorstore::IndexInterval;
 using tensorstore::IndexTransform;
 using tensorstore::IndexTransformBuilder;
 using tensorstore::IndexTransformSpec;
 using tensorstore::kInfIndex;
 using tensorstore::kInfSize;
+using tensorstore::MatchesJson;
 using tensorstore::MatchesStatus;
 using tensorstore::Result;
 using tensorstore::internal::ParseJson;
 
 IndexTransform<> MakeExampleTransform() {
   return tensorstore::IndexTransformBuilder<4, 3>()
       .input_origin({-kInfIndex, 7, -kInfIndex, 8})
@@ -66,28 +69,33 @@
       .output_constant(0, 3)
       .output_single_input_dimension(1, 0, 2, 2)
       .output_index_array(2, 7, 1,
                           tensorstore::MakeArray<Index>({{
                               {{1}},
                               {{2}},
                               {{3}},
-                          }}))
+                          }}),
+                          IndexInterval::Closed(1, 2))
       .Finalize()
       .value();
 }
 
 ::nlohmann::json MakeUnlabeledExampleJson() {
   return ParseJson(R"(
 {
     "input_inclusive_min": ["-inf", 7, ["-inf"], [8]],
     "input_exclusive_max": ["+inf", 10, ["+inf"], [17]],
     "output": [
         {"offset": 3},
         {"stride": 2, "input_dimension": 2},
-        {"offset": 7, "index_array": [[ [[1]], [[2]], [[3]] ]]}
+        {
+            "offset": 7,
+            "index_array": [[ [[1]], [[2]], [[3]] ]],
+            "index_array_bounds": [1, 2]
+        }
     ]
 }
 )");
 }
 
 ::nlohmann::json MakeLabeledExampleJson() {
   return ParseJson(R"(
@@ -109,14 +117,86 @@
             ::nlohmann::json(MakeUnlabeledExampleTransform()));
 }
 
 TEST(ToJsonTest, Labeled) {
   EXPECT_EQ(MakeLabeledExampleJson(), ::nlohmann::json(MakeExampleTransform()));
 }
 
+TEST(IndexTransformJsonBinderTest, IndexArrayOutOfBounds) {
+  tensorstore::TestJsonBinderRoundTrip<IndexTransform<>>({
+      // Index array does not contain out-of-bounds index.
+      {IndexTransformBuilder(1, 1)
+           .input_shape({3})
+           .output_index_array(0, 0, 1,
+                               tensorstore::MakeArray<Index>({1, 2, 3}))
+           .Finalize()
+           .value(),
+       {
+           {"input_inclusive_min", {0}},
+           {"input_exclusive_max", {3}},
+           {"output",
+            {
+                {{"index_array", {1, 2, 3}}},
+            }},
+       }},
+      // Index array contains out-of-bounds index and `index_range` is
+      // bounded.
+      {IndexTransformBuilder(1, 1)
+           .input_shape({3})
+           .output_index_array(0, 0, 1,
+                               tensorstore::MakeArray<Index>({1, 2, 3}),
+                               IndexInterval::UncheckedClosed(1, 2))
+           .Finalize()
+           .value(),
+       {
+           {"input_inclusive_min", {0}},
+           {"input_exclusive_max", {3}},
+           {"output",
+            {
+                {{"index_array", {1, 2, 3}}, {"index_array_bounds", {1, 2}}},
+            }},
+       }},
+      // Index array contains out-of-bounds index, but `index_range` is
+      // unbounded anyway.
+      {IndexTransformBuilder(1, 1)
+           .input_shape({3})
+           .output_index_array(
+               0, 0, 1, tensorstore::MakeArray<Index>({1, kInfIndex + 1, 3}))
+           .Finalize()
+           .value(),
+       {
+           {"input_inclusive_min", {0}},
+           {"input_exclusive_max", {3}},
+           {"output",
+            {
+                {{"index_array", {1, kInfIndex + 1, 3}}},
+            }},
+       }},
+  });
+  tensorstore::TestJsonBinderToJson<IndexTransform<>>({
+      // Because index array does not contain an out-of-bounds index, the
+      // `index_range` of `[1, 3]` is not encoded.
+      {IndexTransformBuilder(1, 1)
+           .input_shape({3})
+           .output_index_array(0, 0, 1,
+                               tensorstore::MakeArray<Index>({1, 2, 3}),
+                               IndexInterval::Closed(1, 3))
+           .Finalize()
+           .value(),
+       ::testing::Optional(MatchesJson(::nlohmann::json{
+           {"input_inclusive_min", {0}},
+           {"input_exclusive_max", {3}},
+           {"output",
+            {
+                {{"index_array", {1, 2, 3}}},
+            }},
+       }))},
+  });
+}
+
 TEST(ToJsonTest, NullTransform) {
   EXPECT_TRUE(::nlohmann::json(tensorstore::IndexTransform<>()).is_discarded());
 }
 
 TEST(ToJsonTest, IdentityTransform) {
   EXPECT_EQ(ParseJson(R"(
 {
@@ -249,15 +329,15 @@
 }
 
 TEST(ParseIndexTransformTest, StaticInputRankMismatch) {
   EXPECT_THAT(
       (tensorstore::ParseIndexTransform<3, 3>(MakeLabeledExampleJson())),
       MatchesStatus(absl::StatusCode::kInvalidArgument,
                     "Error parsing index transform from JSON: "  //
-                    "Expected input rank to be 3, but is: 4"));
+                    "Expected input_rank to be 3, but is: 4"));
 }
 
 TEST(ParseIndexTransformTest, StaticOutputRankMismatch) {
   EXPECT_THAT(
       (tensorstore::ParseIndexTransform<4, 2>(MakeLabeledExampleJson())),
       MatchesStatus(absl::StatusCode::kInvalidArgument,
                     "Error parsing index transform from JSON: "  //
@@ -613,39 +693,133 @@
 }
 )")),
               MatchesStatus(absl::StatusCode::kInvalidArgument,
                             "Error parsing index transform from JSON: "  //
                             "Dimension label.*"));
 }
 
-void TestIndexTransformSpecRoundTrip(IndexTransformSpec spec,
-                                     ::nlohmann::json json) {
-  SCOPED_TRACE(json.dump());
-  namespace jb = tensorstore::internal::json_binding;
-  const auto binder = jb::Object(tensorstore::IndexTransformSpecBinder);
-  EXPECT_THAT(jb::ToJson(spec, binder), ::testing::Optional(json));
-  EXPECT_THAT(jb::FromJson<IndexTransformSpec>(json, binder),
-              ::testing::Optional(spec));
-}
-
 TEST(IndexTransformSpecTest, JsonBinding) {
-  TestIndexTransformSpecRoundTrip(IndexTransformSpec(),
-                                  ::nlohmann::json::object());
-
-  TestIndexTransformSpecRoundTrip(IndexTransformSpec(3),
-                                  ::nlohmann::json{{"rank", 3}});
+  const auto binder = tensorstore::internal::json_binding::Object(
+      tensorstore::IndexTransformSpecBinder);
+  tensorstore::TestJsonBinderRoundTrip<IndexTransformSpec>(
+      {
+          {IndexTransformSpec(), ::nlohmann::json::object()},
+          {IndexTransformSpec(3), {{"rank", 3}}},
+          {IndexTransformSpec(0), {{"rank", 0}}},
+          {IndexTransformSpec(32), {{"rank", 32}}},
+          {IndexTransformSpec(IndexTransformBuilder<>(2, 1)
+                                  .input_shape({2, 3})
+                                  .output_identity_transform()
+                                  .Finalize()
+                                  .value()),
+           {{"transform",
+             {
+                 {"input_exclusive_max", {2, 3}},
+                 {"input_inclusive_min", {0, 0}},
+                 {"output", {{{"input_dimension", 0}}}},
+             }}}},
+      },
+      binder);
+  tensorstore::TestJsonBinderFromJson<IndexTransformSpec>(
+      {
+          {{{"rank", 33}}, MatchesStatus(absl::StatusCode::kInvalidArgument)},
+      },
+      binder);
+}
+
+TEST(IndexDomainJsonBinderTest, Simple) {
+  tensorstore::TestJsonBinderRoundTrip<tensorstore::IndexDomain<>>({
+      {tensorstore::IndexDomainBuilder<4>()
+           .origin({-kInfIndex, 7, -kInfIndex, 8})
+           .exclusive_max({kInfIndex + 1, 10, kInfIndex + 1, 17})
+           .implicit_lower_bounds({0, 0, 1, 1})
+           .implicit_upper_bounds({0, 0, 1, 1})
+           .labels({"x", "y", "z", "t"})
+           .Finalize()
+           .value(),
+       {
+           {"inclusive_min", {"-inf", 7, {"-inf"}, {8}}},
+           {"exclusive_max", {"+inf", 10, {"+inf"}, {17}}},
+           {"labels", {"x", "y", "z", "t"}},
+       }},
+  });
+  tensorstore::TestJsonBinderFromJson<tensorstore::IndexDomain<>>({
+      {{
+           {"rank", 33},
+       },
+       MatchesStatus(
+           absl::StatusCode::kInvalidArgument,
+           "Error parsing index domain from JSON: "
+           "Error parsing object member \"rank\": "
+           "Expected integer in the range \\[0, 32\\], but received: 33")},
+      {{
+           {"shape", {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                      1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                      1, 1, 1, 1, 1, 1, 1, 1, 1, 1,  //
+                      1, 1, 1}},
+       },
+       MatchesStatus(absl::StatusCode::kInvalidArgument,
+                     "Error parsing index domain from JSON: "
+                     "Error parsing object member \"shape\": "
+                     "Rank 33 is outside valid range \\[0, 32\\]")},
+      {{
+           {"labels", {"", "", "", "", "", "", "", "", "", "",  //
+                       "", "", "", "", "", "", "", "", "", "",  //
+                       "", "", "", "", "", "", "", "", "", "",  //
+                       "", "", ""}},
+       },
+       MatchesStatus(absl::StatusCode::kInvalidArgument,
+                     "Error parsing index domain from JSON: "
+                     "Error parsing object member \"labels\": "
+                     "Rank 33 is outside valid range \\[0, 32\\]")},
+      {{
+           {"inclusive_min", {"-inf", 7, {"-inf"}, {8}}},
+           {"exclusive_max", {"+inf", 10, {"+inf"}, {17}}},
+           {"labels", {"x", "y", "z", "t"}},
+           {"output", "abc"},
+       },
+       MatchesStatus(absl::StatusCode::kInvalidArgument,
+                     "Error parsing index domain from JSON: "
+                     "Object includes extra members: \"output\"")},
+  });
+}
 
-  TestIndexTransformSpecRoundTrip(
-      IndexTransformSpec(IndexTransformBuilder<>(2, 1)
-                             .input_shape({2, 3})
-                             .output_identity_transform()
-                             .Finalize()
-                             .value()),
-      ::nlohmann::json{{"transform",
-                        {
-                            {"input_exclusive_max", {2, 3}},
-                            {"input_inclusive_min", {0, 0}},
-                            {"output", {{{"input_dimension", 0}}}},
-                        }}});
+TEST(IndexBinderTest, Basic) {
+  using tensorstore::kMaxFiniteIndex;
+  tensorstore::TestJsonBinderRoundTrip<Index>(
+      {
+          {-kInfIndex, "-inf"},
+          {+kInfIndex, "+inf"},
+          {-kMaxFiniteIndex, -kMaxFiniteIndex},
+          {0, 0},
+          {5, 5},
+          {+kMaxFiniteIndex, +kMaxFiniteIndex},
+      },
+      tensorstore::internal::json_binding::IndexBinder);
+  tensorstore::TestJsonBinderFromJson<Index>(
+      {
+          {"abc", MatchesStatus(absl::StatusCode::kInvalidArgument)},
+          {-kInfIndex, ::testing::Optional(MatchesJson(-kInfIndex))},
+          {+kInfIndex, ::testing::Optional(MatchesJson(+kInfIndex))},
+          {-kInfIndex - 1, MatchesStatus(absl::StatusCode::kInvalidArgument)},
+          {kInfIndex + 1, MatchesStatus(absl::StatusCode::kInvalidArgument)},
+      },
+      tensorstore::internal::json_binding::IndexBinder);
+}
+
+TEST(IndexIntervalBinderTest, Basic) {
+  using tensorstore::IndexInterval;
+  tensorstore::TestJsonBinderRoundTrip<IndexInterval>({
+      {IndexInterval::UncheckedClosed(5, 10), {5, 10}},
+      {IndexInterval(), {"-inf", "+inf"}},
+      {IndexInterval::UncheckedClosed(5, 4), {5, 4}},
+      {IndexInterval::UncheckedClosed(-kInfIndex, 20), {"-inf", 20}},
+      {IndexInterval::UncheckedClosed(20, +kInfIndex), {20, "+inf"}},
+  });
+  tensorstore::TestJsonBinderFromJson<IndexInterval>({
+      {"abc", MatchesStatus(absl::StatusCode::kInvalidArgument)},
+      {{-kInfIndex - 1, 10}, MatchesStatus(absl::StatusCode::kInvalidArgument)},
+      {{10, 5}, MatchesStatus(absl::StatusCode::kInvalidArgument)},
+  });
 }
 
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/label_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/label_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/mark_explicit_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/mark_explicit_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/move_to_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/move_to_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/output_index_map.h` & `tensorstore-0.1.9/tensorstore/index_space/output_index_map.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/output_index_map_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/output_index_map_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/output_index_method.h` & `tensorstore-0.1.9/tensorstore/index_space/output_index_method.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/propagate_bounds_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/propagate_bounds_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/propagate_input_domain_resize_to_output_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/propagate_input_domain_resize_to_output_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/single_index_slice_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/single_index_slice_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/slice_by_index_domain_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/slice_by_index_domain_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transform_array_constraints.h` & `tensorstore-0.1.9/tensorstore/index_space/transform_array_constraints.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transform_array_constraints_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transform_array_constraints_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transform_array_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transform_array_test.cc`

 * *Files 7% similar despite different names*

```diff
@@ -120,14 +120,56 @@
               .output_index_array(0, 1, 1, MakeArray<Index>({0, 2, 2, 1}))
               .Finalize()
               .value())
           .value();
   EXPECT_EQ(MakeOffsetArray<int>({2}, {2, 4, 4, 3}), new_array);
 }
 
+// Tests that TransformArray correctly handles index arrays that exceed the
+// internal buffer size of 1024.
+TEST(TransformArrayTest, OneDArrayOneDIndexArray1025) {
+  constexpr Index kSize = 1025;
+  auto index_array = tensorstore::AllocateArray<Index>({kSize});
+  for (Index i = 0; i < kSize; ++i) index_array(i) = i;
+  auto new_array =
+      tensorstore::TransformArray(index_array,
+                                  IndexTransformBuilder<1, 1>()
+                                      .input_shape({kSize})
+                                      .output_index_array(0, 0, 1, index_array)
+                                      .Finalize()
+                                      .value())
+          .value();
+  EXPECT_EQ(index_array, new_array);
+}
+
+// Tests that TransformArray retains zero-stride dimensions of the array as
+// zero-stride when `skip_repeated_elements` is specified.
+TEST(TransformArrayTest, TwoDArrayOneDIndexArrayRetainZeroStride) {
+  auto index_array = tensorstore::MakeArray<Index>({0, 1, 2, 3, 4});
+  tensorstore::SharedArray<Index, 2> index_array2;
+  index_array2.element_pointer() = index_array.element_pointer();
+  index_array2.shape()[0] = 5;
+  index_array2.shape()[1] = 2;
+  index_array2.byte_strides()[0] = index_array.byte_strides()[0];
+  index_array2.byte_strides()[1] = 0;
+  EXPECT_EQ(index_array2,
+            MakeArray<Index>({{0, 0}, {1, 1}, {2, 2}, {3, 3}, {4, 4}}));
+  auto new_array =
+      tensorstore::TransformArray(index_array2,
+                                  IndexTransformBuilder<2, 2>()
+                                      .input_shape({5, 2})
+                                      .output_index_array(0, 0, 1, index_array2)
+                                      .output_single_input_dimension(1, 1)
+                                      .Finalize()
+                                      .value())
+          .value();
+  EXPECT_EQ(index_array2, new_array);
+  EXPECT_EQ(index_array2.layout(), new_array.layout());
+}
+
 TEST(TransformArrayTest, IndexArrayBoundsOverflow) {
   auto original_array = tensorstore::MakeOffsetArray<int>({5}, {1, 2, 3, 4});
   EXPECT_THAT(tensorstore::TransformArray(
                   original_array,
                   IndexTransformBuilder<1, 1>()
                       .input_origin({2})
                       .input_shape({4})
```

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transform_rep_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transform_rep_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transformed_array.cc` & `tensorstore-0.1.9/tensorstore/index_space/transformed_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transformed_array.h` & `tensorstore-0.1.9/tensorstore/index_space/transformed_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transformed_array_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transformed_array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/translate_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/translate_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transpose_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transpose_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space/transpose_to_op_test.cc` & `tensorstore-0.1.9/tensorstore/index_space/transpose_to_op_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/index_space.h` & `tensorstore-0.1.9/tensorstore/index_space.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/BUILD` & `tensorstore-0.1.9/tensorstore/internal/BUILD`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/aggregate_writeback_cache.h` & `tensorstore-0.1.9/tensorstore/internal/aggregate_writeback_cache.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/arena.h` & `tensorstore-0.1.9/tensorstore/internal/arena.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/arena_test.cc` & `tensorstore-0.1.9/tensorstore/internal/arena_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_cache.cc` & `tensorstore-0.1.9/tensorstore/internal/async_cache.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_cache.h` & `tensorstore-0.1.9/tensorstore/internal/async_cache.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_cache_test.cc` & `tensorstore-0.1.9/tensorstore/internal/async_cache_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_initialized_cache_mixin.h` & `tensorstore-0.1.9/tensorstore/internal/async_initialized_cache_mixin.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_write_array.cc` & `tensorstore-0.1.9/tensorstore/internal/async_write_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_write_array.h` & `tensorstore-0.1.9/tensorstore/internal/async_write_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/async_write_array_test.cc` & `tensorstore-0.1.9/tensorstore/internal/async_write_array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/attributes.h` & `tensorstore-0.1.9/tensorstore/internal/attributes.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/bit_operations.h` & `tensorstore-0.1.9/tensorstore/internal/bit_operations.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/bit_operations_test.cc` & `tensorstore-0.1.9/tensorstore/internal/bit_operations_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/box_difference.cc` & `tensorstore-0.1.9/tensorstore/internal/box_difference.cc`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 /// by picking one of the non-empty parts for each dimension, with the
 /// constraint that at least one part must not be the "intersection" part.
 ///
 /// As a special case, if the intersection is empty in any dimension, the
 /// difference is simply equal to `outer` (which is just a single box).
 namespace {
 Index GetNumSubtractionSubBoxes(BoxView<> outer, BoxView<> inner) {
-  ABSL_ASSERT(outer.rank() == inner.rank());
+  assert(outer.rank() == inner.rank());
   const DimensionIndex rank = outer.rank();
   Index total_count = 1;
   for (DimensionIndex i = 0; i < rank; ++i) {
     IndexInterval outer_interval = outer[i];
     IndexInterval inner_interval = inner[i];
     Index num_parts = 1;
     if (Intersect(outer_interval, inner_interval).empty()) {
@@ -90,33 +90,33 @@
       // "before" part is non-empty
       ++num_parts;
     }
     if (outer_interval.inclusive_max() > inner_interval.inclusive_max()) {
       // "after" part is non-empty
       ++num_parts;
     }
-    if (MulOverflow(num_parts, total_count, &total_count)) {
-      return std::numeric_limits<Index>::max();
-    }
+    // Note: total_count is bounded by `pow(3, kMaxRank)`, which cannot
+    // overflow.
+    total_count *= num_parts;
   }
   // Subtract 1 for the one box corresponding to the intersection interval in
   // all dimensions, which is not included in the difference.
   return total_count - 1;
 }
 }  // namespace
 
 BoxDifference::BoxDifference(BoxView<> outer, BoxView<> inner)
     : outer_(outer),
       inner_(inner),
       num_sub_boxes_(GetNumSubtractionSubBoxes(outer, inner)) {}
 
 void BoxDifference::GetSubBox(Index sub_box_index, MutableBoxView<> out) const {
   const DimensionIndex rank = out.rank();
-  ABSL_ASSERT(rank == outer_.rank());
-  ABSL_ASSERT(sub_box_index >= 0 && sub_box_index < num_sub_boxes_);
+  assert(rank == outer_.rank());
+  assert(sub_box_index >= 0 && sub_box_index < num_sub_boxes_);
   // Increment by 1, because the all zero bit pattern corresponds to the
   // intersection interval of all dimensions, which is not part of the
   // subtraction result.
   ++sub_box_index;
   for (DimensionIndex i = 0; i < rank; ++i) {
     IndexInterval outer_interval = outer_[i];
     IndexInterval inner_interval = inner_[i];
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/box_difference.h` & `tensorstore-0.1.9/tensorstore/internal/box_difference.h`

 * *Files 11% similar despite different names*

```diff
@@ -35,22 +35,14 @@
   /// \param outer The outer box to reference.  Must remain valid as long as the
   ///     `BoxDifference` object is used.
   /// \param inner The inner box to reference.  Must remain valid as long as the
   ///     `BoxDifference` object is used.
   /// \dchecks `outer.rank() == inner.rank()`.
   BoxDifference(BoxView<> outer, BoxView<> inner);
 
-  /// Returns `true` if the `BoxDifference` data structure is valid.  The data
-  /// structure is invalid if, and only if, the number of sub-boxes would exceed
-  /// `std::numeric_limits<Index>::max()` (and it would anyway be infeasible to
-  /// iterate over that many boxes).
-  bool valid() const {
-    return num_sub_boxes_ != std::numeric_limits<Index>::max();
-  }
-
   /// Returns the rank of the boxes.
   DimensionIndex rank() const { return outer_.rank(); }
 
   /// Returns the number of sub-boxes (at most `pow(3, rank()) - 1`) in the
   /// sequence representing the difference.
   Index num_sub_boxes() const { return num_sub_boxes_; }
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/box_difference_test.cc` & `tensorstore-0.1.9/tensorstore/internal/box_difference_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache.cc` & `tensorstore-0.1.9/tensorstore/internal/cache.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache.h` & `tensorstore-0.1.9/tensorstore/internal/cache.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_impl.h` & `tensorstore-0.1.9/tensorstore/internal/cache_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_key.h` & `tensorstore-0.1.9/tensorstore/internal/cache_key.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_pool_limits.h` & `tensorstore-0.1.9/tensorstore/internal/cache_pool_limits.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_pool_resource.cc` & `tensorstore-0.1.9/tensorstore/internal/cache_pool_resource.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_pool_resource.h` & `tensorstore-0.1.9/tensorstore/internal/cache_pool_resource.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_pool_resource_test.cc` & `tensorstore-0.1.9/tensorstore/internal/cache_pool_resource_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cache_test.cc` & `tensorstore-0.1.9/tensorstore/internal/cache_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/chunk_cache.cc` & `tensorstore-0.1.9/tensorstore/internal/chunk_cache.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/chunk_cache.h` & `tensorstore-0.1.9/tensorstore/internal/chunk_cache.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/chunk_cache_benchmark_test.cc` & `tensorstore-0.1.9/tensorstore/internal/chunk_cache_benchmark_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/chunk_cache_test.cc` & `tensorstore-0.1.9/tensorstore/internal/chunk_cache_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compressed_pair.h` & `tensorstore-0.1.9/tensorstore/internal/compressed_pair.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compressed_pair_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compressed_pair_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/BUILD` & `tensorstore-0.1.9/tensorstore/internal/compression/BUILD`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/blosc.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/blosc.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/blosc.h` & `tensorstore-0.1.9/tensorstore/internal/compression/blosc.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/blosc_compressor.h` & `tensorstore-0.1.9/tensorstore/internal/compression/blosc_compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/blosc_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/blosc_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/bzip2.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/bzip2.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/bzip2.h` & `tensorstore-0.1.9/tensorstore/internal/compression/bzip2.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/bzip2_compressor.h` & `tensorstore-0.1.9/tensorstore/internal/compression/bzip2_compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/bzip2_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/bzip2_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/cord_stream_manager.h` & `tensorstore-0.1.9/tensorstore/internal/compression/cord_stream_manager.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/jpeg.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/jpeg.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/jpeg.h` & `tensorstore-0.1.9/tensorstore/internal/compression/jpeg.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/jpeg_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/jpeg_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/json_specified_compressor.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/json_specified_compressor.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/json_specified_compressor.h` & `tensorstore-0.1.9/tensorstore/internal/compression/json_specified_compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/lzma.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/lzma.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/lzma.h` & `tensorstore-0.1.9/tensorstore/internal/compression/lzma.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/lzma_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/lzma_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation.h` & `tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/neuroglancer_compressed_segmentation_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/neuroglancer_compressed_segmentation_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/xz_compressor.h` & `tensorstore-0.1.9/tensorstore/internal/compression/xz_compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/zlib.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/zlib.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/zlib.h` & `tensorstore-0.1.9/tensorstore/internal/compression/zlib.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/zlib_compressor.h` & `tensorstore-0.1.9/tensorstore/internal/compression/zlib_compressor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/compression/zlib_test.cc` & `tensorstore-0.1.9/tensorstore/internal/compression/zlib_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/concurrency_resource.cc` & `tensorstore-0.1.9/tensorstore/internal/concurrency_resource.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/concurrency_resource.h` & `tensorstore-0.1.9/tensorstore/internal/concurrency_resource.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/concurrency_resource_provider.h` & `tensorstore-0.1.9/tensorstore/internal/concurrency_resource_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/concurrent_testutil.cc` & `tensorstore-0.1.9/tensorstore/internal/concurrent_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/concurrent_testutil.h` & `tensorstore-0.1.9/tensorstore/internal/concurrent_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/container_to_shared.h` & `tensorstore-0.1.9/tensorstore/internal/container_to_shared.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/container_to_shared_test.cc` & `tensorstore-0.1.9/tensorstore/internal/container_to_shared_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/context_binding.h` & `tensorstore-0.1.9/tensorstore/internal/context_binding.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cord_util.cc` & `tensorstore-0.1.9/tensorstore/internal/cord_util.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/cord_util.h` & `tensorstore-0.1.9/tensorstore/internal/cord_util.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_copy_concurrency_resource.cc` & `tensorstore-0.1.9/tensorstore/internal/data_copy_concurrency_resource.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_copy_concurrency_resource.h` & `tensorstore-0.1.9/tensorstore/internal/data_copy_concurrency_resource.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion.cc` & `tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion.h` & `tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_endian_conversion_test.cc` & `tensorstore-0.1.9/tensorstore/internal/data_type_endian_conversion_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_json_binder.cc` & `tensorstore-0.1.9/tensorstore/internal/data_type_json_binder.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_json_binder.h` & `tensorstore-0.1.9/tensorstore/internal/data_type_json_binder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_json_binder_test.cc` & `tensorstore-0.1.9/tensorstore/internal/data_type_json_binder_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_random_generator.cc` & `tensorstore-0.1.9/tensorstore/internal/data_type_random_generator.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/data_type_random_generator.h` & `tensorstore-0.1.9/tensorstore/internal/data_type_random_generator.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/decoded_matches.cc` & `tensorstore-0.1.9/tensorstore/internal/decoded_matches.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/decoded_matches.h` & `tensorstore-0.1.9/tensorstore/internal/decoded_matches.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/decoded_matches_test.cc` & `tensorstore-0.1.9/tensorstore/internal/decoded_matches_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/element_copy_function.h` & `tensorstore-0.1.9/tensorstore/internal/element_copy_function.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/elementwise_function.h` & `tensorstore-0.1.9/tensorstore/internal/elementwise_function.h`

 * *Files 2% similar despite different names*

```diff
@@ -358,15 +358,18 @@
   using Closure = ElementwiseClosure<Arity, ExtraArg...>;
 
   using SpecializedFunctionPointer =
       SpecializedElementwiseFunctionPointer<Arity, ExtraArg...>;
 
   constexpr ElementwiseFunction() = default;
 
-  template <typename LoopTemplate>
+  template <
+      typename LoopTemplate,
+      typename = decltype(&LoopTemplate::template Loop<IterationBufferAccessor<
+                              IterationBufferKind::kContiguous>>)>
   constexpr explicit ElementwiseFunction(LoopTemplate)
       : functions_{
             &LoopTemplate::template Loop<
                 IterationBufferAccessor<IterationBufferKind::kContiguous>>,
             &LoopTemplate::template Loop<
                 IterationBufferAccessor<IterationBufferKind::kStrided>>,
             &LoopTemplate::template Loop<
@@ -460,28 +463,28 @@
 ///     struct MyFunc {
 ///       bool operator()(int *a, float *b);
 ///     };
 ///
 ///     MyFunc obj;
 ///     // Implicitly converts to `ElementwiseFunction`.
 ///     ElementwiseFunction<2> func =
-///         SimpleElementwiseFunction<MyFunc, int, float>();
+///         SimpleElementwiseFunction<MyFunc(int, float)>();
 ///
 ///     // Implicitly converts to `const ElementwiseFunction*` (static constant)
 ///     const ElementwiseFunction<2>* func_ptr =
-///         SimpleElementwiseFunction<MyFunc, int, float>();
+///         SimpleElementwiseFunction<MyFunc(int, float)>();
 ///
 ///     // Converts to the closure `{ func_ptr, &obj }`.
 ///     ElementwiseClosure<2> closure =
-///         SimpleElementwiseFunction<MyFunc, int, float>::Closure(&obj);
+///         SimpleElementwiseFunction<MyFunc(int, float)>::Closure(&obj);
 ///
 ///     // Converts to the closure `{ func_ptr, nullptr }` since `MyFunc` is
 ///     // empty.
 ///     ElementwiseClosure<2> stateless_closure =
-///         SimpleElementwiseFunction<MyFunc, int, float>();
+///         SimpleElementwiseFunction<MyFunc(int, float)>();
 ///
 /// \tparam Func The function object type.  Must be callable with
 ///     `(Element*..., ExtraArg...)`, and return either a type explicitly
 ///     convertible to `bool`, or `void` (which is equivalent to returning
 ///     `true`).
 /// \tparam Element... The element types of the arrays over which the
 ///     element-wise function operates.
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/elementwise_function_test.cc` & `tensorstore-0.1.9/tensorstore/internal/elementwise_function_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/endian_elementwise_conversion.h` & `tensorstore-0.1.9/tensorstore/internal/endian_elementwise_conversion.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/env.cc` & `tensorstore-0.1.9/tensorstore/internal/env.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/env.h` & `tensorstore-0.1.9/tensorstore/internal/env.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/env_test.cc` & `tensorstore-0.1.9/tensorstore/internal/env_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/estimate_heap_usage.h` & `tensorstore-0.1.9/tensorstore/internal/estimate_heap_usage.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/exception_macros.h` & `tensorstore-0.1.9/tensorstore/internal/exception_macros.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/file_io_concurrency_resource.cc` & `tensorstore-0.1.9/tensorstore/internal/file_io_concurrency_resource.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/file_io_concurrency_resource.h` & `tensorstore-0.1.9/tensorstore/internal/file_io_concurrency_resource.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/flat_cord_builder.h` & `tensorstore-0.1.9/tensorstore/internal/flat_cord_builder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/gdb_scripting.h` & `tensorstore-0.1.9/tensorstore/internal/gdb_scripting.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/global_initializer.h` & `tensorstore-0.1.9/tensorstore/internal/global_initializer.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/global_initializer_test.cc` & `tensorstore-0.1.9/tensorstore/internal/global_initializer_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition.cc` & `tensorstore-0.1.9/tensorstore/internal/grid_partition.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition.h` & `tensorstore-0.1.9/tensorstore/internal/grid_partition.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition_impl.cc` & `tensorstore-0.1.9/tensorstore/internal/grid_partition_impl.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition_impl.h` & `tensorstore-0.1.9/tensorstore/internal/grid_partition_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition_impl_test.cc` & `tensorstore-0.1.9/tensorstore/internal/grid_partition_impl_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/grid_partition_test.cc` & `tensorstore-0.1.9/tensorstore/internal/grid_partition_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/half_gtest.h` & `tensorstore-0.1.9/tensorstore/internal/half_gtest.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/BUILD` & `tensorstore-0.1.9/tensorstore/internal/http/BUILD`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "//tensorstore/internal:logging",
         "//tensorstore/util:assert_macros",
         "//tensorstore/util:result",
         "//tensorstore/util:span",
         "//tensorstore/util:status",
         "@com_google_absl//absl/status",
         "@com_google_absl//absl/strings",
-        "@se_haxx_curl//:curl",
+        "@se_curl//:curl",
     ],
 )
 
 tensorstore_cc_test(
     name = "curl_handle_test",
     srcs = ["curl_handle_test.cc"],
     deps = [
@@ -47,15 +47,15 @@
         "//tensorstore/internal:logging",
         "//tensorstore/internal:no_destructor",
         "//tensorstore/util:future",
         "@com_google_absl//absl/status",
         "@com_google_absl//absl/strings",
         "@com_google_absl//absl/synchronization",
         "@com_google_absl//absl/time",
-        "@se_haxx_curl//:curl",
+        "@se_curl//:curl",
     ],
 )
 
 tensorstore_cc_library(
     name = "http",
     srcs = [
         "http_request.cc",
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_handle.cc` & `tensorstore-0.1.9/tensorstore/internal/http/curl_handle.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_handle.h` & `tensorstore-0.1.9/tensorstore/internal/http/curl_handle.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_handle_test.cc` & `tensorstore-0.1.9/tensorstore/internal/http/curl_handle_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_transport.cc` & `tensorstore-0.1.9/tensorstore/internal/http/curl_transport.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_transport.h` & `tensorstore-0.1.9/tensorstore/internal/http/curl_transport.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/curl_transport_test.cc` & `tensorstore-0.1.9/tensorstore/internal/http/curl_transport_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_request.cc` & `tensorstore-0.1.9/tensorstore/internal/http/http_request.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_request.h` & `tensorstore-0.1.9/tensorstore/internal/http/http_request.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_request_test.cc` & `tensorstore-0.1.9/tensorstore/internal/http/http_request_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_response.cc` & `tensorstore-0.1.9/tensorstore/internal/http/http_response.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_response.h` & `tensorstore-0.1.9/tensorstore/internal/http/http_response.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_response_test.cc` & `tensorstore-0.1.9/tensorstore/internal/http/http_response_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/http/http_transport.h` & `tensorstore-0.1.9/tensorstore/internal/http/http_transport.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/integer_overflow.h` & `tensorstore-0.1.9/tensorstore/internal/integer_overflow.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/integer_overflow_test.cc` & `tensorstore-0.1.9/tensorstore/internal/integer_overflow_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/integer_types.h` & `tensorstore-0.1.9/tensorstore/internal/integer_types.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_linked_list.h` & `tensorstore-0.1.9/tensorstore/internal/intrusive_linked_list.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_linked_list_test.cc` & `tensorstore-0.1.9/tensorstore/internal/intrusive_linked_list_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_ptr.h` & `tensorstore-0.1.9/tensorstore/internal/intrusive_ptr.h`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,31 @@
   friend void intrusive_ptr_decrement(const AtomicReferenceCount* p) noexcept {
     if (p->ref_count_.fetch_sub(1, std::memory_order_acq_rel) == 1) {
       delete static_cast<const Derived*>(p);
     }
   }
 
  private:
+  template <typename D>
+  friend bool IncrementReferenceCountIfNonZero(
+      const AtomicReferenceCount<D>& base);
   mutable std::atomic<std::uint32_t> ref_count_{0};
 };
 
+template <typename Derived>
+inline bool IncrementReferenceCountIfNonZero(
+    const AtomicReferenceCount<Derived>& base) {
+  uint32_t count = base.ref_count_.load(std::memory_order_relaxed);
+  do {
+    if (count == 0) return false;
+  } while (!base.ref_count_.compare_exchange_weak(count, count + 1,
+                                                  std::memory_order_acq_rel));
+  return true;
+}
+
 /// Specifies the default behavior of `IntrusivePtr<T>`.
 struct DefaultIntrusivePtrTraits {
   template <typename U>
   using pointer = U*;
 
   /// Called to acquire an additional reference to `p`.
   ///
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_ptr_test.cc` & `tensorstore-0.1.9/tensorstore/internal/intrusive_ptr_test.cc`

 * *Files 20% similar despite different names*

```diff
@@ -396,10 +396,58 @@
   IntrusivePtr<Y, XTraits> y1(new Y);
   IntrusivePtr<X, XTraits> y2 = y1;
   IntrusivePtr<Y, XTraits> y3 = dynamic_pointer_cast<Y>(y2);
   EXPECT_EQ(y2, y1);
   EXPECT_EQ(y3, y1);
 }
 
+struct InvokeInDestructorType
+    : public AtomicReferenceCount<InvokeInDestructorType> {
+  std::function<void()> invoke_in_destructor;
+  ~InvokeInDestructorType() { invoke_in_destructor(); }
+};
+
+TEST(AtomicReferenceCountTest, IncrementReferenceCountIfNonZero) {
+  AtomicReferenceCount<int> x;  // refcount == 0.
+  EXPECT_FALSE(IncrementReferenceCountIfNonZero(x));
+  EXPECT_EQ(0, x.use_count());
+  intrusive_ptr_increment(&x);  // refcount == 1.
+  EXPECT_TRUE(IncrementReferenceCountIfNonZero(x));
+  EXPECT_EQ(2, x.use_count());
+}
+
+TEST(AtomicReferenceCountTest,
+     IncrementReferenceCountIfNonZeroDuringDestructor) {
+  IntrusivePtr<InvokeInDestructorType> ptr(new InvokeInDestructorType);
+
+  // Test that `IncrementReferenceCountIfNonZero` succeeds when reference count
+  // is non-zero.
+  {
+    // Can acquire reference
+    ASSERT_TRUE(tensorstore::internal::IncrementReferenceCountIfNonZero(*ptr));
+    IntrusivePtr<InvokeInDestructorType> ptr2(ptr.get(), adopt_object_ref);
+
+    // Can acquire another reference
+    ASSERT_TRUE(tensorstore::internal::IncrementReferenceCountIfNonZero(*ptr));
+    IntrusivePtr<InvokeInDestructorType> ptr3(ptr.get(), adopt_object_ref);
+  }
+
+  // Test that `IncrementReferenceCountIfNonZero` fails when reference count is
+  // zero (called while destructor is in progress).  This is simulating the case
+  // where a "weak reference" is accessed after the reference count has reached
+  // 0 (and the destructor is called) but before the destructor invalidates the
+  // weak reference.
+  bool test_ran = false;
+  bool could_acquire = false;
+  ptr->invoke_in_destructor = [&, ptr_copy = ptr.get()] {
+    test_ran = true;
+    could_acquire =
+        tensorstore::internal::IncrementReferenceCountIfNonZero(*ptr_copy);
+  };
+  ptr.reset();
+  EXPECT_TRUE(test_ran);
+  EXPECT_FALSE(could_acquire);
+}
+
 }  // namespace custom_traits
 
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree.cc` & `tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree.h` & `tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/intrusive_red_black_tree_test.cc` & `tensorstore-0.1.9/tensorstore/internal/intrusive_red_black_tree_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json.cc` & `tensorstore-0.1.9/tensorstore/internal/json.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json.h` & `tensorstore-0.1.9/tensorstore/internal/json.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_array.cc` & `tensorstore-0.1.9/tensorstore/internal/json_array.cc`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,18 @@
       pointer += byte_stride;
     } else {
       // The new element is an array: handle another nesting level.
       path.push_back(j_array);
       const Index size = j_array->size();
       if (!array.data()) {
         shape_or_position.push_back(size);
+        if (shape_or_position.size() > kMaxRank) {
+          return absl::InvalidArgumentError(tensorstore::StrCat(
+              "Nesting level exceeds maximum rank of ", kMaxRank));
+        }
         if (size == 0) {
           // Allocate zero-element array.
           allocate_array();
           return array;
         }
       } else if (path.size() > static_cast<size_t>(array.rank())) {
         return absl::InvalidArgumentError(StrCat(
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_array.h` & `tensorstore-0.1.9/tensorstore/internal/json_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_array_test.cc` & `tensorstore-0.1.9/tensorstore/internal/json_array_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,24 @@
 
 TEST(JsonParseNestedArrayTest, RankTwo) {
   EXPECT_EQ(tensorstore::MakeArray<std::int64_t>({{1, 2, 3}, {4, 5, 6}}),
             JsonParseNestedArray(::nlohmann::json{{1, 2, 3}, {4, 5, 6}},
                                  &DecodeInt64));
 }
 
+TEST(JsonParseNestedArrayTest, InvalidRank) {
+  ::nlohmann::json j = ::nlohmann::json::array_t{1};
+  for (int level = 1; level < 33; ++level) {
+    j = ::nlohmann::json::array_t{j};
+  }
+  EXPECT_THAT(JsonParseNestedArray(j, &DecodeInt64),
+              MatchesStatus(absl::StatusCode::kInvalidArgument,
+                            "Nesting level exceeds maximum rank of 32"));
+}
+
 TEST(JsonParseNestedArrayTest, DecodeElementError) {
   EXPECT_THAT(JsonParseNestedArray(::nlohmann::json{{1, 2, 3}, {4, 5, "a"}},
                                    &DecodeInt64),
               MatchesStatus(absl::StatusCode::kInvalidArgument,
                             "Error parsing array element at position \\{1, "
                             "2\\}: Invalid integer"));
 }
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_bindable.h` & `tensorstore-0.1.9/tensorstore/internal/json_bindable.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_fwd.h` & `tensorstore-0.1.9/tensorstore/internal/json_fwd.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_gtest.h` & `tensorstore-0.1.9/tensorstore/internal/parse_json_matches.h`

 * *Files 18% similar despite different names*

```diff
@@ -8,42 +8,36 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#ifndef TENSORSTORE_INTERNAL_JSON_GTEST_H_
-#define TENSORSTORE_INTERNAL_JSON_GTEST_H_
+#ifndef TENSORSTORE_INTERNAL_PARSE_JSON_MATCHES_H_
+#define TENSORSTORE_INTERNAL_PARSE_JSON_MATCHES_H_
 
-#include <ostream>
+#include <string>
 
-#include <gmock/gmock.h>
+#include <gtest/gtest.h>
 #include <nlohmann/json.hpp>
-#include "tensorstore/internal/json.h"
-
-namespace nlohmann {
-//
-// Google Test uses PrintTo (with many overloads) to print the results of failed
-// comparisons. Most of the time the default overloads for PrintTo() provided
-// by Google Test magically do the job picking a good way to print things, but
-// in this case there is a bug:
-//     https://github.com/nlohmann/json/issues/709
-// explicitly defining an overload, which must be in the namespace of the class,
-// works around the problem, see ADL for why it must be in the right namespace:
-//     https://en.wikipedia.org/wiki/Argument-dependent_name_lookup
-//
-/// Prints json objects to output streams from within Google Test.
-inline void PrintTo(json const& j, std::ostream* os) { *os << j.dump(); }
-}  // namespace nlohmann
+#include "tensorstore/internal/json_gtest.h"
 
 namespace tensorstore {
+namespace internal {
+
+/// Returns a GoogleMock `std::string` matcher that matches if `json_matcher`
+/// matches the result of `ParseJson` on the specified string.
+///
+/// Example usage:
+///
+///     EXPECT_THAT("{\"a\":\"b\"}",
+///                 ParseJsonMatches(::nlohmann::json{{"a", "b"}}));
+::testing::Matcher<std::string> ParseJsonMatches(
+    ::testing::Matcher<::nlohmann::json> json_matcher);
 
-MATCHER_P(MatchesJson, j, "") {
-  *result_listener << "where the difference is:\n"
-                   << ::nlohmann::json::diff(j, arg).dump(2);
-  return tensorstore::internal_json::JsonSame(arg, j);
-}
+/// Equivalent to `ParseJsonMatches(MatchesJson(json))`.
+::testing::Matcher<std::string> ParseJsonMatches(::nlohmann::json json);
 
+}  // namespace internal
 }  // namespace tensorstore
 
-#endif  // TENSORSTORE_INTERNAL_JSON_GTEST_H_
+#endif  // TENSORSTORE_INTERNAL_PARSE_JSON_MATCHES_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pointer.cc` & `tensorstore-0.1.9/tensorstore/internal/json_pointer.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pointer.h` & `tensorstore-0.1.9/tensorstore/internal/json_pointer.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pointer_test.cc` & `tensorstore-0.1.9/tensorstore/internal/json_pointer_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pprint_python.cc` & `tensorstore-0.1.9/tensorstore/internal/json_pprint_python.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pprint_python.h` & `tensorstore-0.1.9/tensorstore/internal/json_pprint_python.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_pprint_python_test.cc` & `tensorstore-0.1.9/tensorstore/internal/json_pprint_python_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_registry.h` & `tensorstore-0.1.9/tensorstore/internal/json_registry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_registry_fwd.h` & `tensorstore-0.1.9/tensorstore/internal/json_registry_fwd.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_registry_impl.cc` & `tensorstore-0.1.9/tensorstore/internal/json_registry_impl.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_registry_impl.h` & `tensorstore-0.1.9/tensorstore/internal/json_registry_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_registry_test.cc` & `tensorstore-0.1.9/tensorstore/internal/json_registry_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/json_test.cc` & `tensorstore-0.1.9/tensorstore/internal/json_test.cc`

 * *Files 9% similar despite different names*

```diff
@@ -840,137 +840,136 @@
               ::testing::Optional(std::string{}));
   EXPECT_THAT(jb::FromJson<std::string>(::nlohmann::json(4), binder),
               MatchesStatus(absl::StatusCode::kInvalidArgument,
                             "Expected 3, but received: 4"));
 }
 
 TEST(JsonBindingTest, Optional) {
-  EXPECT_THAT(jb::ToJson(std::optional<int>(3)),
-              ::testing::Optional(::nlohmann::json(3)));
-  EXPECT_THAT(jb::FromJson<std::optional<int>>(::nlohmann::json(3)),
-              ::testing::Optional(::testing::Optional(3)));
-  EXPECT_THAT(jb::FromJson<std::optional<int>>(
-                  ::nlohmann::json(::nlohmann::json::value_t::discarded)),
-              ::testing::Optional(std::nullopt));
-  EXPECT_THAT(jb::ToJson(std::optional<int>{}),
-              ::testing::Optional(tensorstore::MatchesJson(
-                  ::nlohmann::json(::nlohmann::json::value_t::discarded))));
+  tensorstore::TestJsonBinderRoundTrip<std::optional<int>>({
+      {3, ::nlohmann::json(3)},
+      {std::nullopt, ::nlohmann::json(::nlohmann::json::value_t::discarded)},
+  });
 }
 
 TEST(JsonBindingTest, OptionalExplicitNullopt) {
   const auto binder =
       jb::Optional(jb::DefaultBinder<>, [] { return "nullopt"; });
-  EXPECT_THAT(jb::ToJson(std::optional<int>(3), binder),
-              ::testing::Optional(::nlohmann::json(3)));
-  EXPECT_THAT(jb::FromJson<std::optional<int>>(::nlohmann::json(3), binder),
-              ::testing::Optional(::testing::Optional(3)));
-  EXPECT_THAT(
-      jb::FromJson<std::optional<int>>(::nlohmann::json("nullopt"), binder),
-      ::testing::Optional(std::nullopt));
-  EXPECT_THAT(jb::ToJson(std::optional<int>{}, binder),
-              ::testing::Optional(::nlohmann::json("nullopt")));
+  tensorstore::TestJsonBinderRoundTrip<std::optional<int>>(
+      {
+          {3, 3},
+          {std::nullopt, "nullopt"},
+      },
+      binder);
 }
 
 TEST(JsonBindingTest, DefaultValueDiscarded) {
   const auto binder =
       jb::DefaultValue([](auto* obj) { *obj = 3; },
                        jb::DefaultValue([](auto* obj) { *obj = 3; }));
-  EXPECT_THAT(jb::ToJson(3, binder, tensorstore::IncludeDefaults{false}),
-              ::testing::Optional(tensorstore::MatchesJson(
-                  ::nlohmann::json(::nlohmann::json::value_t::discarded))));
-  EXPECT_THAT(jb::ToJson(3, binder, tensorstore::IncludeDefaults{true}),
-              ::testing::Optional(::nlohmann::json(3)));
-  EXPECT_THAT(jb::ToJson(4, binder, tensorstore::IncludeDefaults{true}),
-              ::testing::Optional(::nlohmann::json(4)));
-  EXPECT_THAT(jb::ToJson(4, binder, tensorstore::IncludeDefaults{false}),
-              ::testing::Optional(::nlohmann::json(4)));
-  EXPECT_THAT(jb::FromJson<int>(::nlohmann::json(4), binder),
-              ::testing::Optional(4));
-  EXPECT_THAT(jb::FromJson<int>(::nlohmann::json(3), binder),
-              ::testing::Optional(3));
-  EXPECT_THAT(
-      jb::FromJson<int>(::nlohmann::json(::nlohmann::json::value_t::discarded),
-                        binder),
-      ::testing::Optional(3));
+  tensorstore::TestJsonBinderRoundTrip<int>(
+      {
+          {3, ::nlohmann::json(::nlohmann::json::value_t::discarded)},
+          {4, 4},
+      },
+      binder, tensorstore::IncludeDefaults{false});
+  tensorstore::TestJsonBinderRoundTrip<int>(
+      {
+          {3, 3},
+          {4, 4},
+      },
+      binder, tensorstore::IncludeDefaults{true});
 }
 
 TEST(JsonBindingTest, Array) {
   const auto binder = jb::Array();
-  EXPECT_THAT(jb::ToJson(std::vector<int>{1, 2, 3}, binder),
-              ::testing::Optional(::nlohmann::json({1, 2, 3})));
-  EXPECT_THAT(jb::FromJson<std::vector<int>>(::nlohmann::json{1, 2, 3}, binder),
-              ::testing::Optional(std::vector<int>{1, 2, 3}));
-  EXPECT_THAT(
-      jb::FromJson<std::vector<int>>(::nlohmann::json{1, 2, "a"}, binder),
-      MatchesStatus(absl::StatusCode::kInvalidArgument,
-                    "Error parsing value at position 2: Expected integer .*"));
+  tensorstore::TestJsonBinderRoundTrip<std::vector<int>>(
+      {
+          {{1, 2, 3}, {1, 2, 3}},
+      },
+      binder);
+  tensorstore::TestJsonBinderFromJson<std::vector<int>>(
+      {
+          {{1, 2, "a"},
+           MatchesStatus(
+               absl::StatusCode::kInvalidArgument,
+               "Error parsing value at position 2: Expected integer .*")},
+      },
+      binder);
 }
 
 TEST(JsonBindingTest, FixedSizeArray) {
   const auto binder = jb::FixedSizeArray();
-  EXPECT_THAT(jb::ToJson(std::array<int, 3>{{1, 2, 3}}, binder),
-              ::testing::Optional(::nlohmann::json({1, 2, 3})));
-  EXPECT_THAT(
-      (jb::FromJson<std::array<int, 3>>(::nlohmann::json{1, 2, 3}, binder)),
-      ::testing::Optional(std::array<int, 3>{{1, 2, 3}}));
-  EXPECT_THAT(
-      (jb::FromJson<std::array<int, 3>>(::nlohmann::json{1, 2, 3, 4}, binder)),
-      MatchesStatus(absl::StatusCode::kInvalidArgument,
-                    "Array has length 4 but should have length 3"));
+  tensorstore::TestJsonBinderRoundTrip<std::array<int, 3>>(
+      {
+          {{{1, 2, 3}}, {1, 2, 3}},
+      },
+      binder);
+  tensorstore::TestJsonBinderFromJson<std::array<int, 3>>(
+      {
+
+          {{1, 2, 3, 4},
+           MatchesStatus(absl::StatusCode::kInvalidArgument,
+                         "Array has length 4 but should have length 3")},
+      },
+      binder);
 }
 
 TEST(JsonBindingTest, Enum) {
   enum class TestEnum { a, b };
   const auto binder = jb::Enum<TestEnum, std::string_view>({
       {TestEnum::a, "a"},
       {TestEnum::b, "b"},
   });
-  EXPECT_THAT(jb::ToJson(TestEnum::a, binder),
-              ::testing::Optional(std::string("a")));
-  EXPECT_THAT(jb::ToJson(TestEnum::b, binder),
-              ::testing::Optional(std::string("b")));
-  EXPECT_THAT(jb::FromJson<TestEnum>(::nlohmann::json("a"), binder),
-              ::testing::Optional(TestEnum::a));
-  EXPECT_THAT(jb::FromJson<TestEnum>(::nlohmann::json("b"), binder),
-              ::testing::Optional(TestEnum::b));
-  EXPECT_THAT(
-      jb::FromJson<TestEnum>(::nlohmann::json("c"), binder),
-      MatchesStatus(absl::StatusCode::kInvalidArgument,
-                    "Expected one of \"a\", \"b\", but received: \"c\""));
+  tensorstore::TestJsonBinderRoundTrip<TestEnum>(
+      {
+          {TestEnum::a, "a"},
+          {TestEnum::b, "b"},
+      },
+      binder);
+  tensorstore::TestJsonBinderFromJson<TestEnum>(
+      {
+          {"c",
+           MatchesStatus(absl::StatusCode::kInvalidArgument,
+                         "Expected one of \"a\", \"b\", but received: \"c\"")},
+      },
+      binder);
 }
 
 // Tests `FixedSizeArray` applied to `tensorstore::span<tensorstore::Index, 3>`.
 TEST(JsonBindingTest, StaticRankBox) {
   using Value = tensorstore::Box<3>;
   const auto binder = jb::Object(
       jb::Member("origin", jb::Projection([](auto& x) { return x.origin(); })),
       jb::Member("shape", jb::Projection([](auto& x) { return x.shape(); })));
-  const auto value = Value({1, 2, 3}, {4, 5, 6});
-  const ::nlohmann::json json{{"origin", {1, 2, 3}}, {"shape", {4, 5, 6}}};
-  EXPECT_THAT(jb::ToJson(value, binder), ::testing::Optional(json));
-  EXPECT_THAT(jb::FromJson<Value>(json, binder), ::testing::Optional(value));
+  tensorstore::TestJsonBinderRoundTrip<Value>(
+      {
+          {Value({1, 2, 3}, {4, 5, 6}),
+           {{"origin", {1, 2, 3}}, {"shape", {4, 5, 6}}}},
+      },
+      binder);
 }
 
 // Tests `FixedSizeArray` applied to `tensorstore::span<tensorstore::Index>`.
 TEST(JsonBindingTest, DynamicRankBox) {
   using Value = tensorstore::Box<>;
   const auto binder = jb::Object(
       jb::Member("rank", jb::GetterSetter(
                              [](auto& x) { return x.rank(); },
                              [](auto& x, tensorstore::DimensionIndex rank) {
                                x.set_rank(rank);
                              },
                              jb::Integer(0))),
       jb::Member("origin", jb::Projection([](auto& x) { return x.origin(); })),
       jb::Member("shape", jb::Projection([](auto& x) { return x.shape(); })));
-  const auto value = Value({1, 2, 3}, {4, 5, 6});
-  const ::nlohmann::json json{
-      {"rank", 3}, {"origin", {1, 2, 3}}, {"shape", {4, 5, 6}}};
-  EXPECT_THAT(jb::ToJson(value, binder), ::testing::Optional(json));
-  EXPECT_THAT(jb::FromJson<Value>(json, binder), ::testing::Optional(value));
+  tensorstore::TestJsonBinderRoundTrip<Value>(
+      {
+          {Value({1, 2, 3}, {4, 5, 6}),
+           {{"rank", 3}, {"origin", {1, 2, 3}}, {"shape", {4, 5, 6}}}},
+      },
+      binder);
 }
 
 TEST(JsonSame, Basic) {
   EXPECT_TRUE(tensorstore::internal_json::JsonSame(1.0, 1));
   EXPECT_FALSE(tensorstore::internal_json::JsonSame(
       ::nlohmann::json::value_t::discarded, ::nlohmann::json::value_t::null));
   EXPECT_TRUE(tensorstore::internal_json::JsonSame(
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache.h` & `tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_test.cc` & `tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_testutil.cc` & `tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/kvs_backed_cache_testutil.h` & `tensorstore-0.1.9/tensorstore/internal/kvs_backed_cache_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/lock_collection.cc` & `tensorstore-0.1.9/tensorstore/internal/lock_collection.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/lock_collection.h` & `tensorstore-0.1.9/tensorstore/internal/lock_collection.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/lock_collection_test.cc` & `tensorstore-0.1.9/tensorstore/internal/lock_collection_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/log_message.cc` & `tensorstore-0.1.9/tensorstore/internal/log_message.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/log_message.h` & `tensorstore-0.1.9/tensorstore/internal/log_message.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/logging.h` & `tensorstore-0.1.9/tensorstore/internal/logging.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/masked_array.cc` & `tensorstore-0.1.9/tensorstore/internal/masked_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/masked_array.h` & `tensorstore-0.1.9/tensorstore/internal/masked_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/masked_array_test.cc` & `tensorstore-0.1.9/tensorstore/internal/masked_array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/masked_array_testutil.cc` & `tensorstore-0.1.9/tensorstore/internal/masked_array_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/masked_array_testutil.h` & `tensorstore-0.1.9/tensorstore/internal/masked_array_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/memory.h` & `tensorstore-0.1.9/tensorstore/internal/memory.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/meta.h` & `tensorstore-0.1.9/tensorstore/internal/meta.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/meta_test.cc` & `tensorstore-0.1.9/tensorstore/internal/meta_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/multi_vector.h` & `tensorstore-0.1.9/tensorstore/internal/multi_vector.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/multi_vector_impl.h` & `tensorstore-0.1.9/tensorstore/internal/multi_vector_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/multi_vector_test.cc` & `tensorstore-0.1.9/tensorstore/internal/multi_vector_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/multi_vector_view.h` & `tensorstore-0.1.9/tensorstore/internal/multi_vector_view.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/multi_vector_view_test.cc` & `tensorstore-0.1.9/tensorstore/internal/multi_vector_view_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/mutex.h` & `tensorstore-0.1.9/tensorstore/internal/mutex.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_array.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_array.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_array_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_array_util.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_array_util.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_buffer_management.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_buffer_management.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_copy.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_copy.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_copy.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_copy.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_copy_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_copy_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_data_type_conversion_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_data_type_conversion_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_input_transform_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_input_transform_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_elementwise_output_transform_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_elementwise_output_transform_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_transformed_array_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_transformed_array_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_util.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_util.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_util.h` & `tensorstore-0.1.9/tensorstore/internal/nditerable_util.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/nditerable_util_test.cc` & `tensorstore-0.1.9/tensorstore/internal/nditerable_util_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/no_destructor.h` & `tensorstore-0.1.9/tensorstore/internal/no_destructor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/no_destructor_test.cc` & `tensorstore-0.1.9/tensorstore/internal/no_destructor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/non_compile_bypass.h` & `tensorstore-0.1.9/tensorstore/internal/non_compile_bypass.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/BUILD` & `tensorstore-0.1.9/tensorstore/internal/oauth2/BUILD`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/fake_private_key.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/fake_private_key.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/fake_private_key.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/fake_private_key.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/fixed_token_auth_provider_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/fixed_token_auth_provider_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/gce_auth_provider_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/gce_auth_provider_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_auth_provider_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_auth_provider_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/google_service_account_auth_provider_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/google_service_account_auth_provider_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth2_auth_provider_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth2_auth_provider_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils.h` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/oauth2/oauth_utils_test.cc` & `tensorstore-0.1.9/tensorstore/internal/oauth2/oauth_utils_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/open_mode_spec.cc` & `tensorstore-0.1.9/tensorstore/internal/open_mode_spec.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/open_mode_spec.h` & `tensorstore-0.1.9/tensorstore/internal/open_mode_spec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/os_error_code.cc` & `tensorstore-0.1.9/tensorstore/internal/os_error_code.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/os_error_code.h` & `tensorstore-0.1.9/tensorstore/internal/os_error_code.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/parse_json_matches.cc` & `tensorstore-0.1.9/tensorstore/internal/parse_json_matches.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/parse_json_matches_test.cc` & `tensorstore-0.1.9/tensorstore/internal/parse_json_matches_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/path.cc` & `tensorstore-0.1.9/tensorstore/internal/path.cc`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     if (!IsValidSchemeChar(uri[scheme_loc++])) {
       // Illegal Scheme found. Everything is a path.
       return;
     }
   }
 
   // 1. Parse host
-  auto path_loc = remaining.find("/");
+  auto path_loc = remaining.find('/');
   if (path_loc == absl::string_view::npos) {
     // No path, everything is the host.
     if (host) *host = remaining;
     if (path) *path = absl::string_view(remaining.data() + remaining.size(), 0);
     return;
   }
   // 2. There is a host and a path.
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/path.h` & `tensorstore-0.1.9/tensorstore/internal/path.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/path_test.cc` & `tensorstore-0.1.9/tensorstore/internal/path_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/poly.cc` & `tensorstore-0.1.9/tensorstore/internal/poly.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/poly.h` & `tensorstore-0.1.9/tensorstore/internal/poly.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/poly_impl.h` & `tensorstore-0.1.9/tensorstore/internal/poly_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/poly_test.cc` & `tensorstore-0.1.9/tensorstore/internal/poly_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/preprocessor.h` & `tensorstore-0.1.9/tensorstore/internal/preprocessor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/queue_testutil.h` & `tensorstore-0.1.9/tensorstore/internal/queue_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/retry.cc` & `tensorstore-0.1.9/tensorstore/internal/retry.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/retry.h` & `tensorstore-0.1.9/tensorstore/internal/retry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/retry_test.cc` & `tensorstore-0.1.9/tensorstore/internal/retry_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/source_location.h` & `tensorstore-0.1.9/tensorstore/internal/source_location.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder.cc` & `tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder.h` & `tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/staleness_bound_json_binder_test.cc` & `tensorstore-0.1.9/tensorstore/internal/staleness_bound_json_binder_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/string_like.h` & `tensorstore-0.1.9/tensorstore/internal/string_like.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/string_like_test.cc` & `tensorstore-0.1.9/tensorstore/internal/string_like_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/tagged_ptr.h` & `tensorstore-0.1.9/tensorstore/internal/tagged_ptr.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/tagged_ptr_test.cc` & `tensorstore-0.1.9/tensorstore/internal/tagged_ptr_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/test_util.cc` & `tensorstore-0.1.9/tensorstore/internal/test_util.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/test_util.h` & `tensorstore-0.1.9/tensorstore/internal/test_util.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/thread_pool.cc` & `tensorstore-0.1.9/tensorstore/internal/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/thread_pool.h` & `tensorstore-0.1.9/tensorstore/internal/thread_pool.h`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 namespace internal {
 
 /// Returns a detached thread pool executor.
 ///
 /// The thread pool remains alive until the last copy of the returned executor
 /// is destroyed and all queued work has finished.
 ///
-/// \param num_threads Number of threads to use.
-Executor DetachedThreadPool(std::size_t num_threads);
+/// \param num_threads Number of threads to use.  By default, the number of
+///     threads is unbounded.
+Executor DetachedThreadPool(
+    size_t num_threads = std::numeric_limits<size_t>::max());
 
 }  // namespace internal
 }  // namespace tensorstore
 
 #endif  //  TENSORSTORE_INTERNAL_THREAD_POOL_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/thread_pool_test.cc` & `tensorstore-0.1.9/tensorstore/internal/thread_pool_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/type_traits.h` & `tensorstore-0.1.9/tensorstore/internal/type_traits.h`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,31 @@
 /// possibly-empty type (e.g. a function object), and wishes to permit `nullptr`
 /// to be specified if the type is in fact empty.
 template <typename T>
 using PossiblyEmptyObjectGetter =
     absl::conditional_t<std::is_empty<T>::value, EmptyObject<T>,
                         NonEmptyObjectGetter>;
 
+template <typename T>
+struct DefaultConstructibleFunction {
+  constexpr DefaultConstructibleFunction() = default;
+  constexpr DefaultConstructibleFunction(const T&) {}
+  template <typename... Arg>
+  constexpr std::invoke_result_t<T&, Arg...> operator()(Arg&&... arg) const {
+    EmptyObject<T> obj;
+    return obj.get()(static_cast<Arg&&>(arg)...);
+  }
+};
+
+template <typename T>
+using DefaultConstructibleFunctionIfEmpty =
+    std::conditional_t<(std::is_empty_v<T> &&
+                        !std::is_default_constructible_v<T>),
+                       DefaultConstructibleFunction<T>, T>;
+
 /// Identity metafunction for types, as added in C++20.
 ///
 /// See https://en.cppreference.com/w/cpp/types/type_identity
 ///
 /// This is useful for preventing deduction of a function parameter.
 template <typename T>
 struct type_identity {
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/type_traits_test.cc` & `tensorstore-0.1.9/tensorstore/internal/type_traits_test.cc`

 * *Files 12% similar despite different names*

```diff
@@ -197,8 +197,17 @@
 static_assert(IsPairOnlyExplicitlyConvertible<int, double*, X, Y>::value, "");
 static_assert(IsPairOnlyExplicitlyConvertible<float*, int*, X, Y>::value, "");
 static_assert(IsPairOnlyExplicitlyConvertible<float*, double*, X, Y>::value,
               "");
 
 }  // namespace explict_conversion_tests
 
+TEST(DefaultConstructibleFunctionIfEmptyTest, Basic) {
+  auto fn = [](int x) { return x + 1; };
+  using Wrapper =
+      tensorstore::internal::DefaultConstructibleFunctionIfEmpty<decltype(fn)>;
+  static_assert(std::is_default_constructible_v<Wrapper>);
+  EXPECT_EQ(4, Wrapper()(3));
+  EXPECT_EQ(4, Wrapper(fn)(3));
+}
+
 }  // namespace
```

### Comparing `tensorstore-0.1.8/tensorstore/internal/unique_with_intrusive_allocator.h` & `tensorstore-0.1.9/tensorstore/internal/unique_with_intrusive_allocator.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/unique_with_intrusive_allocator_test.cc` & `tensorstore-0.1.9/tensorstore/internal/unique_with_intrusive_allocator_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/unowned_to_shared.h` & `tensorstore-0.1.9/tensorstore/internal/unowned_to_shared.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/utf8.cc` & `tensorstore-0.1.9/tensorstore/internal/utf8.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/utf8.h` & `tensorstore-0.1.9/tensorstore/internal/utf8.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/utf8_test.cc` & `tensorstore-0.1.9/tensorstore/internal/utf8_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/void_wrapper.h` & `tensorstore-0.1.9/tensorstore/internal/void_wrapper.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/internal/void_wrapper_test.cc` & `tensorstore-0.1.9/tensorstore/internal/void_wrapper_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/json_serialization_options.h` & `tensorstore-0.1.9/tensorstore/json_serialization_options.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/BUILD` & `tensorstore-0.1.9/tensorstore/kvstore/BUILD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 load("@bazel_skylib//rules:common_settings.bzl", "bool_flag")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+    data = [
+        "//tensorstore/kvstore/file:doc_sources",
+        "//tensorstore/kvstore/gcs:doc_sources",
+        "//tensorstore/kvstore/memory:doc_sources",
+    ],
+)
+
 tensorstore_cc_library(
     name = "byte_range",
     srcs = ["byte_range.cc"],
     hdrs = ["byte_range.h"],
     deps = [
         "//tensorstore/util:result",
         "//tensorstore/util:status",
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/byte_range.cc` & `tensorstore-0.1.9/tensorstore/kvstore/byte_range.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/byte_range.h` & `tensorstore-0.1.9/tensorstore/kvstore/byte_range.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/byte_range_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/byte_range_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/BUILD` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/BUILD`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,108 @@
-# Filesystem-backed KeyValueStore driver
-
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
-package(default_visibility = ["//visibility:public"])
+package(
+    default_visibility = ["//visibility:public"],
+)
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
-    name = "file",
-    srcs = ["file_key_value_store.cc"],
+    name = "gcs",
+    srcs = [
+        "gcs_key_value_store.cc",
+        "object_metadata.cc",
+    ],
+    hdrs = ["object_metadata.h"],
     deps = [
-        ":file_util",
         "//tensorstore:context",
-        "//tensorstore/internal:file_io_concurrency_resource",
-        "//tensorstore/internal:flat_cord_builder",
+        "//tensorstore/internal:concurrency_resource",
+        "//tensorstore/internal:intrusive_ptr",
         "//tensorstore/internal:json",
-        "//tensorstore/internal:os_error_code",
         "//tensorstore/internal:path",
+        "//tensorstore/internal:retry",
+        "//tensorstore/internal/http",
+        "//tensorstore/internal/http:curl_handle",
+        "//tensorstore/internal/http:curl_transport",
+        "//tensorstore/internal/oauth2",
+        "//tensorstore/internal/oauth2:google_auth_provider",
         "//tensorstore/kvstore:byte_range",
         "//tensorstore/kvstore:generation",
         "//tensorstore/kvstore:key_value_store",
         "//tensorstore/util:execution",
         "//tensorstore/util:executor",
-        "//tensorstore/util:function_view",
         "//tensorstore/util:future",
         "//tensorstore/util:quote_string",
         "//tensorstore/util:result",
         "//tensorstore/util:status",
         "//tensorstore/util:str_cat",
         "@com_github_nlohmann_json//:nlohmann_json",
-        "@com_google_absl//absl/base:core_headers",
         "@com_google_absl//absl/status",
         "@com_google_absl//absl/strings",
+        "@com_google_absl//absl/synchronization",
         "@com_google_absl//absl/time",
-        "@com_google_absl//absl/utility",
+        "@com_google_absl//absl/types:optional",
     ],
     alwayslink = 1,
 )
 
 tensorstore_cc_test(
-    name = "file_key_value_store_test",
+    name = "gcs_key_value_store_test",
     size = "small",
-    srcs = ["file_key_value_store_test.cc"],
+    srcs = [
+        "gcs_key_value_store_test.cc",
+        "gcs_mock.cc",
+        "gcs_mock.h",
+    ],
     deps = [
-        ":file",
+        ":gcs",
         "//tensorstore:context",
-        "//tensorstore/internal:file_io_concurrency_resource",
-        "//tensorstore/internal:test_util",
+        "//tensorstore/internal:intrusive_ptr",
+        "//tensorstore/internal:logging",
+        "//tensorstore/internal:mutex",
+        "//tensorstore/internal:path",
+        "//tensorstore/internal/http",
+        "//tensorstore/internal/http:curl_handle",
+        "//tensorstore/internal/http:curl_transport",
         "//tensorstore/kvstore:generation",
-        "//tensorstore/kvstore:generation_testutil",
         "//tensorstore/kvstore:key_value_store",
         "//tensorstore/kvstore:key_value_store_testutil",
         "//tensorstore/util:execution",
         "//tensorstore/util:executor",
+        "//tensorstore/util:future",
         "//tensorstore/util:sender_testutil",
         "//tensorstore/util:status",
         "//tensorstore/util:status_testutil",
-        "//tensorstore/util:str_cat",
         "@com_github_nlohmann_json//:nlohmann_json",
         "@com_google_absl//absl/status",
+        "@com_google_absl//absl/strings",
+        "@com_google_absl//absl/synchronization",
+        "@com_google_absl//absl/time",
+        "@com_google_absl//absl/types:optional",
+        "@com_google_absl//absl/types:variant",
         "@com_google_googletest//:gtest_main",
     ],
 )
 
-tensorstore_cc_library(
-    name = "file_util",
+tensorstore_cc_test(
+    name = "object_metadata_test",
+    size = "small",
     srcs = [
-        "posix_file_util.cc",
-        "windows_file_util.cc",
-    ],
-    hdrs = [
-        "posix_file_util.h",
-        "unique_handle.h",
-        "windows_file_util.h",
+        "object_metadata_test.cc",
     ],
     deps = [
-        "//tensorstore/internal:os_error_code",
+        ":gcs",
+        "//tensorstore/kvstore:key_value_store_testutil",
         "//tensorstore/util:result",
-        "@com_google_absl//absl/status",
-        "@com_google_absl//absl/strings",
+        "//tensorstore/util:status",
+        "@com_google_absl//absl/time",
+        "@com_google_googletest//:gtest_main",
     ],
 )
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/file_key_value_store.cc` & `tensorstore-0.1.9/tensorstore/kvstore/file/file_key_value_store.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/file_key_value_store_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/file/file_key_value_store_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/index.rst` & `tensorstore-0.1.9/tensorstore/kvstore/file/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/posix_file_util.cc` & `tensorstore-0.1.9/tensorstore/kvstore/file/posix_file_util.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/posix_file_util.h` & `tensorstore-0.1.9/tensorstore/kvstore/file/posix_file_util.h`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 using UniqueFileDescriptor =
     internal::UniqueHandle<FileDescriptor, FileDescriptorTraits>;
 
 /// Returns `true` if `c` is a directory separator character.
 constexpr inline bool IsDirSeparator(char c) { return c == '/'; }
 
 /// Representation of file metadata.
-using FileInfo = struct ::stat;
+typedef struct ::stat FileInfo;
 
 /// Retrieves the metadata for an open file.
 ///
 /// \param fd Open file descriptor.
 /// \param info[out] Non-null pointer to location where metadata will be stored.
 /// \returns `true` on success, `false` on error (in which case
 ///     `GetLastErrorCode()` retrieves the error).
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/schema.yml` & `tensorstore-0.1.9/tensorstore/kvstore/file/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/unique_handle.h` & `tensorstore-0.1.9/tensorstore/kvstore/file/unique_handle.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/windows_file_util.cc` & `tensorstore-0.1.9/tensorstore/kvstore/file/windows_file_util.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/file/windows_file_util.h` & `tensorstore-0.1.9/tensorstore/kvstore/file/windows_file_util.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_key_value_store.cc` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_key_value_store.cc`

 * *Files 1% similar despite different names*

```diff
@@ -429,42 +429,40 @@
 /// GcsKeyValueStore::Read request.
 struct ReadTask {
   GcsKeyValueStore::Ptr owner;
   std::string resource;
   KeyValueStore::ReadOptions options;
 
   Result<KeyValueStore::ReadResult> operator()() {
-    TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
-
     /// Reads contents of a GCS object.
     std::string media_url = StrCat(resource, "?alt=media");
 
     // Add the ifGenerationNotMatch condition.
     AddGenerationParam(&media_url, true, "ifGenerationNotMatch",
                        options.if_not_equal);
     AddGenerationParam(&media_url, true, "ifGenerationMatch", options.if_equal);
 
     // Assume that if the user_project field is set, that we want to provide
     // it on the uri for a requestor pays bucket.
     AddUserProjectParam(&media_url, true, owner->encoded_user_project());
-
-    HttpRequestBuilder request_builder(media_url);
-    if (options.byte_range.inclusive_min != 0 ||
-        options.byte_range.exclusive_max) {
-      request_builder.AddHeader(
-          internal_http::GetRangeHeader(options.byte_range));
-    }
-    auto request = request_builder.EnableAcceptEncoding()
-                       .AddHeader(auth_header)
-                       .BuildRequest();
     KeyValueStore::ReadResult read_result;
 
     // TODO: Configure timeouts.
     HttpResponse httpresponse;
     auto retry_status = owner->RetryRequestWithBackoff([&] {
+      TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
+      HttpRequestBuilder request_builder(media_url);
+      if (options.byte_range.inclusive_min != 0 ||
+          options.byte_range.exclusive_max) {
+        request_builder.AddHeader(
+            internal_http::GetRangeHeader(options.byte_range));
+      }
+      auto request = request_builder.EnableAcceptEncoding()
+                         .AddHeader(auth_header)
+                         .BuildRequest();
       read_result.stamp.time = absl::Now();
       auto response = owner->IssueRequest("ReadTask", request, {});
       if (!response.ok()) return GetStatus(response);
       httpresponse = std::move(*response);
       switch (httpresponse.status_code) {
         // Special status codes handled outside the retry loop.
         case 412:
@@ -534,38 +532,37 @@
   std::string encoded_object_name;
   Value value;
   KeyValueStore::WriteOptions options;
 
   /// Writes an object to GCS.
   Result<TimestampedStorageGeneration> operator()() {
     // We use the SimpleUpload technique.
-    TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
 
     std::string upload_url =
         StrCat(owner->upload_root(), "/o", "?uploadType=media",
                "&name=", encoded_object_name);
 
     // Add the ifGenerationNotMatch condition.
     AddGenerationParam(&upload_url, true, "ifGenerationMatch",
                        options.if_equal);
 
     // Assume that if the user_project field is set, that we want to provide
     // it on the uri for a requestor pays bucket.
     AddUserProjectParam(&upload_url, true, owner->encoded_user_project());
 
-    auto request = HttpRequestBuilder(upload_url)
-                       .AddHeader(auth_header)
-                       .AddHeader("Content-Type: application/octet-stream")
-                       .AddHeader(StrCat("Content-Length: ", value.size()))
-                       .BuildRequest();
-
     TimestampedStorageGeneration r;
 
     HttpResponse httpresponse;
     auto retry_status = owner->RetryRequestWithBackoff([&] {
+      TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
+      auto request = HttpRequestBuilder(upload_url)
+                         .AddHeader(auth_header)
+                         .AddHeader("Content-Type: application/octet-stream")
+                         .AddHeader(StrCat("Content-Length: ", value.size()))
+                         .BuildRequest();
       r.time = absl::Now();
       auto response = owner->IssueRequest("WriteTask", request, value);
       if (!response.ok()) return GetStatus(response);
       httpresponse = std::move(*response);
       switch (httpresponse.status_code) {
         case 304:
           // Not modified implies that the generation did not match.
@@ -619,35 +616,32 @@
 struct DeleteTask {
   GcsKeyValueStore::Ptr owner;
   std::string resource;
   KeyValueStore::WriteOptions options;
 
   /// Writes an object to GCS.
   Result<TimestampedStorageGeneration> operator()() {
-    TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
-
     std::string delete_url = resource;
 
     // Add the ifGenerationNotMatch condition.
     bool has_query = AddGenerationParam(&delete_url, false, "ifGenerationMatch",
                                         options.if_equal);
 
     // Assume that if the user_project field is set, that we want to provide
     // it on the uri for a requestor pays bucket.
     AddUserProjectParam(&delete_url, has_query, owner->encoded_user_project());
-
-    auto request = HttpRequestBuilder(delete_url)
-                       .AddHeader(auth_header)
-                       .SetMethod("DELETE")
-                       .BuildRequest();
-
     TimestampedStorageGeneration r;
 
     HttpResponse httpresponse;
     auto retry_status = owner->RetryRequestWithBackoff([&] {
+      TENSORSTORE_ASSIGN_OR_RETURN(auto auth_header, owner->GetAuthHeader());
+      auto request = HttpRequestBuilder(delete_url)
+                         .AddHeader(auth_header)
+                         .SetMethod("DELETE")
+                         .BuildRequest();
       r.time = absl::Now();
       auto response = owner->IssueRequest("DeleteTask", request, {});
       if (!response.ok()) return GetStatus(response);
       httpresponse = std::move(*response);
       switch (httpresponse.status_code) {
         case 412:
           // Failed precondition implies the generation did not match.
@@ -784,29 +778,28 @@
 
     // The nextPageToken is used to page through the list results.
     std::string nextPageToken;
 
     while (true) {
       TENSORSTORE_RETURN_IF_ERROR(maybe_cancelled());
 
-      TENSORSTORE_ASSIGN_OR_RETURN(auto header, state->owner->GetAuthHeader());
-      TENSORSTORE_RETURN_IF_ERROR(maybe_cancelled());
-
       std::string list_url = base_list_url;
       if (!nextPageToken.empty()) {
         absl::StrAppend(&list_url, (url_has_query ? "&" : "?"),
                         "pageToken=", nextPageToken);
       }
 
-      auto request =
-          HttpRequestBuilder(list_url).AddHeader(header).BuildRequest();
-
       HttpResponse httpresponse;
       auto retry_status = state->owner->RetryRequestWithBackoff([&] {
         TENSORSTORE_RETURN_IF_ERROR(maybe_cancelled());
+        TENSORSTORE_ASSIGN_OR_RETURN(auto header,
+                                     state->owner->GetAuthHeader());
+        TENSORSTORE_RETURN_IF_ERROR(maybe_cancelled());
+        auto request =
+            HttpRequestBuilder(list_url).AddHeader(header).BuildRequest();
         auto response = state->owner->IssueRequest("List", request, {});
         if (!response.ok()) return GetStatus(response);
         httpresponse = std::move(*response);
         return HttpResponseCodeToStatus(httpresponse);
       });
 
       TENSORSTORE_RETURN_IF_ERROR(retry_status);
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_key_value_store_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_key_value_store_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_mock.cc` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_mock.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/gcs_mock.h` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/gcs_mock.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/index.rst` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/index.rst`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata.cc` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata.h` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/object_metadata_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/object_metadata_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/gcs/schema.yml` & `tensorstore-0.1.9/tensorstore/kvstore/gcs/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/generation.cc` & `tensorstore-0.1.9/tensorstore/kvstore/generation.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/generation.h` & `tensorstore-0.1.9/tensorstore/kvstore/generation.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/generation_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/generation_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/generation_testutil.h` & `tensorstore-0.1.9/tensorstore/kvstore/generation_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_range.cc` & `tensorstore-0.1.9/tensorstore/kvstore/key_range.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_range.h` & `tensorstore-0.1.9/tensorstore/kvstore/key_range.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_range_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/key_range_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_value_store.cc` & `tensorstore-0.1.9/tensorstore/kvstore/key_value_store.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_value_store.h` & `tensorstore-0.1.9/tensorstore/kvstore/key_value_store.h`

 * *Files 0% similar despite different names*

```diff
@@ -52,27 +52,27 @@
 /// Example of opening directly:
 ///
 ///     Future<KeyValueStore::Ptr> store =
 ///         KeyValueStore::Open(Context::Default(), {"driver", "memory"});
 ///
 /// Example of opening via `KeyValueStore::Spec`:
 ///
-///     KeyValueStore::Spec spec =
-///         KeyValueStore::Spec::FromJson({"driver", "memory"}).value();
+///     KeyValueStore::Spec::Ptr spec =
+///         KeyValueStore::Spec::Ptr::FromJson({"driver", "memory"}).value();
 ///
-///     Future<KeyValueStore::Ptr> store = spec.Open(Context::Default());
+///     Future<KeyValueStore::Ptr> store = spec->Open(Context::Default());
 ///
 /// Example of opening via `KeyValueStore::Spec` and
 /// `KeyValueStore::BoundSpec::Ptr`:
 ///
-///     KeyValueStore::Spec spec =
-///         KeyValueStore::Spec::FromJson({"driver", "memory"}).value();
+///     KeyValueStore::Spec::Ptr spec =
+///         KeyValueStore::Spec::Ptr::FromJson({"driver", "memory"}).value();
 ///
 ///     KeyValueStore::BoundSpec::Ptr bound_spec =
-///         spec.Bind(Context::Default()).value();
+///         spec->Bind(Context::Default()).value();
 ///
 ///     std::string store_cache_key;
 ///     internal::EncodeCacheKey(&store_cache_key, bound_spec);
 ///
 ///     // Compute derived cache key based on `store_cache_key`.  If already
 ///     // present in cache of opened objects, use existing object and return.
 ///
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_value_store_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/key_value_store_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_value_store_testutil.cc` & `tensorstore-0.1.9/tensorstore/kvstore/key_value_store_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/key_value_store_testutil.h` & `tensorstore-0.1.9/tensorstore/kvstore/key_value_store_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/memory/BUILD` & `tensorstore-0.1.9/tensorstore/kvstore/memory/BUILD`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 load("//tensorstore:tensorstore.bzl", "tensorstore_cc_library", "tensorstore_cc_test")
 
 package(default_visibility = ["//visibility:public"])
 
 licenses(["notice"])
 
+filegroup(
+    name = "doc_sources",
+    srcs = glob([
+        "**/*.rst",
+        "**/*.yml",
+    ]),
+)
+
 tensorstore_cc_library(
     name = "memory",
     srcs = ["memory_key_value_store.cc"],
     hdrs = ["memory_key_value_store.h"],
     deps = [
         "//tensorstore:context",
         "//tensorstore/internal:json",
```

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store.cc` & `tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store.h` & `tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/memory/memory_key_value_store_test.cc` & `tensorstore-0.1.9/tensorstore/kvstore/memory/memory_key_value_store_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/memory/schema.yml` & `tensorstore-0.1.9/tensorstore/kvstore/memory/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/registry.h` & `tensorstore-0.1.9/tensorstore/kvstore/registry.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/schema.yml` & `tensorstore-0.1.9/tensorstore/kvstore/schema.yml`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/transaction.cc` & `tensorstore-0.1.9/tensorstore/kvstore/transaction.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/kvstore/transaction.h` & `tensorstore-0.1.9/tensorstore/kvstore/transaction.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/make_array.inc` & `tensorstore-0.1.9/tensorstore/make_array.inc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/non_compile.bzl` & `tensorstore-0.1.9/tensorstore/non_compile.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/open.cc` & `tensorstore-0.1.9/tensorstore/open.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/open.h` & `tensorstore-0.1.9/tensorstore/open.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/open_mode.cc` & `tensorstore-0.1.9/tensorstore/open_mode.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/open_mode.h` & `tensorstore-0.1.9/tensorstore/open_mode.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/open_mode_test.cc` & `tensorstore-0.1.9/tensorstore/open_mode_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/progress.cc` & `tensorstore-0.1.9/tensorstore/progress.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/progress.h` & `tensorstore-0.1.9/tensorstore/progress.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/progress_test.cc` & `tensorstore-0.1.9/tensorstore/progress_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/rank.cc` & `tensorstore-0.1.9/tensorstore/static_cast.cc`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "tensorstore/rank.h"
+#include "tensorstore/static_cast.h"
 
-#include "tensorstore/util/str_cat.h"
+#include "tensorstore/util/status.h"
 
 namespace tensorstore {
-
-std::string StaticCastTraits<DimensionIndex>::Describe(DimensionIndex value) {
-  if (value == dynamic_rank) return "dynamic rank";
-  return StrCat("rank of ", value);
+namespace internal_cast {
+Status CastError(absl::string_view source_description,
+                 absl::string_view target_description) {
+  return absl::InvalidArgumentError(
+      StrCat("Cannot cast ", source_description, " to ", target_description));
 }
 
+}  // namespace internal_cast
 }  // namespace tensorstore
```

### Comparing `tensorstore-0.1.8/tensorstore/rank.h` & `tensorstore-0.1.9/tensorstore/rank.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,37 @@
 #include "tensorstore/static_cast.h"
 #include "tensorstore/util/assert_macros.h"
 #include "tensorstore/util/result.h"
 #include "tensorstore/util/status.h"
 
 namespace tensorstore {
 
+/// Maximum supported rank.
+constexpr DimensionIndex kMaxRank = 32;
+
+constexpr inline bool IsValidRank(DimensionIndex rank) {
+  return 0 <= rank && rank <= kMaxRank;
+}
+
+constexpr inline bool IsValidRankSpec(DimensionIndex rank_spec) {
+  return rank_spec >= (-kMaxRank - 1) && rank_spec <= kMaxRank;
+}
+
 struct DynamicRank {
   /// Enables the use of `dynamic_rank` below as a constant argument for
   /// `DimensionIndex Rank` template parameters to indicate a dynamic rank (with
   /// inline buffer disabled, if applicable).
   constexpr operator DimensionIndex() const { return -1; }
 
   /// Enables the use of `dynamic_rank(n)` as an argument for
   /// `DimensionIndex Rank` template parameters to indicate a dynamic rank with
   /// an inline buffer of size `n`.
   constexpr DimensionIndex operator()(DimensionIndex inline_buffer_size) const {
     assert(inline_buffer_size >= 0);
+    assert(inline_buffer_size <= kMaxRank);
     return -1 - inline_buffer_size;
   }
 };
 
 /// Special rank value indicating a rank specified at run time.
 ///
 /// The value `dynamic_rank` is implicitly convertible to `DimensionIndex(-1)`,
@@ -67,15 +79,16 @@
 
 constexpr inline DimensionIndex NormalizeRankSpec(DimensionIndex rank_spec) {
   return (rank_spec <= -1) ? -1 : rank_spec;
 }
 
 /// Returns `true` if `rank` is a valid static rank value.
 constexpr inline bool IsValidStaticRank(DimensionIndex static_rank) {
-  return static_rank >= 0 || static_rank == dynamic_rank;
+  return (static_rank >= 0 && static_rank <= kMaxRank) ||
+         static_rank == dynamic_rank;
 }
 
 /// Returns `true` if, and only if, a conversion from `source_rank` to
 /// `dest_rank` is always valid.
 constexpr inline bool IsRankImplicitlyConvertible(DimensionIndex source_rank,
                                                   DimensionIndex dest_rank) {
   return source_rank == dest_rank || dest_rank == dynamic_rank;
@@ -345,10 +358,15 @@
   static std::string Describe(StaticRank<Rank>) { return Describe(); }
   // COV_NF_END
 
   template <DimensionIndex TargetRank>
   using RebindRank = StaticOrDynamicRank<TargetRank>;
 };
 
+/// Validates that `0 <= rank <= kMaxRank`.
+///
+/// \error `absl::StatusCode::kInvalidArgument` if `rank` is not valid.
+absl::Status ValidateRank(DimensionIndex rank);
+
 }  // namespace tensorstore
 
 #endif  // TENSORSTORE_RANK_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/rank_test.cc` & `tensorstore-0.1.9/tensorstore/rank_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/read_write_options.h` & `tensorstore-0.1.9/tensorstore/read_write_options.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/resize_options.cc` & `tensorstore-0.1.9/tensorstore/resize_options.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/resize_options.h` & `tensorstore-0.1.9/tensorstore/resize_options.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/resize_options_test.cc` & `tensorstore-0.1.9/tensorstore/resize_options_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/spec.cc` & `tensorstore-0.1.9/tensorstore/spec.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/spec.h` & `tensorstore-0.1.9/tensorstore/spec.h`

 * *Files 11% similar despite different names*

```diff
@@ -20,28 +20,32 @@
 
 #include <nlohmann/json.hpp>
 #include "tensorstore/data_type.h"
 #include "tensorstore/driver/driver.h"
 #include "tensorstore/index.h"
 #include "tensorstore/index_space/index_transform.h"
 #include "tensorstore/index_space/index_transform_spec.h"
+#include "tensorstore/internal/type_traits.h"
 #include "tensorstore/rank.h"
 #include "tensorstore/spec_impl.h"
 #include "tensorstore/util/result.h"
 
 namespace tensorstore {
 
 /// Specifies the parameters necessary to open or create a TensorStore,
 /// including the driver identifier, driver parameters, and optionally the data
 /// type and a transform or rank constraint.
 class Spec {
  public:
   /// Constructs an invalid specification.
   Spec() = default;
 
+  /// Returns `true` if this is a valid spec.
+  bool valid() const { return static_cast<bool>(impl_.driver_spec); }
+
   /// Returns the data type.
   ///
   /// If the data type is unknown, returns the invalid data type.
   DataType data_type() const {
     return impl_.driver_spec ? impl_.driver_spec->constraints().data_type
                              : DataType();
   }
@@ -70,29 +74,38 @@
   /// This definition allows DimExpression objects to be applied to Spec
   /// objects.
   ///
   /// \returns The transformed `Spec` on success.
   /// \error `absl::StatusCode::kInvalidArgument` if `spec.transform()` is not
   ///     valid.
   template <typename Expr>
-  friend Result<Spec> ApplyIndexTransform(Expr&& expr, Spec spec) {
+  friend internal::FirstType<
+      Result<Spec>,
+      decltype(ApplyIndexTransform(std::declval<Expr>(),
+                                   std::declval<IndexTransformSpec>()))>
+  ApplyIndexTransform(Expr&& expr, Spec spec) {
     TENSORSTORE_ASSIGN_OR_RETURN(
         spec.impl_.transform_spec,
         ApplyIndexTransform(std::forward<Expr>(expr),
                             std::move(spec.impl_.transform_spec)));
     return spec;
   }
 
   friend std::ostream& operator<<(std::ostream& os, const Spec& spec);
 
   /// Compares for equality via JSON representation.
   friend bool operator==(const Spec& a, const Spec& b);
 
   friend bool operator!=(const Spec& a, const Spec& b) { return !(a == b); }
 
+  template <typename Func>
+  friend PipelineResultType<Spec, Func> operator|(Spec spec, Func&& func) {
+    return std::forward<Func>(func)(std::move(spec));
+  }
+
  private:
   friend class internal_spec::SpecAccess;
   internal::TransformedDriverSpec<> impl_;
 };
 
 /// Returns an error if `rank_constraint` is not compatible with `actual_rank`.
 ///
```

### Comparing `tensorstore-0.1.8/tensorstore/spec_impl.h` & `tensorstore-0.1.9/tensorstore/spec_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/spec_request_options.h` & `tensorstore-0.1.9/tensorstore/spec_request_options.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/spec_test.cc` & `tensorstore-0.1.9/tensorstore/spec_test.cc`

 * *Files 13% similar despite different names*

```diff
@@ -38,22 +38,28 @@
 using tensorstore::MatchesStatus;
 using tensorstore::Result;
 using tensorstore::Spec;
 using tensorstore::StaticDataType;
 using tensorstore::StaticRankCast;
 using tensorstore::StrCat;
 
+TEST(SpecTest, Invalid) {
+  Spec spec;
+  EXPECT_FALSE(spec.valid());
+}
+
 TEST(SpecTest, ToJson) {
   ::nlohmann::json spec_json({{"driver", "array"},
                               {"dtype", "int32"},
                               {"array", {1, 2, 3}},
                               {"rank", 1}});
   Spec spec =
       Spec::FromJson(spec_json, tensorstore::AllowUnregistered{true}).value();
   EXPECT_THAT(spec.ToJson(), ::testing::Optional(spec_json));
+  EXPECT_TRUE(spec.valid());
 }
 
 TEST(SpecTest, Comparison) {
   Spec spec_a = Spec::FromJson({{"driver", "array"},
                                 {"dtype", "int32"},
                                 {"array", {1, 2, 3}},
                                 {"rank", 1}},
@@ -87,52 +93,92 @@
                               {"output",
                                {{{"input_dimension", 0}, {"offset", -2}},
                                 {{"input_dimension", 1}, {"offset", -4}}}}}}}),
           tensorstore::AllowUnregistered{true})
           .value();
   EXPECT_EQ(2, spec_with_transform.rank());
   EXPECT_THAT(
-      ChainResult(Spec::FromJson(
-                      ::nlohmann::json(
-                          {{"driver", "array"},
-                           {"dtype", "int32"},
-                           {"array",
-                            {
-                                {1, 2, 3, 4},
-                                {5, 6, 7, 8},
-                                {9, 10, 11, 12},
-                            }},
-                           {"transform",
-                            {{"input_inclusive_min", {2, 4}},
-                             {"input_shape", {3, 4}},
-                             {"output",
-                              {{{"input_dimension", 0}, {"offset", -2}},
-                               {{"input_dimension", 1}, {"offset", -4}}}}}}}),
-                      tensorstore::AllowUnregistered{true}),
-                  tensorstore::Dims(1).SizedInterval(4, 2)),
+      Spec::FromJson(
+          ::nlohmann::json({{"driver", "array"},
+                            {"dtype", "int32"},
+                            {"array",
+                             {
+                                 {1, 2, 3, 4},
+                                 {5, 6, 7, 8},
+                                 {9, 10, 11, 12},
+                             }},
+                            {"transform",
+                             {{"input_inclusive_min", {2, 4}},
+                              {"input_shape", {3, 4}},
+                              {"output",
+                               {{{"input_dimension", 0}, {"offset", -2}},
+                                {{"input_dimension", 1}, {"offset", -4}}}}}}}),
+          tensorstore::AllowUnregistered{true}) |
+          tensorstore::Dims(1).SizedInterval(4, 2),
       ::testing::Optional(spec_with_transform));
 
   // Tests applying a DimExpression to a Spec with unknown rank (fails).
   Spec spec_without_transform =
       Spec::FromJson(::nlohmann::json({{"driver", "array"},
                                        {"dtype", "int32"},
                                        {"array",
                                         {
                                             {1, 2, 3, 4},
                                             {5, 6, 7, 8},
                                             {9, 10, 11, 12},
                                         }}}),
                      tensorstore::AllowUnregistered{true})
           .value();
-  EXPECT_THAT(ChainResult(spec_without_transform,
-                          tensorstore::Dims(1).SizedInterval(4, 2)),
+  EXPECT_THAT(spec_without_transform | tensorstore::Dims(1).SizedInterval(4, 2),
               MatchesStatus(absl::StatusCode::kInvalidArgument,
                             "Transform is unspecified"));
 }
 
+TEST(SpecTest, ApplyBox) {
+  // Tests successfully applying a Box to a Spec.
+  TENSORSTORE_ASSERT_OK_AND_ASSIGN(
+      auto spec_with_transform,
+      Spec::FromJson(
+          ::nlohmann::json({{"driver", "array"},
+                            {"dtype", "int32"},
+                            {"array",
+                             {
+                                 {1, 2, 3, 4},
+                                 {5, 6, 7, 8},
+                                 {9, 10, 11, 12},
+                             }},
+                            {"transform",
+                             {{"input_inclusive_min", {3, 4}},
+                              {"input_shape", {2, 2}},
+                              {"output",
+                               {{{"input_dimension", 0}, {"offset", -2}},
+                                {{"input_dimension", 1}, {"offset", -4}}}}}}}),
+          tensorstore::AllowUnregistered{true}));
+  EXPECT_EQ(2, spec_with_transform.rank());
+  EXPECT_THAT(
+      Spec::FromJson(
+          ::nlohmann::json({{"driver", "array"},
+                            {"dtype", "int32"},
+                            {"array",
+                             {
+                                 {1, 2, 3, 4},
+                                 {5, 6, 7, 8},
+                                 {9, 10, 11, 12},
+                             }},
+                            {"transform",
+                             {{"input_inclusive_min", {2, 4}},
+                              {"input_shape", {3, 4}},
+                              {"output",
+                               {{{"input_dimension", 0}, {"offset", -2}},
+                                {{"input_dimension", 1}, {"offset", -4}}}}}}}),
+          tensorstore::AllowUnregistered{true}) |
+          tensorstore::Box({3, 4}, {2, 2}),
+      ::testing::Optional(spec_with_transform));
+}
+
 TEST(SpecTest, PrintToOstream) {
   ::nlohmann::json spec_json({{"driver", "array"},
                               {"dtype", "int32"},
                               {"array", {1, 2, 3}},
                               {"rank", 1}});
   Spec spec =
       Spec::FromJson(spec_json, tensorstore::AllowUnregistered{true}).value();
```

### Comparing `tensorstore-0.1.8/tensorstore/staleness_bound.h` & `tensorstore-0.1.9/tensorstore/staleness_bound.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/static_cast.cc` & `tensorstore-0.1.9/tensorstore/util/span_json.h`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "tensorstore/static_cast.h"
+#ifndef TENSORSTORE_UTIL_SPAN_JSON_H_
+#define TENSORSTORE_UTIL_SPAN_JSON_H_
 
-#include "tensorstore/util/status.h"
+#include <nlohmann/json.hpp>
+#include "tensorstore/util/span.h"
 
 namespace tensorstore {
-namespace internal_cast {
-Status CastError(absl::string_view source_description,
-                 absl::string_view target_description) {
-  return absl::InvalidArgumentError(
-      StrCat("Cannot cast ", source_description, " to ", target_description));
+
+/// Converts a `span` to a JSON array.
+template <typename T, std::ptrdiff_t Extent>
+void to_json(::nlohmann::json& out,  // NOLINT
+             span<T, Extent> s) {
+  out = ::nlohmann::json::array_t(s.begin(), s.end());
 }
 
-}  // namespace internal_cast
 }  // namespace tensorstore
+
+#endif  // TENSORSTORE_UTIL_SPAN_JSON_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/static_cast.h` & `tensorstore-0.1.9/tensorstore/static_cast.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/static_cast_test.cc` & `tensorstore-0.1.9/tensorstore/static_cast_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/strided_layout.cc` & `tensorstore-0.1.9/tensorstore/strided_layout.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/strided_layout.h` & `tensorstore-0.1.9/tensorstore/strided_layout.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,26 @@
 #include <string>
 #include <type_traits>
 #include <utility>
 
 #include "tensorstore/box.h"
 #include "tensorstore/container_kind.h"
 #include "tensorstore/contiguous_layout.h"
+#include "tensorstore/internal/gdb_scripting.h"
 #include "tensorstore/internal/multi_vector.h"
 #include "tensorstore/internal/multi_vector_view.h"
 #include "tensorstore/internal/type_traits.h"
 #include "tensorstore/rank.h"
 #include "tensorstore/util/assert_macros.h"
 #include "tensorstore/util/constant_vector.h"
 #include "tensorstore/util/extents.h"
 #include "tensorstore/util/span.h"
 
+TENSORSTORE_GDB_AUTO_SCRIPT("multi_vector_gdb.py")
+
 namespace tensorstore {
 
 /// Specifies whether array indices start at zero, or at an arbitrary origin
 /// vector.
 enum class ArrayOriginKind { zero, offset };
 
 constexpr ArrayOriginKind zero_origin = ArrayOriginKind::zero;
@@ -349,14 +352,15 @@
 /// \tparam CKind Either `container` (for value semantics) or `view` (for
 ///     unowned view semantics).
 template <DimensionIndex Rank, ArrayOriginKind OriginKind, ContainerKind CKind>
 class StridedLayout
     : public internal_strided_layout::LayoutStorageSelector<Rank, OriginKind,
                                                             CKind>::Storage {
  private:
+  static_assert(IsValidRankSpec(Rank));
   using Selector =
       internal_strided_layout::LayoutStorageSelector<Rank, OriginKind, CKind>;
   using Storage = typename Selector::Storage;
   using Access = typename Selector::Access;
 
  public:
   constexpr static ArrayOriginKind array_origin_kind = OriginKind;
```

### Comparing `tensorstore-0.1.8/tensorstore/strided_layout_test.cc` & `tensorstore-0.1.9/tensorstore/strided_layout_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/tensorstore.bzl` & `tensorstore-0.1.9/tensorstore/tensorstore.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/tensorstore.cc` & `tensorstore-0.1.9/tensorstore/tensorstore.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/tensorstore.h` & `tensorstore-0.1.9/tensorstore/tensorstore.h`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 ///     `ReadWriteMode::dynamic` to indicate that the read-write mode is
 ///     determined at run time.
 template <typename ElementType = void, DimensionIndex Rank = dynamic_rank,
           ReadWriteMode Mode = ReadWriteMode::dynamic>
 class TensorStore {
   static_assert(std::is_same_v<ElementType, std::decay_t<ElementType>>,
                 "Invalid ElementType.");
+  static_assert(IsValidStaticRank(Rank));
   using Access = internal::TensorStoreAccess;
   using Transform = IndexTransform<Rank>;
 
  public:
   using Element = ElementType;
   using DataType = StaticOrDynamicDataTypeOf<Element>;
   using RankType = StaticOrDynamicRank<Rank>;
@@ -173,32 +174,35 @@
   /// In the expression  `x | y`, if
   ///   * y is a function having signature `Result<U>(T)`
   ///
   /// Then operator| applies y to the value of x, returning a
   /// Result<U>. See tensorstore::Result operator| for examples.
   template <typename Func>
   PipelineResultType<const TensorStore&, Func> operator|(Func&& func) const& {
-    return static_cast<Func&&>(func)(*this);
+    return std::forward<Func>(func)(*this);
   }
   template <typename Func>
   PipelineResultType<TensorStore&&, Func> operator|(Func&& func) && {
-    return static_cast<Func&&>(func)(std::move(*this));
+    return std::forward<Func>(func)(std::move(*this));
   }
 
  private:
   friend class internal::TensorStoreAccess;
 
   /// Applies a function that operates on an IndexTransform to a TensorStore.
   ///
   /// This definition allows DimExpression objects to be applied to TensorStore
   /// objects.
   template <typename Expr>
   friend Result<TensorStore<Element,
-                            UnwrapResultType<std::invoke_result_t<
-                                Expr, Transform>>::static_input_rank,
+                            // Note: Use `decltype` directly rather than
+                            // `std::invoke_result_t` to avoid recursive alias
+                            // definition error on MSVC 2019.
+                            UnwrapResultType<decltype(std::declval<Expr>()(
+                                std::declval<Transform>()))>::static_input_rank,
                             Mode>>
   ApplyIndexTransform(Expr&& expr, TensorStore store) {
     TENSORSTORE_ASSIGN_OR_RETURN(
         auto new_transform, expr(tensorstore::StaticRankCast<Rank, unchecked>(
                                 std::move(store.handle_.transform))));
     store.handle_.transform = std::move(new_transform);
     return internal::TensorStoreAccess::Construct<
```

### Comparing `tensorstore-0.1.8/tensorstore/tensorstore_impl.h` & `tensorstore-0.1.9/tensorstore/tensorstore_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/transaction.cc` & `tensorstore-0.1.9/tensorstore/transaction.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/transaction.h` & `tensorstore-0.1.9/tensorstore/transaction.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/transaction_impl.h` & `tensorstore-0.1.9/tensorstore/transaction_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/transaction_test.cc` & `tensorstore-0.1.9/tensorstore/transaction_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/update_generated_source_code.py` & `tensorstore-0.1.9/tensorstore/update_generated_source_code.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/BUILD` & `tensorstore-0.1.9/tensorstore/util/BUILD`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/assert_macros.h` & `tensorstore-0.1.9/tensorstore/util/assert_macros.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/assert_macros_test.cc` & `tensorstore-0.1.9/tensorstore/util/assert_macros_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_span.h` & `tensorstore-0.1.9/tensorstore/util/bit_span.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_span_test.cc` & `tensorstore-0.1.9/tensorstore/util/bit_span_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_vec.h` & `tensorstore-0.1.9/tensorstore/util/bit_vec.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_vec_impl.cc` & `tensorstore-0.1.9/tensorstore/util/bit_vec_impl.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_vec_impl.h` & `tensorstore-0.1.9/tensorstore/util/bit_vec_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/bit_vec_test.cc` & `tensorstore-0.1.9/tensorstore/util/bit_vec_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/byte_strided_pointer.h` & `tensorstore-0.1.9/tensorstore/util/byte_strided_pointer.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/byte_strided_pointer_test.cc` & `tensorstore-0.1.9/tensorstore/util/byte_strided_pointer_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/collecting_sender.h` & `tensorstore-0.1.9/tensorstore/util/collecting_sender.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/collecting_sender_test.cc` & `tensorstore-0.1.9/tensorstore/util/collecting_sender_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/constant_bit_vector.h` & `tensorstore-0.1.9/tensorstore/util/constant_bit_vector.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/constant_bit_vector_test.cc` & `tensorstore-0.1.9/tensorstore/util/constant_bit_vector_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/constant_vector.cc` & `tensorstore-0.1.9/tensorstore/util/constant_vector.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/constant_vector.h` & `tensorstore-0.1.9/tensorstore/util/constant_vector.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/constant_vector_test.cc` & `tensorstore-0.1.9/tensorstore/util/constant_vector_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/default_iteration_result.h` & `tensorstore-0.1.9/tensorstore/util/default_iteration_result.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/default_iteration_result_test.cc` & `tensorstore-0.1.9/tensorstore/util/default_iteration_result_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/division.h` & `tensorstore-0.1.9/tensorstore/util/division.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/division_test.cc` & `tensorstore-0.1.9/tensorstore/util/division_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/element_pointer.cc` & `tensorstore-0.1.9/tensorstore/util/element_pointer.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/element_pointer.h` & `tensorstore-0.1.9/tensorstore/util/element_pointer.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/element_pointer_test.cc` & `tensorstore-0.1.9/tensorstore/util/element_pointer_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/element_traits.h` & `tensorstore-0.1.9/tensorstore/util/element_traits.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/element_traits_test.cc` & `tensorstore-0.1.9/tensorstore/util/element_traits_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/endian.h` & `tensorstore-0.1.9/tensorstore/util/endian.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/execution.h` & `tensorstore-0.1.9/tensorstore/util/execution.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/executor.h` & `tensorstore-0.1.9/tensorstore/util/executor.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/executor_test.cc` & `tensorstore-0.1.9/tensorstore/util/executor_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/extents.h` & `tensorstore-0.1.9/tensorstore/util/extents.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/extents_test.cc` & `tensorstore-0.1.9/tensorstore/util/extents_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/function_view.h` & `tensorstore-0.1.9/tensorstore/util/function_view.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/function_view_test.cc` & `tensorstore-0.1.9/tensorstore/util/function_view_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/future.cc` & `tensorstore-0.1.9/tensorstore/util/future.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/future.h` & `tensorstore-0.1.9/tensorstore/util/future.h`

 * *Files 1% similar despite different names*

```diff
@@ -171,19 +171,31 @@
 template <typename T>
 class [[nodiscard]] Promise;
 template <typename T>
 class [[nodiscard]] PromiseFuturePair;
 template <typename T>
 class [[nodiscard]] ReadyFuture;
 
+template <typename T>
+constexpr inline bool IsFuture = false;
+
+template <typename T>
+constexpr inline bool IsFuture<Future<T>> = true;
+template <typename T>
+constexpr inline bool IsFuture<ReadyFuture<T>> = true;
+
 /// Bool-valued metafunction equal to `true` if, and only if, `Future<SourceT>`
 /// is convertible to `Future<DestT>`.
 template <typename SourceT, typename DestT>
 using IsFutureConvertible = internal::IsConstConvertible<SourceT, DestT>;
 
+/// Alias that maps `Future<T> -> T`, `Result<T> -> T`, or otherwise `T -> T`.
+template <typename T>
+using UnwrapFutureType = typename internal_future::UnwrapFutureHelper<T>::type;
+
 /// Handle to a registered Future or Promise callback, that may be used to
 /// unregister it.
 ///
 /// This type has shared weak ownership semantics, and may be copied to create
 /// an equivalent handle, either of which may be used to unregister the
 /// callback.
 ///
@@ -681,14 +693,19 @@
   constexpr SharedState& rep() const {
     ABSL_ASSERT(rep_);
     return static_cast<SharedState&>(*rep_);
   }
   internal_future::FutureStatePointer rep_;
 };
 
+template <typename T>
+Future(Result<T>&& result) -> Future<T>;
+template <typename T>
+Future(const Result<T>& result) -> Future<T>;
+
 /// Returns `true` if both futures refer to the same shared state, or are both
 /// invalid.
 template <typename T, typename U>
 inline bool HaveSameSharedState(const Future<T>& a, const Future<U>& b) {
   return internal_future::FutureAccess::rep_pointer(a).get() ==
          internal_future::FutureAccess::rep_pointer(b).get();
 }
@@ -1017,29 +1034,33 @@
 /// \param executor Executor with which to invoke the `callback` callback.
 /// \param callback Callback function to be invoked as
 ///     `callback(future.result()...)` when all of the `future` objects become
 ///     ready.  The callback is invoked immediately if all of the `future`
 ///     objects are already ready.
 /// \param future The `Future` objects to link.
 /// \dchecks `future.valid() && ...`
-/// \returns A `Future<UnwrapResultType<remove_cvref_t<U>>>`, where `U` is the
+/// \returns A `Future<UnwrapFutureType<remove_cvref_t<U>>>`, where `U` is the
 ///     return type of the specified `callback` function.
 template <typename Executor, typename Callback, typename... FutureValue>
-Future<UnwrapResultType<internal::remove_cvref_t<std::invoke_result_t<
+Future<UnwrapFutureType<internal::remove_cvref_t<std::invoke_result_t<
     Callback, internal_future::ResultType<FutureValue>&...>>>>
 MapFuture(Executor&& executor, Callback&& callback,
           Future<FutureValue>... future) {
-  using PromiseValue =
-      UnwrapResultType<internal::remove_cvref_t<std::invoke_result_t<
-          Callback, internal_future::ResultType<FutureValue>&...>>>;
+  using R = internal::remove_cvref_t<std::invoke_result_t<
+      Callback, internal_future::ResultType<FutureValue>&...>>;
+  using PromiseValue = UnwrapResultType<UnwrapFutureType<R>>;
   struct SetPromiseFromCallback {
     internal::remove_cvref_t<Callback> callback;
     void operator()(Promise<PromiseValue> promise,
                     Future<FutureValue>... future) {
-      promise.SetResult(callback(future.result()...));
+      if constexpr (IsFuture<R>) {
+        Link(std::move(promise), callback(future.result()...));
+      } else {
+        promise.SetResult(callback(future.result()...));
+      }
     }
   };
   return PromiseFuturePair<PromiseValue>::Link(
              WithExecutor(
                  std::forward<Executor>(executor),
                  SetPromiseFromCallback{std::forward<Callback>(callback)}),
              std::move(future)...)
@@ -1063,28 +1084,33 @@
 ///
 /// \param executor Executor with which to invoke the `callback` callback.
 /// \param callback Callback function to be invoked as
 ///     `callback(future.result().value()...)` when all of the `future` objects
 ///     become ready with non-error results.
 /// \param future The `Future` objects to link.
 /// \dchecks `future.valid() && ...`
-/// \returns A `Future<UnwrapResultType<remove_cvref_t<U>>>`, where `U` is the
+/// \returns A `Future<UnwrapFutureType<remove_cvref_t<U>>>`, where `U` is the
 ///     return type of the specified `callback` function.
 template <typename Executor, typename Callback, typename... FutureValue>
-Future<UnwrapResultType<
+Future<UnwrapFutureType<
     internal::remove_cvref_t<std::invoke_result_t<Callback, FutureValue&...>>>>
 MapFutureValue(Executor&& executor, Callback&& callback,
                Future<FutureValue>... future) {
-  using PromiseValue = UnwrapResultType<internal::remove_cvref_t<
-      std::invoke_result_t<Callback, FutureValue&...>>>;
+  using R =
+      internal::remove_cvref_t<std::invoke_result_t<Callback, FutureValue&...>>;
+  using PromiseValue = UnwrapFutureType<R>;
   struct SetPromiseFromCallback {
     internal::remove_cvref_t<Callback> callback;
     void operator()(Promise<PromiseValue> promise,
                     Future<FutureValue>... future) {
-      promise.SetResult(callback(future.result().value()...));
+      if constexpr (IsFuture<R>) {
+        Link(std::move(promise), callback(future.result().value()...));
+      } else {
+        promise.SetResult(callback(future.result().value()...));
+      }
     }
   };
   return PromiseFuturePair<PromiseValue>::LinkValue(
              WithExecutor(
                  std::forward<Executor>(executor),
                  SetPromiseFromCallback{std::forward<Callback>(callback)}),
              std::move(future)...)
```

### Comparing `tensorstore-0.1.8/tensorstore/util/future_impl.h` & `tensorstore-0.1.9/tensorstore/util/future_impl.h`

 * *Files 2% similar despite different names*

```diff
@@ -673,16 +673,15 @@
 /// \tparam I Unique identifier within the FutureLink.
 template <typename LinkType, typename T, std::size_t I>
 class FutureLinkReadyCallback : public ReadyCallbackBase {
  public:
   using SharedState = FutureStateType<T>;
 
   explicit FutureLinkReadyCallback(FutureStateBase* shared_state)
-      : ReadyCallbackBase(shared_state) {
-  }
+      : ReadyCallbackBase(shared_state) {}
 
   void OnReady() noexcept override {
     GetParent()->OnFutureReady(shared_state());
   }
   void OnUnregistered() noexcept override { GetParent()->EnsureCancelled(); }
   void DestroyCallback() noexcept override {
     GetParent()->MarkLinkCallbackDestroyed(/*promise=*/false);
@@ -1444,11 +1443,32 @@
     std::forward<Callback>(callback)(
         FutureAccess::Construct<Promise<PromiseValue>>(
             PromiseStatePointer(state)));
     return state;
   }
 };
 
+template <typename T>
+struct UnwrapFutureHelper {
+  using type = std::remove_cv_t<T>;
+};
+
+template <typename T>
+struct UnwrapFutureHelper<Future<T>> {
+  using type = std::remove_cv_t<T>;
+};
+
+template <typename T>
+struct UnwrapFutureHelper<ReadyFuture<T>> {
+  using type = std::remove_cv_t<T>;
+};
+
+template <typename T>
+struct UnwrapFutureHelper<Result<T>> {
+  // Result<T> requires `T` to be unqualified.
+  using type = T;
+};
+
 }  // namespace internal_future
 }  // namespace tensorstore
 
 #endif  // TENSORSTORE_UTIL_FUTURE_IMPL_H_
```

### Comparing `tensorstore-0.1.8/tensorstore/util/future_sender_test.cc` & `tensorstore-0.1.9/tensorstore/util/future_sender_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/future_test.cc` & `tensorstore-0.1.9/tensorstore/util/future_test.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1532,14 +1532,22 @@
         return 7;
       },
       a);
   EXPECT_EQ(7, b.value());
   EXPECT_EQ(10, a.value());
 }
 
+TEST(MapFutureTest, ReturnFuture) {
+  Future<int> a = 5;
+  auto f = MapFuture(
+      InlineExecutor{},
+      [](Result<int> a) -> Future<int> { return a.value() + 3; }, a);
+  EXPECT_THAT(f.result(), ::testing::Optional(8));
+}
+
 TEST(MapFutureValueTest, BothReady) {
   auto a = MakeReadyFuture<int>(3);
   auto b = MakeReadyFuture<int>(5);
   auto c = MapFutureValue(InlineExecutor{}, std::plus<int>{}, a, b);
   EXPECT_EQ(8, c.result().value());
 }
 
@@ -1565,14 +1573,21 @@
         return absl::UnknownError(tensorstore::StrCat("Got value: ", x));
       },
       a);
   EXPECT_THAT(b.result(),
               MatchesStatus(absl::StatusCode::kUnknown, "Got value: 3"));
 }
 
+TEST(MapFutureValueTest, ReturnFuture) {
+  Future<int> a = 5;
+  auto f = MapFutureValue(
+      InlineExecutor{}, [](int a) -> Future<int> { return a + 3; }, a);
+  EXPECT_THAT(f.result(), ::testing::Optional(8));
+}
+
 TEST(MapFutureErrorTest, Success) {
   auto pair = PromiseFuturePair<int>::Make();
   auto mapped = MapFutureError(
       InlineExecutor{}, [](Status status) { return 5; }, pair.future);
   EXPECT_FALSE(mapped.ready());
   pair.promise.SetResult(7);
   EXPECT_EQ(7, mapped.result());
```

### Comparing `tensorstore-0.1.8/tensorstore/util/internal/iterate.h` & `tensorstore-0.1.9/tensorstore/util/internal/iterate.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/internal/iterate_impl.h` & `tensorstore-0.1.9/tensorstore/util/internal/iterate_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/iterate.cc` & `tensorstore-0.1.9/tensorstore/util/iterate.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/iterate.h` & `tensorstore-0.1.9/tensorstore/util/iterate.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/iterate_over_index_range.h` & `tensorstore-0.1.9/tensorstore/util/iterate_over_index_range.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/iterate_over_index_range_test.cc` & `tensorstore-0.1.9/tensorstore/util/iterate_over_index_range_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/iterate_test.cc` & `tensorstore-0.1.9/tensorstore/util/iterate_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/quote_string.cc` & `tensorstore-0.1.9/tensorstore/util/quote_string.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/quote_string.h` & `tensorstore-0.1.9/tensorstore/util/quote_string.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/quote_string_test.cc` & `tensorstore-0.1.9/tensorstore/util/quote_string_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/result.h` & `tensorstore-0.1.9/tensorstore/util/result.h`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
   /// \brief Construct a Result<T> with an error status.
   /// \requires `!status`
   Result(const Status& status) : storage(internal_result::status_t(), status) {
     TENSORSTORE_CHECK(!status.ok());
   }
   Result(Status&& status)
       : storage(internal_result::status_t(), std::move(status)) {
-    TENSORSTORE_CHECK(!status.ok());
+    TENSORSTORE_CHECK(!this->status_.ok());
   }
 
   /// \brief Constructs a non-empty `Result` direct-initialized value of type
   /// `T` from the arguments `std::forward<Args>(args)...`  within the `Result`.
   template <typename... Args>
   Result(in_place_t, Args&&... args)
       : storage(internal_result::value_t(), std::forward<Args>(args)...) {}
```

### Comparing `tensorstore-0.1.8/tensorstore/util/result_impl.h` & `tensorstore-0.1.9/tensorstore/util/result_impl.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/result_nc_test.cc` & `tensorstore-0.1.9/tensorstore/util/result_nc_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/result_sender_test.cc` & `tensorstore-0.1.9/tensorstore/util/result_sender_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/result_test.cc` & `tensorstore-0.1.9/tensorstore/util/result_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/sender.h` & `tensorstore-0.1.9/tensorstore/util/sender.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/sender_test.cc` & `tensorstore-0.1.9/tensorstore/util/sender_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/sender_testutil.h` & `tensorstore-0.1.9/tensorstore/util/sender_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/span.h` & `tensorstore-0.1.9/tensorstore/util/span.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/span_json_test.cc` & `tensorstore-0.1.9/tensorstore/util/span_json_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/span_test.cc` & `tensorstore-0.1.9/tensorstore/util/span_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/status.cc` & `tensorstore-0.1.9/tensorstore/util/status.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/status.h` & `tensorstore-0.1.9/tensorstore/util/status.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/status_test.cc` & `tensorstore-0.1.9/tensorstore/util/status_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/status_testutil.cc` & `tensorstore-0.1.9/tensorstore/util/status_testutil.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/status_testutil.h` & `tensorstore-0.1.9/tensorstore/util/status_testutil.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/str_cat.h` & `tensorstore-0.1.9/tensorstore/util/str_cat.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/str_cat_test.cc` & `tensorstore-0.1.9/tensorstore/util/str_cat_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/sync_flow_sender.h` & `tensorstore-0.1.9/tensorstore/util/sync_flow_sender.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/sync_flow_sender_test.cc` & `tensorstore-0.1.9/tensorstore/util/sync_flow_sender_test.cc`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tensorstore/util/utf8_string.h` & `tensorstore-0.1.9/tensorstore/util/utf8_string.h`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/com_facebook_zstd/workspace.bzl` & `tensorstore-0.1.9/third_party/se_curl/workspace.bzl`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_facebook_zstd",
-        strip_prefix = "zstd-1.4.3",
+        name = "se_curl",
+        strip_prefix = "curl-7.70.0",
         urls = [
-            "https://github.com/facebook/zstd/archive/v1.4.3.zip",
+            "https://curl.se/download/curl-7.70.0.tar.gz",
         ],
-        sha256 = "26fcd509af38789185f250c16caaf45c669f2c484533ad9c46eeceb204c81435",
-        build_file = Label("//third_party:com_facebook_zstd/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:com_facebook_zstd/system.BUILD.bazel"),
+        sha256 = "ca2feeb8ef13368ce5d5e5849a5fd5e2dd4755fecf7d8f0cc94000a4206fb8e7",
+        build_file = Label("//third_party:se_curl/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:se_curl/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_github_nlohmann_json/workspace.bzl` & `tensorstore-0.1.9/third_party/com_github_nlohmann_json/workspace.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/com_github_pybind_pybind11/workspace.bzl` & `tensorstore-0.1.9/third_party/com_google_googletest/workspace.bzl`

 * *Files 15% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-load("//third_party:repo.bzl", "third_party_http_archive")
+load(
+    "//third_party:repo.bzl",
+    "third_party_http_archive",
+)
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_github_pybind_pybind11",
-        strip_prefix = "pybind11-2.4.2",
-        urls = [
-            "https://github.com/pybind/pybind11/archive/v2.4.2.tar.gz",
-        ],
-        sha256 = "e212e3043cb7a15466abb8896c6924c1ce40ae2988d8c24c111afcb30735fb8f",
-        build_file = Label("//third_party:com_github_pybind_pybind11/bundled.BUILD.bazel"),
+        name = "com_google_googletest",
+        urls = ["https://github.com/google/googletest/archive/389cb68b87193358358ae87cc56d257fd0d80189.zip"],  # master(2021-01-09)
+        sha256 = "763e20249e76417bed7ebc44aa85fedf5fbac6f9fb6d30bddb628ab07ebf04f5",
+        strip_prefix = "googletest-389cb68b87193358358ae87cc56d257fd0d80189",
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_google_absl/workspace.bzl` & `tensorstore-0.1.9/third_party/com_google_boringssl/workspace.bzl`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_google_absl",
-        sha256 = "d7cc10e05882417ae7a53bc0b121d39863cee82b6b68952e38505c89265c9e5d",
-        strip_prefix = "abseil-cpp-4a851046a0102cd986a5714a1af8deef28a544c4",
+        name = "com_google_boringssl",
         urls = [
-            "https://github.com/abseil/abseil-cpp/archive/4a851046a0102cd986a5714a1af8deef28a544c4.tar.gz",  # 2020-06-16
+            "https://github.com/google/boringssl/archive/bdbe37905216bea8dd4d0fdee93f6ee415d3aa15.tar.gz",  # master-with-bazel(2021-01-09)
         ],
+        sha256 = "ce183cb587c0a0f5982e441dff91cb5456d4c85cfa3fb12816e7a93f20645e51",
+        strip_prefix = "boringssl-bdbe37905216bea8dd4d0fdee93f6ee415d3aa15",
+        system_build_file = Label("//third_party/com_google_boringssl:system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_google_benchmark/workspace.bzl` & `tensorstore-0.1.9/third_party/com_google_benchmark/workspace.bzl`

 * *Files 14% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
         name = "com_google_benchmark",
-        urls = ["https://github.com/google/benchmark/archive/v1.5.0.zip"],  # 2019-05-28
-        sha256 = "2d22dd3758afee43842bb504af1a8385cccb3ee1f164824e4837c1c1b04d92a0",
-        strip_prefix = "benchmark-1.5.0",
+        urls = ["https://github.com/google/benchmark/archive/v1.5.2.zip"],
+        sha256 = "21e6e096c9a9a88076b46bd38c33660f565fa050ca427125f64c4a8bf60f336b",
+        strip_prefix = "benchmark-1.5.2",
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_google_boringssl/workspace.bzl` & `tensorstore-0.1.9/third_party/com_google_absl/workspace.bzl`

 * *Files 20% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_google_boringssl",
+        name = "com_google_absl",
+        sha256 = "b54c84452fc0786c1763eeb1a8d999272f0ecc9ec4ee74eb6cfe0a61adb6aa1c",
+        strip_prefix = "abseil-cpp-62ce712ecc887f669610a93efe18abecf70b47a0",
         urls = [
-            # When updating, always use commit from master-with-bazel branch.
-            "https://github.com/google/boringssl/archive/34693f02f6cf9ac7982778b761c16a27f32433c1.tar.gz",  # 2019-09-25
+            "https://github.com/abseil/abseil-cpp/archive/62ce712ecc887f669610a93efe18abecf70b47a0.tar.gz",  # master(2021-01-09)
         ],
-        sha256 = "633e2e806d01a07a20725d1e68fff0be96db18344ed4389c00de042dcd874cac",
-        strip_prefix = "boringssl-34693f02f6cf9ac7982778b761c16a27f32433c1",
-        system_build_file = Label("//third_party/com_google_boringssl:system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_google_googletest/workspace.bzl` & `tensorstore-0.1.9/third_party/net_zlib/workspace.bzl`

 * *Files 18% similar despite different names*

```diff
@@ -17,12 +17,16 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_google_googletest",
-        urls = ["https://github.com/google/googletest/archive/f2fb48c3b3d79a75a88a99fba6576b25d42ec528.zip"],  # 2019-09-15
-        sha256 = "89e98c265b80181d902b1a19c10c29b3a22d804b207214d8104ad42905fbae87",
-        strip_prefix = "googletest-f2fb48c3b3d79a75a88a99fba6576b25d42ec528",
+        name = "net_zlib",
+        sha256 = "c3e5e9fdd5004dcb542feda5ee4f0ff0744628baf8ed2dd5d66f8ca1197cb1a1",
+        strip_prefix = "zlib-1.2.11",
+        urls = [
+            "https://zlib.net/zlib-1.2.11.tar.gz",
+        ],
+        build_file = Label("//third_party:net_zlib/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:net_zlib/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/com_google_snappy/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/com_google_snappy/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/com_google_snappy/workspace.bzl` & `tensorstore-0.1.9/third_party/org_tukaani_xz/workspace.bzl`

 * *Files 19% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-load(
-    "//third_party:repo.bzl",
-    "third_party_http_archive",
-)
+load("//third_party:repo.bzl", "third_party_http_archive")
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "com_google_snappy",
-        urls = ["https://github.com/google/snappy/archive/1.1.7.zip"],
-        sha256 = "61e05a0295fd849072668b1f3494801237d809427cfe8fd014cda455036c3ef7",
-        strip_prefix = "snappy-1.1.7",
-        build_file = Label("//third_party:com_google_snappy/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:com_google_snappy/system.BUILD.bazel"),
+        name = "org_tukaani_xz",
+        strip_prefix = "xz-5.2.5",
+        urls = [
+            "https://tukaani.org/xz/xz-5.2.5.tar.gz",
+        ],
+        sha256 = "f6f4910fd033078738bd82bfba4f49219d03b17eb0794eb91efbae419f4aba10",
+        build_file = Label("//third_party:org_tukaani_xz/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:org_tukaani_xz/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/jpeg/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/jpeg/bundled.BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 load("@com_github_google_tensorstore//:utils.bzl", "cc_library_with_strip_include_prefix", "template_rule")
 
 licenses(["notice"])
 
 exports_files(["LICENSE.md"])
 
 WIN_COPTS = [
+    "/Ox",
     "-DWITH_SIMD",
     "-wd4996",
 ]
 
 libjpegturbo_copts = select({
-    ":android": [],
+    ":android": [
+        "-O2",
+        "-fPIE",
+        "-w",
+    ],
     ":windows": WIN_COPTS,
-    "//conditions:default": [],
+    "//conditions:default": [
+        "-O3",
+        "-w",
+    ],
 }) + select({
     ":armeabi-v7a": [
         "-D__ARM_NEON__",
         "-march=armv7-a",
         "-mfloat-abi=softfp",
         "-fprefetch-loop-arrays",
     ],
@@ -502,38 +510,38 @@
     },
 )
 
 JCONFIG_NOWIN_COMMON_SUBSTITUTIONS = {
     "@JPEG_LIB_VERSION@": "62",
     "@VERSION@": "2.0.0",
     "@LIBJPEG_TURBO_VERSION_NUMBER@": "2000000",
-    "#cmakedefine C_ARITH_CODING_SUPPORTED": "#define C_ARITH_CODING_SUPPORTED",
-    "#cmakedefine D_ARITH_CODING_SUPPORTED": "#define D_ARITH_CODING_SUPPORTED",
-    "#cmakedefine MEM_SRCDST_SUPPORTED": "#define MEM_SRCDST_SUPPORTED",
+    "#cmakedefine C_ARITH_CODING_SUPPORTED 1": "#define C_ARITH_CODING_SUPPORTED 1",
+    "#cmakedefine D_ARITH_CODING_SUPPORTED 1": "#define D_ARITH_CODING_SUPPORTED 1",
+    "#cmakedefine MEM_SRCDST_SUPPORTED 1": "#define MEM_SRCDST_SUPPORTED 1",
     "@BITS_IN_JSAMPLE@": "8",
-    "#cmakedefine HAVE_LOCALE_H": "#define HAVE_LOCALE_H 1",
-    "#cmakedefine HAVE_STDDEF_H": "#define HAVE_STDDEF_H 1",
-    "#cmakedefine HAVE_STDLIB_H": "#define HAVE_STDLIB_H 1",
-    "#cmakedefine NEED_SYS_TYPES_H": "#define NEED_SYS_TYPES_H",
-    "#cmakedefine NEED_BSD_STRINGS": "",
-    "#cmakedefine HAVE_UNSIGNED_CHAR": "#define HAVE_UNSIGNED_CHAR 1",
-    "#cmakedefine HAVE_UNSIGNED_SHORT": "#define HAVE_UNSIGNED_SHORT 1",
-    "#cmakedefine INCOMPLETE_TYPES_BROKEN": "",
-    "#cmakedefine RIGHT_SHIFT_IS_UNSIGNED": "",
-    "#cmakedefine __CHAR_UNSIGNED__": "",
+    "#cmakedefine HAVE_LOCALE_H 1": "#define HAVE_LOCALE_H 1",
+    "#cmakedefine HAVE_STDDEF_H 1": "#define HAVE_STDDEF_H 1",
+    "#cmakedefine HAVE_STDLIB_H 1": "#define HAVE_STDLIB_H 1",
+    "#cmakedefine NEED_SYS_TYPES_H 1": "#define NEED_SYS_TYPES_H 1",
+    "#cmakedefine NEED_BSD_STRINGS 1": "",
+    "#cmakedefine HAVE_UNSIGNED_CHAR 1": "#define HAVE_UNSIGNED_CHAR 1",
+    "#cmakedefine HAVE_UNSIGNED_SHORT 1": "#define HAVE_UNSIGNED_SHORT 1",
+    "#cmakedefine INCOMPLETE_TYPES_BROKEN 1": "",
+    "#cmakedefine RIGHT_SHIFT_IS_UNSIGNED 1": "",
+    "#cmakedefine __CHAR_UNSIGNED__ 1": "",
     "#undef const": "",
     "#undef size_t": "",
 }
 
 JCONFIG_NOWIN_SIMD_SUBSTITUTIONS = {
-    "#cmakedefine WITH_SIMD": "#define WITH_SIMD",
+    "#cmakedefine WITH_SIMD 1": "#define WITH_SIMD 1",
 }
 
 JCONFIG_NOWIN_NOSIMD_SUBSTITUTIONS = {
-    "#cmakedefine WITH_SIMD": "",
+    "#cmakedefine WITH_SIMD 1": "",
 }
 
 JCONFIG_NOWIN_SIMD_SUBSTITUTIONS.update(JCONFIG_NOWIN_COMMON_SUBSTITUTIONS)
 
 JCONFIG_NOWIN_NOSIMD_SUBSTITUTIONS.update(JCONFIG_NOWIN_COMMON_SUBSTITUTIONS)
 
 template_rule(
```

### Comparing `tensorstore-0.1.8/third_party/jpeg/workspace.bzl` & `tensorstore-0.1.9/third_party/jpeg/workspace.bzl`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     maybe(
         third_party_http_archive,
         # Note: The generic name "jpeg" is used in place of the more canonical
         # "org_libjpeg_turbo" because this repository may actually refer to the
         # system jpeg.
         name = "jpeg",
         urls = [
-            "https://github.com/libjpeg-turbo/libjpeg-turbo/archive/2.0.0.tar.gz",
+            "https://github.com/libjpeg-turbo/libjpeg-turbo/archive/2.0.5.tar.gz",
         ],
-        sha256 = "f892fff427ab3adffc289363eac26d197ce3ccacefe5f5822377348a8166069b",
-        strip_prefix = "libjpeg-turbo-2.0.0",
+        sha256 = "b3090cd37b5a8b3e4dbd30a1311b3989a894e5d3c668f14cbc6739d77c9402b7",
+        strip_prefix = "libjpeg-turbo-2.0.5",
         build_file = Label("//third_party:jpeg/bundled.BUILD.bazel"),
         system_build_file = Label("//third_party:jpeg/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/nasm/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/nasm/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/nasm/workspace.bzl` & `tensorstore-0.1.9/third_party/nasm/workspace.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/net_sourceforge_half/workspace.bzl` & `tensorstore-0.1.9/third_party/net_sourceforge_half/workspace.bzl`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
         name = "net_sourceforge_half",
         urls = [
-            "http://sourceforge.net/projects/half/files/half/2.1.0/half-2.1.0.zip",
+            "https://sourceforge.net/projects/half/files/half/2.1.0/half-2.1.0.zip",
         ],
         sha256 = "ad1788afe0300fa2b02b0d1df128d857f021f92ccf7c8bddd07812685fa07a25",
         build_file = Label("//third_party:net_sourceforge_half/bundled.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/net_zlib/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/net_zlib/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/net_zlib/workspace.bzl` & `tensorstore-0.1.9/third_party/org_sourceware_bzip2/workspace.bzl`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "net_zlib",
-        sha256 = "c3e5e9fdd5004dcb542feda5ee4f0ff0744628baf8ed2dd5d66f8ca1197cb1a1",
-        strip_prefix = "zlib-1.2.11",
+        name = "org_sourceware_bzip2",
         urls = [
-            "https://zlib.net/zlib-1.2.11.tar.gz",
+            "https://sourceware.org/pub/bzip2/bzip2-1.0.8.tar.gz",
         ],
-        build_file = Label("//third_party:net_zlib/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:net_zlib/system.BUILD.bazel"),
+        strip_prefix = "bzip2-1.0.8",
+        sha256 = "ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269",
+        build_file = Label("//third_party:org_sourceware_bzip2/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:org_sourceware_bzip2/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/org_blosc_cblosc/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/org_blosc_cblosc/bundled.BUILD.bazel`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 
 cc_library_with_strip_include_prefix(
     name = "blosc",
     srcs = [
         "blosc/blosc.c",
         "blosc/blosclz.c",
         "blosc/blosclz.h",
-        "blosc/blosclz_impl.inc",
         "blosc/fastcopy.c",
         "blosc/fastcopy.h",
     ],
     hdrs = [
         "blosc/blosc.h",
         "blosc/blosc-export.h",
     ],
```

### Comparing `tensorstore-0.1.8/third_party/org_blosc_cblosc/workspace.bzl` & `tensorstore-0.1.9/third_party/com_google_snappy/workspace.bzl`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "org_blosc_cblosc",
-        strip_prefix = "c-blosc-1.16.3",
-        urls = [
-            "https://github.com/Blosc/c-blosc/archive/v1.16.3.zip",
-        ],
-        sha256 = "e3b4d25296d81e004e8207022c389b38b9376af46be02b1fb22d244ea71331be",
-        build_file = Label("//third_party:org_blosc_cblosc/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:org_blosc_cblosc/system.BUILD.bazel"),
+        name = "com_google_snappy",
+        urls = ["https://github.com/google/snappy/archive/1.1.8.zip"],
+        sha256 = "38b4aabf88eb480131ed45bfb89c19ca3e2a62daeb081bdf001cfb17ec4cd303",
+        strip_prefix = "snappy-1.1.8",
+        build_file = Label("//third_party:com_google_snappy/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:com_google_snappy/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/org_lz4/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/org_lz4/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/org_lz4/workspace.bzl` & `tensorstore-0.1.9/third_party/com_facebook_zstd/workspace.bzl`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "org_lz4",
-        strip_prefix = "lz4-1.9.2",
+        name = "com_facebook_zstd",
+        strip_prefix = "zstd-1.4.8",
         urls = [
-            "https://github.com/lz4/lz4/archive/v1.9.2.zip",
+            "https://github.com/facebook/zstd/archive/v1.4.8.zip",
         ],
-        sha256 = "0b8bf249fd54a0b974de1a50f0a13ba809a78fd48f90c465c240ee28a9e4784d",
-        build_file = Label("//third_party:org_lz4/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:org_lz4/system.BUILD.bazel"),
+        sha256 = "136a9197711e746899b9c8a36db378432427a165d446b19831c400ae30fa2e64",
+        build_file = Label("//third_party:com_facebook_zstd/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:com_facebook_zstd/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/org_nghttp2/workspace.bzl` & `tensorstore-0.1.9/third_party/org_nghttp2/workspace.bzl`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
         name = "org_nghttp2",
-        strip_prefix = "nghttp2-1.41.0",
+        strip_prefix = "nghttp2-1.42.0",
         urls = [
-            "https://github.com/nghttp2/nghttp2/releases/download/v1.41.0/nghttp2-1.41.0.tar.gz",
+            "https://github.com/nghttp2/nghttp2/releases/download/v1.42.0/nghttp2-1.42.0.tar.gz",
         ],
-        sha256 = "eacc6f0f8543583ecd659faf0a3f906ed03826f1d4157b536b4b385fe47c5bb8",
+        sha256 = "884d18a0158908125d58b1b61d475c0325e5a004e3d61a56b5fcc55d5f4b7af5",
         build_file = Label("//third_party:org_nghttp2/bundled.BUILD.bazel"),
         system_build_file = Label("//third_party:org_nghttp2/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/org_sourceware_bzip2/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/org_sourceware_bzip2/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/org_sourceware_bzip2/workspace.bzl` & `tensorstore-0.1.9/third_party/org_blosc_cblosc/workspace.bzl`

 * *Files 25% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "third_party_http_archive",
 )
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
         third_party_http_archive,
-        name = "org_sourceware_bzip2",
+        name = "org_blosc_cblosc",
+        strip_prefix = "c-blosc-1.21.0",
         urls = [
-            "https://sourceware.org/pub/bzip2/bzip2-1.0.8.tar.gz",
+            "https://github.com/Blosc/c-blosc/archive/v1.21.0.zip",
         ],
-        strip_prefix = "bzip2-1.0.8",
-        sha256 = "ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269",
-        build_file = Label("//third_party:org_sourceware_bzip2/bundled.BUILD.bazel"),
-        system_build_file = Label("//third_party:org_sourceware_bzip2/system.BUILD.bazel"),
+        sha256 = "09dee9dc4d1b85463b87d92f1494a44d23eafadbda2580b76e327eaa59f8a9ef",
+        build_file = Label("//third_party:org_blosc_cblosc/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:org_blosc_cblosc/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/org_tukaani_xz/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/org_tukaani_xz/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/pypa/avro_python3/workspace.bzl` & `tensorstore-0.1.9/third_party/com_github_pybind_pybind11/workspace.bzl`

 * *Files 24% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines a third-party bazel repo for the `avro-python3` Python package."""
 
-load(
-    "//third_party:repo.bzl",
-    "third_party_python_package",
-)
+load("//third_party:repo.bzl", "third_party_http_archive")
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
     maybe(
-        third_party_python_package,
-        name = "pypa_avro_python3",
-        target = "avro_python3",
-        requirement = "avro-python3==1.9.2.1",
+        third_party_http_archive,
+        name = "com_github_pybind_pybind11",
+        strip_prefix = "pybind11-2.6.1",
+        urls = [
+            "https://github.com/pybind/pybind11/archive/v2.6.1.tar.gz",
+        ],
+        sha256 = "cdbe326d357f18b83d10322ba202d69f11b2f49e2d87ade0dc2be0c5c34f8e2a",
+        build_file = Label("//third_party:com_github_pybind_pybind11/bundled.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/pypa/generate_pypa_directory.py` & `tensorstore-0.1.9/third_party/pypa/generate_workspace.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,91 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Generates bazel workspace rules for fetching Python packages from PyPI."""
+"""Generates bazel workspace rules for fetching Python packages from PyPI.
+
+This script fetches dependency information from PyPI.
+
+Note depending on how packages are created and uploaded to PyPI, PyPI may not
+contain correct dependency information.  (In that case, it would be necessary to
+actually install the package with `pip` in order to determine the dependencies.)
+However, for all of the packages required by TensorStore, the dependency
+information is available from PyPI.
+"""
 
 import argparse
+import concurrent.futures
 import json
 import os
-import subprocess
+
+import packaging.requirements
+import packaging.version
+import requests
+
+
+def get_package_json(name: str):
+  r = requests.get(f'https://pypi.python.org/pypi/{name}/json')
+  r.raise_for_status()
+  return r.json()
+
+
+class _AnyValue:
+  """Special value for which all comparisons return true.
+
+  This is used for marker evaluation to accept any value.
+  """
+
+  def __eq__(self, other):
+    return True
+
+  def __ne__(self, other):
+    return True
+
+  def __lt__(self, other):
+    return True
+
+  def __gt__(self, other):
+    return True
+
+  def __ge__(self, other):
+    return True
+
+  def __le__(self, other):
+    return True
+
+
+def _evaluate_marker(marker):
+  if marker is None:
+    return True
+  return any(
+      marker.evaluate({
+          "sys_platform": _AnyValue(),
+          "python_version": python_version,
+          "extra": None
+      }) for python_version in ("3.6", "3.7", "3.8", "3.9"))
+
+
+def get_package_metadata(name: str):
+  j = get_package_json(name)
+  requires_dist = j["info"].get("requires_dist", [])
+  if requires_dist is None:
+    requires_dist = []
+  deps = []
+  for req_text in requires_dist:
+    req = packaging.requirements.Requirement(req_text)
+    if _evaluate_marker(req.marker):
+      deps.append(req.name.lower())
+  versions = [packaging.version.parse(v) for v in j["releases"].keys()]
+  versions = [v for v in versions if not v.is_prerelease]
+  versions.sort()
+  return {"Requires": sorted(deps), "Name": name, "Version": str(versions[-1])}
 
 
 def get_target_name(package_name):
   return package_name.lower().replace("-", "_")
 
 
 def get_repo_name(package_name):
@@ -28,145 +99,117 @@
 
 
 def get_full_target_name(package_name):
   return "@%s//:%s" % (get_repo_name(package_name),
                        get_target_name(package_name))
 
 
-def parse_package_metadata(pip_info):
-  deps = []
-  metadata = {}
-  for line in pip_info.splitlines():
-    line = line.strip()
-    if not line:
-      continue
-    colon = line.index(":")
-    key = line[:colon]
-    value = line[colon + 1:].strip()
-    metadata[key] = value
-  if metadata["Requires"]:
-    deps = sorted(x.lower() for x in metadata["Requires"].split(", "))
-  metadata["Requires"] = deps
-  return metadata
-
-
 def get_package_info(package_names):
-  all_pip_info = subprocess.check_output(["pip", "show"] +
-                                         package_names).decode()
   all_metadata = {}
-  for pip_info in all_pip_info.split("\n---\n"):
-    metadata = parse_package_metadata(pip_info)
-    all_metadata[metadata["Name"].lower()] = metadata
+  with concurrent.futures.ThreadPoolExecutor(max_workers=100) as executor:
+    for metadata in executor.map(get_package_metadata, package_names):
+      all_metadata[metadata["Name"].lower()] = metadata
   return all_metadata
 
 
-def write_workspace(package_name, metadata, tools_workspace):
-  dir_name = get_target_name(package_name)
+def write_repo_macros(f, metadata):
+  package_name = metadata["Name"].lower()
   repo_name = get_repo_name(package_name)
-  os.makedirs(dir_name, exist_ok=True)
-  bzl_path = os.path.join(dir_name, "workspace.bzl")
-  with open(bzl_path, "w") as f:
-    f.write("""# Copyright 2020 The TensorStore Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+  f.write(f"""def repo_{repo_name}():
+""")
+  for dep in metadata["Requires"]:
+    f.write(f"    repo_{get_repo_name(dep)}()\n")
+  f.write("""    maybe(
+        third_party_python_package,
+        name = """ + json.dumps(repo_name) + """,
+        target = """ + json.dumps(get_target_name(package_name)) + """,
+        requirement = """ +
+          json.dumps(package_name + "==" + metadata["Version"]) + """,
+""")
+  if metadata["Requires"]:
+    f.write("        deps = [\n")
+    for dep in metadata["Requires"]:
+      f.write("            " + json.dumps(get_full_target_name(dep)) + ",\n")
+    f.write("        ],\n")
+
+  f.write("""    )
 """)
+
+
+def write_workspace(all_metadata, tools_workspace):
+  all_metadata = sorted(all_metadata, key=lambda x: x["Name"].lower())
+  with open("workspace.bzl", "w") as f:
     f.write(
-        '"""Defines a third-party bazel repo for the `%s` Python package."""\n\n'
-        % (package_name,))
+        '"""Defines third-party bazel repos for Python packages fetched with pip."""\n\n'
+    )
     f.write("""load(
     \"""" + tools_workspace + """//third_party:repo.bzl",
     "third_party_python_package",
 )
 """)
-    for dep in metadata["Requires"]:
-      f.write("""load("//third_party:pypa/""" + get_target_name(dep) +
-              """/workspace.bzl", repo_""" + get_repo_name(dep) + """ = "repo")
-""")
     f.write("""load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
-def repo():
 """)
-    for dep in metadata["Requires"]:
-      f.write("    repo_" + get_repo_name(dep) + "()\n")
-
-    f.write("""    maybe(
-        third_party_python_package,
-        name = """ + json.dumps(repo_name) + """,
-        target = """ + json.dumps(dir_name) + """,
-        requirement = """ +
-            json.dumps(package_name + "==" + metadata["Version"]) + """,
+    f.write("""def repo():
 """)
-    if metadata["Requires"]:
-      f.write("        deps = [\n")
-      for dep in metadata["Requires"]:
-        f.write("            " + json.dumps(get_full_target_name(dep)) + ",\n")
-      f.write("        ],\n")
-
-    f.write("""    )
-""")
-  print("Wrote: %s" % (bzl_path,))
+    for metadata in all_metadata:
+      dep_repo_name = get_repo_name(metadata["Name"])
+      f.write(f'    repo_{dep_repo_name}()\n')
+
+    for metadata in all_metadata:
+      f.write("\n")
+      write_repo_macros(f, metadata)
 
 
 def generate(args):
   all_packages = list(args.package)
   if not all_packages:
-    all_packages = [
+    all_packages = set([
         "numpy",
         # Shell
         "ipython",
         "absl-py",
         # Test
         "pytest",
         "pytest-asyncio",
         # Build
         "wheel",
         # Docs
         "sphinx",
-        "sphinx-autobuild",
         "sphinx-rtd-theme",
         "jsonpointer",
         "jsonschema",
         "pyyaml",
+        "astor",
+        "docutils",
         # Examples
         "apache-beam",
         "gin-config",
-    ]
+    ])
   seen_packages = set()
+  all_metadata = {}
   while all_packages:
     cur_packages = all_packages
-    all_metadata = get_package_info(cur_packages)
-    all_packages = []
+    all_metadata.update(get_package_info(cur_packages))
+    all_packages = set()
     for package_name in cur_packages:
       if package_name in seen_packages:
         continue
       seen_packages.add(package_name)
       metadata = all_metadata[package_name]
-      write_workspace(
-          package_name=package_name,
-          metadata=metadata,
-          tools_workspace=args.tools_workspace,
-      )
-      if args.recursive:
-        all_packages.extend(metadata["Requires"])
+      all_packages.update(metadata["Requires"])
+  write_workspace(
+      all_metadata=all_metadata.values(),
+      tools_workspace=args.tools_workspace,
+  )
 
 
 def main():
   ap = argparse.ArgumentParser()
   ap.add_argument("package", nargs="*")
-  ap.add_argument("-r", "--recursive", action="store_true")
   ap.add_argument("--tools-workspace", default="")
   args = ap.parse_args()
   generate(args)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `tensorstore-0.1.8/third_party/pypa/pyarrow/workspace.bzl` & `tensorstore-0.1.9/third_party/org_lz4/workspace.bzl`

 * *Files 26% similar despite different names*

```diff
@@ -7,30 +7,26 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines a third-party bazel repo for the `pyarrow` Python package."""
 
 load(
     "//third_party:repo.bzl",
-    "third_party_python_package",
+    "third_party_http_archive",
 )
-load("//third_party:pypa/numpy/workspace.bzl", repo_pypa_numpy = "repo")
-load("//third_party:pypa/six/workspace.bzl", repo_pypa_six = "repo")
 load("@bazel_tools//tools/build_defs/repo:utils.bzl", "maybe")
 
 def repo():
-    repo_pypa_numpy()
-    repo_pypa_six()
     maybe(
-        third_party_python_package,
-        name = "pypa_pyarrow",
-        target = "pyarrow",
-        requirement = "pyarrow==0.16.0",
-        deps = [
-            "@pypa_numpy//:numpy",
-            "@pypa_six//:six",
+        third_party_http_archive,
+        name = "org_lz4",
+        strip_prefix = "lz4-1.9.3",
+        urls = [
+            "https://github.com/lz4/lz4/archive/v1.9.3.zip",
         ],
+        sha256 = "4ec935d99aa4950eadfefbd49c9fad863185ac24c32001162c44a683ef61b580",
+        build_file = Label("//third_party:org_lz4/bundled.BUILD.bazel"),
+        system_build_file = Label("//third_party:org_lz4/system.BUILD.bazel"),
     )
```

### Comparing `tensorstore-0.1.8/third_party/python/BUILD.tpl` & `tensorstore-0.1.9/third_party/python/BUILD.tpl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/python/python_configure.bzl` & `tensorstore-0.1.9/third_party/python/python_configure.bzl`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/third_party/repo.bzl` & `tensorstore-0.1.9/third_party/repo.bzl`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Supports definining bazel repos for third-party dependencies.
 
 The `TENSORSTORE_SYSTEM_LIBS` environment variable may be used to
 specify that system libraries should be used in place of bundled
 libraries.  It should be set to a comma-separated list of the repo
-names, e.g. `TENSORSTORE_SYSTEM_LIBS=net_zlib,se_haxx_curl` to use
+names, e.g. `TENSORSTORE_SYSTEM_LIBS=net_zlib,se_curl` to use
 system-provided zlib and libcurl.
 """
 
 load(
     "@bazel_tools//tools/build_defs/repo:utils.bzl",
     "patch",
     "update_attrs",
```

### Comparing `tensorstore-0.1.8/third_party/se_haxx_curl/bundled.BUILD.bazel` & `tensorstore-0.1.9/third_party/se_curl/bundled.BUILD.bazel`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tools/docs/build_docs.py` & `tensorstore-0.1.9/docs/build_docs.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,44 +14,36 @@
 """Builds the documentation using sphinx."""
 
 import argparse
 import contextlib
 import os
 import pathlib
 import re
-import subprocess
 import sys
 import tempfile
 import urllib.parse
 
+DOCS_ROOT = 'docs'
+THIRD_PARTY_ROOT = 'third_party'
+CPP_ROOT = 'tensorstore'
 
-def _find_workspace_dir() -> str:
-  workspace_dir = os.getenv('BUILD_WORKSPACE_DIRECTORY')
-  if workspace_dir:
-    return workspace_dir
-  p = pathlib.Path('x')
-  for d in p.parents:
-    if (d / 'WORKSPACE').exists():
-      return str(p)
-  raise RuntimeError('Could not find WORKSPACE root')
 
-
-def _write_third_party_libraries_summary(workspace_dir: str, output_path: str):
+def _write_third_party_libraries_summary(runfiles_dir: str, output_path: str):
   """Generate the third_party_libraries.rst file."""
   with open(output_path, 'w') as f:
     f.write("""
 .. list-table:: Required third-party libraries
    :header-rows: 1
 
    * - Identifier
      - Bundled library
      - Version
 """)
     third_party_libs = []
-    for dep in (pathlib.Path(workspace_dir) / 'third_party').iterdir():
+    for dep in (pathlib.Path(runfiles_dir) / THIRD_PARTY_ROOT).iterdir():
       if not dep.is_dir():
         continue
       workspace_bzl_file = dep / 'workspace.bzl'
       if not workspace_bzl_file.exists():
         continue
       identifier = dep.name
       system_lib_supported = (dep / 'system.BUILD.bazel').exists()
@@ -78,66 +70,80 @@
     for identifier, name, homepage, version in third_party_libs:
       f.write('   * - ``%s``\n' % (identifier,))
       f.write('     - `%s <%s>`_\n' % (name, homepage))
       f.write('     - %s\n' % (version,))
 
 
 @contextlib.contextmanager
-def _prepare_source_tree(workspace_dir: str):
+def _prepare_source_tree(runfiles_dir: str):
   with tempfile.TemporaryDirectory() as temp_src_dir:
 
     _write_third_party_libraries_summary(
-        workspace_dir=workspace_dir,
+        runfiles_dir=runfiles_dir,
         output_path=os.path.join(temp_src_dir, 'third_party_libraries.rst'))
 
     def create_symlinks(source_dir, target_dir):
       for name in os.listdir(source_dir):
         source_path = os.path.join(source_dir, name)
         target_path = os.path.join(target_dir, name)
         if os.path.isdir(source_path):
           os.makedirs(target_path, exist_ok=True)
           create_symlinks(source_path, target_path)
-        else:
-          os.symlink(os.path.abspath(source_path), target_path)
-
-    create_symlinks(os.path.join(workspace_dir, 'docs'), temp_src_dir)
-    os.symlink(
-        os.path.abspath(os.path.join(workspace_dir, 'tensorstore')),
-        os.path.join(temp_src_dir, 'tensorstore'))
+          continue
+        if os.path.exists(target_path):
+          # Remove target path if it already exists from a previous run.
+          os.remove(target_path)
+        os.symlink(os.path.abspath(source_path), target_path)
+
+    create_symlinks(os.path.join(runfiles_dir, DOCS_ROOT), temp_src_dir)
+    source_cpp_root = os.path.abspath(os.path.join(runfiles_dir, CPP_ROOT))
+    temp_cpp_root = os.path.join(temp_src_dir, 'tensorstore')
+    os.makedirs(temp_cpp_root)
+    for name in ['driver', 'kvstore']:
+      os.symlink(
+          os.path.join(source_cpp_root, name),
+          os.path.join(temp_cpp_root, name))
     yield temp_src_dir
 
 
-def auto_build_docs(workspace_dir: str, out_dir: str, extra_args):
-  import sphinx_autobuild
-  with _prepare_source_tree(workspace_dir) as temp_src_dir:
-    os.chdir(temp_src_dir)
-    sys.argv = [
-        sys.argv[0],
-        '.',
-        out_dir,
-        '-i',
-        'python/api/*.rst',
-        '--poll',
-    ] + extra_args
-    sphinx_autobuild.main()
+def run(args, unknown):
+  # Ensure tensorstore sphinx extensions can be imported as absolute modules.
+  sys.path.insert(0, os.path.abspath(DOCS_ROOT))
+  # For some reason, the way bazel sets up import paths causes `import
+  # sphinxcontrib.serializinghtml` not to work unless we first import
+  # `sphinxcontrib.applehelp`.
+  import sphinxcontrib.applehelp
+  if args.sphinx_help:
+    unknown = unknown + ['--help']
+  runfiles_dir = os.getcwd()
+  os.makedirs(args.output, exist_ok=True)
+  with _prepare_source_tree(runfiles_dir) as temp_src_dir:
+    import sphinx.cmd.build
+    sys.exit(
+        sphinx.cmd.build.main(['-j', 'auto', '-a', temp_src_dir, args.output] +
+                              unknown))
 
 
 def main():
   ap = argparse.ArgumentParser()
-  ap.add_argument('--output', '-o', help='Output directory')
+  default_output = os.environ.get('TEST_UNDECLARED_OUTPUTS_DIR', None)
+  ap.add_argument(
+      '--output',
+      '-o',
+      help='Output directory',
+      default=default_output,
+      required=default_output is None)
+  ap.add_argument(
+      '--sphinx-help',
+      action='store_true',
+      help='Show sphinx build command-line help')
+  ap.add_argument('--pdb', action='store_true', help='Run under pdb')
   args, unknown = ap.parse_known_args()
-  workspace_dir = _find_workspace_dir()
-  if args.output:
-    os.makedirs(args.output, exist_ok=True)
-    with _prepare_source_tree(workspace_dir) as temp_src_dir:
-      sys.exit(
-          subprocess.call([
-              'python', '-m', 'sphinx.cmd.build', '-j', 'auto', '-a',
-              temp_src_dir, args.output
-          ] + unknown))
+  if args.pdb:
+    import pdb
+    pdb.runcall(run, args, unknown)
   else:
-    with tempfile.TemporaryDirectory() as out_dir:
-      auto_build_docs(workspace_dir, out_dir, unknown)
+    run(args, unknown)
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `tensorstore-0.1.8/tools/docs/json_pprint.py` & `tensorstore-0.1.9/docs/json_pprint.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tools/docs/tensorstore_autosummary.py` & `tensorstore-0.1.9/docs/tensorstore_autosummary.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
 
 sphinx.domains.python._pseudo_parse_arglist = _render_python_arglist  # pylint: disable=protected-access
 
 old_desc_returns = sphinx.addnodes.desc_returns
 
 
-def _python_desc_returns(part, unused):
+def _python_desc_returns(part, *unused):
   del unused
   rnode = old_desc_returns()
   rnode += _make_python_type_ref_from_annotation(ast.parse(part).body[0].value)
   return rnode
 
 
 _old_handle_signature = sphinx.domains.python.PyObject.handle_signature
```

### Comparing `tensorstore-0.1.8/tools/docs/tensorstore_jsonschema_sphinx.py` & `tensorstore-0.1.9/docs/tensorstore_jsonschema_sphinx.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tools/docs/update_doctests.py` & `tensorstore-0.1.9/docs/update_doctests.py`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tools/python-manylinux/build_wheels_inside_container.sh` & `tensorstore-0.1.9/tools/python-manylinux/build_wheels_inside_container.sh`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/tools/python-manylinux/build_wheels_manylinux2014_x86_64.sh` & `tensorstore-0.1.9/tools/python-manylinux/build_wheels_manylinux2014_x86_64.sh`

 * *Files identical despite different names*

### Comparing `tensorstore-0.1.8/utils.bzl` & `tensorstore-0.1.9/utils.bzl`

 * *Files identical despite different names*

