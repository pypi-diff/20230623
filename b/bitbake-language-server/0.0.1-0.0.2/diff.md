# Comparing `tmp/bitbake-language-server-0.0.1.tar.gz` & `tmp/bitbake-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbake-language-server-0.0.1.tar", last modified: Mon Jun 19 10:40:01 2023, max compression
+gzip compressed data, was "bitbake-language-server-0.0.2.tar", last modified: Fri Jun 23 07:38:37 2023, max compression
```

## Comparing `bitbake-language-server-0.0.1.tar` & `bitbake-language-server-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.021376 bitbake-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.021376 bitbake-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.021376 bitbake-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/api/bitbake-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/requirements/web.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.021376 bitbake-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/src/bitbake_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.021376 bitbake-language-server-0.0.1/src/bitbake_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/src/bitbake_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    52852 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/assets/json/bitbake.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/src/bitbake_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.025376 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 10:40:01.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 10:40:00.000000 bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:40:01.029376 bitbake-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 10:39:46.000000 bitbake-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/api/bitbake-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/bitbake_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    51596 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/bitbake.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/tests/server_test.py
```

### Comparing `bitbake-language-server-0.0.1/.github/workflows/main.yml` & `bitbake-language-server-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/.gitignore` & `bitbake-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/.pre-commit-config.yaml` & `bitbake-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,21 @@
           - mdformat-myst
           - mdformat-toc
           - mdformat-deflist
           - mdformat-beautysh
           - mdformat-black
           - mdformat-config
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.7.1
+    rev: v0.8.1
     hooks:
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath@0.9.1
   - repo: https://github.com/perltidy/perltidy
-    rev: "20230309.02"
+    rev: "20230309.03"
     hooks:
       - id: perltidy
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
@@ -88,15 +88,15 @@
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
           - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.310
+    rev: v1.1.313
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
```

### Comparing `bitbake-language-server-0.0.1/LICENSE` & `bitbake-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/PKG-INFO` & `bitbake-language-server-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -25,15 +25,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: web
 License-File: LICENSE
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/bitbake-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/bitbake-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/bitbake-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/bitbake-language-server/actions)
```

### Comparing `bitbake-language-server-0.0.1/README.md` & `bitbake-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/docs/conf.py` & `bitbake-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/docs/resources/configure.md` & `bitbake-language-server-0.0.2/docs/resources/configure.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # Configure
 
-See customization in
-<https://bitbake-language-server.readthedocs.io/en/latest/api/bitbake-language-server.html#bitbake_language_server.server.get_document>.
-
 ## (Neo)[Vim](https://www.vim.org)
 
 ### [coc.nvim](https://github.com/neoclide/coc.nvim)
 
 ```json
 {
   "languageserver": {
```

### Comparing `bitbake-language-server-0.0.1/docs/resources/install.md` & `bitbake-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/flake.nix` & `bitbake-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/pyproject.toml` & `bitbake-language-server-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -60,17 +60,14 @@
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
-
-[tool.setuptools.dynamic.optional-dependencies.web]
-file = "requirements/web.txt"
 # end: scripts/update-pyproject.toml.pl
 
 [tool.setuptools_scm]
 write_to = "src/bitbake_language_server/_version.py"
 
 [tool.setuptools-generate]
 write-to = "src/bitbake_language_server/_metainfo.py"
