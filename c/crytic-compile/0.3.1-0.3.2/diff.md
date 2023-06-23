# Comparing `tmp/crytic-compile-0.3.1.tar.gz` & `tmp/crytic-compile-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crytic-compile-0.3.1.tar", last modified: Fri Mar 17 18:19:47 2023, max compression
+gzip compressed data, was "crytic-compile-0.3.2.tar", last modified: Fri Jun 23 16:19:02 2023, max compression
```

## Comparing `crytic-compile-0.3.1.tar` & `crytic-compile-0.3.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.124442 crytic-compile-0.3.1/
--rw-r--r--   0 monty      (501) staff       (20)    34523 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/LICENSE
--rw-r--r--   0 monty      (501) staff       (20)     2068 2023-03-17 18:19:47.124306 crytic-compile-0.3.1/PKG-INFO
--rw-r--r--   0 monty      (501) staff       (20)     1795 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/README.md
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.118072 crytic-compile-0.3.1/crytic_compile/
--rw-r--r--   0 monty      (501) staff       (20)      251 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/__init__.py
--rw-r--r--   0 monty      (501) staff       (20)     7841 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/__main__.py
--rw-r--r--   0 monty      (501) staff       (20)     8822 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/compilation_unit.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.119132 crytic-compile-0.3.1/crytic_compile/compiler/
--rw-r--r--   0 monty      (501) staff       (20)        0 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/compiler/__init__.py
--rw-r--r--   0 monty      (501) staff       (20)     1502 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/compiler/compiler.py
--rw-r--r--   0 monty      (501) staff       (20)    23384 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/crytic_compile.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.119511 crytic-compile-0.3.1/crytic_compile/cryticparser/
--rw-r--r--   0 monty      (501) staff       (20)       66 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/cryticparser/__init__.py
--rwxr-xr-x   0 monty      (501) staff       (20)    15605 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/cryticparser/cryticparser.py
--rwxr-xr-x   0 monty      (501) staff       (20)     1618 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/cryticparser/defaults.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.122412 crytic-compile-0.3.1/crytic_compile/platform/
--rw-r--r--   0 monty      (501) staff       (20)       87 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/platform/__init__.py
--rw-r--r--   0 monty      (501) staff       (20)     5257 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/abstract_platform.py
--rw-r--r--   0 monty      (501) staff       (20)      503 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/platform/all_export.py
--rw-r--r--   0 monty      (501) staff       (20)      521 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/platform/all_platforms.py
--rw-r--r--   0 monty      (501) staff       (20)     5145 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/archive.py
--rwxr-xr-x   0 monty      (501) staff       (20)     8396 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/brownie.py
--rwxr-xr-x   0 monty      (501) staff       (20)     9545 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/buidler.py
--rwxr-xr-x   0 monty      (501) staff       (20)     8643 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/dapp.py
--rwxr-xr-x   0 monty      (501) staff       (20)     9800 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/embark.py
--rwxr-xr-x   0 monty      (501) staff       (20)     8283 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/etherlime.py
--rw-r--r--   0 monty      (501) staff       (20)    16717 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/etherscan.py
--rw-r--r--   0 monty      (501) staff       (20)      172 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/platform/exceptions.py
--rwxr-xr-x   0 monty      (501) staff       (20)     4149 2023-02-17 13:20:38.000000 crytic-compile-0.3.1/crytic_compile/platform/foundry.py
--rwxr-xr-x   0 monty      (501) staff       (20)    12354 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/hardhat.py
--rw-r--r--   0 monty      (501) staff       (20)    28511 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/solc.py
--rw-r--r--   0 monty      (501) staff       (20)    14790 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/solc_standard_json.py
--rw-r--r--   0 monty      (501) staff       (20)    20727 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/standard.py
--rwxr-xr-x   0 monty      (501) staff       (20)    18597 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/truffle.py
--rw-r--r--   0 monty      (501) staff       (20)     1597 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/platform/types.py
--rw-r--r--   0 monty      (501) staff       (20)     7187 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/vyper.py
--rwxr-xr-x   0 monty      (501) staff       (20)    13403 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/platform/waffle.py
--rw-r--r--   0 monty      (501) staff       (20)        0 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/py.typed
--rw-r--r--   0 monty      (501) staff       (20)    21585 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/source_unit.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.123916 crytic-compile-0.3.1/crytic_compile/utils/
--rw-r--r--   0 monty      (501) staff       (20)        0 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/utils/__init__.py
--rw-r--r--   0 monty      (501) staff       (20)        0 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/utils/name_collision.py
--rw-r--r--   0 monty      (501) staff       (20)     4895 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/utils/naming.py
--rw-r--r--   0 monty      (501) staff       (20)     5923 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/utils/natspec.py
--rw-r--r--   0 monty      (501) staff       (20)     1342 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/utils/npm.py
--rw-r--r--   0 monty      (501) staff       (20)     2222 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/crytic_compile/utils/subprocess.py
--rw-r--r--   0 monty      (501) staff       (20)      953 2022-05-31 09:08:21.000000 crytic-compile-0.3.1/crytic_compile/utils/unit_tests.py
--rw-r--r--   0 monty      (501) staff       (20)     2074 2023-03-17 18:17:46.000000 crytic-compile-0.3.1/crytic_compile/utils/zip.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.118884 crytic-compile-0.3.1/crytic_compile.egg-info/
--rw-r--r--   0 monty      (501) staff       (20)     2068 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/PKG-INFO
--rw-r--r--   0 monty      (501) staff       (20)     1689 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/SOURCES.txt
--rw-r--r--   0 monty      (501) staff       (20)        1 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/dependency_links.txt
--rw-r--r--   0 monty      (501) staff       (20)       64 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/entry_points.txt
--rw-r--r--   0 monty      (501) staff       (20)      110 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/requires.txt
--rw-r--r--   0 monty      (501) staff       (20)       15 2023-03-17 18:19:47.000000 crytic-compile-0.3.1/crytic_compile.egg-info/top_level.txt
--rw-r--r--   0 monty      (501) staff       (20)      645 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/pyproject.toml
--rw-r--r--   0 monty      (501) staff       (20)       38 2023-03-17 18:19:47.124488 crytic-compile-0.3.1/setup.cfg
--rw-r--r--   0 monty      (501) staff       (20)      888 2023-03-17 18:19:40.000000 crytic-compile-0.3.1/setup.py
-drwxr-xr-x   0 monty      (501) staff       (20)        0 2023-03-17 18:19:47.124076 crytic-compile-0.3.1/tests/
--rw-r--r--   0 monty      (501) staff       (20)    17669 2023-02-17 13:18:41.000000 crytic-compile-0.3.1/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compilation_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/crytic_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile/cryticparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15605 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/cryticparser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/cryticparser/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/crytic_compile/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/abstract_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/all_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/all_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8496 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/brownie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/buidler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8641 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/dapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10118 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/embark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8281 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/etherlime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/foundry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12109 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/hardhat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/solc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/solc_standard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18595 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/truffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/vyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13587 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/platform/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/source_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/crytic_compile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/name_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/crytic_compile/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.838333 crytic-compile-0.3.2/crytic_compile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 16:19:02.000000 crytic-compile-0.3.2/crytic_compile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:19:02.842333 crytic-compile-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-23 16:18:53.000000 crytic-compile-0.3.2/tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.1/LICENSE` & `crytic-compile-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/PKG-INFO` & `crytic-compile-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.1
+Version: 0.3.2
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # Crytic-compile
 [![Build Status](https://img.shields.io/github/workflow/status/crytic/crytic-compile/CI/master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
 [![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
```

### Comparing `crytic-compile-0.3.1/README.md` & `crytic-compile-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/__main__.py` & `crytic-compile-0.3.2/crytic_compile/__main__.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/compilation_unit.py` & `crytic-compile-0.3.2/crytic_compile/compilation_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Each compilation unit represents a call to the compiler
 Each compilation unit has one or more source units associated with it
 At least one compilation unit exists for each version of solc used
     Maybe more dependending on the framework used (hardhat/foundry/etc)
 """
 import uuid
 from collections import defaultdict
-from typing import TYPE_CHECKING, Dict, Set, Optional
+from typing import TYPE_CHECKING, Dict, List, Set, Optional
 
 from crytic_compile.compiler.compiler import CompilerVersion
 from crytic_compile.source_unit import SourceUnit
 from crytic_compile.utils.naming import Filename
 
 # Cycle dependency
 if TYPE_CHECKING:
@@ -32,15 +32,15 @@
         # mapping from filename to contract name
         self._filename_to_contracts: Dict[Filename, Set[str]] = defaultdict(set)
 
         # mapping from filename to source unit
         self._source_units: Dict[Filename, SourceUnit] = {}
 
         # set containing all the filenames of this compilation unit
-        self._filenames: Set[Filename] = set()
+        self._filenames: List[Filename] = []
 
         # mapping from absolute/relative/used to filename
         self._filenames_lookup: Optional[Dict[str, Filename]] = None
 
         # compiler.compiler
         self._compiler_version: CompilerVersion = CompilerVersion(
             compiler="N/A", version="N/A", optimized=False
@@ -110,49 +110,52 @@
         }
 
     def create_source_unit(self, filename: Filename) -> SourceUnit:
         """
         Create the source unit associated with the filename
         Add the relevant info in the compilation unit/crytic compile
         If the source unit already exist, return it
+        Also appends filename to the end of filenames, if not already present
+        So this function should be called in the order you want filenames to have
 
         Args:
             filename (Filename): filename of the source unit
 
         Returns:
             SourceUnit: the source unit
         """
         if not filename in self._source_units:
             source_unit = SourceUnit(self, filename)  # type: ignore
-            self.filenames.add(filename)
             self._source_units[filename] = source_unit
+            if filename not in self.filenames:
+                self.filenames.append(filename)
         return self._source_units[filename]
 
     # endregion
     ###################################################################################
     ###################################################################################
     # region Filenames
     ###################################################################################
     ###################################################################################
 
     @property
-    def filenames(self) -> Set[Filename]:
+    def filenames(self) -> List[Filename]:
         """Return the filenames used by the compilation unit
 
         Returns:
-            Set[Filename]: Filenames used by the compilation units
+            list[Filename]: Filenames used by the compilation units
         """
         return self._filenames
 
     @filenames.setter
-    def filenames(self, all_filenames: Set[Filename]) -> None:
+    def filenames(self, all_filenames: List[Filename]) -> None:
         """Set the filenames
 
         Args:
-            all_filenames (Set[Filename]): new filenames
+            all_filenames (List[Filename]): new filenames
         """
         self._filenames = all_filenames
 
     @property
     def filename_to_contracts(self) -> Dict[Filename, Set[str]]:
         """Return a dict mapping the filename to a list of contract declared
```

### Comparing `crytic-compile-0.3.1/crytic_compile/compiler/compiler.py` & `crytic-compile-0.3.2/crytic_compile/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/crytic_compile.py` & `crytic-compile-0.3.2/crytic_compile/crytic_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,19 +171,19 @@
     ###################################################################################
     @property
     def filenames(self) -> Set[Filename]:
         """
         Return the set of all the filenames used
 
         Returns:
-             Set[Filename]: list of filenames
+             Set[Filename]: set of filenames
         """
         filenames: Set[Filename] = set()
         for compile_unit in self._compilation_units.values():
-            filenames = filenames.union(compile_unit.filenames)
+            filenames |= set(compile_unit.filenames)
         return filenames
 
     def filename_lookup(self, filename: str) -> Filename:
         """Return a crytic_compile.naming.Filename from a any filename
 
         Args:
             filename (str): filename (used/absolute/relative)
@@ -562,15 +562,18 @@
     def _run_custom_build(custom_build: str) -> None:
         """Run a custom build
 
         Args:
             custom_build (str): Command to run
         """
         cmd = custom_build.split(" ")
-
+        LOGGER.info(
+            "'%s' running",
+            " ".join(cmd),
+        )
         with subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as process:
             stdout_bytes, stderr_bytes = process.communicate()
             stdout, stderr = (
                 stdout_bytes.decode(errors="backslashreplace"),
                 stderr_bytes.decode(errors="backslashreplace"),
             )  # convert bytestrings to unicode strings
 
@@ -659,10 +662,10 @@
                 standard_json.add_source_file(filename)
             compilations.append(CryticCompile(standard_json, **kwargs))
         else:
             # We compile each file and add it to our compilations.
             for filename in filenames:
                 compilations.append(CryticCompile(filename, **kwargs))
     else:
-        raise ValueError(f"Unresolved target: {str(target)}")
+        raise ValueError(f"{str(target)} is not a file or directory.")
 
     return compilations
```

### Comparing `crytic-compile-0.3.1/crytic_compile/cryticparser/cryticparser.py` & `crytic-compile-0.3.2/crytic_compile/cryticparser/cryticparser.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/cryticparser/defaults.py` & `crytic-compile-0.3.2/crytic_compile/cryticparser/defaults.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/abstract_platform.py` & `crytic-compile-0.3.2/crytic_compile/platform/abstract_platform.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/all_platforms.py` & `crytic-compile-0.3.2/crytic_compile/platform/all_platforms.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/archive.py` & `crytic-compile-0.3.2/crytic_compile/platform/archive.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/brownie.py` & `crytic-compile-0.3.2/crytic_compile/platform/brownie.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
             "ignore_compile", False
         )
 
         base_cmd = ["brownie"]
 
         if not brownie_ignore_compile:
             cmd = base_cmd + ["compile"]
+            LOGGER.info(
+                "'%s' running",
+                " ".join(cmd),
+            )
             try:
                 with subprocess.Popen(
                     cmd,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=self._target,
                     executable=shutil.which(cmd[0]),
@@ -177,15 +181,15 @@
             source_unit = compilation_unit.create_source_unit(filename)
 
             source_unit.ast = target_loaded["ast"]
             contract_name = target_loaded["contractName"]
 
             compilation_unit.filename_to_contracts[filename].add(contract_name)
 
-            source_unit.contracts_names.add(contract_name)
+            source_unit.add_contract_name(contract_name)
             source_unit.abis[contract_name] = target_loaded["abi"]
             source_unit.bytecodes_init[contract_name] = target_loaded["bytecode"].replace("0x", "")
             source_unit.bytecodes_runtime[contract_name] = target_loaded[
                 "deployedBytecode"
             ].replace("0x", "")
             source_unit.srcmaps_init[contract_name] = target_loaded["sourceMap"].split(";")
             source_unit.srcmaps_runtime[contract_name] = target_loaded["deployedSourceMap"].split(
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/buidler.py` & `crytic-compile-0.3.2/crytic_compile/platform/buidler.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,34 @@
         skip_filename = compilation_unit.compiler_version.version in [
             f"0.4.{x}" for x in range(0, 10)
         ]
 
         with open(target_solc_file, encoding="utf8") as file_desc:
             targets_json = json.load(file_desc)
 
+            if "sources" in targets_json:
+                for path, info in targets_json["sources"].items():
+
+                    if path.startswith("ontracts/") and not skip_directory_name_fix:
+                        path = "c" + path
+
+                    if skip_filename:
+                        path = convert_filename(
+                            self._target,
+                            relative_to_short,
+                            crytic_compile,
+                            working_dir=buidler_working_dir,
+                        )
+                    else:
+                        path = convert_filename(
+                            path, relative_to_short, crytic_compile, working_dir=buidler_working_dir
+                        )
+                    source_unit = compilation_unit.create_source_unit(path)
+                    source_unit.ast = info["ast"]
+
             if "contracts" in targets_json:
                 for original_filename, contracts_info in targets_json["contracts"].items():
                     filename = convert_filename(
                         original_filename,
                         relative_to_short,
                         crytic_compile,
                         working_dir=buidler_working_dir,
@@ -126,15 +146,15 @@
 
                         if (
                             original_filename.startswith("ontracts/")
                             and not skip_directory_name_fix
                         ):
                             original_filename = "c" + original_filename
 
-                        source_unit.contracts_names.add(contract_name)
+                        source_unit.add_contract_name(contract_name)
                         compilation_unit.filename_to_contracts[filename].add(contract_name)
 
                         source_unit.abis[contract_name] = info["abi"]
                         source_unit.bytecodes_init[contract_name] = info["evm"]["bytecode"][
                             "object"
                         ]
                         source_unit.bytecodes_runtime[contract_name] = info["evm"][
@@ -147,34 +167,14 @@
                             "deployedBytecode"
                         ]["sourceMap"].split(";")
                         userdoc = info.get("userdoc", {})
                         devdoc = info.get("devdoc", {})
                         natspec = Natspec(userdoc, devdoc)
                         source_unit.natspec[contract_name] = natspec
 
-            if "sources" in targets_json:
-                for path, info in targets_json["sources"].items():
-
-                    if path.startswith("ontracts/") and not skip_directory_name_fix:
-                        path = "c" + path
-
-                    if skip_filename:
-                        path = convert_filename(
-                            self._target,
-                            relative_to_short,
-                            crytic_compile,
-                            working_dir=buidler_working_dir,
-                        )
-                    else:
-                        path = convert_filename(
-                            path, relative_to_short, crytic_compile, working_dir=buidler_working_dir
-                        )
-                    source_unit = compilation_unit.create_source_unit(path)
-                    source_unit.ast = info["ast"]
-
     def clean(self, **kwargs: str) -> None:
         # TODO: call "buldler clean"?
         pass
 
     @staticmethod
     def is_supported(target: str, **kwargs: str) -> bool:
         """Check if the target is a buidler project
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/dapp.py` & `crytic-compile-0.3.2/crytic_compile/platform/dapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,21 @@
         with open(os.path.join(directory, "dapp.sol.json"), "r", encoding="utf8") as file_desc:
             targets_json = json.load(file_desc)
 
             version: Optional[str] = None
             if "version" in targets_json:
                 version = re.findall(r"\d+\.\d+\.\d+", targets_json["version"])[0]
 
+            for path, info in targets_json["sources"].items():
+                path = convert_filename(
+                    path, _relative_to_short, crytic_compile, working_dir=self._target
+                )
+                source_unit = compilation_unit.create_source_unit(path)
+                source_unit.ast = info["ast"]
+
             for original_filename, contracts_info in targets_json["contracts"].items():
 
                 filename = convert_filename(
                     original_filename, lambda x: x, crytic_compile, self._target
                 )
 
                 source_unit = compilation_unit.create_source_unit(filename)
@@ -83,15 +90,15 @@
                         if (
                             "settings" in metadata
                             and "optimizer" in metadata["settings"]
                             and "enabled" in metadata["settings"]["optimizer"]
                         ):
                             optimized |= metadata["settings"]["optimizer"]["enabled"]
                     contract_name = extract_name(original_contract_name)
-                    source_unit.contracts_names.add(contract_name)
+                    source_unit.add_contract_name(contract_name)
                     compilation_unit.filename_to_contracts[filename].add(contract_name)
 
                     source_unit.abis[contract_name] = info["abi"]
                     source_unit.bytecodes_init[contract_name] = info["evm"]["bytecode"]["object"]
                     source_unit.bytecodes_runtime[contract_name] = info["evm"]["deployedBytecode"][
                         "object"
                     ]
@@ -106,21 +113,14 @@
                     natspec = Natspec(userdoc, devdoc)
                     source_unit.natspec[contract_name] = natspec
 
                     if version is None:
                         metadata = json.loads(info["metadata"])
                         version = re.findall(r"\d+\.\d+\.\d+", metadata["compiler"]["version"])[0]
 
-            for path, info in targets_json["sources"].items():
-                path = convert_filename(
-                    path, _relative_to_short, crytic_compile, working_dir=self._target
-                )
-                source_unit = compilation_unit.create_source_unit(path)
-                source_unit.ast = info["ast"]
-
         compilation_unit.compiler_version = CompilerVersion(
             compiler="solc", version=version, optimized=optimized
         )
 
     def clean(self, **kwargs: str) -> None:
         """Clean compilation artifacts
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/embark.py` & `crytic-compile-0.3.2/crytic_compile/platform/embark.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,23 @@
             )
         compilation_unit = CompilationUnit(crytic_compile, str(self._target))
 
         compilation_unit.compiler_version = _get_version(self._target)
 
         with open(infile, "r", encoding="utf8") as file_desc:
             targets_loaded = json.load(file_desc)
+
+            if "sources" in targets_loaded:
+                compilation_unit.filenames = [
+                    convert_filename(
+                        path, _relative_to_short, crytic_compile, working_dir=self._target
+                    )
+                    for path in targets_loaded["sources"]
+                ]
+
             for k, ast in targets_loaded["asts"].items():
                 filename = convert_filename(
                     k, _relative_to_short, crytic_compile, working_dir=self._target
                 )
                 source_unit = compilation_unit.create_source_unit(filename)
                 source_unit.ast = ast
 
@@ -143,15 +152,15 @@
                     crytic_compile,
                     working_dir=self._target,
                 )
 
                 source_unit = compilation_unit.create_source_unit(filename)
 
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
 
                 if "abi" in info:
                     source_unit.abis[contract_name] = info["abi"]
                 if "bin" in info:
                     source_unit.bytecodes_init[contract_name] = info["bin"].replace("0x", "")
                 if "bin-runtime" in info:
                     source_unit.bytecodes_runtime[contract_name] = info["bin-runtime"].replace(
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/etherlime.py` & `crytic-compile-0.3.2/crytic_compile/platform/etherlime.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
                 source_unit = compilation_unit.create_source_unit(filename)
 
                 source_unit.ast = target_loaded["ast"]
                 contract_name = target_loaded["contractName"]
 
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
                 source_unit.abis[contract_name] = target_loaded["abi"]
                 source_unit.bytecodes_init[contract_name] = target_loaded["bytecode"].replace(
                     "0x", ""
                 )
                 source_unit.bytecodes_runtime[contract_name] = target_loaded[
                     "deployedBytecode"
                 ].replace("0x", "")
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/etherscan.py` & `crytic-compile-0.3.2/crytic_compile/platform/etherscan.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     "arbi:": (".arbiscan.io", "arbiscan.io"),
     "testnet.arbi:": ("-testnet.arbiscan.io", "testnet.arbiscan.io"),
     "poly:": (".polygonscan.com", "polygonscan.com"),
     "mumbai:": ("-testnet.polygonscan.com", "testnet.polygonscan.com"),
     "avax:": (".snowtrace.io", "snowtrace.io"),
     "testnet.avax:": ("-testnet.snowtrace.io", "testnet.snowtrace.io"),
     "ftm:": (".ftmscan.com", "ftmscan.com"),
+    "goerli.base:": ("-goerli.basescan.org", "goerli.basescan.org"),
 }
 
 
 def _handle_bytecode(crytic_compile: "CryticCompile", target: str, result_b: bytes) -> None:
     """Parse the bytecode and populate CryticCompile info
 
     Args:
@@ -74,32 +75,29 @@
 
     contract_filename = Filename(absolute="", relative="", short="", used="")
 
     compilation_unit = CompilationUnit(crytic_compile, str(target))
 
     source_unit = compilation_unit.create_source_unit(contract_filename)
 
-    source_unit.contracts_names.add(contract_name)
+    source_unit.add_contract_name(contract_name)
     compilation_unit.filename_to_contracts[contract_filename].add(contract_name)
     source_unit.abis[contract_name] = {}
     source_unit.bytecodes_init[contract_name] = bytecode
     source_unit.bytecodes_runtime[contract_name] = ""
     source_unit.srcmaps_init[contract_name] = []
     source_unit.srcmaps_runtime[contract_name] = []
 
     compilation_unit.compiler_version = CompilerVersion(
         compiler="unknown", version="", optimized=False
     )
 
     crytic_compile.bytecode_only = True
 
 
-# def _etherscan_single_file():
-
-
 def _handle_single_file(
     source_code: str, addr: str, prefix: Optional[str], contract_name: str, export_dir: str
 ) -> str:
     """Handle a result with a single file
 
     Args:
         source_code (str): source code
@@ -120,26 +118,29 @@
         file_desc.write(source_code)
 
     return filename
 
 
 def _handle_multiple_files(
     dict_source_code: Dict, addr: str, prefix: Optional[str], contract_name: str, export_dir: str
-) -> Tuple[List[str], str]:
+) -> Tuple[List[str], str, Optional[List[str]]]:
     """Handle a result with a multiple files. Generate multiple Solidity files
 
     Args:
         dict_source_code (Dict): dict result from etherscan
         addr (str): contract address
         prefix (Optional[str]): used to separate different chains
         contract_name (str): contract name
         export_dir (str): directory where the code will be saved
 
     Returns:
         Tuple[List[str], str]: filesnames, directory, where target_filename is the main file
+
+    Raises:
+        IOError: if the path is outside of the allowed directory
     """
     if prefix:
         directory = os.path.join(export_dir, f"{addr}{prefix}-{contract_name}")
     else:
         directory = os.path.join(export_dir, f"{addr}-{contract_name}")
 
     if "sources" in dict_source_code:
@@ -148,14 +149,18 @@
     else:
         # or etherscan might return an object with contract names as keys
         source_codes = dict_source_code
 
     filtered_paths: List[str] = []
     for filename, source_code in source_codes.items():
         path_filename = PurePosixPath(filename)
+        # Only keep solidity files
+        if path_filename.suffix not in [".sol", ".vy"]:
+            continue
+
         # https://etherscan.io/address/0x19bb64b80cbf61e61965b0e5c2560cc7364c6546#code has an import of erc721a/contracts/ERC721A.sol
         # if the full path is lost then won't compile
         if "contracts" == path_filename.parts[0] and not filename.startswith("@"):
             path_filename = PurePosixPath(
                 *path_filename.parts[path_filename.parts.index("contracts") :]
             )
 
@@ -165,20 +170,27 @@
         # We need to make sure this is relative, so that Path(directory, ...) remains anchored to directory
         if path_filename.is_absolute():
             path_filename = PurePosixPath(*path_filename.parts[1:])
 
         filtered_paths.append(path_filename.as_posix())
         path_filename_disk = Path(directory, path_filename)
 
+        allowed_path = os.path.abspath(directory)
+        if os.path.commonpath((allowed_path, os.path.abspath(path_filename_disk))) != allowed_path:
+            raise IOError(
+                f"Path '{path_filename_disk}' is outside of the allowed directory: {allowed_path}"
+            )
         if not os.path.exists(path_filename_disk.parent):
             os.makedirs(path_filename_disk.parent)
         with open(path_filename_disk, "w", encoding="utf8") as file_desc:
             file_desc.write(source_code["content"])
 
-    return list(filtered_paths), directory
+    remappings = dict_source_code.get("settings", {}).get("remappings", None)
+
+    return list(filtered_paths), directory, _sanitize_remappings(remappings, directory)
 
 
 class Etherscan(AbstractPlatform):
     """
     Etherscan platform
     """
 
@@ -257,30 +269,35 @@
             etherscan_bytecode_url += f"&apikey={optim_api_key}"
 
         source_code: str = ""
         result: Dict[str, Union[bool, str, int]] = {}
         contract_name: str = ""
 
         if not only_bytecode:
-            if "polygon" in etherscan_url:
+            if "polygon" in etherscan_url or "basescan" in etherscan_url:
                 # build object with headers, then send request
                 new_etherscan_url = urllib.request.Request(
                     etherscan_url, headers={"User-Agent": "Mozilla/5.0"}
                 )
                 with urllib.request.urlopen(new_etherscan_url) as response:
                     html = response.read()
             else:
                 with urllib.request.urlopen(etherscan_url) as response:
                     html = response.read()
 
             info = json.loads(html)
 
-            if "result" in info and info["result"] == "Max rate limit reached":
+            if (
+                "result" in info
+                and "rate limit reached" in info["result"]
+                and "message" in info
+                and info["message"] == "NOTOK"
+            ):
                 LOGGER.error("Etherscan API rate limit exceeded")
-                raise InvalidCompilation("Etherscan api rate limit exceeded")
+                raise InvalidCompilation("Etherscan API rate limit exceeded")
 
             if "message" not in info:
                 LOGGER.error("Incorrect etherscan request")
                 raise InvalidCompilation("Incorrect etherscan request " + etherscan_url)
 
             if not info["message"].startswith("OK"):
                 LOGGER.error("Contract has no public source code")
@@ -319,33 +336,40 @@
         # Assert to help mypy
         assert isinstance(result["CompilerVersion"], str)
 
         compiler_version = re.findall(
             r"\d+\.\d+\.\d+", _convert_version(result["CompilerVersion"])
         )[0]
 
+        # etherscan can report "default" which is not a valid EVM version
+        evm_version: Optional[str] = None
+        if "EVMVersion" in result:
+            assert isinstance(result["EVMVersion"], str)
+            evm_version = result["EVMVersion"] if result["EVMVersion"] != "Default" else None
+
         optimization_used: bool = result["OptimizationUsed"] == "1"
 
         optimize_runs = None
         if optimization_used:
             optimize_runs = int(result["Runs"])
 
         working_dir: Optional[str] = None
+        remappings: Optional[List[str]] = None
 
         try:
             # etherscan might return an object with two curly braces, {{ content }}
             dict_source_code = json.loads(source_code[1:-1])
-            filenames, working_dir = _handle_multiple_files(
+            filenames, working_dir, remappings = _handle_multiple_files(
                 dict_source_code, addr, prefix, contract_name, export_dir
             )
         except JSONDecodeError:
             try:
                 # or etherscan might return an object with single curly braces, { content }
                 dict_source_code = json.loads(source_code)
-                filenames, working_dir = _handle_multiple_files(
+                filenames, working_dir, remappings = _handle_multiple_files(
                     dict_source_code, addr, prefix, contract_name, export_dir
                 )
             except JSONDecodeError:
                 filenames = [
                     _handle_single_file(source_code, addr, prefix, contract_name, export_dir)
                 ]
 
@@ -354,16 +378,21 @@
         compilation_unit.compiler_version = CompilerVersion(
             compiler=kwargs.get("solc", "solc"),
             version=compiler_version,
             optimized=optimization_used,
             optimize_runs=optimize_runs,
         )
         compilation_unit.compiler_version.look_for_installed_version()
-
-        solc_standard_json.standalone_compile(filenames, compilation_unit, working_dir=working_dir)
+        solc_standard_json.standalone_compile(
+            filenames,
+            compilation_unit,
+            working_dir=working_dir,
+            remappings=remappings,
+            evm_version=evm_version,
+        )
 
     def clean(self, **_kwargs: str) -> None:
         pass
 
     @staticmethod
     def is_supported(target: str, **kwargs: str) -> bool:
         """Check if the target is a etherscan project
@@ -410,17 +439,48 @@
 
     Returns:
         str: converted version
     """
     return version[1 : version.find("+")]
 
 
-def _relative_to_short(relative: Path) -> Path:
-    """Translate relative path to short (do nothing for etherscan)
+def _sanitize_remappings(
+    remappings: Optional[List[str]], allowed_directory: str
+) -> Optional[List[str]]:
+    """Sanitize a list of remappings
 
     Args:
-        relative (Path): path to the target
+        remappings: (Optional[List[str]]): a list of remappings
+        allowed_directory: the allowed base directory for remaps
 
     Returns:
-        Path: Translated path
+        Optional[List[str]]: a list of sanitized remappings
     """
-    return relative
+
+    if remappings is None:
+        return remappings
+
+    allowed_path = os.path.abspath(allowed_directory)
+
+    remappings_clean: List[str] = []
+    for r in remappings:
+        split = r.split("=", 2)
+        if len(split) != 2:
+            LOGGER.warning("Invalid remapping %s", r)
+            continue
+
+        origin, dest = split[0], PurePosixPath(split[1])
+
+        # if path is absolute, relativize it
+        if dest.is_absolute():
+            dest = PurePosixPath(*dest.parts[1:])
+
+        dest_disk = Path(allowed_directory, dest)
+
+        if os.path.commonpath((allowed_path, os.path.abspath(dest_disk))) != allowed_path:
+            LOGGER.warning("Remapping %s=%s is potentially unsafe, skipping", origin, dest)
+            continue
+
+        # always use a trailing slash for the destination
+        remappings_clean.append(f"{origin}={str(dest / '_')[:-1]}")
+
+    return remappings_clean
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/foundry.py` & `crytic-compile-0.3.2/crytic_compile/platform/foundry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
-Truffle platform
+Foundry platform
 """
 import logging
 import os
-import shutil
-import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, List
 
 from crytic_compile.platform.abstract_platform import AbstractPlatform
 from crytic_compile.platform.types import Type
 from crytic_compile.platform.hardhat import hardhat_like_parsing
 from crytic_compile.utils.subprocess import run
@@ -47,43 +45,22 @@
 
         if ignore_compile:
             LOGGER.info(
                 "--ignore-compile used, if something goes wrong, consider removing the ignore compile flag"
             )
 
         if not ignore_compile:
-            cmd = [
-                "forge",
-                "build",
-                "--build-info",
-                "--force",
-            ]
-
-            LOGGER.info(
-                "'%s' running",
-                " ".join(cmd),
-            )
-
-            with subprocess.Popen(
-                cmd,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
+            run(
+                [
+                    "forge",
+                    "build",
+                    "--build-info",
+                ],
                 cwd=self._target,
-                executable=shutil.which(cmd[0]),
-            ) as process:
-
-                stdout_bytes, stderr_bytes = process.communicate()
-                stdout, stderr = (
-                    stdout_bytes.decode(errors="backslashreplace"),
-                    stderr_bytes.decode(errors="backslashreplace"),
-                )  # convert bytestrings to unicode strings
-
-                LOGGER.info(stdout)
-                if stderr:
-                    LOGGER.error(stderr)
+            )
 
         build_directory = Path(
             self._target,
             out_directory,
             "build-info",
         )
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/hardhat.py` & `crytic-compile-0.3.2/crytic_compile/platform/hardhat.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,20 +41,26 @@
         build_directory: build directory
         working_dir: working directory
 
     Raises:
         InvalidCompilation: If hardhat failed to run
 
     """
+    if not os.path.isdir(build_directory):
+        txt = (
+            f"Compilation failed. Can you run build command?\n{build_directory} is not a directory."
+        )
+        raise InvalidCompilation(txt)
+
     files = sorted(
         os.listdir(build_directory), key=lambda x: os.path.getmtime(Path(build_directory, x))
     )
     files = [str(f) for f in files if str(f).endswith(".json")]
     if not files:
-        txt = f"`compile` failed. Can you run it?\n{build_directory} is empty"
+        txt = f"Compilation failed. Can you run build command?\n{build_directory} is empty."
         raise InvalidCompilation(txt)
 
     for file in files:
         build_info = Path(build_directory, file)
 
         # The file here should always ends .json, but just in case use ife
         uniq_id = file if ".json" not in file else file[0:-5]
@@ -74,14 +80,38 @@
                 compiler=compiler, version=version_from_config, optimized=optimized
             )
 
             skip_filename = compilation_unit.compiler_version.version in [
                 f"0.4.{x}" for x in range(0, 10)
             ]
 
+            if "sources" in targets_json:
+                for path, info in targets_json["sources"].items():
+                    if skip_filename:
+                        path = convert_filename(
+                            target,
+                            relative_to_short,
+                            crytic_compile,
+                            working_dir=working_dir,
+                        )
+                    else:
+                        path = convert_filename(
+                            path,
+                            relative_to_short,
+                            crytic_compile,
+                            working_dir=working_dir,
+                        )
+
+                    source_unit = compilation_unit.create_source_unit(path)
+                    source_unit.ast = info.get("ast", info.get("legacyAST"))
+                    if source_unit.ast is None:
+                        raise InvalidCompilation(
+                            f"AST not found for {path} in {build_info} directory"
+                        )
+
             if "contracts" in targets_json:
                 for original_filename, contracts_info in targets_json["contracts"].items():
 
                     filename = convert_filename(
                         original_filename,
                         relative_to_short,
                         crytic_compile,
@@ -89,15 +119,15 @@
                     )
 
                     source_unit = compilation_unit.create_source_unit(filename)
 
                     for original_contract_name, info in contracts_info.items():
                         contract_name = extract_name(original_contract_name)
 
-                        source_unit.contracts_names.add(contract_name)
+                        source_unit.add_contract_name(contract_name)
                         compilation_unit.filename_to_contracts[filename].add(contract_name)
 
                         source_unit.abis[contract_name] = info["abi"]
                         source_unit.bytecodes_init[contract_name] = info["evm"]["bytecode"][
                             "object"
                         ]
                         source_unit.bytecodes_runtime[contract_name] = info["evm"][
@@ -110,34 +140,14 @@
                             "deployedBytecode"
                         ]["sourceMap"].split(";")
                         userdoc = info.get("userdoc", {})
                         devdoc = info.get("devdoc", {})
                         natspec = Natspec(userdoc, devdoc)
                         source_unit.natspec[contract_name] = natspec
 
-            if "sources" in targets_json:
-                for path, info in targets_json["sources"].items():
-                    if skip_filename:
-                        path = convert_filename(
-                            target,
-                            relative_to_short,
-                            crytic_compile,
-                            working_dir=working_dir,
-                        )
-                    else:
-                        path = convert_filename(
-                            path,
-                            relative_to_short,
-                            crytic_compile,
-                            working_dir=working_dir,
-                        )
-
-                    source_unit = compilation_unit.create_source_unit(path)
-                    source_unit.ast = info["ast"]
-
 
 class Hardhat(AbstractPlatform):
     """
     Hardhat platform
     """
 
     NAME = "Hardhat"
@@ -164,37 +174,15 @@
             "build-info",
         )
 
         hardhat_working_dir = str(Path(self._target, detected_paths["root"]))
 
         if not hardhat_ignore_compile:
             cmd = base_cmd + ["compile", "--force"]
-
-            LOGGER.info(
-                "'%s' running",
-                " ".join(cmd),
-            )
-
-            with subprocess.Popen(
-                cmd,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                cwd=self._target,
-                executable=shutil.which(cmd[0]),
-            ) as process:
-
-                stdout_bytes, stderr_bytes = process.communicate()
-                stdout, stderr = (
-                    stdout_bytes.decode(errors="backslashreplace"),
-                    stderr_bytes.decode(errors="backslashreplace"),
-                )  # convert bytestrings to unicode strings
-
-                LOGGER.info(stdout)
-                if stderr:
-                    LOGGER.error(stderr)
+            run(cmd, cwd=self._target)
 
         hardhat_like_parsing(crytic_compile, self._target, build_directory, hardhat_working_dir)
 
     def clean(self, **kwargs: str) -> None:
         """Clean compilation artifacts
 
         Args:
@@ -296,15 +284,15 @@
 
         if args.get("hardhat_artifacts_directory", None):
             override_paths["artifacts"] = Path(target_path, args["hardhat_artifacts_directory"])
 
         if args.get("hardhat_working_dir", None):
             override_paths["root"] = Path(target_path, args["hardhat_working_dir"])
 
-        print_paths = "console.log(JSON.stringify(config.paths))"
+        print_paths = "console.log(JSON.stringify(config.paths));process.exit()"
 
         try:
             config_str = self._run_hardhat_console(base_cmd, print_paths)
             paths = json.loads(config_str or "{}")
             return {**default_paths, **paths, **override_paths}
         except ValueError as e:
             LOGGER.info("Problem deserializing hardhat configuration, using defaults: %s", e)
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/solc.py` & `crytic-compile-0.3.2/crytic_compile/platform/solc.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,21 +72,14 @@
     """
     contracts = _build_contract_data(compilation_unit)
 
     # Create additional informational objects.
     sources = {filename: {"AST": ast} for (filename, ast) in compilation_unit.asts.items()}
     source_list = [x.absolute for x in compilation_unit.filenames]
 
-    # needed for Echidna, see https://github.com/crytic/crytic-compile/issues/112
-    first_source_list = list(filter(lambda f: "@" in f, source_list))
-    second_source_list = list(filter(lambda f: "@" not in f, source_list))
-    first_source_list.sort()
-    second_source_list.sort()
-    source_list = first_source_list + second_source_list
-
     # Create our root object to contain the contracts and other information.
     output = {"sources": sources, "sourceList": source_list, "contracts": contracts}
 
     # If we have an export directory specified, we output the JSON.
     if export_dir:
         if not os.path.exists(export_dir):
             os.makedirs(export_dir)
@@ -159,18 +152,14 @@
         if force_legacy_json and _is_at_or_above_minor_version(compilation_unit, 8):
             raise InvalidCompilation("legacy JSON not supported from 0.8.x onwards")
 
         skip_filename = compilation_unit.compiler_version.version in [
             f"0.4.{x}" for x in range(0, 10)
         ]
 
-        solc_handle_contracts(
-            targets_json, skip_filename, compilation_unit, self._target, solc_working_dir
-        )
-
         if "sources" in targets_json:
             for path, info in targets_json["sources"].items():
                 if skip_filename:
                     path = convert_filename(
                         self._target,
                         relative_to_short,
                         crytic_compile,
@@ -179,14 +168,18 @@
                 else:
                     path = convert_filename(
                         path, relative_to_short, crytic_compile, working_dir=solc_working_dir
                     )
                 source_unit = compilation_unit.create_source_unit(path)
                 source_unit.ast = info["AST"]
 
+        solc_handle_contracts(
+            targets_json, skip_filename, compilation_unit, self._target, solc_working_dir
+        )
+
     def clean(self, **_kwargs: str) -> None:
         """Clean compilation artifacts
 
         Args:
             **_kwargs: unused.
         """
         return
@@ -330,15 +323,15 @@
                     relative_to_short,
                     compilation_unit.crytic_compile,
                     working_dir=solc_working_dir,
                 )
 
             source_unit = compilation_unit.create_source_unit(filename)
 
-            source_unit.contracts_names.add(contract_name)
+            source_unit.add_contract_name(contract_name)
             compilation_unit.filename_to_contracts[filename].add(contract_name)
             source_unit.abis[contract_name] = (
                 json.loads(info["abi"]) if not is_above_0_8 else info["abi"]
             )
             source_unit.bytecodes_init[contract_name] = info["bin"]
             source_unit.bytecodes_runtime[contract_name] = info["bin-runtime"]
             source_unit.srcmaps_init[contract_name] = info["srcmap"].split(";")
@@ -374,14 +367,18 @@
         InvalidCompilation: If solc failed to run
 
     Returns:
         str: Returns the version of the provided solc executable.
     """
 
     cmd = [solc, "--version"]
+    LOGGER.info(
+        "'%s' running",
+        " ".join(cmd),
+    )
     try:
         with subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             env=env,
             executable=shutil.which(cmd[0]),
@@ -443,15 +440,15 @@
         return "abi,ast,bin,bin-runtime,srcmap,srcmap-runtime,userdoc,devdoc,hashes"
     if compiler_version.version in explicit_compact_format:
         return "abi,ast,bin,bin-runtime,srcmap,srcmap-runtime,userdoc,devdoc,hashes,compact-format"
 
     return "abi,ast,bin,bin-runtime,srcmap,srcmap-runtime,userdoc,devdoc,hashes"
 
 
-# pylint: disable=too-many-arguments,too-many-locals,too-many-branches
+# pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements
 def _run_solc(
     compilation_unit: "CompilationUnit",
     filename: str,
     solc: str,
     solc_disable_warnings: bool,
     solc_arguments: Optional[str],
     solc_remaps: Optional[Union[str, List[str]]] = None,
@@ -470,26 +467,33 @@
         solc_arguments (Optional[str]): Additional solc cli arguments
         solc_remaps (Optional[Union[str, List[str]]], optional): Solc remaps. Can be a string where remap are separated with space, or list of str, or a list of. Defaults to None.
         env (Optional[Dict]): Environement variable when solc is run. Defaults to None.
         working_dir (Optional[Union[Path, str]]): Working directory when solc is run. Defaults to None.
         force_legacy_json (bool): Force to use the legacy json format. Defaults to False.
 
     Raises:
-        InvalidCompilation: If solc faile to run
+        InvalidCompilation: If solc failed to run or file is not a solidity file
 
     Returns:
         Dict: Json compilation artifacts
     """
     if not os.path.isfile(filename) and (
         not working_dir or not os.path.isfile(os.path.join(str(working_dir), filename))
     ):
-        raise InvalidCompilation(f"{filename} does not exist (are you in the correct directory?)")
+        if os.path.isdir(filename):
+            raise InvalidCompilation(
+                f"{filename} is a directory. Expected a Solidity file when not using a compilation framework."
+            )
+
+        raise InvalidCompilation(
+            f"{filename} does not exist. Are you in the correct working directory?"
+        )
 
     if not filename.endswith(".sol"):
-        raise InvalidCompilation("Incorrect file format")
+        raise InvalidCompilation(f"{filename} is not the expected format '.sol'")
 
     compilation_unit.compiler_version = CompilerVersion(
         compiler="solc", version=get_version(solc, env), optimized=is_optimized(solc_arguments)
     )
 
     compiler_version = compilation_unit.compiler_version
     assert compiler_version
@@ -513,24 +517,34 @@
         solc_args = [item.strip() for sublist in solc_args_ for item in sublist if item]
         cmd += solc_args
 
     additional_kwargs: Dict = {"cwd": working_dir} if working_dir else {}
     if not compiler_version.version in [f"0.4.{x}" for x in range(0, 11)]:
         # Add . as default allowed path
         if "--allow-paths" not in cmd:
-            relative_filepath = filename
+            file_dir_start = os.path.normpath(os.path.dirname(filename))
+            file_dir = os.path.abspath(file_dir_start)
+            if "," in file_dir:
+                try:
+                    file_dir = os.path.relpath(file_dir_start)
+                except ValueError:
+                    pass
 
-            if not working_dir:
-                working_dir = os.getcwd()
-
-            if relative_filepath.startswith(str(working_dir)):
-                relative_filepath = relative_filepath[len(str(working_dir)) + 1 :]
+            if "," not in file_dir:
+                cmd += ["--allow-paths", ".," + file_dir]
+            else:
+                LOGGER.warning(
+                    "Solc filepath contains a comma; omitting the --allow-paths argument. This may result in failed imports.\n"
+                )
 
-            cmd += ["--allow-paths", ".", relative_filepath]
     try:
+        LOGGER.info(
+            "'%s' running",
+            " ".join(cmd),
+        )
         # pylint: disable=consider-using-with
         if env:
             process = subprocess.Popen(
                 cmd,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 executable=shutil.which(cmd[0]),
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/solc_standard_json.py` & `crytic-compile-0.3.2/crytic_compile/platform/solc_standard_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 if TYPE_CHECKING:
     from crytic_compile import CryticCompile
 
 LOGGER = logging.getLogger("CryticCompile")
 
 
 def standalone_compile(
-    filenames: List[str], compilation_unit: CompilationUnit, working_dir: Optional[str] = None
+    filenames: List[str],
+    compilation_unit: CompilationUnit,
+    working_dir: Optional[str] = None,
+    remappings: Optional[List[str]] = None,
+    evm_version: Optional[str] = None,
 ) -> None:
     """
     Boilerplate function to run the the standardjson. compilation_unit.compiler_version must be set before calling this function
 
     Example of usage:
         compilation_unit = CompilationUnit(crytic_compile, name_target)
         compilation_unit.compiler_version = CompilerVersion(
@@ -38,14 +42,16 @@
         )
         standalone_compile(filenames_to_compile, compilation_unit
 
     Args:
         filenames (List[str]): list of the files to compile
         compilation_unit (CompilationUnit): compilation unit object to populate
         working_dir (Optional[str]): working directory
+        remappings (Optional[List[str]]): list of solc remaps to use
+        evm_version (Optional[str]): EVM version to target. None for default
 
     Returns:
 
     """
 
     if compilation_unit.compiler_version.version == "N/A":
         LOGGER.error("The compiler version of the compilation unit must be set")
@@ -53,14 +59,21 @@
 
     standard_json_dict: Dict = {}
     build_standard_json_default(standard_json_dict)
 
     for filename in filenames:
         add_source_file(standard_json_dict, filename)
 
+    if remappings is not None:
+        for remap in remappings:
+            add_remapping(standard_json_dict, remap)
+
+    if evm_version is not None:
+        add_evm_version(standard_json_dict, evm_version)
+
     add_optimization(
         standard_json_dict,
         compilation_unit.compiler_version.optimized,
         compilation_unit.compiler_version.optimize_runs,
     )
 
     targets_json = run_solc_standard_json(
@@ -138,14 +151,18 @@
     additional_kwargs: Dict = {"cwd": working_dir} if working_dir else {}
 
     env = dict(os.environ)
     if compiler_version.version:
         env["SOLC_VERSION"] = compiler_version.version
 
     stderr = ""
+    LOGGER.info(
+        "'%s' running",
+        " ".join(cmd),
+    )
     try:
 
         with subprocess.Popen(
             cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
@@ -239,14 +256,32 @@
         json_dict["settings"]["optimizer"] = {"enabled": True}
         if optimize_runs:
             json_dict["settings"]["optimizer"]["runs"] = optimize_runs
         return
     json_dict["settings"]["optimizer"] = {"enabled": False}
 
 
+def add_evm_version(json_dict: Dict, version: str) -> None:
+    """
+    Add the version of the EVM to compile for.
+
+    Can be one of the following values: homestead, tangerineWhistle,
+    spuriousDragon, byzantium, constantinople, petersburg, istanbul,
+    berlin, london or paris
+
+    Args:
+        json_dict (Dict): solc standard json input
+        version (str): the EVM version to target
+
+    Returns:
+
+    """
+    json_dict["settings"]["evmVersion"] = version
+
+
 def parse_standard_json_output(
     targets_json: Dict, compilation_unit: CompilationUnit, solc_working_dir: Optional[str] = None
 ) -> None:
     """
     Parse the targets_json output from solc, and populate compilation_unit accordingly
 
 
@@ -257,14 +292,34 @@
 
     Returns:
 
     """
 
     skip_filename = compilation_unit.compiler_version.version in [f"0.4.{x}" for x in range(0, 10)]
 
+    if "sources" in targets_json:
+        for path, info in targets_json["sources"].items():
+            if skip_filename:
+                path = convert_filename(
+                    path,
+                    relative_to_short,
+                    compilation_unit.crytic_compile,
+                    working_dir=solc_working_dir,
+                )
+            else:
+                path = convert_filename(
+                    path,
+                    relative_to_short,
+                    compilation_unit.crytic_compile,
+                    working_dir=solc_working_dir,
+                )
+            source_unit = compilation_unit.create_source_unit(path)
+
+            source_unit.ast = info.get("ast")
+
     if "contracts" in targets_json:
         for file_path, file_contracts in targets_json["contracts"].items():
             for contract_name, info in file_contracts.items():
                 # for solc < 0.4.10 we cant retrieve the filename from the ast
                 if skip_filename:
                     filename = convert_filename(
                         file_path,
@@ -278,15 +333,15 @@
                         relative_to_short,
                         compilation_unit.crytic_compile,
                         working_dir=solc_working_dir,
                     )
 
                 source_unit = compilation_unit.create_source_unit(filename)
 
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
                 source_unit.abis[contract_name] = info["abi"]
 
                 userdoc = info.get("userdoc", {})
                 devdoc = info.get("devdoc", {})
                 natspec = Natspec(userdoc, devdoc)
                 source_unit.natspec[contract_name] = natspec
@@ -298,34 +353,14 @@
                 source_unit.srcmaps_init[contract_name] = info["evm"]["bytecode"][
                     "sourceMap"
                 ].split(";")
                 source_unit.srcmaps_runtime[contract_name] = info["evm"]["deployedBytecode"][
                     "sourceMap"
                 ].split(";")
 
-    if "sources" in targets_json:
-        for path, info in targets_json["sources"].items():
-            if skip_filename:
-                path = convert_filename(
-                    path,
-                    relative_to_short,
-                    compilation_unit.crytic_compile,
-                    working_dir=solc_working_dir,
-                )
-            else:
-                path = convert_filename(
-                    path,
-                    relative_to_short,
-                    compilation_unit.crytic_compile,
-                    working_dir=solc_working_dir,
-                )
-            source_unit = compilation_unit.create_source_unit(path)
-
-            source_unit.ast = info.get("ast")
-
 
 # Inherits is_dependency/is_supported from Solc
 class SolcStandardJson(Solc):
     """
     Represent the Standard solc Json object
     """
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/standard.py` & `crytic-compile-0.3.2/crytic_compile/platform/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,20 +281,32 @@
     """
     compilation_unit = CompilationUnit(crytic_compile, "legacy")
     compilation_unit.compiler_version = CompilerVersion(
         compiler=loaded_json["compiler"]["compiler"],
         version=loaded_json["compiler"]["version"],
         optimized=loaded_json["compiler"]["optimized"],
     )
+
+    if "filenames" in loaded_json:
+        compilation_unit.filenames = [
+            _convert_dict_to_filename(filename) for filename in loaded_json["filenames"]
+        ]
+
+    for path, ast in loaded_json["asts"].items():
+        # The following might create lookup issue?
+        filename = crytic_compile.filename_lookup(path)
+        source_unit = compilation_unit.create_source_unit(filename)
+        source_unit.ast = ast
+
     for contract_name, contract in loaded_json["contracts"].items():
         filename = _convert_dict_to_filename(contract["filenames"])
         compilation_unit.filename_to_contracts[filename].add(contract_name)
         source_unit = compilation_unit.create_source_unit(filename)
 
-        source_unit.contracts_names.add(contract_name)
+        source_unit.add_contract_name(contract_name)
         source_unit.abis[contract_name] = contract["abi"]
         source_unit.bytecodes_init[contract_name] = contract["bin"]
         source_unit.bytecodes_runtime[contract_name] = contract["bin-runtime"]
         source_unit.srcmaps_init[contract_name] = contract["srcmap"].split(";")
         source_unit.srcmaps_runtime[contract_name] = contract["srcmap-runtime"].split(";")
         source_unit.libraries[contract_name] = contract["libraries"]
 
@@ -304,31 +316,14 @@
 
         if contract["is_dependency"]:
             compilation_unit.crytic_compile.dependencies.add(filename.absolute)
             compilation_unit.crytic_compile.dependencies.add(filename.relative)
             compilation_unit.crytic_compile.dependencies.add(filename.short)
             compilation_unit.crytic_compile.dependencies.add(filename.used)
 
-    if "filenames" in loaded_json:
-        compilation_unit.filenames = {
-            _convert_dict_to_filename(filename) for filename in loaded_json["filenames"]
-        }
-    else:
-        # For legay code, we recover the filenames from the contracts list
-        # This is not perfect, as a filename might not be associated to any contract
-        for contract_name, contract in loaded_json["contracts"].items():
-            filename = _convert_dict_to_filename(contract["filenames"])
-            compilation_unit.filenames.add(filename)
-
-    for path, ast in loaded_json["asts"].items():
-        # The following might create lookup issue?
-        filename = crytic_compile.filename_lookup(path)
-        source_unit = compilation_unit.create_source_unit(filename)
-        source_unit.ast = ast
-
 
 def _load_from_compile_legacy2(crytic_compile: "CryticCompile", loaded_json: Dict) -> None:
     """Load from old (old) export
 
     Args:
         crytic_compile (CryticCompile): CryticCompile object to populate
         loaded_json (Dict): Json representation of the CryticCompile object
@@ -337,26 +332,39 @@
     for key, compilation_unit_json in loaded_json["compilation_units"].items():
         compilation_unit = CompilationUnit(crytic_compile, key)
         compilation_unit.compiler_version = CompilerVersion(
             compiler=compilation_unit_json["compiler"]["compiler"],
             version=compilation_unit_json["compiler"]["version"],
             optimized=compilation_unit_json["compiler"]["optimized"],
         )
+
+        if "filenames" in compilation_unit_json:
+            compilation_unit.filenames = [
+                _convert_dict_to_filename(filename)
+                for filename in compilation_unit_json["filenames"]
+            ]
+
+        for path, ast in loaded_json["asts"].items():
+            # The following might create lookup issue?
+            filename = crytic_compile.filename_lookup(path)
+            source_unit = compilation_unit.create_source_unit(filename)
+            source_unit.ast = ast
+
         for contract_name, contract in compilation_unit_json["contracts"].items():
 
             filename = Filename(
                 absolute=contract["filenames"]["absolute"],
                 relative=contract["filenames"]["relative"],
                 short=contract["filenames"]["short"],
                 used=contract["filenames"]["used"],
             )
             compilation_unit.filename_to_contracts[filename].add(contract_name)
 
             source_unit = compilation_unit.create_source_unit(filename)
-            source_unit.contracts_names.add(contract_name)
+            source_unit.add_contract_name(contract_name)
             source_unit.abis[contract_name] = contract["abi"]
             source_unit.bytecodes_init[contract_name] = contract["bin"]
             source_unit.bytecodes_runtime[contract_name] = contract["bin-runtime"]
             source_unit.srcmaps_init[contract_name] = contract["srcmap"].split(";")
             source_unit.srcmaps_runtime[contract_name] = contract["srcmap-runtime"].split(";")
             source_unit.libraries[contract_name] = contract["libraries"]
 
@@ -366,53 +374,46 @@
 
             if contract["is_dependency"]:
                 crytic_compile.dependencies.add(filename.absolute)
                 crytic_compile.dependencies.add(filename.relative)
                 crytic_compile.dependencies.add(filename.short)
                 crytic_compile.dependencies.add(filename.used)
 
-        if "filenames" in compilation_unit_json:
-            compilation_unit.filenames = {
-                _convert_dict_to_filename(filename)
-                for filename in compilation_unit_json["filenames"]
-            }
-        else:
-            # For legacy code, we recover the filenames from the contracts list
-            # This is not perfect, as a filename might not be associated to any contract
-            for contract_name, contract in compilation_unit_json["contracts"].items():
-                filename = _convert_dict_to_filename(contract["filenames"])
-                compilation_unit.filenames.add(filename)
-
-        for path, ast in loaded_json["asts"].items():
-            # The following might create lookup issue?
-            filename = crytic_compile.filename_lookup(path)
-            source_unit = compilation_unit.create_source_unit(filename)
-            source_unit.ast = ast
-
 
 def _load_from_compile_0_0_1(crytic_compile: "CryticCompile", loaded_json: Dict) -> None:
     for key, compilation_unit_json in loaded_json["compilation_units"].items():
         compilation_unit = CompilationUnit(crytic_compile, key)
         compilation_unit.compiler_version = CompilerVersion(
             compiler=compilation_unit_json["compiler"]["compiler"],
             version=compilation_unit_json["compiler"]["version"],
             optimized=compilation_unit_json["compiler"]["optimized"],
         )
+
+        compilation_unit.filenames = [
+            _convert_dict_to_filename(filename) for filename in compilation_unit_json["filenames"]
+        ]
+
+        for path, ast in compilation_unit_json["asts"].items():
+            # The following might create lookup issue?
+            filename = crytic_compile.filename_lookup(path)
+            source_unit = compilation_unit.create_source_unit(filename)
+            source_unit.ast = ast
+
         for contracts_data in compilation_unit_json["contracts"].values():
             for contract_name, contract in contracts_data.items():
 
                 filename = Filename(
                     absolute=contract["filenames"]["absolute"],
                     relative=contract["filenames"]["relative"],
                     short=contract["filenames"]["short"],
                     used=contract["filenames"]["used"],
                 )
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
                 source_unit = compilation_unit.create_source_unit(filename)
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
                 source_unit.abis[contract_name] = contract["abi"]
                 source_unit.bytecodes_init[contract_name] = contract["bin"]
                 source_unit.bytecodes_runtime[contract_name] = contract["bin-runtime"]
                 source_unit.srcmaps_init[contract_name] = contract["srcmap"].split(";")
                 source_unit.srcmaps_runtime[contract_name] = contract["srcmap-runtime"].split(";")
                 source_unit.libraries[contract_name] = contract["libraries"]
 
@@ -422,47 +423,37 @@
 
                 if contract["is_dependency"]:
                     crytic_compile.dependencies.add(filename.absolute)
                     crytic_compile.dependencies.add(filename.relative)
                     crytic_compile.dependencies.add(filename.short)
                     crytic_compile.dependencies.add(filename.used)
 
-        compilation_unit.filenames = {
-            _convert_dict_to_filename(filename) for filename in compilation_unit_json["filenames"]
-        }
-
-        for path, ast in compilation_unit_json["asts"].items():
-            # The following might create lookup issue?
-            filename = crytic_compile.filename_lookup(path)
-            source_unit = compilation_unit.create_source_unit(filename)
-            source_unit.ast = ast
-
 
 def _load_from_compile_current(crytic_compile: "CryticCompile", loaded_json: Dict) -> None:
     for key, compilation_unit_json in loaded_json["compilation_units"].items():
         compilation_unit = CompilationUnit(crytic_compile, key)
         compilation_unit.compiler_version = CompilerVersion(
             compiler=compilation_unit_json["compiler"]["compiler"],
             version=compilation_unit_json["compiler"]["version"],
             optimized=compilation_unit_json["compiler"]["optimized"],
         )
 
-        compilation_unit.filenames = {
+        compilation_unit.filenames = [
             _convert_dict_to_filename(filename) for filename in compilation_unit_json["filenames"]
-        }
+        ]
 
         for filename_str, source_unit_data in compilation_unit_json["source_units"].items():
             filename = compilation_unit.filename_lookup(filename_str)
             source_unit = compilation_unit.create_source_unit(filename)
 
             for contract_name, contract in source_unit_data.get("contracts", {}).items():
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
 
                 source_unit = compilation_unit.create_source_unit(filename)
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
                 source_unit.abis[contract_name] = contract["abi"]
                 source_unit.bytecodes_init[contract_name] = contract["bin"]
                 source_unit.bytecodes_runtime[contract_name] = contract["bin-runtime"]
                 source_unit.srcmaps_init[contract_name] = contract["srcmap"].split(";")
                 source_unit.srcmaps_runtime[contract_name] = contract["srcmap-runtime"].split(";")
                 source_unit.libraries[contract_name] = contract["libraries"]
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/truffle.py` & `crytic-compile-0.3.2/crytic_compile/platform/truffle.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
                 source_unit = compilation_unit.create_source_unit(filename)
 
                 source_unit.ast = target_loaded["ast"]
 
                 contract_name = target_loaded["contractName"]
                 source_unit.natspec[contract_name] = natspec
                 compilation_unit.filename_to_contracts[filename].add(contract_name)
-                source_unit.contracts_names.add(contract_name)
+                source_unit.add_contract_name(contract_name)
                 source_unit.abis[contract_name] = target_loaded["abi"]
                 source_unit.bytecodes_init[contract_name] = target_loaded["bytecode"].replace(
                     "0x", ""
                 )
                 source_unit.bytecodes_runtime[contract_name] = target_loaded[
                     "deployedBytecode"
                 ].replace("0x", "")
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/types.py` & `crytic-compile-0.3.2/crytic_compile/platform/types.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/vyper.py` & `crytic-compile-0.3.2/crytic_compile/platform/vyper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Vyper platform
 """
 import json
+import logging
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from crytic_compile.compilation_unit import CompilationUnit
@@ -17,14 +18,16 @@
 
 # Handle cycle
 from crytic_compile.utils.natspec import Natspec
 
 if TYPE_CHECKING:
     from crytic_compile import CryticCompile
 
+LOGGER = logging.getLogger("CryticCompile")
+
 
 class Vyper(AbstractPlatform):
     """
     Vyper platform
     """
 
     NAME = "vyper"
@@ -58,15 +61,15 @@
         info = targets_json[target]
         filename = convert_filename(target, _relative_to_short, crytic_compile)
 
         contract_name = Path(target).parts[-1]
 
         source_unit = compilation_unit.create_source_unit(filename)
 
-        source_unit.contracts_names.add(contract_name)
+        source_unit.add_contract_name(contract_name)
         compilation_unit.filename_to_contracts[filename].add(contract_name)
         source_unit.abis[contract_name] = info["abi"]
         source_unit.bytecodes_init[contract_name] = info["bytecode"].replace("0x", "")
         source_unit.bytecodes_runtime[contract_name] = info["bytecode_runtime"].replace("0x", "")
         # Vyper does not provide the source mapping for the init bytecode
         source_unit.srcmaps_init[contract_name] = []
         # info["source_map"]["pc_pos_map"] contains the source mapping in a simpler format
@@ -146,14 +149,18 @@
     if not os.path.isfile(filename):
         raise InvalidCompilation(f"{filename} does not exist (are you in the correct directory?)")
 
     cmd = [vyper, filename, "-f", "combined_json"]
 
     additional_kwargs: Dict = {"cwd": working_dir} if working_dir else {}
     stderr = ""
+    LOGGER.info(
+        "'%s' running",
+        " ".join(cmd),
+    )
     try:
         with subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             env=env,
             executable=shutil.which(cmd[0]),
```

### Comparing `crytic-compile-0.3.1/crytic_compile/platform/waffle.py` & `crytic-compile-0.3.2/crytic_compile/platform/waffle.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,28 +177,33 @@
         with open(combined_path, encoding="utf8") as f:
             target_all = json.load(f)
 
         optimized = None
 
         compilation_unit = CompilationUnit(crytic_compile, str(target))
 
+        if "sources" in target_all:
+            compilation_unit.filenames = [
+                convert_filename(path, _relative_to_short, crytic_compile, working_dir=target)
+                for path in target_all["sources"]
+            ]
+
         for contract in target_all["contracts"]:
             target_loaded = target_all["contracts"][contract]
             contract = contract.split(":")
             filename = convert_filename(
                 contract[0], _relative_to_short, crytic_compile, working_dir=target
             )
 
             contract_name = contract[1]
             source_unit = compilation_unit.create_source_unit(filename)
 
             source_unit.ast = target_all["sources"][contract[0]]["AST"]
-            compilation_unit.filenames.add(filename)
             compilation_unit.filename_to_contracts[filename].add(contract_name)
-            source_unit.contracts_names.add(contract_name)
+            source_unit.add_contract_name(contract_name)
             source_unit.abis[contract_name] = target_loaded["abi"]
 
             userdoc = target_loaded.get("userdoc", {})
             devdoc = target_loaded.get("devdoc", {})
             natspec = Natspec(userdoc, devdoc)
             source_unit.natspec[contract_name] = natspec
```

### Comparing `crytic-compile-0.3.1/crytic_compile/source_unit.py` & `crytic-compile-0.3.2/crytic_compile/source_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Module handling the source unit
 Each source unit represents one file so may be associated with
 One or more source units are associated with each compilation unit
 """
 import re
-from typing import Dict, List, Optional, Union, Tuple, Set, TYPE_CHECKING
+from typing import Dict, List, Optional, Union, Tuple, TYPE_CHECKING
 import cbor2
 
 from Crypto.Hash import keccak
 
 from crytic_compile.utils.naming import Filename
 from crytic_compile.utils.natspec import Natspec
 
@@ -56,15 +56,15 @@
         sha3_result = keccak.new(digest_bits=256)
         sha3_result.update(name_candidate.encode("utf-8"))
         ret.append("__$" + sha3_result.hexdigest()[:34] + "$__")
 
     return ret
 
 
-# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-instance-attributes,too-many-public-methods
 class SourceUnit:
     """SourceUnit class"""
 
     def __init__(self, compilation_unit: "CompilationUnit", filename: Filename):
 
         self.filename = filename
         self.compilation_unit: "CompilationUnit" = compilation_unit
@@ -83,18 +83,18 @@
         self._natspec: Dict[str, Natspec] = {}
 
         # Libraries used by the contract
         # contract_name -> (library, pattern)
         self._libraries: Dict[str, List[Tuple[str, str]]] = {}
 
         # set containing all the contract names
-        self._contracts_name: Set[str] = set()
+        self._contracts_name: List[str] = []
 
         # set containing all the contract name without the libraries
-        self._contracts_name_without_libraries: Optional[Set[str]] = None
+        self._contracts_name_without_libraries: Optional[List[str]] = None
 
     # region ABI
     ###################################################################################
     ###################################################################################
 
     @property
     def abis(self) -> Dict:
@@ -407,45 +407,54 @@
     ###################################################################################
     ###################################################################################
     # region Contract Names
     ###################################################################################
     ###################################################################################
 
     @property
-    def contracts_names(self) -> Set[str]:
+    def contracts_names(self) -> List[str]:
         """Return the contracts names
 
         Returns:
-            Set[str]: List of the contracts names
+            List[str]: List of the contracts names
         """
         return self._contracts_name
 
     @contracts_names.setter
-    def contracts_names(self, names: Set[str]) -> None:
+    def contracts_names(self, names: List[str]) -> None:
         """Set the contract names
 
         Args:
-            names (Set[str]): New contracts names
+            names (List[str]): New contracts names
         """
         self._contracts_name = names
 
+    def add_contract_name(self, name: str) -> None:
+        """Add name to contracts_names, if not already present
+
+        Args:
+            name (str): Name to add to the list
+        """
+        if name not in self.contracts_names:
+            self.contracts_names.append(name)
+
     @property
-    def contracts_names_without_libraries(self) -> Set[str]:
+    def contracts_names_without_libraries(self) -> List[str]:
         """Return the contracts names without the librairies
 
         Returns:
-            Set[str]: List of contracts
+            List[str]: List of contracts
         """
         if self._contracts_name_without_libraries is None:
             libraries: List[str] = []
             for contract_name in self._contracts_name:
                 libraries += self.libraries_names(contract_name)
-            self._contracts_name_without_libraries = {
+            self._contracts_name_without_libraries = [
                 l for l in self._contracts_name if l not in set(libraries)
-            }
+            ]
         return self._contracts_name_without_libraries
 
     # endregion
     ###################################################################################
     ###################################################################################
     # region Hashes
     ###################################################################################
```

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/naming.py` & `crytic-compile-0.3.2/crytic_compile/utils/naming.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 """
 Module handling the file naming operation (relative -> absolute, etc)
 """
 
 import logging
 import os.path
 import platform
-from collections import namedtuple
+from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Union, Callable, Optional
 
 from crytic_compile.platform.exceptions import InvalidCompilation
 
 # Cycle dependency
 if TYPE_CHECKING:
     from crytic_compile import CryticCompile
 
 LOGGER = logging.getLogger("CryticCompile")
 
-Filename = namedtuple("Filename", ["absolute", "used", "relative", "short"])
+
+@dataclass
+class Filename:
+    """Path metadata for each file in the compilation unit"""
+
+    def __init__(self, absolute: str, used: str, relative: str, short: str):
+        self.absolute = absolute
+        self.used = used
+        self.relative = relative
+        self.short = short
+
+    def __hash__(self) -> int:
+        return hash(self.relative)
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Filename):
+            return NotImplemented
+        return self.relative == other.relative
+
+    def __repr__(self) -> str:
+        return f"Filename(absolute={self.absolute}, used={self.used}, relative={self.relative}, short={self.short}))"
 
 
 def extract_name(name: str) -> str:
     """Convert '/path:Contract' to Contract
 
     Args:
         name (str): name to convert
@@ -145,15 +165,20 @@
             filename = filename.relative_to(Path(crytic_compile.package_name))
         except ValueError:
             pass
 
     filename = _verify_filename_existence(filename, cwd)
 
     absolute = Path(os.path.abspath(filename))
-    relative = Path(os.path.relpath(filename, Path.cwd()))
+
+    # This returns original path if *path* and *start* are on different drives (for Windows platform).
+    try:
+        relative = Path(os.path.relpath(filename, Path.cwd()))
+    except ValueError:
+        relative = Path(filename)
 
     # Build the short path
     try:
         if cwd.is_absolute():
             short = absolute.relative_to(cwd)
         else:
             short = relative.relative_to(cwd)
@@ -164,9 +189,9 @@
 
     short = relative_to_short(short)
 
     return Filename(
         absolute=str(absolute),
         relative=relative.as_posix(),
         short=short.as_posix(),
-        used=used_filename,
+        used=str(used_filename),
     )
```

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/natspec.py` & `crytic-compile-0.3.2/crytic_compile/utils/natspec.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/npm.py` & `crytic-compile-0.3.2/crytic_compile/utils/npm.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/subprocess.py` & `crytic-compile-0.3.2/crytic_compile/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/unit_tests.py` & `crytic-compile-0.3.2/crytic_compile/utils/unit_tests.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile/utils/zip.py` & `crytic-compile-0.3.2/crytic_compile/utils/zip.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/crytic_compile.egg-info/PKG-INFO` & `crytic-compile-0.3.2/crytic_compile.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.1
+Version: 0.3.2
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # Crytic-compile
 [![Build Status](https://img.shields.io/github/workflow/status/crytic/crytic-compile/CI/master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
 [![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
```

### Comparing `crytic-compile-0.3.1/crytic_compile.egg-info/SOURCES.txt` & `crytic-compile-0.3.2/crytic_compile.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 crytic_compile/utils/name_collision.py
 crytic_compile/utils/naming.py
 crytic_compile/utils/natspec.py
 crytic_compile/utils/npm.py
 crytic_compile/utils/subprocess.py
 crytic_compile/utils/unit_tests.py
 crytic_compile/utils/zip.py
-tests/test_metadata.py
+tests/test_metadata.py
+tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.1/pyproject.toml` & `crytic-compile-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.1/setup.py` & `crytic-compile-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,34 @@
     long_description = f.read()
 
 setup(
     name="crytic-compile",
     description="Util to facilitate smart contracts compilation.",
     url="https://github.com/crytic/crytic-compile",
     author="Trail of Bits",
-    version="0.3.1",
+    version="0.3.2",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.2"],
     extras_require={
-        "dev": [
+        "test": [
+            "pytest",
+            "pytest-cov",
+        ],
+        "lint": [
             "black==22.3.0",
             "pylint==2.13.4",
             "mypy==0.942",
             "darglint==1.8.0",
-        ]
+        ],
+        "doc": [
+            "pdoc",
+        ],
+        "dev": [
+            "crytic-compile[test,doc,lint]",
+        ],
     },
     license="AGPL-3.0",
     long_description=long_description,
     package_data={"crytic_compile": ["py.typed"]},
     entry_points={"console_scripts": ["crytic-compile = crytic_compile.__main__:main"]},
 )
```

### Comparing `crytic-compile-0.3.1/tests/test_metadata.py` & `crytic-compile-0.3.2/tests/test_metadata.py`

 * *Files identical despite different names*

