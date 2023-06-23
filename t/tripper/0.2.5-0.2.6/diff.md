# Comparing `tmp/tripper-0.2.5.tar.gz` & `tmp/tripper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripper-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tripper-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tripper-0.2.5.tar` & `tripper-0.2.6.tar`

### file list

```diff
@@ -1,71 +1,75 @@
--rw-r--r--   0        0        0      205 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/dependabot.yml
--rw-r--r--   0        0        0      637 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/pull_request_template.md
--rw-r--r--   0        0        0      916 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      545 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_automerge_dependency_prs.yml
--rw-r--r--   0        0        0      656 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_cd_updated_main.yml
--rw-r--r--   0        0        0      602 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0     2420 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0      838 2023-05-24 14:00:35.357635 tripper-0.2.5/.github/workflows/ci_update_dependencies.yml
--rw-r--r--   0        0        0      137 2023-05-24 14:00:35.357635 tripper-0.2.5/.gitignore
--rw-r--r--   0        0        0     1819 2023-05-24 14:00:35.357635 tripper-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       42 2023-05-24 14:00:35.357635 tripper-0.2.5/.pylintrc
--rw-r--r--   0        0        0    10073 2023-05-24 14:01:27.094360 tripper-0.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-05-24 14:00:35.361635 tripper-0.2.5/LICENSE
--rw-r--r--   0        0        0     2496 2023-05-24 14:00:35.361635 tripper-0.2.5/README.md
-lrwxr-xr-x   0        0        0        0 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/LICENSE.md -> ../LICENSE
--rw-r--r--   0        0        0       23 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/.pages
--rw-r--r--   0        0        0       18 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/.pages
--rw-r--r--   0        0        0       46 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/collection.md
--rw-r--r--   0        0        0       38 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/ontopy.md
--rw-r--r--   0        0        0       38 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/rdflib.md
--rw-r--r--   0        0        0       52 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/backends/sparqlwrapper.md
--rw-r--r--   0        0        0       29 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/errors.md
--rw-r--r--   0        0        0       35 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/interface.md
--rw-r--r--   0        0        0       31 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/literal.md
--rw-r--r--   0        0        0       18 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/mappings/.pages
--rw-r--r--   0        0        0       42 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/mappings/mappings.md
--rw-r--r--   0        0        0       35 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/namespace.md
--rw-r--r--   0        0        0       39 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/triplestore.md
--rw-r--r--   0        0        0       27 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/api_reference/utils.md
--rw-r--r--   0        0        0     2909 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/backend_discovery.md
--rw-r--r--   0        0        0      183 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/css/reference.css
--rw-r--r--   0        0        0     2489 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/index.md
--rw-r--r--   0        0        0    12710 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/mappings/figs/function_emmo.svg
--rw-r--r--   0        0        0      228 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/planned-backends.md
--rw-r--r--   0        0        0     3963 2023-05-24 14:00:35.361635 tripper-0.2.5/docs/tutorial.md
--rw-r--r--   0        0        0     1188 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/README.md
--rw-r--r--   0        0        0    18333 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/knowledge-base.svg
--rw-r--r--   0        0        0     8546 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/route.svg
--rw-r--r--   0        0        0     7117 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow.svg
--rw-r--r--   0        0        0      894 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow_mappings.py
--rw-r--r--   0        0        0    14169 2023-05-24 14:00:35.361635 tripper-0.2.5/examples/workflow-mappings/workflow_w_pipes.svg
--rw-r--r--   0        0        0     1943 2023-05-24 14:00:35.361635 tripper-0.2.5/mkdocs.yml
--rw-r--r--   0        0        0     2713 2023-05-24 14:00:35.361635 tripper-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3444 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0      959 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/mappings/test_function.py
--rw-r--r--   0        0        0     1455 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/mappings/test_mappings.py
--rw-r--r--   0        0        0     5701 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/ontologies/family.ttl
--rw-r--r--   0        0        0     6753 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/ontologies/food.ttl
--rw-r--r--   0        0        0     3166 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_add_function.py
--rw-r--r--   0        0        0      880 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_collection.py
--rw-r--r--   0        0        0     2451 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_get_data.py
--rw-r--r--   0        0        0     3943 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_literals.py
--rw-r--r--   0        0        0     1993 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_namespace.py
--rw-r--r--   0        0        0     7802 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_triplestore.py
--rw-r--r--   0        0        0     6062 2023-05-24 14:00:35.361635 tripper-0.2.5/tests/test_utils.py
--rw-r--r--   0        0        0      705 2023-05-24 14:01:27.594367 tripper-0.2.5/tripper/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/__init__.py
--rw-r--r--   0        0        0     2482 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/collection.py
--rw-r--r--   0        0        0     9100 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/ontopy.py
--rw-r--r--   0        0        0     7363 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/rdflib.py
--rw-r--r--   0        0        0     4112 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/backends/sparqlwrapper.py
--rw-r--r--   0        0        0      362 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/errors.py
--rw-r--r--   0        0        0     5379 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/interface.py
--rw-r--r--   0        0        0     5510 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/literal.py
--rw-r--r--   0        0        0      102 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/mappings/__init__.py
--rw-r--r--   0        0        0    35281 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/mappings/mappings.py
--rw-r--r--   0        0        0     6901 2023-05-24 14:00:35.361635 tripper-0.2.5/tripper/namespace.py
--rw-r--r--   0        0        0    43718 2023-05-24 14:00:35.365635 tripper-0.2.5/tripper/triplestore.py
--rw-r--r--   0        0        0     8237 2023-05-24 14:00:35.365635 tripper-0.2.5/tripper/utils.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 tripper-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      205 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/pull_request_template.md
+-rw-r--r--   0        0        0      916 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      545 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/ci_automerge_dependency_prs.yml
+-rw-r--r--   0        0        0      656 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/ci_cd_updated_main.yml
+-rw-r--r--   0        0        0      602 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0     2428 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0      838 2023-06-23 20:45:01.119169 tripper-0.2.6/.github/workflows/ci_update_dependencies.yml
+-rw-r--r--   0        0        0      137 2023-06-23 20:45:01.119169 tripper-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1819 2023-06-23 20:45:01.119169 tripper-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-06-23 20:45:52.883165 tripper-0.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-06-23 20:45:01.123170 tripper-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2591 2023-06-23 20:45:01.123170 tripper-0.2.6/README.md
+lrwxr-xr-x   0        0        0        0 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/LICENSE.md -> ../LICENSE
+-rw-r--r--   0        0        0       23 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/.pages
+-rw-r--r--   0        0        0       18 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/backends/.pages
+-rw-r--r--   0        0        0       46 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/backends/collection.md
+-rw-r--r--   0        0        0       38 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/backends/ontopy.md
+-rw-r--r--   0        0        0       38 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/backends/rdflib.md
+-rw-r--r--   0        0        0       52 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/backends/sparqlwrapper.md
+-rw-r--r--   0        0        0       29 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/errors.md
+-rw-r--r--   0        0        0       35 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/interface.md
+-rw-r--r--   0        0        0       31 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/literal.md
+-rw-r--r--   0        0        0       18 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/mappings/.pages
+-rw-r--r--   0        0        0       42 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/mappings/mappings.md
+-rw-r--r--   0        0        0       35 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/namespace.md
+-rw-r--r--   0        0        0       39 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/triplestore.md
+-rw-r--r--   0        0        0       31 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/tripper.md
+-rw-r--r--   0        0        0       27 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/api_reference/utils.md
+-rw-r--r--   0        0        0     2909 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/backend_discovery.md
+-rw-r--r--   0        0        0      183 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/css/reference.css
+-rw-r--r--   0        0        0     2584 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/index.md
+-rw-r--r--   0        0        0    12710 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/mappings/figs/function_emmo.svg
+-rw-r--r--   0        0        0      228 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/planned-backends.md
+-rw-r--r--   0        0        0     3963 2023-06-23 20:45:01.123170 tripper-0.2.6/docs/tutorial.md
+-rw-r--r--   0        0        0     1188 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/README.md
+-rw-r--r--   0        0        0    18333 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/knowledge-base.svg
+-rw-r--r--   0        0        0     8546 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/route.svg
+-rw-r--r--   0        0        0     7117 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/workflow.svg
+-rw-r--r--   0        0        0      894 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/workflow_mappings.py
+-rw-r--r--   0        0        0    14169 2023-06-23 20:45:01.123170 tripper-0.2.6/examples/workflow-mappings/workflow_w_pipes.svg
+-rw-r--r--   0        0        0     1943 2023-06-23 20:45:01.123170 tripper-0.2.6/mkdocs.yml
+-rw-r--r--   0        0        0     2849 2023-06-23 20:45:01.123170 tripper-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/backends/__init__.py
+-rw-r--r--   0        0        0      542 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/backends/dummy.py
+-rw-r--r--   0        0        0     3480 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0      951 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/mappings/test_function.py
+-rw-r--r--   0        0        0     1461 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/mappings/test_mappings.py
+-rw-r--r--   0        0        0     5701 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/ontologies/family.ttl
+-rw-r--r--   0        0        0     6753 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/ontologies/food.ttl
+-rw-r--r--   0        0        0     3166 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_add_function.py
+-rw-r--r--   0        0        0      880 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_collection.py
+-rw-r--r--   0        0        0      241 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_custom_backend.py
+-rw-r--r--   0        0        0     2455 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_get_data.py
+-rw-r--r--   0        0        0     4494 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_literals.py
+-rw-r--r--   0        0        0     1993 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_namespace.py
+-rw-r--r--   0        0        0     7895 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_triplestore.py
+-rw-r--r--   0        0        0     6168 2023-06-23 20:45:01.123170 tripper-0.2.6/tests/test_utils.py
+-rw-r--r--   0        0        0      749 2023-06-23 20:45:53.323165 tripper-0.2.6/tripper/__init__.py
+-rw-r--r--   0        0        0     1330 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/backends/__init__.py
+-rw-r--r--   0        0        0     2523 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/backends/collection.py
+-rw-r--r--   0        0        0     9177 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/backends/ontopy.py
+-rw-r--r--   0        0        0     7381 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/backends/rdflib.py
+-rw-r--r--   0        0        0     4144 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/backends/sparqlwrapper.py
+-rw-r--r--   0        0        0      362 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/errors.py
+-rw-r--r--   0        0        0     5401 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/interface.py
+-rw-r--r--   0        0        0     5671 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/literal.py
+-rw-r--r--   0        0        0      102 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/mappings/__init__.py
+-rw-r--r--   0        0        0    35669 2023-06-23 20:45:01.123170 tripper-0.2.6/tripper/mappings/mappings.py
+-rw-r--r--   0        0        0     6995 2023-06-23 20:45:01.127169 tripper-0.2.6/tripper/namespace.py
+-rw-r--r--   0        0        0    32594 2023-06-23 20:45:01.127169 tripper-0.2.6/tripper/triplestore.py
+-rw-r--r--   0        0        0    11004 2023-06-23 20:45:01.127169 tripper-0.2.6/tripper/tripper.py
+-rw-r--r--   0        0        0     8553 2023-06-23 20:45:01.127169 tripper-0.2.6/tripper/utils.py
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 tripper-0.2.6/PKG-INFO
```

### Comparing `tripper-0.2.5/.github/pull_request_template.md` & `tripper-0.2.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.github/workflows/cd_release.yml` & `tripper-0.2.6/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.github/workflows/ci_automerge_dependency_prs.yml` & `tripper-0.2.6/.github/workflows/ci_automerge_dependency_prs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.github/workflows/ci_cd_updated_main.yml` & `tripper-0.2.6/.github/workflows/ci_cd_updated_main.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.github/workflows/ci_check_dependencies.yml` & `tripper-0.2.6/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.github/workflows/ci_tests.yml` & `tripper-0.2.6/.github/workflows/ci_tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
   pytest:
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - name: Checkout tripper
       uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
```

### Comparing `tripper-0.2.5/.github/workflows/ci_update_dependencies.yml` & `tripper-0.2.6/.github/workflows/ci_update_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/.pre-commit-config.yaml` & `tripper-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/CHANGELOG.md` & `tripper-0.2.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 # Changelog
 
