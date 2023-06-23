# Comparing `tmp/cpg-utils-ms-1.3.4.tar.gz` & `tmp/cpg-utils-ms-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-ms-1.3.4.tar", last modified: Thu Jun 22 21:21:55 2023, max compression
+gzip compressed data, was "cpg-utils-ms-1.3.5.tar", last modified: Fri Jun 23 19:49:23 2023, max compression
```

## Comparing `cpg-utils-ms-1.3.4.tar` & `cpg-utils-ms-1.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.842728 cpg-utils-ms-1.3.4/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/deploy_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/cpg_utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 21:21:55.000000 cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:21:55.846728 cpg-utils-ms-1.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-22 21:20:14.000000 cpg-utils-ms-1.3.4/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/deploy_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/cpg_utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-23 19:49:23.000000 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 19:49:23.000000 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:49:23.000000 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 19:49:23.000000 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 19:49:23.000000 cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:49:23.285916 cpg-utils-ms-1.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/test_cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-23 19:47:33.000000 cpg-utils-ms-1.3.5/test/test_storage.py
```

### Comparing `cpg-utils-ms-1.3.4/LICENSE` & `cpg-utils-ms-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/PKG-INFO` & `cpg-utils-ms-1.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils-ms
-Version: 1.3.4
+Version: 1.3.5
 Summary: Library of convenience functions specific to the CPG (MS version)
 Home-page: https://github.com/gregsmi/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-ms-1.3.4/README.md` & `cpg-utils-ms-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/__init__.py` & `cpg-utils-ms-1.3.5/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/auth.py` & `cpg-utils-ms-1.3.5/cpg_utils/auth.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/cloud.py` & `cpg-utils-ms-1.3.5/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-ms-1.3.5/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/config.py` & `cpg-utils-ms-1.3.5/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/creds.py` & `cpg-utils-ms-1.3.5/cpg_utils/creds.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/deploy_config.py` & `cpg-utils-ms-1.3.5/cpg_utils/deploy_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/git.py` & `cpg-utils-ms-1.3.5/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/hail_batch.py` & `cpg-utils-ms-1.3.5/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/secrets.py` & `cpg-utils-ms-1.3.5/cpg_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/slack.py` & `cpg-utils-ms-1.3.5/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/cpg_utils/storage.py` & `cpg-utils-ms-1.3.5/cpg_utils/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         if cloud_type == "azure":
             return DataManagerAzure()
         assert cloud_type == "gcp"
         return DataManagerGCP()
 
     @abstractmethod
     def get_global_bucket_url(self, bucket_type: str) -> str:
-        """Return deployment-level bucket URL with Hail-style scheme ("gs:" or "hail-az:")."""
+        """Return deployment-level bucket URL with Hail-style scheme ("gs:" or "https:")."""
 
     @abstractmethod
     def get_dataset_bucket_url(self, dataset: str, bucket_type: str) -> str:
-        """Build dataset-specific bucket URL with Hail-style scheme ("gs:" or "hail-az:")."""
+        """Build dataset-specific bucket URL with Hail-style scheme ("gs:" or "https:")."""
 
 
 class DataManagerGCP(DataManager):
     """GCP Storage wrapper for building dataset-related cloud URLs."""
 
     def get_global_bucket_url(self, bucket_type: str) -> str:
         """Return deployment-level bucket URLfor GCP ("gs:")."""
@@ -53,20 +53,20 @@
                 raise ValueError(f"No such dataset in server config: {dataset}")
             account = server_config[dataset]["projectId"]
         else: # Otherwise use the base deployment storage account.
             account = get_deploy_config().deployment_name
         return f"{account}sa"
 
     def get_global_bucket_url(self, bucket_type: str) -> str:
-        """Return deployment-level bucket URL with Hail-style scheme ("gs:" or "hail-az:")."""
-        return f"hail-az://{self.get_storage_account()}/{bucket_type}"
+        """Return deployment-level bucket URL for Azure ("https:")."""
+        return f"https://{self.get_storage_account()}.blob.core.windows.net/{bucket_type}"
 
     def get_dataset_bucket_url(self, dataset: str, bucket_type: str) -> str:
-        """Build dataset-specific Hail-style bucket URL for Azure ("hail-az:")."""
-        return f"hail-az://{self.get_storage_account(dataset)}/{bucket_type}"
+        """Build dataset-specific Hail-style bucket URL for Azure ("https:")."""
+        return f"https://{self.get_storage_account(dataset)}.blob.core.windows.net/{bucket_type}"
 
 
 def get_data_manager() -> DataManager:
     global data_manager
     if data_manager is None:
         data_manager = DataManager.get_data_manager()
     return data_manager
@@ -74,20 +74,20 @@
 
 def clear_data_manager() -> None:
     global data_manager
     data_manager = None
 
 
 def get_global_bucket_url(bucket_type: str) -> str:
-    """Return deployment-level bucket URL with Hail-style scheme ("gs:" or "hail-az:")."""
+    """Return deployment-level bucket URL with Hail-style scheme ("gs:" or "https:")."""
     return get_data_manager().get_global_bucket_url(bucket_type)
 
 
 def get_dataset_bucket_url(dataset: str, bucket_type: str) -> str:
-    """Return dataset-specific bucket URL with Hail-style scheme ("gs:" or "hail-az:")."""
+    """Return dataset-specific bucket URL with Hail-style scheme ("gs:" or "https:")."""
     return get_data_manager().get_dataset_bucket_url(dataset, bucket_type)
 
 
 def get_dataset_bucket_config(dataset: str, access_level: str) -> Dict[str, str]:
     """Return full set of dataset-specific bucket URLs for config."""
     assert access_level == "main" or access_level == "test"
     data_manager = get_data_manager()
```

### Comparing `cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/PKG-INFO` & `cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils-ms
-Version: 1.3.4
+Version: 1.3.5
 Summary: Library of convenience functions specific to the CPG (MS version)
 Home-page: https://github.com/gregsmi/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-ms-1.3.4/cpg_utils_ms.egg-info/SOURCES.txt` & `cpg-utils-ms-1.3.5/cpg_utils_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/pyproject.toml` & `cpg-utils-ms-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/setup.py` & `cpg-utils-ms-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='cpg-utils-ms',
     # This tag is automatically updated by bumpversion
-    version='1.3.4',
+    version='1.3.5',
     description='Library of convenience functions specific to the CPG (MS version)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/gregsmi/cpg-utils',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `cpg-utils-ms-1.3.4/test/test_auth.py` & `cpg-utils-ms-1.3.5/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/test/test_cloudpath_hail_az.py` & `cpg-utils-ms-1.3.5/test/test_cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/test/test_config.py` & `cpg-utils-ms-1.3.5/test/test_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 
 
 def test_config_storage(monkeypatch, test_resources_path):
     set_config_paths([os.path.join(test_resources_path, "config_01.toml")])
     monkeypatch.delenv("CPG_DEPLOY_CONFIG", raising=False)
     set_deploy_config_from_env()
 
-    assert dataset_path("one", "web") == "hail-az://sevgen002sa/test-web/one"
-    assert dataset_path("two", "analysis", "rgp") == "hail-az://raregen001sa/test-analysis/two"
-    assert output_path("three") == "hail-az://sevgen002sa/test/gregsmi/three"
-    assert remote_tmpdir() == "hail-az://sevgen002sa/hail/batch-tmp"
+    assert dataset_path("one", "web") == "https://sevgen002sa.blob.core.windows.net/test-web/one"
+    assert dataset_path("two", "analysis", "rgp") == "https://raregen001sa.blob.core.windows.net/test-analysis/two"
+    assert output_path("three") == "https://sevgen002sa.blob.core.windows.net/test/gregsmi/three"
+    assert remote_tmpdir() == "https://sevgen002sa.blob.core.windows.net/hail/batch-tmp"
     assert web_url("four") == "https://test-web-azcpg001.azurewebsites.net/severalgenomes/four"
-    assert reference_path("genome_build") == HailAzureBlobPath("hail-az://cpgar01/reference/GRCh38")
-    assert reference_path("seqr/combined_reference") == HailAzureBlobPath("hail-az://cpgar01/reference/combined_reference_data_grch38.ht")
+    assert reference_path("genome_build") == HailAzureBlobPath("https://cpgar01.blob.core.windows.net/reference/GRCh38")
+    assert reference_path("seqr/combined_reference") == HailAzureBlobPath("https://cpgar01.blob.core.windows.net/reference/combined_reference_data_grch38.ht")
     assert image_path("vep") == "ar-docker.pkg.dev/cpg-common/images/vep:105.0"
```

### Comparing `cpg-utils-ms-1.3.4/test/test_secrets.py` & `cpg-utils-ms-1.3.5/test/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-ms-1.3.4/test/test_storage.py` & `cpg-utils-ms-1.3.5/test/test_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,9 +26,9 @@
     set_deploy_config_from_env()
     clear_data_manager()
 
     with pytest.raises(ValueError) as e:
         get_dataset_bucket_url("dataset0", "main-read")
         assert "No such dataset in server config" in str(e.value)
 
-    assert get_dataset_bucket_url("dataset1", "test") == "hail-az://dataset1_idsa/test"
-    assert get_global_bucket_url("global") == "hail-az://cpgsa/global"
+    assert get_dataset_bucket_url("dataset1", "test") == "https://dataset1_idsa.blob.core.windows.net/test"
+    assert get_global_bucket_url("global") == "https://cpgsa.blob.core.windows.net/global"
```

