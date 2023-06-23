# Comparing `tmp/pip-run-9.4.0.tar.gz` & `tmp/pip-run-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-run-9.4.0.tar", last modified: Tue Dec 27 16:16:26 2022, max compression
+gzip compressed data, was "pip-run-9.5.0.tar", last modified: Fri Dec 30 02:22:40 2022, max compression
```

## Comparing `pip-run-9.4.0.tar` & `pip-run-9.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.711426 pip-run-9.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-27 16:16:06.000000 pip-run-9.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-27 16:16:06.000000 pip-run-9.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-27 16:16:06.000000 pip-run-9.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.703426 pip-run-9.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-27 16:16:06.000000 pip-run-9.4.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-27 16:16:06.000000 pip-run-9.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.703426 pip-run-9.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2022-12-27 16:16:06.000000 pip-run-9.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-27 16:16:06.000000 pip-run-9.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-27 16:16:06.000000 pip-run-9.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2022-12-27 16:16:06.000000 pip-run-9.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-27 16:16:06.000000 pip-run-9.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2022-12-27 16:16:26.711426 pip-run-9.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2022-12-27 16:16:06.000000 pip-run-9.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-27 16:16:06.000000 pip-run-9.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.703426 pip-run-9.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2022-12-27 16:16:06.000000 pip-run-9.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2022-12-27 16:16:06.000000 pip-run-9.4.0/docs/cowsay.svg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-27 16:16:06.000000 pip-run-9.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-27 16:16:06.000000 pip-run-9.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.703426 pip-run-9.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-27 16:16:06.000000 pip-run-9.4.0/examples/plotter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2022-12-27 16:16:06.000000 pip-run-9.4.0/examples/test-mongodb-covered-query.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-27 16:16:06.000000 pip-run-9.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip-run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.707426 pip-run-9.4.0/pip_run/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/_py38compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/persist.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/read-deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2022-12-27 16:16:06.000000 pip-run-9.4.0/pip_run/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.711426 pip-run-9.4.0/pip_run.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-27 16:16:26.000000 pip-run-9.4.0/pip_run.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-27 16:16:06.000000 pip-run-9.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-27 16:16:06.000000 pip-run-9.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-12-27 16:16:26.711426 pip-run-9.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 16:16:26.711426 pip-run-9.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-27 16:16:06.000000 pip-run-9.4.0/tests/test_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2022-12-27 16:16:06.000000 pip-run-9.4.0/tests/test_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2022-12-27 16:16:06.000000 pip-run-9.4.0/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-27 16:16:06.000000 pip-run-9.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.860168 pip-run-9.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-30 02:22:15.000000 pip-run-9.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-30 02:22:15.000000 pip-run-9.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-30 02:22:15.000000 pip-run-9.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.852167 pip-run-9.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-30 02:22:15.000000 pip-run-9.5.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-30 02:22:15.000000 pip-run-9.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.852167 pip-run-9.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2022-12-30 02:22:15.000000 pip-run-9.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-30 02:22:15.000000 pip-run-9.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-30 02:22:15.000000 pip-run-9.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2022-12-30 02:22:15.000000 pip-run-9.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-30 02:22:15.000000 pip-run-9.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2022-12-30 02:22:40.860168 pip-run-9.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2022-12-30 02:22:15.000000 pip-run-9.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-30 02:22:15.000000 pip-run-9.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.852167 pip-run-9.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2022-12-30 02:22:15.000000 pip-run-9.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2022-12-30 02:22:15.000000 pip-run-9.5.0/docs/cowsay.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-30 02:22:15.000000 pip-run-9.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-30 02:22:15.000000 pip-run-9.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.852167 pip-run-9.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-30 02:22:15.000000 pip-run-9.5.0/examples/plotter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2022-12-30 02:22:15.000000 pip-run-9.5.0/examples/test-mongodb-covered-query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-30 02:22:15.000000 pip-run-9.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip-run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.856167 pip-run-9.5.0/pip_run/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/_py38compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/read-deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2022-12-30 02:22:15.000000 pip-run-9.5.0/pip_run/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.860168 pip-run-9.5.0/pip_run.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-30 02:22:40.000000 pip-run-9.5.0/pip_run.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-30 02:22:15.000000 pip-run-9.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-30 02:22:15.000000 pip-run-9.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-12-30 02:22:40.860168 pip-run-9.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:22:40.860168 pip-run-9.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-30 02:22:15.000000 pip-run-9.5.0/tests/test_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-30 02:22:15.000000 pip-run-9.5.0/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2022-12-30 02:22:15.000000 pip-run-9.5.0/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-30 02:22:15.000000 pip-run-9.5.0/tox.ini
```

### Comparing `pip-run-9.4.0/.github/workflows/main.yml` & `pip-run-9.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/CHANGES.rst` & `pip-run-9.5.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v9.5.0
+======
+
+Modernized path handling using pathlib (internal refactoring).
+
+Renamed ``commands.parse_script_args`` to ``separate``, with an
+alias for compatibility.
+
+Restored coverage in tests.
+
 v9.4.0
 ======
 
 #64: Switch to ``platformdirs`` for resolving the cache dir.
 
 v9.3.0
 ======
