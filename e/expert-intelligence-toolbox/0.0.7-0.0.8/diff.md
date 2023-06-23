# Comparing `tmp/expert_intelligence_toolbox-0.0.7.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.8.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.7.tar` & `expert_intelligence_toolbox-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/instructions.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/example.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/geographic.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/snowflake_connector.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/LICENSE
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/instructions.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/geographic.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/snowflake_connector.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/LICENSE
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/README.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.7/instructions.md` & `expert_intelligence_toolbox-0.0.8/instructions.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,23 @@
 `py -m pip install --upgrade build`
 `py -m build`
 
 2 - go to https://test.pypi.org/account/register/ and complete the steps on that page. Verify your email address.
 
 3 - To securely upload your project, you’ll need a PyPI API token. Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”. Don’t close the page until you have copied and saved the token — you won’t see that token again.
 
-4 - Upload to PyPI test index
+4 - Upload to PyPI test index (windows)
 `py -m pip install --upgrade twine`
 `py -m twine upload --repository testpypi dist/*`
+
+4 - Upload to PyPI test index (Mac)
+`python3 -m pip install --upgrade twine`
+`python3 -m twine upload --repository testpypi dist/*`
+
+
 Username: __token__
 PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
 **Note**: 
 - Be carefull to check whether you're using the `pypi` or `test.pypi` to access the package.
 This tutorial is for `test.pypi`, so if you're using `pypi`, please change from `--repository testpypi` into `--repository pypi`
 - If you can't not get to the package using `API key`, using (not recommend, may cause leak private information)
 ```bash
@@ -57,9 +63,9 @@
 `py -m pip install --upgrade build`
 `py -m build`
 Or, for Mac:
 `python3 -m pip install --upgrade build`
 `python3 -m build`
 
 Finally, for both:
-`twine upload --skip-existing dist/*`
+`twine upload --skip-existing dist/*` (for real package)
 `twine upload --skip-existing --repository testpypi dist/*` (for testpypi)
```

### Comparing `expert_intelligence_toolbox-0.0.7/src/expert_intelligence_toolbox/snowflake_connector.py` & `expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.7/LICENSE` & `expert_intelligence_toolbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.7/pyproject.toml` & `expert_intelligence_toolbox-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expert_intelligence_toolbox"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Arnold Kuersteiner", email="arnold.kuersteiner@expert-intelligence.com" },
   { name="Pham Minh Ky", email="ky.pham@expert-intelligence.com" },
 ]
 description = "This is (for now) a test."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `expert_intelligence_toolbox-0.0.7/PKG-INFO` & `expert_intelligence_toolbox-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expert_intelligence_toolbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is (for now) a test.
 Project-URL: Homepage, https://github.com/Point-Topic/expert_intelligence_toolbox
 Project-URL: Bug Tracker, https://github.com/Point-Topic/expert_intelligence_toolbox/issues
 Author-email: Arnold Kuersteiner <arnold.kuersteiner@expert-intelligence.com>, Pham Minh Ky <ky.pham@expert-intelligence.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

