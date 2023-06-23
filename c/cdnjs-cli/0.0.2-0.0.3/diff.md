# Comparing `tmp/cdnjs_cli-0.0.2.tar.gz` & `tmp/cdnjs_cli-0.0.3.tar.gz`

## Comparing `cdnjs_cli-0.0.2.tar` & `cdnjs_cli-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/__main__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/cli.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/injector.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/logger.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/src/cdnjs_cli/util.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/tests/test.html
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/.gitignore
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/README.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/__main__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/cli.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/injector.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/logger.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/src/cdnjs_cli/util.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/tests/test.html
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/README.md
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cdnjs_cli-0.0.3/PKG-INFO
```

### Comparing `cdnjs_cli-0.0.2/src/cdnjs_cli/cli.py` & `cdnjs_cli-0.0.3/src/cdnjs_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 #
 # SPDX-License-Identifier: MIT
 
 import click
 
 from .__about__ import __prog_name__, __version__
 
-from .injector import add
+from .injector import addTag
 from .logger import Logger
 from .util import getLib
 
 
 @click.command(context_settings={"help_option_names": ["-h", "--help"]})
 @click.argument("file")
 @click.argument("lib")
 @click.version_option(version=__version__, prog_name=__prog_name__)
 def cdnjs(file, lib):
     src = getLib(lib)
 
     if src == -1:
         return Logger.error(f"No library named `{lib}` found.")
 
-    add(src, file)
+    addTag(src, file)
     Logger.success(f"Added `{lib}` to a `{file}`.")
```

### Comparing `cdnjs_cli-0.0.2/src/cdnjs_cli/injector.py` & `cdnjs_cli-0.0.3/src/cdnjs_cli/injector.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 
 def inject(file, content):
     with open(file, "w") as f:
         f.writelines(content)
 
 
-def add(src, file):
+def addTag(src, file):
     with open(file, "r") as f:
         content = f.readlines()
 
     tag = f"<script src='{src}'></script>"
     body_end_index = -1
 
     for i, line in enumerate(content):
         if line.strip() == "</body>":
             body_end_index = i
             break
         elif line.strip() == "<body></body>":
             content[i] = "<body>\n\n</body>\n"
             inject(file, content)
-            add(src, file=file)
+            addTag(src, file=file)
             return
 
     if body_end_index == -1:
         raise ValueError("The HTML file does not contain a closing </body> tag.")
 
     previous_line_indentation = ""
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # SPDX-FileCopyrightText: 2023-present woidzero
 gmail.com> # # SPDX-License-Identifier: MIT def inject(file, content): with
-open(file, "w") as f: f.writelines(content) def add(src, file): with open(file,
-"r") as f: content = f.readlines() tag = f"
+open(file, "w") as f: f.writelines(content) def addTag(src, file): with open
+(file, "r") as f: content = f.readlines() tag = f"
 " body_end_index = -1 for i, line in enumerate(content): if line.strip() == "
 ": body_end_index = i break elif line.strip() == "
 ": content[i] = "
 \n\n
-\n" inject(file, content) add(src, file=file) return if body_end_index == -1:
-raise ValueError("The HTML file does not contain a closing
+\n" inject(file, content) addTag(src, file=file) return if body_end_index == -
+1: raise ValueError("The HTML file does not contain a closing
 tag.") previous_line_indentation = "" if body_end_index > 0: previous_line =
 content[body_end_index - 1] if previous_line.strip() != "":
 previous_line_indentation = previous_line[: len(previous_line) - len
 (previous_line.lstrip())] if previous_line_indentation == "":
 previous_line_indentation = "\t" tag = previous_line_indentation + tag + "\n"
 content.insert(body_end_index, tag) inject(file, content)
```

### Comparing `cdnjs_cli-0.0.2/.gitignore` & `cdnjs_cli-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.2/LICENSE.txt` & `cdnjs_cli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.2/README.md` & `cdnjs_cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cdnjs_cli-0.0.2/pyproject.toml` & `cdnjs_cli-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [project.urls]
 Documentation = "https://github.com/woidzero/cdnjs-cli#readme"
 Issues = "https://github.com/woidzero/cdnjs-cli/issues"
 Source = "https://github.com/woidzero/cdnjs-cli"
 
 [project.scripts]
-cdnjs = "cdnjs_cli.__main__:main"
+cdnjs = "src.cdnjs_cli.__main__:main"
 
 [tool.hatch.version]
 path = "src/cdnjs_cli/__about__.py"
 
 [tool.black]
 target-version = ["py311"]
 line-length = 120
```

### Comparing `cdnjs_cli-0.0.2/PKG-INFO` & `cdnjs_cli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnjs-cli
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.2 Summary: CDNjs unofficial
+Metadata-Version: 2.1 Name: cdnjs-cli Version: 0.0.3 Summary: CDNjs unofficial
 CLI tool. Project-URL: Documentation, https://github.com/woidzero/cdnjs-
 cli#readme Project-URL: Issues, https://github.com/woidzero/cdnjs-cli/issues
 Project-URL: Source, https://github.com/woidzero/cdnjs-cli Author-email:
 woidzero
 gmail.com> License-Expression: WTFPL License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

