# Comparing `tmp/dvc-gdrive-2.19.2.tar.gz` & `tmp/dvc-gdrive-2.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-gdrive-2.19.2.tar", last modified: Sun Apr  9 23:34:16 2023, max compression
+gzip compressed data, was "dvc-gdrive-2.20.0.tar", last modified: Fri Jun 23 03:25:30 2023, max compression
```

## Comparing `dvc-gdrive-2.19.2.tar` & `dvc-gdrive-2.20.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.069212 dvc-gdrive-2.19.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.073212 dvc-gdrive-2.19.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.073212 dvc-gdrive-2.19.2/dvc_gdrive/
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive/_dvc_gdrive_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/dvc_gdrive/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/test_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.094224 dvc-gdrive-2.20.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.082224 dvc-gdrive-2.20.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.090224 dvc-gdrive-2.20.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-23 03:25:30.094224 dvc-gdrive-2.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.090224 dvc-gdrive-2.20.0/dvc_gdrive/
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive/_dvc_gdrive_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.090224 dvc-gdrive-2.20.0/dvc_gdrive/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/dvc_gdrive/tests/test_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 03:25:30.090224 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-23 03:25:30.000000 dvc-gdrive-2.20.0/dvc_gdrive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-23 03:25:30.094224 dvc-gdrive-2.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-23 03:25:09.000000 dvc-gdrive-2.20.0/setup.py
```

### Comparing `dvc-gdrive-2.19.2/.github/workflows/release.yaml` & `dvc-gdrive-2.20.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/.github/workflows/tests.yaml` & `dvc-gdrive-2.20.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/.github/workflows/update-template.yaml` & `dvc-gdrive-2.20.0/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/.gitignore` & `dvc-gdrive-2.20.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/.pre-commit-config.yaml` & `dvc-gdrive-2.20.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -38,19 +38,14 @@
     hooks:
     - id: mypy
       name: mypy
       entry: mypy
       files: ^dvc_gdrive/
       language: system
       types: [python]
-    - id: pylint
-      name: pylint
-      entry: pylint
-      language: system
-      types: [python]
   - hooks:
       - args:
           - -i
           - "2"
         id: beautysh
         language_version: python3
     repo: https://github.com/lovesegfault/beautysh
```

### Comparing `dvc-gdrive-2.19.2/LICENSE` & `dvc-gdrive-2.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/PKG-INFO` & `dvc-gdrive-2.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-gdrive
-Version: 2.19.2
+Version: 2.20.0
 Summary: gdrive plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gdrive
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gdrive
 Keywords: dvc,gdrive
```

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive/__init__.py` & `dvc-gdrive-2.20.0/dvc_gdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive/tests/cloud.py` & `dvc-gdrive-2.20.0/dvc_gdrive/tests/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive/tests/test_dvc.py` & `dvc-gdrive-2.20.0/dvc_gdrive/tests/test_dvc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 from dvc.testing.api_tests import (  # noqa, pylint: disable=unused-import
     TestAPI,
 )
 from dvc.testing.remote_tests import (  # noqa, pylint: disable=unused-import
     TestRemote,
 )
-from dvc.testing.workspace_tests import TestAdd as _TestAdd
 from dvc.testing.workspace_tests import TestGetUrl as _TestGetUrl
 from dvc.testing.workspace_tests import TestImport as _TestImport
 from dvc.testing.workspace_tests import TestLsUrl as _TestLsUrl
 
 
 @pytest.fixture
 def cloud(make_cloud):
@@ -28,19 +27,14 @@
 
 @pytest.mark.xfail
 class TestImport(_TestImport):
     pass
 
 
 @pytest.mark.xfail
-class TestAdd(_TestAdd):
-    pass
-
-
-@pytest.mark.xfail
 class TestLsUrl(_TestLsUrl):
     pass
 
 
 @pytest.mark.xfail
 class TestGetUrl(_TestGetUrl):
     pass
```

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive/tests/test_fs.py` & `dvc-gdrive-2.20.0/dvc_gdrive/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive.egg-info/PKG-INFO` & `dvc-gdrive-2.20.0/dvc_gdrive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-gdrive
-Version: 2.19.2
+Version: 2.20.0
 Summary: gdrive plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gdrive
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gdrive
 Keywords: dvc,gdrive
```

### Comparing `dvc-gdrive-2.19.2/dvc_gdrive.egg-info/SOURCES.txt` & `dvc-gdrive-2.20.0/dvc_gdrive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/pyproject.toml` & `dvc-gdrive-2.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.2/setup.cfg` & `dvc-gdrive-2.20.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 	setuptools_scm[toml]>=6.3.1
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
 	dvc
-	pydrive2[fsspec]>=1.15.3
+	pydrive2[fsspec]>=1.16
 
 [options.extras_require]
 tests = 
 	wheel==0.37.0
 	dvc[testing]
 	pytest==6.2.5
 	pytest-cov==3.0.0
```

