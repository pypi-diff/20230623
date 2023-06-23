# Comparing `tmp/cchdo.params-0.1.8.tar.gz` & `tmp/cchdo.params-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpp9rb2xv5/tmpxgr9jn7d/cchdo.params-0.1.8.tar", last modified: Wed Jan  6 17:35:42 2021, max compression
+gzip compressed data, was "/tmp/tmpb_rd1nny/tmpmifnipwz/cchdo.params-0.1.9.tar", last modified: Wed Jan 27 21:28:01 2021, max compression
```

## Comparing `cchdo.params-0.1.8.tar` & `cchdo.params-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.651533 cchdo.params-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.639532 cchdo.params-0.1.8/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (116)     1118 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     1718 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.639532 cchdo.params-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.639532 cchdo.params-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.github/workflows/do-release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2215 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      482 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.639532 cchdo.params-0.1.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (116)     1499 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2394 2021-01-06 17:35:42.651533 cchdo.params-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      238 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.639532 cchdo.params-0.1.8/cchdo/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.651533 cchdo.params-0.1.8/cchdo/params/
--rw-r--r--   0 runner    (1001) docker     (116)     9270 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3941 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo/params/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     5272 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     2710 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/parameters.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)  4055040 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/params.sqlite3
--rw-r--r--   0 runner    (1001) docker     (116)  3389510 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/params.sqlite3.sql
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.651533 cchdo.params-0.1.8/cchdo/params/test/
--rw-r--r--   0 runner    (1001) docker     (116)     3745 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/cchdo/params/test/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-06 17:35:42.643532 cchdo.params-0.1.8/cchdo.params.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2394 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      767 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      491 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-01-06 17:35:42.000000 cchdo.params-0.1.8/cchdo.params.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      232 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2021-01-06 17:35:42.651533 cchdo.params-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-06 17:35:29.000000 cchdo.params-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.936022 cchdo.params-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.924022 cchdo.params-0.1.9/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (116)     1118 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)     1718 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.924022 cchdo.params-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.924022 cchdo.params-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.github/workflows/do-release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1392 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2215 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      482 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.924022 cchdo.params-0.1.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (116)       45 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1499 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2394 2021-01-27 21:28:01.936022 cchdo.params-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      238 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.924022 cchdo.params-0.1.9/cchdo/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.936022 cchdo.params-0.1.9/cchdo/params/
+-rw-r--r--   0 runner    (1001) docker     (116)    10195 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3941 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo/params/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5340 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2710 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/parameters.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)  4055040 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/params.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (116)  3389510 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/params.sqlite3.sql
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.936022 cchdo.params-0.1.9/cchdo/params/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     3745 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)      884 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/cchdo/params/test/test_ordering.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-27 21:28:01.928022 cchdo.params-0.1.9/cchdo.params.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2394 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      802 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      489 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2021-01-27 21:28:01.000000 cchdo.params-0.1.9/cchdo.params.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      232 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1119 2021-01-27 21:28:01.936022 cchdo.params-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-27 21:27:46.000000 cchdo.params-0.1.9/setup.py
```

### Comparing `cchdo.params-0.1.8/.devcontainer/Dockerfile` & `cchdo.params-0.1.9/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/.devcontainer/devcontainer.json` & `cchdo.params-0.1.9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/.github/workflows/do-release.yml` & `cchdo.params-0.1.9/.github/workflows/do-release.yml`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/.github/workflows/python-app.yml` & `cchdo.params-0.1.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/.gitignore` & `cchdo.params-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/LICENSE.md` & `cchdo.params-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/PKG-INFO` & `cchdo.params-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cchdo.params
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/cchdo
 Author: CCHDO
 Author-email: cchdo@ucsd.edu
 License: BSD 3-clause
 Description: cchdo.params
         ============
```

### Comparing `cchdo.params-0.1.8/cchdo/params/__init__.py` & `cchdo.params-0.1.9/cchdo/params/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from collections import namedtuple
 from dataclasses import dataclass, field
 from importlib.resources import path, read_text
-from typing import Optional, Callable, Union
+from typing import cast, Optional, Callable, Union, Tuple
 from collections.abc import Mapping, MutableMapping
 from functools import cached_property
 from json import loads
 from contextlib import contextmanager
 
 __all__ = ["CFStandardNames", "WHPNames"]
 
@@ -100,17 +101,19 @@
 
 
 @dataclass(frozen=True)
 class WHPName:
     """Wrapper for WHP parameters.json"""
 
     whp_name: str
+    nc_name: str = field(repr=False)
+    rank: float = field(repr=False)  # used for sorting in the "classic" WHP order
     data_type: Callable[[str], Union[str, float, int]] = field(repr=False)
+
     whp_unit: Optional[str] = None
-    nc_name: Optional[str] = None
     flag_w: Optional[str] = field(default=None, repr=False)
     cf_name: Optional[str] = None
     numeric_min: Optional[float] = field(default=None, repr=False)
     numeric_max: Optional[float] = field(default=None, repr=False)
     numeric_precision: Optional[int] = field(default=None, repr=False)
     field_width: Optional[int] = field(default=None, repr=False)
     description: Optional[str] = field(default=None, repr=False)
@@ -129,14 +132,22 @@
         """This is the thing that uniquely identifies"""
         return (self.whp_name, self.whp_unit)
 
     @property
     def cf(self):
         return CFStandardNames.get(self.cf_name)
 
