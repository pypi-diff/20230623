# Comparing `tmp/google_play_developer_api-0.2.0.tar.gz` & `tmp/google_play_developer_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.2.0.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.3.0.tar", max compression
```

## Comparing `google_play_developer_api-0.2.0.tar` & `google_play_developer_api-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/LICENSE
--rw-r--r--   0        0        0      829 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/README.md
--rw-r--r--   0        0        0       71 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0      381 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/google_play_developer_api/example.py
--rw-r--r--   0        0        0     2597 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      420 2023-06-20 03:03:49.762734 google_play_developer_api-0.2.0/tests/test_app.py
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 google_play_developer_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      858 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/README.md
+-rw-r--r--   0        0        0       78 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0     7744 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/google_play_developer_api/reporting.py
+-rw-r--r--   0        0        0     2634 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/tests/test_reporting_apis.py
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 google_play_developer_api-0.3.0/PKG-INFO
```

### Comparing `google_play_developer_api-0.2.0/LICENSE` & `google_play_developer_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.2.0/README.md` & `google_play_developer_api-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,9 +5,8 @@
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
 Wrapper for APIs
 
 ## Features
 
-* Something
-* Something else
+* Crash rate hourly report from Google Play Developer API
```

### Comparing `google_play_developer_api-0.2.0/pyproject.toml` & `google_play_developer_api-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.2.0"
+version = "0.3.0"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
 description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
@@ -40,14 +40,15 @@
 mkdocs-autorefs = { version = "^0.4.1", optional = true }
 pre-commit = { version = "^3.3.2", optional = true }
 toml = { version = "^0.10.2", optional = true }
 livereload = { version = "^2.6.3", optional = true }
 pyreadline = { version = "^2.1", optional = true }
 mike = { version = "^1.1.2", optional = true }
 requests = { version = "^2.31.0", optional = true }
+google-api-python-client = "^2.89.0"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
```

### Comparing `google_play_developer_api-0.2.0/PKG-INFO` & `google_play_developer_api-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=23.3.0,<24.0.0) ; extra == "test"
 Requires-Dist: flake8 (==6.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: google-api-python-client (>=2.89.0,<3.0.0)
 Requires-Dist: isort (==5.12.0) ; extra == "test"
 Requires-Dist: livereload (>=2.6.3,<3.0.0)
 Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.4,<5.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=9.1.14,<10.0.0) ; extra == "doc"
@@ -48,10 +49,9 @@
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
 Wrapper for APIs
 
 ## Features
 
-* Something
-* Something else
+* Crash rate hourly report from Google Play Developer API
```

