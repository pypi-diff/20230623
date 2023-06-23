# Comparing `tmp/codebleu-0.0.1.tar.gz` & `tmp/codebleu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebleu-0.0.1.tar", last modified: Fri Jun 23 10:49:47 2023, max compression
+gzip compressed data, was "codebleu-0.0.2.tar", last modified: Fri Jun 23 19:04:52 2023, max compression
```

## Comparing `codebleu-0.0.1.tar` & `codebleu-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 10:49:47.294566 codebleu-0.0.1/
--rw-r--r--   0 kblack     (502) staff       (20)     1078 2023-06-23 10:11:09.000000 codebleu-0.0.1/LICENSE
--rw-r--r--   0 kblack     (502) staff       (20)      645 2023-06-23 10:49:47.294212 codebleu-0.0.1/PKG-INFO
--rw-r--r--   0 kblack     (502) staff       (20)       54 2023-06-23 10:11:09.000000 codebleu-0.0.1/README.md
--rw-r--r--   0 kblack     (502) staff       (20)        5 2023-06-23 10:43:58.000000 codebleu-0.0.1/VERSION
-drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 10:49:47.291869 codebleu-0.0.1/codebleu/
--rw-r--r--   0 kblack     (502) staff       (20)        0 2023-06-23 10:16:33.000000 codebleu-0.0.1/codebleu/__init__.py
-drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 10:49:47.293751 codebleu-0.0.1/codebleu.egg-info/
--rw-r--r--   0 kblack     (502) staff       (20)      645 2023-06-23 10:49:47.000000 codebleu-0.0.1/codebleu.egg-info/PKG-INFO
--rw-r--r--   0 kblack     (502) staff       (20)      229 2023-06-23 10:49:47.000000 codebleu-0.0.1/codebleu.egg-info/SOURCES.txt
--rw-r--r--   0 kblack     (502) staff       (20)        1 2023-06-23 10:49:47.000000 codebleu-0.0.1/codebleu.egg-info/dependency_links.txt
--rw-r--r--   0 kblack     (502) staff       (20)      182 2023-06-23 10:49:47.000000 codebleu-0.0.1/codebleu.egg-info/requires.txt
--rw-r--r--   0 kblack     (502) staff       (20)        9 2023-06-23 10:49:47.000000 codebleu-0.0.1/codebleu.egg-info/top_level.txt
--rw-r--r--   0 kblack     (502) staff       (20)     1660 2023-06-23 10:48:00.000000 codebleu-0.0.1/pyproject.toml
--rw-r--r--   0 kblack     (502) staff       (20)       38 2023-06-23 10:49:47.294659 codebleu-0.0.1/setup.cfg
--rw-r--r--   0 kblack     (502) staff       (20)       88 2023-06-23 10:41:31.000000 codebleu-0.0.1/setup.py
+drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 19:04:52.016613 codebleu-0.0.2/
+-rw-r--r--   0 kblack     (502) staff       (20)     1078 2023-06-23 10:11:09.000000 codebleu-0.0.2/LICENSE
+-rw-r--r--   0 kblack     (502) staff       (20)      779 2023-06-23 19:04:52.015798 codebleu-0.0.2/PKG-INFO
+-rw-r--r--   0 kblack     (502) staff       (20)      244 2023-06-23 18:38:56.000000 codebleu-0.0.2/README.md
+-rw-r--r--   0 kblack     (502) staff       (20)        5 2023-06-23 14:24:10.000000 codebleu-0.0.2/VERSION
+drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 19:04:51.999196 codebleu-0.0.2/codebleu/
+-rw-r--r--   0 kblack     (502) staff       (20)       65 2023-06-23 18:09:55.000000 codebleu-0.0.2/codebleu/__init__.py
+-rw-r--r--   0 kblack     (502) staff       (20)     2833 2023-06-23 18:36:54.000000 codebleu-0.0.2/codebleu/__main__.py
+-rw-r--r--   0 kblack     (502) staff       (20)    28527 2023-06-23 18:09:56.000000 codebleu-0.0.2/codebleu/bleu.py
+-rw-r--r--   0 kblack     (502) staff       (20)     3656 2023-06-23 18:36:54.000000 codebleu-0.0.2/codebleu/codebleu.py
+-rw-r--r--   0 kblack     (502) staff       (20)     5140 2023-06-23 18:18:18.000000 codebleu-0.0.2/codebleu/dataflow_match.py
+drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 19:04:52.012841 codebleu-0.0.2/codebleu/parser/
+-rw-r--r--   0 kblack     (502) staff       (20)    56861 2023-06-23 18:20:06.000000 codebleu-0.0.2/codebleu/parser/DFG.py
+-rw-r--r--   0 kblack     (502) staff       (20)      592 2023-06-23 18:20:06.000000 codebleu-0.0.2/codebleu/parser/__init__.py
+-rw-r--r--   0 kblack     (502) staff       (20)      374 2023-06-23 18:09:55.000000 codebleu-0.0.2/codebleu/parser/build.py
+-rw-r--r--   0 kblack     (502) staff       (20)     3681 2023-06-23 18:09:56.000000 codebleu-0.0.2/codebleu/parser/utils.py
+-rw-r--r--   0 kblack     (502) staff       (20)     2629 2023-06-23 18:20:06.000000 codebleu-0.0.2/codebleu/syntax_match.py
+-rw-r--r--   0 kblack     (502) staff       (20)     4013 2023-06-23 18:09:55.000000 codebleu-0.0.2/codebleu/utils.py
+-rw-r--r--   0 kblack     (502) staff       (20)    25797 2023-06-23 18:14:29.000000 codebleu-0.0.2/codebleu/weighted_ngram_match.py
+drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 19:04:52.005845 codebleu-0.0.2/codebleu.egg-info/
+-rw-r--r--   0 kblack     (502) staff       (20)      779 2023-06-23 19:04:51.000000 codebleu-0.0.2/codebleu.egg-info/PKG-INFO
+-rw-r--r--   0 kblack     (502) staff       (20)      515 2023-06-23 19:04:51.000000 codebleu-0.0.2/codebleu.egg-info/SOURCES.txt
+-rw-r--r--   0 kblack     (502) staff       (20)        1 2023-06-23 19:04:51.000000 codebleu-0.0.2/codebleu.egg-info/dependency_links.txt
+-rw-r--r--   0 kblack     (502) staff       (20)      203 2023-06-23 19:04:51.000000 codebleu-0.0.2/codebleu.egg-info/requires.txt
+-rw-r--r--   0 kblack     (502) staff       (20)        9 2023-06-23 19:04:51.000000 codebleu-0.0.2/codebleu.egg-info/top_level.txt
+-rw-r--r--   0 kblack     (502) staff       (20)     1752 2023-06-23 19:02:36.000000 codebleu-0.0.2/pyproject.toml
+-rw-r--r--   0 kblack     (502) staff       (20)       38 2023-06-23 19:04:52.016868 codebleu-0.0.2/setup.cfg
+-rw-r--r--   0 kblack     (502) staff       (20)       88 2023-06-23 10:41:31.000000 codebleu-0.0.2/setup.py
+drwxr-xr-x   0 kblack     (502) staff       (20)        0 2023-06-23 19:04:52.014311 codebleu-0.0.2/tests/
+-rw-r--r--   0 kblack     (502) staff       (20)     1992 2023-06-23 18:24:12.000000 codebleu-0.0.2/tests/test_codebleu.py
```

### Comparing `codebleu-0.0.1/LICENSE` & `codebleu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codebleu-0.0.1/pyproject.toml` & `codebleu-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "codebleu"
-description = "Pip compatible `CodeBLEU` implementation"
+description = "Unofficial pip/hf compatible `CodeBLEU` implementation"
 readme = "README.md"
 license = {text = "MIT License"}
 authors = [
   {name = "Konstantin Chernyshev", email = "kdchernyshev@gmail.com"},
 ]
 dynamic = ["version"]
 
