# Comparing `tmp/nb-autodoc-1.0.0a6.tar.gz` & `tmp/nb-autodoc-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-autodoc-1.0.0a6.tar", last modified: Wed Jun 21 14:20:57 2023, max compression
+gzip compressed data, was "nb-autodoc-1.0.0a7.tar", last modified: Fri Jun 23 15:04:58 2023, max compression
```

## Comparing `nb-autodoc-1.0.0a6.tar` & `nb-autodoc-1.0.0a7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1064 2021-11-24 06:50:23.530000 nb-autodoc-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     1743 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/README.md
--rw-r--r--   0        0        0       86 2023-06-21 14:18:00.713881 nb-autodoc-1.0.0a6/nb_autodoc/__init__.py
--rw-r--r--   0        0        0     1318 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/__main__.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/__init__.py
--rw-r--r--   0        0        0     2791 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/analyzer.py
--rw-r--r--   0        0        0      484 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/base.py
--rw-r--r--   0        0        0    12841 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/definitionfinder.py
--rw-r--r--   0        0        0     5697 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/unparse_ann.py
--rw-r--r--   0        0        0    10475 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/utils.py
--rw-r--r--   0        0        0    15331 2023-03-22 10:11:28.688069 nb-autodoc-1.0.0a6/nb_autodoc/annotation.py
--rw-r--r--   0        0        0     7597 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/builders/__init__.py
--rw-r--r--   0        0        0      406 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/builders/helpers.py
--rw-r--r--   0        0        0    26266 2023-05-05 09:04:38.574920 nb-autodoc-1.0.0a6/nb_autodoc/builders/markdown.py
--rw-r--r--   0        0        0     2478 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/nb_autodoc/config.py
--rw-r--r--   0        0        0       83 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/__init__.py
--rw-r--r--   0        0        0    15112 2023-06-21 14:14:36.863882 nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/google.py
--rw-r--r--   0        0        0     1991 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/log.py
--rw-r--r--   0        0        0    33670 2023-05-05 09:07:44.174879 nb-autodoc-1.0.0a6/nb_autodoc/manager.py
--rw-r--r--   0        0        0    15796 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/modulefinder.py
--rw-r--r--   0        0        0     4512 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/nodes.py
--rw-r--r--   0        0        0        0 2022-10-10 09:23:09.200000 nb-autodoc-1.0.0a6/nb_autodoc/py.typed
--rw-r--r--   0        0        0     1396 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/nb_autodoc/typing.py
--rw-r--r--   0        0        0     8599 2023-03-22 10:06:52.428169 nb-autodoc-1.0.0a6/nb_autodoc/utils.py
--rw-r--r--   0        0        0     1228 2023-03-22 08:53:54.029767 nb-autodoc-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0       29 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/assigndata-override-ast.py
--rw-r--r--   0        0        0      203 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/exec_type_checking.py
--rw-r--r--   0        0        0      169 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/analyzerdata/extract-docstring.py
--rw-r--r--   0        0        0      380 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/overload.py
--rw-r--r--   0        0        0     1286 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/simple-definition-ast.py
--rw-r--r--   0        0        0      342 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/type-checking-ast.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/__init__.py
--rw-r--r--   0        0        0     9335 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/example_google_docstring.py
--rw-r--r--   0        0        0      362 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/stuff1.py
--rw-r--r--   0        0        0      121 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_bases/__init__.py
--rw-r--r--   0        0        0       20 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_bases/base.py
--rw-r--r--   0        0        0      169 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_instvar_combination.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_prepare/__init__.py
--rw-r--r--   0        0        0      355 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_prepare/instvar.py
--rw-r--r--   0        0        0       89 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/Foo.py
--rw-r--r--   0        0        0       21 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/__init__.py
--rw-r--r--   0        0        0       75 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/a.py
--rw-r--r--   0        0        0       27 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/b.py
--rw-r--r--   0        0        0       37 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/single.py
--rw-r--r--   0        0        0      217 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/variable_is_typealias.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/foo.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/foo.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion1.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion1.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion2/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/stubalone.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/__init__.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/a.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/a.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/stubalone.pyi
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub.pyi
--rw-r--r--   0        0        0     2232 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/__init__.py
--rw-r--r--   0        0        0       41 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/api.py
--rw-r--r--   0        0        0       66 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/namespace/foo.py
--rw-r--r--   0        0        0      132 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.py
--rw-r--r--   0        0        0      630 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.pyi
--rw-r--r--   0        0        0      888 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/nopyi.py
--rw-r--r--   0        0        0      478 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/relative.py
--rw-r--r--   0        0        0       80 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/typing.py
--rw-r--r--   0        0        0       19 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/__init__.py
--rw-r--r--   0        0        0      780 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.py
--rw-r--r--   0        0        0      867 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.pyi
--rw-r--r--   0        0        0       92 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/util.py
--rw-r--r--   0        0        0      458 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/__init__.py
--rw-r--r--   0        0        0      757 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/_sample.py
--rw-r--r--   0        0        0       34 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/inter.py
--rw-r--r--   0        0        0      161 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/typing.py
--rw-r--r--   0        0        0       33 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/__init__.py
--rw-r--r--   0        0        0     1606 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_analyzer.py
--rw-r--r--   0        0        0     9140 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/test_analyzers/test_definitionfinder.py
--rw-r--r--   0        0        0      665 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_unparse_ann.py
--rw-r--r--   0        0        0     2266 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_utils.py
--rw-r--r--   0        0        0     5306 2023-02-04 07:42:44.759251 nb-autodoc-1.0.0a6/tests/test_annotation.py
--rw-r--r--   0        0        0        0 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_docstringparser/__init__.py
--rw-r--r--   0        0        0     5330 2023-06-21 14:08:14.903902 nb-autodoc-1.0.0a6/tests/test_docstringparser/test_google.py
--rw-r--r--   0        0        0     8952 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_manager.py
--rw-r--r--   0        0        0     2102 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_modulefinder.py
--rw-r--r--   0        0        0     6607 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/test_utils.py
--rw-r--r--   0        0        0      738 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/utils.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 nb-autodoc-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-11-24 06:50:23.530000 nb-autodoc-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     1743 2023-06-21 15:24:35.307767 nb-autodoc-1.0.0a7/README.md
+-rw-r--r--   0        0        0       86 2023-06-23 15:04:46.237475 nb-autodoc-1.0.0a7/nb_autodoc/__init__.py
+-rw-r--r--   0        0        0     1318 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a7/nb_autodoc/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/__init__.py
+-rw-r--r--   0        0        0     2791 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/analyzer.py
+-rw-r--r--   0        0        0      484 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/base.py
+-rw-r--r--   0        0        0    12841 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/definitionfinder.py
+-rw-r--r--   0        0        0     5697 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/unparse_ann.py
+-rw-r--r--   0        0        0    10475 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a7/nb_autodoc/analyzers/utils.py
+-rw-r--r--   0        0        0    15331 2023-03-22 10:11:28.688069 nb-autodoc-1.0.0a7/nb_autodoc/annotation.py
+-rw-r--r--   0        0        0     7597 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/builders/__init__.py
+-rw-r--r--   0        0        0      406 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/builders/helpers.py
+-rw-r--r--   0        0        0    26266 2023-05-05 09:04:38.574920 nb-autodoc-1.0.0a7/nb_autodoc/builders/markdown.py
+-rw-r--r--   0        0        0     2478 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a7/nb_autodoc/config.py
+-rw-r--r--   0        0        0       83 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/docstringparser/__init__.py
+-rw-r--r--   0        0        0    15491 2023-06-23 14:16:25.329077 nb-autodoc-1.0.0a7/nb_autodoc/docstringparser/google.py
+-rw-r--r--   0        0        0     1991 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/log.py
+-rw-r--r--   0        0        0    33670 2023-05-05 09:07:44.174879 nb-autodoc-1.0.0a7/nb_autodoc/manager.py
+-rw-r--r--   0        0        0    15796 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/modulefinder.py
+-rw-r--r--   0        0        0     4512 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/nb_autodoc/nodes.py
+-rw-r--r--   0        0        0        0 2022-10-10 09:23:09.200000 nb-autodoc-1.0.0a7/nb_autodoc/py.typed
+-rw-r--r--   0        0        0     1396 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a7/nb_autodoc/typing.py
+-rw-r--r--   0        0        0     8599 2023-03-22 10:06:52.428169 nb-autodoc-1.0.0a7/nb_autodoc/utils.py
+-rw-r--r--   0        0        0     1228 2023-03-22 08:53:54.029767 nb-autodoc-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/analyzerdata/assigndata-override-ast.py
+-rw-r--r--   0        0        0      203 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/analyzerdata/exec_type_checking.py
+-rw-r--r--   0        0        0      169 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a7/tests/analyzerdata/extract-docstring.py
+-rw-r--r--   0        0        0      380 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/analyzerdata/overload.py
+-rw-r--r--   0        0        0     1286 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/analyzerdata/simple-definition-ast.py
+-rw-r--r--   0        0        0      342 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/analyzerdata/type-checking-ast.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/data/__init__.py
+-rw-r--r--   0        0        0     9335 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/data/example_google_docstring.py
+-rw-r--r--   0        0        0      362 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/data/stuff1.py
+-rw-r--r--   0        0        0      121 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/class_bases/__init__.py
+-rw-r--r--   0        0        0       20 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/class_bases/base.py
+-rw-r--r--   0        0        0      169 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/class_instvar_combination.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/class_prepare/__init__.py
+-rw-r--r--   0        0        0      355 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/class_prepare/instvar.py
+-rw-r--r--   0        0        0       89 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/get_canonical_member/Foo.py
+-rw-r--r--   0        0        0       21 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/get_canonical_member/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/get_canonical_member/a.py
+-rw-r--r--   0        0        0       27 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/get_canonical_member/b.py
+-rw-r--r--   0        0        0       37 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/single.py
+-rw-r--r--   0        0        0      217 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/managerdata/variable_is_typealias.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/foo.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/foo.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/simplenamespace/portion1.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/simplenamespace/portion1.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/simplenamespace/portion2/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/stubalone.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub/a.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub/a.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub/stubalone.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/modulefinderdata/simplepkg/sub.pyi
+-rw-r--r--   0        0        0     2232 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/api.py
+-rw-r--r--   0        0        0       66 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/namespace/foo.py
+-rw-r--r--   0        0        0      132 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/overload/__init__.py
+-rw-r--r--   0        0        0      630 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/overload/__init__.pyi
+-rw-r--r--   0        0        0      888 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a7/tests/simple_pkg/overload/nopyi.py
+-rw-r--r--   0        0        0      478 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/overload/relative.py
+-rw-r--r--   0        0        0       80 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/overload/typing.py
+-rw-r--r--   0        0        0       19 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/__init__.py
+-rw-r--r--   0        0        0      780 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/fuzz.py
+-rw-r--r--   0        0        0      867 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/fuzz.pyi
+-rw-r--r--   0        0        0       92 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/util.py
+-rw-r--r--   0        0        0      458 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/reexport/__init__.py
+-rw-r--r--   0        0        0      757 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/reexport/_sample.py
+-rw-r--r--   0        0        0       34 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/reexport/inter.py
+-rw-r--r--   0        0        0      161 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/simple_pkg/typing.py
+-rw-r--r--   0        0        0       33 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_analyzers/__init__.py
+-rw-r--r--   0        0        0     1606 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_analyzers/test_analyzer.py
+-rw-r--r--   0        0        0     9140 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a7/tests/test_analyzers/test_definitionfinder.py
+-rw-r--r--   0        0        0      665 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_analyzers/test_unparse_ann.py
+-rw-r--r--   0        0        0     2266 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_analyzers/test_utils.py
+-rw-r--r--   0        0        0     5306 2023-02-04 07:42:44.759251 nb-autodoc-1.0.0a7/tests/test_annotation.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_docstringparser/__init__.py
+-rw-r--r--   0        0        0     7649 2023-06-23 14:21:03.048925 nb-autodoc-1.0.0a7/tests/test_docstringparser/test_google.py
+-rw-r--r--   0        0        0     8952 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_manager.py
+-rw-r--r--   0        0        0     2102 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/test_modulefinder.py
+-rw-r--r--   0        0        0     6607 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a7/tests/test_utils.py
+-rw-r--r--   0        0        0      738 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a7/tests/utils.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 nb-autodoc-1.0.0a7/PKG-INFO
```

### Comparing `nb-autodoc-1.0.0a6/LICENSE` & `nb-autodoc-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/README.md` & `nb-autodoc-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/__main__.py` & `nb-autodoc-1.0.0a7/nb_autodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/analyzer.py` & `nb-autodoc-1.0.0a7/nb_autodoc/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/definitionfinder.py` & `nb-autodoc-1.0.0a7/nb_autodoc/analyzers/definitionfinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/unparse_ann.py` & `nb-autodoc-1.0.0a7/nb_autodoc/analyzers/unparse_ann.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/utils.py` & `nb-autodoc-1.0.0a7/nb_autodoc/analyzers/utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/annotation.py` & `nb-autodoc-1.0.0a7/nb_autodoc/annotation.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/builders/__init__.py` & `nb-autodoc-1.0.0a7/nb_autodoc/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/builders/markdown.py` & `nb-autodoc-1.0.0a7/nb_autodoc/builders/markdown.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/config.py` & `nb-autodoc-1.0.0a7/nb_autodoc/config.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/google.py` & `nb-autodoc-1.0.0a7/nb_autodoc/docstringparser/google.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,22 +188,32 @@
             descr = self.line.strip()
             if obj is not None:
                 obj.descr = descr
             self.col = 0
             self.lineno += 1
         descr_chunk = []
         breaked = False
