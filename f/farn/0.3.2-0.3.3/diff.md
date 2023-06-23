# Comparing `tmp/farn-0.3.2.tar.gz` & `tmp/farn-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farn-0.3.2.tar", last modified: Thu May  4 15:05:02 2023, max compression
+gzip compressed data, was "farn-0.3.3.tar", last modified: Fri Jun 23 17:15:42 2023, max compression
```

## Comparing `farn-0.3.2.tar` & `farn-0.3.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 15:04:38.000000 farn-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:04:38.000000 farn-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-04 15:05:02.891667 farn-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-04 15:04:38.000000 farn-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 15:04:38.000000 farn-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 15:05:02.891667 farn-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.871667 farn-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.879667 farn-0.3.2/src/farn/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9418 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/cli/farn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn/core/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29786 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/farn.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/batchProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/cli/batchProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/subProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/sampling/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/src/farn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-04 15:04:38.000000 farn-0.3.2/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-05-04 15:04:38.000000 farn-0.3.2/tests/test_farn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-23 17:15:26.000000 farn-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 17:15:26.000000 farn-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-23 17:15:42.182458 farn-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-23 17:15:26.000000 farn-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-23 17:15:26.000000 farn-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-23 17:15:42.182458 farn-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.178458 farn-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.178458 farn-0.3.3/src/farn/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9418 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/cli/farn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14146 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/core/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30187 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/farn.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/batchProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/run/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/cli/batchProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/subProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/run/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/run/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/sampling/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 17:15:26.000000 farn-0.3.3/src/farn/utils/os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/src/farn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 17:15:42.000000 farn-0.3.3/src/farn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:15:42.182458 farn-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 17:15:26.000000 farn-0.3.3/tests/test_always_distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-06-23 17:15:26.000000 farn-0.3.3/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-06-23 17:15:26.000000 farn-0.3.3/tests/test_farn.py
```

### Comparing `farn-0.3.2/LICENSE` & `farn-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/PKG-INFO` & `farn-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.2
+Version: 0.3.3
 Summary: n-dimensional case generator.
 Home-page: https://dnv-opensource.github.io/farn/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
```

### Comparing `farn-0.3.2/README.md` & `farn-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/pyproject.toml` & `farn-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/setup.cfg` & `farn-0.3.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = farn
-version = 0.3.2
+version = 0.3.3
 summary = n-dimensional case generator.
 description = Python package to generate an n-dimensional case folder structure applying linear and spatial sampling strategies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://dnv-opensource.github.io/farn/README.html
 project_urls = 
 	GitHub = https://github.com/dnv-opensource/farn
@@ -45,16 +45,16 @@
 	scipy>=1.10
 	matplotlib>=3.7
 	pyDOE2>=1.3
 	Pillow>=9.5
 	psutil>=5.9
 	SALib>=1.4.7
 	sobol-seq>=0.2
-	dictIO>=0.2.7
-	ospx>=0.2.9
+	dictIO>=0.2.8
+	ospx>=0.2.10
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [options.entry_points]
```

### Comparing `farn-0.3.2/src/farn/cli/farn.py` & `farn-0.3.3/src/farn/cli/farn.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/core/case.py` & `farn-0.3.3/src/farn/core/case.py`

 * *Files 5% similar despite different names*

```diff
@@ -281,22 +281,26 @@
         series: Dict[str, Series] = {  # pyright: ignore
             "case": Series(data=None, dtype=np.dtype(str), name="case"),
             "path": Series(data=None, dtype=np.dtype(str), name="path"),
         }
 
         for _index, case in enumerate(_cases):
             if case.case:
-                series["case"].loc[_index] = case.case
-            series["path"].loc[_index] = str(case.path)
+                series["case"].loc[_index] = case.case  # pyright: ignore
+            series["path"].loc[_index] = str(case.path)  # pyright: ignore
             if case.parameters:
                 for parameter in case.parameters:
                     if parameter.name not in series:
-                        series[parameter.name] = Series(data=None, dtype=parameter.dtype, name=parameter.name)
+                        series[parameter.name] = Series(
+                            data=None,
+                            dtype=parameter.dtype,  # pyright: ignore
+                            name=parameter.name,
+                        )
                     if parameter.value is not None:
-                        series[parameter.name].loc[_index] = parameter.value
+                        series[parameter.name].loc[_index] = parameter.value  # pyright: ignore
 
         if parameters_only:
             _ = series.pop("case")
             if not use_path_as_index:
                 _ = series.pop("path")
 
         df_X = DataFrame(data=series)  # noqa: N806
