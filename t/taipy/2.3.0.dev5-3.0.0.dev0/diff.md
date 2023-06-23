# Comparing `tmp/taipy-2.3.0.dev5.tar.gz` & `tmp/taipy-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.3.0.dev5.tar", last modified: Fri Jun 16 09:43:25 2023, max compression
+gzip compressed data, was "taipy-3.0.0.dev0.tar", last modified: Fri Jun 23 10:47:19 2023, max compression
```

## Comparing `taipy-2.3.0.dev5.tar` & `taipy-3.0.0.dev0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 09:41:43.000000 taipy-2.3.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-16 09:42:19.000000 taipy-2.3.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.037931 taipy-2.3.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/_help_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_cli/_scaffold_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/gui_core/
--rw-r--r--   0 runner    (1001) docker     (123)    21626 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/gui_core/GuiCoreLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/gui_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy/gui_core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   657664 2023-06-16 09:43:18.000000 taipy-2.3.0.dev5/src/taipy/gui_core/lib/taipy-gui-core.js
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.041931 taipy-2.3.0.dev5/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:43:18.000000 taipy-2.3.0.dev5/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 09:43:25.000000 taipy-2.3.0.dev5/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:43:25.045932 taipy-2.3.0.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-16 09:41:44.000000 taipy-2.3.0.dev5/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-23 10:46:09.000000 taipy-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.926101 taipy-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.930101 taipy-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    22398 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/gui_core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/src/taipy/gui_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   658126 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.934102 taipy-3.0.0.dev0/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:47:12.000000 taipy-3.0.0.dev0/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:47:19.000000 taipy-3.0.0.dev0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:47:19.938102 taipy-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-23 10:45:32.000000 taipy-3.0.0.dev0/tests/test_run.py
```

### Comparing `taipy-2.3.0.dev5/LICENSE` & `taipy-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/PKG-INFO` & `taipy-3.0.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev5
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev5/README.md` & `taipy-3.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/setup.py` & `taipy-3.0.0.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "cookiecutter>=2.1.1,<2.2",
-    "taipy-gui==2.3.0.dev6",
-    "taipy-rest==2.3.0.dev2",
-    "taipy-templates==2.3.0.dev1",
+    "taipy-gui==3.0.0.dev0",
+    "taipy-rest==3.0.0.dev0",
+    "taipy-templates==3.0.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "ngrok": ["pyngrok>=5.1,<6.0"],
     "image": [
```

### Comparing `taipy-2.3.0.dev5/src/taipy/_cli/__init__.py` & `taipy-3.0.0.dev0/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/src/taipy/_cli/_help_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_help_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/src/taipy/_cli/_scaffold_cli.py` & `taipy-3.0.0.dev0/src/taipy/_cli/_scaffold_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/src/taipy/_entrypoint.py` & `taipy-3.0.0.dev0/src/taipy/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/src/taipy/_run.py` & `taipy-3.0.0.dev0/src/taipy/_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     gui = __get_app(services, Gui)
     rest = __get_app(services, Rest)
     core = __get_app(services, Core)
 
     if gui and core:
-        from taipy.core._version._cli._core_cli import _CoreCLI
+        from taipy.core._core_cli import _CoreCLI
         from taipy.gui._gui_cli import _GuiCLI
 
         _CoreCLI.create_parser()
         _GuiCLI.create_parser()
 
     if rest or core:
         if not core:
```

### Comparing `taipy-2.3.0.dev5/src/taipy/gui_core/GuiCoreLib.py` & `taipy-3.0.0.dev0/src/taipy/gui_core/GuiCoreLib.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,66 +12,79 @@
 import typing as t
 from datetime import datetime
 from enum import Enum
 from threading import Lock
 
 from dateutil import parser
 
-import taipy as tp
 from taipy.config import Config
-from taipy.core import Cycle, DataNode, Pipeline, Scenario
+from taipy.core import Cycle, DataNode, Pipeline, Scenario, create_scenario
+from taipy.core import delete as core_delete
+from taipy.core import get as core_get
+from taipy.core import (
+    get_cycles_scenarios,
+    get_data_nodes,
+    get_scenarios,
+    is_deletable,
+    is_promotable,
+    is_submittable,
+    set_primary,
+)
+from taipy.core import submit as core_submit
 from taipy.core.notification import CoreEventConsumerBase, EventEntityType
 from taipy.core.notification.event import Event
 from taipy.core.notification.notifier import Notifier
 from taipy.gui import Gui, State
 from taipy.gui.extension import Element, ElementLibrary, ElementProperty, PropertyType
 from taipy.gui.gui import _DoNotUpdate
 from taipy.gui.utils import _TaipyBase
 
 from ..version import _get_version
 
 
 # prevent gui from trying to push scenario instances to the front-end
-class DoNotUpdate(_DoNotUpdate):
+class _GCDoNotUpdate(_DoNotUpdate):
     def __repr__(self):
         return self.get_label() if hasattr(self, "get_label") else super().__repr__()
 
 
-Scenario.__bases__ += (DoNotUpdate,)
-DataNode.__bases__ += (DoNotUpdate,)
+Scenario.__bases__ += (_GCDoNotUpdate,)
+DataNode.__bases__ += (_GCDoNotUpdate,)
 
 Config.configure_global_app(read_entity_retry=3)
 
 
-class EntityType(Enum):
+class _EntityType(Enum):
     CYCLE = 0
     SCENARIO = 1
     PIPELINE = 2
     DATANODE = 3
 
 
 class _GuiCoreScenarioAdapter(_TaipyBase):
     __INNER_PROPS = ["name"]
 
     def get(self):
         data = super().get()
         if isinstance(data, Scenario):
-            scenario = tp.get(data.id)
+            scenario = core_get(data.id)
             if scenario:
                 return [
                     scenario.id,
                     scenario.is_primary,
                     scenario.config_id,
                     scenario.creation_date,
                     scenario.get_simple_label(),
                     list(scenario.tags),
                     [(k, v) for k, v in scenario.properties.items() if k not in _GuiCoreScenarioAdapter.__INNER_PROPS],
-                    [(p.id, p.get_simple_label()) for p in scenario.pipelines.values()],
+                    [(p.id, p.get_simple_label(), is_submittable(p)) for p in scenario.pipelines.values()],
                     list(scenario.properties.get("authorized_tags", set())),
-                    tp.is_deletable(scenario),  # deletable
+                    is_deletable(scenario),  # deletable
+                    is_promotable(scenario),
+                    is_submittable(scenario),
                 ]
         return None
 
     @staticmethod
     def get_hash():
         return _TaipyBase._HOLDER_PREFIX + "Sc"
 
@@ -80,15 +93,15 @@
     @staticmethod
     def get_entity_type(node: t.Any):
         return DataNode.__name__ if isinstance(node.entity, DataNode) else node.type
 
     def get(self):
         data = super().get()
         if isinstance(data, Scenario):
-            scenario = tp.get(data.id)
+            scenario = core_get(data.id)
             if scenario:
                 dag = data._get_dag()
                 nodes = dict()
                 for id, node in dag.nodes.items():
                     entityType = _GuiCoreScenarioDagAdapter.get_entity_type(node)
                     cat = nodes.get(entityType)
                     if cat is None:
@@ -141,42 +154,42 @@
         self.lock = Lock()
         super().__init__(reg_id, reg_queue)
         self.start()
 
     def process_event(self, event: Event):
         if event.entity_type == EventEntityType.SCENARIO:
             self.scenarios_base_level = None
-            scenario = tp.get(event.entity_id) if event.operation.value != 3 else None
+            scenario = core_get(event.entity_id) if event.operation.value != 3 else None
             self.gui.broadcast(
                 _GuiCoreContext._CORE_CHANGED_NAME,
                 {"scenario": event.entity_id if scenario else True},
             )
             self.data_nodes_base_level = None
         elif event.entity_type == EventEntityType.PIPELINE and event.entity_id:  # TODO import EventOperation
-            pipeline = tp.get(event.entity_id) if event.operation.value != 3 else None
+            pipeline = core_get(event.entity_id) if event.operation.value != 3 else None
             if pipeline:
                 if hasattr(pipeline, "parent_ids") and pipeline.parent_ids:
                     self.gui.broadcast(
                         _GuiCoreContext._CORE_CHANGED_NAME, {"scenario": [x for x in pipeline.parent_ids]}
                     )
 
     @staticmethod
     def scenario_adapter(data):
-        if hasattr(data, "id") and tp.get(data.id) is not None:
+        if hasattr(data, "id") and core_get(data.id) is not None:
             if isinstance(data, Cycle):
-                return (data.id, data.get_simple_label(), tp.get_scenarios(data), EntityType.CYCLE.value, False)
+                return (data.id, data.get_simple_label(), get_scenarios(data), _EntityType.CYCLE.value, False)
             elif isinstance(data, Scenario):
-                return (data.id, data.get_simple_label(), None, EntityType.SCENARIO.value, data.is_primary)
+                return (data.id, data.get_simple_label(), None, _EntityType.SCENARIO.value, data.is_primary)
         return None
 
     def get_scenarios(self):
         with self.lock:
             if self.scenarios_base_level is None:
                 self.scenarios_base_level = []
-                for cycle, scenarios in tp.get_cycles_scenarios().items():
+                for cycle, scenarios in get_cycles_scenarios().items():
                     if cycle is None:
                         self.scenarios_base_level.extend(scenarios)
                     else:
                         self.scenarios_base_level.append(cycle)
             return self.scenarios_base_level
 
     def select_scenario(self, state: State, id: str, action: str, payload: t.Dict[str, str]):
@@ -185,27 +198,27 @@
             return
         state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ID_VAR, args[0])
 
     def get_scenario_by_id(self, id: str) -> t.Optional[Scenario]:
         if not id:
             return None
         try:
-            return tp.get(id)
+            return core_get(id)
         except Exception:
             return None
 
     def get_scenario_configs(self):
         with self.lock:
             if self.scenario_configs is None:
-                configs = tp.Config.scenarios
+                configs = Config.scenarios
                 if isinstance(configs, dict):
-                    self.scenario_configs = [(id, f"{c.id}") for id, c in configs.items()]
+                    self.scenario_configs = [(id, f"{c.id}") for id, c in configs.items() if id != "default"]
             return self.scenario_configs
 
-    def crud_scenario(self, state: State, id: str, action: str, payload: t.Dict[str, str]):
+    def crud_scenario(self, state: State, id: str, action: str, payload: t.Dict[str, str]):  # noqa: C901
         args = payload.get("args")
         if (
             args is None
             or not isinstance(args, list)
             or len(args) < 3
             or not isinstance(args[0], bool)
             or not isinstance(args[1], bool)
@@ -217,61 +230,65 @@
         data = args[2]
         scenario = None
         name = data.get(_GuiCoreContext.__PROP_ENTITY_NAME)
         if update:
             scenario_id = data.get(_GuiCoreContext.__PROP_ENTITY_ID)
             if delete:
                 try:
-                    tp.delete(scenario_id)
+                    core_delete(scenario_id)
                 except Exception as e:
                     state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, f"Error deleting Scenario. {e}")
             else:
-                scenario = tp.get(scenario_id)
+                scenario = core_get(scenario_id)
         else:
             config_id = data.get(_GuiCoreContext.__PROP_SCENARIO_CONFIG_ID)
-            scenario_config = tp.Config.scenarios.get(config_id)
+            scenario_config = Config.scenarios.get(config_id)
             if scenario_config is None:
                 state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, f"Invalid configuration id ({config_id})")
                 return
             date_str = data.get(_GuiCoreContext.__PROP_SCENARIO_DATE)
             try:
                 date = parser.parse(date_str) if isinstance(date_str, str) else None
             except Exception as e:
                 state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, f"Invalid date ({date_str}).{e}")
                 return
             try:
-                scenario = tp.create_scenario(scenario_config, date, name)
+                scenario = create_scenario(scenario_config, date, name)
             except Exception as e:
                 state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, f"Error creating Scenario. {e}")
         if scenario:
             with scenario as sc:
-                sc._properties[_GuiCoreContext.__PROP_ENTITY_NAME] = name
+                sc.properties[_GuiCoreContext.__PROP_ENTITY_NAME] = name
                 if props := data.get("properties"):
                     try:
+                        new_keys = [prop.get("key") for prop in props]
+                        for key in t.cast(dict, sc.properties).keys():
+                            if key and key not in _GuiCoreContext.__SCENARIO_PROPS and key not in new_keys:
+                                t.cast(dict, sc.properties).pop(key, None)
                         for prop in props:
                             key = prop.get("key")
                             if key and key not in _GuiCoreContext.__SCENARIO_PROPS:
                                 sc._properties[key] = prop.get("value")
                         state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, "")
                     except Exception as e:
                         state.assign(_GuiCoreContext._SCENARIO_SELECTOR_ERROR_VAR, f"Error creating Scenario. {e}")
 
     def edit_entity(self, state: State, id: str, action: str, payload: t.Dict[str, str]):
         args = payload.get("args")
         if args is None or not isinstance(args, list) or len(args) < 1 or not isinstance(args[0], dict):
             return
         data = args[0]
         entity_id = data.get(_GuiCoreContext.__PROP_ENTITY_ID)
-        entity: t.Union[Scenario, Pipeline] = tp.get(entity_id)
+        entity: t.Union[Scenario, Pipeline] = core_get(entity_id)
         if entity:
             try:
                 if isinstance(entity, Scenario):
                     primary = data.get(_GuiCoreContext.__PROP_SCENARIO_PRIMARY)
                     if primary is True:
-                        tp.set_primary(entity)
+                        set_primary(entity)
                 with entity as ent:
                     if isinstance(ent, Scenario):
                         tags = data.get(_GuiCoreContext.__PROP_SCENARIO_TAGS)
                         if isinstance(tags, (list, tuple)):
                             ent.tags = {t for t in tags}
                     name = data.get(_GuiCoreContext.__PROP_ENTITY_NAME)
                     if isinstance(name, str):
@@ -294,66 +311,66 @@
 
     def submit_entity(self, state: State, id: str, action: str, payload: t.Dict[str, str]):
         args = payload.get("args")
         if args is None or not isinstance(args, list) or len(args) < 1 or not isinstance(args[0], dict):
             return
         data = args[0]
         entity_id = data.get(_GuiCoreContext.__PROP_ENTITY_ID)
-        entity = tp.get(entity_id)
+        entity = core_get(entity_id)
         if entity:
             try:
-                tp.submit(entity)
+                core_submit(entity)
                 state.assign(_GuiCoreContext._SCENARIO_VIZ_ERROR_VAR, "")
             except Exception as e:
                 state.assign(_GuiCoreContext._SCENARIO_VIZ_ERROR_VAR, f"Error submitting entity. {e}")
 
     def get_datanodes_tree(self):
         with self.lock:
             if self.data_nodes_base_level is None:
                 self.data_nodes_base_level = _GuiCoreContext.__get_data_nodes()
-                for cycle, scenarios in tp.get_cycles_scenarios().items():
+                for cycle, scenarios in get_cycles_scenarios().items():
                     if cycle is None:
                         self.data_nodes_base_level.extend(scenarios)
                     else:
                         self.data_nodes_base_level.append(cycle)
             return self.data_nodes_base_level
 
     @staticmethod
     def __get_data_nodes(id: t.Optional[str] = None):
         def from_parent(dn: DataNode):
             if id is None and dn.owner_id is None:
                 return True
             return False if id is None or dn.owner_id is None else dn.owner_id == id
 
-        return [x for x in tp.get_data_nodes() if from_parent(x)]
+        return [x for x in get_data_nodes() if from_parent(x)]
 
     @staticmethod
     def data_node_adapter(data):
-        if hasattr(data, "id") and tp.get(data.id) is not None:
+        if hasattr(data, "id") and core_get(data.id) is not None:
             if isinstance(data, Cycle):
                 return (
                     data.id,
                     data.get_simple_label(),
-                    _GuiCoreContext.__get_data_nodes(data.id) + tp.get_scenarios(data),
-                    EntityType.CYCLE.value,
+                    _GuiCoreContext.__get_data_nodes(data.id) + get_scenarios(data),
+                    _EntityType.CYCLE.value,
                     False,
                 )
             elif isinstance(data, Scenario):
                 return (
                     data.id,
                     data.get_simple_label(),
-                    _GuiCoreContext.__get_data_nodes(data.id) + [tp.get(p) for p in data._pipelines],
-                    EntityType.SCENARIO.value,
+                    _GuiCoreContext.__get_data_nodes(data.id) + [core_get(p) for p in data._pipelines],
+                    _EntityType.SCENARIO.value,
                     data.is_primary,
                 )
             elif isinstance(data, Pipeline):
                 if dn := _GuiCoreContext.__get_data_nodes(data.id):
-                    return (data.id, data.get_simple_label(), dn, EntityType.PIPELINE.value, False)
+                    return (data.id, data.get_simple_label(), dn, _EntityType.PIPELINE.value, False)
             elif isinstance(data, DataNode):
-                return (data.id, data.get_simple_label(), None, EntityType.DATANODE.value, False)
+                return (data.id, data.get_simple_label(), None, _EntityType.DATANODE.value, False)
         return None
 
 
 class _GuiCore(ElementLibrary):
     __LIB_NAME = "taipy_gui_core"
     __CTX_VAR_NAME = f"__{__LIB_NAME}_Ctx"
     __SCENARIO_ADAPTER = "tgc_scenario"
```

### Comparing `taipy-2.3.0.dev5/src/taipy/gui_core/lib/taipy-gui-core.js` & `taipy-3.0.0.dev0/src/taipy/gui_core/lib/taipy-gui-core.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9833,17 +9833,17 @@
             value: !0
         })
     }, i.nmd = e => (e.paths = [], e.children || (e.children = []), e);
     var a = {};
     return (() => {
         "use strict";
         i.r(a), i.d(a, {
-            DataNodeSelector: () => kw,
-            Scenario: () => xy,
-            ScenarioDag: () => yw,
+            DataNodeSelector: () => Ew,
+            Scenario: () => wy,
+            ScenarioDag: () => xw,
             ScenarioSelector: () => jg
         });
         var e = i(5893),
             t = i(6255),
             n = i.t(t, 2),
             r = i(9263);
 
@@ -24311,15 +24311,15 @@
                         onClick: a,
                         children: r
                     })]
                 })]
             });
         var lg;
         ! function(e) {
-            e[e.id = 0] = "id", e[e.is_primary = 1] = "is_primary", e[e.config_id = 2] = "config_id", e[e.creation_date = 3] = "creation_date", e[e.label = 4] = "label", e[e.tags = 5] = "tags", e[e.properties = 6] = "properties", e[e.pipelines = 7] = "pipelines", e[e.authorized_tags = 8] = "authorized_tags", e[e.deletable = 9] = "deletable"
+            e[e.id = 0] = "id", e[e.is_primary = 1] = "is_primary", e[e.config_id = 2] = "config_id", e[e.creation_date = 3] = "creation_date", e[e.label = 4] = "label", e[e.tags = 5] = "tags", e[e.properties = 6] = "properties", e[e.pipelines = 7] = "pipelines", e[e.authorized_tags = 8] = "authorized_tags", e[e.deletable = 9] = "deletable", e[e.promotable = 10] = "promotable", e[e.submittable = 11] = "submittable"
         }(lg || (lg = {}));
         const ug = Object.keys(lg).length / 2,
             cg = {
                 color: "common.white",
                 fontSize: "0.75em"
             },
             dg = {
@@ -24342,16 +24342,15 @@
             },
             hg = {
                 mb: 2,
                 "& .MuiTreeItem-root .MuiTreeItem-content": {
                     mb: .5,
                     py: 1,
                     px: 2,
-                    borderRadius: .5,
-                    backgroundColor: "background.paper"
+                    borderRadius: .5
                 },
                 "& .MuiTreeItem-iconContainer:empty": {
                     display: "none"
                 },
                 maxHeight: "50vh",
                 overflowY: "auto"
             },