+    def __eq__(self, other):
+        return (self.whp_name == other.whp_name) and (self.whp_unit == other.whp_unit)
+
+    def __lt__(self, other):
+        if self.rank == other.rank:
+            return str(self.whp_unit) < str(other.whp_unit)
+        return self.rank < other.rank
+
     def get_nc_attrs(self, error=False):
         attrs = {
             "whp_name": self.whp_name,
         }
 
         if error is True and self.error_name is not None:
             attrs["whp_name"] = self.error_name
@@ -231,14 +242,28 @@
     def error_cols(self):
         return {
             ex.error_name: ex
             for ex in self._cached_dict.values()
             if ex.error_name is not None
         }
 
+    def _scope_filter(self, scope: str = "cruise") -> Tuple[WHPName, ...]:
+        return tuple(
+            sorted(cast(WHPName, name) for name in self.values() if name.scope == scope)
+        )
+
+    @cached_property
+    def groups(self):
+        WHPNameGroups = namedtuple("WHPNameGroups", "cruise, profile, sample")
+        return WHPNameGroups(
+            cruise=self._scope_filter("cruise"),
+            profile=self._scope_filter("profile"),
+            sample=self._scope_filter("sample"),
+        )
+
     @cached_property
     def legacy_json_schema(self):
         return loads(read_text("cchdo.params", "parameters.schema.json"))
 
     @cached_property
     def legacy_json(self):
         with database() as session:
```

### Comparing `cchdo.params-0.1.8/cchdo/params/__main__.py` & `cchdo.params-0.1.9/cchdo/params/__main__.py`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/cchdo/params/models.py` & `cchdo.params-0.1.9/cchdo/params/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     description = Column(Text, nullable=True)
     note = Column(Text, nullable=True)
     warning = Column(Text, nullable=True)
 
     scope = Column(
         Enum("cruise", "profile", "sample"), nullable=False, server_default="sample"
     )
-    dtype = Column(Enum("decimal", "integer", "string"), nullable=False,)
+    dtype = Column(
+        Enum("decimal", "integer", "string"),
+        nullable=False,
+    )
     flag = Column(
         Enum("woce_bottle", "woce_ctd", "woce_discrete", "no_flags"), nullable=False
     )
     ancillary = Column(Boolean, nullable=False, server_default="0")
 
     rank = Column(Float, nullable=False)
 
@@ -154,22 +157,24 @@
             error_name=self.error_name,
             cf_unit=self.cf_unit,
             reference_scale=reference_scale,
             whp_number=self.param.whp_number,
             scope=self.param.scope,
             analytical_temperature_name=self.analytical_temperature_name,
             analytical_temperature_units=self.analytical_temperature_units,
+            rank=self.param.rank,
         )
 
 
 class Alias(Base):
     __tablename__ = "whp_alias"
     old_name = Column(String, primary_key=True)
     old_unit = Column(String, primary_key=True, nullable=True)
     whp_name = Column(String)
     whp_unit = Column(String)
 
     __table_args__ = (
         ForeignKeyConstraint(
-            ["whp_name", "whp_unit"], ["whp_names.whp_name", "whp_names.whp_unit"],
+            ["whp_name", "whp_unit"],
+            ["whp_names.whp_name", "whp_names.whp_unit"],
         ),
     )
```

### Comparing `cchdo.params-0.1.8/cchdo/params/parameters.schema.json` & `cchdo.params-0.1.9/cchdo/params/parameters.schema.json`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/cchdo/params/params.sqlite3` & `cchdo.params-0.1.9/cchdo/params/params.sqlite3`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/cchdo/params/params.sqlite3.sql` & `cchdo.params-0.1.9/cchdo/params/params.sqlite3.sql`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/cchdo/params/test/test_data.py` & `cchdo.params-0.1.9/cchdo/params/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cchdo.params-0.1.8/cchdo.params.egg-info/PKG-INFO` & `cchdo.params-0.1.9/cchdo.params.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cchdo.params
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/cchdo
 Author: CCHDO
 Author-email: cchdo@ucsd.edu
 License: BSD 3-clause
 Description: cchdo.params
         ============
```

### Comparing `cchdo.params-0.1.8/cchdo.params.egg-info/SOURCES.txt` & `cchdo.params-0.1.9/cchdo.params.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 cchdo/params/__main__.py
 cchdo/params/_version.py
 cchdo/params/models.py
 cchdo/params/parameters.schema.json
 cchdo/params/params.sqlite3
 cchdo/params/params.sqlite3.sql
 cchdo/params/py.typed
-cchdo/params/test/test_data.py
+cchdo/params/test/test_data.py
+cchdo/params/test/test_ordering.py
```

### Comparing `cchdo.params-0.1.8/setup.cfg` & `cchdo.params-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 	pytest==5.4.1
 	jsonschema==3.2.0
 dev = 
 	%(selftest)s
 	click==7.1.2
 	pytest-cov==2.10.1
 	pre-commit==2.9.3
-	black==19.10b0
+	black==20.8b1
 	codecov==2.1.11
-	mypy==0.790
+	mypy==0.800
 	flake8==3.8.4
 	pyflakes==2.2.0
 	twine==3.3.0
 	sqlalchemy-stubs>=0.2
 docs = 
 	Sphinx
 	furo
@@ -59,14 +59,17 @@
 
 [mypy]
 plugins = sqlmypy
 
 [mypy-pytest.*]
 ignore_missing_imports = True
 
+[mypy-jsonschema.*]
+ignore_missing_imports = True
+
 [mypy-setup]
 ignore_errors = True
 
 [mypy-docs.conf]
 ignore_errors = True
 
 [egg_info]
```