```

### Comparing `bitbake-language-server-0.0.1/src/bitbake_language_server/__main__.py` & `bitbake-language-server-0.0.2/src/bitbake_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.1/src/bitbake_language_server/assets/json/bitbake.json` & `bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/bitbake.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.06223628691983123%*

 * *Differences: {"'ALLOW_EMPTY'": "'Specifies if an output package should still be produced if it is empty.'",*

 * * "'ALTERNATIVE'": "'Lists commands in a package that need an alternative binary naming scheme.'",*

 * * "'ALTERNATIVE_LINK_NAME'": "'Used by the alternatives system to map duplicated commands to actual "*

 * *                            "locations.'",*

 * * "'ALTERNATIVE_PRIORITY'": "'Used by the alternatives system to create default priorities for "*

 * *                           "duplicated commands.'",*

 * * "'ALTERNATIVE_TARGET'": "' […]*

```diff
@@ -1,136 +1,398 @@
 {
-    "ASSUME_PROVIDED": "Lists recipe names (PN values) BitBake does not attempt to build. Instead, BitBake assumes these recipes have already been built.\nIn OpenEmbedded-Core, ASSUME_PROVIDED mostly specifies native tools that should not be built. An example is git-native, which when specified allows for the Git binary from the host to be used rather than building git-native.",
-    "AZ_SAS": "Azure Storage Shared Access Signature, when using the Azure Storage fetcher This variable can be defined to be used by the fetcher to authenticate and gain access to non-public artifacts:\nFor more information see Microsoft\u2019s Azure Storage documentation at https://docs.microsoft.com/en-us/azure/storage/common/storage-sas-overview",
-    "B": "The directory in which BitBake executes functions during a recipe\u2019s build process.",
-    "BBCLASSEXTEND": "Allows you to extend a recipe so that it builds variants of the software. Some examples of these variants for recipes from the OpenEmbedded-Core metadata are \u201cnatives\u201d such as quilt-native, which is a copy of Quilt built to run on the build system; \u201ccrosses\u201d such as gcc-cross, which is a compiler built to run on the build machine but produces binaries that run on the target MACHINE; \u201cnativesdk\u201d, which targets the SDK machine instead of MACHINE; and \u201cmulitlibs\u201d in the form \u201cmultilib:multilib_name\u201d.\nTo build a different variant of the recipe with a minimal amount of code, it usually is as simple as adding the variable to your recipe. Here are two examples. The \u201cnative\u201d variants are from the OpenEmbedded-Core metadata:\nNote\nInternally, the BBCLASSEXTEND mechanism generates recipe variants by rewriting variable values and applying overrides such as _class-native. For example, to generate a native version of a recipe, a DEPENDS on \u201cfoo\u201d is rewritten to a DEPENDS on \u201cfoo-native\u201d.\nEven when using BBCLASSEXTEND, the recipe is only parsed once. Parsing once adds some limitations. For example, it is not possible to include a different file depending on the variant, since include statements are processed when the recipe is parsed.",
-    "BBDEBUG": "Sets the BitBake debug output level to a specific value as incremented by the -D command line option.\nNote\nYou must set this variable in the external environment in order for it to work.",
-    "BBFILES": "A space-separated list of recipe files BitBake uses to build software.\nWhen specifying recipe files, you can pattern match using Python\u2019s glob syntax. For details on the syntax, see the documentation by following the previous link.",
-    "BBFILES_DYNAMIC": "Activates content depending on presence of identified layers.  You identify the layers by the collections that the layers define.\nUse the BBFILES_DYNAMIC variable to avoid .bbappend files whose corresponding .bb file is in a layer that attempts to modify other layers through .bbappend but does not want to introduce a hard dependency on those other layers.\nAdditionally you can prefix the rule with \u201c!\u201d to add .bbappend and .bb files in case a layer is not present.  Use this avoid hard dependency on those other layers.\nUse the following form for BBFILES_DYNAMIC:\nThe following example identifies two collection names and two filename patterns:\nWhen the collection name is prefixed with \u201c!\u201d it will add the file pattern in case the layer is absent:\nThis next example shows an error message that occurs because invalid entries are found, which cause parsing to fail:",
-    "BBFILE_COLLECTIONS": "Lists the names of configured layers. These names are used to find the other BBFILE_* variables. Typically, each layer appends its name to this variable in its conf/layer.conf file.",
-    "BBFILE_PATTERN": "Variable that expands to match files from BBFILES in a particular layer. This variable is used in the conf/layer.conf file and must be suffixed with the name of the specific layer (e.g. BBFILE_PATTERN_emenlow).",
-    "BBFILE_PRIORITY": "Assigns the priority for recipe files in each layer.\nThis variable is useful in situations where the same recipe appears in more than one layer. Setting this variable allows you to prioritize a layer against other layers that contain the same recipe \u2014 effectively letting you control the precedence for the multiple layers. The precedence established through this variable stands regardless of a recipe\u2019s version (PV variable). For example, a layer that has a recipe with a higher PV value but for which the BBFILE_PRIORITY is set to have a lower precedence still has a lower precedence.\nA larger value for the BBFILE_PRIORITY variable results in a higher precedence. For example, the value 6 has a higher precedence than the value 5. If not specified, the BBFILE_PRIORITY variable is set based on layer dependencies (see the LAYERDEPENDS variable for more information. The default priority, if unspecified for a layer with no dependencies, is the lowest defined priority + 1 (or 1 if no priorities are defined).\nTip\nYou can use the command bitbake-layers show-layers to list all configured layers along with their priorities.",
-    "BBINCLUDED": "Contains a space-separated list of all of all files that BitBake\u2019s parser included during parsing of the current file.",
-    "BBINCLUDELOGS": "If set to a value, enables printing the task log when reporting a failed task.",
-    "BBINCLUDELOGS_LINES": "If BBINCLUDELOGS is set, specifies the maximum number of lines from the task log file to print when reporting a failed task. If you do not set BBINCLUDELOGS_LINES, the entire log is printed.",
-    "BBLAYERS": "Lists the layers to enable during the build. This variable is defined in the bblayers.conf configuration file in the build directory. Here is an example:\nThis example enables four layers, one of which is a custom, user-defined layer named meta-mykernel.",
-    "BBLAYERS_FETCH_DIR": "Sets the base location where layers are stored. This setting is used in conjunction with bitbake-layers layerindex-fetch and tells bitbake-layers where to place the fetched layers.",
-    "BBMASK": "Prevents BitBake from processing recipes and recipe append files.\nYou can use the BBMASK variable to \u201chide\u201d these .bb and .bbappend files. BitBake ignores any recipe or recipe append files that match any of the expressions. It is as if BitBake does not see them at all. Consequently, matching files are not parsed or otherwise used by BitBake.\nThe values you provide are passed to Python\u2019s regular expression compiler. Consequently, the syntax follows Python\u2019s Regular Expression (re) syntax. The expressions are compared against the full paths to the files. For complete syntax information, see Python\u2019s documentation at http://docs.python.org/3/library/re.html.\nThe following example uses a complete regular expression to tell BitBake to ignore all recipe and recipe append files in the meta-ti/recipes-misc/ directory:\nIf you want to mask out multiple directories or recipes, you can specify multiple regular expression fragments. This next example masks out multiple directories and individual recipes:\nNote\nWhen specifying a directory name, use the trailing slash character to ensure you match just that directory name.",
-    "BBMULTICONFIG": "Enables BitBake to perform multiple configuration builds and lists each separate configuration (multiconfig). You can use this variable to cause BitBake to build multiple targets where each target has a separate configuration. Define BBMULTICONFIG in your conf/local.conf configuration file.\nAs an example, the following line specifies three multiconfigs, each having a separate configuration file:\nEach configuration file you use must reside in the build directory within a directory named conf/multiconfig (e.g. build_directory/conf/multiconfig/configA.conf).\nFor information on how to use BBMULTICONFIG in an environment that supports building targets with multiple configurations, see the \u201cExecuting a Multiple Configuration Build\u201d section.",
-    "BBPATH": "Used by BitBake to locate class (.bbclass) and configuration (.conf) files. This variable is analogous to the PATH variable.\nIf you run BitBake from a directory outside of the build directory, you must be sure to set BBPATH to point to the build directory. Set the variable as you would any environment variable and then run BitBake:",
-    "BBSERVER": "Points to the server that runs memory-resident BitBake. The variable is only used when you employ memory-resident BitBake.",
-    "BBTARGETS": "Allows you to use a configuration file to add to the list of command-line target recipes you want to build.",
-    "BB_ALLOWED_NETWORKS": "Specifies a space-delimited list of hosts that the fetcher is allowed to use to obtain the required source code. Following are considerations surrounding this variable:\nThis host list is only used if BB_NO_NETWORK is either not set or set to \u201c0\u201d.\nLimited support for the \u201c*\u201d wildcard character for matching against the beginning of host names exists. For example, the following setting matches git.gnu.org, ftp.gnu.org, and foo.git.gnu.org.\nImportant\nThe use of the \u201c*\u201d character only works at the beginning of a host name and it must be isolated from the remainder of the host name. You cannot use the wildcard character in any other location of the name or combined with the front part of the name.\nFor example, *.foo.bar is supported, while *aa.foo.bar is not.\nMirrors not in the host list are skipped and logged in debug.\nAttempts to access networks not in the host list cause a failure.\nUsing BB_ALLOWED_NETWORKS in conjunction with PREMIRRORS is very useful. Adding the host you want to use to PREMIRRORS results in the source code being fetched from an allowed location and avoids raising an error when a host that is not allowed is in a SRC_URI statement. This is because the fetcher does not attempt to use the host listed in SRC_URI after a successful fetch from the PREMIRRORS occurs.",
-    "BB_BASEHASH_IGNORE_VARS": "Lists variables that are excluded from checksum and dependency data. Variables that are excluded can therefore change without affecting the checksum mechanism. A common example would be the variable for the path of the build. BitBake\u2019s output should not (and usually does not) depend on the directory in which it was built.",
-    "BB_CACHEDIR": "Specifies the code parser cache directory (distinct from CACHE and PERSISTENT_DIR although they can be set to the same value if desired). The default value is \u201c${TOPDIR}/cache\u201d.",
-    "BB_CHECK_SSL_CERTS": "Specifies if SSL certificates should be checked when fetching. The default value is 1 and certificates are not checked if the value is set to 0.",
-    "BB_CONSOLELOG": "Specifies the path to a log file into which BitBake\u2019s user interface writes output during the build.",
-    "BB_CURRENTTASK": "Contains the name of the currently running task. The name does not include the do_ prefix.",
-    "BB_DANGLINGAPPENDS_WARNONLY": "Defines how BitBake handles situations where an append file (.bbappend) has no corresponding recipe file (.bb). This condition often occurs when layers get out of sync (e.g. oe-core bumps a recipe version and the old recipe no longer exists and the other layer has not been updated to the new version of the recipe yet).\nThe default fatal behavior is safest because it is the sane reaction given something is out of sync. It is important to realize when your changes are no longer being applied.",
-    "BB_DEFAULT_TASK": "The default task to use when none is specified (e.g. with the -c command line option). The task name specified should not include the do_ prefix.",
-    "BB_DEFAULT_UMASK": "The default umask to apply to tasks if specified and no task specific umask flag is set.",
-    "BB_DISKMON_DIRS": "Monitors disk space and available inodes during the build and allows you to control the build based on these parameters.\nDisk space monitoring is disabled by default. When setting this variable, use the following form:\nHere are some examples:\nThe first example works only if you also set the BB_DISKMON_WARNINTERVAL variable. This example causes the build system to immediately halt when either the disk space in ${TMPDIR} drops below 1 Gbyte or the available free inodes drops below 100 Kbytes. Because two directories are provided with the variable, the build system also issues a warning when the disk space in the ${SSTATE_DIR} directory drops below 1 Gbyte or the number of free inodes drops below 100 Kbytes. Subsequent warnings are issued during intervals as defined by the BB_DISKMON_WARNINTERVAL variable.\nThe second example stops the build after all currently executing tasks complete when the minimum disk space in the ${TMPDIR} directory drops below 1 Gbyte. No disk monitoring occurs for the free inodes in this case.\nThe final example immediately halts the build when the number of free inodes in the ${TMPDIR} directory drops below 100 Kbytes. No disk space monitoring for the directory itself occurs in this case.",
-    "BB_DISKMON_WARNINTERVAL": "Defines the disk space and free inode warning intervals.\nIf you are going to use the BB_DISKMON_WARNINTERVAL variable, you must also use the BB_DISKMON_DIRS variable and define its action as \u201cWARN\u201d. During the build, subsequent warnings are issued each time disk space or number of free inodes further reduces by the respective interval.\nIf you do not provide a BB_DISKMON_WARNINTERVAL variable and you do use BB_DISKMON_DIRS with the \u201cWARN\u201d action, the disk monitoring interval defaults to the following: BB_DISKMON_WARNINTERVAL = \u201c50M,5K\u201d\nWhen specifying the variable in your configuration file, use the following form:\nHere is an example:\nThese variables cause BitBake to issue subsequent warnings each time the available disk space further reduces by 50 Mbytes or the number of free inodes further reduces by 5 Kbytes in the ${SSTATE_DIR} directory. Subsequent warnings based on the interval occur each time a respective interval is reached beyond the initial warning (i.e. 1 Gbytes and 100 Kbytes).",
-    "BB_ENV_PASSTHROUGH": "Specifies the internal list of variables to allow through from the external environment into BitBake\u2019s datastore. If the value of this variable is not specified (which is the default), the following list is used: BBPATH, BB_PRESERVE_ENV, BB_ENV_PASSTHROUGH, and BB_ENV_PASSTHROUGH_ADDITIONS.\nNote\nYou must set this variable in the external environment in order for it to work.",
-    "BB_ENV_PASSTHROUGH_ADDITIONS": "Specifies an additional set of variables to allow through from the external environment into BitBake\u2019s datastore. This list of variables are on top of the internal list set in BB_ENV_PASSTHROUGH.\nNote\nYou must set this variable in the external environment in order for it to work.",
-    "BB_FETCH_PREMIRRORONLY": "When set to \u201c1\u201d, causes BitBake\u2019s fetcher module to only search PREMIRRORS for files. BitBake will not search the main SRC_URI or MIRRORS.",
-    "BB_FILENAME": "Contains the filename of the recipe that owns the currently running task. For example, if the do_fetch task that resides in the my-recipe.bb is executing, the BB_FILENAME variable contains \u201c/foo/path/my-recipe.bb\u201d.",
-    "BB_GENERATE_MIRROR_TARBALLS": "Causes tarballs of the Git repositories, including the Git metadata, to be placed in the DL_DIR directory. Anyone wishing to create a source mirror would want to enable this variable.\nFor performance reasons, creating and placing tarballs of the Git repositories is not the default action by BitBake.",
-    "BB_GENERATE_SHALLOW_TARBALLS": "Setting this variable to \u201c1\u201d when BB_GIT_SHALLOW is also set to \u201c1\u201d causes bitbake to generate shallow mirror tarballs when fetching git repositories. The number of commits included in the shallow mirror tarballs is controlled by BB_GIT_SHALLOW_DEPTH.\nIf both BB_GIT_SHALLOW and BB_GENERATE_MIRROR_TARBALLS are enabled, bitbake will generate shallow mirror tarballs by default for git repositories. This separate variable exists so that shallow tarball generation can be enabled without needing to also enable normal mirror generation if it is not desired.\nFor example usage, see BB_GIT_SHALLOW.",
-    "BB_GIT_SHALLOW": "Setting this variable to \u201c1\u201d enables the support for fetching, using and generating mirror tarballs of shallow git repositories. The external git-make-shallow script is used for shallow mirror tarball creation.\nWhen BB_GIT_SHALLOW is enabled, bitbake will attempt to fetch a shallow mirror tarball. If the shallow mirror tarball cannot be fetched, it will try to fetch the full mirror tarball and use that.\nWhen a mirror tarball is not available, a full git clone will be performed regardless of whether this variable is set or not. Support for shallow clones is not currently implemented as git does not directly support shallow cloning a particular git commit hash (it only supports cloning from a tag or branch reference).\nSee also BB_GIT_SHALLOW_DEPTH and BB_GENERATE_SHALLOW_TARBALLS.\nExample usage:",
-    "BB_GIT_SHALLOW_DEPTH": "When used with BB_GENERATE_SHALLOW_TARBALLS, this variable sets the number of commits to include in generated shallow mirror tarballs. With a depth of 1, only the commit referenced in SRCREV is included in the shallow mirror tarball. Increasing the depth includes additional parent commits, working back through the commit history.\nIf this variable is unset, bitbake will default to a depth of 1 when generating shallow mirror tarballs.\nFor example usage, see BB_GIT_SHALLOW.",
-    "BB_GLOBAL_PYMODULES": "Specifies the list of Python modules to place in the global namespace. It is intended that only the core layer should set this and it is meant to be a very small list, typically just os and sys. BB_GLOBAL_PYMODULES is expected to be set before the first addpylib directive. See also \u201cExtending Python Library Code\u201d.",
-    "BB_HASHCHECK_FUNCTION": "Specifies the name of the function to call during the \u201csetscene\u201d part of the task\u2019s execution in order to validate the list of task hashes. The function returns the list of setscene tasks that should be executed.\nAt this point in the execution of the code, the objective is to quickly verify if a given setscene function is likely to work or not. It\u2019s easier to check the list of setscene functions in one pass than to call many individual tasks. The returned list need not be completely accurate. A given setscene task can still later fail. However, the more accurate the data returned, the more efficient the build will be.",
-    "BB_HASHCONFIG_IGNORE_VARS": "Lists variables that are excluded from base configuration checksum, which is used to determine if the cache can be reused.\nOne of the ways BitBake determines whether to re-parse the main metadata is through checksums of the variables in the datastore of the base configuration data. There are variables that you typically want to exclude when checking whether or not to re-parse and thus rebuild the cache. As an example, you would usually exclude TIME and DATE because these variables are always changing. If you did not exclude them, BitBake would never reuse the cache.",
-    "BB_HASHSERVE": "Specifies the Hash Equivalence server to use.\nIf set to auto, BitBake automatically starts its own server over a UNIX domain socket. An option is to connect this server to an upstream one, by setting BB_HASHSERVE_UPSTREAM.\nIf set to unix://path, BitBake will connect to an existing hash server available over a UNIX domain socket.\nIf set to host:port, BitBake will connect to a remote server on the specified host. This allows multiple clients to share the same hash equivalence data.\nThe remote server can be started manually through the bin/bitbake-hashserv script provided by BitBake, which supports UNIX domain sockets too. This script also allows to start the server in read-only mode, to avoid accepting equivalences that correspond to Share State caches that are only available on specific clients.",
-    "BB_HASHSERVE_UPSTREAM": "Specifies an upstream Hash Equivalence server.\nThis optional setting is only useful when a local Hash Equivalence server is started (setting BB_HASHSERVE to auto), and you wish the local server to query an upstream server for Hash Equivalence data.\nExample usage:",
-    "BB_HASH_CODEPARSER_VALS": "Specifies values for variables to use when populating the codeparser cache. This can be used selectively to set dummy values for variables to avoid the codeparser cache growing on every parse. Variables that would typically be included are those where the value is not significant for where the codeparser cache is used (i.e. when calculating variable dependencies for code fragments.) The value is space-separated without quoting values, for example:",
-    "BB_INVALIDCONF": "Used in combination with the ConfigParsed event to trigger re-parsing the base metadata (i.e. all the recipes). The ConfigParsed event can set the variable to trigger the re-parse. You must be careful to avoid recursive loops with this functionality.",
-    "BB_LOGCONFIG": "Specifies the name of a config file that contains the user logging configuration. See Logging for additional information",
-    "BB_LOGFMT": "Specifies the name of the log files saved into ${T}. By default, the BB_LOGFMT variable is undefined and the log filenames get created using the following form:\nIf you want to force log files to take a specific name, you can set this variable in a configuration file.",
-    "BB_MULTI_PROVIDER_ALLOWED": "Allows you to suppress BitBake warnings caused when building two separate recipes that provide the same output.\nBitBake normally issues a warning when building two different recipes where each provides the same output. This scenario is usually something the user does not want. However, cases do exist where it makes sense, particularly in the virtual/* namespace. You can use this variable to suppress BitBake\u2019s warnings.\nTo use the variable, list provider names (e.g. recipe names, virtual/kernel, and so forth).",
-    "BB_NICE_LEVEL": "Allows BitBake to run at a specific priority (i.e. nice level). System permissions usually mean that BitBake can reduce its priority but not raise it again. See BB_TASK_NICE_LEVEL for additional information.",
-    "BB_NO_NETWORK": "Disables network access in the BitBake fetcher modules. With this access disabled, any command that attempts to access the network becomes an error.\nDisabling network access is useful for testing source mirrors, running builds when not connected to the Internet, and when operating in certain kinds of firewall environments.",
-    "BB_NUMBER_PARSE_THREADS": "Sets the number of threads BitBake uses when parsing. By default, the number of threads is equal to the number of cores on the system.",
-    "BB_NUMBER_THREADS": "The maximum number of tasks BitBake should run in parallel at any one time. If your host development system supports multiple cores, a good rule of thumb is to set this variable to twice the number of cores.",
-    "BB_ORIGENV": "Contains a copy of the original external environment in which BitBake was run. The copy is taken before any variable values configured to pass through from the external environment are filtered into BitBake\u2019s datastore.\nNote\nThe contents of this variable is a datastore object that can be queried using the normal datastore operations.",
-    "BB_PRESERVE_ENV": "Disables environment filtering and instead allows all variables through from the external environment into BitBake\u2019s datastore.\nNote\nYou must set this variable in the external environment in order for it to work.",
-    "BB_PRESSURE_MAX_CPU": "Specifies a maximum CPU pressure threshold, above which BitBake\u2019s scheduler will not start new tasks (providing there is at least one active task). If no value is set, CPU pressure is not monitored when starting tasks.\nThe pressure data is calculated based upon what Linux kernels since version 4.20 expose under /proc/pressure. The threshold represents the difference in \u201ctotal\u201d pressure from the previous second. The minimum value is 1.0 (extremely slow builds) and the maximum is 1000000 (a pressure value unlikely to ever be reached).\nThis threshold can be set in conf/local.conf as:",
-    "BB_PRESSURE_MAX_IO": "Specifies a maximum I/O pressure threshold, above which BitBake\u2019s scheduler will not start new tasks (providing there is at least one active task). If no value is set, I/O pressure is not monitored when starting tasks.\nThe pressure data is calculated based upon what Linux kernels since version 4.20 expose under /proc/pressure. The threshold represents the difference in \u201ctotal\u201d pressure from the previous second. The minimum value is 1.0 (extremely slow builds) and the maximum is 1000000 (a pressure value unlikely to ever be reached).\nAt this point in time, experiments show that IO pressure tends to be short-lived and regulating just the CPU with BB_PRESSURE_MAX_CPU can help to reduce it.",
-    "BB_PRESSURE_MAX_MEMORY": "Specifies a maximum memory pressure threshold, above which BitBake\u2019s scheduler will not start new tasks (providing there is at least one active task). If no value is set, memory pressure is not monitored when starting tasks.\nThe pressure data is calculated based upon what Linux kernels since version 4.20 expose under /proc/pressure. The threshold represents the difference in \u201ctotal\u201d pressure from the previous second. The minimum value is 1.0 (extremely slow builds) and the maximum is 1000000 (a pressure value unlikely to ever be reached).\nMemory pressure is experienced when time is spent swapping, refaulting pages from the page cache or performing direct reclaim. This is why memory pressure is rarely seen, but setting this variable might be useful as a last resort to prevent OOM errors if they are occurring during builds.",
-    "BB_RUNFMT": "Specifies the name of the executable script files (i.e. run files) saved into ${T}. By default, the BB_RUNFMT variable is undefined and the run filenames get created using the following form:\nIf you want to force run files to take a specific name, you can set this variable in a configuration file.",
-    "BB_RUNTASK": "Contains the name of the currently executing task. The value includes the \u201cdo_\u201d prefix. For example, if the currently executing task is do_config, the value is \u201cdo_config\u201d.",
-    "BB_SCHEDULER": "Selects the name of the scheduler to use for the scheduling of BitBake tasks. Three options exist:\nbasic \u2014 the basic framework from which everything derives. Using this option causes tasks to be ordered numerically as they are parsed.\nspeed \u2014 executes tasks first that have more tasks depending on them. The \u201cspeed\u201d option is the default.\ncompletion \u2014 causes the scheduler to try to complete a given recipe once its build has started.",
-    "BB_SCHEDULERS": "Defines custom schedulers to import. Custom schedulers need to be derived from the RunQueueScheduler class.\nFor information how to select a scheduler, see the BB_SCHEDULER variable.",
-    "BB_SETSCENE_DEPVALID": "Specifies a function BitBake calls that determines whether BitBake requires a setscene dependency to be met.\nWhen running a setscene task, BitBake needs to know which dependencies of that setscene task also need to be run. Whether dependencies also need to be run is highly dependent on the metadata. The function specified by this variable returns a \u201cTrue\u201d or \u201cFalse\u201d depending on whether the dependency needs to be met.",
-    "BB_SIGNATURE_EXCLUDE_FLAGS": "Lists variable flags (varflags) that can be safely excluded from checksum and dependency data for keys in the datastore. When generating checksum or dependency data for keys in the datastore, the flags set against that key are normally included in the checksum.\nFor more information on varflags, see the \u201cVariable Flags\u201d section.",
-    "BB_SIGNATURE_HANDLER": "Defines the name of the signature handler BitBake uses. The signature handler defines the way stamp files are created and handled, if and how the signature is incorporated into the stamps, and how the signature itself is generated.\nA new signature handler can be added by injecting a class derived from the SignatureGenerator class into the global namespace.",
-    "BB_SRCREV_POLICY": "Defines the behavior of the fetcher when it interacts with source control systems and dynamic source revisions. The BB_SRCREV_POLICY variable is useful when working without a network.\nThe variable can be set using one of two policies:\ncache \u2014 retains the value the system obtained previously rather than querying the source control system each time.\nclear \u2014 queries the source controls system every time. With this policy, there is no cache. The \u201cclear\u201d policy is the default.",
-    "BB_STRICT_CHECKSUM": "Sets a more strict checksum mechanism for non-local URLs. Setting this variable to a value causes BitBake to report an error if it encounters a non-local URL that does not have at least one checksum specified.",
-    "BB_TASKHASH": "Within an executing task, this variable holds the hash of the task as returned by the currently enabled signature generator.",
-    "BB_TASK_IONICE_LEVEL": "Allows adjustment of a task\u2019s Input/Output priority. During Autobuilder testing, random failures can occur for tasks due to I/O starvation. These failures occur during various QEMU runtime timeouts. You can use the BB_TASK_IONICE_LEVEL variable to adjust the I/O priority of these tasks.\nNote\nThis variable works similarly to the BB_TASK_NICE_LEVEL variable except with a task\u2019s I/O priorities.\nSet the variable as follows:\nFor class, the default value is \u201c2\u201d, which is a best effort. You can use \u201c1\u201d for realtime and \u201c3\u201d for idle. If you want to use realtime, you must have superuser privileges.\nFor prio, you can use any value from \u201c0\u201d, which is the highest priority, to \u201c7\u201d, which is the lowest. The default value is \u201c4\u201d. You do not need any special privileges to use this range of priority values.\nNote\nIn order for your I/O priority settings to take effect, you need the Completely Fair Queuing (CFQ) Scheduler selected for the backing block device. To select the scheduler, use the following command form where device is the device (e.g. sda, sdb, and so forth):",
-    "BB_TASK_NICE_LEVEL": "Allows specific tasks to change their priority (i.e. nice level).\nYou can use this variable in combination with task overrides to raise or lower priorities of specific tasks. For example, on the Yocto Project autobuilder, QEMU emulation in images is given a higher priority as compared to build tasks to ensure that images do not suffer timeouts on loaded systems.",
-    "BB_VERBOSE_LOGS": "Controls how verbose BitBake is during builds. If set, shell scripts echo commands and shell script output appears on standard out (stdout).",
-    "BB_WORKERCONTEXT": "Specifies if the current context is executing a task. BitBake sets this variable to \u201c1\u201d when a task is being executed. The value is not set when the task is in server context during parsing or event handling.",
-    "BITBAKE_UI": "Used to specify the UI module to use when running BitBake. Using this variable is equivalent to using the -u command-line option.\nNote\nYou must set this variable in the external environment in order for it to work.",
-    "BUILDNAME": "A name assigned to the build. The name defaults to a datetime stamp of when the build was started but can be defined by the metadata.",
-    "BZRDIR": "The directory in which files checked out of a Bazaar system are stored.",
-    "CACHE": "Specifies the directory BitBake uses to store a cache of the metadata so it does not need to be parsed every time BitBake is started.",
-    "CVSDIR": "The directory in which files checked out under the CVS system are stored.",
-    "DEFAULT_PREFERENCE": "Specifies a weak bias for recipe selection priority.\nThe most common usage of this is variable is to set it to \u201c-1\u201d within a recipe for a development version of a piece of software. Using the variable in this way causes the stable version of the recipe to build by default in the absence of PREFERRED_VERSION being used to build the development version.\nNote\nThe bias provided by DEFAULT_PREFERENCE is weak and is overridden by BBFILE_PRIORITY if that variable is different between two layers that contain different versions of the same recipe.",
-    "DEPENDS": "Lists a recipe\u2019s build-time dependencies (i.e. other recipe files).\nConsider this simple example for two recipes named \u201ca\u201d and \u201cb\u201d that produce similarly named packages. In this example, the DEPENDS statement appears in the \u201ca\u201d recipe:\nHere, the dependency is such that the do_configure task for recipe \u201ca\u201d depends on the do_populate_sysroot task of recipe \u201cb\u201d. This means anything that recipe \u201cb\u201d puts into sysroot is available when recipe \u201ca\u201d is configuring itself.\nFor information on runtime dependencies, see the RDEPENDS variable.",
-    "DESCRIPTION": "A long description for the recipe.",
-    "DL_DIR": "The central download directory used by the build process to store downloads. By default, DL_DIR gets files suitable for mirroring for everything except Git repositories. If you want tarballs of Git repositories, use the BB_GENERATE_MIRROR_TARBALLS variable.",
-    "EXCLUDE_FROM_WORLD": "Directs BitBake to exclude a recipe from world builds (i.e. bitbake world). During world builds, BitBake locates, parses and builds all recipes found in every layer exposed in the bblayers.conf configuration file.\nTo exclude a recipe from a world build using this variable, set the variable to \u201c1\u201d in the recipe. Set it to \u201c0\u201d to add it back to world build.\nNote\nRecipes added to EXCLUDE_FROM_WORLD may still be built during a world build in order to satisfy dependencies of other recipes. Adding a recipe to EXCLUDE_FROM_WORLD only ensures that the recipe is not explicitly added to the list of build targets in a world build.",
-    "FAKEROOT": "Contains the command to use when running a shell script in a fakeroot environment. The FAKEROOT variable is obsolete and has been replaced by the other FAKEROOT* variables. See these entries in the glossary for more information.",
-    "FAKEROOTBASEENV": "Lists environment variables to set when executing the command defined by FAKEROOTCMD that starts the bitbake-worker process in the fakeroot environment.",
-    "FAKEROOTCMD": "Contains the command that starts the bitbake-worker process in the fakeroot environment.",
-    "FAKEROOTDIRS": "Lists directories to create before running a task in the fakeroot environment.",
-    "FAKEROOTENV": "Lists environment variables to set when running a task in the fakeroot environment. For additional information on environment variables and the fakeroot environment, see the FAKEROOTBASEENV variable.",
-    "FAKEROOTNOENV": "Lists environment variables to set when running a task that is not in the fakeroot environment. For additional information on environment variables and the fakeroot environment, see the FAKEROOTENV variable.",
-    "FETCHCMD": "Defines the command the BitBake fetcher module executes when running fetch operations. You need to use an override suffix when you use the variable (e.g. FETCHCMD_git or FETCHCMD_svn).",
-    "FILE": "Points at the current file. BitBake sets this variable during the parsing process to identify the file being parsed. BitBake also sets this variable when a recipe is being executed to identify the recipe file.",
-    "FILESPATH": "Specifies directories BitBake uses when searching for patches and files. The \u201clocal\u201d fetcher module uses these directories when handling file:// URLs. The variable behaves like a shell PATH environment variable. The value is a colon-separated list of directories that are searched left-to-right in order.",
-    "GITDIR": "The directory in which a local copy of a Git repository is stored when it is cloned.",
-    "HGDIR": "The directory in which files checked out of a Mercurial system are stored.",
+    "ALLOW_EMPTY": "Specifies if an output package should still be produced if it is empty.",
+    "ALTERNATIVE": "Lists commands in a package that need an alternative binary naming scheme.",
+    "ALTERNATIVE_LINK_NAME": "Used by the alternatives system to map duplicated commands to actual locations.",
+    "ALTERNATIVE_PRIORITY": "Used by the alternatives system to create default priorities for duplicated commands.",
+    "ALTERNATIVE_TARGET": "Used by the alternatives system to create default link locations for duplicated commands.",
+    "ANY_OF_COMBINED_FEATURES": "When a recipe inherits the features_check class, at least one item in this variable must be included in COMBINED_FEATURES.",
+    "ANY_OF_DISTRO_FEATURES": "When a recipe inherits the features_check class, at least one item in this variable must be included in DISTRO_FEATURES.",
+    "ANY_OF_MACHINE_FEATURES": "When a recipe inherits the features_check class, at least one item in this variable must be included in MACHINE_FEATURES.",
+    "ASSUME_PROVIDED": "List of packages (recipes actually) that are assumed to be implicitly available. BitBake does not build these packages.",
+    "ASSUME_SHLIBS": "List of shlib:package[_version] mappings. Useful for lib packages in ASSUME_PROVIDED, for which automatic shlib dependency tracking does not work.",
+    "AUTHOR": "Email address used to contact the original author(s) in order to send patches and forward bugs.",
+    "AUTOREV": "When SRCREV is set to the value of this variable, it specifies to use the latest source revision in the repository.",
+    "AUTO_SYSLINUXMENU": "Enables creating an automatic menu for the syslinux bootloader.",
+    "B": "The Build Directory. The OpenEmbedded build system places generated objects into the Build Directory during a recipe's build process.",
+    "BAD_RECOMMENDATIONS": "A list of packages not to install despite being recommended by a recipe. Support for this variable exists only when using the IPK or RPM packaging backends.",
+    "BBCLASSEXTEND": "Allows you to extend a recipe so that it builds variants of the software. Common variants for recipes are 'native', 'cross', 'nativesdk' and multilibs.",
+    "BBFILES": "List of recipe files used by BitBake to build software.",
+    "BBFILE_COLLECTIONS": "Lists the names of configured layers. These names are used to find the other BBFILE_* variables.",
+    "BBFILE_PATTERN": "Variable that expands to match files from BBFILES in a particular layer. This variable is used in the layer.conf file and must be suffixed with the name of a layer.",
+    "BBFILE_PRIORITY": "Assigns the priority for recipe files in each layer. Setting this variable allows you to prioritize a layer against other layers that contain the same recipe.",
+    "BBINCLUDELOGS": "Variable that controls how BitBake displays logs on build failure.",
+    "BBINCLUDELOGS_LINES": "Amount of log lines printed on failure.",
+    "BBLAYERS": "Lists the layers to enable during the build. This variable is defined in the bblayers.conf configuration file.",
+    "BBMASK": "Prevents BitBake from processing specific recipes or recipe append files.",
+    "BBPATH": "Used by BitBake to locate .bbclass and configuration files. This variable is analogous to the PATH variable.",
+    "BBSERVER": "Points to the server that runs memory-resident BitBake.",
+    "BB_DANGLINGAPPENDS_WARNONLY": "Defines how BitBake handles situations where an append file (.bbappend) has no corresponding recipe file (.bb).",
+    "BB_DISKMON_DIRS": "Monitors disk space and available inodes during the build and allows you to control the build based on these parameters.",
+    "BB_DISKMON_WARNINTERVAL": "Defines the disk space and free inode warning intervals. To set these intervals, define the variable in the conf/local.conf file in the Build Directory.",
+    "BB_GENERATE_MIRROR_TARBALLS": "Causes tarballs of the Git repositories to be placed in the DL_DIR directory.",
+    "BB_NUMBER_THREADS": "The maximum number of tasks BitBake should run in parallel at any one time. A good rule of thumb is to set this variable to twice the number of cores.",
+    "BINCONFIG_GLOB": "When inheriting binconfig.bbclass from a recipe, this variable specifies a wildcard for configuration scripts that need editing.",
+    "BP": "The base recipe name and version but without any special recipe name suffix (i.e. -native, lib64-, and so forth). BP is comprised of ${BPN}-${PV}",
+    "BPN": "The bare name of the recipe. This variable is a version of the PN variable but removes common suffixes and prefixes.",
+    "BUGTRACKER": "Specifies a URL for an upstream bug tracking website for a recipe.",
+    "BUILDDIR": "Points to the location of the Build Directory.",
+    "BUILDSTATS_BASE": "Points to the location of the directory that holds build statistics when you use and enable the buildstats class.",
+    "BUILD_ARCH": "The name of the building architecture (e.g. i686).",
+    "BUILD_OS": "The operating system (in lower case) of the building architecture (e.g. linux).",
+    "BUSYBOX_SPLIT_SUID": "For the BusyBox recipe, specifies whether to split the output executable file into two parts: one for features that require setuid root, and one for the remaining features.",
+    "CACHE": "The directory holding the cache of the metadata.",
+    "CFLAGS": "Flags passed to the C compiler for the target system. This variable evaluates to the same as TARGET_CFLAGS.",
+    "CLASSOVERRIDE": "An internal variable specifying the special class override that should currently apply (e.g. 'class-target', 'class-native', and so forth).",
+    "CLEANBROKEN": "Specifies if 'make clean' does not work for a recipe (and therefore the build system should not try to use it during do_configure)",
+    "COMBINED_FEATURES": "A set of features common between MACHINE_FEATURES and DISTRO_FEATURES.",
+    "COMMON_LICENSE_DIR": "Points to meta/files/common-licenses in the Source Directory, which is where generic license files reside.",
+    "COMPATIBLE_HOST": "A regular expression that resolves to one or more hosts (when the recipe is native) or one or more targets (when the recipe is non-native) with which a recipe is compatible.",
+    "COMPATIBLE_MACHINE": "A regular expression that resolves to one or more target machines with which a recipe is compatible.",
+    "COMPLEMENTARY_GLOB": "Defines wildcards to match when installing a list of complementary packages for all the packages installed in an image.",
+    "CONFFILES": "Identifies editable or configurable files that are part of a package.",
+    "CONFIG_SITE": "A list of files that contains autoconf test results relevant to the current build. This variable is used by the Autotools utilities when running configure.",
+    "CONFLICT_COMBINED_FEATURES": "When a recipe inherits the features_check class, no item in this variable can be included in COMBINED_FEATURES.",
+    "CONFLICT_DISTRO_FEATURES": "When a recipe inherits the features_check class, no item in this variable can be included in DISTRO_FEATURES.",
+    "CONFLICT_MACHINE_FEATURES": "When a recipe inherits the features_check class, no item in this variable can be included in MACHINE_FEATURES.",
+    "CONF_VERSION": "Tracks the version of local.conf.  Increased each time build/conf/ changes incompatibly.",
+    "COREBASE": "Specifies the parent directory of the OpenEmbedded Core Metadata layer (i.e. meta).",
+    "CORE_IMAGE_EXTRA_INSTALL": "Specifies the list of packages to be added to the image. You should only set this variable in the conf/local.conf file in the Build Directory.",
+    "CVE_CHECK_LAYER_EXCLUDELIST": "Defines which layers to exclude from cve-check scanning",
+    "CVE_CHECK_LAYER_INCLUDELIST": "Defines which layers to include during cve-check scanning",
+    "D": "The destination directory.",
+    "DATE": "The date the build was started using YMD format.",
+    "DATETIME": "The date and time the build was started.",
+    "DEBUG_BUILD": "Specifies to build packages with debugging information. This influences the value of the SELECTED_OPTIMIZATION variable.",
+    "DEBUG_OPTIMIZATION": "The options to pass in TARGET_CFLAGS and CFLAGS when compiling a system for debugging. This variable defaults to '-Og ${DEBUG_FLAGS} -pipe'.",
+    "DEFAULT_PREFERENCE": "Specifies a weak bias for recipe selection priority.",
+    "DEPENDS": "Lists a recipe's build-time dependencies (i.e. other recipe files).",
+    "DEPLOYDIR": "For recipes that inherit the deploy class, the DEPLOYDIR points to a temporary work area for deployed files.",
+    "DEPLOY_DIR": "Points to the general area that the OpenEmbedded build system uses to place images, packages, SDKs and other output files that are ready to be used outside of the build system.",
+    "DEPLOY_DIR_IMAGE": "Points to the area that the OpenEmbedded build system uses to place images and other associated output files that are ready to be deployed onto the target machine.",
+    "DESCRIPTION": "The package description used by package managers. If not set, DESCRIPTION takes the value of the SUMMARY variable.",
+    "DISTRO": "The short name of the distribution. If the variable is blank, meta/conf/distro/defaultsetup.conf will be used.",
+    "DISTROOVERRIDES": "Lists overrides specific to the current distribution. By default, the variable list includes the value of the DISTRO variable.",
+    "DISTRO_EXTRA_RDEPENDS": "Specifies a list of distro-specific packages to add to all images. The variable only applies to the images that include packagegroup-base.",
+    "DISTRO_EXTRA_RRECOMMENDS": "Specifies a list of distro-specific packages to add to all images if the packages exist. The list of packages are automatically installed but you can remove them.",
+    "DISTRO_FEATURES": "The features enabled for the distribution.",
+    "DISTRO_FEATURES_BACKFILL": "Features to be added to DISTRO_FEATURES if not also present in DISTRO_FEATURES_BACKFILL_CONSIDERED. This variable is set in the meta/conf/bitbake.conf file and it is not intended to be user-configurable.",
+    "DISTRO_FEATURES_BACKFILL_CONSIDERED": "Features from DISTRO_FEATURES_BACKFILL that should not be backfilled (i.e. added to DISTRO_FEATURES) during the build.",
+    "DISTRO_NAME": "The long name of the distribution.",
+    "DISTRO_PN_ALIAS": "Alias names used for the recipe in various Linux distributions.",
+    "DISTRO_VERSION": "The version of the distribution.",
+    "DL_DIR": "The central download directory used by the build process to store downloads. By default, the directory is 'downloads' in the Build Directory.",
+    "ENABLE_BINARY_LOCALE_GENERATION": "Controls which locales for glibc are generated during the build. The variable is useful if the target device has 64Mbytes of RAM or less.",
+    "ERROR_QA": "Specifies the quality assurance checks whose failures are reported as errors by the OpenEmbedded build system.",
+    "EXCLUDE_FROM_WORLD": "Directs BitBake to exclude a recipe from world builds (i.e. bitbake world).",
+    "EXTENDPE": "Used with file and pathnames to create a prefix for a recipe's version based on the recipe's PE value. If PE is set and greater than zero for a recipe, EXTENDPE becomes that value.",
+    "EXTENDPKGV": "The full package version specification as it appears on the final packages produced by a recipe.",
+    "EXTERNALSRC": "If externalsrc.bbclass is inherited, this variable points to the source tree, which is outside of the OpenEmbedded build system.",
+    "EXTERNALSRC_BUILD": "If externalsrc.bbclass is inherited, this variable points to the directory in which the recipe's source code is built, which is outside of the OpenEmbedded build system.",
+    "EXTRA_IMAGEDEPENDS": "A list of recipes to build that do not provide packages for installing into the root filesystem. Use this variable to list recipes that are required to build the final image, but not needed in the root filesystem.",
+    "EXTRA_IMAGE_FEATURES": "The list of additional features to include in an image. Configure this variable in the conf/local.conf file in the Build Directory.",
+    "EXTRA_OECMAKE": "Additional cmake options.",
+    "EXTRA_OECONF": "Additional configure script options.",
+    "EXTRA_OEMAKE": "Additional GNU make options.",
+    "EXTRA_OESCONS": "When a recipe inherits the scons class, this variable specifies additional configuration options you want to pass to the scons command line.",
+    "EXTRA_QMAKEVARS_POST": "Configuration variables or options you want to pass to qmake when the arguments need to be after the .pro file list on the command line.",
+    "EXTRA_QMAKEVARS_PRE": "Configuration variables or options you want to pass to qmake when the arguments need to be before the .pro file list on the command line.",
+    "EXTRA_USERS_PARAMS": "When a recipe inherits the extrausers class, this variable provides image level user and group operations.",
+    "FEED_DEPLOYDIR_BASE_URI": "Allow to serve ipk deploy directory as an ad hoc feed (bogofeed). Set to base URL of the directory as exported by HTTP. Set of ad hoc feed configs will be generated in the image.",
+    "FILES": "The list of directories or files that are placed in packages.",
+    "FILESEXTRAPATHS": "Extends the search path the OpenEmbedded build system uses when looking for files and patches as it processes recipes and append files.",
+    "FILESOVERRIDES": "A subset of OVERRIDES used by the OpenEmbedded build system for creating FILESPATH.",
+    "FILESPATH": "The default set of directories the OpenEmbedded build system uses when searching for patches and files. It is defined in the base.bbclass class found in meta/classes in the Source Directory. Do not hand-edit the FILESPATH variable.",
+    "FILESYSTEM_PERMS_TABLES": "Allows you to define your own file permissions settings table as part of your configuration for the packaging process.",
+    "FONT_EXTRA_RDEPENDS": "When a recipe inherits the fontcache class, this variable specifies runtime dependencies for font packages. This variable defaults to 'fontconfig-utils'.",
+    "FONT_PACKAGES": "When a recipe inherits the fontcache class, this variable identifies packages containing font files that need to be cached by Fontconfig.",
+    "FULL_OPTIMIZATION": "The options to pass in TARGET_CFLAGS and CFLAGS when compiling an optimized system. This variable defaults to '-O2 -pipe ${DEBUG_FLAGS}'.",
+    "GROUPADD_PARAM": "When a recipe inherits the useradd class, this variable specifies for a package what parameters should be passed to the groupadd command if you wish to add a group to the system when the package is installed.",
+    "GROUPMEMS_PARAM": "When a recipe inherits the useradd class, this variable specifies for a package what parameters should be passed to the groupmems command if you wish to modify the members of a group when the package is installed.",
+    "GRUB_GFXSERIAL": "Configures the GNU GRand Unified Bootloader (GRUB) to have graphics and serial in the boot menu.",
+    "GRUB_OPTS": "Additional options to add to the GNU GRand Unified Bootloader (GRUB) configuration.",
+    "GRUB_TIMEOUT": "Specifies the timeout before executing the default LABEL in the GNU GRand Unified Bootloader (GRUB).",
+    "GTKIMMODULES_PACKAGES": "For recipes that inherit the gtk-immodules-cache class, this variable specifies the packages that contain the GTK+ input method modules being installed when the modules are in packages other than the main package.",
     "HOMEPAGE": "Website where more information about the software the recipe is building can be found.",
-    "INHERIT": "Causes the named class or classes to be inherited globally. Anonymous functions in the class or classes are not executed for the base configuration and in each individual recipe. The OpenEmbedded build system ignores changes to INHERIT in individual recipes.\nFor more information on INHERIT, see the \u201cINHERIT Configuration Directive\u201d section.",
-    "LAYERDEPENDS": "Lists the layers, separated by spaces, upon which this recipe depends. Optionally, you can specify a specific layer version for a dependency by adding it to the end of the layer name with a colon, (e.g. \u201canotherlayer:3\u201d to be compared against LAYERVERSION_anotherlayer in this case). BitBake produces an error if any dependency is missing or the version numbers do not match exactly (if specified).\nYou use this variable in the conf/layer.conf file. You must also use the specific layer name as a suffix to the variable (e.g. LAYERDEPENDS_mylayer).",
-    "LAYERDIR": "When used inside the layer.conf configuration file, this variable provides the path of the current layer. This variable is not available outside of layer.conf and references are expanded immediately when parsing of the file completes.",
-    "LAYERDIR_RE": "When used inside the layer.conf configuration file, this variable provides the path of the current layer, escaped for use in a regular expression (BBFILE_PATTERN). This variable is not available outside of layer.conf and references are expanded immediately when parsing of the file completes.",
-    "LAYERSERIES_COMPAT": "Lists the versions of the OpenEmbedded-Core (OE-Core) for which a layer is compatible. Using the LAYERSERIES_COMPAT variable allows the layer maintainer to indicate which combinations of the layer and OE-Core can be expected to work. The variable gives the system a way to detect when a layer has not been tested with new releases of OE-Core (e.g. the layer is not maintained).\nTo specify the OE-Core versions for which a layer is compatible, use this variable in your layer\u2019s conf/layer.conf configuration file. For the list, use the Yocto Project release name (e.g. \u201ckirkstone\u201d, \u201cmickledore\u201d). To specify multiple OE-Core versions for the layer, use a space-separated list:\nNote\nSetting LAYERSERIES_COMPAT is required by the Yocto Project Compatible version 2 standard. The OpenEmbedded build system produces a warning if the variable is not set for any given layer.",
-    "LAYERVERSION": "Optionally specifies the version of a layer as a single number. You can use this variable within LAYERDEPENDS for another layer in order to depend on a specific version of the layer.\nYou use this variable in the conf/layer.conf file. You must also use the specific layer name as a suffix to the variable (e.g. LAYERDEPENDS_mylayer).",
-    "LICENSE": "The list of source licenses for the recipe.",
-    "MIRRORS": "Specifies additional paths from which BitBake gets source code. When the build system searches for source code, it first tries the local download directory. If that location fails, the build system tries locations defined by PREMIRRORS, the upstream source, and then locations specified by MIRRORS in that order.",
-    "OVERRIDES": "BitBake uses OVERRIDES to control what variables are overridden after BitBake parses recipes and configuration files.\nFollowing is a simple example that uses an overrides list based on machine architectures: OVERRIDES = \u201carm:x86:mips:powerpc\u201d You can find information on how to use OVERRIDES in the \u201cConditional Syntax (Overrides)\u201d section.",
-    "P4DIR": "The directory in which a local copy of a Perforce depot is stored when it is fetched.",
-    "PACKAGES": "The list of packages the recipe creates.",
-    "PACKAGES_DYNAMIC": "A promise that your recipe satisfies runtime dependencies for optional modules that are found in other recipes. PACKAGES_DYNAMIC does not actually satisfy the dependencies, it only states that they should be satisfied. For example, if a hard, runtime dependency (RDEPENDS) of another package is satisfied during the build through the PACKAGES_DYNAMIC variable, but a package with the module name is never actually produced, then the other package will be broken.",
-    "PE": "The epoch of the recipe. By default, this variable is unset. The variable is used to make upgrades possible when the versioning scheme changes in some backwards incompatible way.",
-    "PERSISTENT_DIR": "Specifies the directory BitBake uses to store data that should be preserved between builds. In particular, the data stored is the data that uses BitBake\u2019s persistent data API and the data used by the PR Server and PR Service.",
-    "PF": "Specifies the recipe or package name and includes all version and revision numbers (i.e. eglibc-2.13-r20+svnr15508/ and bash-4.2-r1/).",
-    "PN": "The recipe name.",
-    "PR": "The revision of the recipe.",
-    "PREFERRED_PROVIDER": "Determines which recipe should be given preference when multiple recipes provide the same item. You should always suffix the variable with the name of the provided item, and you should set it to the PN of the recipe to which you want to give precedence. Some examples:",
-    "PREFERRED_PROVIDERS": "Determines which recipe should be given preference for cases where multiple recipes provide the same item. Functionally, PREFERRED_PROVIDERS is identical to PREFERRED_PROVIDER. However, the PREFERRED_PROVIDERS variable lets you define preferences for multiple situations using the following form:\nThis form is a convenient replacement for the following:",
-    "PREFERRED_VERSION": "If there are multiple versions of a recipe available, this variable determines which version should be given preference. You must always suffix the variable with the PN you want to select, and you should set PV accordingly for precedence.\nThe PREFERRED_VERSION variable supports limited wildcard use through the \u201c%\u201d character. You can use the character to match any number of characters, which can be useful when specifying versions that contain long revision numbers that potentially change. Here are two examples:\nImportant\nThe use of the \u201c % \u201c character is limited in that it only works at the end of the string. You cannot use the wildcard character in any other location of the string.\nIf a recipe with the specified version is not available, a warning message will be shown. See REQUIRED_VERSION if you want this to be an error instead.",
-    "PREMIRRORS": "Specifies additional paths from which BitBake gets source code. When the build system searches for source code, it first tries the local download directory. If that location fails, the build system tries locations defined by PREMIRRORS, the upstream source, and then locations specified by MIRRORS in that order.\nTypically, you would add a specific server for the build system to attempt before any others by adding something like the following to your configuration:\nThese changes cause the build system to intercept Git, FTP, HTTP, and HTTPS requests and direct them to the http:// sources mirror. You can use file:// URLs to point to local directories or network shares as well.",
-    "PROVIDES": "A list of aliases by which a particular recipe can be known. By default, a recipe\u2019s own PN is implicitly already in its PROVIDES list. If a recipe uses PROVIDES, the additional aliases are synonyms for the recipe and can be useful satisfying dependencies of other recipes during the build as specified by DEPENDS.\nConsider the following example PROVIDES statement from a recipe file libav_0.8.11.bb:\nThe PROVIDES statement results in the \u201clibav\u201d recipe also being known as \u201clibpostproc\u201d.\nIn addition to providing recipes under alternate names, the PROVIDES mechanism is also used to implement virtual targets. A virtual target is a name that corresponds to some particular functionality (e.g. a Linux kernel). Recipes that provide the functionality in question list the virtual target in PROVIDES. Recipes that depend on the functionality in question can include the virtual target in DEPENDS to leave the choice of provider open.\nConventionally, virtual targets have names on the form \u201cvirtual/function\u201d (e.g. \u201cvirtual/kernel\u201d). The slash is simply part of the name and has no syntactical significance.",
-    "PRSERV_HOST": "The network based PR service host and port.\nFollowing is an example of how the PRSERV_HOST variable is set:\nYou must set the variable if you want to automatically start a local PR service. You can set PRSERV_HOST to other values to use a remote PR service.",
-    "PV": "The version of the recipe.",
-    "RDEPENDS": "Lists a package\u2019s runtime dependencies (i.e. other packages) that must be installed in order for the built package to run correctly. If a package in this list cannot be found during the build, you will get a build error.\nBecause the RDEPENDS variable applies to packages being built, you should always use the variable in a form with an attached package name. For example, suppose you are building a development package that depends on the perl package. In this case, you would use the following RDEPENDS statement:\nIn the example, the development package depends on the perl package. Thus, the RDEPENDS variable has the ${PN}-dev package name as part of the variable.\nBitBake supports specifying versioned dependencies. Although the syntax varies depending on the packaging format, BitBake hides these differences from you. Here is the general syntax to specify versions with the RDEPENDS variable:\nFor operator, you can specify the following:\nFor example, the following sets up a dependency on version 1.2 or greater of the package foo:\nFor information on build-time dependencies, see the DEPENDS variable.",
-    "REPODIR": "The directory in which a local copy of a google-repo directory is stored when it is synced.",
-    "REQUIRED_VERSION": "If there are multiple versions of a recipe available, this variable determines which version should be given preference. REQUIRED_VERSION works in exactly the same manner as PREFERRED_VERSION, except that if the specified version is not available then an error message is shown and the build fails immediately.\nIf both REQUIRED_VERSION and PREFERRED_VERSION are set for the same recipe, the REQUIRED_VERSION value applies.",
-    "RPROVIDES": "A list of package name aliases that a package also provides. These aliases are useful for satisfying runtime dependencies of other packages both during the build and on the target (as specified by RDEPENDS).\nAs with all package-controlling variables, you must always use the variable in conjunction with a package name override. Here is an example:",
-    "RRECOMMENDS": "A list of packages that extends the usability of a package being built. The package being built does not depend on this list of packages in order to successfully build, but needs them for the extended usability. To specify runtime dependencies for packages, see the RDEPENDS variable.\nBitBake supports specifying versioned recommends. Although the syntax varies depending on the packaging format, BitBake hides these differences from you. Here is the general syntax to specify versions with the RRECOMMENDS variable:\nFor operator, you can specify the following:\nFor example, the following sets up a recommend on version 1.2 or greater of the package foo:",
-    "SECTION": "The section in which packages should be categorized.",
+    "HOST_ARCH": "The name of the target architecture. Normally same as the TARGET_ARCH.",
+    "HOST_CC_ARCH": "The name of the host architecture. Normally same as the TARGET_CC_ARCH.",
+    "HOST_OS": "The name of the target operating system. Normally the same as the TARGET_OS.",
+    "HOST_PREFIX": "The prefix for the cross compile toolchain. Normally same as the TARGET_PREFIX.",
+    "HOST_SYS": "Specifies the system, including the architecture and the operating system, for with the build is occurring in the context of the current recipe.",
+    "HOST_VENDOR": "The name of the vendor. Normally same as the TARGET_VENDOR.",
+    "ICECC_CLASS_DISABLE": "Identifies user classes that you do not want the Icecream distributed compile support to consider.",
+    "ICECC_ENV_EXEC": "Points to the icecc-create-env script that you provide.",
+    "ICECC_PATH": "The location of the icecc binary.",
+    "ICECC_RECIPE_DISABLE": "Identifies user recipes that you do not want the Icecream distributed compile support to consider.",
+    "ICECC_RECIPE_ENABLE": "Identifies user recipes that use an empty PARALLEL_MAKE variable that you want to force remote distributed compilation on using the Icecream distributed compile support.",
+    "IMAGE_BASENAME": "The base name of image output files.",
+    "IMAGE_BOOT_FILES": "Whitespace separated list of files from ${DEPLOY_DIR_IMAGE} to place in boot partition. Entries will be installed under a same name as the source file. To change the destination file name, pass a desired name after a semicolon (eg. u-boot.img;uboot).",
+    "IMAGE_CLASSES": "A list of classes that all images should inherit.",
+    "IMAGE_FEATURES": "The primary list of features to include in an image. Configure this variable in an image recipe.",
+    "IMAGE_FSTYPES": "Formats of root filesystem images that you want to have created.",
+    "IMAGE_FSTYPES_DEBUGFS": "Formats of the debug root filesystem images that you want to have created.",
+    "IMAGE_GEN_DEBUGFS": "When set to '1', generate a companion debug object/source filesystem image.",
+    "IMAGE_INSTALL": "Specifies the packages to install into an image. Image recipes set IMAGE_INSTALL to specify the packages to install into an image through image.bbclass.",
+    "IMAGE_LINGUAS": "Specifies the list of locales to install into the image during the root filesystem construction process.",
+    "IMAGE_NAME": "The name of the output image files minus the extension.",
+    "IMAGE_OVERHEAD_FACTOR": "Defines a multiplier that the build system applies to the initial image size for cases when the multiplier times the returned disk usage value for the image is greater than the sum of IMAGE_ROOTFS_SIZE and IMAGE_ROOTFS_EXTRA_SPACE.",
+    "IMAGE_PKGTYPE": "Defines the package type (DEB, RPM, IPK, or TAR) used by the OpenEmbedded build system.",
+    "IMAGE_POSTPROCESS_COMMAND": "Added by classes to run post processing commands once the OpenEmbedded build system has created the image.",
+    "IMAGE_ROOTFS": "The location of the root filesystem while it is under construction (i.e. during do_rootfs).",
+    "IMAGE_ROOTFS_EXTRA_SPACE": "Defines additional free disk space created in the image in Kbytes. By default, this variable is set to '0'.",
+    "IMAGE_ROOTFS_SIZE": "Defines the size in Kbytes for the generated image.",
+    "IMAGE_TYPES": "Specifies the complete list of supported image types by default.",
+    "INCOMPATIBLE_LICENSE": "Specifies a space-separated list of license names (as they would appear in LICENSE) that should be excluded from the build. Wildcard is supported, such as '*GPL-3.0*'",
+    "INC_PR": "Helps define the recipe revision for recipes that share a common include file.",
+    "INHERIT": "Causes the named class to be inherited at this point during parsing. The variable is only valid in configuration files.",
+    "INHERIT_DISTRO": "Lists classes that will be inherited at the distribution level. It is unlikely that you want to edit this variable.",
+    "INHIBIT_DEFAULT_DEPS": "Prevents the default dependencies, namely the C compiler and standard C library (libc), from being added to DEPENDS.",
+    "INHIBIT_PACKAGE_STRIP": "If set to '1', causes the build to not strip binaries in resulting packages.",
+    "INITRAMFS_FSTYPES": "Defines the format for the output image of an initial RAM disk (initramfs), which is used during boot.",
+    "INITRD": "Indicates a list of filesystem images to concatenate and use as an initial RAM disk (initrd).",
+    "INITSCRIPT_NAME": "The filename of the initialization script as installed to ${sysconfdir}/init.d.",
+    "INITSCRIPT_PACKAGES": "A list of the packages that contain initscripts. This variable is used in recipes when using update-rc.d.bbclass. The variable is optional and defaults to the PN variable.",
+    "INITSCRIPT_PARAMS": "Specifies the options to pass to update-rc.d. The variable is mandatory and is used in recipes when using update-rc.d.bbclass.",
+    "INSANE_SKIP": "Specifies the QA checks to skip for a specific package within a recipe.",
+    "IPK_FEED_URIS": "List of ipkg feed records to put into generated image.",
+    "KARCH": "Defines the kernel architecture used when assembling the configuration. You define the KARCH variable in the BSP Descriptions.",
+    "KBRANCH": "A regular expression used by the build process to explicitly identify the kernel branch that is validated, patched and configured during a build.",
+    "KBRANCH_DEFAULT": "Defines the Linux kernel source repository's default branch used to build the Linux kernel. Unless you specify otherwise, the variable initializes to 'master'.",
+    "KERNEL_CLASSES": "A list of classes defining kernel image types that kernel class should inherit.",
+    "KERNEL_EXTRA_ARGS": "Specifies additional make command-line arguments the OpenEmbedded build system passes on when compiling the kernel.",
+    "KERNEL_FEATURES": "Includes additional metadata from the Yocto Project kernel Git repository. The metadata you add through this variable includes config fragments and features descriptions.",
+    "KERNEL_IMAGETYPE": "The type of kernel to build for a device, usually set by the machine configuration files and defaults to 'zImage'.",
+    "KERNEL_IMAGETYPES": "The list of types of kernel to build for a device, usually set by the machine configuration files and defaults to KERNEL_IMAGETYPE.",
+    "KERNEL_LOCALVERSION": "Appends a string to the name of the local version of the kernel image.",
+    "KERNEL_MODULE_AUTOLOAD": "Lists kernel modules that need to be auto-loaded during boot",
+    "KERNEL_MODULE_PROBECONF": "Lists kernel modules for which the build system expects to find module_conf_* values that specify configuration for each of the modules",
+    "KERNEL_PACKAGE_NAME": "Name prefix for kernel packages. Defaults to 'kernel'.",
+    "KERNEL_PATH": "The location of the kernel sources. This variable is set to the value of the STAGING_KERNEL_DIR within the module class (module.bbclass).",
+    "KERNEL_SRC": "The location of the kernel sources. This variable is set to the value of the STAGING_KERNEL_DIR within the module class (module.bbclass).",
+    "KFEATURE_DESCRIPTION": "Provides a short description of a configuration fragment. You use this variable in the .scc file that describes a configuration fragment file.",
+    "KMACHINE": "The machine as known by the kernel.",
+    "KTYPE": "Defines the kernel type to be used in assembling the configuration.",
+    "LAYERDEPENDS": "Lists the layers, separated by spaces, upon which this recipe depends. This variable is used in the conf/layer.conf file and must be suffixed with the name of the specific layer.",
+    "LAYERDIR": "When used inside the layer.conf configuration file, this variable provides the path of the current layer.",
+    "LAYERVERSION": "Optionally specifies the version of a layer as a single number. This variable is used in the conf/layer.conf file and must be suffixed with the name of the specific layer.",
+    "LEAD_SONAME": "Specifies the lead (or primary) compiled library file (.so) that the debian class applies its naming policy to given a recipe that packages multiple libraries.",
+    "LICENSE": "The list of source licenses for the recipe. Logical operators '&' or '|' and parentheses can be used.",
+    "LICENSE_PATH": "Path to additional licenses used during the build.",
+    "LIC_FILES_CHKSUM": "Checksums of the license text in the recipe source code.",
+    "LINUX_KERNEL_TYPE": "Defines the kernel type to be used in assembling the configuration.",
+    "LINUX_VERSION": "The Linux version from kernel.org on which the Linux kernel image being built using the OpenEmbedded build system is based. You define this variable in the kernel recipe.",
+    "LINUX_VERSION_EXTENSION": "A string extension compiled into the version string of the Linux kernel built with the OpenEmbedded build system. You define this variable in the kernel recipe.",
+    "LOCALE_UTF8_IS_DEFAULT": "If set, locale names are renamed such that those lacking an explicit encoding (e.g. en_US) will always be UTF-8, and non-UTF-8 encodings are renamed to, e.g., en_US.ISO-8859-1. Otherwise, the encoding is specified by glibc's SUPPORTED file. Not supported for precompiled locales.",
+    "LOG_DIR": "Specifies the directory to which the OpenEmbedded build system writes overall log files. The default directory is ${TMPDIR}/log",
+    "MACHINE": "Specifies the target device for which the image is built. You define MACHINE in the conf/local.conf file in the Build Directory.",
+    "MACHINEOVERRIDES": "Lists overrides specific to the current machine. By default, this list includes the value of MACHINE.",
+    "MACHINE_ESSENTIAL_EXTRA_RDEPENDS": "A list of required machine-specific packages to install as part of the image being built. Because this is a 'machine essential' variable, the list of packages are essential for the machine to boot.",
+    "MACHINE_ESSENTIAL_EXTRA_RRECOMMENDS": "A list of recommended machine-specific packages to install as part of the image being built. Because this is a 'machine essential' variable, the list of packages are essential for the machine to boot.",
+    "MACHINE_EXTRA_RDEPENDS": "A list of machine-specific packages to install as part of the image being built that are not essential for the machine to boot. However, the build process for more fully-featured images depends on the packages being present.",
+    "MACHINE_EXTRA_RRECOMMENDS": "A list of machine-specific packages to install as part of the image being built that are not essential for booting the machine. The image being built has no build dependencies on the packages in this list.",
+    "MACHINE_FEATURES": "Specifies the list of hardware features the MACHINE supports.",
+    "MACHINE_FEATURES_BACKFILL": "Features to be added to MACHINE_FEATURES if not also present in MACHINE_FEATURES_BACKFILL_CONSIDERED. This variable is set in the meta/conf/bitbake.conf file and is not intended to be user-configurable.",
+    "MACHINE_FEATURES_BACKFILL_CONSIDERED": "Features from MACHINE_FEATURES_BACKFILL that should not be backfilled (i.e. added to MACHINE_FEATURES) during the build.",
+    "MAINTAINER": "The email address of the distribution maintainer.",
+    "MIRRORS": "Specifies additional paths from which the OpenEmbedded build system gets source code.",
+    "MLPREFIX": "Specifies a prefix has been added to PN to create a special version of a recipe or package, such as a Multilib version.",
+    "MODULE_TARBALL_DEPLOY": "Controls creation of the modules-*.tgz file. Set this variable to '0' to disable creation of this file, which contains all of the kernel modules resulting from a kernel build.",
+    "MULTIMACH_TARGET_SYS": "Separates files for different machines such that you can build for multiple target machines using the same output directories.",
+    "NATIVELSBSTRING": "A string identifying the host distribution.",
+    "NO_RECOMMENDATIONS": "When set to '1', no recommended packages will be installed. Realize that some recommended packages might be required for certain system functionality, such as kernel-modules. It is up to the user to add packages to IMAGE_INSTALL as needed.",
+    "OEROOT": "The directory from which the top-level build environment setup script is sourced.",
+    "OE_BINCONFIG_EXTRA_MANGLE": "When a recipe inherits the binconfig.bbclass class, this variable specifies additional arguments passed to the 'sed' command.",
+    "OE_IMPORTS": "An internal variable used to tell the OpenEmbedded build system what Python modules to import for every Python function run by the system.",
+    "OE_TERMINAL": "Controls how the OpenEmbedded build system spawns interactive terminals on the host development system.",
+    "OLDEST_KERNEL": "Declares the oldest version of the Linux kernel that the produced binaries must support.",
+    "OVERRIDES": "BitBake uses OVERRIDES to control what variables are overridden after BitBake parses recipes and configuration files.",
+    "P": "The recipe name and version. P is comprised of ${PN}-${PV}.",
+    "PACKAGECONFIG": "This variable provides a means of enabling or disabling features of a recipe on a per-recipe basis.",
+    "PACKAGES": "The list of packages to be created from the recipe.",
+    "PACKAGES_DYNAMIC": "A promise that your recipe satisfies runtime dependencies for optional modules that are found in other recipes.",
+    "PACKAGE_ARCH": "The architecture of the resulting package or packages.",
+    "PACKAGE_ARCHS": "A list of architectures compatible with the given target in order of priority.",
+    "PACKAGE_BEFORE_PN": "Enables easily adding packages to PACKAGES before ${PN} so that the packages can pick up files that would normally be included in the default package.",
+    "PACKAGE_CLASSES": "This variable specifies the package manager to use when packaging data. It is set in the conf/local.conf file in the Build Directory.",
+    "PACKAGE_EXCLUDE": "Packages to exclude from the installation. If a listed package is required, an error is generated.",
+    "PACKAGE_EXTRA_ARCHS": "Specifies the list of architectures compatible with the device CPU. This variable is useful when you build for several different devices that use miscellaneous processors.",
+    "PACKAGE_INSTALL": "List of the packages to be installed into the image. The variable is generally not user-defined and uses IMAGE_INSTALL as part of the list.",
+    "PACKAGE_INSTALL_ATTEMPTONLY": "List of packages attempted to be installed. If a listed package fails to install, the build system does not generate an error. This variable is generally not user-defined.",
+    "PACKAGE_SNAP_LIB_SYMLINKS": "Rename library files based on their SONAME to avoid an extra layer of indirection through a symlink. Only suitable for a read-only rootfs where libraries are not upgraded in place.",
+    "PARALLEL_MAKE": "Specifies extra options that are passed to the make command during the compile tasks. This variable is usually in the form -j 4, where the number represents the maximum number of parallel threads make can run.",
+    "PARALLEL_MAKEINST": "Extra options passed to the make install command during the do_install task in order to specify parallel installation.",
+    "PATCHRESOLVE": "Enable or disable interactive patch resolution.",
+    "PATCHTOOL": "Specifies the utility used to apply patches for a recipe during do_patch.",
+    "PE": "The epoch of the recipe. The default value is '0'. The field is used to make upgrades possible when the versioning scheme changes in some backwards incompatible way.",
+    "PF": "Specifies the recipe or package name and includes all version and revision numbers. This variable is comprised of ${PN}-${EXTENDPE}${PV}-${PR}.",
+    "PIXBUF_PACKAGES": "When a recipe inherits the pixbufcache class, this variable identifies packages that contain the pixbuf loaders used with gdk-pixbuf.",
+    "PKGD": "Points to the destination directory for files to be packaged before they are split into individual packages.",
+    "PKGDATA_DIR": "Points to a shared, global-state directory that holds data generated during the packaging process.",
+    "PKGDEST": "Points to the parent directory for files to be packaged after they have been split into individual packages.",
+    "PKGDESTWORK": "Points to a temporary work area used by the do_package task to write output from the do_packagedata task.",
+    "PN": "PN refers to a recipe name in the context of a file used by the OpenEmbedded build system as input to create a package. It refers to a package name in the context of a file created or produced by the OpenEmbedded build system.",
+    "PR": "The revision of the recipe. The default value for this variable is 'r0'.",
+    "PREFERRED_PROVIDER": "If multiple recipes provide an item, this variable determines which recipe should be given preference.",
+    "PREFERRED_VERSION": "If there are multiple versions of recipes available, this variable determines which recipe should be given preference.",
+    "PREMIRRORS": "Specifies additional paths from which the OpenEmbedded build system gets source code.",
+    "PRIORITY": "Indicates the importance of a package.  The default value is 'optional'.  Other standard values are 'required', 'standard' and 'extra'.",
+    "PROVIDES": "A list of aliases that a recipe also provides. These aliases are useful for satisfying dependencies of other recipes during the build as specified by DEPENDS.",
+    "PRSERV_HOST": "The network based PR service host and port.",
+    "PV": "The version of the recipe. The version is normally extracted from the recipe filename.",
+    "PYPI_PACKAGE": "The python package name to use for fetching from pypi. Default is parsed from the recipe name, but can be overridden if upstream name is different than recipe name.",
+    "PYPI_PACKAGE_EXT": "The archive file extension to use for fetching from pypi. Default is tar.gz, but can be overridden if upstream uses a different compression scheme.",
+    "PYPI_SRC_URI": "The URI to use to fetch from pypi, default uses pythonhosted.org and is constructed from PYPI_PACKAGE, PYPI_PACKAGE_EXT and PV.",
+    "QA_EMPTY_DIRS": "A list of directories that are expected to be empty.",
+    "QA_EMPTY_DIRS_RECOMMENDATION": "This specifies a recommendation for a directory why it must be empty, which will be included in the error message if the directory is not empty.",
+    "QMAKE_PROFILES": "Specifies your own subset of .pro files to be built for use with qmake.",
+    "RCONFLICTS": "The list of packages that conflict with another package. Note that the package will not be installed if the conflicting packages are not first removed.",
+    "RDEPENDS": "Lists a package's runtime dependencies (i.e. other packages) that must be installed for the package to be built. They must be the names of other packages as listed in the PACKAGES variable, not recipe names (PN).",
+    "REQUIRED_COMBINED_FEATURES": "When a recipe inherits the features_check class, all items in this variable must be included in COMBINED_FEATURES.",
+    "REQUIRED_DISTRO_FEATURES": "When a recipe inherits the features_check class, all items in this variable must be included in DISTRO_FEATURES.",
+    "REQUIRED_MACHINE_FEATURES": "When a recipe inherits the features_check class, all items in this variable must be included in MACHINE_FEATURES.",
+    "RM_WORK_EXCLUDE": "With rm_work enabled, this variable specifies a list of packages whose work directories should not be removed.",
+    "ROOTFS": "Indicates a filesystem image to include as the root filesystem.",
+    "ROOTFS_POSTPROCESS_COMMAND": "Added by classes to run post processing commands once the OpenEmbedded build system has created the root filesystem.",
+    "RPROVIDES": "A list of package name aliases that a package also provides. These aliases are useful for satisfying runtime dependencies of other packages both during the build and on the target.",
+    "RRECOMMENDS": "A list of packages that extends the usability of a package being built. The package being built does not depend on this list of packages in order to successfully build, but needs them for the extended usability.",
+    "RREPLACES": "A list of packages replaced by a package. The package manager uses this variable to determine which package should be installed to replace other package(s) during an upgrade.",
+    "RSUGGESTS": "A list of additional packages that you can suggest for installation by the package manager at the time a package is installed. Not all package managers support this functionality.",
+    "S": "The location in the Build Directory where unpacked package source code resides.",
+    "SANITY_TESTED_DISTROS": "A list of the host distribution identifiers that the build system has been tested against.",
+    "SDKIMAGE_FEATURES": "Equivalent to IMAGE_FEATURES. However, this variable applies to the SDK generated from an image using the command 'bitbake -c populate_sdk imagename'.",
+    "SDKMACHINE": "Specifies the architecture (i.e. i686 or x86_64) for which to build SDK and ADT items.",
+    "SDK_ARCH": "The target architecture for the SDK.",
+    "SDK_DEPLOY": "The directory set up and used by the populate_sdk_base to which the SDK is deployed.",
+    "SDK_DIR": "The parent directory used by the OpenEmbedded build system when creating SDK output.",
+    "SDK_NAME": "The base name for SDK output files.",
+    "SDK_OUTPUT": "The location used by the OpenEmbedded build system when creating SDK output.",
+    "SECTION": "The section in which packages should be categorized. Package management utilities can make use of this variable.",
+    "SELECTED_OPTIMIZATION": "The variable takes the value of FULL_OPTIMIZATION unless DEBUG_BUILD = '1'. In this case, the value of DEBUG_OPTIMIZATION is used.",
+    "SERIAL_CONSOLES": "Defines the serial consoles (TTYs) to enable using getty.",
+    "SERIAL_CONSOLES_CHECK": "Similar to SERIAL_CONSOLES except the device is checked for existence before attempting to enable it. Supported only by SysVinit.",
+    "SIGGEN_EXCLUDERECIPES_ABISAFE": "A list of recipes that are completely stable and will never change.",
+    "SIGGEN_EXCLUDE_SAFE_RECIPE_DEPS": "A list of recipe dependencies that should not be used to determine signatures of tasks from one recipe when they depend on tasks from another recipe.",
+    "SITEINFO_BITS": "Specifies the number of bits for the target system CPU.",
+    "SITEINFO_ENDIANNESS": "Specifies the endian byte order of the target system. The value should be either 'le' for 'little-endian' or 'be' for 'big-endian'.",
+    "SKIP_RECIPE": "Lists recipes you do not want the OpenEmbedded build system to build.",
+    "SOC_FAMILY": "Groups together machines based upon the same family of SOC (System On Chip). You typically set this variable in a common .inc file that you include in the configuration files of all the machines.",
+    "SOLIBS": "Defines the suffix for shared libraries used on the target platform.",
+    "SOLIBSDEV": "Defines the suffix for the development symbolic link (symlink) for shared libraries on the target platform.",
+    "SOURCE_MIRROR_FETCH": "Switch marking build as source fetcher. Used to skip COMPATIBLE_* checking.",
+    "SOURCE_MIRROR_URL": "URL to source mirror that will be used before fetching from original SRC_URI.",
+    "SPECIAL_PKGSUFFIX": "A list of prefixes for PN used by the OpenEmbedded build system to create variants of recipes or packages. The list specifies the prefixes to strip off during certain circumstances such as the generation of the BPN variable.",
     "SRCDATE": "The date of the source code used to build the package. This variable applies only if the source was fetched from a Source Code Manager (SCM).",
-    "SRCREV": "The revision of the source code used to build the package. This variable applies only when using Subversion, Git, Mercurial and Bazaar. If you want to build a fixed revision and you want to avoid performing a query on the remote repository every time BitBake parses your recipe, you should specify a SRCREV that is a full revision identifier and not just a tag.",
-    "SRCREV_FORMAT": "Helps construct valid SRCREV values when multiple source controlled URLs are used in SRC_URI.\nThe system needs help constructing these values under these circumstances. Each component in the SRC_URI is assigned a name and these are referenced in the SRCREV_FORMAT variable. Consider an example with URLs named \u201cmachine\u201d and \u201cmeta\u201d. In this case, SRCREV_FORMAT could look like \u201cmachine_meta\u201d and those names would have the SCM versions substituted into each position. Only one AUTOINC placeholder is added and if needed. And, this placeholder is placed at the start of the returned string.",
-    "SRC_URI": "The list of source files \u2014 local or remote. This variable tells BitBake which bits to pull for the build and how to pull them. For example, if the recipe or append file needs to fetch a single tarball from the Internet, the recipe or append file uses a SRC_URI entry that specifies that tarball. On the other hand, if the recipe or append file needs to fetch a tarball, apply two patches, and include a custom file, the recipe or append file needs an SRC_URI variable that specifies all those sources.\nThe following list explains the available URI protocols. URI protocols are highly dependent on particular BitBake Fetcher submodules. Depending on the fetcher BitBake uses, various URL parameters are employed. For specifics on the supported Fetchers, see the Fetchers section.\naz://: Fetches files from an Azure Storage account using HTTPS.\nbzr://: Fetches files from a Bazaar revision control repository.\nccrc://: Fetches files from a ClearCase repository.\ncvs://: Fetches files from a CVS revision control repository.\nfile://: Fetches files, which are usually files shipped with the Metadata, from the local machine. The path is relative to the FILESPATH variable. Thus, the build system searches, in order, from the following directories, which are assumed to be a subdirectories of the directory in which the recipe file (.bb) or append file (.bbappend) resides:\n${BPN}: the base recipe name without any special suffix or version numbers.\n${BP} - ${BPN}-${PV}: the base recipe name and version but without any special package name suffix.\nfiles: files within a directory, which is named files and is also alongside the recipe or append file.\nftp://: Fetches files from the Internet using FTP.\ngit://: Fetches files from a Git revision control repository.\ngitsm://: Fetches submodules from a Git revision control repository.\nhg://: Fetches files from a Mercurial (hg) revision control repository.\nhttp://: Fetches files from the Internet using HTTP.\nhttps://: Fetches files from the Internet using HTTPS.\nnpm://: Fetches JavaScript modules from a registry.\nosc://: Fetches files from an OSC (OpenSUSE Build service) revision control repository.\np4://: Fetches files from a Perforce (p4) revision control repository.\nrepo://: Fetches files from a repo (Git) repository.\nssh://: Fetches files from a secure shell.\nsvn://: Fetches files from a Subversion (svn) revision control repository.\nHere are some additional options worth mentioning:\ndownloadfilename: Specifies the filename used when storing the downloaded file.\nname: Specifies a name to be used for association with SRC_URI checksums or SRCREV when you have more than one file or git repository specified in SRC_URI. For example:\nsubdir: Places the file (or extracts its contents) into the specified subdirectory. This option is useful for unusual tarballs or other archives that do not have their files already in a subdirectory within the archive.\nsubpath: Limits the checkout to a specific subpath of the tree when using the Git fetcher is used.\nunpack: Controls whether or not to unpack the file if it is an archive. The default action is to unpack the file.",
+    "SRCPV": "Returns the version string of the current package. This string is used to help define the value of PV.",
+    "SRCREV": "The revision of the source code used to build the package. This variable applies to Subversion, Git, Mercurial and Bazaar only.",
+    "SRC_URI": "The list of source files - local or remote. This variable tells the OpenEmbedded build system what bits to pull in for the build and how to pull them in.",
+    "SRC_URI_OVERRIDES_PACKAGE_ARCH": "By default, the OpenEmbedded build system automatically detects whether SRC_URI contains files that are machine-specific. If so, the build system automatically changes PACKAGE_ARCH. Setting this variable to '0' disables this behavior.",
+    "SSTATE_DIR": "The directory for the shared state cache.",
+    "SSTATE_MIRRORS": "Configures the OpenEmbedded build system to search other mirror locations for prebuilt cache data objects before building out the data. You can specify a filesystem directory or a remote URL such as HTTP or FTP.",
+    "STAGING_KERNEL_DIR": "The directory with kernel headers that are required to build out-of-tree modules.",
     "STAMP": "Specifies the base path used to create recipe stamp files. The path to an actual stamp file is constructed by evaluating this string and then appending additional information.",
-    "STAMPCLEAN": "Specifies the base path used to create recipe stamp files. Unlike the STAMP variable, STAMPCLEAN can contain wildcards to match the range of files a clean operation should remove. BitBake uses a clean operation to remove any other stamps it should be removing when creating a new stamp.",
-    "SUMMARY": "A short summary for the recipe, which is 72 characters or less.",
-    "SVNDIR": "The directory in which files checked out of a Subversion system are stored.",
-    "T": "Points to a directory were BitBake places temporary files, which consist mostly of task logs and scripts, when building a particular recipe.",
-    "TOPDIR": "Points to the build directory. BitBake automatically sets this variable."
+    "STAMPS_DIR": "Specifies the base directory in which the OpenEmbedded build system places stamps.",
+    "SUMMARY": "The short (80 characters or less) summary of the binary package for packaging systems such as opkg, rpm or dpkg. By default, SUMMARY is used to define the DESCRIPTION variable if DESCRIPTION is not set in the recipe.",
+    "SYSLINUX_DEFAULT_CONSOLE": "Specifies the kernel boot default console.",
+    "SYSLINUX_OPTS": "Lists additional options to add to the syslinux file.",
+    "SYSLINUX_SERIAL": "Specifies the alternate serial port or turns it off.",
+    "SYSLINUX_SERIAL_TTY": "Specifies the alternate console=tty... kernel boot argument.",
+    "SYSLINUX_SPLASH": "An .LSS file used as the background for the VGA boot menu when you are using the boot menu.",
+    "SYSROOT_PREPROCESS_FUNCS": "A list of functions to execute after files are staged into the sysroot. These functions are usually used to apply additional processing on the staged files, or to stage additional files.",
+    "SYSTEMD_AUTO_ENABLE": "For recipes that inherit the systemd class, this variable specifies whether the service you have specified in SYSTEMD_SERVICE should be started automatically or not.",
+    "SYSTEMD_PACKAGES": "For recipes that inherit the systemd class, this variable locates the systemd unit files when they are not found in the main recipe's package.",
+    "SYSTEMD_SERVICE": "For recipes that inherit the systemd class, this variable specifies the systemd service name for a package.",
+    "SYSVINIT_ENABLED_GETTYS": "Specifies which virtual terminals should be running a getty, the default is '1'.",
+    "T": "This variable points to a directory were BitBake places temporary files, which consist mostly of task logs and scripts, when building a particular recipe.",
+    "TARGET_ARCH": "The architecture of the device being built. The OpenEmbedded build system supports the following architectures: arm, mips, ppc, x86, x86-64.",
+    "TARGET_CFLAGS": "Flags passed to the C compiler for the target system. This variable evaluates to the same as CFLAGS.",
+    "TARGET_FPU": "Specifies the method for handling FPU code. For FPU-less targets, which include most ARM CPUs, the variable must be set to 'soft'. If not, the kernel emulation gets used, which results in a performance penalty.",
+    "TARGET_OS": "Specifies the target's operating system.",
+    "TARGET_PREFIX": "The prefix for the cross-compile toolchain (e.g. arm-linux-).",
+    "TARGET_SYS": "The target system is comprised of TARGET_ARCH,TARGET_VENDOR and TARGET_OS.",
+    "TCLIBC": "Specifies C library (libc) variant to use during the build process. You can select 'baremetal', 'glibc', 'musl' or 'newlib'.",
+    "TCMODE": "Enables an external toolchain (where provided by an additional layer) if set to a value other than 'default'.",
+    "TESTIMAGE_AUTO": "Enables test booting of virtual machine images under the QEMU emulator after any root filesystems are created and runs tests against those images each time an image is built.",
+    "TEST_POWERCONTROL_CMD": "For automated hardware testing, specifies the command to use to control the power of the target machine under test",
+    "TEST_POWERCONTROL_EXTRA_ARGS": "For automated hardware testing, specifies additional arguments to pass through to the command specified in TEST_POWERCONTROL_CMD",
+    "TEST_QEMUBOOT_TIMEOUT": "The time in seconds allowed for an image to boot before automated runtime tests begin to run against an image.",
+    "TEST_SERIALCONTROL_CMD": "For automated hardware testing, specifies the command to use to connect to the serial console of the target machine under test",
+    "TEST_SERIALCONTROL_EXTRA_ARGS": "For automated hardware testing, specifies additional arguments to pass through to the command specified in TEST_SERIALCONTROL_CMD",
+    "TEST_SUITES": "An ordered list of tests (modules) to run against an image when performing automated runtime testing.",
+    "TEST_TARGET": "For automated runtime testing, specifies the method of deploying the image and running tests on the target machine",
+    "THISDIR": "The directory in which the file BitBake is currently parsing is located.",
+    "TIME": "The time the build was started using HMS format.",
+    "TMPDIR": "The temporary directory the OpenEmbedded build system uses when it does its work building images. By default, the TMPDIR variable is named tmp within the Build Directory.",
+    "TOOLCHAIN_HOST_TASK": "This variable lists packages the OpenEmbedded build system uses when building an SDK, which contains a cross-development environment.",
+    "TOOLCHAIN_TARGET_TASK": "This variable lists packages the OpenEmbedded build system uses when it creates the target part of an SDK, which includes libraries and headers.",
+    "TOPDIR": "The Build Directory. BitBake automatically sets this variable. The OpenEmbedded build system uses the Build Directory when building images.",
+    "TRANSLATED_TARGET_ARCH": "A sanitized version of TARGET_ARCH. This variable is used where the architecture is needed in a value where underscores are not allowed.",
+    "TUNECONFLICTS": "List of conflicting features for a given feature.",
+    "TUNEVALID": "Descriptions, stored as flags, of valid tuning features.",
+    "TUNE_PKGARCH": "The package architecture understood by the packaging system to define the architecture, ABI, and tuning of output packages.",
+    "UBOOT_CONFIG": "Configures the UBOOT_MACHINE and can also define IMAGE_FSTYPES for individual cases.",
+    "UBOOT_ENTRYPOINT": "Specifies the entry point for the U-Boot image.",
+    "UBOOT_LOADADDRESS": "Specifies the load address for the U-Boot image.",
+    "UBOOT_LOCALVERSION": "Appends a string to the name of the local version of the U-Boot image.",
+    "UBOOT_MACHINE": "Specifies the value passed on the make command line when building a U-Boot image.",
+    "UBOOT_MAKE_TARGET": "Specifies the target called in the Makefile.",
+    "UBOOT_SUFFIX": "Points to the generated U-Boot extension.",
+    "UBOOT_TARGET": "Specifies the target used for building U-Boot.",
+    "USERADDEXTENSION": "When set to 'useradd-staticids', causes the OpenEmbedded build system to base all user and group additions on files listed in USERADD_UID_TABLES and USERADD_GID_TABLES.",
+    "USERADD_ERROR_DYNAMIC": "If set to 'error', forces the OpenEmbedded build system to produce an error if the user identification (uid) and group identification (gid) values are not defined in any of the files listed in USERADD_UID_TABLES and USERADD_GID_TABLES. If set to 'warn', a warning will be issued instead.",
+    "USERADD_GID_TABLES": "Specifies a password file to use for obtaining static group identification (gid) values when the OpenEmbedded build system adds a group to the system during package installation.",
+    "USERADD_PACKAGES": "When a recipe inherits the useradd class, this variable specifies the individual packages within the recipe that require users and/or groups to be added.",
+    "USERADD_PARAM": "When a recipe inherits the useradd class, this variable specifies for a package what parameters should be passed to the useradd command if you wish to add a user to the system when the package is installed.",
+    "USERADD_UID_TABLES": "Specifies a password file to use for obtaining static user identification (uid) values when the OpenEmbedded build system adds a user to the system during package installation.",
+    "USER_CLASSES": "List of additional classes to use when building images that enable extra features.",
+    "USE_DEVFS": "When building images, specifies to populate or not /dev. This variable defaults to '1' (leave directory empty, surely because devtmpfs do the job). Set it to '0' to use makedevs (or consider using a custom file with IMAGE_DEVICE_TABLES).",
+    "WARN_QA": "Specifies the quality assurance checks whose failures are reported as warnings by the OpenEmbedded build system.",
+    "WORKDIR": "The pathname of the working directory in which the OpenEmbedded build system builds a recipe. This directory is located within the TMPDIR directory structure and changes as different packages are built.",
+    "do_bootimg": "Creates a bootable live image",
+    "do_build": "Default task for a recipe - depends on all other normal tasks required to 'build' a recipe",
+    "do_bundle_initramfs": "Combines an initial ramdisk image and kernel together to form a single image",
+    "do_checkuri": "Validates the SRC_URI value",
+    "do_clean": "Removes all output files for a target",
+    "do_cleanall": "Removes all output files, shared state cache, and downloaded source files for a target",
+    "do_cleansstate": "Removes all output files and shared state cache for a target",
+    "do_compile": "Compiles the source in the compilation directory",
+    "do_compile_kernelmodules": "Compiles loadable modules for the Linux kernel",
+    "do_compile_ptest_base": "Compiles the runtime test suite included in the software being built",
+    "do_configure": "Configures the source by enabling and disabling any build-time and configuration options for the software being built",
+    "do_configure_ptest_base": "Configures the runtime test suite included in the software being built",
+    "do_deploy": "Writes deployable output files to the deploy directory",
+    "do_devshell": "Starts a shell with the environment set up for development/debugging",
+    "do_diffconfig": "Compares the old and new config files after running do_menuconfig for the kernel",
+    "do_fetch": "Fetches the source code",
+    "do_install": "Copies files from the compilation directory to a holding area",
+    "do_install_ptest_base": "Copies the runtime test suite files from the compilation directory to a holding area",
+    "do_kernel_checkout": "Checks out source/meta branches for a linux-yocto style kernel",
+    "do_kernel_configcheck": "Validates the kernel configuration for a linux-yocto style kernel",
+    "do_kernel_configme": "Assembles the kernel configuration for a linux-yocto style kernel",
+    "do_kernel_link_images": "Creates a symbolic link in arch/$arch/boot for vmlinux and vmlinuz kernel images",
+    "do_listtasks": "Lists all defined tasks for a target",
+    "do_menuconfig": "Runs 'make menuconfig' for the kernel",
+    "do_package": "Analyzes the content of the holding area and splits it into subsets based on available packages and files",
+    "do_package_index": "Creates or updates the index in the Package Feed area",
+    "do_package_qa": "Runs QA checks on packaged files",
+    "do_package_write_deb": "Creates the actual DEB packages and places them in the Package Feed area",
+    "do_package_write_ipk": "Creates the actual IPK packages and places them in the Package Feed area",
+    "do_package_write_rpm": "Creates the actual RPM packages and places them in the Package Feed area",
+    "do_package_write_tar": "Creates tar archives for packages and places them in the Package Feed area",
+    "do_packagedata": "Creates package metadata used by the build system to generate the final packages",
+    "do_patch": "Locates patch files and applies them to the source code",
+    "do_populate_lic": "Writes license information for the recipe that is collected later when the image is constructed",
+    "do_populate_sdk": "Creates the file and directory structure for an installable SDK",
+    "do_populate_sysroot": "Copies a subset of files installed by do_install into the sysroot in order to make them available to other recipes",
+    "do_pydevshell": "Starts an interactive Python shell for development/debugging",
+    "do_rm_work": "Removes work files after the build system has finished with them",
+    "do_rm_work_all": "Top-level task for removing work files after the build system has finished with them",
+    "do_rootfs": "Creates the root filesystem (file and directory structure) for an image",
+    "do_savedefconfig": "Creates a minimal Linux kernel configuration file",
+    "do_sizecheck": "Checks the size of the kernel image against KERNEL_IMAGE_MAXSIZE (if set)",
+    "do_spdx": "A build stage that takes the source code and scans it on a remote FOSSOLOGY server in order to produce an SPDX document",
+    "do_strip": "Strips unneeded sections out of the Linux kernel image",
+    "do_testimage": "Boots an image and performs runtime tests within the image",
+    "do_testimage_auto": "Boots an image and performs runtime tests within the image immediately after it has been built",
+    "do_testsdk": "Installs an SDK and performs runtime tests on the tools installed by it",
+    "do_uboot_mkimage": "Creates a uImage file from the kernel for the U-Boot bootloader",
+    "do_unpack": "Unpacks the source code into a working directory",
+    "do_validate_branches": "Ensures that the source/meta branches are on the locations specified by their SRCREV values for a linux-yocto style kernel"
 }
```

### Comparing `bitbake-language-server-0.0.1/src/bitbake_language_server/server.py` & `bitbake-language-server-0.0.2/src/bitbake_language_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,17 @@
 
 
 def get_document(
     method: Literal["builtin", "cache", "web"] = "builtin"
 ) -> dict[str, str]:
     r"""Get document. ``builtin`` will use builtin bitbake.json. ``cache``
     will generate a cache from
-    `<https://www.sublimetext.com/docs/scope_naming.html>`_. ``web`` is same as
-    ``cache`` except it doesn't generate cache. We use ``builtin`` as default.
-    If you want to get the latest result from
-    `<https://www.sublimetext.com/docs/scope_naming.html>`_, you need to
-    install `beautifulsoup4 <https://pypi.org/project/beautifulsoup4>` by
-    ``pip install 'bitbake-language-server[web]'``.
+    `<https://raw.githubusercontent.com/openembedded/openembedded-core/master/meta/conf/documentation.conf>`_.
+    ``web`` is same as ``cache`` except it doesn't generate cache. We use
+    ``builtin`` as default.
 
     :param method:
     :type method: Literal["builtin", "cache", "web"]
     :rtype: dict[str, str]
     """
     if method == "builtin":
         file = os.path.join(
@@ -65,15 +62,15 @@
         from .api import init_document
 
         document = init_document()
     return document
 
 
 class BitbakeLanguageServer(LanguageServer):
-    r"""Sublime syntax language server."""
+    r"""Bitbake language server."""
 
     def __init__(self, *args: Any) -> None:
         r"""Init.
 
         :param args:
         :type args: Any
         :rtype: None
```

### Comparing `bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/PKG-INFO` & `bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -25,15 +25,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: web
 License-File: LICENSE
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/bitbake-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/bitbake-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/bitbake-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/bitbake-language-server/actions)
```

### Comparing `bitbake-language-server-0.0.1/src/bitbake_language_server.egg-info/SOURCES.txt` & `bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 .github/workflows/main.yml
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/api/bitbake-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
+docs/resources/requirements.md
 requirements/dev.txt
-requirements/web.txt
 scripts/generate-api.md.pl
+scripts/generate-requirements.md.pl
 src/bitbake_language_server/__init__.py
 src/bitbake_language_server/__main__.py
 src/bitbake_language_server/_version.py
 src/bitbake_language_server/api.py
 src/bitbake_language_server/py.typed
 src/bitbake_language_server/server.py
 src/bitbake_language_server.egg-info/PKG-INFO
```

