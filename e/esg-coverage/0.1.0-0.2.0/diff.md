# Comparing `tmp/esg_coverage-0.1.0.tar.gz` & `tmp/esg_coverage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esg_coverage-0.1.0.tar", max compression
+gzip compressed data, was "esg_coverage-0.2.0.tar", max compression
```

## Comparing `esg_coverage-0.1.0.tar` & `esg_coverage-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-06-05 10:20:27.887906 esg_coverage-0.1.0/LICENSE
--rw-r--r--   0        0        0     2661 2023-06-05 10:20:27.887906 esg_coverage-0.1.0/README.md
--rw-r--r--   0        0        0     2959 2023-06-05 10:20:42.860121 esg_coverage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      318 2023-06-05 10:20:27.887906 esg_coverage-0.1.0/src/esgcov/__cli__.py
--rw-r--r--   0        0        0      135 2023-06-05 10:20:27.887906 esg_coverage-0.1.0/src/esgcov/__init__.py
--rw-r--r--   0        0        0       22 2023-06-05 10:20:42.804120 esg_coverage-0.1.0/src/esgcov/_version.py
--rw-r--r--   0        0        0      288 2023-06-05 10:20:42.804120 esg_coverage-0.1.0/src/esgcov/conf/about/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-05 10:20:27.887906 esg_coverage-0.1.0/src/esgcov/py.typed
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 esg_coverage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 21:03:21.257344 esg_coverage-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2873 2023-06-23 21:03:21.257344 esg_coverage-0.2.0/README.md
+-rw-r--r--   0        0        0     2996 2023-06-23 21:03:44.650091 esg_coverage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-23 21:03:44.598091 esg_coverage-0.2.0/src/esgcov/_version.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-23 21:03:44.598091 esg_coverage-0.2.0/src/esgcov/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__task__.yaml
+-rw-r--r--   0        0        0       85 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0      113 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      806 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      153 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/py.typed
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 esg_coverage-0.2.0/PKG-INFO
```

### Comparing `esg_coverage-0.1.0/LICENSE` & `esg_coverage-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.1.0/README.md` & `esg_coverage-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # The Analyst Pathway in ESG
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/esg-coverage/branch/main/graph/badge.svg?token=FL2N6C7KFP
+[codecov-url]: https://codecov.io/gh/entelecheia/esg-coverage
 [pypi-image]: https://img.shields.io/pypi/v/esg-coverage
 [license-image]: https://img.shields.io/github/license/entelecheia/esg-coverage
 [license-url]: https://github.com/entelecheia/esg-coverage/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/esg-coverage?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/esg-coverage
 [release-url]: https://github.com/entelecheia/esg-coverage/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

### Comparing `esg_coverage-0.1.0/pyproject.toml` & `esg_coverage-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "esg-coverage"
-version = "0.1.0"
+version = "0.2.0"
 description = "The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://esg-coverage.entelecheia.ai"
 repository = "https://github.com/entelecheia/esg-coverage"
 readme = "README.md"
 packages = [{ include = "esgcov", from = "src" }]
 
 [tool.poetry.scripts]
 esgcov = 'esgcov.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
+hyfi = "^0.12.2"
+tabulate = "^0.9.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `esg_coverage-0.1.0/PKG-INFO` & `esg_coverage-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: esg-coverage
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance
 Home-page: https://esg-coverage.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: hyfi (>=0.12.2,<0.13.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/entelecheia/esg-coverage
 Description-Content-Type: text/markdown
 
 # The Analyst Pathway in ESG
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
+[codecov-image]: https://codecov.io/gh/entelecheia/esg-coverage/branch/main/graph/badge.svg?token=FL2N6C7KFP
+[codecov-url]: https://codecov.io/gh/entelecheia/esg-coverage
 [pypi-image]: https://img.shields.io/pypi/v/esg-coverage
 [license-image]: https://img.shields.io/github/license/entelecheia/esg-coverage
 [license-url]: https://github.com/entelecheia/esg-coverage/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/esg-coverage?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/esg-coverage
 [release-url]: https://github.com/entelecheia/esg-coverage/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

