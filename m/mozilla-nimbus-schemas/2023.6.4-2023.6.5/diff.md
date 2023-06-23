# Comparing `tmp/mozilla_nimbus_schemas-2023.6.4.tar.gz` & `tmp/mozilla_nimbus_schemas-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_schemas-2023.6.4.tar", max compression
+gzip compressed data, was "mozilla_nimbus_schemas-2023.6.5.tar", max compression
```

## Comparing `mozilla_nimbus_schemas-2023.6.4.tar` & `mozilla_nimbus_schemas-2023.6.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    16725 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/LICENSE
--rw-r--r--   0        0        0      839 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/README.md
--rw-r--r--   0        0        0        0 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/__init__.py
--rw-r--r--   0        0        0      365 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/__init__.py
--rw-r--r--   0        0        0      624 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/analysis_errors.py
--rw-r--r--   0        0        0     1386 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/metadata.py
--rw-r--r--   0        0        0      648 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/statistics.py
--rw-r--r--   0        0        0     4646 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py
--rw-r--r--   0        0        0     2266 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py
--rw-r--r--   0        0        0     2521 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py
--rw-r--r--   0        0        0      956 2023-06-16 16:23:03.243354 mozilla_nimbus_schemas-2023.6.4/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.6.4/setup.py
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.6.4/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/LICENSE
+-rw-r--r--   0        0        0      839 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/__init__.py
+-rw-r--r--   0        0        0      365 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/__init__.py
+-rw-r--r--   0        0        0      624 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/analysis_errors.py
+-rw-r--r--   0        0        0     1591 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/metadata.py
+-rw-r--r--   0        0        0      753 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/statistics.py
+-rw-r--r--   0        0        0     4646 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py
+-rw-r--r--   0        0        0     2266 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py
+-rw-r--r--   0        0        0     2521 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py
+-rw-r--r--   0        0        0     1043 2023-06-23 13:07:51.801154 mozilla_nimbus_schemas-2023.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.6.5/setup.py
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 mozilla_nimbus_schemas-2023.6.5/PKG-INFO
```

### Comparing `mozilla_nimbus_schemas-2023.6.4/LICENSE` & `mozilla_nimbus_schemas-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/README.md` & `mozilla_nimbus_schemas-2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/analysis_errors.py` & `mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/analysis_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/jetstream/metadata.py` & `mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/jetstream/metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime as dt
 import json
 from typing import Optional
 
-from pydantic import BaseModel, HttpUrl
+from pydantic import BaseModel, HttpUrl, validator
 
-from mozilla_nimbus_schemas.jetstream.statistics import AnalysisBasis
+from mozilla_nimbus_schemas.jetstream.statistics import SCHEMA_VERSION, AnalysisBasis
 
 
 def nonstrict_json_loads(*args, **kwargs):
     kwargs.update({"strict": False})
     return json.loads(*args, **kwargs)
 
 
@@ -20,15 +20,15 @@
 
     class Config:
         # override json_loads because `description` field may contain \n
         json_loads = nonstrict_json_loads
 
 
 class Outcome(BaseModel):
-    commit_hash: str
+    commit_hash: Optional[str]
     default_metrics: list[str]
     description: str
     friendly_name: str
     metrics: list[str]
     slug: str
 
 
@@ -42,12 +42,18 @@
 
 
 class Metadata(BaseModel):
     analysis_start_time: Optional[dt.datetime] = None
     external_config: Optional[ExternalConfig] = None
     metrics: dict[str, Metric]
     outcomes: dict[str, Outcome] = {}
-    schema_version: int
+    schema_version: int = SCHEMA_VERSION
+
+    @validator("analysis_start_time", pre=True)
+    def treat_empty_str_as_none(cls, v):
+        if v == "":
+            return None
+        return v
 
     class Config:
         # override json_loads because `description` field in Metric may contain \n
         json_loads = nonstrict_json_loads
```

### Comparing `mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py` & `mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_analysis_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py` & `mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py` & `mozilla_nimbus_schemas-2023.6.5/mozilla_nimbus_schemas/tests/jetstream/test_statistics.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_schemas-2023.6.4/pyproject.toml` & `mozilla_nimbus_schemas-2023.6.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozilla-nimbus-schemas"
-version = "2023.6.4"
+version = "2023.6.5"
 description = "Schemas used by Mozilla Nimbus and related projects."
 authors = ["mikewilli"]
 license = "MPL 2.0"
 readme = "README.md"
 packages = [{include = "mozilla_nimbus_schemas"}]
 
 [tool.poetry.dependencies]
@@ -40,12 +40,14 @@
     "N812",
     "N815",
     "RET503",
     "RET504",
     "RET505",
     "SIM102",
 ]
+[tool.ruff.pep8-naming]
+classmethod-decorators = ["classmethod", "pydantic.validator"]
 
 [tool.flake8]
 max-line-length = 90
 [tool.black]
 line-length = 90
```

### Comparing `mozilla_nimbus_schemas-2023.6.4/setup.py` & `mozilla_nimbus_schemas-2023.6.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'mozilla-nimbus-schemas',
-    'version': '2023.6.4',
+    'version': '2023.6.5',
     'description': 'Schemas used by Mozilla Nimbus and related projects.',
     'long_description': '# Nimbus Schemas\n\nThis directory contains a published package of schemas used by different parts of the Mozilla Nimbus experimentation ecosystem.\n\n## Versioning\n`mozilla-nimbus-schemas` uses a date-based versioning scheme. The format is `yyyy.m.#`, where `m` is the non-zero-padded month, and `#` is an incrementing number starting from 1 for each month. For example, the second release in June of 2023 would have a version of `2023.6.2`.\n\n## Installation/Usage\n### Prerequisites\n- python ^3.10\n- poetry ^1.2.2\n\nFrom project root (i.e., parent to this directory)\n- Install: `make schemas_install`\n- Run linting and tests: `make schemas_check`\n- Code formatting: `make schemas_code_format`\n\n## Schemas\n### Jetstream\n\nContains schemas describing analysis results, metadata, and errors from [Jetstream](https://github.com/mozilla/jetstream).\n',
     'author': 'mikewilli',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mozilla_nimbus_schemas-2023.6.4/PKG-INFO` & `mozilla_nimbus_schemas-2023.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-nimbus-schemas
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: Schemas used by Mozilla Nimbus and related projects.
 License: MPL 2.0
 Author: mikewilli
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

