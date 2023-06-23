# Comparing `tmp/pynessie-0.9.0.tar.gz` & `tmp/pynessie-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynessie-0.9.0.tar", last modified: Mon Aug  9 16:28:06 2021, max compression
+gzip compressed data, was "pynessie-0.9.2.tar", last modified: Thu Aug 26 19:19:18 2021, max compression
```

## Comparing `pynessie-0.9.0.tar` & `pynessie-0.9.2.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.266255 pynessie-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-08-09 15:59:25.000000 pynessie-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2021-08-09 15:59:25.000000 pynessie-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-08-09 15:59:25.000000 pynessie-0.9.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-08-09 15:59:25.000000 pynessie-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-08-09 15:59:25.000000 pynessie-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2021-08-09 16:28:06.266255 pynessie-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-08-09 15:59:25.000000 pynessie-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.254254 pynessie-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      945 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/branch.rst
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/cherry-pick.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4968 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/log.rst
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/main.rst
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/merge.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/nessie_client.auth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/nessie_client.conf.rst
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/nessie_client.rst
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/pynessie.auth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/pynessie.conf.rst
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/pynessie.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/remote.rst
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/tag.rst
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-09 15:59:25.000000 pynessie-0.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.258254 pynessie-0.9.0/pynessie/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11005 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.258254 pynessie-0.9.0/pynessie/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/auth/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/auth/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/auth/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    21735 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.262254 pynessie-0.9.0/pynessie/conf/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/conf/config_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/conf/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      825 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/conf/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/conf/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/expression_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     8424 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9310 2021-08-09 15:59:25.000000 pynessie-0.9.0/pynessie/nessie_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.258254 pynessie-0.9.0/pynessie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-09 16:28:06.000000 pynessie-0.9.0/pynessie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-08-09 15:59:25.000000 pynessie-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-08-09 15:59:25.000000 pynessie-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-08-09 16:28:06.266255 pynessie-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-08-09 15:59:25.000000 pynessie-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.262254 pynessie-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.246254 pynessie-0.9.0/tests/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.266255 pynessie-0.9.0/tests/cassettes/test_nessie_cli/
--rw-r--r--   0 runner    (1001) docker     (121)    18178 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_assign.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_command_line_interface.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16407 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_contents_listing.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19085 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_log.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11525 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_merge.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_owner_repo_config_cli.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7857 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_ref.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_remote.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9935 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_tag.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    15936 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_transplant.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:28:06.266255 pynessie-0.9.0/tests/cassettes/test_nessie_client/
--rw-r--r--   0 runner    (1001) docker     (121)     5203 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/cassettes/test_nessie_client/test_client_interface_e2e.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/test_expression_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    18571 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/test_nessie_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-08-09 15:59:25.000000 pynessie-0.9.0/tests/test_nessie_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.766821 pynessie-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-08-26 18:52:04.000000 pynessie-0.9.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3575 2021-08-26 18:52:04.000000 pynessie-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-08-26 18:52:04.000000 pynessie-0.9.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2021-08-26 18:52:04.000000 pynessie-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-08-26 18:52:04.000000 pynessie-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-08-26 19:19:18.766821 pynessie-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-08-26 18:52:04.000000 pynessie-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.746821 pynessie-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/branch.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/cherry-pick.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4968 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/log.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/main.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/merge.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/nessie_client.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/nessie_client.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/nessie_client.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/pynessie.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/pynessie.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/pynessie.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/remote.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/tag.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-26 18:52:04.000000 pynessie-0.9.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.750822 pynessie-0.9.2/pynessie/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11005 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.754822 pynessie-0.9.2/pynessie/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/auth/aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/auth/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3843 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/auth/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21553 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.754822 pynessie-0.9.2/pynessie/conf/
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/conf/config_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/conf/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/conf/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/conf/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3936 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/expression_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8424 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9122 2021-08-26 18:52:04.000000 pynessie-0.9.2/pynessie/nessie_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.750822 pynessie-0.9.2/pynessie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-26 19:19:18.000000 pynessie-0.9.2/pynessie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2021-08-26 18:52:04.000000 pynessie-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-08-26 18:52:04.000000 pynessie-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2021-08-26 19:19:18.766821 pynessie-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-08-26 18:52:04.000000 pynessie-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.758822 pynessie-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.722822 pynessie-0.9.2/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.766821 pynessie-0.9.2/tests/cassettes/test_nessie_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)    18178 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_assign.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_command_line_interface.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16408 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_contents_listing.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19085 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11525 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7857 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_ref.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9935 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_tag.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    15936 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_transplant.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 19:19:18.766821 pynessie-0.9.2/tests/cassettes/test_nessie_client/
+-rw-r--r--   0 runner    (1001) docker     (121)     5203 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/cassettes/test_nessie_client/test_client_interface_e2e.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6674 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/test_expression_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17486 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/test_nessie_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-08-26 18:52:04.000000 pynessie-0.9.2/tests/test_nessie_client.py
```

### Comparing `pynessie-0.9.0/CONTRIBUTING.rst` & `pynessie-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/HISTORY.rst` & `pynessie-0.9.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.9.2 (2021-08-26)
+------------------
+
+* (No Python related highlights)
+
 0.9.0 (2021-08-09)
 ------------------
 
 * (No Python related highlights)
 
 0.8.3 (2021-07-19)
 ------------------
