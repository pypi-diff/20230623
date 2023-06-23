# Comparing `tmp/cdnjs_cli-0.0.1.tar.gz` & `tmp/cdnjs_cli-0.0.2.tar.gz`

## Comparing `cdnjs_cli-0.0.1.tar` & `cdnjs_cli-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/__main__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/cli.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/injector.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/logger.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/src/cdnjs_cli/util.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/tests/test.html
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/.gitignore
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/README.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/__about__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/__main__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/cli.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/injector.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/logger.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/util.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/tests/test.html
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/README.md
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/PKG-INFO
```

### Comparing `cdnjs_cli-0.0.1/src/cdnjs_cli/cli.py` & `cdnjs_cli-0.0.2/src/cdnjs_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present woidzero <woidzeroo@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 import click
 
-from cdnjs_cli.__about__ import __prog_name__, __version__
+from .__about__ import __prog_name__, __version__
 
 from .injector import add
 from .logger import Logger
 from .util import getLib
 
 
 @click.command(context_settings={"help_option_names": ["-h", "--help"]})
```

### Comparing `cdnjs_cli-0.0.1/src/cdnjs_cli/injector.py` & `cdnjs_cli-0.0.2/src/cdnjs_cli/injector.py`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.1/.gitignore` & `cdnjs_cli-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.1/LICENSE.txt` & `cdnjs_cli-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.1/README.md` & `cdnjs_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.1/pyproject.toml` & `cdnjs_cli-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.1/PKG-INFO` & `cdnjs_cli-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnjs-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: CDNjs unofficial CLI tool.
 Project-URL: Documentation, https://github.com/woidzero/cdnjs-cli#readme
 Project-URL: Issues, https://github.com/woidzero/cdnjs-cli/issues
 Project-URL: Source, https://github.com/woidzero/cdnjs-cli
 Author-email: woidzero <woidzeroo@gmail.com>
 License-Expression: WTFPL
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.1 Summary: CDNjs unofficial
+Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.2 Summary: CDNjs unofficial
 CLI tool. Project-URL: Documentation, https://github.com/woidzero/cdnjs-
 cli#readme Project-URL: Issues, https://github.com/woidzero/cdnjs-cli/issues
 Project-URL: Source, https://github.com/woidzero/cdnjs-cli Author-email:
 woidzero
 gmail.com> License-Expression: WTFPL License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

