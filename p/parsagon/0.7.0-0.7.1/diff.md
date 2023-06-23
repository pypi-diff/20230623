# Comparing `tmp/parsagon-0.7.0.tar.gz` & `tmp/parsagon-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.0.tar", last modified: Wed Jun 21 21:20:22 2023, max compression
+gzip compressed data, was "parsagon-0.7.1.tar", last modified: Fri Jun 23 09:51:50 2023, max compression
```

## Comparing `parsagon-0.7.0.tar` & `parsagon-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.822281 parsagon-0.7.0/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-21 21:20:22.821592 parsagon-0.7.0/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.0/README.md
--rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-21 07:48:34.000000 parsagon-0.7.0/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-21 21:20:22.822496 parsagon-0.7.0/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.810031 parsagon-0.7.0/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.0/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.816205 parsagon-0.7.0/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.7.0/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.7.0/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.0/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010    10507 2023-06-21 19:40:39.000000 parsagon-0.7.0/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     6683 2023-06-21 20:28:30.000000 parsagon-0.7.0/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.0/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.820764 parsagon-0.7.0/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.0/src/parsagon/tests/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-21 21:20:22.819899 parsagon-0.7.0/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-21 21:20:22.000000 parsagon-0.7.0/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.884628 parsagon-0.7.1/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-23 09:51:50.884159 parsagon-0.7.1/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.1/README.md
+-rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-23 09:51:06.000000 parsagon-0.7.1/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-23 09:51:50.884807 parsagon-0.7.1/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.872076 parsagon-0.7.1/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.1/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.877690 parsagon-0.7.1/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.7.1/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.7.1/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.1/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010    10224 2023-06-23 09:50:27.000000 parsagon-0.7.1/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     6683 2023-06-21 21:23:22.000000 parsagon-0.7.1/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.1/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.883661 parsagon-0.7.1/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.1/src/parsagon/tests/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.882817 parsagon-0.7.1/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.0/PKG-INFO` & `parsagon-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.0/README.md` & `parsagon-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.0/pyproject.toml` & `parsagon-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.0"
+version = "0.7.1"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.7.0/src/parsagon/api.py` & `parsagon-0.7.1/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.0/src/parsagon/custom_function.py` & `parsagon-0.7.1/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.0/src/parsagon/executor.py` & `parsagon-0.7.1/src/parsagon/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,17 @@
         else:
             self.custom_functions[call_id] = custom_function
 
     def mark_html(self):
         """
         Adds node IDs to elements on the current page that don't already have IDs.
         """
-        # new_max_elem_id = self.driver.execute_script(
-        # f"let elemIdx = {self.max_elem_id}; for (const node of document.querySelectorAll(':not([data-psgn-id]):not(style)')) {{ node.setAttribute('data-psgn-id', elemIdx); elemIdx++; }} return elemIdx;"
-        # )
-        # self.max_elem_id = new_max_elem_id
         logger.debug("  Marking HTML...")
-        self.driver.execute_script(
-            "let elemIdx = 0; for (const node of document.all) { node.setAttribute('data-psgn-id', elemIdx); elemIdx++; }"
+        self.max_elem_id = self.driver.execute_script(
+            "let elemIdx = 0; for (const node of document.all) { node.setAttribute('data-psgn-id', elemIdx); elemIdx++; } return elemIdx;"
         )
         self.driver.execute_script(
             "for (const image of document.images) { image.setAttribute('data-psgn-width', image.width ?? -1); image.setAttribute('data-psgn-height', image.height ?? -1); }"
         )
 
     def _get_cleaned_lxml_root(self):
         driver = self.driver
```

### Comparing `parsagon-0.7.0/src/parsagon/main.py` & `parsagon-0.7.1/src/parsagon/main.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.0/src/parsagon/settings.py` & `parsagon-0.7.1/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.0/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.1/src/parsagon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

