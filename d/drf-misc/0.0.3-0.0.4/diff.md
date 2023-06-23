# Comparing `tmp/drf_misc-0.0.3.tar.gz` & `tmp/drf_misc-0.0.4.tar.gz`

## Comparing `drf_misc-0.0.3.tar` & `drf_misc-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.isort.cfg
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.0.3/ignore-spelling-words.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.0.3/mypy.ini
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.3/setup.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/admin.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/apps.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/settings.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/api_exceptions.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/api_views.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/audit_service.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/cache.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/filter_backend.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/middlewares.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/models.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/paginations.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/parsers.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/permissions.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/serializers.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/services.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/core/throttling.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/utility/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/utility/decorators.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/utility/epoch_util.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/utility/misc.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.0.3/drf_misc/utility/validator.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.0.3/LICENSE
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 drf_misc-0.0.3/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 drf_misc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 drf_misc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.0.4/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.0.4/mypy.ini
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.4/setup.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/admin.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/apps.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/settings.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/api_exceptions.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/api_views.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/audit_service.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/cache.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/filter_backend.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/middlewares.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/models.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/paginations.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/parsers.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/permissions.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/serializers.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/services.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/core/throttling.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/decorators.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/epoch_util.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/misc.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.0.4/drf_misc/utility/validator.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.0.4/README.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 drf_misc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.0.4/PKG-INFO
```

### Comparing `drf_misc-0.0.3/.pre-commit-config.yaml` & `drf_misc-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/.pylintrc` & `drf_misc-0.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/.github/workflows/publish.yaml` & `drf_misc-0.0.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/admin.py` & `drf_misc-0.0.4/drf_misc/admin.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/settings.py` & `drf_misc-0.0.4/drf_misc/settings.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/api_exceptions.py` & `drf_misc-0.0.4/drf_misc/core/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/api_views.py` & `drf_misc-0.0.4/drf_misc/core/api_views.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/audit_service.py` & `drf_misc-0.0.4/drf_misc/core/audit_service.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/filter_backend.py` & `drf_misc-0.0.4/drf_misc/core/filter_backend.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/middlewares.py` & `drf_misc-0.0.4/drf_misc/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/models.py` & `drf_misc-0.0.4/drf_misc/core/models.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/paginations.py` & `drf_misc-0.0.4/drf_misc/core/paginations.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/serializers.py` & `drf_misc-0.0.4/drf_misc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/services.py` & `drf_misc-0.0.4/drf_misc/core/services.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/core/throttling.py` & `drf_misc-0.0.4/drf_misc/core/throttling.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/utility/epoch_util.py` & `drf_misc-0.0.4/drf_misc/utility/epoch_util.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/utility/misc.py` & `drf_misc-0.0.4/drf_misc/utility/misc.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/drf_misc/utility/validator.py` & `drf_misc-0.0.4/drf_misc/utility/validator.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/.gitignore` & `drf_misc-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/LICENSE` & `drf_misc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.3/pyproject.toml` & `drf_misc-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "drf-misc"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

