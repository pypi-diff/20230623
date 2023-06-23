# Comparing `tmp/autogluon.features-0.8.1b20230622.tar.gz` & `tmp/autogluon.features-0.8.1b20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.features-0.8.1b20230622.tar", last modified: Thu Jun 22 09:03:55 2023, max compression
+gzip compressed data, was "autogluon.features-0.8.1b20230623.tar", last modified: Fri Jun 23 09:04:22 2023, max compression
```

## Comparing `autogluon.features-0.8.1b20230622.tar` & `autogluon.features-0.8.1b20230623.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.511786 autogluon.features-0.8.1b20230622/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-22 09:03:55.511786 autogluon.features-0.8.1b20230622/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:03:55.511786 autogluon.features-0.8.1b20230622/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.507786 autogluon.features-0.8.1b20230622/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.507786 autogluon.features-0.8.1b20230622/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.507786 autogluon.features-0.8.1b20230622/src/autogluon/features/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.511786 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/auto_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/drop_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/drop_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/fillna.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/isnan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/memory_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/text_ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/generators/text_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 09:03:32.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon/features/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:55.507786 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:55.000000 autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.525389 autogluon.features-0.8.1b20230623/
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-23 09:04:22.525389 autogluon.features-0.8.1b20230623/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:04:22.525389 autogluon.features-0.8.1b20230623/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.521389 autogluon.features-0.8.1b20230623/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.521389 autogluon.features-0.8.1b20230623/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.525389 autogluon.features-0.8.1b20230623/src/autogluon/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.525389 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44204 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/auto_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/drop_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/drop_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/fillna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/isnan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/memory_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/text_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/generators/text_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-23 09:04:00.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon/features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:22.521389 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:22.000000 autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/zip-safe
```

### Comparing `autogluon.features-0.8.1b20230622/PKG-INFO` & `autogluon.features-0.8.1b20230623/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.1b20230622
+Version: 0.8.1b20230623
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.8.1b20230622/setup.py` & `autogluon.features-0.8.1b20230623/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 #!/usr/bin/env python
 ###########################
 # This code block is a HACK (!), but is necessary to avoid code duplication. Do NOT alter these lines.
+import importlib.util
 import os
+
 from setuptools import setup
-import importlib.util
+
 filepath = os.path.abspath(os.path.dirname(__file__))
-filepath_import = os.path.join(filepath, '..', 'core', 'src', 'autogluon', 'core', '_setup_utils.py')
+filepath_import = os.path.join(filepath, "..", "core", "src", "autogluon", "core", "_setup_utils.py")
 spec = importlib.util.spec_from_file_location("ag_min_dependencies", filepath_import)
 ag = importlib.util.module_from_spec(spec)
 # Identical to `from autogluon.core import _setup_utils as ag`, but works without `autogluon.core` being installed.
 spec.loader.exec_module(ag)
 ###########################
 
 version = ag.load_version_file()
 version = ag.update_version(version)
 
-submodule = 'features'
-install_requires = [
-    # version ranges added in ag.get_dependency_version_ranges()
-    'numpy',  # version range defined in `core/_setup_utils.py`
-    'pandas',  # version range defined in `core/_setup_utils.py`
-    'scikit-learn',  # version range defined in `core/_setup_utils.py`
-    f'autogluon.common=={version}',
-] if not ag.LITE_MODE else [
-    # version ranges added in ag.get_dependency_version_ranges()
-    'numpy',  # version range defined in `core/_setup_utils.py`
-    'pandas',  # version range defined in `core/_setup_utils.py`
-    'scikit-learn',  # version range defined in `core/_setup_utils.py`
-    f'{ag.PACKAGE_NAME}.common=={version}',
-]
+submodule = "features"
+install_requires = (
+    [
+        # version ranges added in ag.get_dependency_version_ranges()
+        "numpy",  # version range defined in `core/_setup_utils.py`
+        "pandas",  # version range defined in `core/_setup_utils.py`
+        "scikit-learn",  # version range defined in `core/_setup_utils.py`
+        f"autogluon.common=={version}",
+    ]
+    if not ag.LITE_MODE
+    else [
+        # version ranges added in ag.get_dependency_version_ranges()
+        "numpy",  # version range defined in `core/_setup_utils.py`
+        "pandas",  # version range defined in `core/_setup_utils.py`
+        "scikit-learn",  # version range defined in `core/_setup_utils.py`
+        f"{ag.PACKAGE_NAME}.common=={version}",
+    ]
+)
 
 install_requires = ag.get_dependency_version_ranges(install_requires)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     ag.create_version_file(version=version, submodule=submodule)
     setup_args = ag.default_setup_args(version=version, submodule=submodule)
     setup(
         install_requires=install_requires,
         **setup_args,
     )
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/binning.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/binning.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/__init__.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from .abstract import AbstractFeatureGenerator
 from .astype import AsTypeFeatureGenerator
+from .auto_ml_pipeline import AutoMLInterpretablePipelineFeatureGenerator, AutoMLPipelineFeatureGenerator
 from .binned import BinnedFeatureGenerator
 from .bulk import BulkFeatureGenerator
 from .category import CategoryFeatureGenerator
 from .datetime import DatetimeFeatureGenerator
 from .drop_duplicates import DropDuplicatesFeatureGenerator
 from .drop_unique import DropUniqueFeatureGenerator
 from .dummy import DummyFeatureGenerator
 from .fillna import FillNaFeatureGenerator
 from .identity import IdentityFeatureGenerator
 from .isnan import IsNanFeatureGenerator
 from .label_encoder import LabelEncoderFeatureGenerator
 from .memory_minimize import CategoryMemoryMinimizeFeatureGenerator, NumericMemoryMinimizeFeatureGenerator
 from .one_hot_encoder import OneHotEncoderFeatureGenerator
+from .pipeline import PipelineFeatureGenerator
 from .rename import RenameFeatureGenerator
 from .text_ngram import TextNgramFeatureGenerator
 from .text_special import TextSpecialFeatureGenerator
-
-from .pipeline import PipelineFeatureGenerator
-from .auto_ml_pipeline import AutoMLPipelineFeatureGenerator, AutoMLInterpretablePipelineFeatureGenerator
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/abstract.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import time
 from collections import defaultdict
 from typing import Dict, List
 
 from pandas import DataFrame, Series
 
-from autogluon.common.features.infer_types import get_type_map_raw, get_type_map_real, get_type_group_map_special
 from autogluon.common.features.feature_metadata import FeatureMetadata
+from autogluon.common.features.infer_types import get_type_group_map_special, get_type_map_raw, get_type_map_real
 from autogluon.common.savers import save_pkl
 
 from ..utils import is_useless_feature
 
 logger = logging.getLogger(__name__)
 
 
@@ -106,31 +106,32 @@
         The FeatureMetadata of data post-transformation (data outputted by fit_transform and transform methods).
     feature_metadata_real : FeatureMetadata
         The FeatureMetadata of data post-transformation consisting of the exact dtypes as opposed to the grouped raw dtypes found in feature_metadata_in,
         with grouped raw dtypes substituting for the special dtypes.
         This is only used in the print_feature_metadata_info method and is intended for introspection. It can be safely set to None to reduce memory and
         disk usage post-fit.
     """
+
     def __init__(
         self,
         features_in: list = None,
         feature_metadata_in: FeatureMetadata = None,
         post_generators: list = None,
         pre_enforce_types=False,
         pre_drop_useless=False,
         post_drop_duplicates=False,
         reset_index=False,
         column_names_as_str=True,
         name_prefix: str = None,
         name_suffix: str = None,
         infer_features_in_args: dict = None,
-        infer_features_in_args_strategy='overwrite',
+        infer_features_in_args_strategy="overwrite",
         banned_feature_special_types: List[str] = None,
-        log_prefix='',
-        verbosity=2
+        log_prefix="",
+        verbosity=2,
     ):
         self._is_fit = False  # Whether the feature generator has been fit
         self.features_in = features_in  # Original features to use as input to feature generation
         self.features_out = None  # Final list of features after transformation
         self.feature_metadata_in: FeatureMetadata = feature_metadata_in  # FeatureMetadata object based on the original input features.
 
         # FeatureMetadata object based on the processed features. Pass to models to enable advanced functionality.
@@ -140,45 +141,49 @@
         #  and special dtypes all at once.
         # FeatureMetadata object based on the processed features, containing the true raw dtype information (such as int32, float64, etc.).
         # Pass to models to enable advanced functionality.
         self.feature_metadata_real: FeatureMetadata = None
         self._feature_metadata_before_post = None  # FeatureMetadata directly prior to applying self._post_generators.
         self._infer_features_in_args = self.get_default_infer_features_in_args()
         if infer_features_in_args is not None:
-            if infer_features_in_args_strategy == 'overwrite':
+            if infer_features_in_args_strategy == "overwrite":
                 self._infer_features_in_args = copy.deepcopy(infer_features_in_args)
-            elif infer_features_in_args_strategy == 'update':
+            elif infer_features_in_args_strategy == "update":
                 self._infer_features_in_args.update(infer_features_in_args)
             else:
                 raise ValueError(f"infer_features_in_args_strategy must be one of: {['overwrite', 'update']}, but was: '{infer_features_in_args_strategy}'")
         if banned_feature_special_types:
-            if 'invalid_special_types' not in self._infer_features_in_args:
-                self._infer_features_in_args['invalid_special_types'] = banned_feature_special_types
+            if "invalid_special_types" not in self._infer_features_in_args:
+                self._infer_features_in_args["invalid_special_types"] = banned_feature_special_types
             else:
                 for f in banned_feature_special_types:
-                    if f not in self._infer_features_in_args['invalid_special_types']:
-                        self._infer_features_in_args['invalid_special_types'].append(f)
+                    if f not in self._infer_features_in_args["invalid_special_types"]:
+                        self._infer_features_in_args["invalid_special_types"].append(f)
 
         if post_generators is None:
             post_generators = []
         elif not isinstance(post_generators, list):
             post_generators = [post_generators]
         self._post_generators: list = post_generators
         if post_drop_duplicates:
             from .drop_duplicates import DropDuplicatesFeatureGenerator
+
             self._post_generators.append(DropDuplicatesFeatureGenerator(post_drop_duplicates=False))
         if name_prefix or name_suffix:
             from .rename import RenameFeatureGenerator
+
             # inplace=False required to avoid altering outer context: refer to https://github.com/autogluon/autogluon/issues/2688
             self._post_generators.append(RenameFeatureGenerator(name_prefix=name_prefix, name_suffix=name_suffix, inplace=False))
 
         if self._post_generators:
-            if not self.get_tags().get('allow_post_generators', True):
-                raise AssertionError(f'{self.__class__.__name__} is not allowed to have post_generators, '
-                                     f'but found: {[generator.__class__.__name__ for generator in self._post_generators]}')
+            if not self.get_tags().get("allow_post_generators", True):
+                raise AssertionError(
+                    f"{self.__class__.__name__} is not allowed to have post_generators, "
+                    f"but found: {[generator.__class__.__name__ for generator in self._post_generators]}"
+                )
 
         self.pre_enforce_types = pre_enforce_types
         self._pre_astype_generator = None
         self.pre_drop_useless = pre_drop_useless
         self.reset_index = reset_index
         self.column_names_as_str = column_names_as_str
         self._useless_features_in: list = None
@@ -228,17 +233,17 @@
 
         Returns
         -------
         X_out : DataFrame object which is the transformed version of the input data X.
 
         """
         start_time = time.time()
-        self._log(20, f'Fitting {self.__class__.__name__}...')
+        self._log(20, f"Fitting {self.__class__.__name__}...")
         if self._is_fit:
-            raise AssertionError(f'{self.__class__.__name__} is already fit.')
+            raise AssertionError(f"{self.__class__.__name__} is already fit.")
         self._pre_fit_validate(X=X, y=y, feature_metadata_in=feature_metadata_in, **kwargs)
 
         if self.reset_index:
             X_index = copy.deepcopy(X.index)
             # TODO: Theoretically inplace=True avoids data copy, but can lead to altering of original DataFrame outside of method context.
             X = X.reset_index(drop=True)
             if y is not None and isinstance(y, Series):
@@ -260,27 +265,30 @@
         self._infer_features_in_full(X=X, feature_metadata_in=feature_metadata_in)
         if self.pre_drop_useless:
             self._useless_features_in = self._get_useless_features(X, columns_to_check=self.features_in)
             if self._useless_features_in:
                 self._remove_features_in(self._useless_features_in)
         if self.pre_enforce_types:
             from .astype import AsTypeFeatureGenerator
+
             self._pre_astype_generator = AsTypeFeatureGenerator(
-                features_in=self.features_in, feature_metadata_in=self.feature_metadata_in, log_prefix=self.log_prefix + '\t')
+                features_in=self.features_in, feature_metadata_in=self.feature_metadata_in, log_prefix=self.log_prefix + "\t"
+            )
             self._pre_astype_generator.fit(X)
 
         # TODO: Add option to return feature_metadata instead to avoid data copy
         #  If so, consider adding validation step to check that X_out matches the feature metadata, error/warning if not
         X_out, type_family_groups_special = self._fit_transform(X[self.features_in], y=y, **kwargs)
 
         type_map_raw = get_type_map_raw(X_out)
         self._feature_metadata_before_post = FeatureMetadata(type_map_raw=type_map_raw, type_group_map_special=type_family_groups_special)
         if self._post_generators:
             X_out, self.feature_metadata, self._post_generators = self._fit_generators(
-                X=X_out, y=y, feature_metadata=self._feature_metadata_before_post, generators=self._post_generators, **kwargs)
+                X=X_out, y=y, feature_metadata=self._feature_metadata_before_post, generators=self._post_generators, **kwargs
+            )
         else:
             self.feature_metadata = self._feature_metadata_before_post
         type_map_real = get_type_map_real(X_out)
         self.features_out = list(X_out.columns)
         self.feature_metadata_real = FeatureMetadata(type_map_raw=type_map_real, type_group_map_special=self.feature_metadata.get_type_group_map_raw())
 
         self._post_fit_cleanup()