```

### Comparing `pynessie-0.9.0/LICENSE` & `pynessie-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/PKG-INFO` & `pynessie-0.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pynessie
-Version: 0.9.0
+Version: 0.9.2
 Summary: Project Nessie: A Git-like Experience for your Data Lake
 Home-page: https://github.com/projectnessie/nessie
 Author: Ryan Murray
 Author-email: nessie-release-builder@dremio.com
 License: Apache Software License 2.0
 Description: =============================
         Python API and CLI for Nessie
@@ -16,14 +16,19 @@
         
         .. _projectnessie.org: https://projectnessie.org
         
         =======
         History
         =======
         
+        0.9.2 (2021-08-26)
+        ------------------
+        
+        * (No Python related highlights)
+        
         0.9.0 (2021-08-09)
         ------------------
         
         * (No Python related highlights)
         
         0.8.3 (2021-07-19)
         ------------------
```

### Comparing `pynessie-0.9.0/docs/Makefile` & `pynessie-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/branch.rst` & `pynessie-0.9.2/docs/branch.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/cli.rst` & `pynessie-0.9.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/conf.py` & `pynessie-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/contents.rst` & `pynessie-0.9.2/docs/contents.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/installation.rst` & `pynessie-0.9.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/log.rst` & `pynessie-0.9.2/docs/log.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/make.bat` & `pynessie-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/merge.rst` & `pynessie-0.9.2/docs/merge.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/nessie_client.auth.rst` & `pynessie-0.9.2/docs/nessie_client.auth.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/nessie_client.rst` & `pynessie-0.9.2/docs/nessie_client.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/pynessie.auth.rst` & `pynessie-0.9.2/docs/pynessie.auth.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/pynessie.conf.rst` & `pynessie-0.9.2/docs/pynessie.conf.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/pynessie.rst` & `pynessie-0.9.2/docs/pynessie.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/docs/tag.rst` & `pynessie-0.9.2/docs/tag.rst`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/__init__.py` & `pynessie-0.9.2/pynessie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import confuse
 
 from .conf import build_config
 from .nessie_client import NessieClient
 
 __author__ = """Project Nessie"""
 __email__ = "nessie-release-builder@dremio.com"
-__version__ = "0.9.0"
+__version__ = "0.9.2"
 
 
 def get_config(config_dir: str = None, args: dict = None) -> confuse.Configuration:
     """Retrieve a confuse Configuration object."""
     if config_dir:
         os.environ["NESSIE_CLIENTDIR"] = config_dir
     return build_config(args)
```

