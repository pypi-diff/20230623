# Comparing `tmp/bitbake-language-server-0.0.2.tar.gz` & `tmp/bitbake-language-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbake-language-server-0.0.2.tar", last modified: Fri Jun 23 07:38:37 2023, max compression
+gzip compressed data, was "bitbake-language-server-0.0.3.tar", last modified: Fri Jun 23 09:07:51 2023, max compression
```

## Comparing `bitbake-language-server-0.0.2.tar` & `bitbake-language-server-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/api/bitbake-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/bitbake_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.686694 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    51596 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/bitbake.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/src/bitbake_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 07:38:37.000000 bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:38:37.690694 bitbake-language-server-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 07:38:25.000000 bitbake-language-server-0.0.2/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/api/bitbake-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements/web.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    51606 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/bitbake.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/tests/server_test.py
```

### Comparing `bitbake-language-server-0.0.2/.github/workflows/main.yml` & `bitbake-language-server-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/.gitignore` & `bitbake-language-server-0.0.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+pyshtables.py
 /result
 _version.py
 _metainfo.py
 
 # create by https://github.com/iamcco/coc-gitignore (Sat Jun 17 2023 19:59:16 GMT+0800 (China Standard Time))
 # pydev.gitignore:
 .pydevproject
```

### Comparing `bitbake-language-server-0.0.2/.pre-commit-config.yaml` & `bitbake-language-server-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/LICENSE` & `bitbake-language-server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/PKG-INFO` & `bitbake-language-server-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: web
 License-File: LICENSE
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/bitbake-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/bitbake-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/bitbake-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/bitbake-language-server/actions)
```

### Comparing `bitbake-language-server-0.0.2/README.md` & `bitbake-language-server-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/docs/conf.py` & `bitbake-language-server-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/docs/resources/configure.md` & `bitbake-language-server-0.0.3/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/docs/resources/install.md` & `bitbake-language-server-0.0.3/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/flake.nix` & `bitbake-language-server-0.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/pyproject.toml` & `bitbake-language-server-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
+
+[tool.setuptools.dynamic.optional-dependencies.web]
+file = "requirements/web.txt"
 # end: scripts/update-pyproject.toml.pl
 
 [tool.setuptools_scm]
 write_to = "src/bitbake_language_server/_version.py"
 
 [tool.setuptools-generate]
 write-to = "src/bitbake_language_server/_metainfo.py"