```

### Comparing `farn-0.3.2/src/farn/core/parameter.py` & `farn-0.3.3/src/farn/core/parameter.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/farn.py` & `farn-0.3.3/src/farn/farn.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,20 @@
     -------
     Cases
         list of case objects representing all created cases.
     """
     log_msg: str = "List all valid cases.." if valid_only else "List all cases.."
     logger.info(log_msg)
 
+    # Check default distributions
+    default_distribution: Dict[str, Any] = {}
+
+    if "_always" in farn_dict:
+        default_distribution = farn_dict["_always"]
+
     # Check arguments.
     if "_layers" not in farn_dict:
         logger.error("create_cases: No '_layers' element contained in farn dict.")
         return Cases()
 
     # Initialize cases list
     cases: Cases = Cases()
@@ -303,14 +309,19 @@
                     f"The parameter {parameter_name} defined in layer {current_layer_name} had already been defined in a preceeding layer.\n"
                     f"The preceeding definition prevails. The samples for parameter {parameter_name} defined in layer {current_layer_name} are skipped. "
                 )
             else:
                 parameter_names_in_current_layer.append(parameter_name)
 
         user_variables_in_current_layer: MutableSequence[Parameter] = []
+        for key, item in default_distribution.items():
+            if not key.startswith("_"):
+                default_variable = Parameter(name=key, value=item)
+                user_variables_in_current_layer.append(default_variable)
+
         for key, item in current_layer.items():
             if not key.startswith("_"):
                 user_variable = Parameter(name=key, value=item)
                 if user_variable.name in parameter_names_used_in_preceeding_layers:
                     logger.warning(
                         f"The user variable {user_variable.name} defined in layer {current_layer_name} matches a parameter that\n"
                         f"had already been defined in a preceeding layer.\n"
```

### Comparing `farn-0.3.2/src/farn/run/batchProcess.py` & `farn-0.3.3/src/farn/run/batchProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/run/cli/batchProcess.py` & `farn-0.3.3/src/farn/run/cli/batchProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/run/subProcess.py` & `farn-0.3.3/src/farn/run/subProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/run/utils/threading.py` & `farn-0.3.3/src/farn/run/utils/threading.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn/sampling/sampling.py` & `farn-0.3.3/src/farn/sampling/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,24 +67,14 @@
                     "_ranges",
                     "_numberOfSamples",
                     "_distributionName",  # uniform|normal|exp... better to have a dedicated name in known_sampling_types
                     "_distributionParameters",  # mu|sigma|skew|camber not applicsble for uniform
                     "_includeBoundingBox",  # required
                 ]
             },
-            # "randNormal": {
-            #     "required_args": [
-            #         "_names",
-            #         "_ranges",
-            #         "_numberOfSamples",
-            #         "_mu",  # 1rst order
-            #         "_sigma",  # 2nd order
-            #         "_includeBoundingBox",
-            #     ]
-            # },
         }
 
     def set_sampling_type(self, sampling_type: str):
         """Set the sampling type.
 
         Valid values:
             "fixed"
@@ -373,15 +363,15 @@
         )
 
         return sample_set.T  # pyright: ignore
 
     def _generate_values_using_normal_lhs_sampling(self) -> ndarray[Any, Any]:
         """Gaussnormal LHS."""
         from pyDOE2 import lhs
-        from scipy.stats import norm  # qmc, truncnorm
+        from scipy.stats import norm  # type: ignore
 
         lhs_distribution: Union[ndarray[Any, Any], None] = lhs(
             self.number_of_fields,
             samples=self.number_of_samples - self.number_of_bb_samples,
             criterion="corr",
             random_state=None,
         )
```

### Comparing `farn-0.3.2/src/farn/utils/logging.py` & `farn-0.3.3/src/farn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/src/farn.egg-info/PKG-INFO` & `farn-0.3.3/src/farn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.2
+Version: 0.3.3
 Summary: n-dimensional case generator.
 Home-page: https://dnv-opensource.github.io/farn/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
```

### Comparing `farn-0.3.2/src/farn.egg-info/SOURCES.txt` & `farn-0.3.3/src/farn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 src/farn/run/utils/__init__.py
 src/farn/run/utils/threading.py
 src/farn/sampling/__init__.py
 src/farn/sampling/sampling.py
 src/farn/utils/__init__.py
 src/farn/utils/logging.py
 src/farn/utils/os.py
+tests/test_always_distribute.py
 tests/test_cases.py
 tests/test_farn.py
```

### Comparing `farn-0.3.2/tests/test_cases.py` & `farn-0.3.3/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.2/tests/test_farn.py` & `farn-0.3.3/tests/test_farn.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     assert Path("cases/layer1_1").exists()
     assert Path("cases/layer1_2").exists()
 
 
 # @TODO: There is nothing  actually asserted in this test. -> Frank to check.
 # CLAROS, 2022-05-13
 def test_execute(caplog: LogCaptureFixture):
+    # sourcery skip: no-conditionals-in-tests
     # Prepare
     farn_dict_file = Path("test_farnDict")
     sampled_file = Path(f"sampled.{farn_dict_file.name}")
     _ = run_farn(farn_dict_file, sample=True)
     _ = run_farn(sampled_file, generate=True)
     caplog.clear()
     # Execute
```

