# Comparing `tmp/up_esb-0.0.131.tar.gz` & `tmp/up_esb-0.0.134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_esb-0.0.131.tar", last modified: Thu Jun 22 12:46:58 2023, max compression
+gzip compressed data, was "up_esb-0.0.134.tar", last modified: Fri Jun 23 10:03:53 2023, max compression
```

## Comparing `up_esb-0.0.131.tar` & `up_esb-0.0.134.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.423386 up_esb-0.0.131/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.415386 up_esb-0.0.131/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.415386 up_esb-0.0.131/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-22 12:46:39.000000 up_esb-0.0.131/.github/scripts/update_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.415386 up_esb-0.0.131/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-22 12:46:39.000000 up_esb-0.0.131/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 12:46:39.000000 up_esb-0.0.131/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-22 12:46:39.000000 up_esb-0.0.131/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-22 12:46:39.000000 up_esb-0.0.131/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 12:46:39.000000 up_esb-0.0.131/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 12:46:58.423386 up_esb-0.0.131/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 12:46:39.000000 up_esb-0.0.131/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.415386 up_esb-0.0.131/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-22 12:46:39.000000 up_esb-0.0.131/docs/callable_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-06-22 12:46:39.000000 up_esb-0.0.131/docs/create_action_interface.drawio.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-22 12:46:39.000000 up_esb-0.0.131/examples/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-22 12:46:39.000000 up_esb-0.0.131/examples/partialorderplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-22 12:46:39.000000 up_esb-0.0.131/examples/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-22 12:46:39.000000 up_esb-0.0.131/examples/time_triggered.py
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-06-22 12:46:39.000000 up_esb-0.0.131/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:46:58.423386 up_esb-0.0.131/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 12:46:39.000000 up_esb-0.0.131/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/components/test_expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/test_create_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-22 12:46:39.000000 up_esb-0.0.131/tests/test_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/up_esb/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/up_esb/components/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/components/expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/components/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.423386 up_esb-0.0.131/up_esb/plexmo/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/plexmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/plexmo/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-22 12:46:39.000000 up_esb-0.0.131/up_esb/plexmo/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:46:58.419386 up_esb-0.0.131/up_esb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 12:46:58.000000 up_esb-0.0.131/up_esb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 12:46:58.000000 up_esb-0.0.131/up_esb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:46:58.000000 up_esb-0.0.131/up_esb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 12:46:58.000000 up_esb-0.0.131/up_esb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 12:46:58.000000 up_esb-0.0.131/up_esb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.464689 up_esb-0.0.134/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.464689 up_esb-0.0.134/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-23 10:03:30.000000 up_esb-0.0.134/.github/scripts/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.464689 up_esb-0.0.134/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-23 10:03:30.000000 up_esb-0.0.134/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 10:03:30.000000 up_esb-0.0.134/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-23 10:03:30.000000 up_esb-0.0.134/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-23 10:03:30.000000 up_esb-0.0.134/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 10:03:30.000000 up_esb-0.0.134/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-23 10:03:53.468689 up_esb-0.0.134/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 10:03:30.000000 up_esb-0.0.134/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 10:03:30.000000 up_esb-0.0.134/docs/callable_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-06-23 10:03:30.000000 up_esb-0.0.134/docs/create_action_interface.drawio.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-23 10:03:30.000000 up_esb-0.0.134/examples/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-23 10:03:30.000000 up_esb-0.0.134/examples/partialorderplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-23 10:03:30.000000 up_esb-0.0.134/examples/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-23 10:03:30.000000 up_esb-0.0.134/examples/time_triggered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-06-23 10:03:30.000000 up_esb-0.0.134/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:03:53.468689 up_esb-0.0.134/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 10:03:30.000000 up_esb-0.0.134/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/components/test_expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/test_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-23 10:03:30.000000 up_esb-0.0.134/tests/test_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/up_esb/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/up_esb/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/components/expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/components/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/up_esb/plexmo/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/plexmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/plexmo/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-23 10:03:30.000000 up_esb-0.0.134/up_esb/plexmo/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:53.468689 up_esb-0.0.134/up_esb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-23 10:03:53.000000 up_esb-0.0.134/up_esb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 10:03:53.000000 up_esb-0.0.134/up_esb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:03:53.000000 up_esb-0.0.134/up_esb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 10:03:53.000000 up_esb-0.0.134/up_esb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 10:03:53.000000 up_esb-0.0.134/up_esb.egg-info/top_level.txt
```

### Comparing `up_esb-0.0.131/.github/scripts/update_version.py` & `up_esb-0.0.134/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/.github/workflows/deploy.yml` & `up_esb-0.0.134/.github/workflows/deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 name: Deploy
 
 on:
-  workflow_dispatch:
+  pull_request:
+    types: [closed]
 
 jobs:
   update_version:
     runs-on: ubuntu-latest
+    if: github.event.pull_request.merged == true
     steps:
       - name: Checkout Repository
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
+          # Allow the action to push to the repository
+          token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Set Up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
 
       - name: Run Version Update Script
         id: update_version
         run: |
           version=$(python3 .github/scripts/update_version.py)
           if git diff --quiet HEAD^ HEAD; then
             echo "No changes detected, exiting."
-            echo "::set-output name=status::no_changes"
+            echo "status=no_changes" >> $GITHUB_OUTPUT
             exit 0
           fi
-          echo "::set-output name=version::$version"
+          echo "version=$version" >> $GITHUB_OUTPUT
 
       - name: Commit and Push Changes
         if: steps.update_version.outputs.status != 'no_changes'
         run: |
           git checkout ${{ github.event.pull_request.base.ref }}
           git config --local user.email "action@github.com"
           git config --local user.name "GitHub Action"
@@ -54,8 +58,7 @@
         run: pip3 install build twine
       - name: Build Package
         run: python3 -m build
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-
```

### Comparing `up_esb-0.0.131/.github/workflows/main.yml` & `up_esb-0.0.134/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/.gitignore` & `up_esb-0.0.134/.gitignore`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/.pre-commit-config.yaml` & `up_esb-0.0.134/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/LICENSE` & `up_esb-0.0.134/LICENSE`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/PKG-INFO` & `up_esb-0.0.134/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up_esb
-Version: 0.0.131
+Version: 0.0.134
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.131/README.md` & `up_esb-0.0.134/README.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/docs/callable_interface.md` & `up_esb-0.0.134/docs/callable_interface.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/docs/create_action_interface.drawio.png` & `up_esb-0.0.134/docs/create_action_interface.drawio.png`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/examples/parallel.py` & `up_esb-0.0.134/examples/parallel.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/examples/partialorderplan.py` & `up_esb-0.0.134/examples/partialorderplan.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/examples/sequential.py` & `up_esb-0.0.134/examples/sequential.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/examples/time_triggered.py` & `up_esb-0.0.134/examples/time_triggered.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/pyproject.toml` & `up_esb-0.0.134/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 description = "General functionalities for using unified-planning in robotic applications"
 keywords = ["unified-planning", "embedded-systems-bridge"]
 license = {text = "Apache-2.0 License"}
 name = "up_esb"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.131"
+version = "0.0.134"
 
 [project.urls]
 Repository = "https://github.com/aiplan4eu/embedded-systems-bridge"
 Homepage = "https://www.aiplan4eu-project.eu/"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "pytest", "pre-commit"]
```

### Comparing `up_esb-0.0.131/tests/components/test_expression_manager.py` & `up_esb-0.0.134/tests/components/test_expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/tests/test_bridge.py` & `up_esb-0.0.134/tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/tests/test_create_action.py` & `up_esb-0.0.134/tests/test_create_action.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/tests/test_dispatcher.py` & `up_esb-0.0.134/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/tests/test_graph.py` & `up_esb-0.0.134/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/tests/test_monitor.py` & `up_esb-0.0.134/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/__init__.py` & `up_esb-0.0.134/up_esb/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/bridge.py` & `up_esb-0.0.134/up_esb/bridge.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/components/__init__.py` & `up_esb-0.0.134/up_esb/components/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/components/actions.py` & `up_esb-0.0.134/up_esb/components/actions.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/components/expression_manager.py` & `up_esb-0.0.134/up_esb/components/expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/components/graph.py` & `up_esb-0.0.134/up_esb/components/graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/executor.py` & `up_esb-0.0.134/up_esb/executor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/plexmo/__init__.py` & `up_esb-0.0.134/up_esb/plexmo/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/plexmo/dispatcher.py` & `up_esb-0.0.134/up_esb/plexmo/dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb/plexmo/monitor.py` & `up_esb-0.0.134/up_esb/plexmo/monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.131/up_esb.egg-info/PKG-INFO` & `up_esb-0.0.134/up_esb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-esb
-Version: 0.0.131
+Version: 0.0.134
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.131/up_esb.egg-info/SOURCES.txt` & `up_esb-0.0.134/up_esb.egg-info/SOURCES.txt`

 * *Files identical despite different names*