@@ -310,15 +318,15 @@
             Extra columns present in X that are not in features_in will be ignored and not affect the output.
 
         Returns
         -------
         X_out : DataFrame object which is the transformed version of the input data X.
         """
         if not self._is_fit:
-            raise AssertionError(f'{self.__class__.__name__} is not fit.')
+            raise AssertionError(f"{self.__class__.__name__} is not fit.")
         if self.reset_index:
             X_index = copy.deepcopy(X.index)
             # TODO: Theoretically inplace=True avoids data copy, but can lead to altering of original DataFrame outside of method context.
             X = X.reset_index(drop=True)
         else:
             X_index = None
         if self.column_names_as_str:
@@ -329,17 +337,19 @@
                 # therefore, try avoid copying by checking the expected features first.
                 X = X[self.features_in]
         except KeyError:
             missing_cols = []
             for col in self.features_in:
                 if col not in X.columns:
                     missing_cols.append(col)
-            raise KeyError(f'{len(missing_cols)} required columns are missing from the provided dataset to transform using {self.__class__.__name__}. '
-                           f'{len(missing_cols)} missing columns: {missing_cols} | '
-                           f'{len(list(X.columns))} available columns: {list(X.columns)}')
+            raise KeyError(
+                f"{len(missing_cols)} required columns are missing from the provided dataset to transform using {self.__class__.__name__}. "
+                f"{len(missing_cols)} missing columns: {missing_cols} | "
+                f"{len(list(X.columns))} available columns: {list(X.columns)}"
+            )
         if self._pre_astype_generator:
             X = self._pre_astype_generator.transform(X)
         X_out = self._transform(X)
         if self._post_generators:
             X_out = self._transform_generators(X=X_out, generators=self._post_generators)
         if self.reset_index:
             X_out.index = X_index
@@ -412,19 +422,24 @@
         feature_metadata_in : FeatureMetadata, optional
             If passed, then self.feature_metadata_in will be set to feature_metadata_in assuming self.feature_metadata_in was None prior.
             If both are None, then self.feature_metadata_in is inferred through _infer_feature_metadata_in(X)
         """
         if self.feature_metadata_in is None:
             self.feature_metadata_in = feature_metadata_in
         elif feature_metadata_in is not None:
-            self._log(30, '\tWarning: feature_metadata_in passed as input to fit_transform, but self.feature_metadata_in was already set. '
-                          'Ignoring feature_metadata_in.')
+            self._log(
+                30,
+                "\tWarning: feature_metadata_in passed as input to fit_transform, but self.feature_metadata_in was already set. "
+                "Ignoring feature_metadata_in.",
+            )
         if self.feature_metadata_in is None:
-            self._log(20, '\tInferring data type of each feature based on column values. Set feature_metadata_in to manually specify special '
-                          'dtypes of the features.')
+            self._log(
+                20,
+                "\tInferring data type of each feature based on column values. Set feature_metadata_in to manually specify special " "dtypes of the features.",
+            )
             self.feature_metadata_in = self._infer_feature_metadata_in(X=X)
         if self.features_in is None:
             self.features_in = self._infer_features_in(X=X)
             self.features_in = [feature for feature in self.features_in if feature in X.columns]
         self.feature_metadata_in = self.feature_metadata_in.keep_features(features=self.features_in)
 
     # TODO: Find way to increase flexibility here, possibly through init args
@@ -475,15 +490,15 @@
         """
         Fit a list of AbstractFeatureGenerator objects in sequence, with the output of generators[i] fed as the input to generators[i+1]
         This is called to sequentially fit self._post_generators generators on the output of _fit_transform to obtain the final output of the generator.
         This should not be overwritten by implementations of AbstractFeatureGenerator.
         """
         for generator in generators:
             generator.verbosity = min(self.verbosity, generator.verbosity)
-            generator.set_log_prefix(log_prefix=self.log_prefix + '\t', prepend=True)
+            generator.set_log_prefix(log_prefix=self.log_prefix + "\t", prepend=True)
             X = generator.fit_transform(X=X, y=y, feature_metadata_in=feature_metadata, **kwargs)
             feature_metadata = generator.feature_metadata
         return X, feature_metadata, generators
 
     @staticmethod
     def _transform_generators(X, generators: list) -> DataFrame:
         """
@@ -536,16 +551,18 @@
             List of feature names to remove from the output of self.transform().
         """
         feature_links_chain = self.get_feature_links_chain()
         if features:
             self.feature_metadata = self.feature_metadata.remove_features(features=features)
             self.feature_metadata_real = self.feature_metadata_real.remove_features(features=features)
             self.features_out = self.feature_metadata.get_features()
-            feature_links_chain[-1] = {feature_in: [feature_out for feature_out in features_out if feature_out not in features] for feature_in, features_out in
-                                       feature_links_chain[-1].items()}
+            feature_links_chain[-1] = {
+                feature_in: [feature_out for feature_out in features_out if feature_out not in features]
+                for feature_in, features_out in feature_links_chain[-1].items()
+            }
         self._remove_unused_features(feature_links_chain=feature_links_chain)
 
     def _remove_unused_features(self, feature_links_chain):
         unused_features = self._get_unused_features(feature_links_chain=feature_links_chain)
         self._remove_features_in(features=unused_features[0])
         for i, generator in enumerate(self._post_generators):
             for feature in unused_features[i + 1]:
@@ -565,15 +582,15 @@
 
     def _pre_fit_validate(self, X: DataFrame, y: Series, **kwargs):
         """
         Any data validation checks prior to fitting the data should be done here.
         """
         if y is not None and isinstance(y, Series):
             if list(y.index) != list(X.index):
-                raise AssertionError(f'y.index and X.index must be equal when fitting {self.__class__.__name__}, but they differ.')
+                raise AssertionError(f"y.index and X.index must be equal when fitting {self.__class__.__name__}, but they differ.")
 
     def _post_fit_cleanup(self):
         """
         Any cleanup operations after all metadata objects have been constructed, but prior to feature renaming, should be done here.
         This includes removing keys from internal lists and dictionaries of features which have been removed, and deletion of any temp variables.
         """
         pass
@@ -583,15 +600,15 @@
             count_dict = defaultdict(int)
             invalid_columns = []
             for column in list(X.columns):
                 count_dict[column] += 1
             for column in count_dict:
                 if count_dict[column] > 1:
                     invalid_columns.append(column)
-            raise AssertionError(f'Columns appear multiple times in X. Columns must be unique. Invalid columns: {invalid_columns}')
+            raise AssertionError(f"Columns appear multiple times in X. Columns must be unique. Invalid columns: {invalid_columns}")
 
     # TODO: Move to a generator
     @staticmethod
     def _get_useless_features(X: DataFrame, columns_to_check: List[str] = None) -> list:
         useless_features = []
         if columns_to_check is None:
             columns_to_check = list(X.columns)
@@ -612,15 +629,15 @@
 
     def _log(self, level, msg, log_prefix=None, verb_min=None):
         if self.verbosity == 0:
             return
         if verb_min is None or self.verbosity >= verb_min:
             if log_prefix is None:
                 log_prefix = self.log_prefix
-            logger.log(level, f'{log_prefix}{msg}')
+            logger.log(level, f"{log_prefix}{msg}")
 
     def is_fit(self):
         return self._is_fit
 
     # TODO: Handle cases where self.features_in or self.feature_metadata_in was already set at init.
     def is_valid_metadata_in(self, feature_metadata_in: FeatureMetadata):
         """
@@ -640,15 +657,15 @@
     def get_feature_links(self) -> Dict[str, List[str]]:
         """Returns feature links including all pre and post generators."""
         return self._get_feature_links_from_chain(self.get_feature_links_chain())
 
     def _get_feature_links(self, features_in: List[str], features_out: List[str]) -> Dict[str, List[str]]:
         """Returns feature links ignoring all pre and post generators."""
         feature_links = {}
-        if self.get_tags().get('feature_interactions', True):
+        if self.get_tags().get("feature_interactions", True):
             for feature_in in features_in:
                 feature_links[feature_in] = features_out
         else:
             for feat_old, feat_new in zip(features_in, features_out):
                 feature_links[feat_old] = feature_links.get(feat_old, []) + [feat_new]
         return feature_links
 
@@ -691,15 +708,15 @@
     def _get_unused_features(self, feature_links_chain: List[Dict[str, List[str]]]):
         features_in_list = [self.features_in]
         if self._post_generators:
             for i in range(len(self._post_generators)):
                 if i == 0:
                     features_in = self._feature_metadata_before_post.get_features()
                 else:
-                    features_in = self._post_generators[i-1].features_out
+                    features_in = self._post_generators[i - 1].features_out
                 features_in_list.append(features_in)
         return self._get_unused_features_generic(feature_links_chain=feature_links_chain, features_in_list=features_in_list)
 
     # TODO: Unit test this
     @staticmethod
     def _get_unused_features_generic(feature_links_chain: List[Dict[str, List[str]]], features_in_list: List[List[str]]) -> List[List[str]]:
         unused_features = []
@@ -726,33 +743,33 @@
 
         Parameters
         ----------
         log_level : int, default 20
             Log level of the logging statements.
         """
         if self.fit_time:
-            self._log(log_level, f'\t{round(self.fit_time, 1)}s = Fit runtime')
-            self._log(log_level, f'\t{len(self.features_in)} features in original data used to generate {len(self.features_out)} features in processed data.')
+            self._log(log_level, f"\t{round(self.fit_time, 1)}s = Fit runtime")
+            self._log(log_level, f"\t{len(self.features_in)} features in original data used to generate {len(self.features_out)} features in processed data.")
 
     def print_feature_metadata_info(self, log_level: int = 20):
         """
         Outputs detailed logs of a fit feature generator including the input and output FeatureMetadata objects' feature types.
 
         Parameters
         ----------
         log_level : int, default 20
             Log level of the logging statements.
         """
-        self._log(log_level, '\tTypes of features in original data (raw dtype, special dtypes):')
-        self.feature_metadata_in.print_feature_metadata_full(self.log_prefix + '\t\t', log_level=log_level)
+        self._log(log_level, "\tTypes of features in original data (raw dtype, special dtypes):")
+        self.feature_metadata_in.print_feature_metadata_full(self.log_prefix + "\t\t", log_level=log_level)
         if self.feature_metadata_real:
-            self._log(log_level-5, '\tTypes of features in processed data (exact raw dtype, raw dtype):')
-            self.feature_metadata_real.print_feature_metadata_full(self.log_prefix + '\t\t', print_only_one_special=True, log_level=log_level-5)
-        self._log(log_level, '\tTypes of features in processed data (raw dtype, special dtypes):')
-        self.feature_metadata.print_feature_metadata_full(self.log_prefix + '\t\t', log_level=log_level)
+            self._log(log_level - 5, "\tTypes of features in processed data (exact raw dtype, raw dtype):")
+            self.feature_metadata_real.print_feature_metadata_full(self.log_prefix + "\t\t", print_only_one_special=True, log_level=log_level - 5)
+        self._log(log_level, "\tTypes of features in processed data (raw dtype, special dtypes):")
+        self.feature_metadata.print_feature_metadata_full(self.log_prefix + "\t\t", log_level=log_level)
 
     def save(self, path: str):
         save_pkl.save(path=path, object=self)
 
     def _more_tags(self) -> dict:
         """
         Special values to enable advanced functionality.
@@ -770,14 +787,14 @@
         """
         return {}
 
     def get_tags(self) -> dict:
         """Gets the tags for this generator."""
         collected_tags = {}
         for base_class in reversed(inspect.getmro(self.__class__)):
-            if hasattr(base_class, '_more_tags'):
+            if hasattr(base_class, "_more_tags"):
                 # need the if because mixins might not have _more_tags
                 # but might do redundant work in estimators
                 # (i.e. calling more tags on BaseEstimator multiple times)
                 more_tags = base_class._more_tags(self)
                 collected_tags.update(more_tags)
         return collected_tags
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/astype.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/astype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
-from autogluon.common.features.types import R_INT, S_BOOL
 from autogluon.common.features.feature_metadata import FeatureMetadata
-from autogluon.common.features.infer_types import get_type_map_raw, get_type_map_real, get_bool_true_val
+from autogluon.common.features.infer_types import get_bool_true_val, get_type_map_raw, get_type_map_real
+from autogluon.common.features.types import R_INT, S_BOOL
 
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add int fillna input value options: 0, set value, mean, mode, median
@@ -36,60 +36,68 @@
         15 is roughly the optimal value on average.
     convert_bool_method_v2_row_threshold : int, default 128
         [Advanced] If using "v2" bool method, this is the row count in which when >=, the batch method is used instead of the realtime method.
         128 is roughly the optimal value on average.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
