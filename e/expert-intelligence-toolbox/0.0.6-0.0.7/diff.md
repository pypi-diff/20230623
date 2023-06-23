# Comparing `tmp/expert_intelligence_toolbox-0.0.6.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.7.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.6.tar` & `expert_intelligence_toolbox-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/example.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/snowflake_connector.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/LICENSE
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/instructions.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/geographic.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/snowflake_connector.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/LICENSE
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/README.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/snowflake_connector.py` & `expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.6/LICENSE` & `expert_intelligence_toolbox-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.6/README.md` & `expert_intelligence_toolbox-0.0.7/instructions.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# expert_intelligence_toolbox
-This is an experimental v0.1, which currently serves no function other than testing.
-Hello update.
-
 ## Internal:
 Follow this:
 https://packaging.python.org/en/latest/tutorials/packaging-projects/
 
 A package needs:
 
 - pyproject.toml (used to define the metadata and configuration for your package. It provides information such as the package name, version, dependencies, and other details required for installation and distribution.)
@@ -17,14 +13,15 @@
 
 
 # How to get the package ready.
 
 **For Unix/MacOS**: see this https://packaging.python.org/en/latest/tutorials/packaging-projects/
 
 1 - Make a 'wheel' and source distribution file (you pack the source code as binary and tar file)
+`python3 -m pip install --upgrade build`
 `py -m pip install --upgrade build`
 `py -m build`
 
 2 - go to https://test.pypi.org/account/register/ and complete the steps on that page. Verify your email address.
 
 3 - To securely upload your project, you’ll need a PyPI API token. Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”. Don’t close the page until you have copied and saved the token — you won’t see that token again.
 
@@ -49,11 +46,20 @@
 `py -m build`
 `py -m twine upload dist/*`
 Username: __token__
 PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
 
 
 5 - What if you make any changes? Just repeat.
+
 Change version number in pyproject.toml
+
+Then, For Windows:
+`py -m pip install --upgrade build`
 `py -m build`
+Or, for Mac:
+`python3 -m pip install --upgrade build`
+`python3 -m build`
+
+Finally, for both:
 `twine upload --skip-existing dist/*`
 `twine upload --skip-existing --repository testpypi dist/*` (for testpypi)
```

### Comparing `expert_intelligence_toolbox-0.0.6/pyproject.toml` & `expert_intelligence_toolbox-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expert_intelligence_toolbox"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Arnold Kuersteiner", email="arnold.kuersteiner@expert-intelligence.com" },
+  { name="Pham Minh Ky", email="ky.pham@expert-intelligence.com" },
 ]
 description = "This is (for now) a test."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

