# Comparing `tmp/sekoia_automation_sdk-1.3.4.tar.gz` & `tmp/sekoia_automation_sdk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.4.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.5.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.4.tar` & `sekoia_automation_sdk-1.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/LICENSE
--rw-r--r--   0        0        0     8422 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/README.md
--rw-r--r--   0        0        0     2114 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/action.py
--rw-r--r--   0        0        0     5193 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/config.py
--rw-r--r--   0        0        0     6955 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      596 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    13709 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     6094 2023-06-21 10:42:11.172765 sekoia_automation_sdk-1.3.4/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14267 2023-06-21 10:42:11.176765 sekoia_automation_sdk-1.3.4/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-06-21 10:42:11.176765 sekoia_automation_sdk-1.3.4/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-23 16:44:27.531147 sekoia_automation_sdk-1.3.5/LICENSE
+-rw-r--r--   0        0        0     8422 2023-06-23 16:44:27.531147 sekoia_automation_sdk-1.3.5/README.md
+-rw-r--r--   0        0        0     2114 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/action.py
+-rw-r--r--   0        0        0     5193 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6955 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      596 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    13709 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     6094 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14583 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.5/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.4/LICENSE` & `sekoia_automation_sdk-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/README.md` & `sekoia_automation_sdk-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/pyproject.toml` & `sekoia_automation_sdk-1.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.4"
+version = "1.3.5"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/cli.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/sync_library.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,21 @@
             self._handle_trigger_exception(ex)
 
     def execute(self) -> None:
         self._ensure_data_path_set()
         # Always restart the trigger, except if the error seems to be unrecoverable
         self._secrets = self._get_secrets_from_server()
         while not self._stop_event.is_set():
-            self._execute_once()
+            try:
+                self._execute_once()
+            except Exception:  # pragma: no cover
+                # Exception are handled in `_execute_once` but in case
+                # an error occurred while handling an error we catch everything
+                # i.e. An error occurred while sending logs to Sekoia.io
+                pass
 
     def _rm_tree(self, path: Path):
         """Delete a directory and its children.
 
         :param Path path: The directory to delete
         """
         # iter over children
```

### Comparing `sekoia_automation_sdk-1.3.4/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.5/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.4/PKG-INFO` & `sekoia_automation_sdk-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