```

### Comparing `pip-run-9.4.0/LICENSE` & `pip-run-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/PKG-INFO` & `pip-run-9.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-run
-Version: 9.4.0
+Version: 9.5.0
 Summary: install packages and run Python with them
 Home-page: https://github.com/jaraco/pip-run
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pip-run-9.4.0/README.rst` & `pip-run-9.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/conftest.py` & `pip-run-9.5.0/conftest.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/docs/conf.py` & `pip-run-9.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/docs/cowsay.svg` & `pip-run-9.5.0/docs/cowsay.svg`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/docs/index.rst` & `pip-run-9.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/examples/plotter.ipynb` & `pip-run-9.5.0/examples/plotter.ipynb`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/examples/test-mongodb-covered-query.py` & `pip-run-9.5.0/examples/test-mongodb-covered-query.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/pip_run/commands.py` & `pip-run-9.5.0/pip_run/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import textwrap
 import pathlib
 import contextlib
 import warnings
+import argparse
 
 from more_itertools import split_before, split_at
 
 
 def _separate_script(args):
     """
     Inject a double-dash before the first arg that appears to be an
@@ -45,25 +46,34 @@
     ...
     ValueError: ...
     """
     pre, post = split_at(args, '--'.__eq__, maxsplit=1)
     return pre, post
 
 
-def parse_script_args(args):
+def separate(args):
     """
     Separate the command line arguments into arguments for pip
     and arguments to Python.
+
+    >>> separate(['foo', '--', 'bar'])
+    (['foo'], ['bar'])
+    >>> separate(['foo', 'bar'])
+    (['foo', 'bar'], [])
     """
     with contextlib.suppress(ValueError):
         return _separate_dash(args)
 
     return _separate_script(args)
 
 
+# for compatibility
+parse_script_args = separate
+
+
 def separate_dash(args):
     """
     Separate args based on dash separator.
 
     Deprecated; retained for compatibility.
 
     >>> separate_dash(['foo', '--', 'bar'])
@@ -74,18 +84,16 @@
     """
     warnings.warn("separate_dash is deprecated", DeprecationWarning)
     with contextlib.suppress(ValueError):
         return _separate_dash(args)
     return [args, []]
 
 
