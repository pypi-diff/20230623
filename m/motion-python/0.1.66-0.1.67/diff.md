# Comparing `tmp/motion_python-0.1.66.tar.gz` & `tmp/motion_python-0.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.66.tar", max compression
+gzip compressed data, was "motion_python-0.1.67.tar", max compression
```

## Comparing `motion_python-0.1.66.tar` & `motion_python-0.1.67.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-17 07:58:41.152077 motion_python-0.1.66/README.md
--rw-r--r--   0        0        0      276 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/component.py
--rw-r--r--   0        0        0    17554 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/execute.py
--rw-r--r--   0        0        0    12849 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/route.py
--rw-r--r--   0        0        0     5944 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/server/fit_task.py
--rw-r--r--   0        0        0     9082 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-17 07:58:59.924236 motion_python-0.1.66/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.66/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-23 20:27:55.379951 motion_python-0.1.67/README.md
+-rw-r--r--   0        0        0      276 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/cli.py
+-rw-r--r--   0        0        0    23926 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/component.py
+-rw-r--r--   0        0        0    17652 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/execute.py
+-rw-r--r--   0        0        0    12849 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/route.py
+-rw-r--r--   0        0        0     5944 2023-06-23 20:27:55.379951 motion_python-0.1.67/motion/server/fit_task.py
+-rw-r--r--   0        0        0     9242 2023-06-23 20:27:55.383951 motion_python-0.1.67/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-23 20:28:18.483990 motion_python-0.1.67/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.67/PKG-INFO
```

### Comparing `motion_python-0.1.66/README.md` & `motion_python-0.1.67/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/cli.py` & `motion_python-0.1.67/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/component.py` & `motion_python-0.1.67/motion/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 Name of the component.
                 params (Dict[str, Any], optional):
                     Parameters to be accessed by the component. Defaults to {}.
                     Usage: `C.params["param_name"]` if C is the Component you
                     have created.
         """
         self._name = name
-        self._params = CustomDict(name, "params", params)
+        self._params = CustomDict(name, "params", "", params)
 
         # Set up routes
         self._infer_routes: Dict[str, Route] = {}
         self._fit_routes: Dict[str, List[Route]] = {}
         self._init_state_func: Optional[Callable] = None
         self._save_state_func: Optional[Callable] = None
         self._load_state_func: Optional[Callable] = None
```

### Comparing `motion_python-0.1.66/motion/execute.py` & `motion_python-0.1.67/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,20 @@
                 + "MOTION_REDIS_PORT, MOTION_REDIS_DB, and/or "
                 + "MOTION_REDIS_PASSWORD to your Redis params."
             )
         self.running.value = True
 
         # Set up state
         self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
-        self._state = CustomDict(self._instance_name, "state", {})
+        self._state = CustomDict(
+            instance_name.split("__")[0],
+            "state",
+            instance_name.split("__")[1],
+            {},
+        )
         if self.version is None:
             self.version = 1
             # Setup state
             self._state.update(self.setUp(**self._init_state_params))
             saveState(
                 self._state,
                 self._redis_con,
```

### Comparing `motion_python-0.1.66/motion/instance.py` & `motion_python-0.1.67/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.67/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/route.py` & `motion_python-0.1.67/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/server/fit_task.py` & `motion_python-0.1.67/motion/server/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.66/motion/utils.py` & `motion_python-0.1.67/motion/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,28 +130,30 @@
 
 
 class CustomDict(dict):
     def __init__(
         self,
         component_name: str,
         dict_type: str,
+        instance_id: Optional[str] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         self.component_name = component_name
+        self.instance_id = instance_id
         self.dict_type = dict_type
         super().__init__(*args, **kwargs)
 
     def __getitem__(self, key: str) -> object:
         try:
             return super().__getitem__(key)
         except KeyError:
             raise KeyError(
                 f"Key `{key}` not found in {self.dict_type} for "
-                + f"component {self.component_name}."
+                + f"instance {self.component_name}__{self.instance_id}."
             )
 
 
 def validate_args(parameters: Any, op: str) -> bool:
     expected_args = (
         ["state", "values", "infer_results"] if op == "fit" else ["state", "value"]
     )
@@ -186,15 +188,17 @@
 
 def loadState(
     redis_con: redis.Redis,
     instance_name: str,
     load_state_func: Optional[Callable],
 ) -> CustomDict:
     # Get state from redis
-    state = CustomDict(instance_name, "state", {})
+    state = CustomDict(
+        instance_name.split("__")[0], "state", instance_name.split("__")[1], {}
+    )
     loaded_state = redis_con.get(f"MOTION_STATE:{instance_name}")
 
     if not loaded_state:
         # This is an error
         logger.warning(f"Could not find state for {instance_name}.")
         return state
```

### Comparing `motion_python-0.1.66/pyproject.toml` & `motion_python-0.1.67/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.66"
+version = "0.1.67"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.66/PKG-INFO` & `motion_python-0.1.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.66
+Version: 0.1.67
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

