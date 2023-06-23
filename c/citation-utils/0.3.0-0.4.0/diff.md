# Comparing `tmp/citation_utils-0.3.0.tar.gz` & `tmp/citation_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.3.0.tar", max compression
+gzip compressed data, was "citation_utils-0.4.0.tar", max compression
```

## Comparing `citation_utils-0.3.0.tar` & `citation_utils-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:09:44.831887 citation_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0       48 2023-06-21 17:13:19.096449 citation_utils-0.3.0/citation_utils/__init__.py
--rw-r--r--   0        0        0     1580 2023-06-21 16:59:09.647600 citation_utils-0.3.0/citation_utils/helpers.py
--rw-r--r--   0        0        0     9366 2023-06-21 17:53:25.038555 citation_utils-0.3.0/citation_utils/main.py
--rw-r--r--   0        0        0      541 2023-06-21 15:09:44.832651 citation_utils-0.3.0/citation_utils/sql/legacy/multiple_cat_idx.sql
--rw-r--r--   0        0        0     1437 2023-06-21 17:51:04.566583 citation_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 citation_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.0/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-23 10:27:21.228547 citation_utils-0.4.0/citation_utils/__init__.py
+-rw-r--r--   0        0        0    13224 2023-06-23 10:27:21.228689 citation_utils-0.4.0/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-23 10:27:21.228818 citation_utils-0.4.0/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3155 2023-06-23 10:27:21.228950 citation_utils-0.4.0/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3194 2023-06-23 10:27:21.229021 citation_utils-0.4.0/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-23 10:27:21.229092 citation_utils-0.4.0/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2893 2023-06-23 10:27:21.229189 citation_utils-0.4.0/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-23 10:27:21.229296 citation_utils-0.4.0/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2385 2023-06-23 10:27:21.229386 citation_utils-0.4.0/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-23 10:27:21.229484 citation_utils-0.4.0/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     1767 2023-06-23 10:27:21.229558 citation_utils-0.4.0/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      349 2023-06-23 10:27:21.229679 citation_utils-0.4.0/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-23 10:27:21.229791 citation_utils-0.4.0/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-23 10:27:21.229898 citation_utils-0.4.0/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1696 2023-06-23 10:27:21.229985 citation_utils-0.4.0/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     3375 2023-06-23 10:27:21.230105 citation_utils-0.4.0/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     1419 2023-06-23 10:27:21.230196 citation_utils-0.4.0/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-23 10:27:21.230290 citation_utils-0.4.0/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-23 10:27:21.230427 citation_utils-0.4.0/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-23 10:27:21.230521 citation_utils-0.4.0/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-23 10:27:21.230609 citation_utils-0.4.0/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-23 10:27:21.230693 citation_utils-0.4.0/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5760 2023-06-23 10:27:21.230811 citation_utils-0.4.0/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-23 10:27:21.231091 citation_utils-0.4.0/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-06-23 10:29:13.617295 citation_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.0/PKG-INFO
```

### Comparing `citation_utils-0.3.0/LICENSE` & `citation_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.3.0/pyproject.toml` & `citation_utils-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
-name = "citation-utils"
-version = "0.3.0"
-description = "Regex-based docket- and report- styled citations based on Philippine Supreme Court decisions."
+name = "citation_utils"
+version = "0.4.0"
+description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
   "Programming Language :: Python :: 3.11",
@@ -14,38 +14,34 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-citation-docket = "^0.1.5"
+citation_report = "^0.1.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
-ipykernel = "^6.23"
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.16"
-types-PyYAML = "^6.0.7"
+ipykernel = "^6.23.2"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
-addopts = "-ra -q --cov --doctest-modules"
+addopts = "-ra -q --doctest-modules --cov"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
 testpaths = ["tests", "citation_utils"]
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
-[tool.ruff.per-file-ignores]
-"tests/test_main.py" = ["E501"]
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `citation_utils-0.3.0/PKG-INFO` & `citation_utils-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.3.0
-Summary: Regex-based docket- and report- styled citations based on Philippine Supreme Court decisions.
+Version: 0.4.0
+Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation-docket (>=0.1.5,<0.2.0)
+Requires-Dist: citation_report (>=0.1.5,<0.2.0)
 Project-URL: Documentation, https://justmars.github.io/citation-utils
 Project-URL: Repository, https://github.com/justmars/citation-utils
```