### Comparing `pynessie-0.9.0/pynessie/_endpoints.py` & `pynessie-0.9.2/pynessie/_endpoints.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/_ref.py` & `pynessie-0.9.2/pynessie/_ref.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/auth/__init__.py` & `pynessie-0.9.2/pynessie/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/auth/basic.py` & `pynessie-0.9.2/pynessie/auth/basic.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/auth/config.py` & `pynessie-0.9.2/pynessie/auth/config.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/cli.py` & `pynessie-0.9.2/pynessie/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,28 +96,25 @@
         return super(DefaultHelp, self).parse_args(ctx, args)
 
 
 @click.group()
 @click.option("--json", is_flag=True, help="write output in json format.")
 @click.option("-v", "--verbose", is_flag=True, help="Verbose output.")
 @click.option("--endpoint", help="Optional endpoint, if different from config file.")
-@click.option("--repo", help="Optional repository owner + name, if different from config file, separated by a slash.")
 @click.option("--version", is_flag=True, callback=_print_version, expose_value=False, is_eager=True)
 @click.pass_context
-def cli(ctx: click.core.Context, json: bool, verbose: bool, endpoint: str, repo: str) -> None:
+def cli(ctx: click.core.Context, json: bool, verbose: bool, endpoint: str) -> None:
     """Nessie cli tool.
 
     Interact with Nessie branches and tables via the command line
     """
     try:
         cfg_map = {}
         if endpoint:
             cfg_map["endpoint"] = endpoint
-        if repo:
-            cfg_map["repo"] = repo
         config = build_config(cfg_map)
         nessie = NessieClient(config)
         ctx.obj = ContextObject(nessie, verbose, json)
     except confuse.exceptions.ConfigTypeError as e:
         raise click.ClickException(str(e))
```

### Comparing `pynessie-0.9.0/pynessie/conf/config_command.py` & `pynessie-0.9.2/pynessie/conf/config_command.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/conf/config_parser.py` & `pynessie-0.9.2/pynessie/conf/config_parser.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/error.py` & `pynessie-0.9.2/pynessie/error.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/expression_util.py` & `pynessie-0.9.2/pynessie/expression_util.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/model.py` & `pynessie-0.9.2/pynessie/model.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/pynessie/nessie_client.py` & `pynessie-0.9.2/pynessie/nessie_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,15 @@
 
 
 class NessieClient(object):
     """Base Nessie Client."""
 
     def __init__(self: "NessieClient", config: confuse.Configuration) -> None:
         """Create a Nessie Client from known config."""
-        url = config["endpoint"].get()
-        repo = config["repo"].get() if "repo" in config else None
-        if repo:
-            sep = "" if url[-1:] == "/" else "/"
-            url = f"{url}{sep}{repo}"
-        self._base_url = url
+        self._base_url = config["endpoint"].get()
         self._ssl_verify = config["verify"].get(bool)
         self._commit_id: str = cast(str, None)
 
         try:
             self._base_branch = config["default_branch"].get()
         except confuse.exceptions.NotFoundError:
             self._base_branch = None
```

### Comparing `pynessie-0.9.0/pynessie.egg-info/PKG-INFO` & `pynessie-0.9.2/pynessie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pynessie
-Version: 0.9.0
+Version: 0.9.2
 Summary: Project Nessie: A Git-like Experience for your Data Lake
 Home-page: https://github.com/projectnessie/nessie
 Author: Ryan Murray
 Author-email: nessie-release-builder@dremio.com
 License: Apache Software License 2.0
 Description: =============================
         Python API and CLI for Nessie
@@ -16,14 +16,19 @@
         
         .. _projectnessie.org: https://projectnessie.org
         
         =======
         History
         =======
         
+        0.9.2 (2021-08-26)
+        ------------------
+        
+        * (No Python related highlights)
+        
         0.9.0 (2021-08-09)
         ------------------
         
         * (No Python related highlights)
         
         0.8.3 (2021-07-19)
         ------------------
