# Comparing `tmp/sea-names-0.1.1.tar.gz` & `tmp/sea-names-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sea-names-0.1.1.tar", last modified: Fri Jun 23 16:01:13 2023, max compression
+gzip compressed data, was "sea-names-0.1.2.tar", last modified: Fri Jun 23 16:03:42 2023, max compression
```

## Comparing `sea-names-0.1.1.tar` & `sea-names-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.233948 sea-names-0.1.1/
--rw-r--r--   0 luke      (1000) luke      (1000)      292 2023-06-16 14:34:08.000000 sea-names-0.1.1/.editorconfig
--rw-r--r--   0 luke      (1000) luke      (1000)       31 2023-06-16 14:34:08.000000 sea-names-0.1.1/.flake8
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/.github/
--rw-r--r--   0 luke      (1000) luke      (1000)      320 2023-06-16 14:34:08.000000 sea-names-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 luke      (1000) luke      (1000)     1877 2023-06-16 14:34:08.000000 sea-names-0.1.1/.gitignore
--rw-r--r--   0 luke      (1000) luke      (1000)     1216 2023-06-16 14:34:08.000000 sea-names-0.1.1/.gitlab-ci.yml
--rw-r--r--   0 luke      (1000) luke      (1000)       88 2023-06-23 14:50:52.000000 sea-names-0.1.1/.isort.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)     1619 2023-06-16 14:34:08.000000 sea-names-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)      151 2023-06-16 14:34:08.000000 sea-names-0.1.1/AUTHORS.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1510 2023-06-16 14:34:08.000000 sea-names-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1624 2023-06-23 14:52:58.000000 sea-names-0.1.1/Dockerfile
--rw-r--r--   0 luke      (1000) luke      (1000)      415 2023-06-23 14:52:58.000000 sea-names-0.1.1/Dockerfile.dev
--rw-r--r--   0 luke      (1000) luke      (1000)       89 2023-06-16 14:34:08.000000 sea-names-0.1.1/HISTORY.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1081 2023-06-16 14:34:08.000000 sea-names-0.1.1/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      262 2023-06-16 14:34:08.000000 sea-names-0.1.1/MANIFEST.in
--rw-r--r--   0 luke      (1000) luke      (1000)     2350 2023-06-16 14:34:08.000000 sea-names-0.1.1/Makefile
--rw-r--r--   0 luke      (1000) luke      (1000)     2431 2023-06-23 16:01:13.233948 sea-names-0.1.1/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     1629 2023-06-23 15:59:23.000000 sea-names-0.1.1/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       29 2023-06-16 14:34:08.000000 sea-names-0.1.1/codecov.yml
--rw-r--r--   0 luke      (1000) luke      (1000)      831 2023-06-16 14:34:08.000000 sea-names-0.1.1/conftest.py
--rw-r--r--   0 luke      (1000) luke      (1000)      148 2023-06-16 14:34:08.000000 sea-names-0.1.1/dev-environment.yml
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.225948 sea-names-0.1.1/docker/
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/docker/linter/
--rw-r--r--   0 luke      (1000) luke      (1000)      462 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/linter/Dockerfile
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/docker/main/
--rwxr-xr-x   0 luke      (1000) luke      (1000)      201 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/main/entrypoint.sh
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/docker/scripts/
--rwxr-xr-x   0 luke      (1000) luke      (1000)      825 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/scripts/install-conda.sh
--rwxr-xr-x   0 luke      (1000) luke      (1000)      121 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/scripts/install-dependencies.sh
--rwxr-xr-x   0 luke      (1000) luke      (1000)      115 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/scripts/install-project.sh
--rwxr-xr-x   0 luke      (1000) luke      (1000)       93 2023-06-16 14:34:08.000000 sea-names-0.1.1/docker/scripts/install-test-dependencies.sh
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)      610 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/Makefile
--rw-r--r--   0 luke      (1000) luke      (1000)       28 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/authors.rst
--rwxr-xr-x   0 luke      (1000) luke      (1000)     4807 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)       33 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/contributing.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       28 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/history.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      306 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1110 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/installation.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      807 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/make.bat
--rw-r--r--   0 luke      (1000) luke      (1000)       27 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/readme.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       73 2023-06-16 14:34:08.000000 sea-names-0.1.1/docs/usage.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      104 2023-06-23 14:50:52.000000 sea-names-0.1.1/environment.yml
--rw-r--r--   0 luke      (1000) luke      (1000)      763 2023-06-16 14:34:08.000000 sea-names-0.1.1/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)       70 2023-06-16 14:34:08.000000 sea-names-0.1.1/requirements-dev.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2023-06-16 14:34:08.000000 sea-names-0.1.1/requirements.txt
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.229948 sea-names-0.1.1/sea_names/
--rw-r--r--   0 luke      (1000) luke      (1000)      260 2023-06-23 14:50:52.000000 sea-names-0.1.1/sea_names/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1956 2023-06-23 14:50:52.000000 sea-names-0.1.1/sea_names/cache.py
--rw-r--r--   0 luke      (1000) luke      (1000)      477 2023-06-16 14:34:08.000000 sea-names-0.1.1/sea_names/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3635 2023-06-23 14:53:17.000000 sea-names-0.1.1/sea_names/geo.py
--rw-r--r--   0 luke      (1000) luke      (1000)      352 2023-06-23 14:50:52.000000 sea-names-0.1.1/sea_names/log.py
--rw-r--r--   0 luke      (1000) luke      (1000)      440 2023-06-16 14:34:08.000000 sea-names-0.1.1/sea_names/logging.conf
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.233948 sea-names-0.1.1/sea_names.egg-info/
--rw-r--r--   0 luke      (1000) luke      (1000)     2431 2023-06-23 16:01:13.000000 sea-names-0.1.1/sea_names.egg-info/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     1069 2023-06-23 16:01:13.000000 sea-names-0.1.1/sea_names.egg-info/SOURCES.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-06-23 16:01:13.000000 sea-names-0.1.1/sea_names.egg-info/dependency_links.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       49 2023-06-23 16:01:13.000000 sea-names-0.1.1/sea_names.egg-info/entry_points.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-06-23 15:46:54.000000 sea-names-0.1.1/sea_names.egg-info/not-zip-safe
--rw-r--r--   0 luke      (1000) luke      (1000)       10 2023-06-23 16:01:13.000000 sea-names-0.1.1/sea_names.egg-info/top_level.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      426 2023-06-23 16:01:13.233948 sea-names-0.1.1/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)     1815 2023-06-23 16:00:35.000000 sea-names-0.1.1/setup.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:01:13.233948 sea-names-0.1.1/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)       39 2023-06-16 14:34:08.000000 sea-names-0.1.1/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1388 2023-06-23 14:50:52.000000 sea-names-0.1.1/tests/test_sea_names.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.415673 sea-names-0.1.2/
+-rw-r--r--   0 luke      (1000) luke      (1000)      292 2023-06-16 14:34:08.000000 sea-names-0.1.2/.editorconfig
+-rw-r--r--   0 luke      (1000) luke      (1000)       31 2023-06-16 14:34:08.000000 sea-names-0.1.2/.flake8
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.411673 sea-names-0.1.2/.github/
+-rw-r--r--   0 luke      (1000) luke      (1000)      320 2023-06-16 14:34:08.000000 sea-names-0.1.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 luke      (1000) luke      (1000)     1877 2023-06-16 14:34:08.000000 sea-names-0.1.2/.gitignore
+-rw-r--r--   0 luke      (1000) luke      (1000)     1216 2023-06-16 14:34:08.000000 sea-names-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0 luke      (1000) luke      (1000)       88 2023-06-23 14:50:52.000000 sea-names-0.1.2/.isort.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)     1619 2023-06-16 14:34:08.000000 sea-names-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)      151 2023-06-16 14:34:08.000000 sea-names-0.1.2/AUTHORS.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1510 2023-06-16 14:34:08.000000 sea-names-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1624 2023-06-23 14:52:58.000000 sea-names-0.1.2/Dockerfile
+-rw-r--r--   0 luke      (1000) luke      (1000)      415 2023-06-23 14:52:58.000000 sea-names-0.1.2/Dockerfile.dev
+-rw-r--r--   0 luke      (1000) luke      (1000)       89 2023-06-16 14:34:08.000000 sea-names-0.1.2/HISTORY.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1081 2023-06-16 14:34:08.000000 sea-names-0.1.2/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      262 2023-06-16 14:34:08.000000 sea-names-0.1.2/MANIFEST.in
+-rw-r--r--   0 luke      (1000) luke      (1000)     2350 2023-06-16 14:34:08.000000 sea-names-0.1.2/Makefile
+-rw-r--r--   0 luke      (1000) luke      (1000)     2413 2023-06-23 16:03:42.415673 sea-names-0.1.2/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     1629 2023-06-23 15:59:23.000000 sea-names-0.1.2/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       29 2023-06-16 14:34:08.000000 sea-names-0.1.2/codecov.yml
+-rw-r--r--   0 luke      (1000) luke      (1000)      831 2023-06-16 14:34:08.000000 sea-names-0.1.2/conftest.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      148 2023-06-16 14:34:08.000000 sea-names-0.1.2/dev-environment.yml
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.407673 sea-names-0.1.2/docker/
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.411673 sea-names-0.1.2/docker/linter/
+-rw-r--r--   0 luke      (1000) luke      (1000)      462 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/linter/Dockerfile
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.411673 sea-names-0.1.2/docker/main/
+-rwxr-xr-x   0 luke      (1000) luke      (1000)      201 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/main/entrypoint.sh
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.411673 sea-names-0.1.2/docker/scripts/
+-rwxr-xr-x   0 luke      (1000) luke      (1000)      825 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/scripts/install-conda.sh
+-rwxr-xr-x   0 luke      (1000) luke      (1000)      121 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/scripts/install-dependencies.sh
+-rwxr-xr-x   0 luke      (1000) luke      (1000)      115 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/scripts/install-project.sh
+-rwxr-xr-x   0 luke      (1000) luke      (1000)       93 2023-06-16 14:34:08.000000 sea-names-0.1.2/docker/scripts/install-test-dependencies.sh
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.411673 sea-names-0.1.2/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)      610 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/Makefile
+-rw-r--r--   0 luke      (1000) luke      (1000)       28 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 luke      (1000) luke      (1000)     4807 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       33 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/contributing.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       28 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/history.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      306 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1110 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/installation.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      807 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/make.bat
+-rw-r--r--   0 luke      (1000) luke      (1000)       27 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/readme.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       73 2023-06-16 14:34:08.000000 sea-names-0.1.2/docs/usage.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      104 2023-06-23 14:50:52.000000 sea-names-0.1.2/environment.yml
+-rw-r--r--   0 luke      (1000) luke      (1000)      763 2023-06-16 14:34:08.000000 sea-names-0.1.2/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)       70 2023-06-16 14:34:08.000000 sea-names-0.1.2/requirements-dev.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2023-06-16 14:34:08.000000 sea-names-0.1.2/requirements.txt
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.415673 sea-names-0.1.2/sea_names/
+-rw-r--r--   0 luke      (1000) luke      (1000)      260 2023-06-23 14:50:52.000000 sea-names-0.1.2/sea_names/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1956 2023-06-23 14:50:52.000000 sea-names-0.1.2/sea_names/cache.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      477 2023-06-16 14:34:08.000000 sea-names-0.1.2/sea_names/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3635 2023-06-23 14:53:17.000000 sea-names-0.1.2/sea_names/geo.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      352 2023-06-23 14:50:52.000000 sea-names-0.1.2/sea_names/log.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      440 2023-06-16 14:34:08.000000 sea-names-0.1.2/sea_names/logging.conf
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.415673 sea-names-0.1.2/sea_names.egg-info/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2413 2023-06-23 16:03:42.000000 sea-names-0.1.2/sea_names.egg-info/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     1069 2023-06-23 16:03:42.000000 sea-names-0.1.2/sea_names.egg-info/SOURCES.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-06-23 16:03:42.000000 sea-names-0.1.2/sea_names.egg-info/dependency_links.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       49 2023-06-23 16:03:42.000000 sea-names-0.1.2/sea_names.egg-info/entry_points.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-06-23 15:46:54.000000 sea-names-0.1.2/sea_names.egg-info/not-zip-safe
+-rw-r--r--   0 luke      (1000) luke      (1000)       10 2023-06-23 16:03:42.000000 sea-names-0.1.2/sea_names.egg-info/top_level.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      426 2023-06-23 16:03:42.415673 sea-names-0.1.2/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)     1797 2023-06-23 16:02:36.000000 sea-names-0.1.2/setup.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-06-23 16:03:42.415673 sea-names-0.1.2/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)       39 2023-06-16 14:34:08.000000 sea-names-0.1.2/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1388 2023-06-23 14:50:52.000000 sea-names-0.1.2/tests/test_sea_names.py
```

### Comparing `sea-names-0.1.1/.gitignore` & `sea-names-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/.gitlab-ci.yml` & `sea-names-0.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/.pre-commit-config.yaml` & `sea-names-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/CONTRIBUTING.rst` & `sea-names-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/Dockerfile` & `sea-names-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/LICENSE` & `sea-names-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/Makefile` & `sea-names-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/PKG-INFO` & `sea-names-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sea-names
-Version: 0.1.1
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Version: 0.1.2
+Summary: Determine the sea-name of any arbitrary point or shapely geometry.
 Home-page: http://git.axiom/axiom/sea-names
 Author: Luke Campbell
 Author-email: luke@axds.co
 License: MIT license
 Keywords: sea-names
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sea-names-0.1.1/README.rst` & `sea-names-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/conftest.py` & `sea-names-0.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/docker/scripts/install-conda.sh` & `sea-names-0.1.2/docker/scripts/install-conda.sh`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/docs/Makefile` & `sea-names-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/docs/conf.py` & `sea-names-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/docs/installation.rst` & `sea-names-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/docs/make.bat` & `sea-names-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/pyproject.toml` & `sea-names-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/sea_names/cache.py` & `sea-names-0.1.2/sea_names/cache.py`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/sea_names/geo.py` & `sea-names-0.1.2/sea_names/geo.py`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/sea_names.egg-info/PKG-INFO` & `sea-names-0.1.2/sea_names.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sea-names
-Version: 0.1.1
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Version: 0.1.2
+Summary: Determine the sea-name of any arbitrary point or shapely geometry.
 Home-page: http://git.axiom/axiom/sea-names
 Author: Luke Campbell
 Author-email: luke@axds.co
 License: MIT license
 Keywords: sea-names
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sea-names-0.1.1/sea_names.egg-info/SOURCES.txt` & `sea-names-0.1.2/sea_names.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sea-names-0.1.1/setup.py` & `sea-names-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    description="Determine the sea-name of any arbitrary point or shapely geometry.",
     entry_points={
         'console_scripts': [
             'sea-names=sea_names.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
@@ -50,10 +50,10 @@
     include_package_data=True,
     keywords='sea-names',
     name='sea-names',
     packages=find_packages(include=['sea_names', 'sea_names.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='http://git.axiom/axiom/sea-names',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `sea-names-0.1.1/tests/test_sea_names.py` & `sea-names-0.1.2/tests/test_sea_names.py`

 * *Files identical despite different names*