```

### Comparing `bitbake-language-server-0.0.2/src/bitbake_language_server/__main__.py` & `bitbake-language-server-0.0.3/src/bitbake_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/src/bitbake_language_server/assets/json/bitbake.json` & `bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/bitbake.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949494949494949%*

 * *Differences: {"'CLASSOVERRIDE'": "'An internal variable specifying the special class override that should "*

 * *                    'currently apply (e.g. "class-target", "class-native", and so forth).\'',*

 * * "'INHIBIT_PACKAGE_STRIP'": '\'If set to "1", causes the build to not strip binaries in resulting '*

 * *                            "packages.'",*

 * * "'MODULE_TARBALL_DEPLOY'": "'Controls creation of the modules-*.tgz file. Set this variable to "*

 * *                            '"0" to disable creation of this file, which contains a […]*

```diff
@@ -37,15 +37,15 @@
     "BUILDDIR": "Points to the location of the Build Directory.",
     "BUILDSTATS_BASE": "Points to the location of the directory that holds build statistics when you use and enable the buildstats class.",
     "BUILD_ARCH": "The name of the building architecture (e.g. i686).",
     "BUILD_OS": "The operating system (in lower case) of the building architecture (e.g. linux).",
     "BUSYBOX_SPLIT_SUID": "For the BusyBox recipe, specifies whether to split the output executable file into two parts: one for features that require setuid root, and one for the remaining features.",
     "CACHE": "The directory holding the cache of the metadata.",
     "CFLAGS": "Flags passed to the C compiler for the target system. This variable evaluates to the same as TARGET_CFLAGS.",
-    "CLASSOVERRIDE": "An internal variable specifying the special class override that should currently apply (e.g. 'class-target', 'class-native', and so forth).",
+    "CLASSOVERRIDE": "An internal variable specifying the special class override that should currently apply (e.g. \"class-target\", \"class-native\", and so forth).",
     "CLEANBROKEN": "Specifies if 'make clean' does not work for a recipe (and therefore the build system should not try to use it during do_configure)",
     "COMBINED_FEATURES": "A set of features common between MACHINE_FEATURES and DISTRO_FEATURES.",
     "COMMON_LICENSE_DIR": "Points to meta/files/common-licenses in the Source Directory, which is where generic license files reside.",
     "COMPATIBLE_HOST": "A regular expression that resolves to one or more hosts (when the recipe is native) or one or more targets (when the recipe is non-native) with which a recipe is compatible.",
     "COMPATIBLE_MACHINE": "A regular expression that resolves to one or more target machines with which a recipe is compatible.",
     "COMPLEMENTARY_GLOB": "Defines wildcards to match when installing a list of complementary packages for all the packages installed in an image.",
     "CONFFILES": "Identifies editable or configurable files that are part of a package.",
@@ -141,15 +141,15 @@
     "IMAGE_ROOTFS_SIZE": "Defines the size in Kbytes for the generated image.",
     "IMAGE_TYPES": "Specifies the complete list of supported image types by default.",
     "INCOMPATIBLE_LICENSE": "Specifies a space-separated list of license names (as they would appear in LICENSE) that should be excluded from the build. Wildcard is supported, such as '*GPL-3.0*'",
     "INC_PR": "Helps define the recipe revision for recipes that share a common include file.",
     "INHERIT": "Causes the named class to be inherited at this point during parsing. The variable is only valid in configuration files.",
     "INHERIT_DISTRO": "Lists classes that will be inherited at the distribution level. It is unlikely that you want to edit this variable.",
     "INHIBIT_DEFAULT_DEPS": "Prevents the default dependencies, namely the C compiler and standard C library (libc), from being added to DEPENDS.",
-    "INHIBIT_PACKAGE_STRIP": "If set to '1', causes the build to not strip binaries in resulting packages.",
+    "INHIBIT_PACKAGE_STRIP": "If set to \"1\", causes the build to not strip binaries in resulting packages.",
     "INITRAMFS_FSTYPES": "Defines the format for the output image of an initial RAM disk (initramfs), which is used during boot.",
     "INITRD": "Indicates a list of filesystem images to concatenate and use as an initial RAM disk (initrd).",
     "INITSCRIPT_NAME": "The filename of the initialization script as installed to ${sysconfdir}/init.d.",
     "INITSCRIPT_PACKAGES": "A list of the packages that contain initscripts. This variable is used in recipes when using update-rc.d.bbclass. The variable is optional and defaults to the PN variable.",
     "INITSCRIPT_PARAMS": "Specifies the options to pass to update-rc.d. The variable is mandatory and is used in recipes when using update-rc.d.bbclass.",
     "INSANE_SKIP": "Specifies the QA checks to skip for a specific package within a recipe.",
     "IPK_FEED_URIS": "List of ipkg feed records to put into generated image.",
@@ -190,20 +190,20 @@
     "MACHINE_EXTRA_RRECOMMENDS": "A list of machine-specific packages to install as part of the image being built that are not essential for booting the machine. The image being built has no build dependencies on the packages in this list.",
     "MACHINE_FEATURES": "Specifies the list of hardware features the MACHINE supports.",
     "MACHINE_FEATURES_BACKFILL": "Features to be added to MACHINE_FEATURES if not also present in MACHINE_FEATURES_BACKFILL_CONSIDERED. This variable is set in the meta/conf/bitbake.conf file and is not intended to be user-configurable.",
     "MACHINE_FEATURES_BACKFILL_CONSIDERED": "Features from MACHINE_FEATURES_BACKFILL that should not be backfilled (i.e. added to MACHINE_FEATURES) during the build.",
     "MAINTAINER": "The email address of the distribution maintainer.",
     "MIRRORS": "Specifies additional paths from which the OpenEmbedded build system gets source code.",
     "MLPREFIX": "Specifies a prefix has been added to PN to create a special version of a recipe or package, such as a Multilib version.",
-    "MODULE_TARBALL_DEPLOY": "Controls creation of the modules-*.tgz file. Set this variable to '0' to disable creation of this file, which contains all of the kernel modules resulting from a kernel build.",
+    "MODULE_TARBALL_DEPLOY": "Controls creation of the modules-*.tgz file. Set this variable to \"0\" to disable creation of this file, which contains all of the kernel modules resulting from a kernel build.",
     "MULTIMACH_TARGET_SYS": "Separates files for different machines such that you can build for multiple target machines using the same output directories.",
     "NATIVELSBSTRING": "A string identifying the host distribution.",
     "NO_RECOMMENDATIONS": "When set to '1', no recommended packages will be installed. Realize that some recommended packages might be required for certain system functionality, such as kernel-modules. It is up to the user to add packages to IMAGE_INSTALL as needed.",
     "OEROOT": "The directory from which the top-level build environment setup script is sourced.",
-    "OE_BINCONFIG_EXTRA_MANGLE": "When a recipe inherits the binconfig.bbclass class, this variable specifies additional arguments passed to the 'sed' command.",
+    "OE_BINCONFIG_EXTRA_MANGLE": "When a recipe inherits the binconfig.bbclass class, this variable specifies additional arguments passed to the \"sed\" command.",
     "OE_IMPORTS": "An internal variable used to tell the OpenEmbedded build system what Python modules to import for every Python function run by the system.",
     "OE_TERMINAL": "Controls how the OpenEmbedded build system spawns interactive terminals on the host development system.",
     "OLDEST_KERNEL": "Declares the oldest version of the Linux kernel that the produced binaries must support.",
     "OVERRIDES": "BitBake uses OVERRIDES to control what variables are overridden after BitBake parses recipes and configuration files.",
     "P": "The recipe name and version. P is comprised of ${PN}-${PV}.",
     "PACKAGECONFIG": "This variable provides a means of enabling or disabling features of a recipe on a per-recipe basis.",
     "PACKAGES": "The list of packages to be created from the recipe.",
```

### Comparing `bitbake-language-server-0.0.2/src/bitbake_language_server/server.py` & `bitbake-language-server-0.0.3/src/bitbake_language_server/server.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/PKG-INFO` & `bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: web
 License-File: LICENSE
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/bitbake-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/bitbake-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/bitbake-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/bitbake-language-server/actions)
```

### Comparing `bitbake-language-server-0.0.2/src/bitbake_language_server.egg-info/SOURCES.txt` & `bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/index.md
 docs/requirements.txt
 docs/api/bitbake-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
+requirements/web.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
 src/bitbake_language_server/__init__.py
 src/bitbake_language_server/__main__.py
 src/bitbake_language_server/_version.py
 src/bitbake_language_server/api.py
 src/bitbake_language_server/py.typed
```