```

### Comparing `pynessie-0.9.0/pynessie.egg-info/SOURCES.txt` & `pynessie-0.9.2/pynessie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,12 @@
 tests/test_nessie_cli.py
 tests/test_nessie_client.py
 tests/cassettes/test_nessie_cli/test_assign.yaml
 tests/cassettes/test_nessie_cli/test_command_line_interface.yaml
 tests/cassettes/test_nessie_cli/test_contents_listing.yaml
 tests/cassettes/test_nessie_cli/test_log.yaml
 tests/cassettes/test_nessie_cli/test_merge.yaml
-tests/cassettes/test_nessie_cli/test_owner_repo_config_cli.yaml
 tests/cassettes/test_nessie_cli/test_ref.yaml
 tests/cassettes/test_nessie_cli/test_remote.yaml
 tests/cassettes/test_nessie_cli/test_tag.yaml
 tests/cassettes/test_nessie_cli/test_transplant.yaml
 tests/cassettes/test_nessie_client/test_client_interface_e2e.yaml
```

### Comparing `pynessie-0.9.0/setup.cfg` & `pynessie-0.9.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 0.9.2
 commit = False
 tag = False
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pynessie-0.9.0/setup.py` & `pynessie-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     keywords="pynessie",
     name="pynessie",
     packages=find_packages(include=["pynessie", "pynessie.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=[],
     url="https://github.com/projectnessie/nessie",
-    version="0.9.0",
+    version="0.9.2",
     zip_safe=False,
 )
```

### Comparing `pynessie-0.9.0/tests/README.md` & `pynessie-0.9.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_assign.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_assign.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_command_line_interface.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_command_line_interface.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_contents_listing.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_contents_listing.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
       Content-Type:
       - application/json
     status:
       code: 404
       message: Not Found
 - request:
     body: '{"operations": [{"key": {"elements": ["this", "is", "sql", "baz"]}, "contents":
-      {"dialect": "HIVE", "id": "uuid3", "sqlText": "SELECT * FROM foo", "type": "VIEW"},
+      {"dialect": "SPARK", "id": "uuid3", "sqlText": "SELECT * FROM foo", "type": "VIEW"},
       "type": "PUT"}], "commitMeta": {"signedOffBy": null, "email": null, "properties":
       null, "message": "test_message3", "authorTime": null, "hash": null, "author":
       null, "commitTime": null, "committer": null}}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
