# Comparing `tmp/flowlang-0.0.4.tar.gz` & `tmp/flowlang-0.0.5.tar.gz`

## Comparing `flowlang-0.0.4.tar` & `flowlang-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,25 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/README.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/models/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/models/base.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/models/openai_model.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/scenarios/__init__.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/scenarios/base.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/base.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/__init__.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/apicall_step.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/control_step.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/summarization_step.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/translation_step.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/helpers/validation_step.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/required/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/required/end_step.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/core/steps/required/start_step.py
--rw-r--r--   0        0        0     9223 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/examples/scenarios_example.ipynb
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 flowlang-0.0.4/Flowlang/examples/steps_example.ipynb
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.4/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.4/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flowlang-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 flowlang-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/LICENSE
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/README.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/models/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/models/base.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/models/openai_model.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/scenarios/__init__.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/scenarios/base.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/base.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/apicall_step.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/control_step.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/summarization_step.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/translation_step.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/helpers/validation_step.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/required/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/required/end_step.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.5/Flowlang/core/steps/required/start_step.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.5/LICENSE
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.5/README.md
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 flowlang-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 flowlang-0.0.5/PKG-INFO
```

### Comparing `flowlang-0.0.4/Flowlang/LICENSE` & `flowlang-0.0.5/Flowlang/LICENSE`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/models/openai_model.py` & `flowlang-0.0.5/Flowlang/core/models/openai_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,19 @@
             ).get('choices')[0].get('message', {})
         except KeyError:
             response = {"error": "Key Error [0]. Do not have enough information."}
         result = {'message': response.get('content', "")}
         function_call = response.get('function_call')
         if function_call:
             function_name = function_call['name']
-            function_kwds = json.loads(function_call['arguments'].replace('\n', ''))
+            try:
+                function_kwds = json.loads(function_call['arguments'])
+            except json.JSONDecodeError:
+                function_kwds = dict()
+                print(function_call['arguments'])
             try:
                 function_response = functions[function_name](**function_kwds)
             except TypeError as ex:
                 function_response = str(ex)
             call_result = {'name': function_name, 'arguments': str(function_kwds)}
             result = {'result': function_response, 'function_call': str(call_result)}
             self.save_history(messages[-1], dict(role='assistant', content=function_response, function_call=str(call_result)))
```

### Comparing `flowlang-0.0.4/Flowlang/core/scenarios/base.py` & `flowlang-0.0.5/Flowlang/core/scenarios/base.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/base.py` & `flowlang-0.0.5/Flowlang/core/steps/base.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/helpers/apicall_step.py` & `flowlang-0.0.5/Flowlang/core/steps/helpers/apicall_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/helpers/control_step.py` & `flowlang-0.0.5/Flowlang/core/steps/helpers/control_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/helpers/summarization_step.py` & `flowlang-0.0.5/Flowlang/core/steps/helpers/summarization_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/helpers/translation_step.py` & `flowlang-0.0.5/Flowlang/core/steps/helpers/translation_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/Flowlang/core/steps/helpers/validation_step.py` & `flowlang-0.0.5/Flowlang/core/steps/helpers/validation_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/LICENSE` & `flowlang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.4/pyproject.toml` & `flowlang-0.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flowlang"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Egor Sheremetov", email="egorsheremetov3.0@gmail.com" },
 ]
 description = "An easy way to create and automate natural language processes and tasks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[tool.hatch.build]
+exclude = ["test_v4.ipynb", "test_data", "examples"]
+
 [project.urls]
 "Homepage" = "https://github.com/ESheremetov/Flowlang"
 "Bug Tracker" = "https://github.com/ESheremetov/Flowlang/issues"
```

### Comparing `flowlang-0.0.4/PKG-INFO` & `flowlang-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowlang
-Version: 0.0.4
+Version: 0.0.5
 Summary: An easy way to create and automate natural language processes and tasks.
 Project-URL: Homepage, https://github.com/ESheremetov/Flowlang
 Project-URL: Bug Tracker, https://github.com/ESheremetov/Flowlang/issues
 Author-email: Egor Sheremetov <egorsheremetov3.0@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

