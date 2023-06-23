# Comparing `tmp/flowlang-0.0.2.tar.gz` & `tmp/flowlang-0.0.3.tar.gz`

## Comparing `flowlang-0.0.2.tar` & `flowlang-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/models/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/models/base.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/models/openai_model.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/scenarios/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/scenarios/base.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/base.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/__init__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/apicall_step.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/control_step.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/summarization_step.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/translation_step.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/helpers/validation_step.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/required/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/required/end_step.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.2/flowlang/core/steps/required/start_step.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.2/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.2/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flowlang-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 flowlang-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/models/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/models/base.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/models/openai_model.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/scenarios/__init__.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/scenarios/base.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/base.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/__init__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/apicall_step.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/control_step.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/summarization_step.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/translation_step.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/helpers/validation_step.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/required/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/required/end_step.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flowlang-0.0.3/flowlang/core/steps/required/start_step.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 flowlang-0.0.3/LICENSE
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 flowlang-0.0.3/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flowlang-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 flowlang-0.0.3/PKG-INFO
```

### Comparing `flowlang-0.0.2/flowlang/core/models/openai_model.py` & `flowlang-0.0.3/flowlang/core/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/scenarios/base.py` & `flowlang-0.0.3/flowlang/core/scenarios/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,21 +52,19 @@
     def run_auto(self):
         self._history['task'] = {'data': self.task, 'id': 0}
         task = self.task
         is_end = False
         attempt = 0
         while not is_end:
             attempt += 1
-            print(f"Task: {task}")
             response = self.control_step(task)['result']
             task = response
             func_call = self.control_step.history[-1].get('function_call')
             if func_call:
                 func_call = ast.literal_eval(func_call)
-                print(f"Func call: {func_call}")
                 self._history[func_call.get('name', 'unknown')] = {'data': response, 'id': attempt}
                 if func_call.get('name') == 'end_step':
                     is_end = True
             else:
                 self._history['control'] = {'data': response, 'id': attempt}
             if attempt == self.max_attempts:
                 is_end = True
```

### Comparing `flowlang-0.0.2/flowlang/core/steps/base.py` & `flowlang-0.0.3/flowlang/core/steps/base.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/steps/helpers/apicall_step.py` & `flowlang-0.0.3/flowlang/core/steps/helpers/apicall_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/steps/helpers/control_step.py` & `flowlang-0.0.3/flowlang/core/steps/helpers/control_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/steps/helpers/summarization_step.py` & `flowlang-0.0.3/flowlang/core/steps/helpers/summarization_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/steps/helpers/translation_step.py` & `flowlang-0.0.3/flowlang/core/steps/helpers/translation_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/flowlang/core/steps/helpers/validation_step.py` & `flowlang-0.0.3/flowlang/core/steps/helpers/validation_step.py`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/LICENSE` & `flowlang-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flowlang-0.0.2/pyproject.toml` & `flowlang-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flowlang"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Egor Sheremetov", email="egorsheremetov3.0@gmail.com" },
 ]
 description = "An easy way to create and automate natural language processes and tasks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flowlang-0.0.2/PKG-INFO` & `flowlang-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowlang
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy way to create and automate natural language processes and tasks.
 Project-URL: Homepage, https://github.com/ESheremetov/Flowlang
 Project-URL: Bug Tracker, https://github.com/ESheremetov/Flowlang/issues
 Author-email: Egor Sheremetov <egorsheremetov3.0@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