```

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_log.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_log.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_merge.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_merge.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_owner_repo_config_cli.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_ref.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,48 +7,52 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/trees/tree
+    uri: http://localhost:19120/api/v1/trees
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
+        \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}\
+        \ ]"
     headers:
       Content-Length:
-      - '121'
+      - '125'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
-    body: null
+    body: '{"name": "dev", "hash": null, "type": "BRANCH"}'
     headers:
       Accept:
-      - application/json
+      - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
+      Content-Length:
+      - '47'
+      Content-Type:
+      - application/json
       User-Agent:
       - python-requests/2.26.0
-    method: GET
-    uri: http://localhost:19120/api/v1/trees
+    method: POST
+    uri: http://localhost:19120/api/v1/trees/tree
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
-        \ \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}\
-        \ ]"
+      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"\
+        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
     headers:
       Content-Length:
-      - '125'
+      - '120'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -58,22 +62,24 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees/tree
+    uri: http://localhost:19120/api/v1/trees
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
+        \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n},\
+        \ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\
+        \n} ]"
     headers:
       Content-Length:
-      - '121'
+      - '247'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -83,74 +89,77 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees
+    uri: http://localhost:19120/api/v1/trees/tree/etl
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
-        \ \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}\
-        \ ]"
+      string: "{\n  \"message\" : \"Unable to find reference [etl].\",\n  \"status\"\
+        \ : 404,\n  \"reason\" : \"Not Found\",\n  \"serverStackTrace\" : null\n}"
     headers:
       Content-Length:
-      - '125'
+      - '124'
       Content-Type:
       - application/json
     status:
-      code: 200
-      message: OK
+      code: 404
+      message: Not Found
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees/tree
+    uri: http://localhost:19120/api/v1/trees/tree/main
   response:
     body:
       string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
       - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
-    body: null
+    body: '{"name": "etl", "hash": "a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a",
+      "type": "BRANCH"}'
     headers:
       Accept:
-      - application/json
+      - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
+      Content-Length:
+      - '109'
+      Content-Type:
+      - application/json
       User-Agent:
       - python-requests/2.26.0
-    method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees
+    method: POST
+    uri: http://localhost:19120/api/v1/trees/tree
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
-        \ \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}\
-        \ ]"
+      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '125'
+      - '120'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -160,22 +169,25 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/snazy/ursus/trees/tree
+    uri: http://localhost:19120/api/v1/trees
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" :\
+        \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n},\
+        \ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\
+        \n}, {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\
+        \n} ]"
     headers:
       Content-Length:
-      - '121'
+      - '369'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -185,70 +197,113 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/snazy/ursus/trees
+    uri: http://localhost:19120/api/v1/trees/tree/etl
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
-        \ \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}\
-        \ ]"
+      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '125'
+      - '120'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
+      Content-Length:
+      - '0'
+      User-Agent:
+      - python-requests/2.26.0
+    method: DELETE
+    uri: http://localhost:19120/api/v1/trees/branch/etl?expectedHash=a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a
+  response:
+    body:
+      string: ''
+    headers: {}
+    status:
+      code: 204
+      message: No Content
+- request:
+    body: null
+    headers:
+      Accept:
+      - application/json
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees/tree
+    uri: http://localhost:19120/api/v1/trees/tree/dev
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
+      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"\
         2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
     headers:
       Content-Length:
-      - '121'
+      - '120'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
+      Content-Length:
+      - '0'
+      User-Agent:
+      - python-requests/2.26.0
+    method: DELETE
+    uri: http://localhost:19120/api/v1/trees/branch/dev?expectedHash=2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d
+  response:
+    body:
+      string: ''
+    headers: {}
+    status:
+      code: 204
+      message: No Content
+- request:
+    body: null
+    headers:
+      Accept:
+      - application/json
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/robert/elani/trees
+    uri: http://localhost:19120/api/v1/trees
   response:
     body:
       string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
-        \ \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}\
+        \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}\
         \ ]"
     headers:
       Content-Length:
       - '125'
       Content-Type:
       - application/json
     status:
```

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_ref.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_tag.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -22,37 +22,88 @@
       - '125'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