-help_doc = textwrap.dedent(
+usage = textwrap.dedent(
     """
-    Usage:
-
     Arguments to pip-run prior to `--` are used to specify the requirements
     to make available, just as arguments to pip install. For example,
 
         pip-run -r requirements.txt "requests>=2.0"
 
     That will launch python after installing the deps in requirements.txt
     and also a late requests. Packages are always installed to a temporary
@@ -112,10 +120,8 @@
 ).lstrip()
 
 
 def intercept(args):
     """
     Detect certain args and intercept them.
     """
-    if '--help' in args or '-h' in args:
-        print(help_doc)
-        raise SystemExit(0)
+    argparse.ArgumentParser(usage=usage).parse_known_args(args)
```

### Comparing `pip-run-9.4.0/pip_run/deps.py` & `pip-run-9.5.0/pip_run/deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import types
 import importlib
 
 import packaging.requirements
 
 try:
     from importlib import metadata  # type: ignore
-except ImportError:
+except ImportError:  # pragma: no cover
     import importlib_metadata as metadata  # type: ignore
 
 from ._py38compat import subprocess_path as sp
 
 
 class Install(types.SimpleNamespace):
 
@@ -67,33 +67,17 @@
 
 
 @contextlib.contextmanager
 def load(*args):
     with target_mod().context(args) as target:
         cmd = (sys.executable, '-m', 'pip', 'install', '-t', sp(target)) + args
         env = dict(os.environ, PIP_QUIET="1")
-        Install.parse(args) and empty(target) and subprocess.check_call(cmd, env=env)
-        yield str(target)
-
-
-@contextlib.contextmanager
-def _save_file(filename):
-    """
-    Capture the state of filename and restore it after the context
-    exits.
-    """
-    # For now, only supports a missing filename.
-    if os.path.exists(filename):
-        tmpl = "Unsupported with extant {filename}"
-        raise NotImplementedError(tmpl.format(**locals()))
-    try:
-        yield
-    finally:
-        if os.path.exists(filename):
-            os.remove(filename)
+        if Install.parse(args) and empty(target):
+            subprocess.check_call(cmd, env=env)
+        yield target
 
 
 # from jaraco.context
 class suppress(contextlib.suppress, contextlib.ContextDecorator):
     """
     A version of contextlib.suppress with decorator support.
```

### Comparing `pip-run-9.4.0/pip_run/launch.py` & `pip-run-9.5.0/pip_run/launch.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
     @classmethod
     def _read(cls, target):
         """
         As .pth files aren't honored except in site dirs,
         read the paths indicated by them.
         """
-        target_path = pathlib.Path(target)
-        pth_files = target_path.glob('*.pth')
+        pth_files = target.glob('*.pth')
         file_items = map(cls._read_file, pth_files)
         return itertools.chain.from_iterable(file_items)
 
 
 def inject_sitecustomize(target):
     """
     Create a sitecustomize file in the target that will install
@@ -43,55 +42,53 @@
     """
     hook = textwrap.dedent(
         f"""
         import site
         site.addsitedir({target!r})
         """
     ).lstrip()
-    sc_fn = pathlib.Path(target) / 'sitecustomize.py'
-    sc_fn.write_text(hook)
+    target.joinpath('sitecustomize.py').write_text(hook)
 
 
 def _pythonpath():
     return 'JYTHONPATH' if sys.platform.startswith('java') else 'PYTHONPATH'
 
 
 def _build_env(target):
     """
     Prepend target and .pth references in target to PYTHONPATH
     """
     key = _pythonpath()
     env = dict(os.environ)
-    suffix = env.get(key)
-    prefix = (target,)
-    items = itertools.chain(
-        prefix, PathReader._read(target), (suffix,) if suffix else ()
-    )
+    previous = env.get(key)
+    suffix = (previous,) * bool(previous)
+    prefix = (os.fspath(target),)
+    items = itertools.chain(prefix, PathReader._read(target), suffix)
     joined = os.pathsep.join(items)
-    env[key] = joined
+    env[key] = os.fspath(joined)
     return env
 
 
 def _setup_env(target):
     inject_sitecustomize(target)
     return _build_env(target)
 
 
-def with_path(target, params):
+def with_path(target: pathlib.Path, params):
     """
     Launch Python with target on the path and params
     """
 
     def null_handler(signum, frame):
-        pass
+        pass  # pragma: no cover
 
     signal.signal(signal.SIGINT, null_handler)
     cmd = [sys.executable] + params
     return subprocess.Popen(cmd, env=_setup_env(target)).wait()
 
 
-def with_path_overlay(target, params):
+def with_path_overlay(target, params):  # pragma: no cover
     """
     Overlay Python with target on the path and params
     """
     cmd = [sys.executable] + params
     os.execve(sys.executable, cmd, _setup_env(target))
```

### Comparing `pip-run-9.4.0/pip_run/persist.py` & `pip-run-9.5.0/pip_run/persist.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/pip_run/read-deps.py` & `pip-run-9.5.0/pip_run/read-deps.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/pip_run/scripts.py` & `pip-run-9.5.0/pip_run/scripts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import sys
 import ast
-import tokenize
 import json
 import pathlib
 import abc
 import contextlib
 import itertools
 import re
 
@@ -141,24 +139,7 @@
         lines = (
             line
             for cell in doc['cells']
             for line in cell['source'] + ['\n']
             if cell['cell_type'] == 'code' and not line.startswith('%')
         )
         return cls(''.join(lines))
-
-
-def run(cmdline):
-    """
-    Execute the script as if it had been invoked naturally.
-    """
-    namespace = dict()
-    filename = cmdline[0]
-    namespace['__file__'] = filename
-    namespace['__name__'] = '__main__'
-    sys.argv[:] = cmdline
-
-    open_ = getattr(tokenize, 'open', open)
-    script = open_(filename).read()
-    norm_script = script.replace('\\r\\n', '\\n')
-    code = compile(norm_script, filename, 'exec')
-    exec(code, namespace)
```

### Comparing `pip-run-9.4.0/pip_run.egg-info/PKG-INFO` & `pip-run-9.5.0/pip_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-run
-Version: 9.4.0
+Version: 9.5.0
 Summary: install packages and run Python with them
 Home-page: https://github.com/jaraco/pip-run
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pip-run-9.4.0/pip_run.egg-info/SOURCES.txt` & `pip-run-9.5.0/pip_run.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/pytest.ini` & `pip-run-9.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/setup.cfg` & `pip-run-9.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/tests/test_deps.py` & `pip-run-9.5.0/tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/tests/test_launch.py` & `pip-run-9.5.0/tests/test_launch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 import sys
 import subprocess
 import textwrap
 import os
+import pathlib
 
 import pytest
 
 from pip_run import launch
 
 
-def test_with_path(tmpdir, capfd):
+def test_with_path(tmp_path, capfd):
     params = ['-c', 'import sys; sys.stdout.write("\\n".join(sys.path))']
-    res = launch.with_path(str(tmpdir), params)
+    res = launch.with_path(tmp_path, params)
     assert res == 0
     out, err = capfd.readouterr()
-    assert tmpdir in out.split(os.linesep)
+    assert str(tmp_path) in out.split(os.linesep)
 
 
-def test_with_path_result_code(tmpdir):
+def test_with_path_result_code(tmp_path):
     """
     result code should be non-zero on error
     """
     params = ['-c', "raise ValueError()"]
-    res = launch.with_path(str(tmpdir), params)
+    res = launch.with_path(tmp_path, params)
     assert res > 0
 
 
 @pytest.mark.xfail(reason="cleanup can't occur with execv; #4")
-def test_with_path_overlay(tmpdir, capfd):
+def test_with_path_overlay(tmp_path, capfd):
     params = ['-c', 'import sys; sys.stdout.write("\\n".join(sys.path))']
     # launch subprocess so as not to overlay the test process
     script = (
         textwrap.dedent(
             """
-        import pip_run.launch
-        pip_run.launch.with_path_overlay({tmpdir!r}, {params!r})
-        print("cleanup")
-    """
+            import pip_run.launch, pathlib
+            pip_run.launch.with_path_overlay(pathlib.Path({temp_dir!r}), {params!r})
+            print("cleanup")
+            """
         )
         .strip()
         .replace('\n', '; ')
-        .format(tmpdir=str(tmpdir), params=params)
+        .format(temp_dir=str(tmp_path), params=params)
     )
-    subprocess.Popen([sys.executable, '-c', script]).wait()
+    subprocess.check_call([sys.executable, '-c', script])
     out, err = capfd.readouterr()
-    assert str(tmpdir) in out.split(os.linesep)
+    assert str(tmp_path) in out.split(os.linesep)
     assert "cleanup" in out
 
 
 @pytest.fixture
 def clean_pythonpath(monkeypatch):
     monkeypatch.delitem(os.environ, 'PYTHONPATH', raising=False)
 
 
 def test_build_env(clean_pythonpath):
     os.environ['PYTHONPATH'] = 'something'
-    env = launch._build_env('else')
+    env = launch._build_env(pathlib.Path('else'))
     expected = os.pathsep.join(('else', 'something'))
     assert env['PYTHONPATH'] == expected
 
     os.environ['PYTHONPATH'] = ''
-    env = launch._build_env('something')
+    env = launch._build_env(pathlib.Path('something'))
     assert env['PYTHONPATH'] == 'something'
 
     initial = os.pathsep.join(['something', 'else'])
     os.environ['PYTHONPATH'] = initial
-    env = launch._build_env('a')
+    env = launch._build_env(pathlib.Path('a'))
     expected = os.pathsep.join(['a', 'something', 'else'])
     assert env['PYTHONPATH'] == expected
 
 
-# protect against ResourceWarning (#56)
-@pytest.mark.filterwarnings("error")
-def test_build_env_includes_pth_files(tmpdir, clean_pythonpath):
+def test_build_env_includes_pth_files(tmp_path, clean_pythonpath):
     """
     If during _build_env, there are .pth files in the target directory,
     they should be processed to include any paths indicated there.
     See #6 for rationale.
     """
-    (tmpdir / 'foo.pth').write_text('pkg-1.0', encoding='utf-8')
-    env = launch._build_env(str(tmpdir))
-    expected = os.pathsep.join([str(tmpdir), str(tmpdir / 'pkg-1.0')])
+    (tmp_path / 'foo.pth').write_text('pkg-1.0', encoding='utf-8')
+    env = launch._build_env(tmp_path)
+    expected = os.pathsep.join([str(tmp_path), str(tmp_path / 'pkg-1.0')])
     assert env['PYTHONPATH'] == expected
```

### Comparing `pip-run-9.4.0/tests/test_scripts.py` & `pip-run-9.5.0/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pip-run-9.4.0/tox.ini` & `pip-run-9.5.0/tox.ini`

 * *Files identical despite different names*