@@ -23,26 +23,26 @@
 
 dependencies = [
     "tree-sitter >=0.20.0,<1.0.0",
 ]
 
 
 [project.urls]
-homepage = "https://github.com/k4black/fastapi-jwt"
-documentation = "https://k4black.github.io/fastapi-jwt/"
+homepage = "https://github.com/k4black/codebleu"
 
 
 [project.optional-dependencies]
 test = [
     "pytest >=7.0.0,<8.0.0",
     "pytest-cov >=4.0.0,<5.0.0",
     "pytest-mock >=3.0.0,<4.0.0",
-    "black ==23.1.0",
+    "black ==23.3.0",
     "mypy >=1.0.0,<2.0.0",
     "flake8 >=6.0.0,<7.0.0",
+    "ruff >=0.0.275,<0.1.0",
     "isort >=5.11.0,<6.0.0",
 ]
 
 
 
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
@@ -61,15 +61,16 @@
 warn_unreachable = true
 allow_untyped_decorators = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 python_files = "test_*.py"
-addopts = "--cov=fastapi_jwt/ --cov-report term-missing"
+addopts = "--cov=codebleu/ --cov-report term-missing"
 
 [tool.isort]
 profile = "black"
-src_paths = ["fastapi-jwt", "tests"]
-known_first_party = ["fastapi_jwt", "tests"]
+src_paths = ["codebleu", "tests"]
+known_first_party = ["codebleu", "tests"]
 line_length = 120
 combine_as_imports = true
+skip = ["build", "dist", ".venv", ".eggs", ".mypy_cache", ".pytest_cache", ".git", ".tox", ".nox", "codebleu/parser"]
```

