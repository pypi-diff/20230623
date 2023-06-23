# Comparing `tmp/idefix_cli-2.2.0.tar.gz` & `tmp/idefix_cli-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.2.0.tar", last modified: Sat May  6 10:39:36 2023, max compression
+gzip compressed data, was "idefix_cli-2.3.0.tar", last modified: Fri Jun 23 09:41:04 2023, max compression
```

## Comparing `idefix_cli-2.2.0.tar` & `idefix_cli-2.3.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.695015 idefix_cli-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 09:41:04.000000 idefix_cli-2.3.0/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:41:04.699015 idefix_cli-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-23 09:40:55.000000 idefix_cli-2.3.0/tests/test_write.py
```

### Comparing `idefix_cli-2.2.0/LICENSE` & `idefix_cli-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/PKG-INFO` & `idefix_cli-2.3.0/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
-Name: idefix_cli
-Version: 2.2.0
+Name: idefix-cli
+Version: 2.3.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: isolated
 License-File: LICENSE
 
-[![PyPI](https://img.shields.io/pypi/v/idefix_cli)](https://pypi.org/project/idefix-cli/)
+[![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
 ![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
 [Idefix](https://github.com/idefix-code/idefix), written by
 [Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
```

### Comparing `idefix_cli-2.2.0/README.md` & `idefix_cli-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-[![PyPI](https://img.shields.io/pypi/v/idefix_cli)](https://pypi.org/project/idefix-cli/)
+[![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
 ![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
 [Idefix](https://github.com/idefix-code/idefix), written by
 [Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
```

### Comparing `idefix_cli-2.2.0/idefix_cli/__main__.py` & `idefix_cli-2.3.0/src/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_backports.py` & `idefix_cli-2.3.0/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/clean.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/clone.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/conf.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/read.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/run.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from multiprocessing import cpu_count
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from time import sleep, time
 from typing import Final
 
 import inifix
+from packaging.version import Version
 from rich.prompt import Confirm
 
 from idefix_cli.lib import (
     files_from_patterns,
     get_config_file,
+    get_idefix_version,
     get_option,
     print_err,
     print_subcommand,
     print_success,
     print_warning,
     requires_idefix,
     run_subcommand,
@@ -42,16 +44,19 @@
 MAIN_LOG_FILE = "idefix.0.log"
 TIME_INTEGRATOR_LOG_LINE = re.compile(
     "^TimeIntegrator:\\s*(?P<time>.+) \\|\\s*(?P<cycle>\\d+) \\|"
 )
 JOB_COMPLETED = re.compile("Main: Job completed")
 
 
-def spawn_idefix(cmd: list[str], *, step_count: int) -> int:
-    if step_count < 0:
+def _spawn_idefix_lt_1(cmd: list[str], *, ncycles: int) -> int:
+    if get_idefix_version() >= Version("1.0"):
+        raise RuntimeError("if you're seeing this error, please file a bug report")
+
+    if ncycles < 0:
         # infinite steps: simple call
         return subprocess.call(cmd)
 
     if sys.platform.startswith("win"):
         print_err("idfx run --one isn't supported on Windows")
         return -3
     else:
@@ -78,15 +83,15 @@
             with open(MAIN_LOG_FILE) as fh:
                 for line in fh:
                     if JOB_COMPLETED.match(line):
                         complete = True
                         break
                     if (match := TIME_INTEGRATOR_LOG_LINE.match(line)) is None:
                         continue
-                    if int(match["cycle"]) == step_count:
+                    if int(match["cycle"]) == ncycles:
                         prog.send_signal(SIGUSR2)
                         complete = True
                         break
             last_edit = new_edit
         sleep(0.01)
     return -1
 
@@ -138,14 +143,37 @@
 @requires_idefix()
 def build_idefix(directory) -> int:
     ncpus = 2 ** min(3, cpu_count().bit_length())
     cmd = ["make", "-j", str(ncpus)]
     return run_subcommand(cmd, loc=Path(directory), err="failed to build idefix")
 
 
+class MultipleMaxCycles(Exception):
+    pass
+
+
+def parse_ncycles(unknown_args: tuple[str, ...], ncycles: int) -> tuple[str, ...]:
+    if "-maxcycles" in unknown_args:
+        # it is assumed that this function is only called when --one is passed
+        raise MultipleMaxCycles
+
+    if get_idefix_version() >= Version("1.0"):
+        # -maxcycles is new in idefix 1.0.0
+        # we support older versions with a far more fragile implementation
+        # (see _spawn_idefix_lt_1)
+        if ncycles != 1:
+            print_warning(
+                "the --times option is deprecated. "
+                "Use idefix's -maxcycles argument instead."
+            )
+        return ("-maxcycles", str(ncycles), *unknown_args)
+    else:
+        return unknown_args
+
+
 def add_arguments(parser) -> None:
     parser.add_argument("--dir", dest="directory", default=".", help="target directory")
     parser.add_argument(
         "-i",
         dest="inifile",
         action="store",
         type=str,
@@ -168,15 +196,24 @@
     time_group = parser.add_mutually_exclusive_group()
     time_group.add_argument(
         "--one",
         "--one-step",
         dest="one_step",
         nargs="*",
         help="run only for one time step. "
-        "Accepts arbitrary output type name(s) (e.g. dmp or vtk).",
+        "Arguments are interpreted as output types (see --output)",
+    )
+    parser.add_argument(
+        "--out",
+        dest="outputs",
+        nargs="+",
+        help=(
+            "Output types (dmp, vtk, ...) to be produced on each cycle "
+            "(requires -maxcycles, cannot be combined with --one-step)"
+        ),
     )
     parser.add_argument(
         "--time-step",
         dest="time_step",
         action="store",
         type=float,
         help="override TimeIntegrator.first_dt",
@@ -190,43 +227,59 @@
             "run idefix in parallel over selected number of ALU. "
             "Requires the code to be configured for MPI. "
             "This parameter can be left unspecified if -dec is passed."
         ),
     )
     parser.add_argument(
         "--times",
-        dest="multiplier",
+        dest="ncycles",
         type=int,
         default=None,
-        help="multiplier for --one (use `--one --times 2` to run for 2 steps)",
+        help="ncycles for --one (use `--one --times 2` to run for 2 steps)",
     )
 
 
 def command(
     *unknown_args: str,
     directory: str = ".",
     inifile: str = "idefix.ini",
     tstop: float | None = None,
     duration: float | None = None,
     time_step: float | None = None,
     one_step: list[str] | None = None,
-    multiplier: int | None = None,
     nproc: int = -1,
+    ncycles: int | None = None,
+    outputs: list[str] | None = None,
 ) -> int:
-    if multiplier is not None:
-        if one_step is None:
+    if one_step is None:
+        if ncycles is not None:
             print_err(
-                "--times argument is invalid if --one/--one-step isn't passed too"
+                "the --times parameter is invalid if --one/--one-step isn't passed too"
             )
             return 1
-        if multiplier < 1:
+        ncycles = -1  # unlimited run
+    elif ncycles is not None:
+        if ncycles < 1:
             print_err(
-                f"--times argument expects a strictly positive integer (got {multiplier})"
+                "the --times parameter expects a strictly "
+                f"positive integer (got {ncycles})"
             )
             return 1
+        try:
+            unknown_args = parse_ncycles(unknown_args, ncycles=ncycles)
+        except MultipleMaxCycles:
+            print_err("-maxcycles cannot be combined with --one/--one-step")
+            return 1
+    else:
+        try:
+            unknown_args = parse_ncycles(unknown_args, ncycles=1)
+        except MultipleMaxCycles:
+            print_err("-maxcycles cannot be combined with --one/--one-step")
+            return 1
+        ncycles = -1  # unlimited run
 
     d = Path(directory).resolve()
     exe = d / "idefix"
     if not exe.is_file() and not (d / "Makefile").is_file():
         print_err(
             f"No idefix executable or Makefile found in the target directory {d} "
             "Run `idfx conf` first"
@@ -251,16 +304,27 @@
     if not isinstance(conf["TimeIntegrator"], dict):
         print_err(
             "configuration file seems malformed, "
             "expected 'TimeIntegrator' to be a section title, not a parameter name."
         )
         return 1
 
-    if one_step is not None:
-        output_types = set(one_step) - {"log"}
+    if outputs and "-maxcycles" not in unknown_args:
+        print_err("--out requires -maxcycles")
+        return 1
+    if outputs and one_step:
+        print_err(
+            "--one-step/--one cannot be followed by output "
+            "types if --out is also passed"
+        )
+        return 1
+    if one_step:
+        outputs = one_step
+    if outputs:
+        output_types = set(outputs) - {"log"}
         if time_step is None:
             conf["TimeIntegrator"].setdefault("first_dt", 1e-6)
             time_step = conf["TimeIntegrator"]["first_dt"]
 
         conf.setdefault("Output", {})
         output_sec = conf["Output"]
         if not isinstance(output_sec, dict):
@@ -272,16 +336,14 @@
 
         output_sec["log"] = 1
 
         if len(output_types) > 0:
             for entry in output_types:
                 output_sec[entry] = 0  # output on every time step
 
-    multiplier = multiplier or -1
-
     if time_step is not None:
         conf["TimeIntegrator"]["first_dt"] = time_step
     if duration is not None:
         print_warning("The --duration argument is deprecated. Use --tstop instead.")
         conf["TimeIntegrator"]["tstop"] = duration
     elif tstop is not None:
         conf["TimeIntegrator"]["tstop"] = tstop
@@ -367,35 +429,41 @@
         inputfile = tmp_inifile.name
     else:
         inputfile = str(pinifile.relative_to(d.resolve()))
 
     cmd = get_command(inputfile, nproc=nproc, idefix_args=unknown_args)
 
     print_subcommand(cmd, loc=d)
-    with chdir(d):
-        ret = spawn_idefix(cmd, step_count=multiplier)
+    if get_idefix_version() >= Version("1.0.0"):
+        with chdir(d):
+            ret = subprocess.call(cmd)
+
+        if ret == 0:
+            # Idefix >= 1.0 intentionally always returns 0, even on failure
+            with open(d / MAIN_LOG_FILE) as fh:
+                last_line = fh.read().strip().split("\n")[-1].strip()
+            if last_line in KNOWN_FAIL:
+                ret = 1
+            elif last_line not in KNOWN_SUCCESS:
+                print_warning(
+                    "Command completed with an unknown status. Please check log files."
+                )
 
-    if ret < 0:
-        # special retcodes from spawn_idefix
-        if ret == -1:
-            print_success("Sucessfully stopped idefix mid-air")
-        elif ret == -2:
-            print_err("idefix timed out (startup took more than a minute)")
-        elif ret == -3:
-            # unsupported operation
-            ret = 1
-        ret = 0
-    elif ret == 0:
-        # Idefix newer than 1.0 intentionally always returns 0, even on failure
-        with open(d / MAIN_LOG_FILE) as fh:
-            last_line = fh.read().strip().split("\n")[-1].strip()
-        if last_line in KNOWN_FAIL:
-            ret = 1
-        elif last_line not in KNOWN_SUCCESS:
-            print_warning(
-                "Command completed with an unknown status. Please check log files."
-            )
+    else:
+        with chdir(d):
+            ret = _spawn_idefix_lt_1(cmd, ncycles=ncycles)
+
+        if ret < 0:
+            # special retcodes from spawn_idefix
+            if ret == -1:
+                print_success("Sucessfully stopped idefix mid-air")
+            elif ret == -2:
+                print_err("idefix timed out (startup took more than a minute)")
+            elif ret == -3:
+                # unsupported operation
+                ret = 1
+            ret = 0
 
     if ret != 0:
         print_err(f"{cmd[0]} terminated with an error")
 
     return ret
```

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/stamp.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/switch.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/_commands/write.py` & `idefix_cli-2.3.0/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli/lib.py` & `idefix_cli-2.3.0/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
-Name: idefix-cli
-Version: 2.2.0
+Name: idefix_cli
+Version: 2.3.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: isolated
 License-File: LICENSE
 
-[![PyPI](https://img.shields.io/pypi/v/idefix_cli)](https://pypi.org/project/idefix-cli/)
+[![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
 ![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
 [Idefix](https://github.com/idefix-code/idefix), written by
 [Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
```

### Comparing `idefix_cli-2.2.0/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.3.0/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
-idefix_cli/__init__.py
-idefix_cli/__main__.py
-idefix_cli/_backports.py
-idefix_cli/_theme.py
-idefix_cli/lib.py
-idefix_cli.egg-info/PKG-INFO
-idefix_cli.egg-info/SOURCES.txt
-idefix_cli.egg-info/dependency_links.txt
-idefix_cli.egg-info/entry_points.txt
-idefix_cli.egg-info/requires.txt
-idefix_cli.egg-info/top_level.txt
-idefix_cli/_commands/__init__.py
-idefix_cli/_commands/clean.py
-idefix_cli/_commands/clone.py
-idefix_cli/_commands/conf.py
-idefix_cli/_commands/read.py
-idefix_cli/_commands/run.py
-idefix_cli/_commands/stamp.py
-idefix_cli/_commands/switch.py
-idefix_cli/_commands/write.py
+src/idefix_cli/__init__.py
+src/idefix_cli/__main__.py
+src/idefix_cli/_backports.py
+src/idefix_cli/_theme.py
+src/idefix_cli/lib.py
+src/idefix_cli.egg-info/PKG-INFO
+src/idefix_cli.egg-info/SOURCES.txt
+src/idefix_cli.egg-info/dependency_links.txt
+src/idefix_cli.egg-info/entry_points.txt
+src/idefix_cli.egg-info/requires.txt
+src/idefix_cli.egg-info/top_level.txt
+src/idefix_cli/_commands/__init__.py
+src/idefix_cli/_commands/clean.py
+src/idefix_cli/_commands/clone.py
+src/idefix_cli/_commands/conf.py
+src/idefix_cli/_commands/read.py
+src/idefix_cli/_commands/run.py
+src/idefix_cli/_commands/stamp.py
+src/idefix_cli/_commands/switch.py
+src/idefix_cli/_commands/write.py
 tests/test_app_structure.py
 tests/test_clean.py
 tests/test_clone.py
 tests/test_commons.py
 tests/test_conf.py
 tests/test_lib.py
 tests/test_read.py
```

### Comparing `idefix_cli-2.2.0/pyproject.toml` & `idefix_cli-2.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "2.2.0"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
@@ -19,14 +18,15 @@
 dependencies = [
     "gitpython>=3.1.18",
     "inifix>=3.0.0",
     "packaging>=21.0",
     "rich>=10.7.0",
     "typing-extensions>=4.1.0;python_version < '3.11'",
 ]
+dynamic = ["version"]
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 isolated = [
     "gitpython==3.1.18",
@@ -49,38 +49,42 @@
 
 [tool.setuptools]
 license-files = [
     "LICENSE",
 ]
 include-package-data = false
 
+[tool.setuptools.dynamic]
+ version = {attr = "idefix_cli.__version__"}
+
 [tool.setuptools.packages.find]
-exclude = [
-    "tests*",
-    "testing*",
-]
+where = ["src"]
 namespaces = false
 
 [tool.black]
 line-length = 88
 
 [tool.ruff]
 exclude = ["*__init__.py"]
 ignore = ["E501"]
 select = [
     "E",
     "F",
     "W",
-    "B",
-    "I",
-    "UP",
+    "C4",  # flake8-comprehensions
+    "B",   # flake8-bugbear
+    "YTT", # flake8-2020
+    "ISC", # flake8-implicit-string-concatenation
+    "I",   # isort
+    "UP",  # pyupgrade
 ]
 
 [tool.ruff.isort]
 combine-as-imports = true
+known-first-party = ["idefix_cli"]
 
 [tool.mypy]
 python_version = 3.8
 show_error_codes = true
 ignore_missing_imports = true
 warn_unused_configs = true
 warn_unused_ignores = true
```

### Comparing `idefix_cli-2.2.0/tests/test_app_structure.py` & `idefix_cli-2.3.0/tests/test_app_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @pytest.mark.skipif(
     sys.platform.startswith("win"), reason="plugin system tests are broken on windows"
 )
 @pytest.mark.parametrize(
     "content, msg",
     (
-        (("\n"), " is missing required functions " "'command' and 'add_arguments'"),
+        (("\n"), " is missing required functions 'command' and 'add_arguments'"),
         (
             ("def add_arguments():\n", "    return\n"),
             " is missing a 'command' function",
         ),
         (
             ("def command():\n", "    return\n"),
             " is missing a 'add_arguments' function",
```

### Comparing `idefix_cli-2.2.0/tests/test_clean.py` & `idefix_cli-2.3.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_clone.py` & `idefix_cli-2.3.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_commons.py` & `idefix_cli-2.3.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_conf.py` & `idefix_cli-2.3.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_read.py` & `idefix_cli-2.3.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_run.py` & `idefix_cli-2.3.0/tests/test_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,28 @@
 
 
 def test_times_without_one_step(capsys):
     ret = main(["run", "--times", "1"])
     assert ret != 0
     out, err = capsys.readouterr()
     assert out == ""
-    assert err == "💥 --times argument is invalid if --one/--one-step isn't passed too\n"
+    assert err == (
+        "💥 the --times parameter is invalid if --one/--one-step isn't passed too\n"
+    )
 
 
-def test_negative_multiplier(capsys):
+def test_negative_times(capsys):
     ret = main(["run", "--one", "--times", "-1"])
     assert ret != 0
     out, err = capsys.readouterr()
     assert out == ""
-    assert err == "💥 --times argument expects a strictly positive integer (got -1)\n"
+    assert err == (
+        "💥 the --times parameter expects a strictly positive integer (got -1)\n"
+    )
+
+
+def test_one_and_maxncycles(capsys):
+    ret = main(["run", "--one", "-maxcycles", "1"])
+    assert ret != 0
+    out, err = capsys.readouterr()
+    assert out == ""
+    assert err == "💥 -maxcycles cannot be combined with --one/--one-step\n"
```

### Comparing `idefix_cli-2.2.0/tests/test_stamp.py` & `idefix_cli-2.3.0/tests/test_stamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     ret = main(["stamp"])
     with check:
         assert ret == 0
     out, err = capsys.readouterr()
     # skiping the last line as it contains a date and I'm not sure how to test it.
     with check:
-        assert out.splitlines()[:-1] == [v for v in mock_data.values()]
+        assert out.splitlines()[:-1] == list(mock_data.values())
     with check:
         assert err == ""
 
 
 @pytest.mark.parametrize("flag", ["-d", "--json"])
 def test_stamp_json(flag, capsys, monkeypatch, tmp_path):
     monkeypatch.setenv("IDEFIX_DIR", str(tmp_path))
```

### Comparing `idefix_cli-2.2.0/tests/test_ux.py` & `idefix_cli-2.3.0/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.2.0/tests/test_write.py` & `idefix_cli-2.3.0/tests/test_write.py`

 * *Files identical despite different names*