@@ -24815,15 +24814,21 @@
                 (0, t.useEffect)((() => {
                     var e;
                     if (null === (e = n.coreChanged) || void 0 === e ? void 0 : e.scenario) {
                         const e = (0, Qh.getUpdateVar)(n.updateVars, "scenarios");
                         e && g((0, Qh.createRequestUpdateAction)(r, v, [e], !0))
                     }
                 }), [n.coreChanged, n.updateVars, v, g, r]), (0, t.useEffect)((() => {
-                    void 0 !== s ? f(s) : a && f(a)
+                    if (null != s) f(s);
+                    else if (a) try {
+                        const e = JSON.parse(a);
+                        Array.isArray(e) ? e.length && f(e[0]) : f(e)
+                    } catch (e) {
+                        f(a)
+                    } else null === s && f("")
                 }), [a, s]), (0, t.useEffect)((() => {
                     o.length || E()
                 }), [o, E]);
                 const O = (0, t.useMemo)((() => Object.assign(Object.assign({}, hg), {
                     maxHeight: n.height || "50vh"
                 })), [n.height]);
                 return (0, e.jsxs)(e.Fragment, {
@@ -28376,210 +28381,227 @@
                 label: i,
                 submitEntity: a,
                 enableScenarioFields: s,
                 submit: l,
                 editLabel: u,
                 onFocus: c,
                 focusName: d,
-                setFocusName: p
+                setFocusName: p,
+                submittable: f
             }) => {
-                const [f, h] = (0, t.useState)(i), g = (0, t.useCallback)((e => h(e.currentTarget.value)), []), v = (0, t.useCallback)((e => {
-                    e.stopPropagation(), u(o, f)
-                }), [o, f, u]), m = (0, t.useCallback)((e => {
-                    e.stopPropagation(), h(i), p("")
-                }), [i, p]), y = (0, t.useCallback)((() => a(o)), [a, o]);
-                (0, t.useEffect)((() => h(i)), [i]);
-                const b = `pipeline${r}`,
-                    x = r + 1;
+                const [h, g] = (0, t.useState)(i), v = (0, t.useCallback)((e => g(e.currentTarget.value)), []), m = (0, t.useCallback)((e => {
+                    e.stopPropagation(), u(o, h)
+                }), [o, h, u]), y = (0, t.useCallback)((e => {
+                    e.stopPropagation(), g(i), p("")
+                }), [i, p]), b = (0, t.useCallback)((e => {
+                    e.stopPropagation(), a(o)
+                }), [a, o]);
+                (0, t.useEffect)((() => g(i)), [i]);
+                const x = `pipeline${r}`,
+                    w = r + 1;
                 return (0, e.jsxs)(Nr, {
                     item: !0,
                     xs: 12,
                     container: !0,
                     justifyContent: "space-between",
-                    "data-focus": b,
+                    "data-focus": x,
                     onClick: c,
                     sx: vy,
                     children: [(0, e.jsx)(Nr, {
                         item: !0,
                         container: !0,
                         xs: 10,
-                        children: n && d === b ? (0, e.jsx)(As, {
-                            label: `Pipeline ${x}`,
+                        children: n && d === x ? (0, e.jsx)(As, {
+                            label: `Pipeline ${w}`,
                             variant: "outlined",
-                            value: f,
-                            onChange: g,
+                            value: h,
+                            onChange: v,
                             sx: cy,
                             disabled: !s,
                             fullWidth: !0,
                             InputProps: {
                                 endAdornment: (0, e.jsxs)(ly, {
                                     position: "end",
                                     children: [(0, e.jsx)(zr, {
                                         sx: fy,
-                                        onClick: v,
+                                        onClick: m,
                                         children: (0, e.jsx)(Rs.CheckCircle, {
                                             color: "primary"
                                         })
                                     }), (0, e.jsx)(zr, {
                                         sx: fy,
-                                        onClick: m,
+                                        onClick: y,
                                         children: (0, e.jsx)(Rs.Cancel, {
                                             color: "inherit"
                                         })
                                     })]
                                 })
                             }
                         }) : (0, e.jsx)(Qn, {
                             variant: "subtitle2",
-                            children: f
+                            children: h
                         })
                     }), (0, e.jsx)(Nr, {
                         item: !0,
                         xs: 2,
                         container: !0,
                         alignContent: "center",
                         alignItems: "center",
                         justifyContent: "center",
                         children: l ? (0, e.jsx)(zr, {
                             size: "small",
-                            onClick: y,
-                            disabled: !s || !n,
+                            onClick: b,
+                            disabled: !s || !n || !f,
                             children: (0, e.jsx)(Rs.Send, {
-                                color: yy("info", !s)
+                                color: yy("info", !s || !n || !f)
                             })
                         }) : null
                     })]
                 })
             },
-            xy = n => {
+            xy = e => e.length == ug && "string" == typeof e[lg.id] ? e : 1 == e.length ? e[0] : void 0,
+            wy = n => {
                 const {
                     id: r = "",
                     expandable: o = !0,
                     showConfig: i = !1,
                     showCycle: a = !1,
                     showDelete: s = !0,
                     showProperties: l = !0,
                     showPipelines: u = !0,
                     showSubmit: c = !0,
                     showSubmitPipelines: d = !0,
                     showTags: p = !1
-                } = n, f = (0, Qh.useDispatch)(), h = (0, Qh.useModule)(), [g, v, m, y, b, x, w, k, S, E, C] = (0, t.useMemo)((() => {
-                    const e = Array.isArray(n.scenario) ? n.scenario.length == ug && "string" == typeof n.scenario[lg.id] ? n.scenario : 1 == n.scenario.length ? n.scenario[0] : void 0 : void 0;
+                } = n, f = (0, Qh.useDispatch)(), h = (0, Qh.useModule)(), [g, v, m, y, b, x, w, k, S, E, C, O, _] = (0, t.useMemo)((() => {
+                    let e;
+                    if (Array.isArray(n.scenario)) e = xy(n.scenario);
+                    else if (n.defaultScenario) try {
+                        e = xy(JSON.parse(n.defaultScenario))
+                    } catch (e) {}
                     return e ? [...e, !0] : ["", !1, "", "", "", [],
                         [],
                         [],
-                        [], !1, !1
+                        [], !1, !1, !1, !1
                     ]
-                }), [n.scenario]), O = (0, Qh.useDynamicProperty)(n.active, n.defaultActive, !0), _ = (0, Qh.useDynamicProperty)(n.expanded, n.defaultExpanded, !1), T = vg(n.libClassName, n.dynamicClassName, n.className), [P, M] = (0, t.useState)(!1), j = (0, t.useCallback)((() => M(!0)), []), A = (0, t.useCallback)((() => M(!1)), []), R = (0, t.useCallback)((() => {
-                    M(!1), C && f((0, Qh.createSendActionNameAction)(r, h, n.onDelete, !0, !0, {
+                }), [n.scenario, n.defaultScenario]), T = (0, Qh.useDynamicProperty)(n.active, n.defaultActive, !0), P = (0, Qh.useDynamicProperty)(n.expanded, n.defaultExpanded, !1), M = vg(n.libClassName, n.dynamicClassName, n.className), [j, A] = (0, t.useState)(!1), R = (0, t.useCallback)((() => A(!0)), []), I = (0, t.useCallback)((() => A(!1)), []), N = (0, t.useCallback)((() => {
+                    A(!1), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onDelete, !0, !0, {
                         id: g
                     }))
-                }), [C, n.onDelete, g, r, f, h]), [I, N] = (0, t.useState)(!1), L = (0, t.useCallback)((() => N(!0)), []), D = (0, t.useCallback)((() => N(!1)), []), F = (0, t.useCallback)((() => {
-                    N(!1), C && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                }), [_, n.onDelete, g, r, f, h]), [L, D] = (0, t.useState)(!1), F = (0, t.useCallback)((() => D(!0)), []), $ = (0, t.useCallback)((() => D(!1)), []), z = (0, t.useCallback)((() => {
+                    D(!1), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
                         id: g,
                         primary: !0
                     }))
-                }), [C, n.onEdit, g, r, f, h]), [$, z] = (0, t.useState)([]), [W, B] = (0, t.useState)({
+                }), [_, n.onEdit, g, r, f, h]), [W, B] = (0, t.useState)([]), [U, Y] = (0, t.useState)({
                     id: "",
                     key: "",
                     value: ""
-                }), [U, Y] = (0, t.useState)(!1), H = (0, t.useCallback)(((e, t) => Y(t)), []), V = (0, t.useCallback)((e => {
+                }), [H, V] = (0, t.useState)(!1), G = (0, t.useCallback)(((e, t) => V(t)), []), q = (0, t.useCallback)((e => {
                     f((0, Qh.createSendActionNameAction)(r, h, n.onSubmit, {
                         id: e
                     }))
-                }), [n.onSubmit, r, f, h]), G = (0, t.useCallback)((e => {
-                    e.stopPropagation(), C && f((0, Qh.createSendActionNameAction)(r, h, n.onSubmit, {
+                }), [n.onSubmit, r, f, h]), X = (0, t.useCallback)((e => {
+                    e.stopPropagation(), _ && f((0, Qh.createSendActionNameAction)(r, h, n.onSubmit, {
                         id: g
                     }))
-                }), [C, n.onSubmit, r, g, f, h]), [q, X] = (0, t.useState)(""), K = (0, t.useCallback)((e => {
-                    e.stopPropagation(), X(e.currentTarget.dataset.focus || "")
-                }), []), [Z, Q] = (0, t.useState)(), J = (0, t.useCallback)((e => {
-                    e.stopPropagation(), C && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                }), [_, n.onSubmit, r, g, f, h]), [K, Z] = (0, t.useState)(""), Q = (0, t.useCallback)((e => {
+                    e.stopPropagation(), Z(e.currentTarget.dataset.focus || "")
+                }), []), [J, ee] = (0, t.useState)(), te = (0, t.useCallback)((e => {
+                    e.stopPropagation(), _ && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
                         id: g,
-                        name: Z
-                    })), X(""))
-                }), [C, n.onEdit, g, Z, r, f, h]), ee = (0, t.useCallback)((e => {
-                    e.stopPropagation(), Q(b), X("")
-                }), [b, Q, X]), te = (0, t.useCallback)((e => Q(e.target.value)), []), [ne, re] = (0, t.useState)([]), oe = (0, t.useCallback)((e => {
-                    e.stopPropagation(), C && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
+                        name: J
+                    })), Z(""))
+                }), [_, n.onEdit, g, J, r, f, h]), ne = (0, t.useCallback)((e => {
+                    e.stopPropagation(), ee(b), Z("")
+                }), [b, ee, Z]), re = (0, t.useCallback)((e => ee(e.target.value)), []), [oe, ie] = (0, t.useState)([]), ae = (0, t.useCallback)((e => {
+                    e.stopPropagation(), _ && (f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
                         id: g,
-                        tags: ne
-                    })), X(""))
-                }), [C, n.onEdit, g, ne, r, f, h]), ie = (0, t.useCallback)((e => {
-                    e.stopPropagation(), re(x), X("")
-                }), [x]), ae = (0, t.useCallback)(((e, t) => re(t)), []), se = (0, t.useCallback)((e => {
+                        tags: oe
+                    })), Z(""))
+                }), [_, n.onEdit, g, oe, r, f, h]), se = (0, t.useCallback)((e => {
+                    e.stopPropagation(), ie(x), Z("")
+                }), [x]), le = (0, t.useCallback)(((e, t) => ie(t)), []), ue = (0, t.useCallback)((e => {
                     var t, n;
                     const {
                         id: r = "",
                         name: o = ""
                     } = (null === (n = null === (t = e.currentTarget.parentElement) || void 0 === t ? void 0 : t.parentElement) || void 0 === n ? void 0 : n.dataset) || {};
-                    o && (r ? z((t => t.map((t => (r == t.id && (t[o] = e.target.value), t))))) : B((t => Object.assign(Object.assign({}, t), {
+                    o && (r ? B((t => t.map((t => r === t.id ? Object.assign(Object.assign({}, t), {
+                        [o]: e.target.value
+                    }) : t)))) : Y((t => Object.assign(Object.assign({}, t), {
                         [o]: e.target.value
                     }))))
-                }), []), le = (0, t.useCallback)((e => {
-                    if (e.stopPropagation(), C) {
+                }), []), ce = (0, t.useCallback)((e => {
+                    if (e.stopPropagation(), _) {
                         const {
                             id: t = ""
-                        } = e.currentTarget.dataset || {}, o = t ? $.find((e => e.id === t)) : W;
-                        o && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
-                            id: g,
-                            properties: [o]
-                        })), B((e => Object.assign(Object.assign({}, e), {
+                        } = e.currentTarget.dataset || {}, o = t ? W.find((e => e.id === t)) : U;
+                        if (o) {
+                            const e = o.id,
+                                t = {
+                                    id: g,
+                                    properties: [o]
+                                };
+                            e && e != o.key && (t.deleted_properties = [{
+                                key: e
+                            }]), f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, t))
+                        }
+                        Y((e => Object.assign(Object.assign({}, e), {
                             key: "",
                             value: ""
-                        }))), X("")
+                        }))), Z("")
                     }
-                }), [C, n.onEdit, g, $, W, r, f, h]), ue = (0, t.useCallback)((e => {
-                    if (e.stopPropagation(), C) {
+                }), [_, n.onEdit, g, W, U, r, f, h]), de = (0, t.useCallback)((e => {
+                    if (e.stopPropagation(), _) {
                         const {
                             id: t = ""
-                        } = e.currentTarget.dataset || {}, n = $.findIndex((e => e.id === t));
-                        n > -1 && n < w.length && z((e => e.map(((e, t) => t == n ? Object.assign(Object.assign({}, e), {
-                            key: w[t][0],
-                            value: w[t][1]
-                        }) : e)))), X("")
+                        } = e.currentTarget.dataset || {}, n = w.find((([e]) => e === t));
+                        n && B((e => e.map((e => e.id === n[0] ? Object.assign(Object.assign({}, e), {
+                            key: n[0],
+                            value: n[1]
+                        }) : e)))), Z("")
                     }
-                }), [C, $, w]), ce = (0, t.useCallback)((e => {
+                }), [_, w]), pe = (0, t.useCallback)((e => {
                     e.stopPropagation();
                     const {
-                        id: t = "-1"
+                        id: t = ""
                     } = e.currentTarget.dataset;
-                    z((e => e.filter((e => e.id !== t))));
-                    const o = $.find((e => e.id === t));
+                    B((e => e.filter((e => e.id !== t))));
+                    const o = W.find((e => e.id === t));
                     o && f((0, Qh.createSendActionNameAction)(r, h, n.onEdit, {
                         id: g,
                         deleted_properties: [o]
-                    })), X("")
-                }), [n.onEdit, g, r, f, h, $]), de = (0, t.useCallback)(((e, t) => {
-                    C && (f((0, Qh.createSendActionNameAction)(e, h, n.onEdit, {
+                    })), Z("")
+                }), [n.onEdit, g, r, f, h, W]), fe = (0, t.useCallback)(((e, t) => {
+                    _ && (f((0, Qh.createSendActionNameAction)(e, h, n.onEdit, {
                         id: e,
                         name: t
-                    })), X(""))
-                }), [C, n.onEdit, f, h]);
+                    })), Z(""))
+                }), [_, n.onEdit, f, h]);
                 return (0, t.useEffect)((() => {
-                    p && re(x), l && z(w.map((([e, t], n) => ({
-                        id: n + "",
+                    p && ie(x), l && B(w.map((([e, t]) => ({
+                        id: e,
                         key: e,
                         value: t
-                    })))), Q(b), C || Y(!1)
-                }), [x, w, b, C, p, l]), (0, t.useEffect)((() => {
+                    })))), ee(b), _ || V(!1)
+                }), [x, w, b, _, p, l]), (0, t.useEffect)((() => {
                     var e;
                     const t = null === (e = n.coreChanged) || void 0 === e ? void 0 : e.scenario;
                     ("string" == typeof t ? t === g : Array.isArray(t) ? t.includes(g) : t) && n.updateVarName && f((0, Qh.createRequestUpdateAction)(r, h, [n.updateVarName], !0))
                 }), [n.coreChanged, n.updateVarName, r, h, f, g]), (0, e.jsxs)(e.Fragment, {
                     children: [(0, e.jsxs)(Ft, {
                         sx: uy,
                         id: r,
-                        onClick: K,
-                        className: T,
+                        onClick: Q,
+                        className: M,
                         children: [(0, e.jsxs)(Dg, {
-                            defaultExpanded: o && _,
-                            expanded: U,
-                            onChange: H,
-                            disabled: !C,
+                            defaultExpanded: o && P,
+                            expanded: H,
+                            onChange: G,
+                            disabled: !_,
                             children: [(0, e.jsx)(qg, {
                                 expandIcon: (0, e.jsx)(Rs.ArrowForwardIosSharp, {
                                     sx: dy
                                 }),
                                 sx: my,
                                 children: (0, e.jsxs)(Nr, {
                                     container: !0,
@@ -28598,19 +28620,19 @@
                                             size: "small",
                                             sx: py
                                         })]
                                     }), (0, e.jsx)(Nr, {
                                         item: !0,
                                         children: c ? (0, e.jsx)(zr, {
                                             sx: fy,
-                                            onClick: G,
-                                            disabled: !C || !O,
+                                            onClick: X,
+                                            disabled: !_ || !T || !O,
                                             children: (0, e.jsx)(Rs.Send, {
                                                 fontSize: "medium",
-                                                color: yy("info", !C || !O)
+                                                color: yy("info", !_ || !T || !O)
                                             })
                                         }) : null
                                     })]
                                 })
                             }), (0, e.jsx)(Wg, {
                                 children: (0, e.jsxs)(Nr, {
                                     container: !0,
@@ -28664,42 +28686,42 @@
                                         spacing: 1,
                                         children: [(0, e.jsxs)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             justifyContent: "space-between",
                                             "data-focus": "label",
-                                            onClick: K,
+                                            onClick: Q,
                                             sx: vy,
-                                            children: [O && "label" === q ? (0, e.jsx)(As, {
+                                            children: [T && "label" === K ? (0, e.jsx)(As, {
                                                 label: "Label",
                                                 variant: "outlined",
                                                 fullWidth: !0,
                                                 sx: cy,
-                                                value: Z || "",
-                                                onChange: te,
+                                                value: J || "",
+                                                onChange: re,
                                                 InputProps: {
                                                     endAdornment: (0, e.jsxs)(ly, {
                                                         position: "end",
                                                         children: [(0, e.jsx)(zr, {
                                                             sx: fy,
-                                                            onClick: J,
+                                                            onClick: te,
                                                             children: (0, e.jsx)(Rs.CheckCircle, {
                                                                 color: "primary"
                                                             })
                                                         }), (0, e.jsx)(zr, {
                                                             sx: fy,
-                                                            onClick: ee,
+                                                            onClick: ne,
                                                             children: (0, e.jsx)(Rs.Cancel, {
                                                                 color: "inherit"
                                                             })
                                                         })]
                                                     })
                                                 },
-                                                disabled: !C
+                                                disabled: !_
                                             }) : (0, e.jsxs)(e.Fragment, {
                                                 children: [(0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 4,
                                                     children: (0, e.jsx)(Qn, {
                                                         variant: "subtitle2",
                                                         children: "Label"
@@ -28715,66 +28737,66 @@
                                             }), " "]
                                         }), p ? (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             justifyContent: "space-between",
                                             "data-focus": "tags",
-                                            onClick: K,
+                                            onClick: Q,
                                             sx: vy,
-                                            children: O && "tags" === q ? (0, e.jsx)(Zm, {
+                                            children: T && "tags" === K ? (0, e.jsx)(Zm, {
                                                 multiple: !0,
                                                 options: S,
                                                 freeSolo: !S.length,
                                                 renderTags: (t, n) => t.map(((t, r) => (0, e.jsx)(jm, Object.assign({
                                                     variant: "outlined",
                                                     label: t,
                                                     sx: fy
                                                 }, n({
                                                     index: r
                                                 }))))),
-                                                value: ne,
-                                                onChange: ae,
+                                                value: oe,
+                                                onChange: le,
                                                 fullWidth: !0,
                                                 renderInput: t => (0, e.jsx)(As, Object.assign({}, t, {
                                                     variant: "outlined",
                                                     label: "Tags",
                                                     sx: gy,
                                                     fullWidth: !0,
                                                     InputProps: Object.assign(Object.assign({}, t.InputProps), {
                                                         endAdornment: (0, e.jsxs)(e.Fragment, {
                                                             children: [(0, e.jsx)(zr, {
                                                                 sx: fy,
-                                                                onClick: oe,
+                                                                onClick: ae,
                                                                 children: (0, e.jsx)(Rs.CheckCircle, {
                                                                     color: "primary"
                                                                 })
                                                             }), (0, e.jsx)(zr, {
                                                                 sx: fy,
-                                                                onClick: ie,
+                                                                onClick: se,
                                                                 children: (0, e.jsx)(Rs.Cancel, {
                                                                     color: "inherit"
                                                                 })
                                                             })]
                                                         })
                                                     })
                                                 })),
-                                                disabled: !C
+                                                disabled: !_
                                             }) : (0, e.jsxs)(e.Fragment, {
                                                 children: [(0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 4,
                                                     children: (0, e.jsx)(Qn, {
                                                         variant: "subtitle2",
                                                         children: "Tags"
                                                     })
                                                 }), (0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 8,
-                                                    children: ne.map(((t, n) => (0, e.jsx)(jm, {
+                                                    children: oe.map(((t, n) => (0, e.jsx)(jm, {
                                                         label: t,
                                                         variant: "outlined"
                                                     }, n)))
                                                 })]
                                             })
                                         }) : null]
                                     }), (0, e.jsx)(Nr, {
@@ -28791,89 +28813,89 @@
                                                 children: "Custom Properties"
                                             })
                                         }), (0, e.jsxs)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             container: !0,
                                             rowSpacing: 2,
-                                            children: [$ ? $.map((t => {
+                                            children: [W ? W.map((t => {
                                                 const n = `property-${t.id}`;
                                                 return (0, e.jsx)(Nr, {
                                                     item: !0,
                                                     xs: 12,
                                                     spacing: 1,
                                                     container: !0,
                                                     justifyContent: "space-between",
                                                     "data-focus": n,
-                                                    onClick: K,
+                                                    onClick: Q,
                                                     sx: vy,
-                                                    children: O && q === n ? (0, e.jsxs)(e.Fragment, {
+                                                    children: T && K === n ? (0, e.jsxs)(e.Fragment, {
                                                         children: [(0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 4,
                                                             children: (0, e.jsx)(As, {
                                                                 label: "Key",
                                                                 variant: "outlined",
                                                                 value: t.key,
                                                                 sx: cy,
-                                                                disabled: !C,
+                                                                disabled: !_,
                                                                 "data-name": "key",
                                                                 "data-id": t.id,
-                                                                onChange: se
+                                                                onChange: ue
                                                             })
                                                         }), (0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 6,
                                                             children: (0, e.jsx)(As, {
                                                                 label: "Value",
                                                                 variant: "outlined",
                                                                 value: t.value,
                                                                 sx: cy,
-                                                                disabled: !C,
+                                                                disabled: !_,
                                                                 "data-name": "value",
                                                                 "data-id": t.id,
-                                                                onChange: se
+                                                                onChange: ue
                                                             })
                                                         }), (0, e.jsxs)(Nr, {
                                                             item: !0,
                                                             xs: 1,
                                                             container: !0,
                                                             alignContent: "center",
                                                             alignItems: "center",
                                                             justifyContent: "center",
                                                             children: [(0, e.jsx)(zr, {
                                                                 sx: fy,
                                                                 "data-id": t.id,
-                                                                onClick: le,
+                                                                onClick: ce,
                                                                 children: (0, e.jsx)(Rs.CheckCircle, {
                                                                     color: "primary"
                                                                 })
                                                             }), (0, e.jsx)(zr, {
                                                                 sx: fy,
                                                                 "data-id": t.id,
-                                                                onClick: ue,
+                                                                onClick: de,
                                                                 children: (0, e.jsx)(Rs.Cancel, {
                                                                     color: "inherit"
                                                                 })
                                                             })]
                                                         }), (0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 1,
                                                             container: !0,
                                                             alignContent: "center",
                                                             alignItems: "center",
                                                             justifyContent: "center",
                                                             children: (0, e.jsx)(zr, {
                                                                 sx: hy,
                                                                 "data-id": t.id,
-                                                                onClick: ce,
-                                                                disabled: !C,
+                                                                onClick: pe,
+                                                                disabled: !_,
                                                                 children: (0, e.jsx)(Rs.DeleteOutline, {
                                                                     fontSize: "small",
-                                                                    color: yy("primary", !C)
+                                                                    color: yy("primary", !_)
                                                                 })
                                                             })
                                                         })]
                                                     }) : (0, e.jsxs)(e.Fragment, {
                                                         children: [(0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 4,
@@ -28889,65 +28911,65 @@
                                                                 children: t.value
                                                             })
                                                         }), " ", (0, e.jsx)(Nr, {
                                                             item: !0,
                                                             xs: 2
                                                         })]
                                                     })
-                                                }, t.key)
+                                                }, t.id)
                                             })) : null, (0, e.jsx)(Nr, {
                                                 item: !0,
                                                 xs: 12,
                                                 spacing: 1,
                                                 container: !0,
                                                 justifyContent: "space-between",
-                                                "data-focus": "property-new",
-                                                onClick: K,
+                                                "data-focus": "new-property",
+                                                onClick: Q,
                                                 sx: vy,
-                                                children: O && "property-new" == q ? (0, e.jsxs)(e.Fragment, {
+                                                children: T && "new-property" == K ? (0, e.jsxs)(e.Fragment, {
                                                     children: [(0, e.jsx)(Nr, {
                                                         item: !0,
                                                         xs: 4,
                                                         children: (0, e.jsx)(As, {
-                                                            value: W.key,
+                                                            value: U.key,
                                                             "data-name": "key",
-                                                            onChange: se,
+                                                            onChange: ue,
                                                             label: "Key",
                                                             variant: "outlined",
                                                             sx: cy,
-                                                            disabled: !C
+                                                            disabled: !_
                                                         })
                                                     }), (0, e.jsx)(Nr, {
                                                         item: !0,
                                                         xs: 6,
                                                         children: (0, e.jsx)(As, {
-                                                            value: W.value,
+                                                            value: U.value,
                                                             "data-name": "value",
-                                                            onChange: se,
+                                                            onChange: ue,
                                                             label: "Value",
                                                             variant: "outlined",
                                                             sx: cy,
-                                                            disabled: !C
+                                                            disabled: !_
                                                         })
                                                     }), (0, e.jsxs)(Nr, {
                                                         item: !0,
                                                         xs: 1,
                                                         container: !0,
                                                         alignContent: "center",
                                                         alignItems: "center",
                                                         justifyContent: "center",
                                                         children: [(0, e.jsx)(zr, {
                                                             sx: fy,
-                                                            onClick: le,
+                                                            onClick: ce,
                                                             children: (0, e.jsx)(Rs.CheckCircle, {
                                                                 color: "primary"
                                                             })
                                                         }), (0, e.jsx)(zr, {
                                                             sx: fy,
-                                                            onClick: ue,
+                                                            onClick: de,
                                                             children: (0, e.jsx)(Rs.Cancel, {
                                                                 color: "inherit"
                                                             })
                                                         })]
                                                     }), (0, e.jsx)(Nr, {
                                                         item: !0,
                                                         xs: 1
@@ -28985,78 +29007,79 @@
                                             container: !0,
                                             justifyContent: "space-between",
                                             children: (0, e.jsx)(Qn, {
                                                 variant: "h6",
                                                 children: "Pipelines"
                                             })
                                         }), k && k.map(((t, n) => {
-                                            const [r, o] = t;
+                                            const [r, o, i] = t;
                                             return (0, e.jsx)(by, {
-                                                active: O,
+                                                active: T,
                                                 number: n,
                                                 id: r,
                                                 label: o,
-                                                submitEntity: V,
-                                                enableScenarioFields: C,
+                                                submitEntity: q,
+                                                enableScenarioFields: _,
                                                 submit: d,
-                                                editLabel: de,
-                                                onFocus: K,
-                                                focusName: q,
-                                                setFocusName: X
+                                                editLabel: fe,
+                                                onFocus: Q,
+                                                focusName: K,
+                                                setFocusName: Z,
+                                                submittable: i
                                             }, r)
                                         })), (0, e.jsx)(Nr, {
                                             item: !0,
                                             xs: 12,
                                             children: (0, e.jsx)(ny, {})
                                         })]
                                     }) : null, (0, e.jsxs)(Nr, {
                                         item: !0,
                                         xs: 12,
                                         container: !0,
                                         justifyContent: "space-between",
                                         children: [s ? (0, e.jsx)(Ln, {
                                             variant: "outlined",
                                             color: "primary",
-                                            disabled: !O || !C || !E,
-                                            onClick: j,
+                                            disabled: !T || !_ || !E,
+                                            onClick: R,
                                             children: "DELETE"
                                         }) : null, (0, e.jsx)(Ln, {
                                             variant: "outlined",
                                             color: "primary",
-                                            disabled: !O || !C || v,
-                                            onClick: L,
+                                            disabled: !T || !_ || v || !C,
+                                            onClick: F,
                                             children: "PROMOTE TO PRIMARY"
                                         })]
                                     })]
                                 })
                             })]
                         }), (0, e.jsx)(Ft, {
                             children: n.error
                         })]
                     }), (0, e.jsx)(sg, {
                         title: "Delete Scenario",
                         message: "Are you sure you want to delete this scenario?",
                         confirm: "Delete",
-                        open: P,
-                        onClose: A,
-                        onConfirm: R
+                        open: j,
+                        onClose: I,
+                        onConfirm: N
                     }), (0, e.jsx)(sg, {
                         title: "Promote Scenario",
                         message: "Are you sure you want to promote this scenario?",
                         confirm: "Promote",
-                        open: I,
-                        onClose: D,
-                        onConfirm: F
+                        open: L,
+                        onClose: $,
+                        onConfirm: z
                     })]
                 })
             };
-        var wy, ky = i(6486);
-        class Sy {
+        var ky, Sy = i(6486);
+        class Ey {
             static UID() {
-                return Sy.TESTING ? (Sy.TESTING_UID++, `${Sy.TESTING_UID}`) : "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, (e => {
+                return Ey.TESTING ? (Ey.TESTING_UID++, `${Ey.TESTING_UID}`) : "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, (e => {
                     const t = 16 * Math.random() | 0;
                     return ("x" === e ? t : 3 & t | 8).toString(16)
                 }))
             }
             static closest(e, t) {
                 return Element.prototype.closest || (Element.prototype.closest = function(e) {
                     var t = this;
@@ -29064,16 +29087,16 @@
                         if (Element.prototype.matches.call(t, e)) return t;
                         t = t.parentElement || t.parentNode
                     } while (null !== t && 1 === t.nodeType);
                     return null
                 }), e.closest(t)
             }
         }
