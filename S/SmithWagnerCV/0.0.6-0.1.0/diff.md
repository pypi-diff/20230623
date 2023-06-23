# Comparing `tmp/smithwagnercv-0.0.6.tar.gz` & `tmp/smithwagnercv-0.1.0.tar.gz`

## Comparing `smithwagnercv-0.0.6.tar` & `smithwagnercv-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/.DS_Store
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/Methods.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/LICENSE
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/README.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/src/SmithWagnerCV/.DS_Store
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/src/SmithWagnerCV/Methods.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/src/SmithWagnerCV/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/LICENSE
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/README.md
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 smithwagnercv-0.1.0/PKG-INFO
```

### Comparing `smithwagnercv-0.0.6/src/SmithWagnerCV/.DS_Store` & `smithwagnercv-0.1.0/src/SmithWagnerCV/.DS_Store`

 * *Files identical despite different names*

### Comparing `smithwagnercv-0.0.6/src/SmithWagnerCV/Methods.py` & `smithwagnercv-0.1.0/src/SmithWagnerCV/Methods.py`

 * *Files identical despite different names*

### Comparing `smithwagnercv-0.0.6/.gitignore` & `smithwagnercv-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `smithwagnercv-0.0.6/LICENSE` & `smithwagnercv-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smithwagnercv-0.0.6/README.md` & `smithwagnercv-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `smithwagnercv-0.0.6/pyproject.toml` & `smithwagnercv-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SmithWagnerCV"
-version = "0.0.6"
+version = "0.1.0"
 description = "Produces critical values for value-added learning scores proposed in Smith and Wagner (2018) through Monte Carlo simulations."
 license = "MIT"
 authors = [
   { name="Ben Smith", email="bosmith@unomaha.edu" },
 ]
 maintainers = [
   { name="Ben Smith", email="bosmith@unomaha.edu" },
@@ -31,8 +31,8 @@
     "numpy>=1.21.0",
     "pandas>=1.3.0",
     "tqdm>=4.26.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tazzben/SmithWagnerCV"
-"Bug Tracker" = "https://github.com/tazzben/SmithWagnerCV"
+"Bug Tracker" = "https://github.com/tazzben/SmithWagnerCV/issues"
```

### Comparing `smithwagnercv-0.0.6/PKG-INFO` & `smithwagnercv-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SmithWagnerCV
-Version: 0.0.6
+Version: 0.1.0
 Summary: Produces critical values for value-added learning scores proposed in Smith and Wagner (2018) through Monte Carlo simulations.
 Project-URL: Homepage, https://github.com/tazzben/SmithWagnerCV
-Project-URL: Bug Tracker, https://github.com/tazzben/SmithWagnerCV
+Project-URL: Bug Tracker, https://github.com/tazzben/SmithWagnerCV/issues
 Author-email: Ben Smith <bosmith@unomaha.edu>
 Maintainer-email: Ben Smith <bosmith@unomaha.edu>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Monte Carlo,Statistics,Value-added Learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