-## [v0.2.5](https://github.com/EMMC-ASBL/tripper/tree/v0.2.5) (2023-05-23)
+## [v0.2.6](https://github.com/EMMC-ASBL/tripper/tree/v0.2.6) (2023-06-23)
+
+[Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.5...v0.2.6)
+
+**Closed issues:**
+
+- Add CI/CD tests for Python 3.11 [\#102](https://github.com/EMMC-ASBL/tripper/issues/102)
+
+**Merged pull requests:**
+
+- One letter words where not allowed in mappings, now they are [\#117](https://github.com/EMMC-ASBL/tripper/pull/117) ([francescalb](https://github.com/francescalb))
+- pylint settings [\#115](https://github.com/EMMC-ASBL/tripper/pull/115) ([jesper-friis](https://github.com/jesper-friis))
+- Fix issue with entry points for Python 3.6 and 3.7 [\#113](https://github.com/EMMC-ASBL/tripper/pull/113) ([jesper-friis](https://github.com/jesper-friis))
+- Added DOI badge [\#109](https://github.com/EMMC-ASBL/tripper/pull/109) ([jesper-friis](https://github.com/jesper-friis))
+- Fixed parsing rdf:HTML literals with the rdflib backend [\#106](https://github.com/EMMC-ASBL/tripper/pull/106) ([jesper-friis](https://github.com/jesper-friis))
+- Support Python 3.11 [\#103](https://github.com/EMMC-ASBL/tripper/pull/103) ([jesper-friis](https://github.com/jesper-friis))
+- 92 new triplestore subclass [\#99](https://github.com/EMMC-ASBL/tripper/pull/99) ([alfredoisg](https://github.com/alfredoisg))
+
+## [v0.2.5](https://github.com/EMMC-ASBL/tripper/tree/v0.2.5) (2023-05-24)
 
 [Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.4...v0.2.5)
 
 ## [v0.2.4](https://github.com/EMMC-ASBL/tripper/tree/v0.2.4) (2023-04-30)
 
 [Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.3...v0.2.4)
```

### Comparing `tripper-0.2.5/LICENSE` & `tripper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/README.md` & `tripper-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 =======
 _Triplestore wrapper for Python providing a simple and consistent interface to a range of triplestore backends - the best ride when handling any triplestore._
 
 
 [![PyPI](https://img.shields.io/pypi/v/tripper?logo=pypi)](https://pypi.org/project/tripper)
 [![Documentation](https://img.shields.io/badge/documentation-informational?logo=github)](https://emmc-asbl.github.io/tripper/latest/)
 [![CI tests](https://github.com/EMMC-ASBL/tripper/workflows/CI%20-%20Tests/badge.svg)](https://github.com/EMMC-ASBL/tripper/actions/workflows/ci_tests.yml?query=branch%3Amain)
+[![DOI](https://zenodo.org/badge/547162834.svg)](https://zenodo.org/badge/latestdoi/547162834)
+
 
 
 Basic concepts
 --------------
 Tripper provides a simple and consistent interface to a range of triplestore backends.
 It strives for simplicity and is modelled after [rdflib] (with a few simplifications).
 
@@ -26,15 +28,14 @@
 
 To make it easy to work with IRIs, provide Tripper a set of pre-defined namespaces, like `XSD.float`.
 New namespaces can be defined with the [`tripper.Namespace`][Namespace] class.
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
-
 Documentation
 -------------
 * Getting started: See the [tutorial](docs/tutorial.md)
 * [Discovery of custom backends](docs/backend_discovery.md)
 * [Reference manual]
```

### Comparing `tripper-0.2.5/docs/backend_discovery.md` & `tripper-0.2.6/docs/backend_discovery.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/docs/index.md` & `tripper-0.2.6/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 =======
 _Triplestore wrapper for Python providing a simple and consistent interface to a range of triplestore backends - the best ride when handling any triplestore._
 
 
 [![PyPI](https://img.shields.io/pypi/v/tripper?logo=pypi)](https://pypi.org/project/tripper)
 [![Documentation](https://img.shields.io/badge/documentation-informational?logo=github)](https://emmc-asbl.github.io/tripper/latest/)
 [![CI tests](https://github.com/EMMC-ASBL/tripper/workflows/CI%20-%20Tests/badge.svg)](https://github.com/EMMC-ASBL/tripper/actions/workflows/ci_tests.yml?query=branch%3Amain)
+[![DOI](https://zenodo.org/badge/547162834.svg)](https://zenodo.org/badge/latestdoi/547162834)
+
 
 
 Basic concepts
 --------------
 Tripper provides a simple and consistent interface to a range of triplestore backends.
 It strives for simplicity and is modelled after [rdflib] (with a few simplifications).
 
@@ -26,15 +28,14 @@
 
 To make it easy to work with IRIs, provide Tripper a set of pre-defined namespaces, like `XSD.float`.
 New namespaces can be defined with the [`tripper.Namespace`][Namespace] class.
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
-
 Documentation
 -------------
 * Getting started: See the [tutorial](tutorial.md)
 * [Discovery of custom backends](backend_discovery.md)
 * [Reference manual]
```

### Comparing `tripper-0.2.5/docs/mappings/figs/function_emmo.svg` & `tripper-0.2.6/docs/mappings/figs/function_emmo.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/docs/tutorial.md` & `tripper-0.2.6/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/README.md` & `tripper-0.2.6/examples/workflow-mappings/README.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/knowledge-base.svg` & `tripper-0.2.6/examples/workflow-mappings/knowledge-base.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/route.svg` & `tripper-0.2.6/examples/workflow-mappings/route.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/workflow.svg` & `tripper-0.2.6/examples/workflow-mappings/workflow.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/workflow_mappings.py` & `tripper-0.2.6/examples/workflow-mappings/workflow_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/examples/workflow-mappings/workflow_w_pipes.svg` & `tripper-0.2.6/examples/workflow-mappings/workflow_w_pipes.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/mkdocs.yml` & `tripper-0.2.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/pyproject.toml` & `tripper-0.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Environment :: Plugins",
     "Natural Language :: English",
     "Operating System :: OS Independent",
 ]
 keywords = ["triplestore", "ontology", "RDF"]
 requires-python = "~=3.7"
 dynamic = ["version"]
@@ -32,75 +33,83 @@
 
 [project.optional-dependencies]
 docs = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
     "mkdocs-awesome-pages-plugin ~=2.9",
     "mkdocs-material ~=9.1",
-    "mkdocstrings[python-legacy] ~=0.21.2",
+    "mkdocstrings[python-legacy] ~=0.22.0",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.19,<1",
+    "DLite-Python >=0.3.20,<1",
 ]
 pre-commit = [
     "pre-commit ~=2.21",
     "pylint ~=2.13",
 ]
 testing = [
     "pytest ~=7.3",
-    "pytest-cov ~=4.0",
+    "pytest-cov ~=4.1",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.19,<1",
+    "DLite-Python >=0.3.20,<1",
 ]
 dev = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
     "mkdocs-awesome-pages-plugin ~=2.9",
     "mkdocs-material ~=9.1",
-    "mkdocstrings[python-legacy] ~=0.21.2",
+    "mkdocstrings[python-legacy] ~=0.22.0",
     "pre-commit ~=2.21",
     "pylint ~=2.13",
     "pytest ~=7.3",
-    "pytest-cov ~=4.0",
+    "pytest-cov ~=4.1",
     "EMMOntoPy ~=0.5",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.19,<1",
+    "DLite-Python >=0.3.20,<1",
 ]
 
 [project.urls]
 Home = "https://github.com/EMMC-ASBL/tripper"
 Documentation = "https://EMMC-ASBL.github.io/tripper"
 Source = "https://github.com/EMMC-ASBL/tripper"
 "Issue Tracker" = "https://github.com/EMMC-ASBL/tripper/issues"
 Changelog = "https://github.com/EMMC-ASBL/tripper/blob/main/CHANGELOG.md"
 Package = "https://pypi.org/project/tripper"
 
+[tool.isort]
+line_length = 79  # PEP8
+
+[tool.black]
+line-length = 79
+
 [tool.mypy]
 python_version = "3.7"
 ignore_missing_imports = true
 scripts_are_modules = true
 warn_unused_configs = true
 show_error_codes = true
 allow_redefinition = true
 
-[tool.pylint.messages_control]
-max-line-length = 88
+[tool.pylint]
+max-line-length = 79
 max-args = 10
 max-public-methods = 25
 max-locals = 20
 disable = [
     "fixme",
 ]
 good-names = [
     # Default
     "i", "j", "k", "ex", "Run", "_",
+    # Triplestore instance
+    "ts",
     # Triple components: subject, predicate, object
     "s", "p", "o",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-rs --cov=tripper --cov-report=term"
```

### Comparing `tripper-0.2.5/tests/conftest.py` & `tripper-0.2.6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,42 +6,47 @@
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any, Callable
 
 
 @pytest.fixture(scope="session")
 def get_ontology_path() -> "Callable[[str], Path]":
-    """Return a function to retrieve a Path object to a Turtle file used for testing.
+    """Return a function to retrieve a Path object to a Turtle file used
+    for testing.
 
-    This fixture will be called once during the test session and will then be cached.
+    This fixture will be called once during the test session and will then
+    be cached.
 
     Returns:
-        A function that can retrieve a Path object to a static ontology test file.
+        A function that can retrieve a Path object to a static ontology test
+    file.
 
     """
     from pathlib import Path
 
     ontologies_dir = Path(__file__).resolve().parent / "ontologies"
 
     def _get_ontology_path(ontology_name: str) -> "Path":
         """Return a Path object to at Turtle file used for testing.
 
         Parameters:
-            ontology_name: The ontology file base name to retrieve from the list of
-                static ontology test files.
+            ontology_name: The ontology file base name to retrieve from the
+                list of static ontology test files.
+
 
         Returns:
             A `pathlib.Path` instance, representing the ontology test file.
 
         """
         ontology_path = ontologies_dir / f"{ontology_name}.ttl"
         if ontology_path.exists():
             return ontology_path
         raise ValueError(
-            f"{ontology_name}.ttl does not exist in the 'ontologies' test folder."
+            f"{ontology_name}.ttl does not exist in the 'ontologies' test "
+            f"folder."
         )
 
     return _get_ontology_path
 
 
 @pytest.fixture
 def example_function() -> "Callable[[Any, Any], Any]":
@@ -56,15 +61,17 @@
         """Returns the sum of `first_param` and `second_param`."""
         return first_param + second_param
 
     return sum_
 
 
 @pytest.fixture
-def expected_function_triplestore(example_function: "Callable[[Any, Any], Any]") -> str:
+def expected_function_triplestore(
+    example_function: "Callable[[Any, Any], Any]",
+) -> str:
     """The expected Turtle-serialized output of a Triplestore.
 
     Parameters:
         example_function: Pytest fixture found in `conftest.py`.
             This becomes a function implementation that can be used with the
             Triplestore.
```

### Comparing `tripper-0.2.5/tests/mappings/test_function.py` & `tripper-0.2.6/tests/mappings/test_function.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 We also have two mapping functions; first() and sum()
   - first(): ex:B[0] -> ex:C
   - sum(): ex:A + ex:C -> ex:D
 
 The test asks for the value of an individual of ex:D
 """
 # pylint: disable=unused-argument,invalid-name
-from tripper import Literal, Triplestore
+from tripper import Literal, Tripper
 
-ts = Triplestore(backend="rdflib")
-EX = ts.bind("ex", "http://example.com/onto#")
+tp = Tripper(backend="rdflib")
+EX = tp.bind("ex", "http://example.com/onto#")
 
 
 def first(vector):
     """Return first element of the vector."""
     return vector[0]
 
 
@@ -28,15 +28,15 @@
 
 
 def vector(iri, configurations, triplestore):
     """Return a vector."""
     return [0.5, 1.2, 3.4, 6.6]
 
 
-ts.add_data(Literal(3.2), EX.A)
-ts.add_data(vector, EX.B)
+tp.add_data(Literal(3.2), EX.A)
+tp.add_data(vector, EX.B)
 
-ts.add_function(first, expects=EX.B, returns=EX.C)
-ts.add_function(add, expects=(EX.A, EX.C), returns=EX.D)
+tp.add_function(first, expects=EX.B, returns=EX.C)
+tp.add_function(add, expects=(EX.A, EX.C), returns=EX.D)
 
-ts.map(EX.indv, EX.D)
-assert ts.get_value(EX.indv) == 3.7
+tp.map(EX.indv, EX.D)
+assert tp.get_value(EX.indv) == 3.7
```

### Comparing `tripper-0.2.5/tests/mappings/test_mappings.py` & `tripper-0.2.6/tests/mappings/test_mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 routes = mapping_routes(
     target=SUB.molecule_energy,
     sources={MOL.groundstate_energy: 1.0},
     triplestore=ts,
 )
 
 assert routes.number_of_routes() == 1
-assert routes.output_iri == ("http://onto-ns.com/meta/0.1/Substance#molecule_energy")
+assert routes.output_iri == (
+    "http://onto-ns.com/meta/0.1/Substance#molecule_energy"
+)
 assert routes.cost == 2.0
 assert (
     routes.visualise(0).strip()
     == """
 digraph G {
   "mol:groundstate_energy" -> "chem:GroundStateEnergy" [label="mapsTo"];
   "chem:GroundStateEnergy" -> "sub:molecule_energy" [label="inverse(mapsTo)"];
```

### Comparing `tripper-0.2.5/tests/ontologies/family.ttl` & `tripper-0.2.6/tests/ontologies/family.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/tests/ontologies/food.ttl` & `tripper-0.2.6/tests/ontologies/food.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/tests/test_add_function.py` & `tripper-0.2.6/tests/test_add_function.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/tests/test_collection.py` & `tripper-0.2.6/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/tests/test_get_data.py` & `tripper-0.2.6/tests/test_get_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test Triplestore.get_data() and related methods."""
 # pylint: disable=unused-argument,invalid-name
 import numpy as np
 
-from tripper import Literal, Triplestore
+from tripper import Literal, Tripper
 from tripper.mappings import Value
 
 
 def get_lengths(iri, configurations, triplestore):
     """Return data from a data source. Here a length with unit."""
     return Value([1, 7, 2, 3], unit="m")
 
@@ -27,47 +27,51 @@
 
 
 def ycoords(iri, configurations, triplestore):
     """Return data from a data source. Here a list of voltages."""
     return Value(value=[0, 4, 16, 36, 64, 100], unit="V")
 
 
-ts = Triplestore(backend="rdflib")
-EX = ts.bind("ex", "http://example.com/onto#")
+tp = Tripper(backend="rdflib")
+EX = tp.bind("ex", "http://example.com/onto#")
 
-string_iri = ts.add_data(Literal("string value"), EX.Description)
-number_iri = ts.add_data(Literal(3.14), EX.WellKnownNumber)
-length_iri = ts.add_data(get_lengths, EX.Length)
-string2_iri = ts.add_data(get_string, EX.String)
-xcoords_iri = ts.add_data(xcoords)
-ycoords_iri = ts.add_data(ycoords)
-
-assert ts.get_value(string_iri) == "string value"
-assert ts.get_value(number_iri) == 3.14
-assert np.allclose(ts.get_value(length_iri).m, [1, 7, 2, 3])
-assert ts.get_value(string2_iri) == "a string"
-assert np.allclose(ts.get_value(xcoords_iri).m, [0, 2, 4, 6, 8, 10])
-assert np.allclose(ts.get_value(xcoords_iri, magnitude=True), [0, 2, 4, 6, 8, 10])
-assert np.allclose(ts.get_value(xcoords_iri, unit="dm"), [0, 20, 40, 60, 80, 100])
-assert np.allclose(ts.get_value(ycoords_iri).m, [0, 4, 16, 36, 64, 100])
+string_iri = tp.add_data(Literal("string value"), EX.Description)
+number_iri = tp.add_data(Literal(3.14), EX.WellKnownNumber)
+length_iri = tp.add_data(get_lengths, EX.Length)
+string2_iri = tp.add_data(get_string, EX.String)
+xcoords_iri = tp.add_data(xcoords)
+ycoords_iri = tp.add_data(ycoords)
+
+assert tp.get_value(string_iri) == "string value"
+assert tp.get_value(number_iri) == 3.14
+assert np.allclose(tp.get_value(length_iri).m, [1, 7, 2, 3])
+assert tp.get_value(string2_iri) == "a string"
+assert np.allclose(tp.get_value(xcoords_iri).m, [0, 2, 4, 6, 8, 10])
+assert np.allclose(
+    tp.get_value(xcoords_iri, magnitude=True), [0, 2, 4, 6, 8, 10]
+)
+assert np.allclose(
+    tp.get_value(xcoords_iri, unit="dm"), [0, 20, 40, 60, 80, 100]
+)
+assert np.allclose(tp.get_value(ycoords_iri).m, [0, 4, 16, 36, 64, 100])
 
 
 # Test get_value() via mappings
-ts.map(EX.indv, EX.Description)
-assert ts.get_value(EX.indv) == "string value"
+tp.map(EX.indv, EX.Description)
+assert tp.get_value(EX.indv) == "string value"
 
-ts.map(EX.indv2, EX.WellKnownNumber)
-assert ts.get_value(EX.indv2) == 3.14
+tp.map(EX.indv2, EX.WellKnownNumber)
+assert tp.get_value(EX.indv2) == 3.14
 
-ts.map(EX.indv3, EX.Length)
-q3 = ts.get_value(EX.indv3)
+tp.map(EX.indv3, EX.Length)
+q3 = tp.get_value(EX.indv3)
 assert np.allclose(q3.m, [1, 7, 2, 3])
 assert np.allclose(q3.m_as("dm"), [10, 70, 20, 30])
 
-ts.map(EX.indv4, EX.String)
-assert ts.get_value(EX.indv4) == "a string"
+tp.map(EX.indv4, EX.String)
+assert tp.get_value(EX.indv4) == "a string"
 
 
 # Test interpolation source
-ts.add_interpolation_source(xcoords_iri, ycoords_iri, EX.Length, EX.Voltage)
-ts.map(EX.indv5, EX.Voltage)
-assert np.allclose(ts.get_value(EX.indv5).m, [2, 50, 4, 10])
+tp.add_interpolation_source(xcoords_iri, ycoords_iri, EX.Length, EX.Voltage)
+tp.map(EX.indv5, EX.Voltage)
+assert np.allclose(tp.get_value(EX.indv5).m, [2, 50, 4, 10])
```

### Comparing `tripper-0.2.5/tests/test_literals.py` & `tripper-0.2.6/tests/test_literals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Test RDF literals."""
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name,too-many-statements
 
 
 def test_string() -> None:
     """Test creating a string literal."""
     from tripper.literal import Literal
 
     literal = Literal("Hello world!")
@@ -71,15 +71,15 @@
     assert name == "subClassOf"
 
 
 def test_parse_literal() -> None:
     """Test parse n3-encoded literal value."""
     from datetime import datetime
 
-    from tripper import XSD, Literal
+    from tripper import RDF, XSD, Literal
     from tripper.utils import parse_literal
 
     literal = parse_literal(Literal("abc").n3())
     assert literal.value == "abc"
     assert literal.lang is None
     assert literal.datatype == XSD.string
 
@@ -129,7 +129,22 @@
     assert literal.lang is None
     assert literal.datatype == XSD.double
 
     literal = parse_literal(False)
     assert literal.value is False
     assert literal.lang is None
     assert literal.datatype == XSD.boolean
+
+    literal = parse_literal(f'"text"^^{RDF.HTML}')
+    assert literal.value == "text"
+    assert literal.lang is None
+    assert literal.datatype == RDF.HTML
+
+    literal = parse_literal(f'"text"^^<{RDF.HTML}>')
+    assert literal.value == "text"
+    assert literal.lang is None
+    assert literal.datatype == RDF.HTML
+
+    literal = parse_literal('"value"^^http://example.com/vocab#mytype')
+    assert literal.value == "value"
+    assert literal.lang is None
+    assert literal.datatype == "http://example.com/vocab#mytype"
```

### Comparing `tripper-0.2.5/tests/test_namespace.py` & `tripper-0.2.6/tests/test_namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     from typing import Callable
 
 
 def test_namespaces(get_ontology_path: "Callable[[str], Path]") -> None:
     """Test namespaces.
 
     Parameters:
-        get_ontology_path: Fixture from `conftest.py` to retrieve a `pathlib.Path`
-            object pointing to an ontology test file.
+        get_ontology_path: Fixture from `conftest.py` to retrieve a
+            `pathlib.Path` object pointing to an ontology test file.
 
     """
     from tripper import RDF, Namespace
     from tripper.errors import NoSuchIRIError
 
     assert str(RDF) == "http://www.w3.org/1999/02/22-rdf-syntax-ns#"
     assert RDF.type == "http://www.w3.org/1999/02/22-rdf-syntax-ns#type"
```

### Comparing `tripper-0.2.5/tests/test_triplestore.py` & `tripper-0.2.6/tests/test_triplestore.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,31 @@
 ) -> None:
     """Test the Triplestore class.
 
     Parameters:
         backend: Dynamic parameter based on the parametrize decorator.
         example_function: Fixture from `conftest.py` to return a function
             implementation example for use with Triplestore.
-        expected_function_triplestore: Fixture from `conftest.py`, which returns a
-            Turtle-serialized string of what is expected when serializing the
-            Triplestore in this test.
+        expected_function_triplestore: Fixture from `conftest.py`, which
+            returns a Turtle-serialized string of what is expected when
+            serializing the Triplestore in this test.
 
     """
     from tripper.triplestore import DCTERMS, OWL, RDF, RDFS, XSD, Triplestore
 
     ts = Triplestore(backend)
     assert ts.expand_iri("xsd:integer") == XSD.integer
     assert ts.prefix_iri(RDF.type) == "rdf:type"
-    EX = ts.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
+    EX = ts.bind(
+        "ex", "http://example.com/onto#"
+    )  # pylint: disable=invalid-name
     assert str(EX) == "http://example.com/onto#"
-    ts.add_mapsTo(EX.MyConcept, "http://onto-ns.com/meta/0.1/MyEntity", "myprop")
+    ts.add_mapsTo(
+        EX.MyConcept, "http://onto-ns.com/meta/0.1/MyEntity", "myprop"
+    )
     ts.add((EX.MyConcept, RDFS.subClassOf, OWL.Thing))
     ts.add((EX.AnotherConcept, RDFS.subClassOf, OWL.Thing))
     ts.add((EX.Sum, RDFS.subClassOf, OWL.Thing))
     assert ts.has(EX.Sum) is True
     assert ts.has(EX.Sum, RDFS.subClassOf, OWL.Thing) is True
     assert ts.has(object=EX.NotInOntology) is False
 
@@ -81,40 +85,45 @@
             "http://example.com/onto#Sum",
             "http://www.w3.org/2002/07/owl#Thing",
         )
 
     # Test value() method
     assert ts.value(func_iri, DCTERMS.description) == example_function.__doc__
     assert (
-        ts.value(func_iri, DCTERMS.description, lang="en") == example_function.__doc__
+        ts.value(func_iri, DCTERMS.description, lang="en")
+        == example_function.__doc__
     )
     assert ts.value(func_iri, DCTERMS.description, lang="de") is None
 
 
 def test_backend_rdflib(expected_function_triplestore: str) -> None:
     """Specifically test the rdflib backend Triplestore.
 
     Parameters:
-        expected_function_triplestore: Fixture from `conftest.py`, which returns a
-            Turtle-serialized string of what is expected when serializing the
-            Triplestore in this test.
+        expected_function_triplestore: Fixture from `conftest.py`, which
+            returns a Turtle-serialized string of what is expected when
+            serializing the Triplestore in this test.
 
     """
     from tripper.triplestore import RDFS, Triplestore
 
     ts = Triplestore("rdflib")
-    EX = ts.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
+    EX = ts.bind(
+        "ex", "http://example.com/onto#"
+    )  # pylint: disable=invalid-name
     ts.parse(format="turtle", data=expected_function_triplestore)
     assert ts.serialize(format="turtle") == expected_function_triplestore
     ts.set((EX.AnotherConcept, RDFS.subClassOf, EX.MyConcept))
 
     def cost(parameter):
         return 2 * parameter
 
-    ts.add_mapsTo(EX.Sum, "http://onto-ns.com/meta/0.1/MyEntity#sum", cost=cost)
+    ts.add_mapsTo(
+        EX.Sum, "http://onto-ns.com/meta/0.1/MyEntity#sum", cost=cost
+    )
     assert list(ts.function_repo.values())[0] == cost
 
     def func(parameter):
         return parameter + 1
 
     ts.add_function(func, expects=EX.Sum, returns=EX.OneMore, cost=cost)
     assert list(ts.function_repo.values())[1] == func
@@ -132,18 +141,18 @@
 
 def test_backend_rdflib_base_iri(
     get_ontology_path: "Callable[[str], Path]", tmp_path: "Path"
 ) -> None:
     """Test rdflib with `base_iri`.
 
     Parameters:
-        get_ontology_path: Fixture from `conftest.py` to retrieve a `pathlib.Path`
-            object pointing to an ontology test file.
-        tmp_path: Built-in pytest fixture, which returns a `pathlib.Path` object
-            representing a temporary folder.
+        get_ontology_path: Fixture from `conftest.py` to retrieve a
+            `pathlib.Path` object pointing to an ontology test file.
+        tmp_path: Built-in pytest fixture, which returns a `pathlib.Path`
+            object representing a temporary folder.
 
     """
     import shutil
 
     from tripper.triplestore import RDF, Triplestore
 
     ontopath_family = get_ontology_path("family")
@@ -164,16 +173,16 @@
     ts.close()
 
 
 def test_backend_ontopy(get_ontology_path: "Callable[[str], Path]") -> None:
     """Specifically test the ontopy backend Triplestore.
 
     Parameters:
-        get_ontology_path: Fixture from `conftest.py` to retrieve a `pathlib.Path`
-            object pointing to an ontology test file.
+        get_ontology_path: Fixture from `conftest.py` to retrieve a
+            `pathlib.Path` object pointing to an ontology test file.
 
     """
     from tripper import Namespace, Triplestore
 
     ontopath_food = get_ontology_path("food")
 
     FOOD = Namespace(  # pylint: disable=invalid-name
@@ -201,33 +210,36 @@
 def test_backend_sparqlwrapper() -> None:
     """Specifically test the SPARQLWrapper backend Triplestore."""
     from tripper import SKOS, Triplestore
 
     ts = Triplestore(
         backend="sparqlwrapper",
         base_iri="http://vocabs.ardc.edu.au/repository/api/sparql/"
-        "csiro_international-chronostratigraphic-chart_geologic-time-scale-2020",
+        "csiro_international-chronostratigraphic-chart_geologic-"
+        "time-scale-2020",
     )
     for s, p, o in ts.triples(predicate=SKOS.notation):
         assert s
         assert p
         assert o
 
 
 @pytest.mark.skip(
-    "These will fail because we do not have credentials to modify the triplestore"
+    "These will fail because we do not have credentials to modify the "
+    "triplestore"
 )
 def test_backend_sparqlwrapper_methods() -> None:
     """Test SPARQLWrapper methods."""
     from tripper import RDFS, SKOS, Literal, Namespace, Triplestore
 
     ts = Triplestore(
         backend="sparqlwrapper",
         base_iri="http://vocabs.ardc.edu.au/repository/api/sparql/"
-        "csiro_international-chronostratigraphic-chart_geologic-time-scale-2020",
+        "csiro_international-chronostratigraphic-chart_geologic-"
+        "time-scale-2020",
     )
 
     ts.remove((None, SKOS.notation, None))
 
     EX = Namespace("http://example.com#")  # pylint: disable=invalid-name
     ts.add_triples(
         [
```

### Comparing `tripper-0.2.5/tests/test_utils.py` & `tripper-0.2.6/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,34 +31,41 @@
 else:
     from typing import Any, Optional
 
     class Property(BaseModel):
         """A property."""
 
         # pylint: disable=unsubscriptable-object
-        # Yet another pylint bug, see https://github.com/PyCQA/pylint/issues/1498
+        # Yet another pylint bug, see
+        # https://github.com/PyCQA/pylint/issues/1498
         type: Any = Field(..., description="Valid type name.")
         shape: Optional[list[str]] = Field(
             None, description="List of dimension expressions."
         )
         unit: Optional[str] = Field(None, description="Unit of a property.")
         description: Optional[str] = Field(
             None, description="A human description of the property."
         )
 
     class Entity(BaseModel):
         """An entity."""
 
         # pylint: disable=unsubscriptable-object
-        identity: AnyUrl = Field(..., description="Unique URI identifying the entity.")
-        description: str = Field("", description="A description of the entity.")
+        identity: AnyUrl = Field(
+            ..., description="Unique URI identifying the entity."
+        )
+        description: str = Field(
+            "", description="A description of the entity."
+        )
         dimensions: Optional[dict[str, str]] = Field(
             None, description="Dict mapping dimension names to descriptions."
         )
-        properties: dict[str, Property] = Field(..., description="Dict of properties.")
+        properties: dict[str, Property] = Field(
+            ..., description="Dict of properties."
+        )
 
     user = Entity(
         identity="http://onto-ns.com/meta/0.1/User",
         properties={
             "username": Property(type=str, description="username"),
             "quota": Property(type=float, unit="GB", description="User quota"),
         },
@@ -110,15 +117,17 @@
 assert en("abc") == Literal("abc", lang="en")
 
 # test parse_literal()
 assert parse_literal("abc") == Literal("abc", datatype=XSD.string)
 assert parse_literal(True) == Literal("True", datatype=XSD.boolean)
 assert parse_literal(1) == Literal("1", datatype=XSD.integer)
 assert parse_literal(3.14) == Literal("3.14", datatype=XSD.double)
-assert parse_literal(f'"3.14"^^{XSD.double}') == Literal("3.14", datatype=XSD.double)
+assert parse_literal(f'"3.14"^^{XSD.double}') == Literal(
+    "3.14", datatype=XSD.double
+)
 
 
 # test parse_object()
 assert parse_object("true") == Literal("true", datatype=XSD.boolean)
 assert parse_object("false") == Literal("false", datatype=XSD.boolean)
 assert parse_object("True") == Literal("True", datatype=XSD.string)
 assert parse_object("0") == Literal("0", datatype=XSD.integer)
@@ -130,15 +139,17 @@
 assert parse_object("1.") == Literal("1.", datatype=XSD.double)
 assert parse_object("1e10") == Literal("1e10", datatype=XSD.double)
 assert parse_object("1E10") == Literal("1E10", datatype=XSD.double)
 assert parse_object("1e+10") == Literal("1e+10", datatype=XSD.double)
 assert parse_object("1e-10") == Literal("1e-10", datatype=XSD.double)
 assert parse_object(".1e10") == Literal(".1e10", datatype=XSD.double)
 assert parse_object("1.e10") == Literal("1.e10", datatype=XSD.double)
-assert parse_object("2022-12-01") == Literal("2022-12-01", datatype=XSD.dateTime)
+assert parse_object("2022-12-01") == Literal(
+    "2022-12-01", datatype=XSD.dateTime
+)
 assert parse_object("2022-12-01 12:30") == Literal(
     "2022-12-01 12:30", datatype=XSD.dateTime
 )
 assert parse_object("2022-12-01 12:30:30") == Literal(
     "2022-12-01 12:30:30", datatype=XSD.dateTime
 )
 assert parse_object("2022-12-01T12:30:30") == Literal(
@@ -154,17 +165,23 @@
 assert parse_object("2022-12-01 12:30:30+01:00") == Literal(
     "2022-12-01 12:30:30+01:00", datatype=XSD.dateTime
 )
 assert parse_object("abc") == Literal("abc", datatype=XSD.string)
 assert parse_object('"abc"@en') == Literal("abc", lang="en")
 assert parse_object(str(XSD)) == str(XSD)
 assert parse_object(XSD.int) == XSD.int
-assert parse_object(f'"42"^^{XSD.integer}') == Literal("42", datatype=XSD.integer)
-assert parse_object(f'"4.2"^^{XSD.double}') == Literal("4.2", datatype=XSD.double)
-assert parse_object(f'"42"^^{XSD.double}') == Literal("42.0", datatype=XSD.double)
+assert parse_object(f'"42"^^{XSD.integer}') == Literal(
+    "42", datatype=XSD.integer
+)
+assert parse_object(f'"4.2"^^{XSD.double}') == Literal(
+    "4.2", datatype=XSD.double
+)
+assert parse_object(f'"42"^^{XSD.double}') == Literal(
+    "42.0", datatype=XSD.double
+)
 assert parse_object(f'"42"^^{XSD.int}') == Literal("42", datatype=XSD.int)
 
 
 # test as_python()
 assert as_python("abc") == "abc"
 assert as_python('"abc"@en') == "abc"
 assert as_python(f'"42"^^{XSD.double}') == 42
```

### Comparing `tripper-0.2.5/tripper/__init__.py` & `tripper-0.2.6/tripper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     RDFS,
     SKOS,
     XML,
     XSD,
     Namespace,
 )
 from .triplestore import Triplestore, backend_packages
+from .tripper import Tripper
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 __all__ = (
     "Literal",
     #
     "DC",
     "DCTERMS",
     "DM",
@@ -42,8 +43,9 @@
     "SKOS",
     "XML",
     "XSD",
     "Namespace",
     #
     "Triplestore",
     "backend_packages",
+    "Tripper",
 )
```

### Comparing `tripper-0.2.5/tripper/backends/__init__.py` & `tripper-0.2.6/tripper/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.5/tripper/backends/collection.py` & `tripper-0.2.6/tripper/backends/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from tripper.literal import Literal
 from tripper.utils import parse_object
 
 try:
     import dlite
 except ImportError as exc:
     raise ImportError(
-        "DLite is not installed.\nInstall it with:\n\n    pip install DLite-Python"
+        "DLite is not installed.\nInstall it with:\n\n"
+        "    pip install DLite-Python"
     ) from exc
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Sequence
     from typing import Generator, List, Optional, Union
 
     from tripper.triplestore import Triple
@@ -46,15 +47,17 @@
                 raise TypeError(
                     f"expected '{collection}' to be a collection, was a "
                     f"{self.collection.meta.uri}"
                 )
         elif isinstance(collection, dlite.Collection):
             self.collection = collection
         else:
-            raise TypeError("`collection` should be None, string or a collection")
+            raise TypeError(
+                "`collection` should be None, string or a collection"
+            )
 
     def triples(self, triple: "Triple") -> "Generator[Triple, None, None]":
         """Returns a generator over matching triples."""
         for s, p, o in self.collection.get_relations(*triple):
             yield s, p, parse_object(o)
 
     def add_triples(self, triples: "Sequence[Triple]"):
```

### Comparing `tripper-0.2.5/tripper/backends/ontopy.py` & `tripper-0.2.6/tripper/backends/ontopy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Backend for EMMOntoPy.
 
-For developers: The usage of `s`, `p`, and `o` represent the different parts of an
-RDF Triple: subject, predicate, and object.
+For developers: The usage of `s`, `p`, and `o` represent the different parts of
+an RDF Triple: subject, predicate, and object.
 """
 # pylint: disable=protected-access
 import os
 import tempfile
 from typing import TYPE_CHECKING
 
 from tripper.literal import Literal
 
 try:
     from ontopy.ontology import Ontology, _unabbreviate, get_ontology
 except ImportError as exc:
     raise ImportError(
-        "EMMOntoPy is not installed.\nInstall it with:\n\n    pip install EMMOntoPy"
+        "EMMOntoPy is not installed.\nInstall it with:\n\n"
+        "    pip install EMMOntoPy"
     ) from exc
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Sequence
     from typing import Generator, List, Optional, Union
 
     from rdflib.query import Result
@@ -79,15 +80,17 @@
         )
         for s, p, o in self.onto._get_obj_triples_spo_spo(*abb):
             yield (
                 _unabbreviate(self.onto, s),
                 _unabbreviate(self.onto, p),
                 _unabbreviate(self.onto, o),
             )
-        for s, p, o, datatype in self.onto._get_data_triples_spod_spod(*abb, d=""):
+        for s, p, o, datatype in self.onto._get_data_triples_spod_spod(
+            *abb, d=""
+        ):
             yield (
                 _unabbreviate(self.onto, s),
                 _unabbreviate(self.onto, p),
                 to_literal(o, datatype),
             )
 
     def add_triples(self, triples: "Sequence[Triple]"):
@@ -172,15 +175,17 @@
                     filename = handle.name
                 self.onto.load(filename=filename, format=format, **kwargs)
             finally:
                 if filename:
                     os.remove(filename)
 
         else:
-            raise ValueError("either `source`, `location` or `data` must be given")
+            raise ValueError(
+                "either `source`, `location` or `data` must be given"
+            )
 
     def serialize(
         self,
         destination=None,
         format="turtle",  # pylint: disable=redefined-builtin
         **kwargs,
     ) -> "Union[None, str]":
@@ -208,15 +213,17 @@
                 with open(filename, "rt", encoding="utf8") as handle:
                     return handle.read()
             finally:
                 if filename:
                     os.remove(filename)
         return None
 
-    def query(self, query_object, native=True, **kwargs) -> "Union[List, Result]":
+    def query(
+        self, query_object, native=True, **kwargs
+    ) -> "Union[List, Result]":
         """SPARQL query.
 
         Parameters:
             query_object: String with the SPARQL query.
             native: Whether or not to use EMMOntoPy/Owlready2 or RDFLib.
             kwargs: Keyword arguments passed to rdflib.Graph.query().
```

### Comparing `tripper-0.2.5/tripper/backends/rdflib.py` & `tripper-0.2.6/tripper/backends/rdflib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Backend for RDFLib.
 
-For developers: The usage of `s`, `p`, and `o` represent the different parts of an
-RDF Triple: subject, predicate, and object.
+For developers: The usage of `s`, `p`, and `o` represent the different parts of
+an RDF Triple: subject, predicate, and object.
 """
 # pylint: disable=line-too-long
 import warnings
 from typing import TYPE_CHECKING
 
 try:
     import rdflib  # pylint: disable=unused-import
@@ -16,29 +16,31 @@
 
 from rdflib import BNode, Graph
 from rdflib import Literal as rdflibLiteral
 from rdflib import URIRef
 from rdflib.util import guess_format
 
 from tripper import Literal
-from tripper.utils import UnusedArgumentWarning
+from tripper.utils import UnusedArgumentWarning, parse_literal
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Sequence
     from typing import Generator, List, Optional, Tuple, Union
 
     from tripper.triplestore import Triple
 
 
 def asuri(value: "Union[None, Literal, str]"):
     """Help function converting a spo-value to proper rdflib type."""
     if value is None:
         return None
     if isinstance(value, Literal):
-        return rdflibLiteral(value.value, lang=value.lang, datatype=value.datatype)
+        return rdflibLiteral(
+            value.value, lang=value.lang, datatype=value.datatype
+        )
     if value.startswith("_:"):
         return BNode(value)
     return URIRef(value)
 
 
 def astriple(triple: "Triple"):
     """Help function converting a triple to rdflib triple."""
@@ -82,21 +84,15 @@
         """Returns a generator over matching triples."""
         for s, p, o in self.graph.triples(  # pylint: disable=not-an-iterable
             astriple(triple)
         ):
             yield (
                 str(s),
                 str(p),
-                Literal(
-                    o.value,
-                    lang=o.language,
-                    datatype=str(o.datatype) if o.datatype else o.datatype,
-                )
-                if isinstance(o, rdflibLiteral)
-                else str(o),
+                parse_literal(o) if isinstance(o, rdflibLiteral) else str(o),
             )
 
     def add_triples(self, triples: "Sequence[Triple]"):
         """Add a sequence of triples."""
         for triple in triples:
             self.graph.add(astriple(triple))
 
@@ -104,15 +100,17 @@
         """Remove all matching triples from the backend."""
         self.graph.remove(astriple(triple))
 
     # Optional methods
     def close(self):
         """Close the internal RDFLib graph."""
         if self.triplestore_url:
-            self.serialize(destination=self.triplestore_url, format=self.base_format)
+            self.serialize(
+                destination=self.triplestore_url, format=self.base_format
+            )
         self.graph.close()
 
     def parse(
         self,
         source=None,
         location=None,
         data=None,
@@ -128,15 +126,19 @@
             location: String with relative or absolute URL to source.
             data: String containing the data to be parsed.
             format: Needed if format can not be inferred from source.
             kwargs: Additional less used keyword arguments.
                 See https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.parse
         """
         self.graph.parse(
-            source=source, location=location, data=data, format=format, **kwargs
+            source=source,
+            location=location,
+            data=data,
+            format=format,
+            **kwargs,
         )
 
     def serialize(
         self,
         destination=None,
         format="turtle",  # pylint: disable=redefined-builtin
         **kwargs,
@@ -149,15 +151,17 @@
             format: Format to serialise as. Supported formats, depends on the backend.
             kwargs: Passed to the rdflib.Graph.serialize() method.
                 See https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize
 
         Returns:
             Serialised string if `destination` is None.
         """
-        result = self.graph.serialize(destination=destination, format=format, **kwargs)
+        result = self.graph.serialize(
+            destination=destination, format=format, **kwargs
+        )
         if destination is None:
             # Depending on the version of rdflib the return value of
             # graph.serialize() man either be a string or a bytes object...
             return result if isinstance(result, str) else result.decode()
         return None
 
     def query(self, query_object, **kwargs) -> "List[Tuple[str, ...]]":
@@ -193,17 +197,22 @@
 
         Should only be defined if the backend supports namespaces.
         Called by triplestore.bind().
         """
         if namespace:
             self.graph.bind(prefix, namespace, replace=True)
         else:
-            warnings.warn("rdflib does not support removing namespace prefixes")
+            warnings.warn(
+                "rdflib does not support removing namespace prefixes"
+            )
 
     def namespaces(self) -> dict:
         """Returns a dict mapping prefixes to namespaces.
 
         Should only be defined if the backend supports namespaces.
         Used by triplestore.parse() to get prefixes after reading
         triples from an external source.
         """
-        return {prefix: str(namespace) for prefix, namespace in self.graph.namespaces()}
+        return {
+            prefix: str(namespace)
+            for prefix, namespace in self.graph.namespaces()
+        }
```

### Comparing `tripper-0.2.5/tripper/backends/sparqlwrapper.py` & `tripper-0.2.6/tripper/backends/sparqlwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         )
         self.sparql.setReturnFormat(JSON)
         self.sparql.setMethod(GET)
         self.sparql.setQuery(query)
         ret = self.sparql.queryAndConvert()
         for binding in ret["results"]["bindings"]:
             yield tuple(
-                convert_json_entrydict(binding[name]) if name in binding else value
+                convert_json_entrydict(binding[name])
+                if name in binding
+                else value
                 for name, value in zip("spo", triple)
             )
 
     def add_triples(self, triples: "Sequence[Triple]") -> "QueryResult":
         """Add a sequence of triples."""
         spec = "\n".join(
             "  "
```

### Comparing `tripper-0.2.5/tripper/interface.py` & `tripper-0.2.6/tripper/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,27 @@
 if sys.version_info < (3, 8):
     from typing_extensions import Protocol
 else:
     from typing import Protocol
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Sequence
-    from typing import Generator
+    from typing import Generator, Optional
 
     from tripper.triplestore import Triple
 
 
 class ITriplestore(Protocol):
     '''Interface for triplestore backends.
 
     In addition to the methods specified by this interface, a backend
     may also implement the following optional methods:
 
     ```python
 
-    def __init__(self, base_iri: str = None, **kwargs):
-        """Initialise triplestore.
-
-        Arguments:
-            base_iri: Optional base IRI to initiate the triplestore from.
-            kwargs: Additional keyword arguments passed to the backend.
-        """
-
     def parse(
             self,
             source: Union[str, Path, IO] = None,
             location: str = None,
             data: str = None,
             format: str = None,
             **kwargs
@@ -150,14 +142,22 @@
             This is a class method, which operates on the backend
             triplestore without connecting to it.
         """
 
     ```
     '''
 
+    def __init__(self, base_iri: "Optional[str]" = None, **kwargs):
+        """Initialise triplestore.
+
+        Arguments:
+            base_iri: Optional base IRI to initiate the triplestore from.
+            kwargs: Additional keyword arguments passed to the backend.
+        """
+
     def triples(self, triple: "Triple") -> "Generator":
         """Returns a generator over matching triples.
 
         Arguments:
             triple: A `(s, p, o)` tuple where `s`, `p` and `o` should
                 either be None (matching anything) or an exact IRI to
                 match.
```

### Comparing `tripper-0.2.5/tripper/literal.py` & `tripper-0.2.6/tripper/literal.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,24 @@
             XSD.negativeInteger,
             XSD.unsignedInt,
             XSD.unsignedShort,
             XSD.unsignedLong,
             XSD.byte,
             XSD.unsignedByte,
         ),
-        float: (XSD.double, XSD.decimal, XSD.dateTimeStamp, XSD.real, XSD.rational),
+        float: (
+            XSD.double,
+            XSD.decimal,
+            XSD.dateTimeStamp,
+            XSD.real,
+            XSD.rational,
+        ),
         str: (
             XSD.string,
+            RDF.HTML,
             RDF.PlainLiteral,
             RDF.XMLLiteral,
             RDFS.Literal,
             XSD.anyURI,
             XSD.language,
             XSD.Name,
             XSD.NMName,
@@ -67,15 +74,17 @@
         value: "Union[datetime, bytes, bytearray, bool, int, float, str]",
         lang: "Optional[str]" = None,
         datatype: "Optional[Any]" = None,
     ):
         string = super().__new__(cls, value)
         if lang:
             if datatype:
-                raise TypeError("A literal can only have one of `lang` or `datatype`.")
+                raise TypeError(
+                    "A literal can only have one of `lang` or `datatype`."
+                )
             string.lang = str(lang)
             string.datatype = None
         else:
             string.lang = None
             if datatype:
                 string.datatype = cls.datatypes.get(datatype, (datatype,))[0]
             elif isinstance(value, str):
@@ -83,16 +92,16 @@
             elif isinstance(value, bool):
                 string.datatype = XSD.boolean
             elif isinstance(value, int):
                 string.datatype = XSD.integer
             elif isinstance(value, float):
                 string.datatype = XSD.double
             elif isinstance(value, (bytes, bytearray)):
-                # Re-initialize the value anew, similarly to what is done in the first
-                # line of this method.
+                # Re-initialize the value anew, similarly to what is done in
+                # the first line of this method.
                 string = super().__new__(cls, value.hex())
                 string.lang = None
                 string.datatype = XSD.hexBinary
             elif isinstance(value, datetime):
                 string.datatype = XSD.dateTime
                 # TODO:
                 #   - XSD.base64Binary
@@ -141,15 +150,17 @@
         elif self.datatype in self.datatypes[float]:
             value = float(self)
         elif self.datatype == XSD.hexBinary:
             value = self.encode()
         elif self.datatype == XSD.dateTime:
             value = datetime.fromisoformat(self)
         elif self.datatype and self.datatype not in self.datatypes[str]:
-            warnings.warn(f"unknown datatype: {self.datatype} - assuming string")
+            warnings.warn(
+                f"unknown datatype: {self.datatype} - assuming string"
+            )
 
         return value
 
     def n3(self) -> str:  # pylint: disable=invalid-name
         """Returns a representation in n3 format."""
         if self.lang:
             return f'"{self}"@{self.lang}'
```

### Comparing `tripper-0.2.5/tripper/mappings/mappings.py` & `tripper-0.2.6/tripper/mappings/mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,16 @@
         argname = name if name else f"arg{len(self.joined_input)+1}"
         if self.join_mode:
             self.joined_input[argname] = input
         else:
             self.add_inputs({argname: input})
 
     def join_input(self) -> None:
-        """Join all input added with add_input() since `join_mode` was set true.
-        Resets `join_mode` to false."""
+        """Join all input added with add_input() since `join_mode` was set
+        true.  Resets `join_mode` to false."""
         if not self.join_mode:
             raise MappingError("Calling join_input() when join_mode is false.")
         self.join_mode = False
         self.add_inputs(self.joined_input)
         self.joined_input = {}
 
     def eval(
@@ -273,41 +273,47 @@
         if quantity is None:
             quantity = Quantity
         if routeno is None:
             ((_, routeno),) = self.lowest_costs(nresults=1)
         inputs, idx = self.get_inputs(routeno)
         values = get_values(inputs, idx, quantity=quantity)
 
-        if len(inputs) == 1 and all(isinstance(v, Value) for v in inputs.values()):
+        if len(inputs) == 1 and all(
+            isinstance(v, Value) for v in inputs.values()
+        ):
             (value,) = tuple(inputs.values())
         elif self.function:
             value = self.function(**values)
         elif len(values) == 1:
             (value,) = values.values()
         else:
-            raise TypeError(f"Expected inputs to be a single argument: {values}")
+            raise TypeError(
+                f"Expected inputs to be a single argument: {values}"
+            )
 
         if isinstance(value, Quantity) and unit:
             return value.m_as(unit)
         if isinstance(value, Quantity) and magnitude:
             return value.m
         if isinstance(value, Value):
-            return value.get_value(unit=unit, magnitude=magnitude, quantity=quantity)
+            return value.get_value(
+                unit=unit, magnitude=magnitude, quantity=quantity
+            )
         return value
 
     def get_inputs(self, routeno: int) -> "Tuple[Inputs, int]":
         """Returns input and input index `(inputs, idx)` for route number
         `routeno`.
 
         Arguments:
             routeno: The route number to return inputs for.
 
         Returns:
-            Inputs and difference between route number and number of routes for an
-            input dictioary.
+            Inputs and difference between route number and number of routes for
+            an input dictioary.
         """
         n = 0
         for inputs in self.input_routes:
             n0 = n
             n += get_nroutes(inputs)
             if n > routeno:
                 return inputs, routeno - n0
@@ -366,15 +372,17 @@
             #
             #     nresults * number_of_input_arguments
             #
             # possibilities. We calculate the costs for all of them and
             # store them in an array with two columns: `cost` and `routeno`.
             # The `results` list is extended with the cost array
             # for each toplevel route leading into this step.
-            base = np.rec.fromrecords([(0.0, 0)], names="cost,routeno", formats="f8,i8")
+            base = np.rec.fromrecords(
+                [(0.0, 0)], names="cost,routeno", formats="f8,i8"
+            )
             m = 1
             for input in inputs.values():
                 if isinstance(input, MappingStep):
                     nroutes = input.number_of_routes()
                     res = np.rec.fromrecords(
                         sorted(
                             input.lowest_costs(nresults=nresults),
@@ -407,16 +415,20 @@
             # Add the cost for this step to `res`.  If `self.cost` is
             # a callable, we call it with the input for each routeno
             # as arguments.  Otherwise `self.cost` is the cost of this
             # mapping step.
             if callable(self.cost):
                 for i, rno in enumerate(base.routeno):
                     inputs, _ = self.get_inputs(rno)
-                    input_iris = [input.output_iri for input in inputs.values()]
-                    owncost = self.cost(self.triplestore, input_iris, self.output_iri)
+                    input_iris = [
+                        input.output_iri for input in inputs.values()
+                    ]
+                    owncost = self.cost(
+                        self.triplestore, input_iris, self.output_iri
+                    )
                     base.cost[i] += owncost
             else:
                 owncost = self.cost
                 base.cost += owncost
 
             result.extend(base.tolist())
 
@@ -441,15 +453,16 @@
         Returns:
             String representation of the mapping routes.
         """
         strings = []
         ind = " " * indent
         strings.append(ind + f'{name if name else "Step"}:')
         strings.append(
-            ind + f"  steptype: " f"{self.steptype.name if self.steptype else None}"
+            ind + f"  steptype: "
+            f"{self.steptype.name if self.steptype else None}"
         )
         strings.append(ind + f"  output_iri: {self.output_iri}")
         strings.append(ind + f"  output_unit: {self.output_unit}")
         strings.append(ind + f"  cost: {self.cost}")
         if routeno is None:
             strings.append(ind + "  routes:")
             for inputs in self.input_routes:
@@ -469,18 +482,21 @@
                     for name_, input_ in inputs.items()
                 ]
             )
             strings.append(ind + "    - " + t[indent + 6 :])
         return "\n".join(strings)
 
     def _iri(self, iri: str) -> str:
-        """Help method that returns prefixed iri if possible, otherwise `iri`."""
+        """Help method that returns prefixed iri if possible, otherwise
+        `iri`."""
         return self.triplestore.prefix_iri(iri) if self.triplestore else iri
 
-    def _visualise(self, routeno: int, next_iri: str, next_steptype: StepType) -> str:
+    def _visualise(
+        self, routeno: int, next_iri: str, next_steptype: StepType
+    ) -> str:
         """Help function for visualise().
 
         Arguments:
             routeno: Route number to visualise.
             next_iri: IRI of the next mapping step (i.e. the previous mapping
                 when starting from the target).
             next_steptype: Step type from this to next iri.
@@ -624,24 +640,27 @@
             value = v.eval(routeno=routeno, quantity=quantity)
             values[k] = (
                 value.to(v.output_unit)
                 if v.output_unit and isinstance(v, quantity)
                 else value
             )
         elif isinstance(v, Value):
-            values[k] = v.value if v.unit is None else quantity(v.value, v.unit)
+            values[k] = (
+                v.value if v.unit is None else quantity(v.value, v.unit)
+            )
         else:
             raise TypeError(
                 "Expected values in inputs to be either `MappingStep` or "
                 "`Value` objects."
             )
 
         if magnitudes:
             values = {
-                k: v.m if isinstance(v, quantity) else v for k, v in values.items()
+                k: v.m if isinstance(v, quantity) else v
+                for k, v in values.items()
             }
 
     return values
 
 
 def emmo_mapper(triplestore: "Triplestore") -> "Dict[str, list]":
     """Finds all function definitions in `triplestore` based on EMMO.
@@ -669,15 +688,18 @@
     """Finds all function definitions in `triplestore` based on the function
     ontololy (FNO).
 
     Arguments:
         triplestore: The triplestore to investigate.
 
     Returns:
-        A mapping of output IRIs to a list of `(function_iri, [input_iris, ...])`
+        A mapping of output IRIs to a list of
+
+            (function_iri, [input_iris, ...])
+
         tuples.
     """
     # pylint: disable=too-many-branches
 
     # Temporary dicts for fast lookup
     Dfirst = dict(triplestore.subject_objects(RDF.first))
     Drest = dict(triplestore.subject_objects(RDF.rest))
@@ -719,15 +741,18 @@
 
 
 def mapping_routes(
     target: str,
     sources: "Union[Dict[str, Union[Value, None]], Sequence[str]]",
     triplestore: "Triplestore",
     function_repo: "Optional[dict]" = None,
-    function_mappers: "Union[str, Sequence[Callable]]" = (emmo_mapper, fno_mapper),
+    function_mappers: "Union[str, Sequence[Callable]]" = (
+        emmo_mapper,
+        fno_mapper,
+    ),
     default_costs: "Tuple" = (
         ("function", 10.0),
         ("mapsTo", 2.0),
         ("instanceOf", 1.0),
         ("subClassOf", 1.0),
         ("value", 0.0),
     ),
@@ -812,18 +837,24 @@
         value_class = Value
 
     if mappingstep_class is None:
         mappingstep_class = MappingStep
 
     # Create lookup tables for fast access to triplestore content
     soMaps = defaultdict(list)  # (s, mapsTo, o)     ==> soMaps[s]  -> [o, ..]
-    osMaps = defaultdict(list)  # (o, inv(mapsTo), s)     ==> osMaps[o]  -> [s, ..]
-    osSubcl = defaultdict(list)  # (o, inv(subClassOf), s) ==> osSubcl[o] -> [s, ..]
+    osMaps = defaultdict(
+        list
+    )  # (o, inv(mapsTo), s)     ==> osMaps[o]  -> [s, ..]
+    osSubcl = defaultdict(
+        list
+    )  # (o, inv(subClassOf), s) ==> osSubcl[o] -> [s, ..]
     soInst = {}  # (s, instanceOf, o) ==> soInst[s]  -> o
-    osInst = defaultdict(list)  # (o, inv(instanceOf), s) ==> osInst[o]  -> [s, ..]
+    osInst = defaultdict(
+        list
+    )  # (o, inv(instanceOf), s) ==> osInst[o]  -> [s, ..]
     for s, o in triplestore.subject_objects(mapsTo):
         soMaps[s].append(o)
         osMaps[o].append(s)
     for s, o in triplestore.subject_objects(subClassOf):
         osSubcl[o].append(s)
     for s, o in triplestore.subject_objects(instanceOf):
         if s in soInst:
@@ -842,15 +873,17 @@
     def getcost(target, stepname):
         """Returns the cost assigned to IRI `target` for a mapping step
         of type `stepname`."""
         cost = soCost.get(target, default_costs[stepname])
         if cost is None:
             return None
         return (
-            function_repo[cost] if cost in function_repo else float(parse_literal(cost))
+            function_repo[cost]
+            if cost in function_repo
+            else float(parse_literal(cost))
         )
 
     def walk(target, visited, step):
         """Walk backward in rdf graph from `node` to sources."""
         if target in visited:
             return
         visited.add(target)
```

### Comparing `tripper-0.2.5/tripper/namespace.py` & `tripper-0.2.6/tripper/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,19 @@
 
         self._iri = str(iri)
         self._label_annotations = tuple(label_annotations)
         self._check = bool(check)
 
         need_triplestore = bool(check or label_annotations)
         if cachemode == -1:
-            cachemode = Namespace.ONLY_CACHE if need_triplestore else Namespace.NO_CACHE
+            cachemode = (
+                Namespace.ONLY_CACHE
+                if need_triplestore
+                else Namespace.NO_CACHE
+            )
 
         if need_triplestore and triplestore is None:
             # Import Triplestore here to break cyclic-import
             from .triplestore import (  # pylint: disable=import-outside-toplevel,cyclic-import
                 Triplestore,
             )
 
@@ -88,15 +92,17 @@
             self._update_cache(triplestore)
 
     def _update_cache(self, triplestore=None):
         """Update the internal cache from `triplestore`."""
         if not triplestore:
             triplestore = self._triplestore
         if not triplestore:
-            raise NamespaceError("`triplestore` argument needed for updating the cache")
+            raise NamespaceError(
+                "`triplestore` argument needed for updating the cache"
+            )
         if self._cache is None:
             self._cache = {}
 
         # Add (label, full_iri) pairs to cache
         for label in reversed(self._label_annotations):
             self._cache.update(
                 (o, s)
```

### Comparing `tripper-0.2.5/tripper/triplestore.py` & `tripper-0.2.6/tripper/triplestore.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 See
 https://raw.githubusercontent.com/EMMC-ASBL/tripper/master/README.md
 for an introduction.
 
 This module has no dependencies outside the standard library, but the
 triplestore backends may have.
 
-For developers: The usage of `s`, `p`, and `o` represent the different parts of an
-RDF Triple: subject, predicate, and object.
+For developers: The usage of `s`, `p`, and `o` represent the different parts of
+an RDF Triple: subject, predicate, and object.
 """
 # pylint: disable=invalid-name,too-many-public-methods,too-many-lines
 from __future__ import annotations  # Support Python 3.7 (PEP 585)
 
 import importlib
 import inspect
 import re
 import sys
-import uuid
 import warnings
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 from tripper.errors import NamespaceError, TriplestoreError, UniquenessError
 from tripper.literal import Literal
 from tripper.namespace import (
@@ -34,26 +33,28 @@
     OWL,
     RDF,
     RDFS,
     XML,
     XSD,
     Namespace,
 )
-from tripper.utils import (
-    en,
-    function_id,
-    infer_iri,
-    parse_literal,
-    random_string,
-    split_iri,
-)
+from tripper.utils import en, function_id, infer_iri, split_iri
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Mapping
-    from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
+    from typing import (
+        Any,
+        Callable,
+        Dict,
+        Generator,
+        List,
+        Optional,
+        Tuple,
+        Union,
+    )
 
     from tripper.mappings import Value
     from tripper.utils import OptionalTriple, Triple
 
 try:
     from importlib.metadata import entry_points
 except ImportError:
@@ -71,15 +72,15 @@
 hasAccessFunction = EMMO.hasAccessFunction
 hasDataValue = RDF.value  # ??
 hasUnit = DM.hasUnit
 hasCost = DM.hasCost
 
 
 # Regular expression matching a prefixed IRI
-_MATCH_PREFIXED_IRI = re.compile(r"^([a-z]+):([^/]{2}.*)$")
+_MATCH_PREFIXED_IRI = re.compile(r"^([a-z]+):([^/]{1}.*)$")
 
 
 class Triplestore:
     """Provides a common frontend to a range of triplestore backends."""
 
     default_namespaces = {
         "xml": XML,
@@ -125,69 +126,70 @@
                 supports it).
             package: Required when `backend` is a relative module.  In that
                 case, it is relative to `package`.
             kwargs: Keyword arguments passed to the backend's __init__()
                 method.
 
         """
+        backend_name = backend.rsplit(".", 1)[-1]
         module = self._load_backend(backend, package)
-        cls = getattr(module, f"{backend.title()}Strategy")
+        cls = getattr(module, f"{backend_name.title()}Strategy")
         self.base_iri = base_iri
         self.namespaces: "Dict[str, Namespace]" = {}
         self.closed = False
-        self.backend_name = backend
+        self.backend_name = backend_name
         self.backend = cls(base_iri=base_iri, database=database, **kwargs)
 
         # Keep functions in the triplestore for convienence even though
         # they usually do not belong to the triplestore per se.
         self.function_repo: "Dict[str, Union[float, Callable, None]]" = {}
         for prefix, namespace in self.default_namespaces.items():
             self.bind(prefix, namespace)
 
     @classmethod
     def _load_backend(cls, backend: str, package: "Optional[str]" = None):
         """Load and return backend module.  The arguments has the same meaning
         as corresponding arguments to __init__().
 
-        If `backend` contains a dot or `package` is given, import `backend` using
-        `package` for relative imports.
+        If `backend` contains a dot or `package` is given, import `backend`
+        using `package` for relative imports.
 
         Otherwise, if there in the "tripper.backends" entry point group exists
-        an entry point who's name matches `backend`, then the corresponding module
-        is loaded.
+        an entry point who's name matches `backend`, then the corresponding
+        module is loaded.
 
         Otherwise, look for the `backend` in any of the (sub)packages listed
         `backend_packages` module variable.
         """
         # Explicitly specified backend
         if "." in backend or package:
             return importlib.import_module(backend, package)
 
         # Installed backend package
-        if (3, 8) <= sys.version_info < (3, 10):
-            # Fallback for Python 3.8 and 3.9
+        if sys.version_info < (3, 10):
+            # Fallback for Python < 3.10
             eps = entry_points().get("tripper.backends", ())
         else:
-            # New entry_point interface from Python 3.10+, which is also
-            # implemented in the importlib_metadata backport for Python 3.6
-            # and 3.7.
-            eps = entry_points(group="tripper.backends")
+            # New entry_point interface from Python 3.10+
+            eps = entry_points(  # pylint: disable=unexpected-keyword-arg
+                group="tripper.backends"
+            )
         for entry_point in eps:
             if entry_point.name == backend:
                 return importlib.import_module(entry_point.module)
 
         # Backend module
         for pack in backend_packages:
             try:
                 return importlib.import_module(f"{pack}.{backend}")
             except ModuleNotFoundError:
                 pass
 
         raise ModuleNotFoundError(
-            "No tripper backend named '{backend}'",
+            f"No tripper backend named '{backend}'",
             name=backend,
         )
 
     # Methods implemented by backend
     # ------------------------------
     def triples(  # pylint: disable=redefined-builtin
         self,
@@ -274,15 +276,18 @@
         # It should be ok to call close() regardless of whether the backend
         # implements this method or not.  Hence, don't call _check_method().
         if not self.closed and hasattr(self.backend, "close"):
             self.backend.close()
         self.closed = True
 
     def parse(
-        self, source=None, format=None, **kwargs  # pylint: disable=redefined-builtin
+        self,
+        source=None,
+        format=None,
+        **kwargs,  # pylint: disable=redefined-builtin
     ) -> None:
         """Parse source and add the resulting triples to triplestore.
 
         Parameters:
             source: File-like object or file name.
             format: Needed if format can not be inferred from source.
             kwargs: Keyword arguments passed to the backend.
@@ -313,15 +318,17 @@
                 the backend.
             kwargs: Passed to the backend serialize() method.
 
         Returns:
             Serialized string if `destination` is None.
         """
         self._check_method("serialize")
-        return self.backend.serialize(destination=destination, format=format, **kwargs)
+        return self.backend.serialize(
+            destination=destination, format=format, **kwargs
+        )
 
     def query(self, query_object, **kwargs) -> "List[Tuple[str, ...]]":
         """SPARQL query.
 
         Parameters:
             query_object: String with the SPARQL query.
             kwargs: Keyword arguments passed to the backend query() method.
@@ -447,15 +454,16 @@
         """Checks that `backend` has a method called `name`.
 
         Raises NotImplementedError if it hasn't.
         """
         backend_class = cls._get_backend(backend)
         if not hasattr(backend_class, name):
             raise NotImplementedError(
-                f'Triplestore backend {backend!r} do not implement a "{name}()" method.'
+                f"Triplestore backend {backend!r} do not implement a "
+                f'"{name}()" method.'
             )
 
     def _check_method(self, name):
         """Check that backend implements the given method."""
         self._check_backend_method(self.backend_name, name)
 
     def add(self, triple: "Triple"):
@@ -487,15 +495,16 @@
         Returns:
             The value of the `subject`, `predicate` or `object` that is
             None.
         """
         spo = (subject, predicate, object)
         if sum(iri is None for iri in spo) != 1:
             raise ValueError(
-                "Exactly one of `subject`, `predicate` or `object` must be None."
+                "Exactly one of `subject`, `predicate` or `object` must be "
+                "None."
             )
 
         # Index of subject-predicate-object argument that is None
         (idx,) = [i for i, v in enumerate(spo) if v is None]
 
         triples = self.triples(subject, predicate, object)
         if lang:
@@ -542,15 +551,17 @@
             yield p
 
     def objects(self, subject=None, predicate=None):
         """Returns a generator of objects for given subject and predicate."""
         for _, _, o in self.triples(subject=subject, predicate=predicate):
             yield o
 
-    def subject_predicates(self, object=None):  # pylint: disable=redefined-builtin
+    def subject_predicates(
+        self, object=None
+    ):  # pylint: disable=redefined-builtin
         """Returns a generator of (subject, predicate) tuples for given
         object."""
         for s, p, _ in self.triples(object=object):
             yield s, p
 
     def subject_objects(self, predicate=None):
         """Returns a generator of (subject, object) tuples for given
@@ -575,15 +586,17 @@
         self.add(triple)
 
     def has(
         self, subject=None, predicate=None, object=None
     ):  # pylint: disable=redefined-builtin
         """Returns true if the triplestore has any triple matching
         the give subject, predicate and/or object."""
-        triple = self.triples(subject=subject, predicate=predicate, object=object)
+        triple = self.triples(
+            subject=subject, predicate=predicate, object=object
+        )
         try:
             next(triple)
         except StopIteration:
             return False
         return True
 
     # Methods providing additional functionality
@@ -767,23 +780,26 @@
             doc_string = inspect.getdoc(func)
             parlist = f"_:{func.__name__}{fid}_parlist"
             outlist = f"_:{func.__name__}{fid}_outlist"
             if isinstance(expects, Sequence):
                 pars = list(zip(expects, inspect.signature(func).parameters))
             else:
                 pars = [
-                    (expects[par], par) for par in inspect.signature(func).parameters
+                    (expects[par], par)
+                    for par in inspect.signature(func).parameters
                 ]
         elif isinstance(func, str):
             func_iri = func
             name = split_iri(func)[1]
             doc_string = ""
             parlist = f"_:{func_iri}_parlist"
             outlist = f"_:{func_iri}_outlist"
-            pariris = expects if isinstance(expects, Sequence) else expects.values()
+            pariris = (
+                expects if isinstance(expects, Sequence) else expects.values()
+            )
             parnames = [split_iri(pariri)[1] for pariri in pariris]
             pars = list(zip(pariris, parnames))
         else:
             raise TypeError("`func` should be either a callable or an IRI")
 
         self.add((func_iri, RDF.type, FNO.Function))
         self.add((func_iri, RDFS.label, en(name)))
@@ -842,15 +858,17 @@
                 pars = list(zip(inspect.signature(func).parameters, expects))
             else:
                 pars = expects.items()
         elif isinstance(func, str):
             func_iri = func
             name = split_iri(func)[1]
             doc_string = ""
-            pariris = expects if isinstance(expects, Sequence) else expects.values()
+            pariris = (
+                expects if isinstance(expects, Sequence) else expects.values()
+            )
             parnames = [split_iri(pariri)[1] for pariri in pariris]
             pars = list(zip(parnames, pariris))
         else:
             raise TypeError("`func` should be either a callable or an IRI")
 
         self.add((func_iri, RDF.type, Task))
         self.add((func_iri, RDFS.label, en(name)))
@@ -861,282 +879,7 @@
         for iri in returns:
             self.add((iri, RDF.type, DataSet))
             self.add((func_iri, hasOutput, iri))
         if doc_string:
             self.add((func_iri, DCTERMS.description, en(doc_string)))
 
         return func_iri
-
-    def add_interpolation_source(  # pylint: disable=too-many-arguments
-        self,
-        xcoord: str,
-        ycoord: str,
-        input_iri: str,
-        output_iri: str,
-        base_iri: "Optional[str]" = None,
-        standard: str = "emmo",
-        cost: "Optional[Union[float, Callable]]" = None,
-        left: "Optional[float]" = None,
-        right: "Optional[float]" = None,
-        period: "Optional[float]" = None,
-    ) -> str:
-        """Add data source to triplestore, such that it can be used to
-        transparently transform other data.
-
-        No data will be fetch before it is actually needed.
-
-        Parameters:
-            xcoord: IRI of data source with x-coordinates `xp`.  Must be
-                increasing if argument `period` is not specified. Otherwise,
-                `xp` is internally sorted after normalising the periodic
-                boundaries with ``xp = xp % period``.
-            ycoord: IRI of data source with y-coordinates `yp`.  Must have
-                the same length as `xp`.
-            input_iri: IRI of ontological concept that interpolation input-
-                data should be mapped to.
-            output_iri: IRI of ontological concept that interpolation output-
-                data should be mapped to.
-            base_iri: Base of the IRI representing the transformation in the
-                knowledge base.  Defaults to the base IRI of the triplestore.
-            standard: Name of ontology to use when describing the
-                transformation.  Valid values are:
-                - "emmo": Elementary Multiperspective Material Ontology (EMMO)
-                - "fno": Function Ontology (FnO)
-            cost: User-defined cost of following this mapping relation
-                represented as a float.  It may be given either as a
-                float or as a callable taking the same arguments as `func`
-                returning the cost as a float.
-            left: Value to return for `x < xp[0]`, default is `fp[0]`.
-            right: Value to return for `x > xp[-1]`, default is `fp[-1]`.
-            period: A period for the x-coordinates. This parameter allows the
-                proper interpolation of angular x-coordinates. Parameters
-                `left` and `right` are ignored if `period` is specified.
-
-        Returns:
-            transformation_iri: IRI of the added transformation.
-
-        Example:
-            Assume we have a data source that relates water temperature
-            (mapped to EX.Temp) to the amount of blue-green algae (mapped to
-            EX.AlgaeConc). By registering it with
-
-            >>> from tripper import Triplestore
-            >>> from tripper.mappings import Value
-
-            >>> ts = Triplestore(backend="rdflib")
-            >>> EX = ts.bind("ex", "http://example.com#")
-
-            # Add data source with temperatures
-            >>> temp = ts.add_data(
-            ...     lambda ret, conf, ts: Value([0., 20., 30., 37., 40.], unit="degC")
-            ... )
-
-            # Add data source with algae conc.
-            >>> conc = ts.add_data(
-            ...     lambda ret, conf, ts: Value([1e4, 1e6, 1e7, 1e8, 1e3], unit="")
-            ... )
-
-            >>> ts.add_interpolation_source(temp, conc, EX.Temp, EX.AlgaeConc)
-            ':func_3c61cfff'
-
-            we can now ask for the blue-green algae concentration in a fjord,
-            given we have a data source with the water temperature field in
-            the same fjord.
-            >>> ts.add_data(
-            ...     lambda ret, conf, ts: Value([10., 5., 0., 20.], unit="degC"),
-            ...     iri=EX.Temp,
-            ... )  # doctest: +ELLIPSIS
-            '_data_source_...'
-            >>> ts.map(EX.indv, EX.AlgaeConc)
-            >>> ts.get_value(EX.indv)  # should return the algae conc. field
-            array([ 505000.,  257500.,   10000., 1000000.])
-        """
-        try:
-            import numpy as np  # pylint: disable=import-outside-toplevel
-        except ImportError as exc:
-            raise RuntimeError(
-                "Triplestore.add_interpolation_source() requires numpy.\n"
-                "Install it with\n\n"
-                "    pip install numpy"
-            ) from exc
-
-        def func(x):
-            xp = self.get_value(xcoord)
-            fp = self.get_value(ycoord)
-            return np.interp(
-                x,
-                xp=xp,
-                fp=fp,
-                left=left,
-                right=right,
-                period=period,
-            )
-
-        return self.add_function(
-            func,
-            expects=input_iri,
-            returns=output_iri,
-            base_iri=base_iri,
-            standard=standard,
-            cost=cost,
-        )
-
-    def add_data(
-        self,
-        func: "Union[Callable, Literal]",
-        iri: "Optional[Union[str, Sequence]]" = None,
-        configurations: "Optional[dict]" = None,
-        base_iri: "Optional[str]" = None,
-        standard: str = "emmo",
-        cost: "Optional[Union[float, Callable]]" = None,
-    ) -> str:
-        """Register a data source to the triplestore.
-
-        Parameters:
-            func: A callable that should return the value of the registered
-                data source.  It is called with following protopype:
-
-                    func(returns, configurations, triplestore)
-
-                The returned value may in principle be of any type, but for
-                values with unit, it is recommended to return a
-                tripper.mappings.Value object.
-                Alternatively, `func` may also be a literal value.
-            iri: IRI of ontological concept or individual that the data
-                returned by `func` should be mapped to.  If `func` is a
-                callable and multiple values are returned, it may also be
-                given as a sequenceof IRIs.
-                If not given, it will default to a new blank node.
-            configurations: Configurations passed on to `func`.
-            base_iri: Base of the IRI representing the function in the
-                knowledge base.  Defaults to the base IRI of the triplestore.
-            standard: Name of ontological standard to use when describing the
-                function.  Valid values are:
-                - "emmo": Elementary Multiperspective Material Ontology (EMMO)
-                - "fno": Function Ontology (FnO)
-            cost: User-defined cost of following this mapping relation
-                represented as a float.  It may be given either as a
-                float or as a callable taking the same arguments as `func`
-                returning the cost as a float.
-
-        Returns:
-            IRI of data source.
-        """
-        if iri is None:
-            # pylint complains about uuid being unused if we make this an
-            # f-string
-            iri = "_bnode_" + str(uuid.uuid4())
-        data_source = "_data_source_" + random_string(8)
-        self.add((data_source, RDF.type, DataSource))
-
-        if isinstance(func, Literal):
-            self.add((data_source, hasDataValue, func))
-            if cost is not None:
-                self._add_cost(cost, data_source)
-            if isinstance(iri, str):
-                self.map(data_source, iri)
-            else:
-                raise TypeError("literal data can only have a single `iri`")
-
-        elif callable(func):
-
-            def fn():
-                return func(iri, configurations, self)
-
-            # Include data source IRI in documentation to ensure that the
-            # function_id of `fn()` will differ for different data sources...
-            fn.__doc__ = f"Function for data source: {data_source}.\n\n{func.__doc__}"
-            fn.__name__ = func.__name__
-
-            func_iri = self.add_function(
-                fn,
-                expects=(),
-                returns=iri,
-                base_iri=base_iri,
-                standard=standard,
-                cost=cost,
-            )
-            self.add((data_source, hasAccessFunction, func_iri))
-        else:
-            raise TypeError(f"`func` must be a callable or literal, got {type(func)}")
-
-        return data_source
-
-    def get_value(
-        self,
-        iri,
-        routeno=0,
-        unit: "Optional[str]" = None,
-        magnitude: bool = False,
-        quantity: "Optional[Any]" = None,
-        **kwargs,
-    ) -> "Value":
-        """Return the value of an individual.
-
-        Parameters:
-            iri: IRI of individual who's value we want to return.  IRI may
-                either refer to a data source or an individual mapped to
-                an ontological concept.
-            routeno: Number identifying the mapping route to apply for
-                retrieving the individual value in case IRI does not refer
-                to a data source.
-            unit: return the result in the given unit.
-                Implies `magnitude=True`.
-            magnitude: Whether to only return the magnitude of the evaluated
-                value (with no unit).
-            quantity: Quantity class to use for evaluation.  Defaults to pint.
-            kwargs: Additional arguments passed on to `mapping_routes()`.
-
-        Returns:
-            The value of the individual.
-        """
-        from tripper.mappings import (  # pylint: disable=import-outside-toplevel
-            Value,
-            mapping_routes,
-        )
-
-        if self.has(iri, RDF.type, DataSource):
-            # `iri` refer to a DataSource
-            if self.has(iri, hasDataValue):  # literal value
-                return Value(
-                    value=parse_literal(self.value(iri, hasDataValue)).to_python(),
-                    unit=parse_literal(self.value(iri, hasUnit)).to_python()
-                    if self.has(iri, hasUnit)
-                    else None,
-                    iri=self.value(iri, MAP.mapsTo),
-                    cost=parse_literal(self.value(iri, hasCost)).to_python()
-                    if self.has(iri, hasCost)
-                    else 0.0,
-                ).get_value(unit=unit, magnitude=magnitude, quantity=quantity)
-
-            if self.has(iri, hasAccessFunction):  # callable
-                func_iri = self.value(iri, hasAccessFunction)
-                func = self.function_repo[func_iri]
-                assert callable(func)  # nosec
-                retval = func()
-                if isinstance(retval, Value):
-                    return retval.get_value(
-                        unit=unit, magnitude=magnitude, quantity=quantity
-                    )
-                return retval
-
-            raise TriplestoreError(
-                f"data source {iri} has neither a 'hasDataValue' or a "
-                f"'hasAccessFunction' property"
-            )
-
-        # `iri` correspond to an individual mapped to an ontological concept.
-        # In this case we check if there exists a mapping route.
-        routes = mapping_routes(
-            target=iri,
-            sources=list(self.subjects(RDF.type, DataSource)),
-            triplestore=self,
-            **kwargs,
-        )
-        if isinstance(routes, Value):
-            return routes.get_value(unit=unit, magnitude=magnitude, quantity=quantity)
-        return routes.eval(
-            routeno=routeno,
-            unit=unit,
-            magnitude=magnitude,
-            quantity=quantity,
-        )
```

### Comparing `tripper-0.2.5/tripper/utils.py` & `tripper-0.2.6/tripper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             iri = obj.identity
         else:
             # pydantic instance
             schema = obj.schema()
             properties = schema["properties"]
             if "uri" in properties and isinstance(properties["uri"], str):
                 iri = properties["uri"]
-            if "identity" in properties and isinstance(properties["identity"], str):
+            if "identity" in properties and isinstance(
+                properties["identity"], str
+            ):
                 iri = properties["identity"]
             if "uuid" in properties and properties["uuid"]:
                 iri = str(properties["uuid"])
     else:
         raise TypeError(f"cannot infer IRI from object: {obj!r}")
     return str(iri)
 
@@ -125,29 +127,37 @@
         return literal
 
     if not isinstance(literal, str):
         if isinstance(literal, tuple(Literal.datatypes)):
             return Literal(
                 literal,
                 lang=lang,
-                datatype=Literal.datatypes.get(type(literal))[0],  # type: ignore
+                datatype=Literal.datatypes.get(type(literal))[
+                    0
+                ],  # type: ignore
             )
         raise TypeError(f"unsupported literal type: {type(literal)}")
 
+    if hasattr(literal, "n3") and callable(literal.n3):
+        return parse_literal(literal.n3())
+
     match = re.match(r'^\s*("""(.*)"""|"(.*)")\s*$', literal, flags=re.DOTALL)
     if match:
         _, v1, v2 = match.groups()
         value, datatype = v1 if v1 else v2, XSD.string
     else:
         match = re.match(
-            r'^\s*("""(.*)"""|"(.*)")\^\^(.*)\s*$', literal, flags=re.DOTALL
+            r'^\s*("""(.*)"""|"(.*)")\^\^(<([^>]+)>|([^<].*))\s*$',
+            literal,
+            flags=re.DOTALL,
         )
         if match:
-            _, v1, v2, datatype = match.groups()
+            _, v1, v2, _, d1, d2 = match.groups()
             value = v1 if v1 else v2
+            datatype = d1 if d1 else d2
         else:
             match = re.match(
                 r'^\s*("""(.*)"""|"(.*)")@(.*)\s*$', literal, flags=re.DOTALL
             )
             if match:
                 _, v1, v2, lang = match.groups()
                 value = v1 if v1 else v2
@@ -155,25 +165,27 @@
                 value = literal
 
     if lang or datatype:
         if datatype:
             types = {}
             for pytype, datatypes in Literal.datatypes.items():
                 types.update({t: pytype for t in datatypes})
-            type_ = types[datatype]
+            type_ = types.get(datatype, str)
             try:
                 value = type_(value)
             except TypeError:
                 pass
         return Literal(value, lang=lang, datatype=datatype)
 
     for type_, datatypes in Literal.datatypes.items():
         if type_ is not bool:
             try:
-                return Literal(type_(literal), lang=lang, datatype=datatypes[0])
+                return Literal(
+                    type_(literal), lang=lang, datatype=datatypes[0]
+                )
             except (ValueError, TypeError):
                 pass
 
     raise ValueError(f'cannot parse literal "{literal}"')
 
 
 def parse_object(obj: "Union[str, Literal]") -> "Union[str, Literal]":
@@ -202,15 +214,17 @@
             return obj
         if obj in ("true", "false"):  # boolean
             return Literal(obj, datatype=XSD.boolean)
         if re.match(r"^\s*[+-]?\d+\s*$", obj):  # integer
             return Literal(obj, datatype=XSD.integer)
         if check(float, obj, ValueError):  #  float
             return Literal(obj, datatype=XSD.double)
-        if check(datetime.datetime.fromisoformat, obj, ValueError):  #  datetime
+        if check(
+            datetime.datetime.fromisoformat, obj, ValueError
+        ):  #  datetime
             return Literal(obj, datatype=XSD.dateTime)
         return parse_literal(obj)
     raise ValueError("`obj` should be a literal or a string.")
 
 
 def as_python(value: "Any") -> "Any":
     """Converts `value` to a native Python representation.
@@ -224,15 +238,15 @@
         return value.to_python()
     if isinstance(value, str):
         return parse_literal(value).to_python()
     return value
 
 
 def check(func: "Callable", s: str, exceptions) -> bool:
-    """Help function that returns true if `func(s)` does not raise an exception.
+    """Help function returning true if `func(s)` does not raise an exception.
 
     False is returned if `func(s)` raises an exception listed in `exceptions`.
     Otherwise the exception is propagated.
     """
     # Note that the missing type hint on `exceptions` is deliberate, see
     # https://peps.python.org/pep-0484/#exceptions
     try:
```

### Comparing `tripper-0.2.5/PKG-INFO` & `tripper-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: tripper
-Version: 0.2.5
+Version: 0.2.6
 Summary: A triplestore wrapper for Python.
 Keywords: triplestore,ontology,RDF
 Author-email: SINTEF <TEAM4.0@sintef.no>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Plugins
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Dist: typing-extensions ~=4.6; python_version<'3.8'
 Requires-Dist: mike ~=1.1 ; extra == "dev"
 Requires-Dist: mkdocs ~=1.4 ; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "dev"
 Requires-Dist: mkdocs-material ~=9.1 ; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy] ~=0.21.2 ; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy] ~=0.22.0 ; extra == "dev"
 Requires-Dist: pre-commit ~=2.21 ; extra == "dev"
 Requires-Dist: pylint ~=2.13 ; extra == "dev"
 Requires-Dist: pytest ~=7.3 ; extra == "dev"
-Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
+Requires-Dist: pytest-cov ~=4.1 ; extra == "dev"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "dev"
 Requires-Dist: rdflib ~=6.3 ; extra == "dev"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "dev"
-Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "dev"
+Requires-Dist: DLite-Python >=0.3.20,<1 ; extra == "dev"
 Requires-Dist: mike ~=1.1 ; extra == "docs"
 Requires-Dist: mkdocs ~=1.4 ; extra == "docs"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "docs"
 Requires-Dist: mkdocs-material ~=9.1 ; extra == "docs"
-Requires-Dist: mkdocstrings[python-legacy] ~=0.21.2 ; extra == "docs"
+Requires-Dist: mkdocstrings[python-legacy] ~=0.22.0 ; extra == "docs"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "docs"
 Requires-Dist: rdflib ~=6.3 ; extra == "docs"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "docs"
-Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "docs"
+Requires-Dist: DLite-Python >=0.3.20,<1 ; extra == "docs"
 Requires-Dist: pre-commit ~=2.21 ; extra == "pre-commit"
 Requires-Dist: pylint ~=2.13 ; extra == "pre-commit"
 Requires-Dist: pytest ~=7.3 ; extra == "testing"
-Requires-Dist: pytest-cov ~=4.0 ; extra == "testing"
+Requires-Dist: pytest-cov ~=4.1 ; extra == "testing"
 Requires-Dist: EMMOntoPy ~=0.5 ; extra == "testing"
 Requires-Dist: rdflib ~=6.3 ; extra == "testing"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "testing"
-Requires-Dist: DLite-Python >=0.3.19,<1 ; extra == "testing"
+Requires-Dist: DLite-Python >=0.3.20,<1 ; extra == "testing"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/tripper/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/tripper
 Project-URL: Home, https://github.com/EMMC-ASBL/tripper
 Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/tripper/issues
 Project-URL: Package, https://pypi.org/project/tripper
 Project-URL: Source, https://github.com/EMMC-ASBL/tripper
 Provides-Extra: dev
@@ -62,14 +63,16 @@
 =======
 _Triplestore wrapper for Python providing a simple and consistent interface to a range of triplestore backends - the best ride when handling any triplestore._
 
 
 [![PyPI](https://img.shields.io/pypi/v/tripper?logo=pypi)](https://pypi.org/project/tripper)
 [![Documentation](https://img.shields.io/badge/documentation-informational?logo=github)](https://emmc-asbl.github.io/tripper/latest/)
 [![CI tests](https://github.com/EMMC-ASBL/tripper/workflows/CI%20-%20Tests/badge.svg)](https://github.com/EMMC-ASBL/tripper/actions/workflows/ci_tests.yml?query=branch%3Amain)
+[![DOI](https://zenodo.org/badge/547162834.svg)](https://zenodo.org/badge/latestdoi/547162834)
+
 
 
 Basic concepts
 --------------
 Tripper provides a simple and consistent interface to a range of triplestore backends.
 It strives for simplicity and is modelled after [rdflib] (with a few simplifications).
 
@@ -86,15 +89,14 @@
 
 To make it easy to work with IRIs, provide Tripper a set of pre-defined namespaces, like `XSD.float`.
 New namespaces can be defined with the [`tripper.Namespace`][Namespace] class.
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
-
 Documentation
 -------------
 * Getting started: See the [tutorial](docs/tutorial.md)
 * [Discovery of custom backends](docs/backend_discovery.md)
 * [Reference manual]
```

