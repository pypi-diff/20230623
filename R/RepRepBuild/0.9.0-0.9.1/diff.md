# Comparing `tmp/RepRepBuild-0.9.0.tar.gz` & `tmp/RepRepBuild-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.9.0.tar", last modified: Fri Jun 16 10:01:22 2023, max compression
+gzip compressed data, was "RepRepBuild-0.9.1.tar", last modified: Wed Jun 21 07:00:01 2023, max compression
```

## Comparing `RepRepBuild-0.9.0.tar` & `RepRepBuild-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.052119 RepRepBuild-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.052119 RepRepBuild-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/HEADER
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.048119 RepRepBuild-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.056119 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.056119 RepRepBuild-0.9.0/src/reprepbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 10:01:21.000000 RepRepBuild-0.9.0/src/reprepbuild/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/articlezip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/latexdep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.035771 RepRepBuild-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.031771 RepRepBuild-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.031771 RepRepBuild-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-06-21 07:00:01.035771 RepRepBuild-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:00:01.035771 RepRepBuild-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.031771 RepRepBuild-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.031771 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 07:00:01.000000 RepRepBuild-0.9.1/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.035771 RepRepBuild-0.9.1/src/reprepbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 07:00:00.000000 RepRepBuild-0.9.1/src/reprepbuild/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/articlezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/latexdep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:00:01.035771 RepRepBuild-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-21 06:59:47.000000 RepRepBuild-0.9.1/tests/test_utils.py
```

### Comparing `RepRepBuild-0.9.0/.github/workflows/pypi.yaml` & `RepRepBuild-0.9.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/.pre-commit-config.yaml` & `RepRepBuild-0.9.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
   hooks:
     - id: black
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   rev: 'v0.0.272'
   hooks:
     - id: ruff
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.23.1
+  rev: 0.23.2
   hooks:
     - id: check-github-workflows
```

### Comparing `RepRepBuild-0.9.0/CHANGELOG.md` & `RepRepBuild-0.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.1] - 2023-06-21
+
+### Fixed
+
+- Print out BibTeX error messages from the correct `.blg` file.
+
 ## [0.9.0] - 2023-06-16
 
 ## Changed
 
 - The variable `REPREPBUILD_CASE_FMT` is no longer prefixed with the script name
   to create filenames for log and dependency files.
   Instead, it is used as such, without prefixing anything to it.
```

### Comparing `RepRepBuild-0.9.0/COPYING` & `RepRepBuild-0.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/HEADER` & `RepRepBuild-0.9.1/HEADER`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/PKG-INFO` & `RepRepBuild-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,14 +694,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
+[![PyPI Upload](https://github.com/reproducible-reporting/reprepbuild/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/reprepbuild/actions/workflows/pypi.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/reprepbuild)](https://pypi.org/project/reprepbuild/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reprepbuild)
+![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/reprepbuild)
+
 # RepRepBuild
 
 RepRepBuild is the build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
 Run `rr` in a source directory, and the publication will be rebuilt from its source.
 
 To get started, follow the [documentation](https://github.com/reproducible-reporting/templates/blob/main/DOCUMENTATION.md) of the [templates](https://github.com/reproducible-reporting/templates) repository.
 RepRepBuild will be installed in your instance of the template, as part of the setup.
```

### Comparing `RepRepBuild-0.9.0/pyproject.toml` & `RepRepBuild-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.9.1/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,14 +694,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
+[![PyPI Upload](https://github.com/reproducible-reporting/reprepbuild/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/reprepbuild/actions/workflows/pypi.yaml)
+[![PyPI Version](https://img.shields.io/pypi/v/reprepbuild)](https://pypi.org/project/reprepbuild/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reprepbuild)
+![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/reprepbuild)
+
 # RepRepBuild
 
 RepRepBuild is the build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
 Run `rr` in a source directory, and the publication will be rebuilt from its source.
 
 To get started, follow the [documentation](https://github.com/reproducible-reporting/templates/blob/main/DOCUMENTATION.md) of the [templates](https://github.com/reproducible-reporting/templates) repository.
 RepRepBuild will be installed in your instance of the template, as part of the setup.
```

### Comparing `RepRepBuild-0.9.0/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.9.1/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 src/reprepbuild/bibtex.py
 src/reprepbuild/latex.py
 src/reprepbuild/latexdep.py
 src/reprepbuild/normalizepdf.py
 src/reprepbuild/pythonscript.py
 src/reprepbuild/repeat.py
 src/reprepbuild/utils.py
-src/reprepbuild/zip.py
+src/reprepbuild/zip.py
+tests/test_utils.py
```

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/__init__.py` & `RepRepBuild-0.9.1/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/__main__.py` & `RepRepBuild-0.9.1/src/reprepbuild/__main__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/articlezip.py` & `RepRepBuild-0.9.1/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/bibtex.py` & `RepRepBuild-0.9.1/src/reprepbuild/bibtex.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if not path_aux.endswith(".first.aux"):
         print(f"BibTeX input must have a `.first.aux` extension. Got {path_aux}")
         return 2
     workdir, fn_aux = os.path.split(path_aux)
     prefix = fn_aux[:-10]
 
     args = ["bibtex", fn_aux]
-    path_blg = os.path.join(workdir, prefix + ".blg")
+    path_blg = os.path.join(workdir, prefix + ".first.blg")
     cp = subprocess.run(
         args,
         cwd=workdir,
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
@@ -86,14 +86,15 @@
         os.rename(
             os.path.join(workdir, f"{prefix}.first.{ext}"),
             os.path.join(workdir, f"{prefix}.{ext}"),
         )
 
     # Parse the blg file to get a list of used bib files.
     paths_bib = set()
+    path_blg = os.path.join(workdir, prefix + ".blg")
     with open(path_blg) as f:
         for line in f:
             if line.startswith("Database file #"):
                 paths_bib.add(os.path.join(workdir, line.split()[-1]))
 
     # Discard the bib files generated by LaTeX.
     path_fls = os.path.join(workdir, prefix + ".fls")
```

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/latex.py` & `RepRepBuild-0.9.1/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/latexdep.py` & `RepRepBuild-0.9.1/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.9.1/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.9.1/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/repeat.py` & `RepRepBuild-0.9.1/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/utils.py` & `RepRepBuild-0.9.1/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.9.0/src/reprepbuild/zip.py` & `RepRepBuild-0.9.1/src/reprepbuild/zip.py`

 * *Files identical despite different names*

