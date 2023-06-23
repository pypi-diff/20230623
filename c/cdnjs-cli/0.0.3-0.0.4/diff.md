# Comparing `tmp/cdnjs_cli-0.0.3.tar.gz` & `tmp/cdnjs_cli-0.0.4.tar.gz`

## Comparing `cdnjs_cli-0.0.3.tar` & `cdnjs_cli-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/__main__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/cli.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/injector.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/logger.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/util.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/tests/test.html
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/.gitignore
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/README.md
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/__main__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/cli.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/injector.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/logger.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/src/cdnjs_cli/util.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/tests/test.html
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/README.md
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.4/PKG-INFO
```

### Comparing `cdnjs_cli-0.0.3/src/cdnjs_cli/cli.py` & `cdnjs_cli-0.0.4/src/cdnjs_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/src/cdnjs_cli/injector.py` & `cdnjs_cli-0.0.4/src/cdnjs_cli/injector.py`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/.gitignore` & `cdnjs_cli-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/LICENSE.txt` & `cdnjs_cli-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/README.md` & `cdnjs_cli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/pyproject.toml` & `cdnjs_cli-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.3/PKG-INFO` & `cdnjs_cli-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnjs-cli
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.3 Summary: CDNjs unofficial
+Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.4 Summary: CDNjs unofficial
 CLI tool. Project-URL: Documentation, https://github.com/woidzero/cdnjs-
 cli#readme Project-URL: Issues, https://github.com/woidzero/cdnjs-cli/issues
 Project-URL: Source, https://github.com/woidzero/cdnjs-cli Author-email:
 woidzero
 gmail.com> License-Expression: WTFPL License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