+        merging_short = True
+        line_count = 0
         for i in range(self.lineno, len(self.lines)):
             line = self.lines[i]
+            line_count += 1
+            if include_short and not line.strip() and merging_short:
+                merging_short = False
+                continue
             if line and len(line) - len(line.lstrip()) < least_indent:
                 breaked = True
+                line_count -= 1
                 break
+            if include_short and merging_short and obj is not None:
+                obj.descr += " " + line.strip()
+                continue
             descr_chunk.append(line)
         if breaked:
-            self.lineno += len(descr_chunk)
+            self.lineno += line_count
         else:
             self.lineno = len(self.lines) - 1  # move to ending
         long_descr = dedent("\n".join(descr_chunk)).strip()
         if obj is not None:
             obj.long_descr = long_descr
         return descr_chunk
```

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/log.py` & `nb-autodoc-1.0.0a7/nb_autodoc/log.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/manager.py` & `nb-autodoc-1.0.0a7/nb_autodoc/manager.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/modulefinder.py` & `nb-autodoc-1.0.0a7/nb_autodoc/modulefinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/nodes.py` & `nb-autodoc-1.0.0a7/nb_autodoc/nodes.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/typing.py` & `nb-autodoc-1.0.0a7/nb_autodoc/typing.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/nb_autodoc/utils.py` & `nb-autodoc-1.0.0a7/nb_autodoc/utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/pyproject.toml` & `nb-autodoc-1.0.0a7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "documentation-tool",
     "markdown",
 ]
 dependencies = [
     "typing-extensions>=4.0",
     "click==8.*",
 ]
-version = "1.0.0a6"
+version = "1.0.0a7"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 
 [project.urls]
```

