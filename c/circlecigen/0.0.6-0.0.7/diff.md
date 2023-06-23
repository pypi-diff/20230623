# Comparing `tmp/circlecigen-0.0.6.tar.gz` & `tmp/circlecigen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.6.tar", last modified: Tue Jun 20 22:32:03 2023, max compression
+gzip compressed data, was "circlecigen-0.0.7.tar", last modified: Fri Jun 23 06:47:21 2023, max compression
```

## Comparing `circlecigen-0.0.6.tar` & `circlecigen-0.0.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.161690 circlecigen-0.0.6/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-20 22:31:57.000000 circlecigen-0.0.6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-20 22:32:03.165690 circlecigen-0.0.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-20 22:31:57.000000 circlecigen-0.0.6/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-20 22:31:57.000000 circlecigen-0.0.6/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:31:57.000000 circlecigen-0.0.6/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.161690 circlecigen-0.0.6/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/top_level.txt
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-20 22:31:57.000000 circlecigen-0.0.6/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-20 22:31:57.000000 circlecigen-0.0.6/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-20 22:31:57.000000 circlecigen-0.0.6/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-20 22:31:57.000000 circlecigen-0.0.6/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-20 22:32:03.165690 circlecigen-0.0.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-20 22:31:57.000000 circlecigen-0.0.6/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-20 22:32:03.000000 circlecigen-0.0.6/src/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5805 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.286356 circlecigen-0.0.7/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-23 06:47:15.000000 circlecigen-0.0.7/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-23 06:47:21.290356 circlecigen-0.0.7/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-23 06:47:15.000000 circlecigen-0.0.7/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-23 06:47:15.000000 circlecigen-0.0.7/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:15.000000 circlecigen-0.0.7/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.286356 circlecigen-0.0.7/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5643 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-23 06:47:15.000000 circlecigen-0.0.7/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-23 06:47:15.000000 circlecigen-0.0.7/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-23 06:47:15.000000 circlecigen-0.0.7/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-23 06:47:15.000000 circlecigen-0.0.7/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-23 06:47:21.290356 circlecigen-0.0.7/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-23 06:47:15.000000 circlecigen-0.0.7/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-23 06:47:21.000000 circlecigen-0.0.7/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6019 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5643 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_utils.py
```

### Comparing `circlecigen-0.0.6/.circleci/config.yml` & `circlecigen-0.0.7/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/.pre-commit-config.yaml` & `circlecigen-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/.pylintrc` & `circlecigen-0.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/LICENSE` & `circlecigen-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/PKG-INFO` & `circlecigen-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.6
+Version: 0.0.7
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.6 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.7 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `circlecigen-0.0.6/README.md` & `circlecigen-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.7/circlecigen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.6
+Version: 0.0.7
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.6 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.7 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `circlecigen-0.0.6/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.7/circlecigen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/env_test/config.yml` & `circlecigen-0.0.7/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/env_test/generated_config.yml` & `circlecigen-0.0.7/env_test/generated_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,16 @@
 
 
       - approve prod changes:
           type: approval
           requires:
             - plan prod-us-west-2 change
             - plan prod-us-east-2 change
+            - apply nonprod-us-west-2 change plan
+            - apply nonprod-us-east-2 change plan
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
```

### Comparing `circlecigen-0.0.6/env_test/multi.json` & `circlecigen-0.0.7/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/env_test/post-approve.yml` & `circlecigen-0.0.7/env_test/post-approve.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/pyproject.toml` & `circlecigen-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/setup.py` & `circlecigen-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/src/circlecigen.py` & `circlecigen-0.0.7/src/circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/src/template.py` & `circlecigen-0.0.7/src/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
             })
             if priorapprovalrequired:
                 instance_vars.update({
                     "priorapprovalrequired": PRIOR_APPROVAL.format(priorapprovalrequired)
                 })
             approvalrequiredjobs += f"\n            - plan {instance} change"
             f.write(pre.render(instance_vars))
+
+        if priorapprovalrequired:
+            for prior_role_instance in pipeline[priorapprovalrequired].keys():
+                approvalrequiredjobs += f"\n            - apply {prior_role_instance} change plan"
+
         return approvalrequiredjobs
     return None
 
 def generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role):
     approve_vars.update ({
         "role": role,
         "approvalrequiredjobs": approvalrequiredjobs
```

### Comparing `circlecigen-0.0.6/src/tfvars.py` & `circlecigen-0.0.7/src/tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/src/utils.py` & `circlecigen-0.0.7/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/test/generated_config.yml` & `circlecigen-0.0.7/test/generated_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,16 @@
 
 
       - approve prod changes:
           type: approval
           requires:
             - plan prod-us-west-2 change
             - plan prod-us-east-2 change
+            - apply nonprod-us-west-2 change plan
+            - apply nonprod-us-east-2 change plan
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply prod-us-west-2 change plan
           context: *context
           workspace: prod-us-west-2
           var-file: env_test/prod-us-west-2.tfvars.json
```

### Comparing `circlecigen-0.0.6/test/generated_config_setup.yml` & `circlecigen-0.0.7/test/generated_config_setup.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/test/test_circlecigen.py` & `circlecigen-0.0.7/test/test_circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/test/test_template.py` & `circlecigen-0.0.7/test/test_template.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/test/test_tfvars.py` & `circlecigen-0.0.7/test/test_tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.6/test/test_utils.py` & `circlecigen-0.0.7/test/test_utils.py`

 * *Files identical despite different names*