-    body: '{"name": "dev", "hash": null, "type": "BRANCH"}'
+    body: null
+    headers:
+      Accept:
+      - application/json
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.26.0
+    method: GET
+    uri: http://localhost:19120/api/v1/trees/tree/dev-tag
+  response:
+    body:
+      string: "{\n  \"message\" : \"Unable to find reference [dev-tag].\",\n  \"status\"\
+        \ : 404,\n  \"reason\" : \"Not Found\",\n  \"serverStackTrace\" : null\n}"
+    headers:
+      Content-Length:
+      - '128'
+      Content-Type:
+      - application/json
+    status:
+      code: 404
+      message: Not Found
+- request:
+    body: null
+    headers:
+      Accept:
+      - application/json
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.26.0
+    method: GET
+    uri: http://localhost:19120/api/v1/trees/tree/main
+  response:
+    body:
+      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
+    headers:
+      Content-Length:
+      - '121'
+      Content-Type:
+      - application/json
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"name": "dev-tag", "hash": "a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a",
+      "type": "TAG"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '47'
+      - '110'
       Content-Type:
       - application/json
       User-Agent:
       - python-requests/2.26.0
     method: POST
     uri: http://localhost:19120/api/v1/trees/tree
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+      string: "{\n  \"type\" : \"TAG\",\n  \"name\" : \"dev-tag\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '120'
+      - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -65,21 +116,21 @@
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
     uri: http://localhost:19120/api/v1/trees
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" :\
+      string: "[ {\n  \"type\" : \"TAG\",\n  \"name\" : \"dev-tag\",\n  \"hash\" :\
         \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n},\
-        \ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\
+        \ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\
         \n} ]"
     headers:
       Content-Length:
-      - '247'
+      - '248'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -89,22 +140,22 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/trees/tree/etl
+    uri: http://localhost:19120/api/v1/trees/tree/etl-tag
   response:
     body:
-      string: "{\n  \"message\" : \"Unable to find reference [etl].\",\n  \"status\"\
+      string: "{\n  \"message\" : \"Unable to find reference [etl-tag].\",\n  \"status\"\
         \ : 404,\n  \"reason\" : \"Not Found\",\n  \"serverStackTrace\" : null\n}"
     headers:
       Content-Length:
-      - '124'
+      - '128'
       Content-Type:
       - application/json
     status:
       code: 404
       message: Not Found
 - request:
     body: null
@@ -128,38 +179,38 @@
       - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
-    body: '{"name": "etl", "hash": "a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a",
-      "type": "BRANCH"}'
+    body: '{"name": "etl-tag", "hash": "a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a",
+      "type": "TAG"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '109'
+      - '110'
       Content-Type:
       - application/json
       User-Agent:
       - python-requests/2.26.0
     method: POST
     uri: http://localhost:19120/api/v1/trees/tree
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" : \"\
+      string: "{\n  \"type\" : \"TAG\",\n  \"name\" : \"etl-tag\",\n  \"hash\" : \"\
         a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '120'
+      - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -172,22 +223,22 @@
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
     uri: http://localhost:19120/api/v1/trees
   response:
     body:
-      string: "[ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" :\
+      string: "[ {\n  \"type\" : \"TAG\",\n  \"name\" : \"dev-tag\",\n  \"hash\" :\
         \ \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n},\
         \ {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"main\",\n  \"hash\" : \"a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\
-        \n}, {\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\
-        \n} ]"
+        \n}, {\n  \"type\" : \"TAG\",\n  \"name\" : \"etl-tag\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n} ]"
     headers:
       Content-Length:
-      - '369'
+      - '371'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -197,22 +248,22 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/trees/tree/etl
+    uri: http://localhost:19120/api/v1/trees/tree/etl-tag
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"etl\",\n  \"hash\" : \"\
+      string: "{\n  \"type\" : \"TAG\",\n  \"name\" : \"etl-tag\",\n  \"hash\" : \"\
         a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '120'
+      - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -224,15 +275,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
       - python-requests/2.26.0
     method: DELETE
-    uri: http://localhost:19120/api/v1/trees/branch/etl?expectedHash=a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a
+    uri: http://localhost:19120/api/v1/trees/tag/etl-tag?expectedHash=a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a
   response:
     body:
       string: ''
     headers: {}
     status:
       code: 204
       message: No Content
@@ -244,22 +295,22 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.26.0
     method: GET
-    uri: http://localhost:19120/api/v1/trees/tree/dev
+    uri: http://localhost:19120/api/v1/trees/tree/dev-tag
   response:
     body:
-      string: "{\n  \"type\" : \"BRANCH\",\n  \"name\" : \"dev\",\n  \"hash\" : \"\
-        2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d\"\n}"
+      string: "{\n  \"type\" : \"TAG\",\n  \"name\" : \"dev-tag\",\n  \"hash\" : \"\
+        a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a\"\n}"
     headers:
       Content-Length:
-      - '120'
+      - '121'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -271,15 +322,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
       - python-requests/2.26.0
     method: DELETE
-    uri: http://localhost:19120/api/v1/trees/branch/dev?expectedHash=2e1cfa82b035c26cbbbdae632cea070514eb8b773f616aaeaf668e2f0be8f10d
+    uri: http://localhost:19120/api/v1/trees/tag/dev-tag?expectedHash=a615031ae80f9e42ffaaeeba5ac67e1dddaa86fecbc20a14b91aac19f1fa748a
   response:
     body:
       string: ''
     headers: {}
     status:
       code: 204
       message: No Content
@@ -305,8 +356,38 @@
       Content-Length:
       - '125'
       Content-Type:
       - application/json
     status:
       code: 200
       message: OK
+- request:
+    body: '{"name": "v1.0", "hash": null, "type": "TAG"}'
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      User-Agent:
+      - python-requests/2.26.0
+    method: POST
+    uri: http://localhost:19120/api/v1/trees/tree
+  response:
+    body:
+      string: "{\n  \"message\" : \"Cannot create an unassigned tag reference\",\n\
+        \  \"status\" : 400,\n  \"reason\" : \"Bad Request\",\n  \"serverStackTrace\"\
+        \ : null\n}"
+    headers:
+      Content-Length:
+      - '136'
+      Content-Type:
+      - application/json
+    status:
+      code: 400
+      message: Bad Request
 version: 1
```

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_remote.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_remote.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_cli/test_transplant.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_cli/test_transplant.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/cassettes/test_nessie_client/test_client_interface_e2e.yaml` & `pynessie-0.9.2/tests/cassettes/test_nessie_client/test_client_interface_e2e.yaml`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/test_expression_util.py` & `pynessie-0.9.2/tests/test_expression_util.py`

 * *Files identical despite different names*

### Comparing `pynessie-0.9.0/tests/test_nessie_cli.py` & `pynessie-0.9.2/tests/test_nessie_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,39 +46,14 @@
     help_result = _run(runner, ["--json", "branch", "-l"])
     references = ReferenceSchema().loads(help_result.output, many=True)
     assert len(references) == 1
     assert references[0].name == "main"
     assert isinstance(references[0], Branch)
 
 
-@pytest.mark.vcr
-def test_owner_repo_config_cli() -> None:
-    """Ensure the CLI handles owner + repo specified in the config file + on the command line."""
-    runner = CliRunner()
-
-    # clean up config file
-    runner.invoke(cli.cli, ["config", "--unset", "repo"])
-
-    result = _run(runner, ["remote", "show"])
-    assert "Remote URL: http://localhost:19120/api/v1\n" in result.output
-    result = _run(runner, ["--repo", "robert/elani", "remote", "show"])
-    assert "Remote URL: http://localhost:19120/api/v1/robert/elani\n" in result.output
-
-    _run(runner, ["config", "--add", "repo", "robert/elani"])
-
-    result = _run(runner, ["remote", "show"])
-    assert "Remote URL: http://localhost:19120/api/v1/robert/elani\n" in result.output
-    result = _run(runner, ["--repo", "snazy/ursus", "remote", "show"])
-    assert "Remote URL: http://localhost:19120/api/v1/snazy/ursus\n" in result.output
-    result = _run(runner, ["remote", "show"])
-    assert "Remote URL: http://localhost:19120/api/v1/robert/elani\n" in result.output
-
-    _run(runner, ["config", "--unset", "repo"])
-
-
 def test_config_options() -> None:
     """Ensure config cli option is consistent."""
     runner = CliRunner()
     result = _run(runner, ["config"])
     assert "Usage: cli" in result.output
     vars = ["--add x", "--get x", "--list", "--unset x"]
     for i in itertools.permutations(vars, 2):
@@ -409,15 +384,15 @@
     branch = "contents_listing_dev"
     _run(runner, ["branch", branch])
 
     iceberg_table = IcebergTable(id="uuid", metadata_location="/a/b/c")
     delta_lake_table = DeltaLakeTable(
         id="uuid2", metadata_location_history=["asd"], checkpoint_location_history=["def"], last_checkpoint="x"
     )
-    sql_view = SqlView(id="uuid3", sql_text="SELECT * FROM foo", dialect="HIVE")
+    sql_view = SqlView(id="uuid3", sql_text="SELECT * FROM foo", dialect="SPARK")
 
     refs = ReferenceSchema().loads(_run(runner, ["--json", "branch", "-l", branch]).output, many=True)
     _run(
         runner,
         ["contents", "--set", "this.is.iceberg.foo", "--ref", branch, "-m", "test_message1", "-c", refs[0].hash_],
         input=ContentsSchema().dumps(iceberg_table),
     )
```

### Comparing `pynessie-0.9.0/tests/test_nessie_client.py` & `pynessie-0.9.2/tests/test_nessie_client.py`

 * *Files identical despite different names*