### Comparing `nb-autodoc-1.0.0a6/tests/analyzerdata/simple-definition-ast.py` & `nb-autodoc-1.0.0a7/tests/analyzerdata/simple-definition-ast.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/data/example_google_docstring.py` & `nb-autodoc-1.0.0a7/tests/data/example_google_docstring.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/__init__.py` & `nb-autodoc-1.0.0a7/tests/simple_pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.pyi` & `nb-autodoc-1.0.0a7/tests/simple_pkg/overload/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/overload/nopyi.py` & `nb-autodoc-1.0.0a7/tests/simple_pkg/overload/nopyi.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.py` & `nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/fuzz.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.pyi` & `nb-autodoc-1.0.0a7/tests/simple_pkg/pyi/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/_sample.py` & `nb-autodoc-1.0.0a7/tests/simple_pkg/reexport/_sample.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_analyzers/test_analyzer.py` & `nb-autodoc-1.0.0a7/tests/test_analyzers/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_analyzers/test_definitionfinder.py` & `nb-autodoc-1.0.0a7/tests/test_analyzers/test_definitionfinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_analyzers/test_unparse_ann.py` & `nb-autodoc-1.0.0a7/tests/test_analyzers/test_unparse_ann.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_analyzers/test_utils.py` & `nb-autodoc-1.0.0a7/tests/test_analyzers/test_utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_annotation.py` & `nb-autodoc-1.0.0a7/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_docstringparser/test_google.py` & `nb-autodoc-1.0.0a7/tests/test_docstringparser/test_google.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nb_autodoc.docstringparser.google import GoogleStyleParser
-from nb_autodoc.nodes import Args, ColonArg, Docstring, Returns, Role, Text
+from nb_autodoc.nodes import Args, ColonArg, Docstring, Returns, Role, Text, Raises
 from nb_autodoc.utils import cleandoc
 
 
 class TestGoogleStyleParser:
     def test_parse_common(self):
         parse = lambda doc: GoogleStyleParser(doc).parse()
         assert parse(" ") == Docstring(
@@ -166,7 +166,80 @@
                         roles=[],
                         descr="descr",
                         long_descr="",
                     ),
                 ),
             ],
         )