-    def __init__(self,
-                 convert_bool: bool = True,
-                 convert_bool_method: str = "auto",
-                 convert_bool_method_v2_threshold: int = 15,
-                 convert_bool_method_v2_row_threshold: int = 128,
-                 **kwargs):
+
+    def __init__(
+        self,
+        convert_bool: bool = True,
+        convert_bool_method: str = "auto",
+        convert_bool_method_v2_threshold: int = 15,
+        convert_bool_method_v2_row_threshold: int = 128,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         # FeatureMetadata object based on the original input features real dtypes
         # (will contain dtypes such as 'int16' and 'float32' instead of 'int' and 'float').
         self._feature_metadata_in_real: FeatureMetadata = None
         self._type_map_real_opt: dict = None  # Optimized representation of data types, saves a few milliseconds during comparisons in online inference
         # self.inplace = inplace  # TODO, also add check if dtypes are same as expected and skip .astype
         self._int_features = None
         self._bool_features = None
         self._convert_bool = convert_bool
         self._convert_bool_method_v2_threshold = convert_bool_method_v2_threshold
         self._convert_bool_method_v2_row_threshold = convert_bool_method_v2_row_threshold
-        if convert_bool_method == 'v1':
+        if convert_bool_method == "v1":
             self._use_fast_bool_method = False
-        elif convert_bool_method == 'v2':
+        elif convert_bool_method == "v2":
             self._use_fast_bool_method = True
-        elif convert_bool_method == 'auto':
+        elif convert_bool_method == "auto":
             self._use_fast_bool_method = "auto"
         else:
-            raise ValueError(f'Unknown `convert_bool_method` value: {convert_bool_method}. '
-                             f'Valid values: ["v1", "v2", "auto"]')
+            raise ValueError(f"Unknown `convert_bool_method` value: {convert_bool_method}. " f'Valid values: ["v1", "v2", "auto"]')
         self._bool_features_list = None
         self._non_bool_features_list = None
         self._bool_features_val = None
         self._bool_features_val_np = None
 
     # TODO: consider returning self._transform(X) if we allow users to specify real dtypes as input
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         feature_type_raw_cur_dict = get_type_map_raw(X)
         feature_map_to_update = dict()
         type_map_special = self.feature_metadata_in.get_type_map_special()
         for feature in self.features_in:
             feature_type_raw = self.feature_metadata_in.get_feature_type_raw(feature)
             feature_type_raw_cur = feature_type_raw_cur_dict[feature]
             if feature_type_raw != feature_type_raw_cur:
-                self._log(30, f'\tWARNING: Actual dtype differs from dtype in FeatureMetadata for feature "{feature}". '
-                              f'Actual dtype: {feature_type_raw_cur} | Expected dtype: {feature_type_raw}')
+                self._log(
+                    30,
+                    f'\tWARNING: Actual dtype differs from dtype in FeatureMetadata for feature "{feature}". '
+                    f"Actual dtype: {feature_type_raw_cur} | Expected dtype: {feature_type_raw}",
+                )
                 feature_map_to_update[feature] = feature_type_raw
         if feature_map_to_update:
-            self._log(30, '\tWARNING: Forcefully converting features to expected dtypes. '
-                          'Please manually align the input data with the expected dtypes if issues occur.')
+            self._log(
+                30,
+                "\tWARNING: Forcefully converting features to expected dtypes. "
+                "Please manually align the input data with the expected dtypes if issues occur.",
+            )
             X = X.astype(feature_map_to_update)
 
         self._bool_features = dict()
         if self._convert_bool:
             num_rows = len(X)
             if num_rows > 1000:
                 # Sample and filter out features that already have >2 unique values
@@ -103,18 +111,17 @@
                 if S_BOOL not in type_map_special[feature]:
                     uniques = X[feature].unique()
                     if len(uniques) == 2:
                         feature_bool_val = get_bool_true_val(uniques=uniques)
                         self._bool_features[feature] = feature_bool_val
 
         if self._bool_features:
-            self._log(20, f'\tNote: Converting {len(self._bool_features)} features to boolean dtype '
-                          f'as they only contain 2 unique values.')
+            self._log(20, f"\tNote: Converting {len(self._bool_features)} features to boolean dtype " f"as they only contain 2 unique values.")
             self._set_bool_features_val()
-            if self._use_fast_bool_method == 'auto':
+            if self._use_fast_bool_method == "auto":
                 self._use_fast_bool_method = len(self._bool_features) >= self._convert_bool_method_v2_threshold
             X = self._convert_to_bool(X)
             for feature in self._bool_features:
                 type_map_special[feature] = [S_BOOL]
                 self._type_map_real_opt[feature] = np.int8
             type_group_map_special = FeatureMetadata.get_type_group_map_special_from_type_map_special(type_map_special)
         else:
@@ -131,18 +138,20 @@
                 null_count = X[self._int_features].isnull().any()
                 # If int feature contains null during inference but not during fit.
                 if null_count.any():
                     # TODO: Consider imputing to mode? This is tricky because training data had no missing values.
                     # TODO: Add unit test for this situation, to confirm it is handled properly.
                     with_null = null_count[null_count]
                     with_null_features = list(with_null.index)
-                    logger.warning('WARNING: Int features without null values '
-                                   'at train time contain null values at inference time! '
-                                   'Imputing nulls to 0. To avoid this, pass the features as floats during fit!')
-                    logger.warning(f'WARNING: Int features with nulls: {with_null_features}')
+                    logger.warning(
+                        "WARNING: Int features without null values "
+                        "at train time contain null values at inference time! "
+                        "Imputing nulls to 0. To avoid this, pass the features as floats during fit!"
+                    )
+                    logger.warning(f"WARNING: Int features with nulls: {with_null_features}")
                     X[with_null_features] = X[with_null_features].fillna(0)
 
             if self._type_map_real_opt:
                 # TODO: Confirm this works with sparse and other feature types!
                 # FIXME: Address situation where test-time invalid type values cause crash:
                 #  https://stackoverflow.com/questions/49256211/how-to-set-unexpected-data-type-to-na?noredirect=1&lq=1
                 X = X.astype(self._type_map_real_opt)
@@ -184,15 +193,15 @@
 
         # TODO: re-order columns to features_in required because `feature_interactions=False` to avoid error when feature prune.
         #  Note that this is slower than avoiding the re-order, but avoiding the re-order is very complicated to do correctly.
         return pd.concat([X[self._non_bool_features_list], X_bool], axis=1)[self.features_in]
 
     def _convert_to_bool_fast_realtime(self, X: DataFrame) -> DataFrame:
         """Optimized for when X is <= 100 rows"""
-        X_bool_features_np = X[self._bool_features_list].to_numpy(dtype='object')
+        X_bool_features_np = X[self._bool_features_list].to_numpy(dtype="object")
         X_bool_numpy = X_bool_features_np == self._bool_features_val_np
         X_bool = pd.DataFrame(X_bool_numpy, columns=self._bool_features_list, dtype=np.int8, index=X.index)
 
         # TODO: re-order columns to features_in required because `feature_interactions=False` to avoid error when feature prune.
         #  Note that this is slower than avoiding the re-order, but avoiding the re-order is very complicated to do correctly.
         return pd.concat([X[self._non_bool_features_list], X_bool], axis=1)[self.features_in]
 
@@ -214,18 +223,18 @@
                 self._type_map_real_opt.pop(feature, None)
                 self._bool_features.pop(feature, None)
             self._set_bool_features_val()
             self._int_features = np.array(self.feature_metadata_in.get_features(valid_raw_types=[R_INT]))
 
     def _set_bool_features_val(self):
         self._bool_features_val = [self._bool_features[f] for f in self._bool_features]
-        self._bool_features_val_np = np.array(self._bool_features_val, dtype='object')
+        self._bool_features_val_np = np.array(self._bool_features_val, dtype="object")
         self._bool_features_list = list(self._bool_features.keys())
         self._non_bool_features_list = [f for f in self.features_in if f not in self._bool_features]
 
     def print_feature_metadata_info(self, log_level=20):
-        self._log(log_level, '\tOriginal Features (exact raw dtype, raw dtype):')
-        self._feature_metadata_in_real.print_feature_metadata_full(self.log_prefix + '\t\t', print_only_one_special=True, log_level=log_level)
+        self._log(log_level, "\tOriginal Features (exact raw dtype, raw dtype):")
+        self._feature_metadata_in_real.print_feature_metadata_full(self.log_prefix + "\t\t", print_only_one_special=True, log_level=log_level)
         super().print_feature_metadata_info(log_level=log_level)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/auto_ml_pipeline.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/auto_ml_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
-from autogluon.common.features.types import R_INT, R_FLOAT, S_TEXT, R_OBJECT, S_IMAGE_PATH, S_IMAGE_BYTEARRAY
+from autogluon.common.features.types import R_FLOAT, R_INT, R_OBJECT, S_IMAGE_BYTEARRAY, S_IMAGE_PATH, S_TEXT
 
-from .pipeline import PipelineFeatureGenerator
 from .category import CategoryFeatureGenerator
 from .datetime import DatetimeFeatureGenerator
 from .identity import IdentityFeatureGenerator
 from .isnan import IsNanFeatureGenerator
 from .one_hot_encoder import OneHotEncoderFeatureGenerator
+from .pipeline import PipelineFeatureGenerator
 from .text_ngram import TextNgramFeatureGenerator
 from .text_special import TextSpecialFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: write out in English the full set of transformations that are applied (and eventually host page on website).
@@ -73,32 +73,38 @@
     >>>
     >>> X_train_transformed = feature_generator.fit_transform(X=X_train, y=y_train)
     >>>
     >>> test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
     >>>
     >>> X_test_transformed = feature_generator.transform(test_data)
     """
-    def __init__(self,
-                 enable_numeric_features=True,
-                 enable_categorical_features=True,
-                 enable_datetime_features=True,
-                 enable_text_special_features=True,
-                 enable_text_ngram_features=True,
-                 enable_raw_text_features=False,
-                 enable_vision_features=True,
-                 vectorizer=None,
-                 text_ngram_params=None,
-                 **kwargs):
-        if 'generators' in kwargs:
-            raise KeyError(f'generators is not a valid parameter to {self.__class__.__name__}. '
-                           f'Use {PipelineFeatureGenerator.__name__} to specify custom generators.')
-        if 'enable_raw_features' in kwargs:
-            enable_numeric_features = kwargs.pop('enable_raw_features')
-            logger.warning("'enable_raw_features is a deprecated parameter, use 'enable_numeric_features' instead. "
-                           "Specifying 'enable_raw_features' will raise an exception starting in 0.1.0")
+
+    def __init__(
+        self,
+        enable_numeric_features=True,
+        enable_categorical_features=True,
+        enable_datetime_features=True,
+        enable_text_special_features=True,
+        enable_text_ngram_features=True,
+        enable_raw_text_features=False,
+        enable_vision_features=True,
+        vectorizer=None,
+        text_ngram_params=None,
+        **kwargs,
+    ):
+        if "generators" in kwargs:
+            raise KeyError(
+                f"generators is not a valid parameter to {self.__class__.__name__}. " f"Use {PipelineFeatureGenerator.__name__} to specify custom generators."
+            )
+        if "enable_raw_features" in kwargs:
+            enable_numeric_features = kwargs.pop("enable_raw_features")
+            logger.warning(
+                "'enable_raw_features is a deprecated parameter, use 'enable_numeric_features' instead. "
+                "Specifying 'enable_raw_features' will raise an exception starting in 0.1.0"
+            )
 
         self.enable_numeric_features = enable_numeric_features
         self.enable_categorical_features = enable_categorical_features
         self.enable_datetime_features = enable_datetime_features
         self.enable_text_special_features = enable_text_special_features
         self.enable_text_ngram_features = enable_text_ngram_features
         self.enable_raw_text_features = enable_raw_text_features
@@ -107,41 +113,52 @@
 
         generators = self._get_default_generators(vectorizer=vectorizer)
         super().__init__(generators=generators, **kwargs)
 
     def _get_default_generators(self, vectorizer=None):
         generator_group = []
         if self.enable_numeric_features:
-            generator_group.append(IdentityFeatureGenerator(infer_features_in_args=dict(
-                valid_raw_types=[R_INT, R_FLOAT])))
+            generator_group.append(IdentityFeatureGenerator(infer_features_in_args=dict(valid_raw_types=[R_INT, R_FLOAT])))
         if self.enable_raw_text_features:
-            generator_group.append(IdentityFeatureGenerator(infer_features_in_args=dict(
-                required_special_types=[S_TEXT], invalid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY]), name_suffix='_raw_text'))
+            generator_group.append(
+                IdentityFeatureGenerator(
+                    infer_features_in_args=dict(required_special_types=[S_TEXT], invalid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY]),
+                    name_suffix="_raw_text",
+                )
+            )
         if self.enable_categorical_features:
             generator_group.append(self._get_category_feature_generator())
         if self.enable_datetime_features:
             generator_group.append(DatetimeFeatureGenerator())
         if self.enable_text_special_features:
             generator_group.append(TextSpecialFeatureGenerator())
         if self.enable_text_ngram_features:
             generator_group.append(TextNgramFeatureGenerator(vectorizer=vectorizer, **self.text_ngram_params))
         if self.enable_vision_features:
-            generator_group.append(IdentityFeatureGenerator(infer_features_in_args=dict(
-                valid_raw_types=[R_OBJECT], valid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY], required_at_least_one_special=True,
-            )))
-            generator_group.append(IsNanFeatureGenerator(infer_features_in_args=dict(
-                valid_raw_types=[R_OBJECT], valid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY], required_at_least_one_special=True,
-            )))
+            generator_group.append(
+                IdentityFeatureGenerator(
+                    infer_features_in_args=dict(
+                        valid_raw_types=[R_OBJECT],
+                        valid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY],
+                        required_at_least_one_special=True,
+                    )
+                )
+            )
+            generator_group.append(
+                IsNanFeatureGenerator(
+                    infer_features_in_args=dict(
+                        valid_raw_types=[R_OBJECT],
+                        valid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY],
+                        required_at_least_one_special=True,
+                    )
+                )
+            )
         generators = [generator_group]
         return generators
 
     def _get_category_feature_generator(self):
         return CategoryFeatureGenerator()
 
 
 class AutoMLInterpretablePipelineFeatureGenerator(AutoMLPipelineFeatureGenerator):
     def _get_category_feature_generator(self):
-        return CategoryFeatureGenerator(
-            minimize_memory=False,
-            maximum_num_cat=10,
-            post_generators=[OneHotEncoderFeatureGenerator()]
-        )
+        return CategoryFeatureGenerator(minimize_memory=False, maximum_num_cat=10, post_generators=[OneHotEncoderFeatureGenerator()])
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/binned.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/binned.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import copy
 import logging
 
 import pandas as pd
 from pandas import DataFrame
 
-from autogluon.common.features.types import R_INT, R_FLOAT, S_BINNED
+from autogluon.common.features.types import R_FLOAT, R_INT, S_BINNED
 
-from .abstract import AbstractFeatureGenerator
 from .. import binning
 from ..utils import get_smallest_valid_dtype_int
+from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add more parameters (possibly pass in binning function as an argument for full control)
 class BinnedFeatureGenerator(AbstractFeatureGenerator):
     """BinnedFeatureGenerator bins incoming int and float features to num_bins unique int values, maintaining relative rank order."""
+
     def __init__(self, num_bins=10, **kwargs):
         super().__init__(**kwargs)
         self.num_bins = num_bins
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         self._bin_map = self._get_bin_map(X=X)
         self._astype_map = {feature: get_smallest_valid_dtype_int(min_val=0, max_val=len(bin_index)) for feature, bin_index in self._bin_map.items()}
@@ -53,8 +54,8 @@
                     self._bin_map.pop(feature)
         if self._astype_map:
             for feature in features:
                 if feature in self._astype_map:
                     self._astype_map.pop(feature)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/bulk.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,74 +79,77 @@
     >>>
     >>> X_train_transformed = feature_generator.fit_transform(X=X_train, y=y_train)
     >>>
     >>> test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
     >>>
     >>> X_test_transformed = feature_generator.transform(test_data)
     """
+
     def __init__(self, generators: List[List[AbstractFeatureGenerator]], pre_generators: List[AbstractFeatureGenerator] = None, **kwargs):
         super().__init__(**kwargs)
         if not isinstance(generators, list):
             generators = [[generators]]
         elif len(generators) == 0:
-            raise AssertionError('generators must contain at least one AbstractFeatureGenerator.')
+            raise AssertionError("generators must contain at least one AbstractFeatureGenerator.")
         generators = [generator_group if isinstance(generator_group, list) else [generator_group] for generator_group in generators]
         if pre_generators is None:
             pre_generators = []
         elif not isinstance(pre_generators, list):
             pre_generators = [pre_generators]
         if self.pre_enforce_types:
             from .astype import AsTypeFeatureGenerator
+
             pre_generators = [AsTypeFeatureGenerator()] + pre_generators
             self.pre_enforce_types = False
         pre_generators = [[pre_generator] for pre_generator in pre_generators]
 
         if self._post_generators is not None:
             post_generators = [[post_generator] for post_generator in self._post_generators]
             self._post_generators = []
         else:
             post_generators = []
         self.generators: List[List[AbstractFeatureGenerator]] = pre_generators + generators + post_generators
 
         for generator_group in self.generators:
             for generator in generator_group:
                 if not isinstance(generator, AbstractFeatureGenerator):
-                    raise AssertionError(f'generators contains an object which is not an instance of AbstractFeatureGenerator. Invalid generator: {generator}')
+                    raise AssertionError(f"generators contains an object which is not an instance of AbstractFeatureGenerator. Invalid generator: {generator}")
 
         # FeatureMetadata object based on the original input features that were unused by any feature generator.
         self._feature_metadata_in_unused: FeatureMetadata = None
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         feature_metadata = self.feature_metadata_in
         for i in range(len(self.generators)):
-            self._log(20, f'\tStage {i + 1} Generators:')
+            self._log(20, f"\tStage {i + 1} Generators:")
             feature_df_list = []
             generator_group_valid = []
             for generator in self.generators[i]:
                 if generator.is_valid_metadata_in(feature_metadata):
                     if generator.verbosity > self.verbosity:
                         generator.verbosity = self.verbosity
-                    generator.set_log_prefix(log_prefix=self.log_prefix + '\t\t', prepend=True)
+                    generator.set_log_prefix(log_prefix=self.log_prefix + "\t\t", prepend=True)
                     feature_df_list.append(generator.fit_transform(X, feature_metadata_in=feature_metadata, **kwargs))
                     generator_group_valid.append(generator)
                 else:
-                    self._log(15, f'\t\tSkipping {generator.__class__.__name__}: No input feature with required dtypes.')
+                    self._log(15, f"\t\tSkipping {generator.__class__.__name__}: No input feature with required dtypes.")
 
             self.generators[i] = generator_group_valid
 
-            self.generators[i] = [generator for j, generator in enumerate(self.generators[i]) if
-                                  feature_df_list[j] is not None and len(feature_df_list[j].columns) > 0]
+            self.generators[i] = [
+                generator for j, generator in enumerate(self.generators[i]) if feature_df_list[j] is not None and len(feature_df_list[j].columns) > 0
+            ]
             feature_df_list = [feature_df for feature_df in feature_df_list if feature_df is not None and len(feature_df.columns) > 0]
 
             if self.generators[i]:
                 # Raise an exception if generators expect different raw input types for the same feature.
-                FeatureMetadata.join_metadatas([generator.feature_metadata_in for generator in self.generators[i]], shared_raw_features='error_if_diff')
+                FeatureMetadata.join_metadatas([generator.feature_metadata_in for generator in self.generators[i]], shared_raw_features="error_if_diff")
 
             if self.generators[i]:
-                feature_metadata = FeatureMetadata.join_metadatas([generator.feature_metadata for generator in self.generators[i]], shared_raw_features='error')
+                feature_metadata = FeatureMetadata.join_metadatas([generator.feature_metadata for generator in self.generators[i]], shared_raw_features="error")
             else:
                 feature_metadata = FeatureMetadata(type_map_raw=dict())
 
             if not feature_df_list:
                 X = DataFrame(index=X.index)
             elif len(feature_df_list) == 1:
                 X = feature_df_list[0]
@@ -216,16 +219,17 @@
 
     def _get_unused_features(self, feature_links_chain):
         features_in_list = []
         for i in range(len(self.generators)):
             stage = i + 1
             if stage > 1:
                 if self.generators[stage - 2]:
-                    features_in = FeatureMetadata.join_metadatas([generator.feature_metadata for generator in self.generators[stage - 2]],
-                                                                 shared_raw_features='error').get_features()
+                    features_in = FeatureMetadata.join_metadatas(
+                        [generator.feature_metadata for generator in self.generators[stage - 2]], shared_raw_features="error"
+                    ).get_features()
                 else:
                     features_in = []
             else:
                 features_in = self.features_in
             features_in_list.append(features_in)
         return self._get_unused_features_generic(feature_links_chain=feature_links_chain, features_in_list=features_in_list)
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/category.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import copy
 import logging
 
 import pandas as pd
 from pandas import DataFrame
 from pandas.api.types import CategoricalDtype
 
-from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_OBJECT, S_DATETIME_AS_OBJECT, S_IMAGE_PATH, S_IMAGE_BYTEARRAY, S_TEXT, S_TEXT_AS_CATEGORY
+from autogluon.common.features.types import (
+    R_BOOL,
+    R_CATEGORY,
+    R_OBJECT,
+    S_DATETIME_AS_OBJECT,
+    S_IMAGE_BYTEARRAY,
+    S_IMAGE_PATH,
+    S_TEXT,
+    S_TEXT_AS_CATEGORY,
+)
 
 from .abstract import AbstractFeatureGenerator
 from .memory_minimize import CategoryMemoryMinimizeFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
@@ -51,28 +60,36 @@
         Valid values:
             None : Keep missing values as is. They will appear as NaN and have no category assigned to them.
             'mode' : Set missing values to the most frequent category in their feature.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
 
-    def __init__(self, stateful_categories=True, minimize_memory=True, cat_order='original', minimum_cat_count: int = 2, maximum_num_cat: int = None,
-                 fillna: str = None, **kwargs):
+    def __init__(
+        self,
+        stateful_categories=True,
+        minimize_memory=True,
+        cat_order="original",
+        minimum_cat_count: int = 2,
+        maximum_num_cat: int = None,
+        fillna: str = None,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         self._stateful_categories = stateful_categories
         if minimum_cat_count is not None and minimum_cat_count < 1:
             minimum_cat_count = None
-        if cat_order not in ['original', 'alphanumeric', 'count']:
+        if cat_order not in ["original", "alphanumeric", "count"]:
             raise ValueError(f"cat_order must be one of {['original', 'alphanumeric', 'count']}, but was: {cat_order}")
         self.cat_order = cat_order
         self._minimum_cat_count = minimum_cat_count
         self._maximum_num_cat = maximum_num_cat
         self.category_map = None
         if fillna is not None:
-            if fillna not in ['mode']:
+            if fillna not in ["mode"]:
                 raise ValueError(f"fillna={fillna} is not a valid value. Valid values: {[None, 'mode']}")
         self._fillna = fillna
         self._fillna_flag = self._fillna is not None
         self._fillna_map = None
 
         if minimize_memory:
             self._post_generators = [CategoryMemoryMinimizeFeatureGenerator()] + self._post_generators
@@ -84,27 +101,25 @@
                 for column in self._fillna_map:
                     X_out[column] = X_out[column].fillna(self._fillna_map[column])
         else:
             X_out = self._transform(X)
         feature_metadata_out_type_group_map_special = copy.deepcopy(self.feature_metadata_in.type_group_map_special)
         if S_TEXT in feature_metadata_out_type_group_map_special:
             text_features = feature_metadata_out_type_group_map_special.pop(S_TEXT)
-            feature_metadata_out_type_group_map_special[S_TEXT_AS_CATEGORY] += [feature for feature in text_features if
-                                                                                feature not in feature_metadata_out_type_group_map_special[S_TEXT_AS_CATEGORY]]
+            feature_metadata_out_type_group_map_special[S_TEXT_AS_CATEGORY] += [
+                feature for feature in text_features if feature not in feature_metadata_out_type_group_map_special[S_TEXT_AS_CATEGORY]
+            ]
         return X_out, feature_metadata_out_type_group_map_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
         return self._generate_features_category(X)
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
-        return dict(
-            valid_raw_types=[R_OBJECT, R_CATEGORY, R_BOOL],
-            invalid_special_types=[S_DATETIME_AS_OBJECT, S_IMAGE_PATH, S_IMAGE_BYTEARRAY]
-        )
+        return dict(valid_raw_types=[R_OBJECT, R_CATEGORY, R_BOOL], invalid_special_types=[S_DATETIME_AS_OBJECT, S_IMAGE_PATH, S_IMAGE_BYTEARRAY])
 
     def _generate_features_category(self, X: DataFrame) -> DataFrame:
         if self.features_in:
             X_category = dict()
             if self.category_map is not None:
                 for column, column_map in self.category_map.items():
                     X_category[column] = pd.Categorical(X[column], categories=column_map)
@@ -116,40 +131,40 @@
             X_category = DataFrame(index=X.index)
         return X_category
 
     def _generate_category_map(self, X: DataFrame) -> (DataFrame, dict):
         if self.features_in:
             fill_nan_map = dict()
             category_map = dict()
-            X_category = X.astype('category')
+            X_category = X.astype("category")
             for column in X_category:
                 rank = X_category[column].value_counts().sort_values(ascending=True)
                 if self._minimum_cat_count is not None:
                     rank = rank[rank >= self._minimum_cat_count]
                 if self._maximum_num_cat is not None:
-                    rank = rank[-self._maximum_num_cat:]
-                if self.cat_order == 'count' or self._minimum_cat_count is not None or self._maximum_num_cat is not None:
+                    rank = rank[-self._maximum_num_cat :]
+                if self.cat_order == "count" or self._minimum_cat_count is not None or self._maximum_num_cat is not None:
                     category_list = list(rank.index)  # category_list in 'count' order
                     if len(category_list) > 1:
-                        if self.cat_order == 'original':
+                        if self.cat_order == "original":
                             original_cat_order = list(X_category[column].cat.categories)
                             set_category_list = set(category_list)
                             category_list = [cat for cat in original_cat_order if cat in set_category_list]
-                        elif self.cat_order == 'alphanumeric':
+                        elif self.cat_order == "alphanumeric":
                             category_list.sort()
                     X_category[column] = X_category[column].astype(CategoricalDtype(categories=category_list))  # TODO: Remove columns if all NaN after this?
                     X_category[column] = X_category[column].cat.reorder_categories(category_list)
-                elif self.cat_order == 'alphanumeric':
+                elif self.cat_order == "alphanumeric":
                     category_list = list(X_category[column].cat.categories)
                     category_list.sort()
                     X_category[column] = X_category[column].astype(CategoricalDtype(categories=category_list))
                     X_category[column] = X_category[column].cat.reorder_categories(category_list)
                 category_map[column] = copy.deepcopy(X_category[column].cat.categories)
                 if self._fillna_flag:
-                    if self._fillna == 'mode':
+                    if self._fillna == "mode":
                         if len(rank) > 0:
                             fill_nan_map[column] = list(rank.index)[-1]
             if not self._fillna_flag:
                 fill_nan_map = None
             return X_category, category_map, fill_nan_map
         else:
             return DataFrame(index=X.index), None, None
@@ -162,8 +177,8 @@
                     self.category_map.pop(feature)
         if self._fillna_map:
             for feature in features:
                 if feature in self._fillna_map:
                     self._fillna_map.pop(feature)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/datetime.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/datetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 from pandas import DataFrame
 
 from autogluon.common.features.types import R_DATETIME, S_DATETIME_AS_OBJECT
+
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 class DatetimeFeatureGenerator(AbstractFeatureGenerator):
     """Transforms datetime features into numeric features.
@@ -16,62 +17,55 @@
     Parameters
     ----------
     features : list, optional
         A list of datetime features to parse out of dates.
         For a full list of options see the methods inside pandas.Series.dt at https://pandas.pydata.org/docs/reference/api/pandas.Series.html
     """
 
-    def __init__(self,
-                 features: list = ['year', 'month', 'day', 'dayofweek'],
-                 **kwargs):
+    def __init__(self, features: list = ["year", "month", "day", "dayofweek"], **kwargs):
         super().__init__(**kwargs)
         self.features = features
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         self._fillna_map = dict()
         X_out = self._transform(X, is_fit=True)
-        type_family_groups_special = dict(
-            datetime_as_int=list(X_out.columns)
-        )
+        type_family_groups_special = dict(datetime_as_int=list(X_out.columns))
         return X_out, type_family_groups_special
 
     def _transform(self, X: DataFrame, is_fit=False) -> DataFrame:
         return self._generate_features_datetime(X, is_fit=is_fit)
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
-        return dict(required_raw_special_pairs=[
-            (R_DATETIME, None),
-            (None, [S_DATETIME_AS_OBJECT])
-        ])
+        return dict(required_raw_special_pairs=[(R_DATETIME, None), (None, [S_DATETIME_AS_OBJECT])])
 
     def normalize_timeseries(self, X: pd.DataFrame, feature: str, is_fit: bool) -> pd.Series:
         # TODO: Be aware: When converted to float32 by downstream models, the seconds value will be up to 3 seconds off the true time due to rounding error.
         #  If seconds matter, find a separate way to generate (Possibly subtract smallest datetime from all values).
         # TODO: could also return an extra boolean column is_nan which could provide predictive signal.
         # Note: The .replace call is required to handle the obnoxious edge-case of:
         #   NaN, empty string, datetime without timezone, and datetime with timezone, all as an object type, all being present in the same column.
         #   I don't know why, but in this specific situation (and not otherwise), NaN will be filled by .fillna, but empty string will be converted to NaT
         #   and refuses to be filled by .fillna, requiring a dedicated replace call. (NaT is filled by .fillna in every other situation...)
-        series = pd.to_datetime(X[feature].copy(), utc=True, errors='coerce')
-        broken_idx = series[(series == 'NaT') | series.isna() | series.isnull()].index
+        series = pd.to_datetime(X[feature].copy(), utc=True, errors="coerce")
+        broken_idx = series[(series == "NaT") | series.isna() | series.isnull()].index
         bad_rows = series.iloc[broken_idx]
         if is_fit:
             good_rows = series[~series.isin(bad_rows)].astype(np.int64)
             self._fillna_map[feature] = pd.to_datetime(int(good_rows.mean()), utc=True)
         series[broken_idx] = self._fillna_map[feature]
         return series
 
     # TODO: Improve handling of missing datetimes
     def _generate_features_datetime(self, X: DataFrame, is_fit: bool) -> DataFrame:
         X_datetime = DataFrame(index=X.index)
         for datetime_feature in self.features_in:
             X_datetime[datetime_feature] = self.normalize_timeseries(X, datetime_feature, is_fit=is_fit)
             for feature in self.features:
-                X_datetime[datetime_feature + '.' + feature] = getattr(X_datetime[datetime_feature].dt, feature).astype(np.int64)
+                X_datetime[datetime_feature + "." + feature] = getattr(X_datetime[datetime_feature].dt, feature).astype(np.int64)
             X_datetime[datetime_feature] = pd.to_numeric(X_datetime[datetime_feature])
         return X_datetime
 
     def _remove_features_in(self, features: list):
         super()._remove_features_in(features)
         if self._fillna_map:
             for feature in features:
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/drop_duplicates.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/drop_duplicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-from typing import Union
 from collections import defaultdict
+from typing import Union
 
 import numpy as np
 from pandas import DataFrame
 
-from autogluon.common.features.types import R_INT, R_FLOAT, R_CATEGORY, R_BOOL
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Not necessary to exist after fitting, can just update outer context feature_out/feature_in and then delete this
@@ -28,41 +28,42 @@
         This theoretically can lead to features that are very nearly duplicates but not exact duplicates being removed,
         but should be near impossible in practice.
         If None or greater than the number of rows, will perform exact duplicate detection (most expensive).
         It is recommended to keep this value below 100000 to maintain reasonable fit times.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
+
     def __init__(self, sample_size_init=500, sample_size_final=2000, **kwargs):
         super().__init__(**kwargs)
         self.sample_size_init = sample_size_init
         self.sample_size_final = sample_size_final
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         if self.sample_size_init is not None and len(X) > self.sample_size_init:
             features_to_check = self._drop_duplicate_features(X, self.feature_metadata_in, keep=False, sample_size=self.sample_size_init)
             X_candidates = X[features_to_check]
         else:
             X_candidates = X
         features_to_drop = self._drop_duplicate_features(X_candidates, self.feature_metadata_in, sample_size=self.sample_size_final)
         self._remove_features_in(features_to_drop)
         if features_to_drop:
-            self._log(15, f'\t{len(features_to_drop)} duplicate columns removed: {features_to_drop}')
+            self._log(15, f"\t{len(features_to_drop)} duplicate columns removed: {features_to_drop}")
         X_out = X[self.features_in]
         return X_out, self.feature_metadata_in.type_group_map_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
         return X
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict()
 
     @classmethod
-    def _drop_duplicate_features(cls, X: DataFrame, feature_metadata_in, keep: Union[str, bool] = 'first', sample_size=None) -> list:
+    def _drop_duplicate_features(cls, X: DataFrame, feature_metadata_in, keep: Union[str, bool] = "first", sample_size=None) -> list:
         if sample_size is not None and len(X) > sample_size:
             X = X.sample(sample_size, random_state=0)
         features_to_remove = []
 
         X_columns = set(X.columns)
         features_to_check_numeric = feature_metadata_in.get_features(valid_raw_types=[R_INT, R_FLOAT])
         features_to_check_numeric = [feature for feature in features_to_check_numeric if feature in X_columns]
@@ -79,23 +80,23 @@
 
         if len(X.columns) > 0:
             features_to_remove += cls._drop_duplicate_features_generic(X=X, keep=keep)
 
         return features_to_remove
 
     @classmethod
-    def _drop_duplicate_features_generic(cls, X: DataFrame, keep: Union[str, bool] = 'first'):
+    def _drop_duplicate_features_generic(cls, X: DataFrame, keep: Union[str, bool] = "first"):
         """Generic duplication dropping method. Much slower than optimized variants, but can handle all data types."""
         X_columns = list(X.columns)
         features_to_keep = set(X.T.drop_duplicates(keep=keep).T.columns)
         features_to_remove = [column for column in X_columns if column not in features_to_keep]
         return features_to_remove
 
     @classmethod
-    def _drop_duplicate_features_numeric(cls, X: DataFrame, keep: Union[str, bool] = 'first'):
+    def _drop_duplicate_features_numeric(cls, X: DataFrame, keep: Union[str, bool] = "first"):
         X_columns = list(X.columns)
         feature_sum_map = defaultdict(list)
         for feature in X_columns:
             feature_sum_map[round(X[feature].sum(), 2)].append(feature)
 
         features_to_remove = []
         for key in feature_sum_map:
@@ -103,15 +104,15 @@
                 continue
             features_to_keep = set(X[feature_sum_map[key]].T.drop_duplicates(keep=keep).T.columns)
             features_to_remove += [feature for feature in feature_sum_map[key] if feature not in features_to_keep]
 
         return features_to_remove
 
     @classmethod
-    def _drop_duplicate_features_categorical(cls, X: DataFrame, keep: Union[str, bool] = 'first'):
+    def _drop_duplicate_features_categorical(cls, X: DataFrame, keep: Union[str, bool] = "first"):
         """
         Drops duplicate features if they contain the same information, ignoring the actual values in the features.
         For example, ['a', 'b', 'b'] is considered a duplicate of ['b', 'a', 'a'], but not ['a', 'b', 'a'].
         """
         X_columns = list(X.columns)
         mapping_features_val_dict = {}
         features_unique_count_dict = defaultdict(list)
@@ -127,14 +128,14 @@
             if len(features_to_check) <= 1:
                 continue
             mapping_features_val_dict_cur = {feature: mapping_features_val_dict[feature] for feature in features_to_check}
             # Converts ['a', 'd', 'f', 'a'] to [0, 1, 2, 0]
             # Converts [5, 'a', np.nan, 5] to [0, 1, 2, 0], these would be considered duplicates since they carry the same information.
 
             # Have to convert to object dtype because category dtype for unknown reasons will refuse to replace NaNs.
-            X_cur = X[features_to_check].astype('object').replace(mapping_features_val_dict_cur).astype(np.int64)
+            X_cur = X[features_to_check].astype("object").replace(mapping_features_val_dict_cur).astype(np.int64)
             features_to_remove += cls._drop_duplicate_features_numeric(X=X_cur, keep=keep)
 
         return features_to_remove
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/drop_unique.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/drop_unique.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 
 from pandas import DataFrame
 
-from autogluon.common.features.types import R_CATEGORY, R_OBJECT, S_TEXT, S_IMAGE_PATH, S_IMAGE_BYTEARRAY
 from autogluon.common.features.feature_metadata import FeatureMetadata
+from autogluon.common.features.types import R_CATEGORY, R_OBJECT, S_IMAGE_BYTEARRAY, S_IMAGE_PATH, S_TEXT
 
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Not necessary to exist after fitting, can just update outer context feature_out/feature_in and then delete this
 class DropUniqueFeatureGenerator(AbstractFeatureGenerator):
     """Drops features which only have 1 unique value or which have nearly no repeated values (based on max_unique_ratio) and are of category or object type."""
+
     def __init__(self, max_unique_ratio=0.99, **kwargs):
         super().__init__(**kwargs)
         self.max_unique_ratio = max_unique_ratio
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         features_to_drop = self._drop_unique_features(X, self.feature_metadata_in, max_unique_ratio=self.max_unique_ratio)
         self._remove_features_in(features_to_drop)
@@ -37,16 +38,15 @@
         X_len = len(X)
         max_unique_value_count = X_len * max_unique_ratio
         for column in X:
             unique_value_count = len(X[column].unique())
             # Drop features that are always the same
             if unique_value_count == 1:
                 features_to_drop.append(column)
-            elif feature_metadata.get_feature_type_raw(column) in [R_CATEGORY, R_OBJECT]\
-                    and (unique_value_count > max_unique_value_count):
+            elif feature_metadata.get_feature_type_raw(column) in [R_CATEGORY, R_OBJECT] and (unique_value_count > max_unique_value_count):
                 special_types = feature_metadata.get_feature_types_special(column)
                 if S_TEXT in special_types:
                     # We should not drop a text column
                     continue
                 elif S_IMAGE_PATH in special_types:
                     # We should not drop an image path column
                     continue
@@ -54,8 +54,8 @@
                     # We should not drop an image bytearray column
                     continue
                 else:
                     features_to_drop.append(column)
         return features_to_drop
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/dummy.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 
 class DummyFeatureGenerator(AbstractFeatureGenerator):
     """
     Ignores all input features and returns a single int feature with all 0 values.
     Useful for testing purposes or to avoid crashes if no features were given.
     """
-    def __init__(self, features_in='empty', feature_metadata_in='empty', **kwargs):
-        if features_in == 'empty':
+
+    def __init__(self, features_in="empty", feature_metadata_in="empty", **kwargs):
+        if features_in == "empty":
             features_in = []
-        if feature_metadata_in == 'empty':
+        if feature_metadata_in == "empty":
             feature_metadata_in = FeatureMetadata(type_map_raw={})
         super().__init__(features_in=features_in, feature_metadata_in=feature_metadata_in, **kwargs)
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         X_out = self._transform(X)
         return X_out, dict()
 
@@ -31,12 +32,12 @@
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict(valid_raw_types=[])
 
     @staticmethod
     def _generate_features_dummy(X: DataFrame):
         X_out = DataFrame(index=X.index)
-        X_out['__dummy__'] = 0
+        X_out["__dummy__"] = 0
         return X_out
 
     def is_valid_metadata_in(self, feature_metadata_in: FeatureMetadata):
         return True
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/fillna.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/fillna.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,19 @@
         Be careful about setting this to anything other than np.nan, as not all raw types can handle int, float, or string values.
     inplace : bool, default False
         If True, then the NaN values are filled inplace without copying the input data.
         This will alter the input data outside of the scope of this function.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
+
     def __init__(self, fillna_map=None, fillna_default=np.nan, inplace=False, **kwargs):
         super().__init__(**kwargs)
         if fillna_map is None:
-            fillna_map = {R_OBJECT: ''}
+            fillna_map = {R_OBJECT: ""}
         self.fillna_map = fillna_map
         self.fillna_default = fillna_default
         self._fillna_feature_map = None
         self.inplace = inplace
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         features = self.feature_metadata_in.get_features()
@@ -66,8 +67,8 @@
     def _remove_features_in(self, features):
         super()._remove_features_in(features)
         if features:
             for feature in features:
                 self._fillna_feature_map.pop(feature, None)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/identity.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/identity.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 class IdentityFeatureGenerator(AbstractFeatureGenerator):
     """IdentityFeatureGenerator simply passes the data along without alterations."""
+
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         X_out = self._transform(X)
         return X_out, self.feature_metadata_in.type_group_map_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
         return X
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict()
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/isnan.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/isnan.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,19 @@
         Map which dictates the values to consider as NaN.
         Keys are the raw types of the features as in self.feature_metadata_in.type_map_raw.
         If a feature's raw type is not present in null_map, np.nan is treated as NaN.
         If a value other than np.nan is specified, np.nan is not considered NaN.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
+
     def __init__(self, null_map=None, **kwargs):
         super().__init__(**kwargs)
         if null_map is None:
-            null_map = {R_OBJECT: ''}
+            null_map = {R_OBJECT: ""}
         self.null_map = null_map
         self._null_feature_map = None
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         features = self.feature_metadata_in.get_features()
         self._null_feature_map = dict()
         for feature in features:
@@ -45,25 +46,25 @@
 
     # TODO: Try returning bool type instead of uint8
     def _transform(self, X: DataFrame) -> DataFrame:
         is_nan_features = dict()
         for feature in self.features_in:
             if feature in self._null_feature_map:
                 null_val = self._null_feature_map[feature]
-                is_nan_features['__nan__.' + feature] = (X[feature] == null_val).astype(np.uint8)
+                is_nan_features["__nan__." + feature] = (X[feature] == null_val).astype(np.uint8)
             else:
-                is_nan_features['__nan__.' + feature] = X[feature].isnull().astype(np.uint8)
+                is_nan_features["__nan__." + feature] = X[feature].isnull().astype(np.uint8)
         return pd.DataFrame(is_nan_features, index=X.index)
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict()
 
     def _remove_features_in(self, features: list):
         super()._remove_features_in(features)
         if self._null_feature_map:
             for feature in features:
                 if feature in self._null_feature_map:
                     self._null_feature_map.pop(feature)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/label_encoder.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/label_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: LabelEncoderTransformer
 class LabelEncoderFeatureGenerator(AbstractFeatureGenerator):
     """Converts category features to int features by mapping to the category codes."""
+
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         X_out = self._transform(X)
         feature_metadata_out_type_group_map_special = copy.deepcopy(self.feature_metadata_in.type_group_map_special)
         if S_TEXT_AS_CATEGORY in feature_metadata_out_type_group_map_special:
             feature_metadata_out_type_group_map_special.pop(S_TEXT_AS_CATEGORY)
         return X_out, feature_metadata_out_type_group_map_special
 
@@ -30,8 +31,8 @@
     @staticmethod
     def convert_category_to_int(X: DataFrame) -> DataFrame:
         # TODO: add inplace option?
         X = X.apply(lambda x: x.cat.codes)
         return X
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/memory_minimize.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/memory_minimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 
 import numpy as np
 from pandas import DataFrame, RangeIndex
 
 from autogluon.common.features.types import R_CATEGORY, R_INT
 
-from . import AbstractFeatureGenerator
 from ..utils import clip_and_astype
+from . import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 class CategoryMemoryMinimizeFeatureGenerator(AbstractFeatureGenerator):
     """
     Minimizes memory usage of category features by converting the category values to monotonically increasing int values.
     This is important for category features with string values which can take up significant memory despite the string information not being used downstream.
     """
+
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         self._category_maps = self._get_category_map(X=X)
 
         X_out = self._transform(X)
         return X_out, self.feature_metadata_in.type_group_map_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
@@ -50,28 +51,29 @@
         super()._remove_features_in(features)
         if self._category_maps:
             for feature in features:
                 if feature in self._category_maps:
                     self._category_maps.pop(feature)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
 
 
 # TODO: What about nulls / unknowns?
 class NumericMemoryMinimizeFeatureGenerator(AbstractFeatureGenerator):
     """
     Clips and converts dtype of int features to minimize memory usage.
 
     dtype_out : np.dtype, default np.uint8
         dtype to clip and convert features to.
         Clipping will automatically use the correct min and max values for the dtype provided.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
+
     def __init__(self, dtype_out=np.uint8, **kwargs):
         super().__init__(**kwargs)
         self.dtype_out, self._clip_min, self._clip_max = self._get_dtype_clip_args(dtype_out)
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         X_out = self._transform(X)
         return X_out, self.feature_metadata_in.type_group_map_special
@@ -91,8 +93,8 @@
             dtype_info = np.finfo(dtype)
         return dtype_info.dtype, dtype_info.min, dtype_info.max
 
     def _minimize_numeric_memory_usage(self, X: DataFrame):
         return clip_and_astype(df=X, clip_min=self._clip_min, clip_max=self._clip_max, dtype=self.dtype_out)
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/one_hot_encoder.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/one_hot_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 from sklearn.preprocessing import OneHotEncoder
 
-from autogluon.common.features.types import R_CATEGORY, S_BOOL, S_SPARSE, R_INT
+from autogluon.common.features.types import R_CATEGORY, R_INT, S_BOOL, S_SPARSE
 
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 class CatToInt:
@@ -25,58 +25,59 @@
         The default value to fill NaN.
         If None, automatically inferred as a new value not present in existing categories.
     infrequent_val : int or {'na', 'na+1}, default = 'na'
         The value to group all infrequent categories to (those that aren't within the max_levels most frequent categories).
         If 'na', uses `fillna_val`.
         If 'na+1', uses `fillna_val+1`. This guarantees a new category for infrequent values separate from missing values if `fillna_val=None`.
     """
-    def __init__(self, max_levels, fillna_val=None, infrequent_val='na'):
+
+    def __init__(self, max_levels, fillna_val=None, infrequent_val="na"):
         self.max_levels = max_levels
         self.fillna_val = fillna_val
         self.infrequent_val = infrequent_val
         self.cats = dict()
         self.num_cols = None
         self._dtype = None
 
     def fit(self, X: DataFrame):
         # dtype_buffer=2 is required to avoid edge case errors with invalid self.infrequent_val in 'na+1' mode.
         self._dtype, fillna_val = self._get_dtype_and_fillna(X, dtype_buffer=2)
         if self.fillna_val is None:
             self.fillna_val = fillna_val
-        if self.infrequent_val == 'na':
+        if self.infrequent_val == "na":
             self.infrequent_val = self.fillna_val
-        elif self.infrequent_val == 'na+1':
+        elif self.infrequent_val == "na+1":
             self.infrequent_val = self.fillna_val + 1
 
         X = self.pd_to_np(X)
         self.num_cols = X.shape[1]
         for col in range(self.num_cols):
             data = X[:, col]
             uniques, counts = np.unique(data, return_counts=True)
-            self.cats[col] = uniques[np.argsort(counts)[-self.max_levels:]]
+            self.cats[col] = uniques[np.argsort(counts)[-self.max_levels :]]
             with warnings.catch_warnings():
                 # Refer to https://stackoverflow.com/questions/40659212/futurewarning-elementwise-comparison-failed-returning-scalar-but-in-the-futur
-                warnings.simplefilter(action='ignore', category=FutureWarning)
+                warnings.simplefilter(action="ignore", category=FutureWarning)
                 if self.infrequent_val in self.cats[col] or str(self.infrequent_val) in self.cats[col]:
                     # Add one extra level since NaN values shouldn't be counted towards max levels
-                    self.cats[col] = uniques[np.argsort(counts)[-(self.max_levels+1):]]
+                    self.cats[col] = uniques[np.argsort(counts)[-(self.max_levels + 1) :]]
 
     def transform(self, X: DataFrame):
         X = self.pd_to_np(X)
         mask = np.zeros(shape=X.shape, dtype=bool)
         for col in range(self.num_cols):
             mask[:, col] = np.isin(X[:, col], self.cats[col], invert=True)
         X[mask] = self.infrequent_val
         return X
 
     def pd_to_np(self, X: DataFrame) -> np.ndarray:
         return X.to_numpy(dtype=self._dtype, na_value=self.fillna_val, copy=True)
 
     def _get_dtype_and_fillna(self, X: DataFrame, dtype_buffer=2):
-        assert dtype_buffer >= 1, 'dtype_buffer must be >= 1 or else fillna_val could be invalid.'
+        assert dtype_buffer >= 1, "dtype_buffer must be >= 1 or else fillna_val could be invalid."
         dtype = None
         max_val_all = None
         for col in X.columns:
             try:
                 max_val = X[col].dtype.categories.max()
                 min_val = X[col].dtype.categories.min()
             except:
@@ -117,19 +118,20 @@
     dtype : number type, default = np.uint8
         Desired dtype of output.
     sparse : bool, default = True
         Will return sparse matrix if set True else will return an array.
     drop : str, default = None
         Refer to OneHotEncoder documentation for details.
     """
+
     def __init__(self, max_levels=None, dtype=np.uint8, sparse=True, drop=None, **kwargs):
         super().__init__(**kwargs)
         self.max_levels = max_levels
         self.sparse = sparse
-        self._ohe = OneHotEncoder(dtype=dtype, sparse=self.sparse, handle_unknown='ignore', drop=drop)
+        self._ohe = OneHotEncoder(dtype=dtype, sparse=self.sparse, handle_unknown="ignore", drop=drop)
         self._ohe_columns = None
         self._cat_feat_gen = None
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         if self.max_levels is not None:
             self._cat_feat_gen = CatToInt(max_levels=self.max_levels)
             self._cat_feat_gen.fit(X)
@@ -167,8 +169,8 @@
         """
         if self._cat_feat_gen is not None:
             X = self._cat_feat_gen.transform(X)
         X = self._ohe.transform(X)
         return X
 
     def _more_tags(self):
-        return {'feature_interactions': False}
+        return {"feature_interactions": False}
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/pipeline.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,39 +5,57 @@
 
 from autogluon.common.features.feature_metadata import FeatureMetadata
 from autogluon.common.features.infer_types import get_type_map_real
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
 
 from .bulk import BulkFeatureGenerator
-from .dummy import DummyFeatureGenerator
 from .drop_unique import DropUniqueFeatureGenerator
+from .dummy import DummyFeatureGenerator
 from .fillna import FillNaFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Documentation
 class PipelineFeatureGenerator(BulkFeatureGenerator):
     """
     PipelineFeatureGenerator is an implementation of BulkFeatureGenerator with various smart defaults and edge case handling functionality to enable
     robust data handling.
     It is recommended that users base any custom feature generators meant for end-to-end data transformation from PipelineFeatureGenerator.
         Reference AutoMLPipelineFeatureGenerator for an example of extending PipelineFeatureGenerator.
     It is not recommended that PipelineFeatureGenerator be used as a generator within any other generator's pre or post generators.
     """
-    def __init__(self, pre_generators=None, post_generators=None, pre_drop_useless=True, pre_enforce_types=True, reset_index=True, post_drop_duplicates=True, verbosity=3, **kwargs):
+
+    def __init__(
+        self,
+        pre_generators=None,
+        post_generators=None,
+        pre_drop_useless=True,
+        pre_enforce_types=True,
+        reset_index=True,
+        post_drop_duplicates=True,
+        verbosity=3,
+        **kwargs,
+    ):
         if pre_generators is None:
             pre_generators = [FillNaFeatureGenerator(inplace=True)]
         if post_generators is None:
             post_generators = [DropUniqueFeatureGenerator()]
 
-        super().__init__(pre_generators=pre_generators, post_generators=post_generators,
-                         post_drop_duplicates=post_drop_duplicates, pre_drop_useless=pre_drop_useless, pre_enforce_types=pre_enforce_types,
-                         reset_index=reset_index, verbosity=verbosity, **kwargs)
+        super().__init__(
+            pre_generators=pre_generators,
+            post_generators=post_generators,
+            post_drop_duplicates=post_drop_duplicates,
+            pre_drop_useless=pre_drop_useless,
+            pre_enforce_types=pre_enforce_types,
+            reset_index=reset_index,
+            verbosity=verbosity,
+            **kwargs,
+        )
 
         # FeatureMetadata object based on the original input features real dtypes
         # (will contain dtypes such as 'int16' and 'float32' instead of 'int' and 'float').
         self._feature_metadata_in_real: FeatureMetadata = None
 
         self._is_dummy = False  # If True, returns a single dummy feature as output. Occurs if fit with no useful features.
 
@@ -57,16 +75,19 @@
         X_out, type_group_map_special = super()._fit_transform(X=X, y=y, **kwargs)
         X_out, type_group_map_special = self._fit_transform_custom(X_out=X_out, type_group_map_special=type_group_map_special, y=y)
         return X_out, type_group_map_special
 
     def _fit_transform_custom(self, X_out: DataFrame, type_group_map_special: dict, y=None) -> (DataFrame, dict):
         if len(list(X_out.columns)) == 0:
             self._is_dummy = True
-            self._log(30, '\tWARNING: No useful features were detected in the data! AutoGluon will train using 0 features, '
-                          'and will always predict the same value. Ensure that you are passing the correct data to AutoGluon!')
+            self._log(
+                30,
+                "\tWARNING: No useful features were detected in the data! AutoGluon will train using 0 features, "
+                "and will always predict the same value. Ensure that you are passing the correct data to AutoGluon!",
+            )
             dummy_generator = DummyFeatureGenerator()
             X_out = dummy_generator.fit_transform(X=X_out)
             type_group_map_special = copy.deepcopy(dummy_generator.feature_metadata.type_group_map_special)
             self.generators = [[dummy_generator]]
             self._remove_features_in(features=self.features_in)
         return X_out, type_group_map_special
 
@@ -87,48 +108,69 @@
 
     def _compute_pre_memory_usage(self, X: DataFrame):
         X_len = len(X)
         self.pre_memory_usage = get_approximate_df_mem_usage(X, sample_ratio=0.2).sum()
         self.pre_memory_usage_per_row = self.pre_memory_usage / X_len
         available_mem = ResourceManager.get_available_virtual_mem()
         pre_memory_usage_percent = self.pre_memory_usage / (available_mem + self.pre_memory_usage)
-        self._log(20, f'\tAvailable Memory:                    {(round((self.pre_memory_usage + available_mem) / 1e6, 2))} MB')
-        self._log(20, f'\tTrain Data (Original)  Memory Usage: {round(self.pre_memory_usage / 1e6, 2)} MB '
-                      f'({round(pre_memory_usage_percent * 100, 1)}% of available memory)')
+        self._log(20, f"\tAvailable Memory:                    {(round((self.pre_memory_usage + available_mem) / 1e6, 2))} MB")
+        self._log(
+            20,
+            f"\tTrain Data (Original)  Memory Usage: {round(self.pre_memory_usage / 1e6, 2)} MB "
+            f"({round(pre_memory_usage_percent * 100, 1)}% of available memory)",
+        )
         if pre_memory_usage_percent > 0.05:
-            self._log(30, f'\tWarning: Data size prior to feature transformation consumes {round(pre_memory_usage_percent * 100, 1)}% of available memory. '
-                          f'Consider increasing memory or subsampling the data to avoid instability.')
+            self._log(
+                30,
+                f"\tWarning: Data size prior to feature transformation consumes {round(pre_memory_usage_percent * 100, 1)}% of available memory. "
+                f"Consider increasing memory or subsampling the data to avoid instability.",
+            )
 
     def _compute_post_memory_usage(self, X: DataFrame):
         X_len = len(X)
         self.post_memory_usage = get_approximate_df_mem_usage(X, sample_ratio=0.2).sum()
         self.post_memory_usage_per_row = self.post_memory_usage / X_len
 
         available_mem = ResourceManager.get_available_virtual_mem()
         post_memory_usage_percent = self.post_memory_usage / (available_mem + self.post_memory_usage + self.pre_memory_usage)
-        self._log(20, f'\tTrain Data (Processed) Memory Usage: {round(self.post_memory_usage / 1e6, 2)} MB '
-                      f'({round(post_memory_usage_percent * 100, 1)}% of available memory)')
+        self._log(
+            20,
+            f"\tTrain Data (Processed) Memory Usage: {round(self.post_memory_usage / 1e6, 2)} MB "
+            f"({round(post_memory_usage_percent * 100, 1)}% of available memory)",
+        )
         if post_memory_usage_percent > 0.15:
-            self._log(30, f'\tWarning: Data size post feature transformation consumes {round(post_memory_usage_percent * 100, 1)}% of available memory. '
-                          f'Consider increasing memory or subsampling the data to avoid instability.')
+            self._log(
+                30,
+                f"\tWarning: Data size post feature transformation consumes {round(post_memory_usage_percent * 100, 1)}% of available memory. "
+                f"Consider increasing memory or subsampling the data to avoid instability.",
+            )
 
     def print_feature_metadata_info(self, log_level=20):
         if self._useless_features_in:
-            self._log(log_level, f'\tUseless Original Features (Count: {len(self._useless_features_in)}): {list(self._useless_features_in)}')
+            self._log(log_level, f"\tUseless Original Features (Count: {len(self._useless_features_in)}): {list(self._useless_features_in)}")
             # TODO: What about features with 1 unique value but also np.nan?
-            self._log(log_level, '\t\tThese features carry no predictive signal and should be manually investigated.')
-            self._log(log_level, '\t\tThis is typically a feature which has the same value for all rows.')
-            self._log(log_level, '\t\tThese features do not need to be present at inference time.')
+            self._log(log_level, "\t\tThese features carry no predictive signal and should be manually investigated.")
+            self._log(log_level, "\t\tThis is typically a feature which has the same value for all rows.")
+            self._log(log_level, "\t\tThese features do not need to be present at inference time.")
         if self._feature_metadata_in_unused.get_features():
             # TODO: Consider highlighting why a feature was unused
             #  (complex to implement, can check if was valid input to any generator in a generator group through feature chaining)
-            self._log(log_level, f'\tUnused Original Features (Count: {len(self._feature_metadata_in_unused.get_features())}): '
-                                 f'{self._feature_metadata_in_unused.get_features()}')
-            self._log(log_level, '\t\tThese features were not used to generate any of the output features. '
-                                 'Add a feature generator compatible with these features to utilize them.')
-            self._log(log_level, '\t\tFeatures can also be unused if they carry very little information, '
-                                 'such as being categorical but having almost entirely unique values or being duplicates of other features.')
-            self._log(log_level, '\t\tThese features do not need to be present at inference time.')
-            self._feature_metadata_in_unused.print_feature_metadata_full(self.log_prefix + '\t\t', log_level=log_level)
-        self._log(log_level-5, '\tTypes of features in original data (exact raw dtype, raw dtype):')
-        self._feature_metadata_in_real.print_feature_metadata_full(self.log_prefix + '\t\t', print_only_one_special=True, log_level=log_level-5)
+            self._log(
+                log_level,
+                f"\tUnused Original Features (Count: {len(self._feature_metadata_in_unused.get_features())}): "
+                f"{self._feature_metadata_in_unused.get_features()}",
+            )
+            self._log(
+                log_level,
+                "\t\tThese features were not used to generate any of the output features. "
+                "Add a feature generator compatible with these features to utilize them.",
+            )
+            self._log(
+                log_level,
+                "\t\tFeatures can also be unused if they carry very little information, "
+                "such as being categorical but having almost entirely unique values or being duplicates of other features.",
+            )
+            self._log(log_level, "\t\tThese features do not need to be present at inference time.")
+            self._feature_metadata_in_unused.print_feature_metadata_full(self.log_prefix + "\t\t", log_level=log_level)
+        self._log(log_level - 5, "\tTypes of features in original data (exact raw dtype, raw dtype):")
+        self._feature_metadata_in_real.print_feature_metadata_full(self.log_prefix + "\t\t", print_only_one_special=True, log_level=log_level - 5)
         super().print_feature_metadata_info(log_level=log_level)
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/rename.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         Name suffix to add to all output feature names.
     inplace : bool, default False
         If True, then the column names are renamed inplace without copying the input data.
         This will alter the input data outside of the scope of this function.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
+
     def __init__(self, name_prefix=None, name_suffix=None, inplace=False, **kwargs):
         super().__init__(**kwargs)
         self._name_prefix = name_prefix
         self._name_suffix = name_suffix
         self.inplace = inplace
         self._is_updated_name = None
 
@@ -65,10 +66,10 @@
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict()
 
     def _more_tags(self):
         return {
-            'feature_interactions': False,
-            'allow_post_generators': False,  # TODO: This might not be necessary anymore
+            "feature_interactions": False,
+            "allow_post_generators": False,  # TODO: This might not be necessary anymore
         }
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/text_ngram.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/text_ngram.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import traceback
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 from sklearn.feature_selection import SelectKBest, f_classif, f_regression
 
+from autogluon.common.features.types import S_IMAGE_BYTEARRAY, S_IMAGE_PATH, S_TEXT, S_TEXT_NGRAM
 from autogluon.common.utils.lite import disable_if_lite_mode
-from autogluon.common.features.types import S_IMAGE_PATH, S_IMAGE_BYTEARRAY, S_TEXT, S_TEXT_NGRAM
 
+from ..vectorizers import downscale_vectorizer, get_ngram_freq, vectorizer_auto_ml_default
 from .abstract import AbstractFeatureGenerator
-from ..vectorizers import get_ngram_freq, downscale_vectorizer, vectorizer_auto_ml_default
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add argument to define the text preprocessing logic
 # TODO: Add argument to output ngrams as a sparse matrix
 # TODO: Add HashingVectorizer support
@@ -44,109 +44,108 @@
         treating the ngrams as float32 values.
         ngram features will be removed in least frequent to most frequent order.
         Note: For vectorizer_strategy values other than 'combined', the resulting ngrams may use more than this value.
         It is recommended to only increase this value above 0.15 if confident that higher values will not result in out-of-memory errors.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
-    def __init__(self, vectorizer=None, vectorizer_strategy='combined', max_memory_ratio=0.15, prefilter_tokens=False, prefilter_token_count=100, **kwargs):
+
+    def __init__(self, vectorizer=None, vectorizer_strategy="combined", max_memory_ratio=0.15, prefilter_tokens=False, prefilter_token_count=100, **kwargs):
         super().__init__(**kwargs)
         self.vectorizers = []
         # TODO: 0.20 causes OOM error with 64 GB ram on NN with several datasets. LightGBM and CatBoost succeed
         # TODO: Finetune this, or find a better way to ensure stability
         # TODO: adjust max_memory_ratio correspondingly if prefilter_tokens==True
         self.max_memory_ratio = max_memory_ratio  # Ratio of maximum memory the output ngram features are allowed to use in dense int32 form.
 
         if vectorizer is None:
             self.vectorizer_default_raw = vectorizer_auto_ml_default()
         else:
             self.vectorizer_default_raw = vectorizer
 
-        if vectorizer_strategy not in ['combined', 'separate', 'both']:
+        if vectorizer_strategy not in ["combined", "separate", "both"]:
             raise ValueError(f"vectorizer_strategy must be one of {['combined', 'separate', 'both']}, but value is: {vectorizer_strategy}")
         self.vectorizer_strategy = vectorizer_strategy
         self.vectorizer_features = None
         self.prefilter_tokens = prefilter_tokens
         self.prefilter_token_count = prefilter_token_count
         self.token_mask = None
         self._feature_names_dict = dict()
 
     def _fit_transform(self, X: DataFrame, y: Series = None, problem_type: str = None, **kwargs) -> (DataFrame, dict):
         X_out = self._fit_transform_ngrams(X)
 
         if self.prefilter_tokens and self.prefilter_token_count >= X_out.shape[1]:
-            logger.warning('`prefilter_tokens` was enabled but `prefilter_token_count` larger than the vocabulary. Disabling `prefilter_tokens`.')
+            logger.warning("`prefilter_tokens` was enabled but `prefilter_token_count` larger than the vocabulary. Disabling `prefilter_tokens`.")
             self.prefilter_tokens = False
 
-        if self.prefilter_tokens and problem_type not in ['binary', 'regression']:
-            logger.warning('`prefilter_tokens` was enabled but invalid `problem_type`. Disabling `prefilter_tokens`.')
+        if self.prefilter_tokens and problem_type not in ["binary", "regression"]:
+            logger.warning("`prefilter_tokens` was enabled but invalid `problem_type`. Disabling `prefilter_tokens`.")
             self.prefilter_tokens = False
 
         if self.prefilter_tokens and y is None:
-            logger.warning('`prefilter_tokens` was enabled but `y` values were not provided to fit_transform. Disabling `prefilter_tokens`.')
+            logger.warning("`prefilter_tokens` was enabled but `y` values were not provided to fit_transform. Disabling `prefilter_tokens`.")
             self.prefilter_tokens = False
 
         if self.prefilter_tokens:
-            scoring_function = f_classif if problem_type == 'binary' else f_regression
+            scoring_function = f_classif if problem_type == "binary" else f_regression
             selector = SelectKBest(scoring_function, k=self.prefilter_token_count)
             selector.fit(X_out, y)
             self.token_mask = selector.get_support()
             X_out = X_out[X_out.columns[self.token_mask]]  # select the columns that are most correlated with y
 
-        type_family_groups_special = {
-            S_TEXT_NGRAM: list(X_out.columns)
-        }
+        type_family_groups_special = {S_TEXT_NGRAM: list(X_out.columns)}
         return X_out, type_family_groups_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
         # TODO: Optimize for inference
         if not self.features_in:
             return DataFrame(index=X.index)
         try:
             X_out = self._generate_ngrams(X=X)
             if self.prefilter_tokens:
                 X_out = X_out[X_out.columns[self.token_mask]]  # select the columns identified during training
         except Exception:
-            self._log(40, '\tError: OOM error during NLP feature transform, unrecoverable. Increase memory allocation or reduce data size to avoid this error.')
+            self._log(40, "\tError: OOM error during NLP feature transform, unrecoverable. Increase memory allocation or reduce data size to avoid this error.")
             raise
         return X_out
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict(required_special_types=[S_TEXT], invalid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY])
 
     def _fit_transform_ngrams(self, X):
         if not self.features_in:
             return DataFrame(index=X.index)
         features_nlp_to_remove = []
-        if self.vectorizer_strategy == 'combined':
-            self.vectorizer_features = ['__nlp__']
-        elif self.vectorizer_strategy == 'separate':
+        if self.vectorizer_strategy == "combined":
+            self.vectorizer_features = ["__nlp__"]
+        elif self.vectorizer_strategy == "separate":
             self.vectorizer_features = copy.deepcopy(self.features_in)
-        elif self.vectorizer_strategy == 'both':
-            self.vectorizer_features = ['__nlp__'] + copy.deepcopy(self.features_in)
+        elif self.vectorizer_strategy == "both":
+            self.vectorizer_features = ["__nlp__"] + copy.deepcopy(self.features_in)
         else:
             raise ValueError(f"vectorizer_strategy must be one of {['combined', 'separate', 'both']}, but value is: {self.vectorizer_features}")
-        self._log(20, f'Fitting {self.vectorizer_default_raw.__class__.__name__} for text features: ' + str(self.features_in), self.log_prefix + '\t')
-        self._log(15, f'{self.vectorizer_default_raw}', self.log_prefix + '\t\t')
+        self._log(20, f"Fitting {self.vectorizer_default_raw.__class__.__name__} for text features: " + str(self.features_in), self.log_prefix + "\t")
+        self._log(15, f"{self.vectorizer_default_raw}", self.log_prefix + "\t\t")
         for nlp_feature in self.vectorizer_features:
             # TODO: Preprocess text?
-            if nlp_feature == '__nlp__':  # Combine Text Fields
+            if nlp_feature == "__nlp__":  # Combine Text Fields
                 features_in_str = X[self.features_in].astype(str)
-                text_list = list(set(['. '.join(row) for row in features_in_str.values]))
+                text_list = list(set([". ".join(row) for row in features_in_str.values]))
             else:
                 text_list = list(X[nlp_feature].astype(str).drop_duplicates().values)
             vectorizer_raw = copy.deepcopy(self.vectorizer_default_raw)
             try:
                 # Don't use transform_matrix output because it may contain fewer rows due to drop_duplicates call.
                 vectorizer_fit, _ = self._train_vectorizer(text_list, vectorizer_raw)
-                self._log(20, f'{vectorizer_fit.__class__.__name__} fit with vocabulary size = {len(vectorizer_fit.vocabulary_)}', self.log_prefix + '\t')
+                self._log(20, f"{vectorizer_fit.__class__.__name__} fit with vocabulary size = {len(vectorizer_fit.vocabulary_)}", self.log_prefix + "\t")
             except ValueError:
-                self._log(30, f"Removing text_ngram feature due to error: '{nlp_feature}'", self.log_prefix + '\t')
-                if nlp_feature == '__nlp__':
+                self._log(30, f"Removing text_ngram feature due to error: '{nlp_feature}'", self.log_prefix + "\t")
+                if nlp_feature == "__nlp__":
                     self.vectorizer_features = []
                     features_nlp_to_remove = self.features_in
                     break
                 else:
                     features_nlp_to_remove.append(nlp_feature)
             else:
                 self.vectorizers.append(vectorizer_fit)
@@ -172,47 +171,54 @@
                         skip_nlp = True
                         break
                 else:
                     if nlp_failure_count >= 3:
                         skip_nlp = True
 
                 if skip_nlp:
-                    self._log(30, 'Warning: ngrams generation resulted in OOM error, removing ngrams features. '
-                                  'If you want to use ngrams for this problem, increase memory allocation for AutoGluon.', self.log_prefix + '\t')
+                    self._log(
+                        30,
+                        "Warning: ngrams generation resulted in OOM error, removing ngrams features. "
+                        "If you want to use ngrams for this problem, increase memory allocation for AutoGluon.",
+                        self.log_prefix + "\t",
+                    )
                     self._log(10, str(err))
                     self.vectorizers = []
                     self.features_in = []
                     keep_trying_nlp = False
                 else:
-                    self._log(20, 'Warning: ngrams generation resulted in OOM error, attempting to reduce ngram feature count. '
-                                  'If you want to optimally use ngrams for this problem, increase memory allocation for AutoGluon.', self.log_prefix + '\t')
+                    self._log(
+                        20,
+                        "Warning: ngrams generation resulted in OOM error, attempting to reduce ngram feature count. "
+                        "If you want to optimally use ngrams for this problem, increase memory allocation for AutoGluon.",
+                        self.log_prefix + "\t",
+                    )
                     self._log(10, str(err))
                     downsample_ratio = 0.25
         if X_text_ngram is None:
             X_text_ngram = DataFrame(index=X.index)
         return X_text_ngram
 
     def _generate_ngrams(self, X, downsample_ratio: int = None):
         X_nlp_features_combined = []
         for nlp_feature, vectorizer_fit in zip(self.vectorizer_features, self.vectorizers):
-            if nlp_feature == '__nlp__':
+            if nlp_feature == "__nlp__":
                 X_str = X.astype(str)
-                text_data = ['. '.join(row) for row in X_str.values]
+                text_data = [". ".join(row) for row in X_str.values]
             else:
                 nlp_feature_str = X[nlp_feature].astype(str)
                 text_data = nlp_feature_str.values
             transform_matrix = vectorizer_fit.transform(text_data)
 
             if not self._is_fit:
-                transform_matrix = self._adjust_vectorizer_memory_usage(transform_matrix=transform_matrix, text_data=text_data, vectorizer_fit=vectorizer_fit,
-                                                                        downsample_ratio=downsample_ratio)
+                transform_matrix = self._adjust_vectorizer_memory_usage(
+                    transform_matrix=transform_matrix, text_data=text_data, vectorizer_fit=vectorizer_fit, downsample_ratio=downsample_ratio
+                )
                 nlp_features_names = vectorizer_fit.get_feature_names_out()
-                nlp_features_names_final = np.array([f'{nlp_feature}.{x}' for x in nlp_features_names]
-                                                    + [f'{nlp_feature}._total_']
-                                                    )
+                nlp_features_names_final = np.array([f"{nlp_feature}.{x}" for x in nlp_features_names] + [f"{nlp_feature}._total_"])
                 self._feature_names_dict[nlp_feature] = nlp_features_names_final
 
             transform_array = transform_matrix.toarray()
             # This count could technically overflow in absurd situations. Consider making dtype a variable that is computed.
             nonzero_count = np.count_nonzero(transform_array, axis=1).astype(np.uint16)
             transform_array = np.append(transform_array, np.expand_dims(nonzero_count, axis=1), axis=1)
             X_nlp_features = pd.DataFrame(transform_array, columns=self._feature_names_dict[nlp_feature], index=X.index)  # TODO: Consider keeping sparse
@@ -229,33 +235,34 @@
         return X_nlp_features_combined
 
     # TODO: REMOVE NEED FOR text_data input!
     def _adjust_vectorizer_memory_usage(self, transform_matrix, text_data, vectorizer_fit, downsample_ratio: int = None):
         @disable_if_lite_mode(ret=downsample_ratio)
         def _adjust_per_memory_constraints(downsample_ratio: int):
             import psutil
+
             # This assumes that the ngrams eventually turn into int32/float32 downstream
             predicted_ngrams_memory_usage_bytes = len(text_data) * 4 * (transform_matrix.shape[1] + 1) + 80
             mem_avail = psutil.virtual_memory().available
             mem_rss = psutil.Process().memory_info().rss
             predicted_rss = mem_rss + predicted_ngrams_memory_usage_bytes
             predicted_percentage = predicted_rss / mem_avail
             if downsample_ratio is None:
                 if self.max_memory_ratio is not None and predicted_percentage > self.max_memory_ratio:
-                    self._log(30, 'Warning: Due to memory constraints, ngram feature count is being reduced. Allocate more memory to maximize model quality.')
+                    self._log(30, "Warning: Due to memory constraints, ngram feature count is being reduced. Allocate more memory to maximize model quality.")
                     return self.max_memory_ratio / predicted_percentage
 
         downsample_ratio = _adjust_per_memory_constraints(downsample_ratio)
 
         if downsample_ratio is not None:
             if (downsample_ratio >= 1) or (downsample_ratio <= 0):
-                raise ValueError(f'downsample_ratio must be >0 and <1, but downsample_ratio is {downsample_ratio}')
+                raise ValueError(f"downsample_ratio must be >0 and <1, but downsample_ratio is {downsample_ratio}")
             vocab_size = len(vectorizer_fit.vocabulary_)
             downsampled_vocab_size = int(np.floor(vocab_size * downsample_ratio))
-            self._log(20, f'Reducing Vectorizer vocab size from {vocab_size} to {downsampled_vocab_size} to avoid OOM error')
+            self._log(20, f"Reducing Vectorizer vocab size from {vocab_size} to {downsampled_vocab_size} to avoid OOM error")
             ngram_freq = get_ngram_freq(vectorizer=vectorizer_fit, transform_matrix=transform_matrix)
             downscale_vectorizer(vectorizer=vectorizer_fit, ngram_freq=ngram_freq, vocab_size=downsampled_vocab_size)
             # TODO: This doesn't have to be done twice, can update transform matrix based on new vocab instead of calling .transform
             #  If we have this functionality, simply update transform_matrix each time OOM occurs instead of re-calling .transform
             transform_matrix = vectorizer_fit.transform(text_data)
 
         return transform_matrix
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/generators/text_special.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/generators/text_special.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 
-from autogluon.common.features.types import S_IMAGE_PATH, S_IMAGE_BYTEARRAY, S_TEXT, S_TEXT_SPECIAL
+from autogluon.common.features.types import S_IMAGE_BYTEARRAY, S_IMAGE_PATH, S_TEXT, S_TEXT_SPECIAL
 
 from .abstract import AbstractFeatureGenerator
 from .binned import BinnedFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,50 +35,46 @@
     post_drop_duplicates : bool, default True
         Identical to AbstractFeatureGenerator's post_drop_duplicates, except it is defaulted to True instead of False.
         This helps to clean the output of this generator when symbols aren't present in the data.
     **kwargs :
         Refer to AbstractFeatureGenerator documentation for details on valid keyword arguments.
     """
 
-    def __init__(self, symbols: List[str] = None, min_occur_ratio=0.01, min_occur_offset=10, bin_features: bool = True, post_drop_duplicates: bool = True,
-                 **kwargs):
+    def __init__(
+        self, symbols: List[str] = None, min_occur_ratio=0.01, min_occur_offset=10, bin_features: bool = True, post_drop_duplicates: bool = True, **kwargs
+    ):
         super().__init__(post_drop_duplicates=post_drop_duplicates, **kwargs)
         if symbols is None:
-            symbols = ['!', '?', '@', '%', '$', '*', '&', '#', '^', '.', ':', ' ', '/', ';', '-', '=']
+            symbols = ["!", "?", "@", "%", "$", "*", "&", "#", "^", ".", ":", " ", "/", ";", "-", "="]
         self._symbols = symbols  # Symbols to generate count and ratio features for.
         self._symbols_per_feature = {}
         self._min_occur_ratio = min_occur_ratio
         self._min_occur_offset = min_occur_offset
         if bin_features:
             self._post_generators = [BinnedFeatureGenerator()] + self._post_generators
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> Tuple[DataFrame, dict]:
         self._symbols_per_feature = self._filter_symbols(X, self._symbols)
         self._feature_names_dict = self._compute_feature_names_dict()
         X_out = self._transform(X)
-        type_family_groups_special = {
-            S_TEXT_SPECIAL: list(X_out.columns)
-        }
+        type_family_groups_special = {S_TEXT_SPECIAL: list(X_out.columns)}
         return X_out, type_family_groups_special
 
     def _transform(self, X: DataFrame) -> DataFrame:
         return self._generate_features_text_special(X)
 
     def _compute_feature_names_dict(self) -> dict:
         feature_names = {}
         for feature in self.features_in:
             feature_names_cur = {}
-            for feature_name_base in ['char_count', 'word_count', 'capital_ratio', 'lower_ratio', 'digit_ratio', 'special_ratio']:
-                feature_names_cur[feature_name_base] = f'{feature}.{feature_name_base}'
+            for feature_name_base in ["char_count", "word_count", "capital_ratio", "lower_ratio", "digit_ratio", "special_ratio"]:
+                feature_names_cur[feature_name_base] = f"{feature}.{feature_name_base}"
             symbols = self._symbols_per_feature[feature]
             for symbol in symbols:
-                feature_names_cur[symbol] = {
-                    'count': f'{feature}.symbol_count.{symbol}',
-                    'ratio': f'{feature}.symbol_ratio.{symbol}'
-                }
+                feature_names_cur[symbol] = {"count": f"{feature}.symbol_count.{symbol}", "ratio": f"{feature}.symbol_ratio.{symbol}"}
             feature_names[feature] = feature_names_cur
         return feature_names
 
     @staticmethod
     def get_default_infer_features_in_args() -> dict:
         return dict(required_special_types=[S_TEXT], invalid_special_types=[S_IMAGE_PATH, S_IMAGE_BYTEARRAY])
 
@@ -97,41 +93,42 @@
                 symbols_per_feature[text_feature_name] = np.array(above_threshold_symbols)
         return symbols_per_feature
 
     def _generate_features_text_special(self, X: DataFrame) -> DataFrame:
         if self.features_in:
             X_text_special_combined = {}
             for text_feature in self.features_in:
-                X_text_special_combined = self._generate_text_special(X[text_feature], text_feature, symbols=self._symbols_per_feature[text_feature],
-                                                                      X_dict=X_text_special_combined)
+                X_text_special_combined = self._generate_text_special(
+                    X[text_feature], text_feature, symbols=self._symbols_per_feature[text_feature], X_dict=X_text_special_combined
+                )
             X_text_special_combined = pd.DataFrame(X_text_special_combined, index=X.index)
         else:
             X_text_special_combined = pd.DataFrame(index=X.index)
         return X_text_special_combined
 
     def _generate_text_special(self, X: Series, feature: str, symbols: list, X_dict: dict) -> dict:
         fn = self._feature_names_dict[feature]
         X_str = X.astype(str)
 
-        X_no_ws = X_str.str.replace(' ', '')
+        X_no_ws = X_str.str.replace(" ", "")
         X_no_ws_text_len = X_no_ws.str.len()
 
         char_count = X_str.str.len()
 
-        X_dict[fn['char_count']] = char_count.to_numpy(dtype=np.uint32)
-        X_dict[fn['word_count']] = X_str.str.split().str.len().to_numpy(dtype=np.uint32)
-        X_dict[fn['capital_ratio']] = X_no_ws.str.count('[A-Z]').divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
-        X_dict[fn['lower_ratio']] = X_no_ws.str.count('[a-z]').divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
-        X_dict[fn['digit_ratio']] = X_no_ws.str.count('[0-9]').divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
-        X_dict[fn['special_ratio']] = X_no_ws.str.count(r'[^\w]').divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
+        X_dict[fn["char_count"]] = char_count.to_numpy(dtype=np.uint32)
+        X_dict[fn["word_count"]] = X_str.str.split().str.len().to_numpy(dtype=np.uint32)
+        X_dict[fn["capital_ratio"]] = X_no_ws.str.count("[A-Z]").divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
+        X_dict[fn["lower_ratio"]] = X_no_ws.str.count("[a-z]").divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
+        X_dict[fn["digit_ratio"]] = X_no_ws.str.count("[0-9]").divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
+        X_dict[fn["special_ratio"]] = X_no_ws.str.count(r"[^\w]").divide(X_no_ws_text_len, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
 
         for symbol in symbols:
             symbol_count = X_str.str.count("\\" + symbol)
-            X_dict[fn[symbol]['count']] = symbol_count.to_numpy(dtype=np.uint32)
-            X_dict[fn[symbol]['ratio']] = symbol_count.divide(char_count, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
+            X_dict[fn[symbol]["count"]] = symbol_count.to_numpy(dtype=np.uint32)
+            X_dict[fn[symbol]["ratio"]] = symbol_count.divide(char_count, fill_value=0.0).fillna(0.0).to_numpy(dtype=np.float32)
 
         return X_dict
 
     def _remove_features_in(self, features: list):
         super()._remove_features_in(features)
         if self._symbols_per_feature:
             for feature in features:
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/utils.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 from pandas import DataFrame, Series
 
 logger = logging.getLogger(__name__)
 
 
-def clip_and_astype(df: DataFrame, columns: list = None, clip_min=0, clip_max=255, dtype: str = 'uint8') -> DataFrame:
+def clip_and_astype(df: DataFrame, columns: list = None, clip_min=0, clip_max=255, dtype: str = "uint8") -> DataFrame:
     """
     Clips columns in a DataFrame to min and max values, and then converts dtype.
 
     Parameters
     ----------
     df : DataFrame
         Input DataFrame.
@@ -46,8 +46,8 @@
     if min_val < 0:
         dtypes_to_check = [np.int8, np.int16, np.int32, np.int64]
     else:
         dtypes_to_check = [np.uint8, np.uint16, np.uint32, np.uint64]
     for dtype in [np.uint8, np.uint16, np.uint32, np.uint64]:
         if max_val <= np.iinfo(dtype).max and min_val >= np.iinfo(dtype).min:
             return dtype
-    raise ValueError(f'Value is not able to be represented by {dtypes_to_check[-1].__name__}. (min_val, max_val): ({min_val}, {max_val})')
+    raise ValueError(f"Value is not able to be represented by {dtypes_to_check[-1].__name__}. (min_val, max_val): ({min_val}, {max_val})")
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon/features/vectorizers.py` & `autogluon.features-0.8.1b20230623/src/autogluon/features/vectorizers.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/PKG-INFO` & `autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.1b20230622
+Version: 0.8.1b20230623
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.8.1b20230622/src/autogluon.features.egg-info/SOURCES.txt` & `autogluon.features-0.8.1b20230623/src/autogluon.features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