-        Sy.TESTING = !1, Sy.TESTING_UID = 0;
-        class Ey {
+        Ey.TESTING = !1, Ey.TESTING_UID = 0;
+        class Cy {
             constructor() {
                 this.listeners = {}
             }
             fireEventInternal(e, t, n) {
                 this.iterateListeners((r => {
                     if (!e && !n.firing) return !1;
                     r[t] && r[t](n)
@@ -29102,35 +29125,35 @@
                         listener: e,
                         deregister: () => {
                             delete this.listeners[t]
                         }
                     }
             }
             registerListener(e) {
-                const t = Sy.UID();
+                const t = Ey.UID();
                 return this.listeners[t] = e, {
                     id: t,
                     listener: e,
                     deregister: () => {
                         delete this.listeners[t]
                     }
                 }
             }
             deregisterListener(e) {
                 if ("object" == typeof e) return e.deregister(), !0;
                 const t = this.getListenerHandle(e);
                 return !!t && (t.deregister(), !0)
             }
         }
-        class Cy extends Ey {
+        class Oy extends Cy {
             constructor() {
                 super(), this.factories = {}
             }
             getFactories() {
-                return ky.values(this.factories)
+                return Sy.values(this.factories)
             }
             clearFactories() {
                 for (let e in this.factories) this.deregisterFactory(e)
             }
             getFactory(e) {
                 if (!this.factories[e]) throw new Error(`Cannot find factory with type [${e}]`);
                 return this.factories[e]
@@ -29143,15 +29166,15 @@
             deregisterFactory(e) {
                 const t = this.factories[e];
                 t.setFactoryBank(null), delete this.factories[e], this.fireEvent({
                     factory: t
                 }, "factoryRemoved")
             }
         }
-        class Oy {
+        class _y {
             constructor(e) {
                 this.matrix = e
             }
             mmul(e) {
                 return this.matrix = this.matrix.map(((t, n) => e.asArray()[0].map(((r, o) => t.reduce(((t, r, i) => t + this.matrix[n][i] * e.asArray()[i][o]), 0))))), this
             }
             asArray() {
@@ -29162,161 +29185,161 @@
             }
             static multiply(...e) {
                 let t = e[0];
                 for (let n = 1; n < e.length; n++) t = t.mmul(e[n]);
                 return t
             }
             static scaleMatrix(e, t) {
-                return new Oy([
+                return new _y([
                     [e, 0, 0],
                     [0, t, 0],
                     [0, 0, 1]
                 ])
             }
             static translateMatrix(e, t) {
-                return new Oy([
+                return new _y([
                     [1, 0, e],
                     [0, 1, t],
                     [0, 0, 1]
                 ])
             }
             static rotateMatrix(e) {
-                return new Oy([
+                return new _y([
                     [Math.cos(e), -1 * Math.sin(e), 0],
                     [Math.sin(e), Math.cos(e), 0],
                     [0, 0, 1]
                 ])
             }
             static createScaleMatrix(e, t, n) {
-                return this.multiply(Oy.translateMatrix(n.x, n.y), Oy.scaleMatrix(e, t), Oy.translateMatrix(-n.x, -n.y))
+                return this.multiply(_y.translateMatrix(n.x, n.y), _y.scaleMatrix(e, t), _y.translateMatrix(-n.x, -n.y))
             }
             static createRotateMatrix(e, t) {
-                return this.multiply(Oy.translateMatrix(t.x, t.y), Oy.rotateMatrix(e), Oy.translateMatrix(-t.x, -t.y))
+                return this.multiply(_y.translateMatrix(t.x, t.y), _y.rotateMatrix(e), _y.translateMatrix(-t.x, -t.y))
             }
         }
-        class _y {
+        class Ty {
             constructor(e = 0, t = 0) {
                 this.x = e, this.y = t
             }
             translate(e, t) {
                 this.x += e, this.y += t
             }
             clone() {
-                return new _y(this.x, this.y)
+                return new Ty(this.x, this.y)
             }
             toSVG() {
                 return this.x + " " + this.y
             }
             asMatrix() {
-                return new Oy([
+                return new _y([
                     [this.x],
                     [this.y],
                     [1]
                 ])
             }
             transform(e) {
                 let t = e.mmul(this.asMatrix());
                 this.x = t.get(0, 0), this.y = t.get(1, 0)
             }
             static middlePoint(e, t) {
-                return new _y((t.x + e.x) / 2, (t.y + e.y) / 2)
+                return new Ty((t.x + e.x) / 2, (t.y + e.y) / 2)
             }
         }! function(e) {
             e.TOP_LEFT = "TL", e.TOP_RIGHT = "TR", e.BOTTOM_RIGHT = "BR", e.BOTTOM_LEFT = "BL"
-        }(wy || (wy = {}));
-        const Ty = (e, t, n, r) => ({
-                [wy.TOP_LEFT]: new _y(e, t),
-                [wy.TOP_RIGHT]: new _y(e + n, t),
-                [wy.BOTTOM_RIGHT]: new _y(e + n, t + r),
-                [wy.BOTTOM_LEFT]: new _y(e, t + r)
+        }(ky || (ky = {}));
+        const Py = (e, t, n, r) => ({
+                [ky.TOP_LEFT]: new Ty(e, t),
+                [ky.TOP_RIGHT]: new Ty(e + n, t),
+                [ky.BOTTOM_RIGHT]: new Ty(e + n, t + r),
+                [ky.BOTTOM_LEFT]: new Ty(e, t + r)
             }),
-            Py = () => ({
-                [wy.TOP_LEFT]: new _y,
-                [wy.TOP_RIGHT]: new _y,
-                [wy.BOTTOM_RIGHT]: new _y,
-                [wy.BOTTOM_LEFT]: new _y
+            My = () => ({
+                [ky.TOP_LEFT]: new Ty,
+                [ky.TOP_RIGHT]: new Ty,
+                [ky.BOTTOM_RIGHT]: new Ty,
+                [ky.BOTTOM_LEFT]: new Ty
             }),
-            My = e => {
-                if (0 === e.length) return Py();
+            jy = e => {
+                if (0 === e.length) return My();
                 let t = e[0].x,
                     n = e[0].x,
                     r = e[0].y,
                     o = e[0].y;
                 for (let i = 1; i < e.length; i++) e[i].x < t && (t = e[i].x), e[i].x > n && (n = e[i].x), e[i].y < r && (r = e[i].y), e[i].y > o && (o = e[i].y);
                 return {
-                    [wy.TOP_LEFT]: new _y(t, r),
-                    [wy.TOP_RIGHT]: new _y(n, r),
-                    [wy.BOTTOM_RIGHT]: new _y(n, o),
-                    [wy.BOTTOM_LEFT]: new _y(t, o)
+                    [ky.TOP_LEFT]: new Ty(t, r),
+                    [ky.TOP_RIGHT]: new Ty(n, r),
+                    [ky.BOTTOM_RIGHT]: new Ty(n, o),
+                    [ky.BOTTOM_LEFT]: new Ty(t, o)
                 }
             };
-        class jy {
+        class Ay {
             constructor(e = []) {
                 this.points = e
             }
             serialize() {
-                return ky.map(this.points, (e => [e.x, e.y]))
+                return Sy.map(this.points, (e => [e.x, e.y]))
             }
             deserialize(e) {
-                this.points = ky.map(e, (e => new _y(e[0], e[1])))
+                this.points = Sy.map(e, (e => new Ty(e[0], e[1])))
             }
             scale(e, t, n) {
-                let r = Oy.createScaleMatrix(e, t, n);
-                ky.forEach(this.points, (e => {
+                let r = _y.createScaleMatrix(e, t, n);
+                Sy.forEach(this.points, (e => {
                     e.transform(r)
                 }))
             }
             transform(e) {
-                ky.forEach(this.points, (t => {
+                Sy.forEach(this.points, (t => {
                     t.transform(e)
                 }))
             }
             setPoints(e) {
                 this.points = e
             }
             getPoints() {
                 return this.points
             }
             rotate(e) {
-                this.transform(Oy.createRotateMatrix(e / (180 / Math.PI), this.getOrigin()))
+                this.transform(_y.createRotateMatrix(e / (180 / Math.PI), this.getOrigin()))
             }
             translate(e, t) {
-                ky.forEach(this.points, (n => {
+                Sy.forEach(this.points, (n => {
                     n.translate(e, t)
                 }))
             }
             doClone(e) {
-                this.points = ky.map(e.points, (e => e.clone()))
+                this.points = Sy.map(e.points, (e => e.clone()))
             }
             clone() {
                 let e = Object.create(this);
                 return e.doClone(this), e
             }
             getOrigin() {
                 if (0 === this.points.length) return null;
-                let e = My(this.points);
-                return _y.middlePoint(e[wy.TOP_LEFT], e[wy.BOTTOM_RIGHT])
+                let e = jy(this.points);
+                return Ty.middlePoint(e[ky.TOP_LEFT], e[ky.BOTTOM_RIGHT])
             }
             getBoundingBox() {
-                return My(this.points)
+                return jy(this.points)
             }
         }
-        class Ay extends jy {
+        class Ry extends Ay {
             static fromPositionAndSize(e, t, n, r) {
-                return new Ay(Ty(e, t, n, r))
+                return new Ry(Py(e, t, n, r))
             }
             static fromPointAndSize(e, t, n) {
-                return new Ay(Ty(e.x, e.y, t, n))
+                return new Ry(Py(e.x, e.y, t, n))
             }
             constructor(e) {
-                e || (e = Py()), super([e[wy.TOP_LEFT], e[wy.TOP_RIGHT], e[wy.BOTTOM_RIGHT], e[wy.BOTTOM_LEFT]])
+                e || (e = My()), super([e[ky.TOP_LEFT], e[ky.TOP_RIGHT], e[ky.BOTTOM_RIGHT], e[ky.BOTTOM_LEFT]])
             }
             updateDimensions(e, t, n, r) {
-                const o = Ty(e, t, n, r);
-                this.setPoints([o[wy.TOP_LEFT], o[wy.TOP_RIGHT], o[wy.BOTTOM_RIGHT], o[wy.BOTTOM_LEFT]])
+                const o = Py(e, t, n, r);
+                this.setPoints([o[ky.TOP_LEFT], o[ky.TOP_RIGHT], o[ky.BOTTOM_RIGHT], o[ky.BOTTOM_LEFT]])
             }
             setPoints(e) {
                 if (4 !== e.length) throw "Rectangles must always have 4 points";
                 super.setPoints(e)
             }
             containsPoint(e) {
                 const t = this.getTopLeft(),
@@ -29326,122 +29349,122 @@
             getWidth() {
                 return Math.sqrt(Math.pow(this.getTopLeft().x - this.getTopRight().x, 2) + Math.pow(this.getTopLeft().y - this.getTopRight().y, 2))
             }
             getHeight() {
                 return Math.sqrt(Math.pow(this.getBottomLeft().x - this.getTopLeft().x, 2) + Math.pow(this.getBottomLeft().y - this.getTopLeft().y, 2))
             }
             getTopMiddle() {
-                return _y.middlePoint(this.getTopLeft(), this.getTopRight())
+                return Ty.middlePoint(this.getTopLeft(), this.getTopRight())
             }
             getBottomMiddle() {
-                return _y.middlePoint(this.getBottomLeft(), this.getBottomRight())
+                return Ty.middlePoint(this.getBottomLeft(), this.getBottomRight())
             }
             getLeftMiddle() {
-                return _y.middlePoint(this.getBottomLeft(), this.getTopLeft())
+                return Ty.middlePoint(this.getBottomLeft(), this.getTopLeft())
             }
             getRightMiddle() {
-                return _y.middlePoint(this.getBottomRight(), this.getTopRight())
+                return Ty.middlePoint(this.getBottomRight(), this.getTopRight())
             }
             getTopLeft() {
                 return this.points[0]
             }
             getTopRight() {
                 return this.points[1]
             }
             getBottomRight() {
                 return this.points[2]
             }
             getBottomLeft() {
                 return this.points[3]
             }
         }
-        var Ry, Iy, Ny, Ly, Dy, Fy;
+        var Iy, Ny, Ly, Dy, Fy, $y;
         ! function(e) {
             e[e.SOURCE = 0] = "SOURCE", e[e.SOURCE_CONTROL = 1] = "SOURCE_CONTROL", e[e.TARGET_CONTROL = 2] = "TARGET_CONTROL", e[e.TARGET = 3] = "TARGET"
-        }(Ry || (Ry = {}));
-        class $y extends jy {
+        }(Iy || (Iy = {}));
+        class zy extends Ay {
             constructor() {
-                super([new _y(0, 0), new _y(0, 0), new _y(0, 0), new _y(0, 0)])
+                super([new Ty(0, 0), new Ty(0, 0), new Ty(0, 0), new Ty(0, 0)])
             }
             getSVGCurve() {
                 return `M${this.getSource().toSVG()} C${this.getSourceControl().toSVG()}, ${this.getTargetControl().toSVG()}, ${this.getTarget().toSVG()}`
             }
             setPoints(e) {
                 if (4 !== e.length) throw new Error("BezierCurve must have extactly 4 points");
                 super.setPoints(e)
             }
             getSource() {
-                return this.points[Ry.SOURCE]
+                return this.points[Iy.SOURCE]
             }
             getSourceControl() {
-                return this.points[Ry.SOURCE_CONTROL]
+                return this.points[Iy.SOURCE_CONTROL]
             }
             getTargetControl() {
-                return this.points[Ry.TARGET_CONTROL]
+                return this.points[Iy.TARGET_CONTROL]
             }
             getTarget() {
-                return this.points[Ry.TARGET]
+                return this.points[Iy.TARGET]
             }
             setSource(e) {
-                this.points[Ry.SOURCE] = e
+                this.points[Iy.SOURCE] = e
             }
             setSourceControl(e) {
-                this.points[Ry.SOURCE_CONTROL] = e
+                this.points[Iy.SOURCE_CONTROL] = e
             }
             setTargetControl(e) {
-                this.points[Ry.TARGET_CONTROL] = e
+                this.points[Iy.TARGET_CONTROL] = e
             }
             setTarget(e) {
-                this.points[Ry.TARGET] = e
+                this.points[Iy.TARGET] = e
             }
-        }(Fy = Iy || (Iy = {})).MOUSE_DOWN = "mouse-down", Fy.MOUSE_UP = "mouse-up", Fy.MOUSE_MOVE = "mouse-move", Fy.MOUSE_WHEEL = "mouse-wheel", Fy.KEY_DOWN = "key-down", Fy.KEY_UP = "key-up", Fy.TOUCH_START = "touch-start", Fy.TOUCH_END = "touch-end", Fy.TOUCH_MOVE = "touch-move";
-        class zy {
+        }($y = Ny || (Ny = {})).MOUSE_DOWN = "mouse-down", $y.MOUSE_UP = "mouse-up", $y.MOUSE_MOVE = "mouse-move", $y.MOUSE_WHEEL = "mouse-wheel", $y.KEY_DOWN = "key-down", $y.KEY_UP = "key-up", $y.TOUCH_START = "touch-start", $y.TOUCH_END = "touch-end", $y.TOUCH_MOVE = "touch-move";
+        class Wy {
             constructor(e) {
-                this.options = e, this.id = Sy.UID()
+                this.options = e, this.id = Ey.UID()
             }
             setEngine(e) {
                 this.engine = e
             }
         }
-        class Wy {
+        class By {
             constructor(e) {
                 this.actions = {}, this.engine = e, this.keys = {}
             }
             getKeys() {
-                return ky.keys(this.keys)
+                return Sy.keys(this.keys)
             }
             registerAction(e) {
                 return e.setEngine(this.engine), this.actions[e.id] = e, () => {
                     this.deregisterAction(e)
                 }
             }
             deregisterAction(e) {
                 e.setEngine(null), delete this.actions[e.id]
             }
             getActionsForType(e) {
-                return ky.filter(this.actions, (t => t.options.type === e))
+                return Sy.filter(this.actions, (t => t.options.type === e))
             }
             getModelForEvent(e) {
                 return e.model ? e.model : this.engine.getMouseElement(e.event)
             }
             getActionsForEvent(e) {
                 const {
                     event: t
                 } = e;
-                return "mousedown" === t.type ? this.getActionsForType(Iy.MOUSE_DOWN) : "mouseup" === t.type ? this.getActionsForType(Iy.MOUSE_UP) : "keydown" === t.type ? (this.keys[t.key.toLowerCase()] = !0, this.getActionsForType(Iy.KEY_DOWN)) : "keyup" === t.type ? (delete this.keys[t.key.toLowerCase()], this.getActionsForType(Iy.KEY_UP)) : "mousemove" === t.type ? this.getActionsForType(Iy.MOUSE_MOVE) : "wheel" === t.type ? this.getActionsForType(Iy.MOUSE_WHEEL) : "touchstart" === t.type ? this.getActionsForType(Iy.TOUCH_START) : "touchend" === t.type ? this.getActionsForType(Iy.TOUCH_END) : "touchmove" === t.type ? this.getActionsForType(Iy.TOUCH_MOVE) : []
+                return "mousedown" === t.type ? this.getActionsForType(Ny.MOUSE_DOWN) : "mouseup" === t.type ? this.getActionsForType(Ny.MOUSE_UP) : "keydown" === t.type ? (this.keys[t.key.toLowerCase()] = !0, this.getActionsForType(Ny.KEY_DOWN)) : "keyup" === t.type ? (delete this.keys[t.key.toLowerCase()], this.getActionsForType(Ny.KEY_UP)) : "mousemove" === t.type ? this.getActionsForType(Ny.MOUSE_MOVE) : "wheel" === t.type ? this.getActionsForType(Ny.MOUSE_WHEEL) : "touchstart" === t.type ? this.getActionsForType(Ny.TOUCH_START) : "touchend" === t.type ? this.getActionsForType(Ny.TOUCH_END) : "touchmove" === t.type ? this.getActionsForType(Ny.TOUCH_MOVE) : []
             }
             fireAction(e) {
                 const t = this.getActionsForEvent(e);
                 for (let n of t) n.options.fire(e)
             }
         }
-        class By extends zy {
+        class Uy extends Wy {
             constructor(e = {}) {
                 super({
-                    type: Iy.MOUSE_WHEEL,
+                    type: Ny.MOUSE_WHEEL,
                     fire: t => {
                         const {
                             event: n
                         } = t;
                         for (let e of this.engine.getModel().getLayers()) e.allowRepaint(!1);
                         const r = this.engine.getModel();
                         if (n.stopPropagation(), n.ctrlKey) {
@@ -29466,18 +29489,18 @@
                         }
                         this.engine.repaintCanvas();
                         for (let e of this.engine.getModel().getLayers()) e.allowRepaint(!0)
                     }
                 })
             }
         }
-        class Uy extends zy {
+        class Yy extends Wy {
             constructor(e = {}) {
                 super({
-                    type: Iy.MOUSE_WHEEL,
+                    type: Ny.MOUSE_WHEEL,
                     fire: t => {
                         const {
                             event: n
                         } = t;
                         for (let e of this.engine.getModel().getLayers()) e.allowRepaint(!1);
                         const r = this.engine.getModel();
                         n.stopPropagation();
@@ -29496,83 +29519,83 @@
                             g = (f - r.getOffsetY()) / o / u;
                         r.setOffset(r.getOffsetX() - c * h, r.getOffsetY() - d * g), this.engine.repaintCanvas();
                         for (let e of this.engine.getModel().getLayers()) e.allowRepaint(!0)
                     }
                 })
             }
         }
-        class Yy extends zy {
+        class Hy extends Wy {
             constructor(e = {}) {
                 const t = e.keyCodes || [46, 8],
                     n = Object.assign({
                         ctrlKey: !1,
                         shiftKey: !1,
                         altKey: !1,
                         metaKey: !1
                     }, e.modifiers);
                 super({
-                    type: Iy.KEY_DOWN,
+                    type: Ny.KEY_DOWN,
                     fire: e => {
                         const {
                             keyCode: r,
                             ctrlKey: o,
                             shiftKey: i,
                             altKey: a,
                             metaKey: s
-                        } = e.event; - 1 !== t.indexOf(r) && ky.isEqual({
+                        } = e.event; - 1 !== t.indexOf(r) && Sy.isEqual({
                             ctrlKey: o,
                             shiftKey: i,
                             altKey: a,
                             metaKey: s
-                        }, n) && (ky.forEach(this.engine.getModel().getSelectedEntities(), (e => {
+                        }, n) && (Sy.forEach(this.engine.getModel().getSelectedEntities(), (e => {
                             e.isLocked() || e.remove()
                         })), this.engine.repaintCanvas())
                     }
                 })
             }
         }
-        class Hy extends Ey {
+        class Vy extends Cy {
             constructor(e) {
                 super(), this.engine = e, this.stateStack = []
             }
             getCurrentState() {
                 return this.currentState
             }
             pushState(e) {
                 this.stateStack.push(e), this.setState(e)
             }
             popState() {
-                this.stateStack.pop(), this.setState(ky.last(this.stateStack))
+                this.stateStack.pop(), this.setState(Sy.last(this.stateStack))
             }
             setState(e) {
                 e.setEngine(this.engine), this.currentState && this.currentState.deactivated(e);
                 const t = this.currentState;
                 this.currentState = e, this.currentState && (this.currentState.activated(t), this.fireEvent({
                     newState: e
                 }, "stateChanged"))
             }
         }
-        class Vy extends Ey {
+        class Gy extends Cy {
             constructor(e = {}) {
-                super(), this.model = null, this.eventBus = new Wy(this), this.stateMachine = new Hy(this), this.layerFactories = new Cy, this.registerFactoryBank(this.layerFactories), this.options = Object.assign({
+                super(), this.model = null, this.eventBus = new By(this), this.stateMachine = new Vy(this), this.layerFactories = new Oy, this.registerFactoryBank(this.layerFactories), this.options = Object.assign({
                     registerDefaultDeleteItemsAction: !0,
                     registerDefaultZoomCanvasAction: !0,
                     repaintDebounceMs: 0
-                }, e), !0 === this.options.registerDefaultZoomCanvasAction ? this.eventBus.registerAction(new Uy) : !0 === this.options.registerDefaultPanAndZoomCanvasAction && this.eventBus.registerAction(new By), !0 === this.options.registerDefaultDeleteItemsAction && this.eventBus.registerAction(new Yy)
+                }, e), !0 === this.options.registerDefaultZoomCanvasAction ? this.eventBus.registerAction(new Yy) : !0 === this.options.registerDefaultPanAndZoomCanvasAction && this.eventBus.registerAction(new Uy), !0 === this.options.registerDefaultDeleteItemsAction && this.eventBus.registerAction(new Hy)
             }
             getStateMachine() {
                 return this.stateMachine
             }
             getRelativeMousePoint(e) {
                 const t = this.getRelativePoint(e.clientX, e.clientY);
-                return new _y((t.x - this.model.getOffsetX()) / (this.model.getZoomLevel() / 100), (t.y - this.model.getOffsetY()) / (this.model.getZoomLevel() / 100))
+                return new Ty((t.x - this.model.getOffsetX()) / (this.model.getZoomLevel() / 100), (t.y - this.model.getOffsetY()) / (this.model.getZoomLevel() / 100))
             }
             getRelativePoint(e, t) {
                 const n = this.canvas.getBoundingClientRect();
-                return new _y(e - n.left, t - n.top)
+                return new Ty(e - n.left, t - n.top)
             }
             registerFactoryBank(e) {
                 e.registerListener({
                     factoryAdded: e => {
                         e.factory.setDiagramEngine(this)
                     },
                     factoryRemoved: e => {
@@ -29602,15 +29625,15 @@
                     repaintDebounceMs: t
                 } = this.options, n = () => {
                     this.iterateListeners((e => {
                         e.repaintCanvas && e.repaintCanvas()
                     }))
                 };
                 let r = n;
-                if (t > 0 && (r = (0, ky.debounce)(n, t)), e) return new Promise((e => {
+                if (t > 0 && (r = (0, Sy.debounce)(n, t)), e) return new Promise((e => {
                     const t = this.registerListener({
                         rendered: () => {
                             e(), t.deregister()
                         }
                     });
                     r()
                 }));
@@ -29628,32 +29651,32 @@
             zoomToFit() {
                 const e = this.canvas.clientWidth / this.canvas.scrollWidth,
                     t = this.canvas.clientHeight / this.canvas.scrollHeight,
                     n = e < t ? e : t;
                 this.model.setZoomLevel(this.model.getZoomLevel() * n), this.model.setOffset(0, 0), this.repaintCanvas()
             }
         }
-        class Gy extends Ey {
+        class qy extends Cy {
             constructor(e = {}) {
                 super(), this.options = Object.assign({
-                    id: Sy.UID()
+                    id: Ey.UID()
                 }, e)
             }
             getOptions() {
                 return this.options
             }
             getID() {
                 return this.options.id
             }
             doClone(e = {}, t) {}
             clone(e = {}) {
                 if (e[this.options.id]) return e[this.options.id];
-                let t = ky.cloneDeep(this);
+                let t = Sy.cloneDeep(this);
                 return t.options = Object.assign(Object.assign({}, this.options), {
-                    id: Sy.UID()
+                    id: Ey.UID()
                 }), t.clearListeners(), e[this.options.id] = t, this.doClone(e, t), t
             }
             clearListeners() {
                 this.listeners = {}
             }
             deserialize(e) {
                 this.options.id = e.data.id, this.options.locked = e.data.locked
@@ -29674,36 +29697,36 @@
             }
             setLocked(e = !0) {
                 this.options.locked = e, this.fireEvent({
                     locked: e
                 }, "lockChanged")
             }
         }
-        class qy extends Gy {
+        class Xy extends qy {
             constructor(e = {}) {
                 super(Object.assign({
                     zoom: 100,
                     gridSize: 0,
                     offsetX: 0,
                     offsetY: 0
                 }, e)), this.layers = []
             }
             getSelectionEntities() {
-                return ky.flatMap(this.layers, (e => e.getSelectionEntities()))
+                return Sy.flatMap(this.layers, (e => e.getSelectionEntities()))
             }
             getSelectedEntities() {
-                return ky.filter(this.getSelectionEntities(), (e => e.isSelected()))
+                return Sy.filter(this.getSelectionEntities(), (e => e.isSelected()))
             }
             clearSelection() {
-                ky.forEach(this.getSelectedEntities(), (e => {
+                Sy.forEach(this.getSelectedEntities(), (e => {
                     e.setSelected(!1)
                 }))
             }
             getModels() {
-                return ky.flatMap(this.layers, (e => ky.values(e.getModels())))
+                return Sy.flatMap(this.layers, (e => Sy.values(e.getModels())))
             }
             addLayer(e) {
                 e.setParent(this), e.registerListener({
                     entityRemoved: e => {}
                 }), this.layers.push(e)
             }
             removeLayer(e) {
@@ -29734,30 +29757,30 @@
                         getModel: e => n[e] ? Promise.resolve(n[e]) : (r[e] || (r[e] = new Promise((t => {
                             o[e] = t
                         }))), r[e])
                     };
                 this.deserialize(i)
             }
             deserialize(e) {
-                super.deserialize(e), this.options.offsetX = e.data.offsetX, this.options.offsetY = e.data.offsetY, this.options.zoom = e.data.zoom, this.options.gridSize = e.data.gridSize, ky.forEach(e.data.layers, (t => {
+                super.deserialize(e), this.options.offsetX = e.data.offsetX, this.options.offsetY = e.data.offsetY, this.options.zoom = e.data.zoom, this.options.gridSize = e.data.gridSize, Sy.forEach(e.data.layers, (t => {
                     const n = e.engine.getFactoryForLayer(t.type).generateModel({
                         initialConfig: t
                     });
                     n.deserialize(Object.assign(Object.assign({}, e), {
                         data: t
                     })), this.addLayer(n)
                 }))
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     offsetX: this.options.offsetX,
                     offsetY: this.options.offsetY,
                     zoom: this.options.zoom,
                     gridSize: this.options.gridSize,
-                    layers: ky.map(this.layers, (e => e.serialize()))
+                    layers: Sy.map(this.layers, (e => e.serialize()))
                 })
             }
             setZoomLevel(e) {
                 this.options.zoom = e, this.fireEvent({
                     zoom: e
                 }, "zoomUpdated")
             }
@@ -29779,39 +29802,39 @@
             getOffsetX() {
                 return this.options.offsetX
             }
             getZoomLevel() {
                 return this.options.zoom
             }
         }
-        class Xy {
+        class Ky {
             constructor(e) {
                 this.type = e
             }
             setDiagramEngine(e) {
                 this.engine = e
             }
             setFactoryBank(e) {
                 this.bank = e
             }
             getType() {
                 return this.type
             }
         }
-        class Ky extends Xy {}
         class Zy extends Ky {}
-        class Qy extends Gy {
+        class Qy extends Zy {}
+        class Jy extends qy {
             constructor(e) {
                 super(e)
             }
             performanceTune() {
                 return !0
             }
             getParentCanvasModel() {
-                return this.parent ? this.parent instanceof qy ? this.parent : this.parent instanceof Qy ? this.parent.getParentCanvasModel() : null : null
+                return this.parent ? this.parent instanceof Xy ? this.parent : this.parent instanceof Jy ? this.parent.getParentCanvasModel() : null : null
             }
             getParent() {
                 return this.parent
             }
             setParent(e) {
                 this.parent = e
             }
@@ -29842,26 +29865,26 @@
                     isSelected: e
                 }, "selectionChanged"))
             }
             remove() {
                 this.fireEvent({}, "entityRemoved")
             }
         }
-        class Jy extends Qy {
+        class eb extends Jy {
             constructor(e) {
-                super(e), this.position = e.position || new _y(0, 0)
+                super(e), this.position = e.position || new Ty(0, 0)
             }
             setPosition(e, t) {
-                this.position = e instanceof _y ? e : new _y(e, t), this.fireEvent({}, "positionChanged")
+                this.position = e instanceof Ty ? e : new Ty(e, t), this.fireEvent({}, "positionChanged")
             }
             getBoundingBox() {
-                return Ay.fromPointAndSize(this.position, 0, 0)
+                return Ry.fromPointAndSize(this.position, 0, 0)
             }
             deserialize(e) {
-                super.deserialize(e), this.position = new _y(e.data.x, e.data.y)
+                super.deserialize(e), this.position = new Ty(e.data.x, e.data.y)
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     x: this.position.x,
                     y: this.position.y
                 })
             }
@@ -29888,53 +29911,53 @@
 		overflow: visible;
 	`;
             e.DivLayer = b.default.div`
 		${t}
 	`, e.SvgLayer = b.default.svg`
 		${t}
 	`
-        }(Ny || (Ny = {}));
-        class eb extends t.Component {
+        }(Ly || (Ly = {}));
+        class tb extends t.Component {
             constructor(e) {
                 super(e), this.state = {}
             }
             getTransform() {
                 const e = this.props.layer.getParent();
                 return `\n\t\t\ttranslate(\n\t\t\t\t${e.getOffsetX()}px,\n\t\t\t\t${e.getOffsetY()}px)\n\t\t\tscale(\n\t\t\t\t${e.getZoomLevel()/100}\n\t\t\t)\n  \t`
             }
             getTransformStyle() {
                 return this.props.layer.getOptions().transformed ? {
                     transform: this.getTransform()
                 } : {}
             }
             render() {
-                return this.props.layer.getOptions().isSvg ? t.createElement(Ny.SvgLayer, {
+                return this.props.layer.getOptions().isSvg ? t.createElement(Ly.SvgLayer, {
                     style: this.getTransformStyle()
-                }, this.props.children) : t.createElement(Ny.DivLayer, {
+                }, this.props.children) : t.createElement(Ly.DivLayer, {
                     style: this.getTransformStyle()
                 }, this.props.children)
             }
         }
-        class tb extends t.Component {
+        class nb extends t.Component {
             shouldComponentUpdate() {
                 return this.props.layer.isRepaintEnabled()
             }
             render() {
                 return this.props.engine.getFactoryForLayer(this.props.layer).generateReactWidget({
                     model: this.props.layer
                 })
             }
         }! function(e) {
             e.Canvas = b.default.div`
 		position: relative;
 		cursor: move;
 		overflow: hidden;
 	`
-        }(Ly || (Ly = {}));
-        class nb extends t.Component {
+        }(Dy || (Dy = {}));
+        class rb extends t.Component {
             constructor(e) {
                 super(e), this.ref = t.createRef(), this.state = {
                     action: null,
                     diagramEngineListener: null
                 }
             }
             componentWillUnmount() {
@@ -29961,15 +29984,15 @@
                     this.props.engine.getActionEventBus().fireAction({
                         event: e
                     })
                 }, document.addEventListener("keyup", this.keyUp), document.addEventListener("keydown", this.keyDown), this.registerCanvas()
             }
             render() {
                 const e = this.props.engine.getModel();
-                return t.createElement(Ly.Canvas, {
+                return t.createElement(Dy.Canvas, {
                     className: this.props.className,
                     ref: this.ref,
                     onWheel: e => {
                         this.props.engine.getActionEventBus().fireAction({
                             event: e
                         })
                     },
@@ -29999,43 +30022,43 @@
                         })
                     },
                     onTouchMove: e => {
                         this.props.engine.getActionEventBus().fireAction({
                             event: e
                         })
                     }
-                }, e.getLayers().map((e => t.createElement(eb, {
+                }, e.getLayers().map((e => t.createElement(tb, {
                     layer: e,
                     key: e.getID()
-                }, t.createElement(tb, {
+                }, t.createElement(nb, {
                     layer: e,
                     engine: this.props.engine,
                     key: e.getID()
                 })))))
             }
         }
-        class rb extends Qy {
+        class ob extends Jy {
             constructor(e = {}) {
                 super(e), this.models = {}, this.repaintEnabled = !0
             }
             deserialize(e) {
-                super.deserialize(e), this.options.isSvg = !!e.data.isSvg, this.options.transformed = !!e.data.transformed, ky.forEach(e.data.models, (t => {
+                super.deserialize(e), this.options.isSvg = !!e.data.isSvg, this.options.transformed = !!e.data.transformed, Sy.forEach(e.data.models, (t => {
                     const n = this.getChildModelFactoryBank(e.engine).getFactory(t.type).generateModel({
                         initialConfig: t
                     });
                     n.deserialize(Object.assign(Object.assign({}, e), {
                         data: t
                     })), this.addModel(n)
                 }))
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     isSvg: this.options.isSvg,
                     transformed: this.options.transformed,
-                    models: ky.mapValues(this.models, (e => e.serialize()))
+                    models: Sy.mapValues(this.models, (e => e.serialize()))
                 })
             }
             isRepaintEnabled() {
                 return this.repaintEnabled
             }
             allowRepaint(e = !0) {
                 this.repaintEnabled = e
@@ -30043,28 +30066,28 @@
             remove() {
                 this.parent && this.parent.removeLayer(this), super.remove()
             }
             addModel(e) {
                 e.setParent(this), this.models[e.getID()] = e
             }
             getSelectionEntities() {
-                return ky.flatMap(this.models, (e => e.getSelectionEntities()))
+                return Sy.flatMap(this.models, (e => e.getSelectionEntities()))
             }
             getModels() {
                 return this.models
             }
             getModel(e) {
                 return this.models[e]
             }
             removeModel(e) {
                 const t = "string" == typeof e ? e : e.getID();
                 return !!this.models[t] && (delete this.models[t], !0)
             }
         }
-        class ob extends rb {
+        class ib extends ob {
             constructor() {
                 super({
                     transformed: !1,
                     isSvg: !1,
                     type: "selection"
                 })
             }
@@ -30076,52 +30099,52 @@
             }
         }! function(e) {
             e.Container = b.default.div`
 		position: absolute;
 		background-color: rgba(0, 192, 255, 0.2);
 		border: solid 2px rgb(0, 192, 255);
 	`
-        }(Dy || (Dy = {}));
-        class ib extends t.Component {
+        }(Fy || (Fy = {}));
+        class ab extends t.Component {
             render() {
                 const {
                     rect: e
                 } = this.props;
-                return e ? t.createElement(Dy.Container, {
+                return e ? t.createElement(Fy.Container, {
                     style: {
                         top: e.top,
                         left: e.left,
                         width: e.width,
                         height: e.height
                     }
                 }) : null
             }
         }
-        class ab extends Zy {
+        class sb extends Qy {
             constructor() {
                 super("selection")
             }
             generateModel(e) {
-                return new ob
+                return new ib
             }
             generateReactWidget(e) {
-                return t.createElement(ib, {
+                return t.createElement(ab, {
                     rect: e.model.box
                 })
             }
         }
-        class sb extends t.Component {
+        class lb extends t.Component {
             shouldComponentUpdate(e, t, n) {
-                return !this.props.model.performanceTune() || this.props.model !== e.model || !ky.isEqual(this.props.serialized, e.serialized)
+                return !this.props.model.performanceTune() || this.props.model !== e.model || !Sy.isEqual(this.props.serialized, e.serialized)
             }
             render() {
                 return this.props.children()
             }
         }
-        class lb {
+        class ub {
             constructor(e) {
                 this.actions = [], this.keys = [], this.childStates = [], this.options = e
             }
             setEngine(e) {
                 this.engine = e
             }
             getOptions() {
@@ -30145,87 +30168,87 @@
             }
             findStateToActivate(e) {
                 for (let t of this.childStates)
                     if (t.isKeysFullfilled(e)) return t;
                 return null
             }
             isKeysFullfilled(e) {
-                return ky.intersection(this.keys, e).length === this.keys.length
+                return Sy.intersection(this.keys, e).length === this.keys.length
             }
             activated(e) {
                 const t = this.engine.getActionEventBus().getKeys();
                 if (!this.tryActivateParentState(t) && !this.tryActivateChildState(t)) {
-                    this.handler1 = this.engine.getActionEventBus().registerAction(new zy({
-                        type: Iy.KEY_DOWN,
+                    this.handler1 = this.engine.getActionEventBus().registerAction(new Wy({
+                        type: Ny.KEY_DOWN,
                         fire: () => {
                             this.tryActivateChildState(this.engine.getActionEventBus().getKeys())
                         }
-                    })), this.handler2 = this.engine.getActionEventBus().registerAction(new zy({
-                        type: Iy.KEY_UP,
+                    })), this.handler2 = this.engine.getActionEventBus().registerAction(new Wy({
+                        type: Ny.KEY_UP,
                         fire: () => {
                             this.tryActivateParentState(this.engine.getActionEventBus().getKeys())
                         }
                     }));
                     for (let e of this.actions) this.engine.getActionEventBus().registerAction(e)
                 }
             }
             deactivated(e) {
                 this.handler1 && this.handler1(), this.handler2 && this.handler2();
                 for (let e of this.actions) this.engine.getActionEventBus().deregisterAction(e)
             }
         }
-        class ub extends lb {
+        class cb extends ub {
             constructor(e) {
-                super(e), this.registerAction(new zy({
-                    type: Iy.MOUSE_DOWN,
+                super(e), this.registerAction(new Wy({
+                    type: Ny.MOUSE_DOWN,
                     fire: e => {
                         const {
                             clientX: t,
                             clientY: n
                         } = e.event;
                         this.handleMoveStart(t, n)
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.MOUSE_MOVE,
+                })), this.registerAction(new Wy({
+                    type: Ny.MOUSE_MOVE,
                     fire: e => {
                         const {
                             event: t
                         } = e;
                         if (0 === t.buttons) return void this.eject();
                         const {
                             clientX: n,
                             clientY: r
                         } = t;
                         this.handleMove(n, r, t)
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.MOUSE_UP,
+                })), this.registerAction(new Wy({
+                    type: Ny.MOUSE_UP,
                     fire: () => this.handleMoveEnd()
-                })), this.registerAction(new zy({
-                    type: Iy.TOUCH_START,
+                })), this.registerAction(new Wy({
+                    type: Ny.TOUCH_START,
                     fire: e => {
                         const {
                             clientX: t,
                             clientY: n
                         } = e.event.touches[0];
                         this.handleMoveStart(t, n)
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.TOUCH_MOVE,
+                })), this.registerAction(new Wy({
+                    type: Ny.TOUCH_MOVE,
                     fire: e => {
                         const {
                             event: t
                         } = e, {
                             clientX: n,
                             clientY: r
                         } = t.touches[0];
                         this.handleMove(n, r, t)
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.TOUCH_END,
+                })), this.registerAction(new Wy({
+                    type: Ny.TOUCH_END,
                     fire: () => this.handleMoveEnd()
                 }))
             }
             handleMoveStart(e, t) {
                 this.initialX = e, this.initialY = t;
                 const n = this.engine.getRelativePoint(e, t);
                 this.initialXRelative = n.x, this.initialYRelative = n.y
@@ -30239,15 +30262,15 @@
                     event: n
                 })
             }
             handleMoveEnd() {
                 this.eject()
             }
         }
-        class cb extends ub {
+        class db extends cb {
             constructor(e = {}) {
                 super({
                     name: "drag-canvas"
                 }), this.config = Object.assign({
                     allowDrag: !0
                 }, e)
             }
@@ -30292,22 +30315,22 @@
                 super.deactivated(e);
                 for (let e of this.engine.getModel().getLayers()) e.allowRepaint(!0)
             }
             fireMouseMoved(e) {
                 this.config.allowDrag && (this.engine.getModel().setOffset(this.initialCanvasX + e.displacementX, this.initialCanvasY + e.displacementY), this.engine.repaintCanvas())
             }
         }
-        class db extends ub {
+        class pb extends cb {
             constructor() {
                 super({
                     name: "selection-box"
                 })
             }
             activated(e) {
-                super.activated(e), this.layer = new ob, this.engine.getModel().addLayer(this.layer)
+                super.activated(e), this.layer = new ib, this.engine.getModel().addLayer(this.layer)
             }
             deactivated(e) {
                 super.deactivated(e), this.layer.remove(), this.engine.repaintCanvas()
             }
             getBoxDimensions(e) {
                 let t;
                 if ("touches" in e.event) {
@@ -30326,73 +30349,73 @@
             fireMouseMoved(e) {
                 this.layer.setBox(this.getBoxDimensions(e));
                 const t = this.engine.getRelativeMousePoint({
                     clientX: this.initialX,
                     clientY: this.initialY
                 });
                 e.virtualDisplacementX < 0 && (t.x -= Math.abs(e.virtualDisplacementX)), e.virtualDisplacementY < 0 && (t.y -= Math.abs(e.virtualDisplacementY));
-                const n = Ay.fromPointAndSize(t, Math.abs(e.virtualDisplacementX), Math.abs(e.virtualDisplacementY));
+                const n = Ry.fromPointAndSize(t, Math.abs(e.virtualDisplacementX), Math.abs(e.virtualDisplacementY));
                 for (let e of this.engine.getModel().getSelectionEntities())
                     if (e.getBoundingBox) {
                         const t = e.getBoundingBox();
                         n.containsPoint(t.getTopLeft()) && n.containsPoint(t.getBottomRight()) ? e.setSelected(!0) : e.setSelected(!1)
                     } this.engine.repaintCanvas()
             }
         }
-        class pb extends lb {
+        class fb extends ub {
             constructor() {
                 super({
                     name: "selecting"
-                }), this.keys = ["shift"], this.registerAction(new zy({
-                    type: Iy.MOUSE_DOWN,
+                }), this.keys = ["shift"], this.registerAction(new Wy({
+                    type: Ny.MOUSE_DOWN,
                     fire: e => {
                         const t = this.engine.getActionEventBus().getModelForEvent(e);
-                        t ? (t.setSelected(!0), this.engine.repaintCanvas()) : this.transitionWithEvent(new db, e)
+                        t ? (t.setSelected(!0), this.engine.repaintCanvas()) : this.transitionWithEvent(new pb, e)
                     }
                 }))
             }
         }
-        class fb extends ub {
+        class hb extends cb {
             constructor() {
                 super({
                     name: "move-items"
-                }), this.registerAction(new zy({
-                    type: Iy.MOUSE_DOWN,
+                }), this.registerAction(new Wy({
+                    type: Ny.MOUSE_DOWN,
                     fire: e => {
                         const t = this.engine.getActionEventBus().getModelForEvent(e);
                         t && (t.isSelected() || this.engine.getModel().clearSelection(), t.setSelected(!0), this.engine.repaintCanvas())
                     }
                 }))
             }
             activated(e) {
                 super.activated(e), this.initialPositions = {}
             }
             fireMouseMoved(e) {
                 const t = this.engine.getModel().getSelectedEntities(),
                     n = this.engine.getModel();
                 for (let r of t)
-                    if (r instanceof Jy) {
+                    if (r instanceof eb) {
                         if (r.isLocked()) continue;
                         this.initialPositions[r.getID()] || (this.initialPositions[r.getID()] = {
                             point: r.getPosition(),
                             item: r
                         });
                         const t = this.initialPositions[r.getID()].point;
                         r.setPosition(n.getGridPosition(t.x + e.virtualDisplacementX), n.getGridPosition(t.y + e.virtualDisplacementY))
                     } this.engine.repaintCanvas()
             }
         }
 
-        function hb(e) {
+        function gb(e) {
             return Ot("MuiAppBar", e)
         }
         _t("MuiAppBar", ["root", "positionFixed", "positionAbsolute", "positionSticky", "positionStatic", "positionRelative", "colorDefault", "colorPrimary", "colorSecondary", "colorInherit", "colorTransparent"]);
-        const gb = ["className", "color", "enableColorOnDark", "position"],
-            vb = (e, t) => e ? `${null==e?void 0:e.replace(")","")}, ${t})` : t,
-            mb = vt(ii, {
+        const vb = ["className", "color", "enableColorOnDark", "position"],
+            mb = (e, t) => e ? `${null==e?void 0:e.replace(")","")}, ${t})` : t,
+            yb = vt(ii, {
                 name: "MuiAppBar",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.root, t[`position${kt(n.position)}`], t[`color${kt(n.color)}`]]
@@ -30446,71 +30469,71 @@
                     color: null
                 }, "transparent" === t.color && s({
                     backgroundColor: "transparent",
                     color: "inherit"
                 }, "dark" === e.palette.mode && {
                     backgroundImage: "none"
                 })), e.vars && s({}, "default" === t.color && {
-                    "--AppBar-background": t.enableColorOnDark ? e.vars.palette.AppBar.defaultBg : vb(e.vars.palette.AppBar.darkBg, e.vars.palette.AppBar.defaultBg),
-                    "--AppBar-color": t.enableColorOnDark ? e.vars.palette.text.primary : vb(e.vars.palette.AppBar.darkColor, e.vars.palette.text.primary)
+                    "--AppBar-background": t.enableColorOnDark ? e.vars.palette.AppBar.defaultBg : mb(e.vars.palette.AppBar.darkBg, e.vars.palette.AppBar.defaultBg),
+                    "--AppBar-color": t.enableColorOnDark ? e.vars.palette.text.primary : mb(e.vars.palette.AppBar.darkColor, e.vars.palette.text.primary)
                 }, t.color && !t.color.match(/^(default|inherit|transparent)$/) && {
-                    "--AppBar-background": t.enableColorOnDark ? e.vars.palette[t.color].main : vb(e.vars.palette.AppBar.darkBg, e.vars.palette[t.color].main),
-                    "--AppBar-color": t.enableColorOnDark ? e.vars.palette[t.color].contrastText : vb(e.vars.palette.AppBar.darkColor, e.vars.palette[t.color].contrastText)
+                    "--AppBar-background": t.enableColorOnDark ? e.vars.palette[t.color].main : mb(e.vars.palette.AppBar.darkBg, e.vars.palette[t.color].main),
+                    "--AppBar-color": t.enableColorOnDark ? e.vars.palette[t.color].contrastText : mb(e.vars.palette.AppBar.darkColor, e.vars.palette[t.color].contrastText)
                 }, {
                     backgroundColor: "var(--AppBar-background)",
                     color: "inherit" === t.color ? "inherit" : "var(--AppBar-color)"
                 }, "transparent" === t.color && {
                     backgroundImage: "none",
                     backgroundColor: "transparent",
                     color: "inherit"
                 }))
             })),
-            yb = t.forwardRef((function(t, n) {
+            bb = t.forwardRef((function(t, n) {
                 const r = wt({
                         props: t,
                         name: "MuiAppBar"
                     }),
                     {
                         className: i,
                         color: a = "primary",
                         enableColorOnDark: l = !1,
                         position: c = "fixed"
                     } = r,
-                    p = o(r, gb),
+                    p = o(r, vb),
                     f = s({}, r, {
                         color: a,
                         position: c,
                         enableColorOnDark: l
                     }),
                     h = (e => {
                         const {
                             color: t,
                             position: n,
                             classes: r
                         } = e;
                         return d({
                             root: ["root", `color${kt(t)}`, `position${kt(n)}`]
-                        }, hb, r)
+                        }, gb, r)
                     })(f);
-                return (0, e.jsx)(mb, s({
+                return (0, e.jsx)(yb, s({
                     square: !0,
                     component: "header",
                     ownerState: f,
                     elevation: 4,
                     className: u(h.root, i, "fixed" === c && "mui-fixed"),
                     ref: n
                 }, p))
             }));
 
-        function bb(e) {
+        function xb(e) {
             return Ot("MuiToolbar", e)
         }
         _t("MuiToolbar", ["root", "gutters", "regular", "dense"]);
-        const xb = ["className", "component", "disableGutters", "variant"],
-            wb = vt("div", {
+        const wb = ["className", "component", "disableGutters", "variant"],
+            kb = vt("div", {
                 name: "MuiToolbar",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.root, !n.disableGutters && t.gutters, t[n.variant]]
@@ -30531,49 +30554,49 @@
                 }
             }, "dense" === t.variant && {
                 minHeight: 48
             })), (({
                 theme: e,
                 ownerState: t
             }) => "regular" === t.variant && e.mixins.toolbar)),
-            kb = t.forwardRef((function(t, n) {
+            Sb = t.forwardRef((function(t, n) {
                 const r = wt({
                         props: t,
                         name: "MuiToolbar"
                     }),
                     {
                         className: i,
                         component: a = "div",
                         disableGutters: l = !1,
                         variant: c = "regular"
                     } = r,
-                    p = o(r, xb),
+                    p = o(r, wb),
                     f = s({}, r, {
                         component: a,
                         disableGutters: l,
                         variant: c
                     }),
                     h = (e => {
                         const {
                             classes: t,
                             disableGutters: n,
                             variant: r
                         } = e;
                         return d({
                             root: ["root", !n && "gutters", r]
-                        }, bb, t)
+                        }, xb, t)
                     })(f);
-                return (0, e.jsx)(wb, s({
+                return (0, e.jsx)(kb, s({
                     as: a,
                     className: u(h.root, i),
                     ref: n,
                     ownerState: f
                 }, p))
             }));
-        class Sb extends Jy {
+        class Eb extends eb {
             constructor(e) {
                 super(Object.assign(Object.assign({}, e), {
                     type: "point"
                 })), this.parent = e.link
             }
             isConnectedToPort() {
                 return null !== this.parent.getPortForPoint(this)
@@ -30584,38 +30607,38 @@
             remove() {
                 this.parent && this.parent.removePoint(this), super.remove()
             }
             isLocked() {
                 return super.isLocked() || this.getParent().isLocked()
             }
         }
-        class Eb extends Qy {
+        class Cb extends Jy {
             constructor(e) {
-                super(e), this.points = [new Sb({
+                super(e), this.points = [new Eb({
                     link: this
-                }), new Sb({
+                }), new Eb({
                     link: this
                 })], this.sourcePort = null, this.targetPort = null, this.renderedPaths = [], this.labels = []
             }
             getBoundingBox() {
-                return new Ay(My(ky.map(this.points, (e => e.getPosition()))))
+                return new Ry(jy(Sy.map(this.points, (e => e.getPosition()))))
             }
             getSelectionEntities() {
-                return this.getTargetPort() && this.getSourcePort() ? super.getSelectionEntities().concat(ky.slice(this.points, 1, this.points.length - 1)) : this.getSourcePort() ? this.getTargetPort() ? super.getSelectionEntities().concat(this.points) : super.getSelectionEntities().concat(ky.slice(this.points, 1, this.points.length)) : super.getSelectionEntities().concat(ky.slice(this.points, 0, this.points.length - 1))
+                return this.getTargetPort() && this.getSourcePort() ? super.getSelectionEntities().concat(Sy.slice(this.points, 1, this.points.length - 1)) : this.getSourcePort() ? this.getTargetPort() ? super.getSelectionEntities().concat(this.points) : super.getSelectionEntities().concat(Sy.slice(this.points, 1, this.points.length)) : super.getSelectionEntities().concat(Sy.slice(this.points, 0, this.points.length - 1))
             }
             deserialize(e) {
-                super.deserialize(e), this.points = ky.map(e.data.points || [], (t => {
-                    var n = new Sb({
+                super.deserialize(e), this.points = Sy.map(e.data.points || [], (t => {
+                    var n = new Eb({
                         link: this,
-                        position: new _y(t.x, t.y)
+                        position: new Ty(t.x, t.y)
                     });
                     return n.deserialize(Object.assign(Object.assign({}, e), {
                         data: t
                     })), n
-                })), ky.forEach(e.data.labels || [], (t => {
+                })), Sy.forEach(e.data.labels || [], (t => {
                     let n = e.engine.getFactoryForLabel(t.type).generateModel({});
                     n.deserialize(Object.assign(Object.assign({}, e), {
                         data: t
                     })), this.addLabel(n)
                 })), e.data.target && e.getModel(e.data.targetPort).then((e => {
                     this.setTargetPort(e)
                 })), e.data.source && e.getModel(e.data.sourcePort).then((e => {
@@ -30630,20 +30653,20 @@
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     source: this.sourcePort ? this.sourcePort.getParent().getID() : null,
                     sourcePort: this.sourcePort ? this.sourcePort.getID() : null,
                     target: this.targetPort ? this.targetPort.getParent().getID() : null,
                     targetPort: this.targetPort ? this.targetPort.getID() : null,
-                    points: ky.map(this.points, (e => e.serialize())),
-                    labels: ky.map(this.labels, (e => e.serialize()))
+                    points: Sy.map(this.points, (e => e.serialize())),
+                    labels: Sy.map(this.labels, (e => e.serialize()))
                 })
             }
             doClone(e = {}, t) {
-                t.setPoints(ky.map(this.getPoints(), (t => t.clone(e)))), this.sourcePort && t.setSourcePort(this.sourcePort.clone(e)), this.targetPort && t.setTargetPort(this.targetPort.clone(e))
+                t.setPoints(Sy.map(this.getPoints(), (t => t.clone(e)))), this.sourcePort && t.setSourcePort(this.sourcePort.clone(e)), this.targetPort && t.setTargetPort(this.targetPort.clone(e))
             }
             clearPort(e) {
                 this.sourcePort === e ? this.setSourcePort(null) : this.targetPort === e && this.setTargetPort(null)
             }
             remove() {
                 this.sourcePort && (this.sourcePort.removeLink(this), delete this.sourcePort), this.targetPort && (this.targetPort.removeLink(this), delete this.targetPort), super.remove()
             }
@@ -30695,15 +30718,15 @@
             getPoints() {
                 return this.points
             }
             getLabels() {
                 return this.labels
             }
             setPoints(e) {
-                ky.forEach(e, (e => {
+                Sy.forEach(e, (e => {
                     e.setParent(this)
                 })), this.points = e
             }
             removePoint(e) {
                 this.isLastPoint(e) && this.remove(), this.points.splice(this.getPointIndex(e), 1)
             }
             removePointsBefore(e) {
@@ -30715,54 +30738,54 @@
             removeMiddlePoints() {
                 this.points.length > 2 && this.points.splice(1, this.points.length - 2)
             }
             addPoint(e, t = 1) {
                 return e.setParent(this), this.points.splice(t, 0, e), e
             }
             generatePoint(e = 0, t = 0) {
-                return new Sb({
+                return new Eb({
                     link: this,
-                    position: new _y(e, t)
+                    position: new Ty(e, t)
                 })
             }
         }
-        class Cb extends Jy {
+        class Ob extends eb {
             constructor(e) {
                 super(e), this.ports = {}, this.width = 0, this.height = 0
             }
             getBoundingBox() {
-                return Ay.fromPointAndSize(this.getPosition(), this.width, this.height)
+                return Ry.fromPointAndSize(this.getPosition(), this.width, this.height)
             }
             setPosition(e, t) {
                 const n = this.position;
-                e instanceof _y ? super.setPosition(e) : super.setPosition(e, t), ky.forEach(this.ports, (e => {
+                e instanceof Ty ? super.setPosition(e) : super.setPosition(e, t), Sy.forEach(this.ports, (e => {
                     e.setPosition(e.getX() + this.position.x - n.x, e.getY() + this.position.y - n.y)
                 }))
             }
             deserialize(e) {
-                super.deserialize(e), ky.forEach(e.data.ports, (t => {
+                super.deserialize(e), Sy.forEach(e.data.ports, (t => {
                     let n = e.engine.getFactoryForPort(t.type).generateModel({});
                     n.deserialize(Object.assign(Object.assign({}, e), {
                         data: t
                     })), e.registerModel(n), this.addPort(n)
                 }))
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
-                    ports: ky.map(this.ports, (e => e.serialize()))
+                    ports: Sy.map(this.ports, (e => e.serialize()))
                 })
             }
             doClone(e = {}, t) {
-                t.ports = {}, ky.forEach(this.ports, (n => {
+                t.ports = {}, Sy.forEach(this.ports, (n => {
                     t.addPort(n.clone(e))
                 }))
             }
             remove() {
-                super.remove(), ky.forEach(this.ports, (e => {
-                    ky.forEach(e.getLinks(), (e => {
+                super.remove(), Sy.forEach(this.ports, (e => {
+                    Sy.forEach(e.getLinks(), (e => {
                         e.remove()
                     }))
                 }))
             }
             getPortFromID(e) {
                 for (var t in this.ports)
                     if (this.ports[t].getID() === e) return this.ports[t];
@@ -30777,100 +30800,100 @@
             getPort(e) {
                 return this.ports[e]
             }
             getPorts() {
                 return this.ports
             }
             removePort(e) {
-                for (let t of ky.values(e.getLinks())) t.clearPort(e);
+                for (let t of Sy.values(e.getLinks())) t.clearPort(e);
                 this.ports[e.getName()] && (this.ports[e.getName()].setParent(null), delete this.ports[e.getName()])
             }
             addPort(e) {
                 return e.setParent(this), this.ports[e.getName()] = e, e
             }
             updateDimensions({
                 width: e,
                 height: t
             }) {
                 this.width = e, this.height = t
             }
         }
-        class Ob extends rb {
+        class _b extends ob {
             constructor() {
                 super({
                     type: "diagram-nodes",
                     isSvg: !1,
                     transformed: !0
                 })
             }
             addModel(e) {
-                if (!(e instanceof Cb)) throw new Error("Can only add nodes to this layer");
+                if (!(e instanceof Ob)) throw new Error("Can only add nodes to this layer");
                 e.registerListener({
                     entityRemoved: () => {
                         this.getParent().removeNode(e)
                     }
                 }), super.addModel(e)
             }
             getChildModelFactoryBank(e) {
                 return e.getNodeFactories()
             }
             getNodes() {
                 return this.getModels()
             }
         }
-        class _b extends rb {
+        class Tb extends ob {
             constructor() {
                 super({
                     type: "diagram-links",
                     isSvg: !0,
                     transformed: !0
                 })
             }
             addModel(e) {
-                if (!(e instanceof Eb)) throw new Error("Can only add links to this layer");
+                if (!(e instanceof Cb)) throw new Error("Can only add links to this layer");
                 e.registerListener({
                     entityRemoved: () => {
                         this.getParent().removeLink(e)
                     }
                 }), super.addModel(e)
             }
             getLinks() {
                 return this.getModels()
             }
             getChildModelFactoryBank(e) {
                 return e.getLinkFactories()
             }
         }
-        class Tb extends qy {
+        class Pb extends Xy {
             constructor(e = {}) {
-                super(e), this.addLayer(new _b), this.addLayer(new Ob)
+                super(e), this.addLayer(new Tb), this.addLayer(new _b)
             }
             deserialize(e) {
                 this.layers = [], super.deserialize(e)
             }
             addLayer(e) {
-                super.addLayer(e), e instanceof Ob && (this.activeNodeLayer = e), e instanceof _b && (this.activeLinkLayer = e)
+                super.addLayer(e), e instanceof _b && (this.activeNodeLayer = e), e instanceof Tb && (this.activeLinkLayer = e)
             }
             getLinkLayers() {
-                return ky.filter(this.layers, (e => e instanceof _b))
+                return Sy.filter(this.layers, (e => e instanceof Tb))
             }
             getNodeLayers() {
-                return ky.filter(this.layers, (e => e instanceof Ob))
+                return Sy.filter(this.layers, (e => e instanceof _b))
             }
             getActiveNodeLayer() {
                 if (!this.activeNodeLayer) {
                     const e = this.getNodeLayers();
-                    0 === e.length ? this.addLayer(new Ob) : this.activeNodeLayer = e[0]
+                    0 === e.length ? this.addLayer(new _b) : this.activeNodeLayer = e[0]
                 }
                 return this.activeNodeLayer
             }
             getActiveLinkLayer() {
                 if (!this.activeLinkLayer) {
                     const e = this.getLinkLayers();
-                    0 === e.length ? this.addLayer(new _b) : this.activeLinkLayer = e[0]
+                    0 === e.length ? this.addLayer(new Tb) : this.activeLinkLayer = e[0]
                 }
                 return this.activeLinkLayer
             }
             getNode(e) {
                 for (const t of this.getNodeLayers()) {
                     const n = t.getModel(e);
                     if (n) return n
@@ -30879,16 +30902,16 @@
             getLink(e) {
                 for (const t of this.getLinkLayers()) {
                     const n = t.getModel(e);
                     if (n) return n
                 }
             }
             addAll(...e) {
-                return ky.forEach(e, (e => {
-                    e instanceof Eb ? this.addLink(e) : e instanceof Cb && this.addNode(e)
+                return Sy.forEach(e, (e => {
+                    e instanceof Cb ? this.addLink(e) : e instanceof Ob && this.addNode(e)
                 })), e
             }
             addLink(e) {
                 return this.getActiveLinkLayer().addModel(e), this.fireEvent({
                     link: e,
                     isCreated: !0
                 }, "linksUpdated"), e
@@ -30896,33 +30919,33 @@
             addNode(e) {
                 return this.getActiveNodeLayer().addModel(e), this.fireEvent({
                     node: e,
                     isCreated: !0
                 }, "nodesUpdated"), e
             }
             removeLink(e) {
-                ky.some(this.getLinkLayers(), (t => t.removeModel(e))) && this.fireEvent({
+                Sy.some(this.getLinkLayers(), (t => t.removeModel(e))) && this.fireEvent({
                     link: e,
                     isCreated: !1
                 }, "linksUpdated")
             }
             removeNode(e) {
-                ky.some(this.getNodeLayers(), (t => t.removeModel(e))) && this.fireEvent({
+                Sy.some(this.getNodeLayers(), (t => t.removeModel(e))) && this.fireEvent({
                     node: e,
                     isCreated: !1
                 }, "nodesUpdated")
             }
             getLinks() {
-                return ky.flatMap(this.getLinkLayers(), (e => ky.values(e.getModels())))
+                return Sy.flatMap(this.getLinkLayers(), (e => Sy.values(e.getModels())))
             }
             getNodes() {
-                return ky.flatMap(this.getNodeLayers(), (e => ky.values(e.getModels())))
+                return Sy.flatMap(this.getNodeLayers(), (e => Sy.values(e.getModels())))
             }
         }
-        class Pb extends Qy {
+        class Mb extends Jy {
             constructor(e) {
                 super(Object.assign(Object.assign({}, e), {
                     offsetX: e.offsetX || 0,
                     offsetY: e.offsetY || 0
                 }))
             }
             deserialize(e) {
@@ -30931,25 +30954,25 @@
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     offsetX: this.options.offsetX,
                     offsetY: this.options.offsetY
                 })
             }
         }
-        var Mb, jb;
+        var jb, Ab;
         ! function(e) {
             e.Label = b.default.div`
 		display: inline-block;
 		position: absolute;
 	`, e.Foreign = b.default.foreignObject`
 		pointer-events: none;
 		overflow: visible;
 	`
-        }(Mb || (Mb = {}));
-        class Ab extends t.Component {
+        }(jb || (jb = {}));
+        class Rb extends t.Component {
             constructor(e) {
                 super(e), this.findPathAndRelativePositionToRenderLabel = e => {
                     const t = this.props.label.getParent(),
                         n = t.getRenderedPath().map((e => e.getTotalLength()));
                     let r = n.reduce(((e, t) => e + t), 0) * (e / (t.getLabels().length + 1)),
                         o = 0;
                     for (; o < t.getRenderedPath().length;) {
@@ -30973,26 +30996,26 @@
                 window.requestAnimationFrame(this.calculateLabelPosition)
             }
             componentDidMount() {
                 window.requestAnimationFrame(this.calculateLabelPosition)
             }
             render() {
                 const e = this.props.engine.getCanvas();
-                return t.createElement(Mb.Foreign, {
+                return t.createElement(jb.Foreign, {
                     key: this.props.label.getID(),
                     width: null == e ? void 0 : e.offsetWidth,
                     height: null == e ? void 0 : e.offsetHeight
-                }, t.createElement(Mb.Label, {
+                }, t.createElement(jb.Label, {
                     ref: this.ref
                 }, this.props.engine.getFactoryForLabel(this.props.label).generateReactWidget({
                     model: this.props.label
                 })))
             }
         }
-        class Rb extends t.Component {
+        class Ib extends t.Component {
             constructor(e) {
                 super(e), this.state = {
                     sourcePort: null,
                     targetPort: null
                 }
             }
             componentWillUnmount() {
@@ -31027,53 +31050,53 @@
             componentDidMount() {
                 this.props.link.getSourcePort() && this.installSource(), this.props.link.getTargetPort() && this.installTarget()
             }
             render() {
                 const {
                     link: e
                 } = this.props;
-                return e.getSourcePort() && !e.getSourcePort().reportedPosition || e.getTargetPort() && !e.getTargetPort().reportedPosition ? null : t.createElement(sb, {
+                return e.getSourcePort() && !e.getSourcePort().reportedPosition || e.getTargetPort() && !e.getTargetPort().reportedPosition ? null : t.createElement(lb, {
                     model: this.props.link,
                     serialized: this.props.link.serialize()
                 }, (() => t.createElement("g", {
                     "data-linkid": this.props.link.getID()
-                }, this.props.diagramEngine.generateWidgetForLink(e), ky.map(this.props.link.getLabels(), ((e, n) => t.createElement(Ab, {
+                }, this.props.diagramEngine.generateWidgetForLink(e), Sy.map(this.props.link.getLabels(), ((e, n) => t.createElement(Rb, {
                     key: e.getID(),
                     engine: this.props.diagramEngine,
                     label: e,
                     index: n
                 }))))))
             }
         }! function(e) {
             e.Container = b.default.div``
-        }(jb || (jb = {}));
-        class Ib extends t.Component {
+        }(Ab || (Ab = {}));
+        class Nb extends t.Component {
             render() {
-                return t.createElement(t.Fragment, null, ky.map(this.props.layer.getLinks(), (e => t.createElement(Rb, {
+                return t.createElement(t.Fragment, null, Sy.map(this.props.layer.getLinks(), (e => t.createElement(Ib, {
                     key: e.getID(),
                     link: e,
                     diagramEngine: this.props.engine
                 }))))
             }
         }
-        class Nb extends Zy {
+        class Lb extends Qy {
             constructor() {
                 super("diagram-links")
             }
             generateModel(e) {
-                return new _b
+                return new Tb
             }
             generateReactWidget(e) {
-                return t.createElement(Ib, {
+                return t.createElement(Nb, {
                     layer: e.model,
                     engine: this.engine
                 })
             }
         }
-        var Lb = function() {
+        var Db = function() {
                 if ("undefined" != typeof Map) return Map;
 
                 function e(e, t) {
                     var n = -1;
                     return e.some((function(e, r) {
                         return e[0] === t && (n = r, !0)
                     })), n
@@ -31108,36 +31131,36 @@
                         for (var n = 0, r = this.__entries__; n < r.length; n++) {
                             var o = r[n];
                             e.call(t, o[1], o[0])
                         }
                     }, t
                 }()
             }(),
-            Db = "undefined" != typeof window && "undefined" != typeof document && window.document === document,
-            Fb = void 0 !== i.g && i.g.Math === Math ? i.g : "undefined" != typeof self && self.Math === Math ? self : "undefined" != typeof window && window.Math === Math ? window : Function("return this")(),
-            $b = "function" == typeof requestAnimationFrame ? requestAnimationFrame.bind(Fb) : function(e) {
+            Fb = "undefined" != typeof window && "undefined" != typeof document && window.document === document,
+            $b = void 0 !== i.g && i.g.Math === Math ? i.g : "undefined" != typeof self && self.Math === Math ? self : "undefined" != typeof window && window.Math === Math ? window : Function("return this")(),
+            zb = "function" == typeof requestAnimationFrame ? requestAnimationFrame.bind($b) : function(e) {
                 return setTimeout((function() {
                     return e(Date.now())
                 }), 1e3 / 60)
             },
-            zb = ["top", "right", "bottom", "left", "width", "height", "size", "weight"],
-            Wb = "undefined" != typeof MutationObserver,
-            Bb = function() {
+            Wb = ["top", "right", "bottom", "left", "width", "height", "size", "weight"],
+            Bb = "undefined" != typeof MutationObserver,
+            Ub = function() {
                 function e() {
                     this.connected_ = !1, this.mutationEventsAdded_ = !1, this.mutationsObserver_ = null, this.observers_ = [], this.onTransitionEnd_ = this.onTransitionEnd_.bind(this), this.refresh = function(e, t) {
                         var n = !1,
                             r = !1,
                             o = 0;
 
                         function i() {
                             n && (n = !1, e()), r && s()
                         }
 
                         function a() {
-                            $b(i)
+                            zb(i)
                         }
 
                         function s() {
                             var e = Date.now();
                             if (n) {
                                 if (e - o < 2) return;
                                 r = !0
@@ -31159,208 +31182,208 @@
                     var e = this.observers_.filter((function(e) {
                         return e.gatherActive(), e.hasActive()
                     }));
                     return e.forEach((function(e) {
                         return e.broadcastActive()
                     })), e.length > 0
                 }, e.prototype.connect_ = function() {
-                    Db && !this.connected_ && (document.addEventListener("transitionend", this.onTransitionEnd_), window.addEventListener("resize", this.refresh), Wb ? (this.mutationsObserver_ = new MutationObserver(this.refresh), this.mutationsObserver_.observe(document, {
+                    Fb && !this.connected_ && (document.addEventListener("transitionend", this.onTransitionEnd_), window.addEventListener("resize", this.refresh), Bb ? (this.mutationsObserver_ = new MutationObserver(this.refresh), this.mutationsObserver_.observe(document, {
                         attributes: !0,
                         childList: !0,
                         characterData: !0,
                         subtree: !0
                     })) : (document.addEventListener("DOMSubtreeModified", this.refresh), this.mutationEventsAdded_ = !0), this.connected_ = !0)
                 }, e.prototype.disconnect_ = function() {
-                    Db && this.connected_ && (document.removeEventListener("transitionend", this.onTransitionEnd_), window.removeEventListener("resize", this.refresh), this.mutationsObserver_ && this.mutationsObserver_.disconnect(), this.mutationEventsAdded_ && document.removeEventListener("DOMSubtreeModified", this.refresh), this.mutationsObserver_ = null, this.mutationEventsAdded_ = !1, this.connected_ = !1)
+                    Fb && this.connected_ && (document.removeEventListener("transitionend", this.onTransitionEnd_), window.removeEventListener("resize", this.refresh), this.mutationsObserver_ && this.mutationsObserver_.disconnect(), this.mutationEventsAdded_ && document.removeEventListener("DOMSubtreeModified", this.refresh), this.mutationsObserver_ = null, this.mutationEventsAdded_ = !1, this.connected_ = !1)
                 }, e.prototype.onTransitionEnd_ = function(e) {
                     var t = e.propertyName,
                         n = void 0 === t ? "" : t;
-                    zb.some((function(e) {
+                    Wb.some((function(e) {
                         return !!~n.indexOf(e)
                     })) && this.refresh()
                 }, e.getInstance = function() {
                     return this.instance_ || (this.instance_ = new e), this.instance_
                 }, e.instance_ = null, e
             }(),
-            Ub = function(e, t) {
+            Yb = function(e, t) {
                 for (var n = 0, r = Object.keys(t); n < r.length; n++) {
                     var o = r[n];
                     Object.defineProperty(e, o, {
                         value: t[o],
                         enumerable: !1,
                         writable: !1,
                         configurable: !0
                     })
                 }
                 return e
             },
-            Yb = function(e) {
-                return e && e.ownerDocument && e.ownerDocument.defaultView || Fb
+            Hb = function(e) {
+                return e && e.ownerDocument && e.ownerDocument.defaultView || $b
             },
-            Hb = Kb(0, 0, 0, 0);
+            Vb = Zb(0, 0, 0, 0);
 
-        function Vb(e) {
+        function Gb(e) {
             return parseFloat(e) || 0
         }
 
-        function Gb(e) {
+        function qb(e) {
             for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
             return t.reduce((function(t, n) {
-                return t + Vb(e["border-" + n + "-width"])
+                return t + Gb(e["border-" + n + "-width"])
             }), 0)
         }
-        var qb = "undefined" != typeof SVGGraphicsElement ? function(e) {
-            return e instanceof Yb(e).SVGGraphicsElement
+        var Xb = "undefined" != typeof SVGGraphicsElement ? function(e) {
+            return e instanceof Hb(e).SVGGraphicsElement
         } : function(e) {
-            return e instanceof Yb(e).SVGElement && "function" == typeof e.getBBox
+            return e instanceof Hb(e).SVGElement && "function" == typeof e.getBBox
         };
 
-        function Xb(e) {
-            return Db ? qb(e) ? function(e) {
+        function Kb(e) {
+            return Fb ? Xb(e) ? function(e) {
                 var t = e.getBBox();
-                return Kb(0, 0, t.width, t.height)
+                return Zb(0, 0, t.width, t.height)
             }(e) : function(e) {
                 var t = e.clientWidth,
                     n = e.clientHeight;
-                if (!t && !n) return Hb;
-                var r = Yb(e).getComputedStyle(e),
+                if (!t && !n) return Vb;
+                var r = Hb(e).getComputedStyle(e),
                     o = function(e) {
                         for (var t = {}, n = 0, r = ["top", "right", "bottom", "left"]; n < r.length; n++) {
                             var o = r[n],
                                 i = e["padding-" + o];
-                            t[o] = Vb(i)
+                            t[o] = Gb(i)
                         }
                         return t
                     }(r),
                     i = o.left + o.right,
                     a = o.top + o.bottom,
-                    s = Vb(r.width),
-                    l = Vb(r.height);
-                if ("border-box" === r.boxSizing && (Math.round(s + i) !== t && (s -= Gb(r, "left", "right") + i), Math.round(l + a) !== n && (l -= Gb(r, "top", "bottom") + a)), ! function(e) {
-                        return e === Yb(e).document.documentElement
+                    s = Gb(r.width),
+                    l = Gb(r.height);
+                if ("border-box" === r.boxSizing && (Math.round(s + i) !== t && (s -= qb(r, "left", "right") + i), Math.round(l + a) !== n && (l -= qb(r, "top", "bottom") + a)), ! function(e) {
+                        return e === Hb(e).document.documentElement
                     }(e)) {
                     var u = Math.round(s + i) - t,
                         c = Math.round(l + a) - n;
                     1 !== Math.abs(u) && (s -= u), 1 !== Math.abs(c) && (l -= c)
                 }
-                return Kb(o.left, o.top, s, l)
-            }(e) : Hb
+                return Zb(o.left, o.top, s, l)
+            }(e) : Vb
         }
 
-        function Kb(e, t, n, r) {
+        function Zb(e, t, n, r) {
             return {
                 x: e,
                 y: t,
                 width: n,
                 height: r
             }
         }
-        var Zb = function() {
+        var Qb = function() {
                 function e(e) {
-                    this.broadcastWidth = 0, this.broadcastHeight = 0, this.contentRect_ = Kb(0, 0, 0, 0), this.target = e
+                    this.broadcastWidth = 0, this.broadcastHeight = 0, this.contentRect_ = Zb(0, 0, 0, 0), this.target = e
                 }
                 return e.prototype.isActive = function() {
-                    var e = Xb(this.target);
+                    var e = Kb(this.target);
                     return this.contentRect_ = e, e.width !== this.broadcastWidth || e.height !== this.broadcastHeight
                 }, e.prototype.broadcastRect = function() {
                     var e = this.contentRect_;
                     return this.broadcastWidth = e.width, this.broadcastHeight = e.height, e
                 }, e
             }(),
-            Qb = function(e, t) {
+            Jb = function(e, t) {
                 var n = function(e) {
                     var t = e.x,
                         n = e.y,
                         r = e.width,
                         o = e.height,
                         i = "undefined" != typeof DOMRectReadOnly ? DOMRectReadOnly : Object,
                         a = Object.create(i.prototype);
-                    return Ub(a, {
+                    return Yb(a, {
                         x: t,
                         y: n,
                         width: r,
                         height: o,
                         top: n,
                         right: t + r,
                         bottom: o + n,
                         left: t
                     }), a
                 }(t);
-                Ub(this, {
+                Yb(this, {
                     target: e,
                     contentRect: n
                 })
             },
-            Jb = function() {
+            ex = function() {
                 function e(e, t, n) {
-                    if (this.activeObservations_ = [], this.observations_ = new Lb, "function" != typeof e) throw new TypeError("The callback provided as parameter 1 is not a function.");
+                    if (this.activeObservations_ = [], this.observations_ = new Db, "function" != typeof e) throw new TypeError("The callback provided as parameter 1 is not a function.");
                     this.callback_ = e, this.controller_ = t, this.callbackCtx_ = n
                 }
                 return e.prototype.observe = function(e) {
                     if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
                     if ("undefined" != typeof Element && Element instanceof Object) {
-                        if (!(e instanceof Yb(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
+                        if (!(e instanceof Hb(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
                         var t = this.observations_;
-                        t.has(e) || (t.set(e, new Zb(e)), this.controller_.addObserver(this), this.controller_.refresh())
+                        t.has(e) || (t.set(e, new Qb(e)), this.controller_.addObserver(this), this.controller_.refresh())
                     }
                 }, e.prototype.unobserve = function(e) {
                     if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
                     if ("undefined" != typeof Element && Element instanceof Object) {
-                        if (!(e instanceof Yb(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
+                        if (!(e instanceof Hb(e).Element)) throw new TypeError('parameter 1 is not of type "Element".');
                         var t = this.observations_;
                         t.has(e) && (t.delete(e), t.size || this.controller_.removeObserver(this))
                     }
                 }, e.prototype.disconnect = function() {
                     this.clearActive(), this.observations_.clear(), this.controller_.removeObserver(this)
                 }, e.prototype.gatherActive = function() {
                     var e = this;
                     this.clearActive(), this.observations_.forEach((function(t) {
                         t.isActive() && e.activeObservations_.push(t)
                     }))
                 }, e.prototype.broadcastActive = function() {
                     if (this.hasActive()) {
                         var e = this.callbackCtx_,
                             t = this.activeObservations_.map((function(e) {
-                                return new Qb(e.target, e.broadcastRect())
+                                return new Jb(e.target, e.broadcastRect())
                             }));
                         this.callback_.call(e, t, e), this.clearActive()
                     }
                 }, e.prototype.clearActive = function() {
                     this.activeObservations_.splice(0)
                 }, e.prototype.hasActive = function() {
                     return this.activeObservations_.length > 0
                 }, e
             }(),
-            ex = "undefined" != typeof WeakMap ? new WeakMap : new Lb,
-            tx = function e(t) {
+            tx = "undefined" != typeof WeakMap ? new WeakMap : new Db,
+            nx = function e(t) {
                 if (!(this instanceof e)) throw new TypeError("Cannot call a class as a function.");
                 if (!arguments.length) throw new TypeError("1 argument required, but only 0 present.");
-                var n = Bb.getInstance(),
-                    r = new Jb(t, n, this);
-                ex.set(this, r)
+                var n = Ub.getInstance(),
+                    r = new ex(t, n, this);
+                tx.set(this, r)
             };
         ["observe", "unobserve", "disconnect"].forEach((function(e) {
-            tx.prototype[e] = function() {
+            nx.prototype[e] = function() {
                 var t;
-                return (t = ex.get(this))[e].apply(t, arguments)
+                return (t = tx.get(this))[e].apply(t, arguments)
             }
         }));
-        const nx = void 0 !== Fb.ResizeObserver ? Fb.ResizeObserver : tx;
-        var rx, ox, ix, ax, sx, lx, ux;
+        const rx = void 0 !== $b.ResizeObserver ? $b.ResizeObserver : nx;
+        var ox, ix, ax, sx, lx, ux, cx;
         ! function(e) {
             e.Node = b.default.div`
 		position: absolute;
 		-webkit-touch-callout: none; /* iOS Safari */
 		-webkit-user-select: none; /* Chrome/Safari/Opera */
 		user-select: none;
 		cursor: move;
 		pointer-events: all;
 	`
-        }(rx || (rx = {}));
-        class cx extends t.Component {
+        }(ox || (ox = {}));
+        class dx extends t.Component {
             constructor(e) {
                 super(e), this.ref = t.createRef()
             }
             componentWillUnmount() {
                 var e;
                 this.ob.disconnect(), this.ob = null, null === (e = this.listener) || void 0 === e || e.deregister(), this.listener = null
             }
@@ -31376,85 +31399,85 @@
             }
             updateSize(e, t) {
                 this.props.node.updateDimensions({
                     width: e,
                     height: t
                 });
                 try {
-                    ky.forEach(this.props.node.getPorts(), (e => {
+                    Sy.forEach(this.props.node.getPorts(), (e => {
                         e.updateCoords(this.props.diagramEngine.getPortCoords(e))
                     }))
                 } catch (e) {}
             }
             componentDidMount() {
-                this.ob = new nx((e => {
+                this.ob = new rx((e => {
                     const t = e[0].contentRect;
                     this.updateSize(t.width, t.height)
                 }));
                 const e = this.ref.current.getBoundingClientRect();
                 this.updateSize(e.width, e.height), this.ob.observe(this.ref.current), this.installSelectionListener()
             }
             render() {
-                return t.createElement(sb, {
+                return t.createElement(lb, {
                     model: this.props.node,
                     serialized: this.props.node.serialize()
-                }, (() => t.createElement(rx.Node, {
+                }, (() => t.createElement(ox.Node, {
                     className: "node",
                     ref: this.ref,
                     "data-nodeid": this.props.node.getID(),
                     style: {
                         top: this.props.node.getY(),
                         left: this.props.node.getX()
                     }
                 }, this.props.diagramEngine.generateWidgetForNode(this.props.node))))
             }
         }
-        class dx extends t.Component {
+        class px extends t.Component {
             render() {
-                return t.createElement(t.Fragment, null, ky.map(this.props.layer.getNodes(), (e => t.createElement(cx, {
+                return t.createElement(t.Fragment, null, Sy.map(this.props.layer.getNodes(), (e => t.createElement(dx, {
                     key: e.getID(),
                     diagramEngine: this.props.engine,
                     node: e
                 }))))
             }
         }
-        class px extends Zy {
+        class fx extends Qy {
             constructor() {
                 super("diagram-nodes")
             }
             generateModel(e) {
-                return new Ob
+                return new _b
             }
             generateReactWidget(e) {
-                return t.createElement(dx, {
+                return t.createElement(px, {
                     layer: e.model,
                     engine: this.engine
                 })
             }
         }! function(e) {
             e.TOP = "top", e.LEFT = "left", e.BOTTOM = "bottom", e.RIGHT = "right"
-        }(ox || (ox = {}));
-        class fx extends Jy {
+        }(ix || (ix = {}));
+        class hx extends eb {
             constructor(e) {
                 super(e), this.links = {}, this.reportedPosition = !1
             }
             deserialize(e) {
                 super.deserialize(e), this.reportedPosition = !1, this.options.name = e.data.name, this.options.alignment = e.data.alignment
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     name: this.options.name,
                     alignment: this.options.alignment,
                     parentNode: this.parent.getID(),
-                    links: ky.map(this.links, (e => e.getID()))
+                    links: Sy.map(this.links, (e => e.getID()))
                 })
             }
             setPosition(e, t) {
                 let n = this.position;
-                super.setPosition(e, t), ky.forEach(this.getLinks(), (r => {
+                super.setPosition(e, t), Sy.forEach(this.getLinks(), (r => {
                     let o = r.getPointForPort(this);
                     o.setPosition(o.getX() + e - n.x, o.getY() + t - n.y)
                 }))
             }
             doClone(e = {}, t) {
                 t.links = {}, t.parent = this.getParent().clone(e)
             }
@@ -31476,45 +31499,45 @@
             addLink(e) {
                 this.links[e.getID()] = e
             }
             getLinks() {
                 return this.links
             }
             createLinkModel() {
-                if (ky.isFinite(this.options.maximumLinks)) {
-                    var e = ky.size(this.links);
-                    if (1 === this.options.maximumLinks && e >= 1) return ky.values(this.links)[0];
+                if (Sy.isFinite(this.options.maximumLinks)) {
+                    var e = Sy.size(this.links);
+                    if (1 === this.options.maximumLinks && e >= 1) return Sy.values(this.links)[0];
                     if (e >= this.options.maximumLinks) return null
                 }
                 return null
             }
             reportPosition() {
-                ky.forEach(this.getLinks(), (e => {
+                Sy.forEach(this.getLinks(), (e => {
                     e.getPointForPort(this).setPosition(this.getCenter())
                 })), this.fireEvent({
                     entity: this
                 }, "reportInitialPosition")
             }
             getCenter() {
-                return new _y(this.getX() + this.width / 2, this.getY() + this.height / 2)
+                return new Ty(this.getX() + this.width / 2, this.getY() + this.height / 2)
             }
             getBoundingBox() {
-                return Ay.fromPointAndSize(this.position, this.width, this.height)
+                return Ry.fromPointAndSize(this.position, this.width, this.height)
             }
             updateCoords(e) {
                 this.width = e.getWidth(), this.height = e.getHeight(), this.setPosition(e.getTopLeft()), this.reportedPosition = !0, this.reportPosition()
             }
             canLinkToPort(e) {
                 return !0
             }
             isLocked() {
                 return super.isLocked() || this.getParent().isLocked()
             }
         }
-        class hx extends t.Component {
+        class gx extends t.Component {
             constructor(e) {
                 super(e), this.ref = t.createRef()
             }
             report() {
                 this.props.port.updateCoords(this.props.engine.getPortCoords(this.props.port, this.ref.current))
             }
             componentWillUnmount() {
@@ -31527,45 +31550,45 @@
                 this.engineListenerHandle = this.props.engine.registerListener({
                     canvasReady: () => {
                         this.report()
                     }
                 }), this.props.engine.getCanvas() && this.report()
             }
             getExtraProps() {
-                return Sy.TESTING ? {
-                    "data-links": ky.keys(this.props.port.getNode().getPort(this.props.port.getName()).links).join(",")
+                return Ey.TESTING ? {
+                    "data-links": Sy.keys(this.props.port.getNode().getPort(this.props.port.getName()).links).join(",")
                 } : {}
             }
             render() {
                 return t.createElement("div", Object.assign({
                     style: this.props.style,
                     ref: this.ref,
                     className: `port ${this.props.className||""}`,
                     "data-name": this.props.port.getName(),
                     "data-nodeid": this.props.port.getNode().getID()
                 }, this.getExtraProps()), this.props.children)
             }
         }
-        class gx extends ub {
+        class vx extends cb {
             constructor(e = {}) {
                 super({
                     name: "drag-new-link"
                 }), this.config = Object.assign({
                     allowLooseLinks: !0,
                     allowLinksFromLockedPorts: !1
-                }, e), this.registerAction(new zy({
-                    type: Iy.MOUSE_DOWN,
+                }, e), this.registerAction(new Wy({
+                    type: Ny.MOUSE_DOWN,
                     fire: e => {
                         this.port = this.engine.getMouseElement(e.event), this.config.allowLinksFromLockedPorts || !this.port.isLocked() ? (this.link = this.port.createLinkModel(), this.link ? (this.link.setSelected(!0), this.link.setSourcePort(this.port), this.engine.getModel().addLink(this.link), this.port.reportPosition()) : this.eject()) : this.eject()
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.MOUSE_UP,
+                })), this.registerAction(new Wy({
+                    type: Ny.MOUSE_UP,
                     fire: e => {
                         const t = this.engine.getMouseElement(e.event);
-                        if (t instanceof fx) return this.port.canLinkToPort(t) ? (this.link.setTargetPort(t), t.reportPosition(), void this.engine.repaintCanvas()) : (this.link.remove(), void this.engine.repaintCanvas());
+                        if (t instanceof hx) return this.port.canLinkToPort(t) ? (this.link.setTargetPort(t), t.reportPosition(), void this.engine.repaintCanvas()) : (this.link.remove(), void this.engine.repaintCanvas());
                         this.config.allowLooseLinks || (this.link.remove(), this.engine.repaintCanvas())
                     }
                 }))
             }
             fireMouseMoved(e) {
                 const t = this.port.getPosition(),
                     n = this.engine.getModel().getZoomLevel() / 100,
@@ -31574,52 +31597,52 @@
                     i = this.initialXRelative / n,
                     a = this.initialYRelative / n,
                     s = t.x - r + (i - t.x) + e.virtualDisplacementX,
                     l = t.y - o + (a - t.y) + e.virtualDisplacementY;
                 this.link.getLastPoint().setPosition(s, l), this.engine.repaintCanvas()
             }
         }
-        class vx extends fb {
+        class mx extends hb {
             constructor() {
-                super(), this.registerAction(new zy({
-                    type: Iy.MOUSE_UP,
+                super(), this.registerAction(new Wy({
+                    type: Ny.MOUSE_UP,
                     fire: e => {
                         const t = this.engine.getMouseElement(e.event);
-                        t instanceof fx && ky.forEach(this.initialPositions, (e => {
-                            if (e.item instanceof Sb) {
+                        t instanceof hx && Sy.forEach(this.initialPositions, (e => {
+                            if (e.item instanceof Eb) {
                                 const n = e.item.getParent();
                                 if (n.getLastPoint() !== e.item) return;
                                 n.getSourcePort().canLinkToPort(t) && (n.setTargetPort(t), t.reportPosition(), this.engine.repaintCanvas())
                             }
                         }))
                     }
                 }))
             }
         }
-        class mx extends lb {
+        class yx extends ub {
             constructor() {
                 super({
                     name: "default-diagrams"
-                }), this.childStates = [new pb], this.dragCanvas = new cb, this.dragNewLink = new gx, this.dragItems = new vx, this.registerAction(new zy({
-                    type: Iy.MOUSE_DOWN,
+                }), this.childStates = [new fb], this.dragCanvas = new db, this.dragNewLink = new vx, this.dragItems = new mx, this.registerAction(new Wy({
+                    type: Ny.MOUSE_DOWN,
                     fire: e => {
                         const t = this.engine.getActionEventBus().getModelForEvent(e);
-                        t ? t instanceof fx ? this.transitionWithEvent(this.dragNewLink, e) : this.transitionWithEvent(this.dragItems, e) : this.transitionWithEvent(this.dragCanvas, e)
+                        t ? t instanceof hx ? this.transitionWithEvent(this.dragNewLink, e) : this.transitionWithEvent(this.dragItems, e) : this.transitionWithEvent(this.dragCanvas, e)
                     }
-                })), this.registerAction(new zy({
-                    type: Iy.TOUCH_START,
+                })), this.registerAction(new Wy({
+                    type: Ny.TOUCH_START,
                     fire: e => {
                         this.transitionWithEvent(this.dragCanvas, e)
                     }
                 }))
             }
         }
-        class yx extends Vy {
+        class bx extends Gy {
             constructor(e = {}) {
-                super(e), this.maxNumberPointsPerLink = 1e3, this.nodeFactories = new Cy, this.linkFactories = new Cy, this.portFactories = new Cy, this.labelFactories = new Cy;
+                super(e), this.maxNumberPointsPerLink = 1e3, this.nodeFactories = new Oy, this.linkFactories = new Oy, this.portFactories = new Oy, this.labelFactories = new Oy;
                 const t = e => {
                     e.registerListener({
                         factoryAdded: e => {
                             e.factory.setDiagramEngine(this)
                         },
                         factoryRemoved: e => {
                             e.factory.setDiagramEngine(null)
@@ -31627,20 +31650,20 @@
                     })
                 };
                 t(this.nodeFactories), t(this.linkFactories), t(this.portFactories), t(this.labelFactories)
             }
             getMouseElement(e) {
                 var t = e.target,
                     n = this.model,
-                    r = Sy.closest(t, ".port[data-name]");
+                    r = Ey.closest(t, ".port[data-name]");
                 if (r) {
-                    var o = Sy.closest(t, ".node[data-nodeid]");
+                    var o = Ey.closest(t, ".node[data-nodeid]");
                     return n.getNode(o.getAttribute("data-nodeid")).getPort(r.getAttribute("data-name"))
                 }
-                return (r = Sy.closest(t, ".point[data-id]")) ? n.getLink(r.getAttribute("data-linkid")).getPointModel(r.getAttribute("data-id")) : (r = Sy.closest(t, "[data-linkid]")) ? n.getLink(r.getAttribute("data-linkid")) : (r = Sy.closest(t, ".node[data-nodeid]")) ? n.getNode(r.getAttribute("data-nodeid")) : null
+                return (r = Ey.closest(t, ".point[data-id]")) ? n.getLink(r.getAttribute("data-linkid")).getPointModel(r.getAttribute("data-id")) : (r = Ey.closest(t, "[data-linkid]")) ? n.getLink(r.getAttribute("data-linkid")) : (r = Ey.closest(t, ".node[data-nodeid]")) ? n.getNode(r.getAttribute("data-nodeid")) : null
             }
             getNodeFactories() {
                 return this.nodeFactories
             }
             getLinkFactories() {
                 return this.linkFactories
             }
@@ -31690,33 +31713,33 @@
                 t || (t = this.getNodePortElement(e));
                 const n = t.getBoundingClientRect(),
                     r = this.getRelativeMousePoint({
                         clientX: n.left,
                         clientY: n.top
                     }),
                     o = this.model.getZoomLevel() / 100;
-                return Ay.fromPointAndSize(r, n.width / o, n.height / o)
+                return Ry.fromPointAndSize(r, n.width / o, n.height / o)
             }
             getNodeDimensions(e) {
                 if (!this.canvas) return {
                     width: 0,
                     height: 0
                 };
                 const t = this.getNodeElement(e).getBoundingClientRect();
                 return {
                     width: t.width,
                     height: t.height
                 }
             }
             getBoundingNodesRect(e) {
-                if (e) return 0 === e.length ? new Ay : new Ay((t = e.map((e => e.getBoundingBox())), My(ky.flatMap(t, (e => e.getPoints())))));
+                if (e) return 0 === e.length ? new Ry : new Ry((t = e.map((e => e.getBoundingBox())), jy(Sy.flatMap(t, (e => e.getPoints())))));
                 var t
             }
             zoomToFitSelectedNodes(e) {
-                const t = this.model.getSelectedEntities().filter((e => e instanceof Cb));
+                const t = this.model.getSelectedEntities().filter((e => e instanceof Ob));
                 this.zoomToFitNodes({
                     margin: e.margin,
                     maxZoom: e.maxZoom,
                     nodes: t.length > 0 ? t : null
                 })
             }
             zoomToFitNodes(e) {
@@ -31744,15 +31767,15 @@
             getMaxNumberPointsPerLink() {
                 return this.maxNumberPointsPerLink
             }
             setMaxNumberPointsPerLink(e) {
                 this.maxNumberPointsPerLink = e
             }
         }
-        class bx extends Pb {
+        class xx extends Mb {
             constructor(e = {}) {
                 super(Object.assign({
                     offsetY: null == e.offsetY ? -23 : e.offsetY,
                     type: "default"
                 }, e))
             }
             setLabel(e) {
@@ -31772,49 +31795,49 @@
 		border-radius: 5px;
 		color: white;
 		font-size: 12px;
 		padding: 4px 8px;
 		font-family: sans-serif;
 		user-select: none;
 	`
-        }(ix || (ix = {}));
-        class xx extends t.Component {
+        }(ax || (ax = {}));
+        class wx extends t.Component {
             render() {
-                return t.createElement(ix.Label, null, this.props.model.getOptions().label)
+                return t.createElement(ax.Label, null, this.props.model.getOptions().label)
             }
         }
-        class wx extends Zy {
+        class kx extends Qy {
             constructor() {
                 super("default")
             }
             generateReactWidget(e) {
-                return t.createElement(xx, {
+                return t.createElement(wx, {
                     model: e.model
                 })
             }
             generateModel(e) {
-                return new bx
+                return new xx
             }
         }
-        class kx extends Eb {
+        class Sx extends Cb {
             constructor(e = {}) {
                 super(Object.assign({
                     type: "default",
                     width: e.width || 3,
                     color: e.color || "gray",
                     selectedColor: e.selectedColor || "rgb(0,192,255)",
                     curvyness: 50
                 }, e))
             }
             calculateControlOffset(e) {
-                return e.getOptions().alignment === ox.RIGHT ? [this.options.curvyness, 0] : e.getOptions().alignment === ox.LEFT ? [-this.options.curvyness, 0] : e.getOptions().alignment === ox.TOP ? [0, -this.options.curvyness] : [0, this.options.curvyness]
+                return e.getOptions().alignment === ix.RIGHT ? [this.options.curvyness, 0] : e.getOptions().alignment === ix.LEFT ? [-this.options.curvyness, 0] : e.getOptions().alignment === ix.TOP ? [0, -this.options.curvyness] : [0, this.options.curvyness]
             }
             getSVGPath() {
                 if (2 == this.points.length) {
-                    const e = new $y;
+                    const e = new zy;
                     return e.setSource(this.getFirstPoint().getPosition()), e.setTarget(this.getLastPoint().getPosition()), e.setSourceControl(this.getFirstPoint().getPosition().clone()), e.setTargetControl(this.getLastPoint().getPosition().clone()), this.sourcePort && e.getSourceControl().translate(...this.calculateControlOffset(this.getSourcePort())), this.targetPort && e.getTargetControl().translate(...this.calculateControlOffset(this.getTargetPort())), e.getSVGCurve()
                 }
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     width: this.options.width,
                     color: this.options.color,
@@ -31822,16 +31845,16 @@
                     selectedColor: this.options.selectedColor
                 })
             }
             deserialize(e) {
                 super.deserialize(e), this.options.color = e.data.color, this.options.width = e.data.width, this.options.curvyness = e.data.curvyness, this.options.selectedColor = e.data.selectedColor
             }
             addLabel(e) {
-                if (e instanceof Pb) return super.addLabel(e);
-                let t = new bx;
+                if (e instanceof Mb) return super.addLabel(e);
+                let t = new xx;
                 return t.setLabel(e), super.addLabel(t)
             }
             setWidth(e) {
                 this.options.width = e, this.fireEvent({
                     width: e
                 }, "widthChanged")
             }
@@ -31840,31 +31863,31 @@
                     color: e
                 }, "colorChanged")
             }
         }! function(e) {
             e.PointTop = b.default.circle`
 		pointer-events: all;
 	`
-        }(ax || (ax = {}));
-        class Sx extends t.Component {
+        }(sx || (sx = {}));
+        class Ex extends t.Component {
             constructor(e) {
                 super(e), this.state = {
                     selected: !1
                 }
             }
             render() {
                 const {
                     point: e
                 } = this.props;
                 return t.createElement("g", null, t.createElement("circle", {
                     cx: e.getPosition().x,
                     cy: e.getPosition().y,
                     r: 5,
                     fill: this.state.selected || this.props.point.isSelected() ? this.props.colorSelected : this.props.color
-                }), t.createElement(ax.PointTop, {
+                }), t.createElement(sx.PointTop, {
                     className: "point",
                     onMouseLeave: () => {
                         this.setState({
                             selected: !1
                         })
                     },
                     onMouseEnter: () => {
@@ -31877,15 +31900,15 @@
                     cx: e.getPosition().x,
                     cy: e.getPosition().y,
                     r: 15,
                     opacity: 0
                 }))
             }
         }
-        class Ex extends t.Component {
+        class Cx extends t.Component {
             render() {
                 const e = t.cloneElement(this.props.factory.generateLinkSegment(this.props.link, this.props.selected || this.props.link.isSelected(), this.props.path), {
                         ref: this.props.forwardRef
                     }),
                     n = t.cloneElement(e, Object.assign(Object.assign({
                         strokeLinecap: "round",
                         onMouseLeave: () => {
@@ -31903,15 +31926,15 @@
                         onContextMenu: () => {
                             this.props.link.isLocked() || (event.preventDefault(), this.props.link.remove())
                         }
                     }));
                 return t.createElement("g", null, e, n)
             }
         }
-        class Cx extends t.Component {
+        class Ox extends t.Component {
             constructor(e) {
                 super(e), this.refPaths = [], this.state = {
                     selected: !1
                 }
             }
             renderPoints() {
                 var e;
@@ -31935,24 +31958,24 @@
                             event: e,
                             model: r
                         })
                     }))
                 }
             }
             generatePoint(e) {
-                return t.createElement(Sx, {
+                return t.createElement(Ex, {
                     key: e.getID(),
                     point: e,
                     colorSelected: this.props.link.getOptions().selectedColor,
                     color: this.props.link.getOptions().color
                 })
             }
             generateLink(e, n, r) {
                 const o = t.createRef();
-                return this.refPaths.push(o), t.createElement(Ex, {
+                return this.refPaths.push(o), t.createElement(Cx, {
                     key: `link-${r}`,
                     path: e,
                     selected: this.state.selected,
                     diagramEngine: this.props.diagramEngine,
                     factory: this.props.diagramEngine.getFactoryForLink(this.props.link),
                     link: this.props.link,
                     forwardRef: o,
@@ -31970,15 +31993,15 @@
                 if (this.refPaths = [], 2 === e.length) n.push(this.generateLink(this.props.link.getSVGPath(), {
                     onMouseDown: e => {
                         var t, n;
                         null === (n = (t = this.props).selected) || void 0 === n || n.call(t, e), this.addPointToLink(e, 1)
                     }
                 }, "0")), null == this.props.link.getTargetPort() && n.push(this.generatePoint(e[1]));
                 else {
-                    for (let t = 0; t < e.length - 1; t++) n.push(this.generateLink(Rb.generateLinePath(e[t], e[t + 1]), {
+                    for (let t = 0; t < e.length - 1; t++) n.push(this.generateLink(Ib.generateLinePath(e[t], e[t + 1]), {
                         "data-linkid": this.props.link.getID(),
                         "data-point": t,
                         onMouseDown: e => {
                             var n, r;
                             null === (r = (n = this.props).selected) || void 0 === r || r.call(n, e), this.addPointToLink(e, t + 1)
                         }
                     }, t));
@@ -32005,46 +32028,46 @@
 		animation: ${e.Keyframes} 1s linear infinite;
 	`;
             e.Path = b.default.path`
 		${e=>e.selected&&t};
 		fill: none;
 		pointer-events: auto;
 	`
-        }(sx || (sx = {}));
-        class Ox extends Zy {
+        }(lx || (lx = {}));
+        class _x extends Qy {
             constructor(e = "default") {
                 super(e)
             }
             generateReactWidget(e) {
-                return t.createElement(Cx, {
+                return t.createElement(Ox, {
                     link: e.model,
                     diagramEngine: this.engine
                 })
             }
             generateModel(e) {
-                return new kx
+                return new Sx
             }
             generateLinkSegment(e, n, r) {
-                return t.createElement(sx.Path, {
+                return t.createElement(lx.Path, {
                     selected: n,
                     stroke: n ? e.getOptions().selectedColor : e.getOptions().color,
                     strokeWidth: e.getOptions().width,
                     d: r
                 })
             }
         }
-        class _x extends fx {
+        class Tx extends hx {
             constructor(e, t, n) {
                 t && (e = {
                     in: !!e,
                     name: t,
                     label: n
                 }), super(Object.assign({
                     label: e.label || e.name,
-                    alignment: e.in ? ox.LEFT : ox.RIGHT,
+                    alignment: e.in ? ix.LEFT : ix.RIGHT,
                     type: "default"
                 }, e))
             }
             deserialize(e) {
                 super.deserialize(e), this.options.in = e.data.in, this.options.label = e.data.label
             }
             serialize() {
@@ -32054,22 +32077,22 @@
                 })
             }
             link(e, t) {
                 let n = this.createLinkModel(t);
                 return n.setSourcePort(this), n.setTargetPort(e), n
             }
             canLinkToPort(e) {
-                return !(e instanceof _x) || this.options.in !== e.getOptions().in
+                return !(e instanceof Tx) || this.options.in !== e.getOptions().in
             }
             createLinkModel(e) {
                 let t = super.createLinkModel();
-                return !t && e ? e.generateModel({}) : t || new kx
+                return !t && e ? e.generateModel({}) : t || new Sx
             }
         }
-        class Tx extends Cb {
+        class Px extends Ob {
             constructor(e = {}, t) {
                 "string" == typeof e && (e = {
                     name: e,
                     color: t
                 }), super(Object.assign({
                     type: "default",
                     name: "Untitled",
@@ -32082,40 +32105,40 @@
             removePort(e) {
                 super.removePort(e), e.getOptions().in ? this.portsIn.splice(this.portsIn.indexOf(e), 1) : this.portsOut.splice(this.portsOut.indexOf(e), 1)
             }
             addPort(e) {
                 return super.addPort(e), e.getOptions().in ? -1 === this.portsIn.indexOf(e) && this.portsIn.push(e) : -1 === this.portsOut.indexOf(e) && this.portsOut.push(e), e
             }
             addInPort(e, t = !0) {
-                const n = new _x({
+                const n = new Tx({
                     in: !0,
                     name: e,
                     label: e,
-                    alignment: ox.LEFT
+                    alignment: ix.LEFT
                 });
                 return t || this.portsIn.splice(0, 0, n), this.addPort(n)
             }
             addOutPort(e, t = !0) {
-                const n = new _x({
+                const n = new Tx({
                     in: !1,
                     name: e,
                     label: e,
-                    alignment: ox.RIGHT
+                    alignment: ix.RIGHT
                 });
                 return t || this.portsOut.splice(0, 0, n), this.addPort(n)
             }
             deserialize(e) {
-                super.deserialize(e), this.options.name = e.data.name, this.options.color = e.data.color, this.portsIn = ky.map(e.data.portsInOrder, (e => this.getPortFromID(e))), this.portsOut = ky.map(e.data.portsOutOrder, (e => this.getPortFromID(e)))
+                super.deserialize(e), this.options.name = e.data.name, this.options.color = e.data.color, this.portsIn = Sy.map(e.data.portsInOrder, (e => this.getPortFromID(e))), this.portsOut = Sy.map(e.data.portsOutOrder, (e => this.getPortFromID(e)))
             }
             serialize() {
                 return Object.assign(Object.assign({}, super.serialize()), {
                     name: this.options.name,
                     color: this.options.color,
-                    portsInOrder: ky.map(this.portsIn, (e => e.getID())),
-                    portsOutOrder: ky.map(this.portsOut, (e => e.getID()))
+                    portsInOrder: Sy.map(this.portsIn, (e => e.getID())),
+                    portsOutOrder: Sy.map(this.portsOut, (e => e.getID()))
                 })
             }
             getInPorts() {
                 return this.portsIn
             }
             getOutPorts() {
                 return this.portsOut
@@ -32133,23 +32156,23 @@
 		height: 15px;
 		background: rgba(255, 255, 255, 0.1);
 
 		&:hover {
 			background: rgb(192, 255, 0);
 		}
 	`
-        }(lx || (lx = {}));
-        class Px extends t.Component {
+        }(ux || (ux = {}));
+        class Mx extends t.Component {
             render() {
-                const e = t.createElement(hx, {
+                const e = t.createElement(gx, {
                         engine: this.props.engine,
                         port: this.props.port
-                    }, t.createElement(lx.Port, null)),
-                    n = t.createElement(lx.Label, null, this.props.port.getOptions().label);
-                return t.createElement(lx.PortLabel, null, this.props.port.getOptions().in ? e : n, this.props.port.getOptions().in ? n : e)
+                    }, t.createElement(ux.Port, null)),
+                    n = t.createElement(ux.Label, null, this.props.port.getOptions().label);
+                return t.createElement(ux.PortLabel, null, this.props.port.getOptions().in ? e : n, this.props.port.getOptions().in ? n : e)
             }
         }! function(e) {
             e.Node = b.default.div`
 		background-color: ${e=>e.background};
 		border-radius: 5px;
 		font-family: sans-serif;
 		color: white;
@@ -32177,78 +32200,78 @@
 			margin-right: 10px;
 		}
 
 		&:only-child {
 			margin-right: 0px;
 		}
 	`
-        }(ux || (ux = {}));
-        class Mx extends t.Component {
+        }(cx || (cx = {}));
+        class jx extends t.Component {
             constructor() {
-                super(...arguments), this.generatePort = e => t.createElement(Px, {
+                super(...arguments), this.generatePort = e => t.createElement(Mx, {
                     engine: this.props.engine,
                     port: e,
                     key: e.getID()
                 })
             }
             render() {
-                return t.createElement(ux.Node, {
+                return t.createElement(cx.Node, {
                     "data-default-node-name": this.props.node.getOptions().name,
                     selected: this.props.node.isSelected(),
                     background: this.props.node.getOptions().color
-                }, t.createElement(ux.Title, null, t.createElement(ux.TitleName, null, this.props.node.getOptions().name)), t.createElement(ux.Ports, null, t.createElement(ux.PortsContainer, null, ky.map(this.props.node.getInPorts(), this.generatePort)), t.createElement(ux.PortsContainer, null, ky.map(this.props.node.getOutPorts(), this.generatePort))))
+                }, t.createElement(cx.Title, null, t.createElement(cx.TitleName, null, this.props.node.getOptions().name)), t.createElement(cx.Ports, null, t.createElement(cx.PortsContainer, null, Sy.map(this.props.node.getInPorts(), this.generatePort)), t.createElement(cx.PortsContainer, null, Sy.map(this.props.node.getOutPorts(), this.generatePort))))
             }
         }
-        class jx extends Zy {
+        class Ax extends Qy {
             constructor() {
                 super("default")
             }
             generateReactWidget(e) {
-                return t.createElement(Mx, {
+                return t.createElement(jx, {
                     engine: this.engine,
                     node: e.model
                 })
             }
             generateModel(e) {
-                return new Tx
+                return new Px
             }
         }
-        class Ax extends Ky {
+        class Rx extends Zy {
             constructor() {
                 super("default")
             }
             generateModel() {
-                return new _x({
+                return new Tx({
                     name: "unknown"
                 })
             }
         }
-        class Rx extends kx {
+        class Ix extends Sx {
             constructor(e = {}) {
                 super(Object.assign({
-                    type: $x.NAME
+                    type: zx.NAME
                 }, e))
             }
             performanceTune() {
                 return !1
             }
         }
-        var Ix = i(9657);
-        const Nx = new Ix.JumpPointFinder({
-            heuristic: Ix.Heuristic.manhattan,
-            diagonalMovement: Ix.DiagonalMovement.Never
+        var Nx = i(9657);
+        const Lx = new Nx.JumpPointFinder({
+            heuristic: Nx.Heuristic.manhattan,
+            diagonalMovement: Nx.DiagonalMovement.Never
         });
-        class Lx {
+        class Dx {
             constructor(e) {
-                this.instance = Nx, this.factory = e
+                this.instance = Lx, this.factory = e
             }
             calculateDirectPath(e, t) {
                 const n = this.factory.getCanvasMatrix(),
-                    r = new Ix.Grid(n);
-                return Nx.findPath(this.factory.translateRoutingX(Math.floor(e.getX() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingY(Math.floor(e.getY() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingX(Math.floor(t.getX() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingY(Math.floor(t.getY() / this.factory.ROUTING_SCALING_FACTOR)), r)
+                    r = new Nx.Grid(n);
+                return Lx.findPath(this.factory.translateRoutingX(Math.floor(e.getX() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingY(Math.floor(e.getY() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingX(Math.floor(t.getX() / this.factory.ROUTING_SCALING_FACTOR)), this.factory.translateRoutingY(Math.floor(t.getY() / this.factory.ROUTING_SCALING_FACTOR)), r)
             }
             calculateLinkStartEndCoords(e, t) {
                 const n = t.findIndex((t => !!e[t[1]] && 0 === e[t[1]][t[0]])),
                     r = t.length - 1 - t.slice().reverse().findIndex((t => !!e[t[1]] && 0 === e[t[1]][t[0]]));
                 if (-1 === n || -1 === r) return;
                 const o = t.slice(0, n),
                     i = t.slice(r);
@@ -32262,38 +32285,38 @@
                         y: t[r][1]
                     },
                     pathToStart: o,
                     pathToEnd: i
                 }
             }
             calculateDynamicPath(e, t, n, r, o) {
-                const i = new Ix.Grid(e),
-                    a = Nx.findPath(t.x, t.y, n.x, n.y, i),
+                const i = new Nx.Grid(e),
+                    a = Lx.findPath(t.x, t.y, n.x, n.y, i),
                     s = r.concat(a, o).map((e => [this.factory.translateRoutingX(e[0], !0), this.factory.translateRoutingY(e[1], !0)]));
-                return Ix.Util.compressPath(s)
+                return Nx.Util.compressPath(s)
             }
         }
-        class Dx extends t.Component {
+        class Fx extends t.Component {
             constructor(e) {
                 super(e), this.refPaths = [], this.state = {
                     selected: !1
-                }, this.pathFinding = new Lx(this.props.factory)
+                }, this.pathFinding = new Dx(this.props.factory)
             }
             componentDidUpdate() {
                 this.props.link.setRenderedPaths(this.refPaths.map((e => e.current)))
             }
             componentDidMount() {
                 this.props.link.setRenderedPaths(this.refPaths.map((e => e.current)))
             }
             componentWillUnmount() {
                 this.props.link.setRenderedPaths([])
             }
             generateLink(e, n) {
                 const r = t.createRef();
-                return this.refPaths.push(r), t.createElement(Ex, {
+                return this.refPaths.push(r), t.createElement(Cx, {
                     key: `link-${n}`,
                     path: e,
                     selected: this.state.selected,
                     diagramEngine: this.props.diagramEngine,
                     factory: this.props.diagramEngine.getFactoryForLink(this.props.link),
                     link: this.props.link,
                     forwardRef: r,
@@ -32305,160 +32328,160 @@
                     extras: {}
                 })
             }
             render() {
                 this.refPaths = [];
                 var e = this.props.link.getPoints(),
                     n = [];
-                const r = this.pathFinding.calculateDirectPath(ky.first(e), ky.last(e)),
+                const r = this.pathFinding.calculateDirectPath(Sy.first(e), Sy.last(e)),
                     o = this.props.factory.getRoutingMatrix(),
                     i = this.pathFinding.calculateLinkStartEndCoords(o, r);
                 if (i) {
                     const {
                         start: e,
                         end: t,
                         pathToStart: r,
                         pathToEnd: a
                     } = i, s = this.pathFinding.calculateDynamicPath(o, e, t, r, a);
                     n.push(this.generateLink(this.props.factory.generateDynamicPath(s), "0"))
                 }
                 return t.createElement(t.Fragment, null, n)
             }
         }
-        var Fx = i(3736);
-        class $x extends Ox {
+        var $x = i(3736);
+        class zx extends _x {
             constructor() {
-                super($x.NAME), this.ROUTING_SCALING_FACTOR = 5, this.canvasMatrix = [], this.routingMatrix = [], this.hAdjustmentFactor = 0, this.vAdjustmentFactor = 0, this.calculateMatrixDimensions = () => {
-                    const e = ky.values(this.engine.getModel().getNodes()).map((e => ({
+                super(zx.NAME), this.ROUTING_SCALING_FACTOR = 5, this.canvasMatrix = [], this.routingMatrix = [], this.hAdjustmentFactor = 0, this.vAdjustmentFactor = 0, this.calculateMatrixDimensions = () => {
+                    const e = Sy.values(this.engine.getModel().getNodes()).map((e => ({
                             x: e.getX(),
                             width: e.width,
                             y: e.getY(),
                             height: e.height
                         }))),
-                        t = ky.values(this.engine.getModel().getLinks()),
-                        n = ky.flatMap(t.map((e => [e.getSourcePort(), e.getTargetPort()]))).filter((e => null !== e)).map((e => ({
+                        t = Sy.values(this.engine.getModel().getLinks()),
+                        n = Sy.flatMap(t.map((e => [e.getSourcePort(), e.getTargetPort()]))).filter((e => null !== e)).map((e => ({
                             x: e.getX(),
                             width: e.width,
                             y: e.getY(),
                             height: e.height
                         }))),
-                        r = ky.flatMap(t.map((e => e.getPoints()))).map((e => ({
+                        r = Sy.flatMap(t.map((e => e.getPoints()))).map((e => ({
                             x: e.getX(),
                             width: 0,
                             y: e.getY(),
                             height: 0
                         }))),
-                        o = (e, t) => ky.reduce(t, ((t, n) => t + ky.get(e, n, 0)), 0),
+                        o = (e, t) => Sy.reduce(t, ((t, n) => t + Sy.get(e, n, 0)), 0),
                         i = this.engine.getCanvas(),
-                        a = ky.concat(e, n, r),
-                        s = Math.floor(Math.min(ky.get(ky.minBy(a, "x"), "x", 0), 0) / this.ROUTING_SCALING_FACTOR) * this.ROUTING_SCALING_FACTOR,
-                        l = ky.maxBy(a, (e => o(e, ["x", "width"]))),
+                        a = Sy.concat(e, n, r),
+                        s = Math.floor(Math.min(Sy.get(Sy.minBy(a, "x"), "x", 0), 0) / this.ROUTING_SCALING_FACTOR) * this.ROUTING_SCALING_FACTOR,
+                        l = Sy.maxBy(a, (e => o(e, ["x", "width"]))),
                         u = Math.max(o(l, ["x", "width"]), i.offsetWidth),
-                        c = ky.minBy(a, "y"),
-                        d = Math.floor(Math.min(ky.get(c, "y", 0), 0) / this.ROUTING_SCALING_FACTOR) * this.ROUTING_SCALING_FACTOR,
-                        p = ky.maxBy(a, (e => o(e, ["y", "height"]))),
+                        c = Sy.minBy(a, "y"),
+                        d = Math.floor(Math.min(Sy.get(c, "y", 0), 0) / this.ROUTING_SCALING_FACTOR) * this.ROUTING_SCALING_FACTOR,
+                        p = Sy.maxBy(a, (e => o(e, ["y", "height"]))),
                         f = Math.max(o(p, ["y", "height"]), i.offsetHeight);
                     return {
                         width: Math.ceil(Math.abs(s) + u),
                         hAdjustmentFactor: Math.abs(s) / this.ROUTING_SCALING_FACTOR + 1,
                         height: Math.ceil(Math.abs(d) + f),
                         vAdjustmentFactor: Math.abs(d) / this.ROUTING_SCALING_FACTOR + 1
                     }
                 }, this.markNodes = e => {
-                    ky.values(this.engine.getModel().getNodes()).forEach((t => {
+                    Sy.values(this.engine.getModel().getNodes()).forEach((t => {
                         const n = Math.floor(t.getX() / this.ROUTING_SCALING_FACTOR),
                             r = Math.ceil((t.getX() + t.width) / this.ROUTING_SCALING_FACTOR),
                             o = Math.floor(t.getY() / this.ROUTING_SCALING_FACTOR),
                             i = Math.ceil((t.getY() + t.height) / this.ROUTING_SCALING_FACTOR);
                         for (let t = n - 1; t <= r + 1; t++)
                             for (let n = o - 1; n < i + 1; n++) this.markMatrixPoint(e, this.translateRoutingX(t), this.translateRoutingY(n))
                     }))
                 }, this.markPorts = e => {
-                    ky.flatMap(ky.values(this.engine.getModel().getLinks()).map((e => [].concat(e.getSourcePort(), e.getTargetPort())))).filter((e => null !== e)).forEach((t => {
+                    Sy.flatMap(Sy.values(this.engine.getModel().getLinks()).map((e => [].concat(e.getSourcePort(), e.getTargetPort())))).filter((e => null !== e)).forEach((t => {
                         const n = Math.floor(t.x / this.ROUTING_SCALING_FACTOR),
                             r = Math.ceil((t.x + t.width) / this.ROUTING_SCALING_FACTOR),
                             o = Math.floor(t.y / this.ROUTING_SCALING_FACTOR),
                             i = Math.ceil((t.y + t.height) / this.ROUTING_SCALING_FACTOR);
                         for (let t = n - 1; t <= r + 1; t++)
                             for (let n = o - 1; n < i + 1; n++) this.markMatrixPoint(e, this.translateRoutingX(t), this.translateRoutingY(n))
                     }))
                 }, this.markMatrixPoint = (e, t, n) => {
                     void 0 !== e[n] && void 0 !== e[n][t] && (e[n][t] = 1)
                 }
             }
             setDiagramEngine(e) {
                 super.setDiagramEngine(e), e.getStateMachine().registerListener({
                     stateChanged: t => {
-                        if (t.newState instanceof ub) {
-                            const t = e.getActionEventBus().registerAction(new zy({
-                                type: Iy.MOUSE_UP,
+                        if (t.newState instanceof cb) {
+                            const t = e.getActionEventBus().registerAction(new Wy({
+                                type: Ny.MOUSE_UP,
                                 fire: () => {
                                     this.calculateRoutingMatrix(), e.repaintCanvas(), t()
                                 }
                             }))
                         }
                     }
                 }), this.listener = e.registerListener({
                     canvasReady: () => {
-                        ky.defer((() => {
+                        Sy.defer((() => {
                             this.calculateRoutingMatrix(), e.repaintCanvas()
                         }))
                     }
                 })
             }
             setFactoryBank(e) {
                 super.setFactoryBank(e), !e && this.listener && this.listener.deregister()
             }
             generateReactWidget(e) {
-                return t.createElement(Dx, {
+                return t.createElement(Fx, {
                     diagramEngine: this.engine,
                     link: e.model,
                     factory: this
                 })
             }
             generateModel(e) {
-                return new Rx
+                return new Ix
             }
             getCanvasMatrix() {
                 return 0 === this.canvasMatrix.length && this.calculateCanvasMatrix(), this.canvasMatrix
             }
             calculateCanvasMatrix() {
                 const {
                     width: e,
                     hAdjustmentFactor: t,
                     height: n,
                     vAdjustmentFactor: r
                 } = this.calculateMatrixDimensions();
                 this.hAdjustmentFactor = t, this.vAdjustmentFactor = r;
                 const o = Math.ceil(e / this.ROUTING_SCALING_FACTOR),
                     i = Math.ceil(n / this.ROUTING_SCALING_FACTOR);
-                this.canvasMatrix = ky.range(0, i).map((() => new Array(o).fill(0)))
+                this.canvasMatrix = Sy.range(0, i).map((() => new Array(o).fill(0)))
             }
             getRoutingMatrix() {
                 return 0 === this.routingMatrix.length && this.calculateRoutingMatrix(), this.routingMatrix
             }
             calculateRoutingMatrix() {
-                const e = ky.cloneDeep(this.getCanvasMatrix());
+                const e = Sy.cloneDeep(this.getCanvasMatrix());
                 this.markNodes(e), this.markPorts(e), this.routingMatrix = e
             }
             translateRoutingX(e, t = !1) {
                 return e + this.hAdjustmentFactor * (t ? -1 : 1)
             }
             translateRoutingY(e, t = !1) {
                 return e + this.vAdjustmentFactor * (t ? -1 : 1)
             }
             generateDynamicPath(e) {
-                let t = Fx();
+                let t = $x();
                 return t = t.moveto(e[0][0] * this.ROUTING_SCALING_FACTOR, e[0][1] * this.ROUTING_SCALING_FACTOR), e.slice(1).forEach((e => {
                     t = t.lineto(e[0] * this.ROUTING_SCALING_FACTOR, e[1] * this.ROUTING_SCALING_FACTOR)
                 })), t.print()
             }
         }
-        $x.NAME = "pathfinding";
-        class zx extends t.Component {
+        zx.NAME = "pathfinding";
+        class Wx extends t.Component {
             constructor(e) {
                 super(e), this.handleMove = function(e) {
                     this.draggingEvent(e, this.dragging_index)
                 }.bind(this), this.handleUp = function(e) {
                     this.setState({
                         canDrag: !1,
                         selected: !1
@@ -32475,15 +32498,15 @@
                 this.props.link.setRenderedPaths(this.refPaths.map((e => e.current)))
             }
             componentWillUnmount() {
                 this.props.link.setRenderedPaths([])
             }
             generateLink(e, n, r) {
                 const o = t.createRef();
-                return this.refPaths.push(o), t.createElement(Ex, {
+                return this.refPaths.push(o), t.createElement(Cx, {
                     key: `link-${r}`,
                     path: e,
                     selected: this.state.selected,
                     diagramEngine: this.props.diagramEngine,
                     factory: this.props.diagramEngine.getFactoryForLink(this.props.link),
                     link: this.props.link,
                     forwardRef: o,
@@ -32493,24 +32516,24 @@
                         })
                     },
                     extras: n
                 })
             }
             calculatePositions(e, t, n, r) {
                 if (0 === n) {
-                    let t = new Sb({
+                    let t = new Eb({
                         link: this.props.link,
-                        position: new _y(e[n].getX(), e[n].getY())
+                        position: new Ty(e[n].getX(), e[n].getY())
                     });
                     return this.props.link.addPoint(t, n), void this.dragging_index++
                 }
                 if (n === e.length - 2) {
-                    let t = new Sb({
+                    let t = new Eb({
                         link: this.props.link,
-                        position: new _y(e[n + 1].getX(), e[n + 1].getY())
+                        position: new Ty(e[n + 1].getX(), e[n + 1].getY())
                     });
                     return void this.props.link.addPoint(t, n + 1)
                 }
                 if (n - 2 > 0) {
                     let o = {
                         [n - 2]: e[n - 2].getPosition(),
                         [n + 1]: e[n + 1].getPosition(),
@@ -32544,27 +32567,27 @@
                     n = [],
                     r = e[0],
                     o = e[e.length - 1],
                     i = !1;
                 r.getX() > o.getX() && (r = e[e.length - 1], o = e[0], i = !0);
                 let a = Math.abs(e[0].getY() - e[e.length - 1].getY());
                 if (null === this.props.link.getTargetPort() && 2 === e.length)[...Array(2)].forEach((e => {
-                    this.props.link.addPoint(new Sb({
+                    this.props.link.addPoint(new Eb({
                         link: this.props.link,
-                        position: new _y(r.getX(), o.getY())
+                        position: new Ty(r.getX(), o.getY())
                     }), 1)
                 })), this.props.link.setManuallyFirstAndLastPathsDirection(!0, !0);
                 else if (null === this.props.link.getTargetPort() && null !== this.props.link.getSourcePort()) e[1].setPosition(o.getX() + (r.getX() - o.getX()) / 2, i ? o.getY() : r.getY()), e[2].setPosition(o.getX() + (r.getX() - o.getX()) / 2, i ? r.getY() : o.getY());
                 else if (!this.state.canDrag && e.length > 2)
                     for (let t = 1; t < e.length; t += e.length - 2) t - 1 == 0 ? this.props.link.getFirstPathXdirection() ? e[t].setPosition(e[t].getX(), e[t - 1].getY()) : e[t].setPosition(e[t - 1].getX(), e[t].getY()) : this.props.link.getLastPathXdirection() ? e[t - 1].setPosition(e[t - 1].getX(), e[t].getY()) : e[t - 1].setPosition(e[t].getX(), e[t - 1].getY());
-                2 !== e.length || 0 === a || this.state.canDrag || this.props.link.addPoint(new Sb({
+                2 !== e.length || 0 === a || this.state.canDrag || this.props.link.addPoint(new Eb({
                     link: this.props.link,
-                    position: new _y(r.getX(), o.getY())
+                    position: new Ty(r.getX(), o.getY())
                 }));
-                for (let t = 0; t < e.length - 1; t++) n.push(this.generateLink(Rb.generateLinePath(e[t], e[t + 1]), {
+                for (let t = 0; t < e.length - 1; t++) n.push(this.generateLink(Ib.generateLinePath(e[t], e[t + 1]), {
                     "data-linkid": this.props.link.getID(),
                     "data-point": t,
                     onMouseDown: e => {
                         0 === e.button && (this.setState({
                             canDrag: !0
                         }), this.dragging_index = t, window.addEventListener("mousemove", this.handleMove), window.addEventListener("mouseup", this.handleUp))
                     },
@@ -32575,26 +32598,26 @@
                     }
                 }, t));
                 return this.refPaths = [], t.createElement("g", {
                     "data-default-link-test": this.props.link.getOptions().testName
                 }, n)
             }
         }
-        zx.defaultProps = {
+        Wx.defaultProps = {
             color: "red",
             width: 3,
             link: null,
             smooth: !1,
             diagramEngine: null,
             factory: null
         };
-        class Wx extends kx {
+        class Bx extends Sx {
             constructor(e = {}) {
                 super(Object.assign({
-                    type: Bx.NAME
+                    type: Ux.NAME
                 }, e)), this.lastHoverIndexOfPath = 0, this._lastPathXdirection = !1, this._firstPathXdirection = !1
             }
             setFirstAndLastPathsDirection() {
                 let e = this.getPoints();
                 for (let t = 1; t < e.length; t += e.length - 2) {
                     let n = Math.abs(e[t].getX() - e[t - 1].getX()),
                         r = Math.abs(e[t].getY() - e[t - 1].getY());
@@ -32623,91 +32646,91 @@
             }
             setColor(e) {
                 this.options.color = e, this.fireEvent({
                     color: e
                 }, "colorChanged")
             }
         }
-        class Bx extends Ox {
+        class Ux extends _x {
             constructor() {
-                super(Bx.NAME)
+                super(Ux.NAME)
             }
             generateModel(e) {
-                return new Wx
+                return new Bx
             }
             generateReactWidget(e) {
-                return t.createElement(zx, {
+                return t.createElement(Wx, {
                     diagramEngine: this.engine,
                     link: e.model,
                     factory: this
                 })
             }
         }
-        Bx.NAME = "rightAngle";
-        var Ux = i(681);
-        class Yx {
+        Ux.NAME = "rightAngle";
+        var Yx = i(681);
+        class Hx {
             constructor(e = {}) {
                 this.options = e
             }
             redistribute(e) {
-                var t = new Ux.graphlib.Graph({
+                var t = new Yx.graphlib.Graph({
                     multigraph: !0,
                     compound: !0
                 });
                 t.setGraph(this.options.graph || {}), t.setDefaultEdgeLabel((function() {
                     return {}
-                })), ky.forEach(e.getNodes(), (e => {
+                })), Sy.forEach(e.getNodes(), (e => {
                     t.setNode(e.getID(), {
                         width: e.width,
                         height: e.height
                     })
-                })), ky.forEach(e.getLinks(), (e => {
+                })), Sy.forEach(e.getLinks(), (e => {
                     e.getSourcePort() && e.getTargetPort() && t.setEdge({
                         v: e.getSourcePort().getNode().getID(),
                         w: e.getTargetPort().getNode().getID(),
                         name: e.getID()
                     })
-                })), Ux.layout(t), t.nodes().forEach((n => {
+                })), Yx.layout(t), t.nodes().forEach((n => {
                     const r = t.node(n);
                     e.getNode(n).setPosition(r.x - r.width / 2, r.y - r.height / 2)
                 })), this.options.includeLinks && t.edges().forEach((n => {
                     const r = t.edge(n),
                         o = e.getLink(n.name),
                         i = [o.getFirstPoint()];
-                    for (let e = 1; e < r.points.length - 1; e++) i.push(new Sb({
+                    for (let e = 1; e < r.points.length - 1; e++) i.push(new Eb({
                         link: o,
-                        position: new _y(r.points[e].x, r.points[e].y)
+                        position: new Ty(r.points[e].x, r.points[e].y)
                     }));
                     o.setPoints(i.concat(o.getLastPoint()))
                 }))
             }
             refreshLinks(e) {
                 const {
                     nodeMargin: t
                 } = this.options, n = e.getNodes(), r = e.getLinks();
                 let o = -1;
                 const i = {},
                     a = {};
                 let s = [];
-                ky.forEach(n, (e => {
+                Sy.forEach(n, (e => {
                     const n = e.getX() + e.width / 2;
-                    ky.every(s, (e => Math.abs(n - e) > t)) && s.push(n)
-                })), s = s.sort(((e, t) => e - t)), ky.forEach(s, ((e, t) => {
+                    Sy.every(s, (e => Math.abs(n - e) > t)) && s.push(n)
+                })), s = s.sort(((e, t) => e - t)), Sy.forEach(s, ((e, t) => {
                     i[t] = {}, i[t + .5] = {}
-                })), ky.forEach(n, (e => {
+                })), Sy.forEach(n, (e => {
                     const n = e.getX() + e.width / 2,
                         r = Math.floor(e.getY() / t),
                         l = Math.floor((e.getY() + e.height) / t);
                     l > o && (o = l);
-                    const u = ky.findIndex(s, (e => Math.abs(n - e) <= t));
-                    ky.forEach(ky.range(r, l + 1), (e => {
+                    const u = Sy.findIndex(s, (e => Math.abs(n - e) <= t));
+                    Sy.forEach(Sy.range(r, l + 1), (e => {
                         i[u][e] = !0
                     })), a[e.getX()] = u
                 }));
-                const l = ky.map(r, (e => {
+                const l = Sy.map(r, (e => {
                         if (e.getSourcePort() && e.getTargetPort()) {
                             const t = e.getSourcePort().getNode(),
                                 n = e.getTargetPort().getNode(),
                                 r = a[t.getX()],
                                 o = a[n.getX()];
                             return r > o ? {
                                 link: e,
@@ -32724,102 +32747,102 @@
                                 source: n,
                                 targetIndex: r,
                                 targetY: t.getY() + t.height / 2,
                                 target: t
                             }
                         }
                     })),
-                    u = ky.sortBy(l, (e => Math.abs(e.targetIndex - e.sourceIndex)));
-                this.options.includeLinks && ky.forEach(u, (n => {
+                    u = Sy.sortBy(l, (e => Math.abs(e.targetIndex - e.sourceIndex)));
+                this.options.includeLinks && Sy.forEach(u, (n => {
                     const r = e.getLink(n.link.getID());
                     if (Math.abs(n.sourceIndex - n.targetIndex) > 1) {
-                        const e = ky.range(n.sourceIndex - 1, n.targetIndex),
+                        const e = Sy.range(n.sourceIndex - 1, n.targetIndex),
                             a = Math.floor(n.sourceY / t),
                             l = Math.floor(n.targetY / t);
                         let u = 1,
                             c = a;
-                        for (; c >= 0 && !ky.every(e, (e => !(i[e][c] || i[e + .5][c] || i[e - .5][c]))); c--, u++);
+                        for (; c >= 0 && !Sy.every(e, (e => !(i[e][c] || i[e + .5][c] || i[e - .5][c]))); c--, u++);
                         let d = 0,
                             p = a;
-                        for (; p <= o && !ky.every(e, (e => !(i[e][p] || i[e + .5][p] || i[e - .5][p]))); p++, d++);
+                        for (; p <= o && !Sy.every(e, (e => !(i[e][p] || i[e + .5][p] || i[e - .5][p]))); p++, d++);
                         const f = d + (p - l) < u + (l - c) ? p + 1 : c - 1,
                             h = [r.getFirstPoint()];
-                        h.push(new Sb({
+                        h.push(new Eb({
                             link: r,
-                            position: new _y((s[e[0]] + s[e[0] + 1]) / 2, (f + .5) * t)
-                        })), ky.forEach(e, (e => {
-                            h.push(new Sb({
+                            position: new Ty((s[e[0]] + s[e[0] + 1]) / 2, (f + .5) * t)
+                        })), Sy.forEach(e, (e => {
+                            h.push(new Eb({
                                 link: r,
-                                position: new _y(s[e], (f + .5) * t)
-                            })), h.push(new Sb({
+                                position: new Ty(s[e], (f + .5) * t)
+                            })), h.push(new Eb({
                                 link: r,
-                                position: new _y((s[e] + s[e - 1]) / 2, (f + .5) * t)
+                                position: new Ty((s[e] + s[e - 1]) / 2, (f + .5) * t)
                             })), i[e][f] = !0, i[e][f + 1] = !0, i[e + .5][f] = !0, i[e + .5][f + 1] = !0
                         })), r.setPoints(h.concat(r.getLastPoint()))
                     } else {
                         r.setPoints([r.getFirstPoint(), r.getLastPoint()]);
                         const e = (n.sourceIndex + n.targetIndex) / 2;
                         i[e] || (i[e] = {});
                         const o = Math.floor((n.sourceY + n.targetY) / 2 / t);
                         i[e][o] = !0, i[e][o + 1] = !0
                     }
                 }))
             }
         }
-        const Hx = "DataNode",
-            Vx = "Task",
-            Gx = "Pipeline",
-            qx = "Scenario",
-            Xx = {
-                [Hx]: "#283282",
-                [Vx]: "#ff462b",
+        const Vx = "DataNode",
+            Gx = "Task",
+            qx = "Pipeline",
+            Xx = "Scenario",
+            Kx = {
+                [Vx]: "#283282",
                 [Gx]: "#ff462b",
-                [qx]: "#f0faff"
+                [qx]: "#ff462b",
+                [Xx]: "#f0faff"
             },
-            Kx = e => Xx[e] || "pink",
-            Zx = [Hx, Gx, qx, Vx],
-            Qx = {
-                [Vx]: Hx,
+            Zx = e => Kx[e] || "pink",
+            Qx = [Vx, qx, Xx, Gx],
+            Jx = {
                 [Gx]: Vx,
-                [qx]: Gx
+                [qx]: Gx,
+                [Xx]: qx
             };
-        class Jx extends Tb {}
-        class ew extends Tx {
+        class ew extends Pb {}
+        class tw extends Px {
             constructor(e) {
                 super(e), this.subtype = null == e ? void 0 : e.subtype
             }
         }
-        class tw extends _x {
+        class nw extends Tx {
             static createInPort() {
-                return new tw({
+                return new nw({
                     in: !0,
-                    name: aw,
-                    label: aw,
-                    alignment: ox.LEFT
+                    name: sw,
+                    label: sw,
+                    alignment: ix.LEFT
                 })
             }
             static createOutPort() {
-                return new tw({
+                return new nw({
                     in: !1,
-                    name: sw,
-                    label: sw,
-                    alignment: ox.RIGHT
+                    name: lw,
+                    label: lw,
+                    alignment: ix.RIGHT
                 })
             }
             constructor(e) {
                 super(Object.assign(Object.assign({}, e), {
                     type: "taipy-port"
                 }))
             }
             canLinkToPort(e) {
                 var t, n, r;
-                return !(this.options.in || !e.getOptions().in || (null === (t = e.getNode()) || void 0 === t ? void 0 : t.getType()) !== (r = null === (n = this.getNode()) || void 0 === n ? void 0 : n.getType(), Qx[r] || "") && (e.getNode().getType() != Vx || this.getNode().getType() != Hx) || Object.values(this.getLinks()).some((t => t.getTargetPort() === e)))
+                return !(this.options.in || !e.getOptions().in || (null === (t = e.getNode()) || void 0 === t ? void 0 : t.getType()) !== (r = null === (n = this.getNode()) || void 0 === n ? void 0 : n.getType(), Jx[r] || "") && (e.getNode().getType() != Gx || this.getNode().getType() != Vx) || Object.values(this.getLinks()).some((t => t.getTargetPort() === e)))
             }
         }
-        var nw;
+        var rw;
         ! function(e) {
             e.Node = b.default.div`
         background-color: ${e=>e.background};
         border-radius: 5px;
         color: white;
         border: solid 2px black;
         overflow: visible;
@@ -32854,271 +32877,280 @@
     `, e.InPortLabel = b.default.div`
         display: flex;
         align-items: end;
         & svg {
             display: block;
         }
     `
-        }(nw || (nw = {}));
-        const rw = ({
+        }(rw || (rw = {}));
+        const ow = ({
             node: n,
             engine: r
         }) => {
-            const o = (0, t.useCallback)((t => t.getName() == aw ? (0, e.jsx)(nw.InPortLabel, {
-                children: (0, e.jsx)(hx, {
+            const o = (0, t.useCallback)((t => t.getName() == sw ? (0, e.jsx)(rw.InPortLabel, {
+                children: (0, e.jsx)(gx, {
                     engine: r,
                     port: t,
                     children: (0, e.jsx)(og, {})
                 }, t.getID())
-            }, "inlabel") : (0, e.jsx)(nw.OutPortLabel, {
-                children: (0, e.jsx)(hx, {
+            }, "inlabel") : (0, e.jsx)(rw.OutPortLabel, {
+                children: (0, e.jsx)(gx, {
                     engine: r,
                     port: t,
                     children: (0, e.jsx)(ig, {})
                 }, t.getID())
             }, "outlabel")), [r]);
-            return (0, e.jsxs)(nw.Node, {
+            return (0, e.jsxs)(rw.Node, {
                 "data-default-node-name": n.getOptions().name,
                 selected: n.isSelected(),
                 background: n.getOptions().color,
-                children: [(0, e.jsxs)(nw.Title, {
-                    children: [(0, e.jsx)(nw.TitleIcon, {
+                children: [(0, e.jsxs)(rw.Title, {
+                    children: [(0, e.jsx)(rw.TitleIcon, {
                         className: "icon",
                         title: n.getType(),
-                        children: n.getType() == Hx ? (0, e.jsx)(eg, {}) : n.getType() == Vx ? (0, e.jsx)(rg, {}) : n.getType() == Gx ? (0, e.jsx)(tg, {}) : (0, e.jsx)(ng, {})
-                    }), (0, e.jsxs)(nw.TitleName, {
-                        children: [n.getOptions().name, n.subtype ? (0, e.jsx)(nw.SubTitleName, {
+                        children: n.getType() == Vx ? (0, e.jsx)(eg, {}) : n.getType() == Gx ? (0, e.jsx)(rg, {}) : n.getType() == qx ? (0, e.jsx)(tg, {}) : (0, e.jsx)(ng, {})
+                    }), (0, e.jsxs)(rw.TitleName, {
+                        children: [n.getOptions().name, n.subtype ? (0, e.jsx)(rw.SubTitleName, {
                             children: n.subtype
                         }) : null]
                     })]
-                }), (0, e.jsxs)(nw.Ports, {
-                    children: [(0, e.jsx)(nw.PortsContainer, {
+                }), (0, e.jsxs)(rw.Ports, {
+                    children: [(0, e.jsx)(rw.PortsContainer, {
                         children: n.getInPorts().map(o)
-                    }), (0, e.jsx)(nw.PortsContainer, {
+                    }), (0, e.jsx)(rw.PortsContainer, {
                         children: n.getOutPorts().map(o)
                     })]
                 })]
             })
         };
-        class ow extends Zy {
+        class iw extends Qy {
             constructor(e) {
                 super(e)
             }
             generateReactWidget(t) {
-                return (0, e.jsx)(rw, {
+                return (0, e.jsx)(ow, {
                     engine: this.engine,
                     node: t.model
                 })
             }
             generateModel() {
-                return new ew
+                return new tw
             }
         }
-        class iw extends Ky {
+        class aw extends Zy {
             constructor() {
                 super("taipy-port")
             }
             generateModel() {
-                return new tw({
+                return new nw({
                     type: "taipy-port",
                     name: "fred"
                 })
             }
         }
-        const aw = "In",
-            sw = "Out",
-            lw = (e, t, n) => {
+        const sw = "In",
+            lw = "Out",
+            uw = (e, t, n) => {
                 const r = (n.getX() - t.getX()) * (n.getX() - t.getX()) + (n.getY() - t.getY()) * (n.getY() - t.getY());
                 if (0 === r) return !1;
                 const o = ((e.getX() - t.getX()) * (n.getX() - t.getX()) + (e.getY() - t.getY()) * (n.getY() - t.getY())) / r;
                 if (0 <= o && o <= 1) {
                     const o = ((t.getY() - e.getY()) * (n.getX() - t.getX()) - (t.getX() - e.getX()) * (n.getY() - t.getY())) / r;
-                    return Math.abs(o) * Math.sqrt(r) <= uw
+                    return Math.abs(o) * Math.sqrt(r) <= cw
                 }
                 return !1
             },
-            uw = .1,
-            cw = {
+            cw = .1,
+            dw = {
                 "&>div": {
                     height: "100%",
                     width: "100%"
                 },
                 height: "100%",
                 width: "100%"
             },
-            dw = {
+            pw = {
                 ml: 2,
                 flex: 1
             },
-            pw = {
+            fw = {
                 position: "relative"
             },
-            [fw, hw] = (() => {
+            [hw, gw] = (() => {
                 const e = ((e = {}) => {
-                    const t = new yx(e);
-                    return t.getLayerFactories().registerFactory(new px), t.getLayerFactories().registerFactory(new Nb), t.getLayerFactories().registerFactory(new ab), t.getLabelFactories().registerFactory(new wx), t.getNodeFactories().registerFactory(new jx), t.getLinkFactories().registerFactory(new Ox), t.getLinkFactories().registerFactory(new $x), t.getPortFactories().registerFactory(new Ax), t.getStateMachine().pushState(new mx), t
+                    const t = new bx(e);
+                    return t.getLayerFactories().registerFactory(new fx), t.getLayerFactories().registerFactory(new Lb), t.getLayerFactories().registerFactory(new sb), t.getLabelFactories().registerFactory(new kx), t.getNodeFactories().registerFactory(new Ax), t.getLinkFactories().registerFactory(new _x), t.getLinkFactories().registerFactory(new zx), t.getPortFactories().registerFactory(new Rx), t.getStateMachine().pushState(new yx), t
                 })();
-                Zx.forEach((t => e.getNodeFactories().registerFactory(new ow(t)))), e.getPortFactories().registerFactory(new iw);
+                Qx.forEach((t => e.getNodeFactories().registerFactory(new iw(t)))), e.getPortFactories().registerFactory(new aw);
                 const t = e.getStateMachine().getCurrentState();
-                t instanceof mx && (t.dragNewLink.config.allowLooseLinks = !1);
-                const n = new Yx({
+                t instanceof yx && (t.dragNewLink.config.allowLooseLinks = !1);
+                const n = new Hx({
                         graph: {
                             rankdir: "LR",
                             ranker: "longest-path",
                             marginx: 25,
                             marginy: 25
                         },
                         includeLinks: !1
                     }),
-                    r = new Jx;
+                    r = new ew;
                 return e.setModel(r), [e, n, r]
             })(),
-            gw = () => ((e, t) => {
+            vw = () => ((e, t) => {
                 const n = e.getModel();
                 t.redistribute(n), (e => Object.values(e.getActiveLinkLayer().getLinks()))(n).forEach((e => {
                     const t = e.getPoints();
-                    if (3 === t.length)(Math.abs(t[0].getX() - t[2].getX()) < uw || Math.abs(t[0].getY() - t[2].getY()) < uw) && (t.splice(1, 1), e.setPoints(t));
+                    if (3 === t.length)(Math.abs(t[0].getX() - t[2].getX()) < cw || Math.abs(t[0].getY() - t[2].getY()) < cw) && (t.splice(1, 1), e.setPoints(t));
                     else if (t.length > 3) {
                         const n = [];
                         let r = 0;
-                        for (; r + 2 < t.length;) lw(t[r + 1], t[r], t[r + 2]) && n.push(r + 1), r++;
+                        for (; r + 2 < t.length;) uw(t[r + 1], t[r], t[r + 2]) && n.push(r + 1), r++;
                         n.reverse().forEach((e => t.splice(e, 1))), e.setPoints(t)
                     }
                 })), e.repaintCanvas()
-            })(fw, hw),
-            vw = () => fw.zoomToFit(),
-            mw = t => (0, e.jsx)(yb, {
-                sx: pw,
-                children: (0, e.jsxs)(kb, {
+            })(hw, gw),
+            mw = () => hw.zoomToFit(),
+            yw = t => (0, e.jsx)(bb, {
+                sx: fw,
+                children: (0, e.jsxs)(Sb, {
                     children: [(0, e.jsx)(Ft, {
-                        sx: dw
+                        sx: pw
                     }), " ", (0, e.jsx)(zr, {
                         edge: "end",
                         color: "inherit",
                         onClick: t.zoomToFit,
                         title: "zoom to fit",
                         children: (0, e.jsx)(Rs.ZoomIn, {})
                     })]
                 })
             }),
-            yw = n => {
+            bw = e => 3 == e.length && "string" == typeof e[0] ? e : 1 == e.length ? e[0] : void 0,
+            xw = n => {
                 const {
                     showToolbar: r = !0
                 } = n, [o, i] = (0, t.useState)(""), a = (0, Qh.useDispatch)(), s = (0, Qh.useModule)(), l = (0, Qh.useDynamicProperty)(n.render, n.defaultRender, !0), u = vg(n.libClassName, n.dynamicClassName, n.className), c = (0, t.useMemo)((() => ({
-                    width: n.width || "50vw",
+                    width: n.width || "100%",
                     height: n.height || "50vh"
                 })), [n.width, n.height]);
-                return (0, t.useEffect)((() => {
+                (0, t.useEffect)((() => {
                     var e;
                     const t = null === (e = n.coreChanged) || void 0 === e ? void 0 : e.scenario;
                     ("string" == typeof t ? t === o : Array.isArray(t) ? t.includes(o) : t) && n.updateVarName && a((0, Qh.createRequestUpdateAction)(n.id, s, [n.updateVarName], !0))
-                }), [n.coreChanged, n.updateVarName, o, s, a, n.id]), (0, t.useEffect)((() => {
-                    const e = Array.isArray(n.scenario) ? 3 == n.scenario.length && "string" == typeof n.scenario[0] ? n.scenario : 1 == n.scenario.length ? n.scenario[0] : void 0 : void 0,
-                        t = new Jx;
-                    e && n.scenario && (i(e[0]), ((e, t) => {
+                }), [n.coreChanged, n.updateVarName, o, s, a, n.id]);
+                const d = (0, t.useMemo)((() => {
+                    let e;
+                    if (Array.isArray(n.scenario)) e = bw(n.scenario);
+                    else if (n.defaultScenario) try {
+                        e = bw(JSON.parse(n.defaultScenario))
+                    } catch (e) {}
+                    return e
+                }), [n.scenario, n.defaultScenario]);
+                return (0, t.useEffect)((() => {
+                    const e = new ew;
+                    d && (i(d[0]), ((e, t) => {
                         const n = [],
                             r = {};
                         e[1] && Object.entries(e[1]).forEach((([e, t]) => {
                             Object.entries(t).forEach((([t, n]) => {
-                                const o = ((e, t, n, r) => new ew({
+                                const o = ((e, t, n, r) => new tw({
                                     id: t,
                                     type: e,
                                     name: n,
-                                    color: Kx(e),
+                                    color: Zx(e),
                                     subtype: r
                                 }))(e, t, n.name, n.type);
                                 r[e] = r[e] || {}, r[e][t] = o
                             }))
                         })), Array.isArray(e[2]) && e[2].forEach((([e, t, o, i]) => {
                             const a = r[e] && r[e][t],
                                 s = r[o] && r[o][i];
                             if (a && s) {
-                                const e = (l = a.getPort(sw) || a.addOutPort(sw), u = s.getPort(aw) || s.addInPort(aw), l.link(u));
+                                const e = (l = a.getPort(lw) || a.addOutPort(lw), u = s.getPort(sw) || s.addInPort(sw), l.link(u));
                                 n.push(e)
                             }
                             var l, u
                         }));
                         const o = t.getActiveNodeLayer();
                         Object.values(r).forEach((e => Object.values(e).forEach((e => o.addModel(e)))));
                         const i = t.getActiveLinkLayer();
                         n.forEach((e => i.addModel(e)))
-                    })(e, t)), fw.setModel(t), t.setLocked(!0), setTimeout(gw, 500)
-                }), [n.scenario]), (0, t.useEffect)((() => {
+                    })(d, e)), hw.setModel(e), e.setLocked(!0), setTimeout(vw, 500)
+                }), [d]), (0, t.useEffect)((() => {
                     const e = (0, Qh.getUpdateVar)(n.updateVars, "show");
                     e && a((0, Qh.createSendUpdateAction)(e, l, s))
-                }), [l, n.updateVars, a, s]), l ? (0, e.jsxs)(Ft, {
+                }), [l, n.updateVars, a, s]), l && o ? (0, e.jsxs)(Ft, {
                     sx: c,
                     id: n.id,
                     className: u,
-                    children: [r && o ? (0, e.jsx)(mw, {
-                        zoomToFit: vw
+                    children: [r ? (0, e.jsx)(yw, {
+                        zoomToFit: mw
                     }) : null, (0, e.jsx)(Ft, {
-                        sx: cw,
-                        children: (0, e.jsx)(nb, {
-                            engine: fw
+                        sx: dw,
+                        children: (0, e.jsx)(rb, {
+                            engine: hw
                         })
                     })]
                 }) : null
             };
-        var bw;
+        var ww;
         ! function(e) {
             e[e.CYCLE = 0] = "CYCLE", e[e.SCENARIO = 1] = "SCENARIO", e[e.PIPELINE = 2] = "PIPELINE", e[e.NODE = 3] = "NODE"
-        }(bw || (bw = {}));
-        const xw = {
+        }(ww || (ww = {}));
+        const kw = {
                 display: "flex",
                 alignItems: "center",
                 gap: 1
             },
-            ww = t => {
+            Sw = t => {
                 const [n, r, o = [], i, a] = t.item;
-                return t.displayCycles || i !== bw.CYCLE ? (0, e.jsx)(el, {
+                return t.displayCycles || i !== ww.CYCLE ? (0, e.jsx)(el, {
                     nodeId: n,
-                    "data-selectable": i === bw.NODE,
+                    "data-selectable": i === ww.NODE,
                     label: (0, e.jsxs)(Ft, {
-                        sx: xw,
-                        children: [i === bw.CYCLE ? (0, e.jsx)(Jh, {
+                        sx: kw,
+                        children: [i === ww.CYCLE ? (0, e.jsx)(Jh, {
                             fontSize: "small",
                             color: "primary"
-                        }) : i === bw.SCENARIO ? t.showPrimaryFlag && a ? (0, e.jsx)(Rt, {
+                        }) : i === ww.SCENARIO ? t.showPrimaryFlag && a ? (0, e.jsx)(Rt, {
                             badgeContent: (0, e.jsx)(Rs.FlagOutlined, {
                                 sx: cg
                             }),
                             color: "primary",
                             anchorOrigin: dg,
                             sx: pg,
                             children: (0, e.jsx)(ng, {
                                 fontSize: "small",
                                 color: "primary"
                             })
                         }) : (0, e.jsx)(ng, {
                             fontSize: "small",
                             color: "primary"
-                        }) : i === bw.PIPELINE ? (0, e.jsx)(tg, {
+                        }) : i === ww.PIPELINE ? (0, e.jsx)(tg, {
                             fontSize: "small",
                             color: "primary"
                         }) : (0, e.jsx)(eg, {
                             fontSize: "small",
                             color: "primary"
                         }), r]
                     }),
-                    sx: i === bw.NODE ? void 0 : gg,
-                    children: o.map((n => (0, e.jsx)(ww, {
+                    sx: i === ww.NODE ? void 0 : gg,
+                    children: o.map((n => (0, e.jsx)(Sw, {
                         item: n,
                         displayCycles: !0,
                         showPrimaryFlag: t.showPrimaryFlag
                     }, n[0])))
                 }, n) : (0, e.jsx)(e.Fragment, {
-                    children: o.map((n => (0, e.jsx)(ww, {
+                    children: o.map((n => (0, e.jsx)(Sw, {
                         item: n,
                         displayCycles: !1,
                         showPrimaryFlag: t.showPrimaryFlag
                     }, n[0])))
                 })
             },
-            kw = n => {
+            Ew = n => {
                 const {
                     id: r = "",
                     datanodes: o = [],
                     propagate: i = !0
                 } = n, [a, s] = (0, t.useState)(""), l = vg(n.libClassName, n.dynamicClassName, n.className), u = (0, Qh.useDispatch)(), c = (0, Qh.useModule)();
                 (0, Qh.useDispatchRequestUpdateOnFirstRender)(u, r, c, n.updateVars);
                 const d = (0, Qh.useDynamicProperty)(n.displayCycles, n.defaultDisplayCycles, !0),
@@ -33156,15 +33188,15 @@
                     className: l,
                     children: [(0, e.jsx)(cl, {
                         defaultCollapseIcon: (0, e.jsx)(Rs.ExpandMore, {}),
                         defaultExpandIcon: (0, e.jsx)(Rs.ChevronRight, {}),
                         sx: g,
                         onNodeSelect: f,
                         selected: a,
-                        children: o.map((t => (0, e.jsx)(ww, {
+                        children: o.map((t => (0, e.jsx)(Sw, {
                             item: t,
                             displayCycles: d,
                             showPrimaryFlag: p
                         }, t[0])))
                     }), (0, e.jsx)(Ft, {
                         children: n.error
                     })]
```

### Comparing `taipy-2.3.0.dev5/src/taipy/version.py` & `taipy-3.0.0.dev0/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.3.0.dev5/src/taipy.egg-info/PKG-INFO` & `taipy-3.0.0.dev0/src/taipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.3.0.dev5
+Version: 3.0.0.dev0
 Summary: A 360° open-source platform from Python pilots to production-ready web apps.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.3.0.dev5/src/taipy.egg-info/SOURCES.txt` & `taipy-3.0.0.dev0/src/taipy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 src/taipy.egg-info/requires.txt
 src/taipy.egg-info/top_level.txt
 src/taipy/_cli/__init__.py
 src/taipy/_cli/_help_cli.py
 src/taipy/_cli/_scaffold_cli.py
 src/taipy/gui_core/GuiCoreLib.py
 src/taipy/gui_core/__init__.py
+src/taipy/gui_core/_init.py
 src/taipy/gui_core/lib/taipy-gui-core.js
 tests/test_run.py
```

### Comparing `taipy-2.3.0.dev5/tests/test_run.py` & `taipy-3.0.0.dev0/tests/test_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,7 +49,15 @@
 @mock.patch("taipy.rest.Rest.run")
 @mock.patch("taipy.core.Core.run")
 def test_run_pass_with_gui_and_rest(core_run, rest_run, gui_run):
     _run(Gui(), Rest())
     gui_run.assert_called_once()
     core_run.assert_called_once()
     rest_run.assert_not_called()
+
+
+@mock.patch("taipy.gui.Gui.run")
+@mock.patch("taipy.core.Core.run")
+def test_run_pass_with_gui_and_core(core_run, gui_run):
+    _run(Gui(), Core())
+    gui_run.assert_called_once()
+    core_run.assert_called_once()
```

