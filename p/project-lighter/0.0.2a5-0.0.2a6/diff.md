# Comparing `tmp/project_lighter-0.0.2a5.tar.gz` & `tmp/project_lighter-0.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a5.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a6.tar", max compression
```

## Comparing `project_lighter-0.0.2a5.tar` & `project_lighter-0.0.2a6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-06-12 22:30:54.732785 project_lighter-0.0.2a5/LICENSE
--rw-r--r--   0        0        0     2164 2023-06-12 22:30:54.732785 project_lighter-0.0.2a5/README.md
--rw-r--r--   0        0        0       67 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    14196 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     6508 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    19796 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/system.py
--rw-r--r--   0        0        0       36 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/__init__.py
--rw-r--r--   0        0        0      627 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/cli.py
--rw-r--r--   0        0        0     2566 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/collate.py
--rw-r--r--   0        0        0     1547 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3431 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2278 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/misc.py
--rw-r--r--   0        0        0     5881 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/model.py
--rw-r--r--   0        0        0     2483 2023-06-12 22:30:54.736785 project_lighter-0.0.2a5/lighter/utils/runner.py
--rw-r--r--   0        0        0       24 2023-06-12 22:31:23.504970 project_lighter-0.0.2a5/lighter/version.py
--rw-r--r--   0        0        0     4399 2023-06-12 22:31:23.436969 project_lighter-0.0.2a5/pyproject.toml
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 project_lighter-0.0.2a5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/LICENSE
+-rw-r--r--   0        0        0     2164 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/README.md
+-rw-r--r--   0        0        0       67 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    14204 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    19796 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3866 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2278 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5881 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-06-23 16:46:22.909276 project_lighter-0.0.2a6/lighter/version.py
+-rw-r--r--   0        0        0     4420 2023-06-23 16:46:22.837276 project_lighter-0.0.2a6/pyproject.toml
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 project_lighter-0.0.2a6/PKG-INFO
```

### Comparing `project_lighter-0.0.2a5/LICENSE` & `project_lighter-0.0.2a6/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/README.md` & `project_lighter-0.0.2a6/README.md`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/callbacks/logger.py` & `project_lighter-0.0.2a6/lighter/callbacks/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,20 +302,20 @@
         self.loss["val"] = 0
         self.epoch_step_counter["val"] = 0
 
     def on_train_batch_end(self, trainer: Trainer, pl_module: LighterSystem, outputs: Any, batch: Any, batch_idx: int) -> None:
         self._on_batch_end(outputs, trainer)
 
     def on_validation_batch_end(
-        self, trainer: Trainer, pl_module: LighterSystem, outputs: Any, batch: Any, batch_idx: int, dataloader_idx: int
+        self, trainer: Trainer, pl_module: LighterSystem, outputs: Any, batch: Any, batch_idx: int, dataloader_idx: int = 0
     ) -> None:
         self._on_batch_end(outputs, trainer)
 
     def on_test_batch_end(
-        self, trainer: Trainer, pl_module: LighterSystem, outputs: Any, batch: Any, batch_idx: int, dataloader_idx: int
+        self, trainer: Trainer, pl_module: LighterSystem, outputs: Any, batch: Any, batch_idx: int, dataloader_idx: int = 0
     ) -> None:
         self._on_batch_end(outputs, trainer)
 
     def on_train_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         self._on_epoch_end(trainer, pl_module)
 
     def on_validation_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
```

### Comparing `project_lighter-0.0.2a5/lighter/callbacks/utils.py` & `project_lighter-0.0.2a6/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a6/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a6/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a6/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/system.py` & `project_lighter-0.0.2a6/lighter/system.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/cli.py` & `project_lighter-0.0.2a6/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/collate.py` & `project_lighter-0.0.2a6/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a6/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/misc.py` & `project_lighter-0.0.2a6/lighter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/model.py` & `project_lighter-0.0.2a6/lighter/utils/model.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/lighter/utils/runner.py` & `project_lighter-0.0.2a6/lighter/utils/runner.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a5/pyproject.toml` & `project_lighter-0.0.2a6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a5"
+version = "0.0.2a6"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
@@ -49,14 +49,15 @@
 fire = "^0.5.0"
 loguru = "^0.6.0"
 lightly = "^1.2.43"
 torchmetrics = "^0.11.0"
 py = "^1.11.0"
 tensorboard = "^2.11.2"
 monai-weekly = "^1.2.dev2305"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 black = {version = "^23.1a1", allow-prereleases = true}
 isort = {extras = ["colors"], version = "^5.11.4"}
 mypy = "^0.991"
 mypy-extensions = "^0.4.3"
```

### Comparing `project_lighter-0.0.2a5/PKG-INFO` & `project_lighter-0.0.2a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,15 @@
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: lightly (>=1.2.43,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: monai-weekly (>=1.2.dev2305,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: py (>=1.11.0,<2.0.0)
 Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
 Requires-Dist: torch (>=2.0,<3.0)
 Requires-Dist: torchmetrics (>=0.11.0,<0.12.0)
 Requires-Dist: torchvision (>=0.15,<0.16)
 Project-URL: Repository, https://github.com/lighter/lighter
 Description-Content-Type: text/markdown
```

