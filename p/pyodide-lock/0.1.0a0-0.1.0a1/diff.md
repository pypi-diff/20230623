# Comparing `tmp/pyodide_lock-0.1.0a0.tar.gz` & `tmp/pyodide_lock-0.1.0a1.tar.gz`

## Comparing `pyodide_lock-0.1.0a0.tar` & `pyodide_lock-0.1.0a1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/.codecov.yml
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/.github/workflows/main.yml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/pyodide_lock/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/pyodide_lock/py.typed
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/pyodide_lock/spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/tests/test_spec.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/tests/data/pyodide-lock-0.22.1.json.gz
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/tests/data/pyodide-lock-0.23.3.json.gz
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/.gitignore
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/README.md
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/.codecov.yml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/pyodide_lock/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/pyodide_lock/py.typed
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/pyodide_lock/spec.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/pyodide_lock/utils.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/tests/test_spec.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/tests/data/pyodide-lock-0.22.1.json.gz
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/tests/data/pyodide-lock-0.23.3.json.gz
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a1/PKG-INFO
```

### Comparing `pyodide_lock-0.1.0a0/.pre-commit-config.yaml` & `pyodide_lock-0.1.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/.github/workflows/main.yml` & `pyodide_lock-0.1.0a1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/pyodide_lock/spec.py` & `pyodide_lock-0.1.0a1/pyodide_lock/spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 import json
 from pathlib import Path
 from typing import Literal
 
 from pydantic import BaseModel, Extra
 
+from .utils import _generate_package_hash
+
 
 class InfoSpec(BaseModel):
-    arch: str
+    arch: Literal["wasm32", "wasm64"] = "wasm32"
     platform: str
     version: str
     python: str
 
     class Config:
         extra = Extra.forbid
 
 
 class PackageSpec(BaseModel):
     name: str
     version: str
     file_name: str
     install_dir: str
-    sha256: str
+    sha256: str = ""
     package_type: Literal[
         "package", "cpython_module", "shared_library", "static_library"
     ] = "package"
-    imports: list[str]
-    depends: list[str]
+    imports: list[str] = []
+    depends: list[str] = []
     unvendored_tests: bool = False
     # This field is deprecated
     shared_library: bool = False
 
     class Config:
         extra = Extra.forbid
 
+    def update_sha256(self, path: Path) -> "PackageSpec":
+        """Update the sha256 hash for a package."""
+        self.sha256 = _generate_package_hash(path)
+        return self
+
 
 class PyodideLockSpec(BaseModel):
     """A specification for the pyodide-lock.json file."""
 
     info: InfoSpec
     packages: dict[str, PackageSpec]
 
     class Config:
         extra = Extra.forbid
 
     @classmethod
-    def from_json(cls, json_path: Path):
+    def from_json(cls, path: Path) -> "PyodideLockSpec":
         """Read the lock spec from a json file."""
-        with json_path.open("r") as fh:
+        with path.open("r") as fh:
             data = json.load(fh)
         return cls(**data)
 
-    def to_json(self, json_path: Path, indent: int = 0):
+    def to_json(self, path: Path, indent: int = 0) -> None:
         """Write the lock spec to a json file."""
-        with json_path.open("w") as fh:
+        with path.open("w") as fh:
             json.dump(self.dict(), fh, indent=indent)
```

### Comparing `pyodide_lock-0.1.0a0/tests/test_spec.py` & `pyodide_lock-0.1.0a1/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/tests/data/pyodide-lock-0.22.1.json.gz` & `pyodide_lock-0.1.0a1/tests/data/pyodide-lock-0.22.1.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/tests/data/pyodide-lock-0.23.3.json.gz` & `pyodide_lock-0.1.0a1/tests/data/pyodide-lock-0.23.3.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/LICENSE` & `pyodide_lock-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/README.md` & `pyodide_lock-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a0/pyproject.toml` & `pyodide_lock-0.1.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -52,7 +52,11 @@
   "F",      # pyflakes
   "I",      # isort
   "PGH",    # pygrep-hooks
   "PLC",    # pylint conventions
   "PLE",    # pylint errors
   "UP",     # pyupgrade
 ]
+
+[tool.pytest.ini_options]
+addopts = '''
+--doctest-modules'''
```

### Comparing `pyodide_lock-0.1.0a0/PKG-INFO` & `pyodide_lock-0.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-lock
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Tooling to manage the `pyodide-lock.json` file
 Project-URL: Homepage, https://github.com/pyodide-lock/pyodide-lock
 Project-URL: Bug Tracker, https://github.com/pyodide-lock/pyodide-lock/issues
 Author: Pyodide developers
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

