# Comparing `tmp/jsonschema_specifications-2023.5.2.tar.gz` & `tmp/jsonschema_specifications-2023.6.1.tar.gz`

## Comparing `jsonschema_specifications-2023.5.2.tar` & `jsonschema_specifications-2023.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.coveragerc
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.flake8
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.readthedocs.yml
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/release.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/Makefile
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/api.rst
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/conf.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/index.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/requirements.in
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/__init__.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/_core.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/metaschema.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/content
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/core
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/validation
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/metaschema.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/content
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/core
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/validation
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft3/metaschema.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft4/metaschema.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft6/metaschema.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft7/metaschema.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/tests/test_jsonschema_specifications.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/COPYING
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/README.rst
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/pyproject.toml
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.coveragerc
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.flake8
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.github/release.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/Makefile
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/api.rst
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/conf.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/index.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/requirements.in
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/_core.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/metaschema.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/content
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/core
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/metaschema.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/content
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/core
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/format
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft3/metaschema.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft4/metaschema.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft6/metaschema.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft7/metaschema.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/jsonschema_specifications/tests/test_jsonschema_specifications.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/COPYING
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/README.rst
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.6.1/PKG-INFO
```

### Comparing `jsonschema_specifications-2023.5.2/.pre-commit-config.yaml` & `jsonschema_specifications-2023.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/noxfile.py` & `jsonschema_specifications-2023.6.1/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 PACKAGE = ROOT / "jsonschema_specifications"
@@ -19,15 +20,16 @@
 
     return _session
 
 
 @session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
     session.install("pytest", ROOT)
-    session.run("pytest", "--verbosity=3")
+    env = dict(os.environ, PYTHONWARNDEFAULTENCODING="1")
+    session.run("pytest", "--verbosity=3", "--pythonwarnings=error", env=env)
 
 
 @session()
 def audit(session):
     session.install("pip-audit", ROOT)
     session.run("python", "-m", "pip_audit")
```

### Comparing `jsonschema_specifications-2023.5.2/.github/SECURITY.md` & `jsonschema_specifications-2023.6.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/.github/workflows/ci.yml` & `jsonschema_specifications-2023.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/docs/Makefile` & `jsonschema_specifications-2023.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/docs/conf.py` & `jsonschema_specifications-2023.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/docs/index.rst` & `jsonschema_specifications-2023.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/docs/requirements.txt` & `jsonschema_specifications-2023.6.1/docs/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-docutils==0.19
+docutils==0.20.1
     # via sphinx
 fonttools==4.39.4
     # via matplotlib
-furo==2023.3.27
+furo==2023.5.20
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
@@ -59,27 +59,27 @@
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
 pyparsing==3.0.9
     # via matplotlib
 python-dateutil==2.8.2
     # via matplotlib
-referencing==0.28.1
+referencing==0.28.5
     # via jsonschema-specifications
-requests==2.30.0
+requests==2.31.0
     # via sphinx
 rpds-py==0.7.1
     # via referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.0.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
```

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/_core.py` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     # So this takes some liberties given the real layout of what we ship
     # (only 2 levels of nesting, no directories within the second level).
 
     for version in files(__package__).joinpath("schemas").iterdir():
         for child in version.iterdir():
             children = [child] if child.is_file() else child.iterdir()
             for path in children:
-                contents = json.loads(path.read_text())
+                contents = json.loads(path.read_text(encoding="utf-8"))
                 yield Resource.from_contents(contents)
```

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/applicator` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/content` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/core` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/validation` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/applicator` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/content` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/core` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/validation` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft3/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft3/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft4/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft4/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft6/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft6/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft7/metaschema.json` & `jsonschema_specifications-2023.6.1/jsonschema_specifications/schemas/draft7/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/COPYING` & `jsonschema_specifications-2023.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/README.rst` & `jsonschema_specifications-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/pyproject.toml` & `jsonschema_specifications-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.2/PKG-INFO` & `jsonschema_specifications-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-specifications
-Version: 2023.5.2
+Version: 2023.6.1
 Summary: The JSON Schema meta-schemas and vocabularies, exposed as a Registry
 Project-URL: Documentation, https://jsonschema-specifications.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/jsonschema-specifications
 Project-URL: Issues, https://github.com/python-jsonschema/jsonschema-specifications/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/jsonschema-specifications
 Author: Julian Berman
```

