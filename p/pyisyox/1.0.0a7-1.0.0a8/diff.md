# Comparing `tmp/pyisyox-1.0.0a7.tar.gz` & `tmp/pyisyox-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyisyox-1.0.0a7.tar", last modified: Sun Jun 18 15:31:50 2023, max compression
+gzip compressed data, was "pyisyox-1.0.0a8.tar", last modified: Fri Jun 23 01:26:13 2023, max compression
```

## Comparing `pyisyox-1.0.0a7.tar` & `pyisyox-1.0.0a8.tar`

### file list

```diff
@@ -1,97 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.devcontainer/postCreate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.github/workflows/pythonpublish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.616330 pyisyox-1.0.0a7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/api/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/docs/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/test_cases/node_battery_only.xml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/docs/test_cases/parsed_node_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/clock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30753 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/events/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/eventreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/tcpsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/events/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/entity_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/timeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/helpers/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/isy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/node_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox/nodes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11942 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/folder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21160 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/node_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7857 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/nodes/nodebase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/programs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/programs/program.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/backports.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/util/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/pyisyox/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyisyox/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:31:50.620329 pyisyox-1.0.0a7/pyisyox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-18 15:31:49.000000 pyisyox-1.0.0a7/pyisyox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:31:49.000000 pyisyox-1.0.0a7/pyisyox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 15:31:50.000000 pyisyox-1.0.0a7/pyisyox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-18 15:31:50.624329 pyisyox-1.0.0a7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-06-18 15:31:39.000000 pyisyox-1.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.devcontainer/postCreate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.github/workflows/pythonpublish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/api/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.845494 pyisyox-1.0.0a8/docs/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/test_cases/node_battery_only.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/docs/test_cases/parsed_node_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/clock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4282 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30753 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/eventreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/tcpsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/events/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/entity_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/timeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/helpers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/isy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/node_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/nodes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11942 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/folder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4513 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21160 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/node_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7857 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/nodes/nodebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/programs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/programs/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/backports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/util/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/pyisyox/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyisyox/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:26:13.849494 pyisyox-1.0.0a8/pyisyox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 01:26:13.000000 pyisyox-1.0.0a8/pyisyox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 01:26:03.000000 pyisyox-1.0.0a8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 01:26:13.853494 pyisyox-1.0.0a8/setup.cfg
```

### Comparing `pyisyox-1.0.0a7/.devcontainer/Dockerfile` & `pyisyox-1.0.0a8/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/.devcontainer/devcontainer.json` & `pyisyox-1.0.0a8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/.github/workflows/pythonpublish.yml` & `pyisyox-1.0.0a8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/.gitignore` & `pyisyox-1.0.0a8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/.pre-commit-config.yaml` & `pyisyox-1.0.0a8/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.274
     hooks:
       - id: ruff
         args:
           - --fix
   - hooks:
       - args: [--safe, --quiet]
         files: ^((pyisyox|examples)/.+)?[^/]+\.py$
```

### Comparing `pyisyox-1.0.0a7/.vscode/settings.json` & `pyisyox-1.0.0a8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/.yamllint` & `pyisyox-1.0.0a8/.yamllint`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/CHANGELOG.md` & `pyisyox-1.0.0a8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/LICENSE.txt` & `pyisyox-1.0.0a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/PKG-INFO` & `pyisyox-1.0.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
-Author: shbatm
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
 Keywords: home,automation,isy,isy994,isy-994,UDI,polisy,eisy,home-assistant
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyisyox-1.0.0a7/README.md` & `pyisyox-1.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/Makefile` & `pyisyox-1.0.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/conf.py` & `pyisyox-1.0.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/events.rst` & `pyisyox-1.0.0a8/docs/events.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/index.rst` & `pyisyox-1.0.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/library.rst` & `pyisyox-1.0.0a8/docs/library.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/make.bat` & `pyisyox-1.0.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/quickstart.rst` & `pyisyox-1.0.0a8/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/test_cases/node_battery_only.xml` & `pyisyox-1.0.0a8/docs/test_cases/node_battery_only.xml`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/docs/test_cases/parsed_node_info.json` & `pyisyox-1.0.0a8/docs/test_cases/parsed_node_info.json`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/mypy.ini` & `pyisyox-1.0.0a8/mypy.ini`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/__init__.py` & `pyisyox-1.0.0a8/pyisyox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/__main__.py` & `pyisyox-1.0.0a8/pyisyox/__main__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/clock.py` & `pyisyox-1.0.0a8/pyisyox/clock.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/configuration.py` & `pyisyox-1.0.0a8/pyisyox/configuration.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/connection.py` & `pyisyox-1.0.0a8/pyisyox/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,25 +125,25 @@
         return url
 
     async def request(
         self, url: str, retries: int = 0, ok404: bool = False, delay: float = 0
     ) -> str | None:
         """Execute request to ISY REST interface."""
         _LOGGER.debug("Request: %s", url)
+        endpoint = url.split("rest", 1)[1]
         if delay:
             await asyncio.sleep(delay)
         try:
             async with self.semaphore, self.req_session.get(
                 url,
                 auth=self.connection_info.auth,
                 headers=HTTP_HEADERS,
                 timeout=HTTP_TIMEOUT,
                 ssl=self.sslcontext,
             ) as res:
-                endpoint = url.split("rest", 1)[1]
                 if res.status == HTTP_OK:
                     _LOGGER.debug("Response received: %s", endpoint)
                     results = await res.text(encoding="utf-8", errors="ignore")
                     if results != EMPTY_XML_RESPONSE:
                         return results
                     _LOGGER.debug("Invalid empty XML returned: %s", endpoint)
                     res.release()