+
+    def test_combined_colonarg_short_description(self):
+        parse = lambda doc: GoogleStyleParser(doc).parse()
+        doc = cleandoc(
+            """
+            Args:
+                arg: short
+                    short descr.
+                arg2: short
+                    short descr.
+
+                    long
+                    long descr.
+                arg3: short descr.
+
+                    long descr.
+            Raises:
+                ValueError: short
+                    short descr.
+
+                    long
+                    long descr.
+            """
+        )
+        assert parse(doc) == Docstring(
+            roles=[],
+            annotation=None,
+            descr="",
+            long_descr="",
+            sections=[
+                Args(
+                    name="Args",
+                    args=[
+                        ColonArg(
+                            name="arg",
+                            annotation=None,
+                            roles=[],
+                            descr="short short descr.",
+                            long_descr="",
+                        ),
+                        ColonArg(
+                            name="arg2",
+                            annotation=None,
+                            roles=[],
+                            descr="short short descr.",
+                            long_descr="long\nlong descr.",
+                        ),
+                        ColonArg(
+                            name="arg3",
+                            annotation=None,
+                            roles=[],
+                            descr="short descr.",
+                            long_descr="long descr.",
+                        ),
+                    ],
+                    vararg=None,
+                    kwonlyargs=[],
+                    kwarg=None,
+                ),
+                Raises(
+                    name="Raises",
+                    args=[
+                        ColonArg(
+                            name=None,
+                            annotation="ValueError",
+                            roles=[],
+                            descr="short short descr.",
+                            long_descr="long\nlong descr.",
+                        )
+                    ],
+                ),
+            ],
+        )
```

### Comparing `nb-autodoc-1.0.0a6/tests/test_manager.py` & `nb-autodoc-1.0.0a7/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_modulefinder.py` & `nb-autodoc-1.0.0a7/tests/test_modulefinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/test_utils.py` & `nb-autodoc-1.0.0a7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/tests/utils.py` & `nb-autodoc-1.0.0a7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a6/PKG-INFO` & `nb-autodoc-1.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-autodoc
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Python API documentation tool supporting the modern PEPs and typing features.
 License: MIT
 Keywords: nonebot,autodoc,apidoc,documentation-tool,markdown
 Author-email: iyume <iyumelive@gmail.com>
 Requires-Python: >=3.8
 Project-URL: homepage, https://github.com/nonebot/nb-autodoc
 Project-URL: repository, https://github.com/nonebot/nb-autodoc
```

