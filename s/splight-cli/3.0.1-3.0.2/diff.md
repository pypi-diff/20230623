# Comparing `tmp/splight-cli-3.0.1.tar.gz` & `tmp/splight-cli-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-3.0.1.tar", last modified: Wed Jun 21 18:32:06 2023, max compression
+gzip compressed data, was "splight-cli-3.0.2.tar", last modified: Fri Jun 23 18:26:12 2023, max compression
```

## Comparing `splight-cli-3.0.1.tar` & `splight-cli-3.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 18:32:06.186962 splight-cli-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-21 18:32:05.000000 splight-cli-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.182962 splight-cli-3.0.1/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.182962 splight-cli-3.0.1/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/.splightignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/templates/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/component/tests/test_component_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-21 18:32:05.000000 splight-cli-3.0.1/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:32:06.186962 splight-cli-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-21 18:32:05.000000 splight-cli-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:32:06.186962 splight-cli-3.0.1/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 18:32:06.000000 splight-cli-3.0.1/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.281909 splight-cli-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-23 18:26:12.281909 splight-cli-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-23 18:26:11.000000 splight-cli-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/.splightignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/templates/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/component/tests/test_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.277909 splight-cli-3.0.2/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-23 18:26:11.000000 splight-cli-3.0.2/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:26:12.281909 splight-cli-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-23 18:26:11.000000 splight-cli-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:26:12.281909 splight-cli-3.0.2/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 18:26:12.000000 splight-cli-3.0.2/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-3.0.1/README.md` & `splight-cli-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/cli.py` & `splight-cli-3.0.2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/__init__.py` & `splight-cli-3.0.2/cli/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/component.py` & `splight-cli-3.0.2/cli/component/component.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/exceptions.py` & `splight-cli-3.0.2/cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/loaders.py` & `splight-cli-3.0.2/cli/component/loaders.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/templates/.splightignore` & `splight-cli-3.0.2/cli/component/templates/.splightignore`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/templates/auto_readme.md` & `splight-cli-3.0.2/cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/templates/main.py` & `splight-cli-3.0.2/cli/component/templates/main.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/templates/spec.json` & `splight-cli-3.0.2/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/templates/tests.py` & `splight-cli-3.0.2/cli/component/templates/tests.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/component/tests/test_component_manager.py` & `splight-cli-3.0.2/cli/component/tests/test_component_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/config/__init__.py` & `splight-cli-3.0.2/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/constants.py` & `splight-cli-3.0.2/cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/context/__init__.py` & `splight-cli-3.0.2/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/context/workspace.py` & `splight-cli-3.0.2/cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/__init__.py` & `splight-cli-3.0.2/cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/alert/__init__.py` & `splight-cli-3.0.2/cli/engine/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/asset/__init__.py` & `splight-cli-3.0.2/cli/engine/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/attribute/__init__.py` & `splight-cli-3.0.2/cli/engine/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/component/__init__.py` & `splight-cli-3.0.2/cli/engine/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/datalake/__init__.py` & `splight-cli-3.0.2/cli/engine/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/file/__init__.py` & `splight-cli-3.0.2/cli/engine/file/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/manager/exceptions.py` & `splight-cli-3.0.2/cli/engine/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/manager/manager.py` & `splight-cli-3.0.2/cli/engine/manager/manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/secret/__init__.py` & `splight-cli-3.0.2/cli/engine/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/engine/setpoint/__init__.py` & `splight-cli-3.0.2/cli/engine/setpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/hub/component/__init__.py` & `splight-cli-3.0.2/cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/hub/component/exceptions.py` & `splight-cli-3.0.2/cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/hub/component/hub_manager.py` & `splight-cli-3.0.2/cli/hub/component/hub_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/settings.py` & `splight-cli-3.0.2/cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/utils/input.py` & `splight-cli-3.0.2/cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/utils/loader.py` & `splight-cli-3.0.2/cli/utils/loader.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/utils/pprint.py` & `splight-cli-3.0.2/cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/utils/yaml.py` & `splight-cli-3.0.2/cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/cli/workspace/__init__.py` & `splight-cli-3.0.2/cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/setup.py` & `splight-cli-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.0.1/splight_cli.egg-info/SOURCES.txt` & `splight-cli-3.0.2/splight_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

