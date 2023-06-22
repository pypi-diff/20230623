# Comparing `tmp/function-analyser-0.0.8.tar.gz` & `tmp/function-analyser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-analyser-0.0.8.tar", last modified: Thu Jun 22 10:54:27 2023, max compression
+gzip compressed data, was "function-analyser-0.0.9.tar", last modified: Thu Jun 22 16:03:58 2023, max compression
```

## Comparing `function-analyser-0.0.8.tar` & `function-analyser-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 10:53:55.000000 function-analyser-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:54:26.994257 function-analyser-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 10:53:55.000000 function-analyser-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 10:54:16.000000 function-analyser-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:54:26.994257 function-analyser-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/function_analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/function_analyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:58.969552 function-analyser-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 16:03:46.000000 function-analyser-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 16:03:58.969552 function-analyser-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 16:03:46.000000 function-analyser-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 16:03:51.000000 function-analyser-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:03:58.969552 function-analyser-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:58.969552 function-analyser-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:58.969552 function-analyser-0.0.9/src/function_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:46.000000 function-analyser-0.0.9/src/function_analyser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 16:03:46.000000 function-analyser-0.0.9/src/function_analyser/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 16:03:46.000000 function-analyser-0.0.9/src/function_analyser/missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-22 16:03:46.000000 function-analyser-0.0.9/src/function_analyser/parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-22 16:03:46.000000 function-analyser-0.0.9/src/function_analyser/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:58.969552 function-analyser-0.0.9/src/function_analyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 16:03:58.000000 function-analyser-0.0.9/src/function_analyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 16:03:58.000000 function-analyser-0.0.9/src/function_analyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:03:58.000000 function-analyser-0.0.9/src/function_analyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 16:03:58.000000 function-analyser-0.0.9/src/function_analyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 16:03:58.000000 function-analyser-0.0.9/src/function_analyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:03:58.969552 function-analyser-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 16:03:46.000000 function-analyser-0.0.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 16:03:46.000000 function-analyser-0.0.9/tests/test_missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-22 16:03:46.000000 function-analyser-0.0.9/tests/test_parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-22 16:03:46.000000 function-analyser-0.0.9/tests/test_statistics.py
```

### Comparing `function-analyser-0.0.8/LICENSE.txt` & `function-analyser-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.8/PKG-INFO` & `function-analyser-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `function-analyser-0.0.8/README.md` & `function-analyser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.8/pyproject.toml` & `function-analyser-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "function-analyser"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = '0.0.8'  # Required
+version = '0.0.9'  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Identify long functions to refactor with this function analyser"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `function-analyser-0.0.8/src/function_analyser/main.py` & `function-analyser-0.0.9/src/function_analyser/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
+import pathlib
 
-from parse_function import parse_files
+from function_analyser.parse_function import parse_files
 from function_analyser.statistics import get_statistics, filter_by_percentile
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Function analysis')
     parser.add_argument('-f', '--filepath', help='Source file path to analyse', required=False)
     args = vars(parser.parse_args())
```

### Comparing `function-analyser-0.0.8/src/function_analyser/parse_function.py` & `function-analyser-0.0.9/src/function_analyser/parse_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,42 @@
 
 def get_function_length(function_def: ast.FunctionDef):
     """
     return the length of an ast functiondef node
     :param function_def:
     :return: int
     """
-    return function_def.end_lineno - function_def.lineno
+    try:
+        function_length = int(function_def.end_lineno - function_def.lineno)
+    except Exception as e:
+        # not an integer ...
+        return None
+
+    return function_length
 
 
 def parse_functions(tree):
     """
     Parse functions in an AST tree
     :param tree:
     :return:
     """
     function_names = []
     function_lengths = []
-    parameter_count = []
+    parameter_counts = []
     functions = [n for n in tree.body if isinstance(n, ast.FunctionDef)]
     for node in functions:
-        function_names.append(node.name)
-        parameter_count.append(len(node.args.args))
-        function_lengths.append(get_function_length(node))
+        parameter_count = len(node.args.args)
+        function_length = get_function_length(node)
+        if function_length and parameter_count:
+            function_names.append(node.name)
+            parameter_counts.append(parameter_count)
+            function_lengths.append(function_length)
 
-    return {"function_names": function_names, FUNCTION_LENGTHS: function_lengths, PARAMETER_COUNT: parameter_count}
+    return {"function_names": function_names, FUNCTION_LENGTHS: function_lengths, PARAMETER_COUNT: parameter_counts}
 
 
 def parse_classes(tree):
     """
     Parse the classes in an AST tree
     :param tree:
     :return:
@@ -60,24 +69,25 @@
     Parse files
 
     :param file_path:
     :param file_type:
     :param threshold:
     :return:
     """
-    print(f"Parsing source files in {file_path} ...")
+    file_path2 = os.path.join(file_path, "**", file_type)
+    file_list = glob.glob(file_path2, recursive=True)
 
-    file_path = os.path.join(file_path, file_type)
-    # recurse into sub-folders ...
-    file_list = glob.glob(file_path, recursive=True)
+    print(f"Parsing {len(file_list)} source files in {file_path} ...")
 
     d = {}
     for file_item in file_list:
         with open(file_item) as file:
             file_series_list = parse_file(file)
+            if file_series_list is None:
+                continue
             for series in file_series_list:
                 series_by_type = d.get(series.type)
                 if isinstance(series_by_type, Series):
                     new_series = pandas.concat([series_by_type, series])
                     new_series.type = series.type
                     d[series.type] = new_series
                 else:
@@ -111,15 +121,20 @@
     Pass in a file and yield function lengths
     :param file:
     :param function_length_threshold
     :param parameter_count_threshold
     :return:
     """
     # parse the file ...
-    tree = ast.parse(file.read())
+    try:
+        tree = ast.parse(file.read())
+    except (SyntaxError, UnicodeDecodeError) as e:
+        print(f"Unable to parse file {file}, {e}")
+        return None
+
     d1 = parse_functions(tree)
     d2 = parse_classes(tree)
 
     # concatenate the lists ...
     function_names = [*d1["function_names"], *d2["function_names"]]
     function_lengths = [*d1[FUNCTION_LENGTHS], *d2[FUNCTION_LENGTHS]]
     parameter_count = [*d1[PARAMETER_COUNT], *d2[PARAMETER_COUNT]]
```

### Comparing `function-analyser-0.0.8/src/function_analyser/statistics.py` & `function-analyser-0.0.9/src/function_analyser/statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas
 
-from parse_function import FUNCTION_LENGTHS, PARAMETER_COUNT
+from function_analyser.parse_function import FUNCTION_LENGTHS, PARAMETER_COUNT
 
 
 def get_mean(series):
     mean = series.mean()
     if mean is np.nan:
         mean = None
     else:
@@ -109,13 +109,13 @@
     """
     series = series.loc[lambda x: x > np.percentile(x, percentile)]
     # TODO - use the old type as suffix ...
     series.type = "percentile_" + str(percentile)
     return series
 
 
-def filter_by_percentile(series_list, percentile=95):
+def filter_by_percentile(series_list, percentile=99):
     series_list2 = []
     for series in series_list:
         series = filter_series_by_percentile(series, percentile)
         series_list2.append(series)
     return series_list2
```

### Comparing `function-analyser-0.0.8/src/function_analyser.egg-info/PKG-INFO` & `function-analyser-0.0.9/src/function_analyser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `function-analyser-0.0.8/src/function_analyser.egg-info/SOURCES.txt` & `function-analyser-0.0.9/src/function_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.8/tests/test_missing_docstring.py` & `function-analyser-0.0.9/tests/test_missing_docstring.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.8/tests/test_parse_function.py` & `function-analyser-0.0.9/tests/test_parse_function.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.8/tests/test_statistics.py` & `function-analyser-0.0.9/tests/test_statistics.py`

 * *Files identical despite different names*

