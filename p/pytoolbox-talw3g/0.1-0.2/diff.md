# Comparing `tmp/pytoolbox_talw3g-0.1.tar.gz` & `tmp/pytoolbox_talw3g-0.2.tar.gz`

## Comparing `pytoolbox_talw3g-0.1.tar` & `pytoolbox_talw3g-0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/src/pytoolbox_talw3g/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/src/pytoolbox_talw3g/colortxt.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/src/pytoolbox_talw3g/confirm.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/LICENSE
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/README.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/pyproject.toml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/src/pytoolbox_talw3g/__init__.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/src/pytoolbox_talw3g/colortxt.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/src/pytoolbox_talw3g/confirm.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/LICENSE
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/README.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pytoolbox_talw3g-0.2/PKG-INFO
```

### Comparing `pytoolbox_talw3g-0.1/src/pytoolbox_talw3g/colortxt.py` & `pytoolbox_talw3g-0.2/src/pytoolbox_talw3g/colortxt.py`

 * *Files identical despite different names*

### Comparing `pytoolbox_talw3g-0.1/src/pytoolbox_talw3g/confirm.py` & `pytoolbox_talw3g-0.2/src/pytoolbox_talw3g/confirm.py`

 * *Files identical despite different names*

### Comparing `pytoolbox_talw3g-0.1/LICENSE` & `pytoolbox_talw3g-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytoolbox_talw3g-0.1/README.md` & `pytoolbox_talw3g-0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,21 +9,16 @@
 
   * **colortxt**: offers a convenient way to customize text with color, background and blink.
   * **confirm**: a dialog wrapper that asks for user's
   choice in the infamous *[Y/n], [y/N]* way.
 
 ## Installation
 
-Currently, only installation via Github is supported.
-
-#### Using Github:
 ```bash
-git clone https://github.com/Talw3g/pytoolbox
-cd pytoolbox
-sudo python3 setup.py install
+pip install pytoolbox-talw3g
 ```
 
 ## Usage
 
 ##### colortxt:
 ```python
 from pytoolbox import colortxt
```

### Comparing `pytoolbox_talw3g-0.1/pyproject.toml` & `pytoolbox_talw3g-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytoolbox_talw3g"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Thibault MARION", email="pytoolbox@otter.mozmail.com"},
 ]
 description = "A small package with useful simple tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pytoolbox_talw3g-0.1/PKG-INFO` & `pytoolbox_talw3g-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox_talw3g
-Version: 0.1
+Version: 0.2
 Summary: A small package with useful simple tools
 Project-URL: Homepage, https://github.com/Talw3g/pytoolbox
 Project-URL: Bug Tracker, https://github.com/Talw3g/pytoolbox/issues
 Author-email: Thibault MARION <pytoolbox@otter.mozmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,21 +23,16 @@
 
   * **colortxt**: offers a convenient way to customize text with color, background and blink.
   * **confirm**: a dialog wrapper that asks for user's
   choice in the infamous *[Y/n], [y/N]* way.
 
 ## Installation
 
-Currently, only installation via Github is supported.
-
-#### Using Github:
 ```bash
-git clone https://github.com/Talw3g/pytoolbox
-cd pytoolbox
-sudo python3 setup.py install
+pip install pytoolbox-talw3g
 ```
 
 ## Usage
 
 ##### colortxt:
 ```python
 from pytoolbox import colortxt
```