```

### Comparing `pyisyox-1.0.0a7/pyisyox/constants.py` & `pyisyox-1.0.0a8/pyisyox/constants.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/events/eventreader.py` & `pyisyox-1.0.0a8/pyisyox/events/eventreader.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/events/router.py` & `pyisyox-1.0.0a8/pyisyox/events/router.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/events/strings.py` & `pyisyox-1.0.0a8/pyisyox/events/strings.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/events/tcpsocket.py` & `pyisyox-1.0.0a8/pyisyox/events/tcpsocket.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/events/websocket.py` & `pyisyox-1.0.0a8/pyisyox/events/websocket.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/exceptions.py` & `pyisyox-1.0.0a8/pyisyox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/__init__.py` & `pyisyox-1.0.0a8/pyisyox/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/entity.py` & `pyisyox-1.0.0a8/pyisyox/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/entity_platform.py` & `pyisyox-1.0.0a8/pyisyox/helpers/entity_platform.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/events.py` & `pyisyox-1.0.0a8/pyisyox/helpers/events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/models.py` & `pyisyox-1.0.0a8/pyisyox/helpers/models.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/session.py` & `pyisyox-1.0.0a8/pyisyox/helpers/session.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/timeit.py` & `pyisyox-1.0.0a8/pyisyox/helpers/timeit.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/helpers/xml.py` & `pyisyox-1.0.0a8/pyisyox/helpers/xml.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/isy.py` & `pyisyox-1.0.0a8/pyisyox/isy.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/logging.py` & `pyisyox-1.0.0a8/pyisyox/logging.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/networking.py` & `pyisyox-1.0.0a8/pyisyox/networking.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/node_servers.py` & `pyisyox-1.0.0a8/pyisyox/node_servers.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def from_dict(cls, props: dict) -> NodeDef:
         """Create a dataclass from a dictionary."""
         return cls(
             **{k: v for k, v in props.items() if k in inspect.signature(cls).parameters}
         )
 
     sts: InitVar[dict[str, list | dict]]
-    cmds: InitVar[dict[str, Any]] | None
+    cmds: InitVar[dict[str, Any]] | None = None
     id: str = ""
     node_type: str = ""
     name: str = ""
     nls: str = ""
     slot: str = ""
     editors: Any = ""
     statuses: dict[str, str] = field(init=False, default_factory=dict)
```

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/__init__.py` & `pyisyox-1.0.0a8/pyisyox/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/folder.py` & `pyisyox-1.0.0a8/pyisyox/nodes/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/group.py` & `pyisyox-1.0.0a8/pyisyox/nodes/group.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/node.py` & `pyisyox-1.0.0a8/pyisyox/nodes/node.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/node_events.py` & `pyisyox-1.0.0a8/pyisyox/nodes/node_events.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/nodes/nodebase.py` & `pyisyox-1.0.0a8/pyisyox/nodes/nodebase.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/programs/__init__.py` & `pyisyox-1.0.0a8/pyisyox/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/programs/folder.py` & `pyisyox-1.0.0a8/pyisyox/programs/folder.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/programs/program.py` & `pyisyox-1.0.0a8/pyisyox/programs/program.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/util/backports.py` & `pyisyox-1.0.0a8/pyisyox/util/backports.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/util/output.py` & `pyisyox-1.0.0a8/pyisyox/util/output.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/variables/__init__.py` & `pyisyox-1.0.0a8/pyisyox/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox/variables/variable.py` & `pyisyox-1.0.0a8/pyisyox/variables/variable.py`

 * *Files identical despite different names*

### Comparing `pyisyox-1.0.0a7/pyisyox.egg-info/PKG-INFO` & `pyisyox-1.0.0a8/pyisyox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: pyisyox
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Python module for asynchronous communication with Universal Devices, Inc.'s ISY & IoX controllers.
 Home-page: https://github.com/shbatm/pyisyox
-Author: shbatm
 Author-email: Ryan Kraus <automicus@gmail.com>, shbatm <support@shbatm.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/shbatm/pyisyox
 Project-URL: Homepage, https://github.com/shbatm/pyisyox
 Keywords: home,automation,isy,isy994,isy-994,UDI,polisy,eisy,home-assistant
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyisyox-1.0.0a7/pyisyox.egg-info/SOURCES.txt` & `pyisyox-1.0.0a8/pyisyox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 LICENSE.txt
 README.md
 mypy.ini
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
-setup.py
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/postCreate.sh
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/pythonpublish.yml
 .vscode/extensions.json
@@ -43,15 +42,14 @@
 pyisyox/logging.py
 pyisyox/networking.py
 pyisyox/node_servers.py
 pyisyox/py.typed
 pyisyox.egg-info/PKG-INFO
 pyisyox.egg-info/SOURCES.txt
 pyisyox.egg-info/dependency_links.txt
-pyisyox.egg-info/not-zip-safe
 pyisyox.egg-info/requires.txt
 pyisyox.egg-info/top_level.txt
 pyisyox/events/__init__.py
 pyisyox/events/eventreader.py
 pyisyox/events/router.py
 pyisyox/events/strings.py
 pyisyox/events/tcpsocket.py
```

### Comparing `pyisyox-1.0.0a7/pyproject.toml` & `pyisyox-1.0.0a8/pyproject.toml`

 * *Files identical despite different names*

