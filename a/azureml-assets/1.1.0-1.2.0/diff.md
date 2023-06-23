# Comparing `tmp/azureml-assets-1.1.0.tar.gz` & `tmp/azureml-assets-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.1.0.tar", last modified: Thu Jun  8 19:23:09 2023, max compression
+gzip compressed data, was "azureml-assets-1.2.0.tar", last modified: Fri Jun 23 15:38:33 2023, max compression
```

## Comparing `azureml-assets-1.1.0.tar` & `azureml-assets-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.764191 azureml-assets-1.1.0/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.764191 azureml-assets-1.1.0/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      669 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36250 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8088 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.768191 azureml-assets-1.1.0/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6517 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.768191 azureml-assets-1.1.0/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10380 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.385058 azureml-assets-1.2.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6521 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6897 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16581 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/setup.py
```

### Comparing `azureml-assets-1.1.0/PKG-INFO` & `azureml-assets-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.1.0
+Version: 1.2.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.1.0/azureml/assets/__init__.py` & `azureml-assets-1.2.0/azureml/assets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 )
 from .deployment_config import (
     DeploymentConfig,
 )
 from .update_assets import (
     pin_env_files,
     release_tag_exists,
+    get_latest_release_tag_version,
     update_asset,
     update_assets,
 )
+from .environment.pin_image_versions import get_manifest
 from .update_spec import create_template_data, update as update_spec
 from .validate_assets import validate_assets
```

### Comparing `azureml-assets-1.1.0/azureml/assets/asset_utils.py` & `azureml-assets-1.2.0/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/config.py` & `azureml-assets-1.2.0/azureml/assets/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -794,14 +794,18 @@
         # Reject auto-versioned assets
         if self.version is None or other.version is None:
             raise ValueError("Cannot compare auto-versioned assets")
 
         # Compare versions using packaging's version object
         return version.parse(self.version) < version.parse(other.version)
 
+    def __hash__(self) -> int:
+        """Hash an AssetConfig object."""
+        return hash((self.type.value, self.name, self.version))
+
     def _validate(self):
         """Validate asset config.
 
         Raises:
             ValidationException: If validation fails.
         """
         Config._validate_enum('type', self._type, AssetType, True)
```

### Comparing `azureml-assets-1.1.0/azureml/assets/deployment_config.py` & `azureml-assets-1.2.0/azureml/assets/deployment_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,14 +181,26 @@
         Returns:
             DeploymentConfig: Deployment config.
         """
         with open(deployment_config) as fp:
             config = YAML().load(fp)
             return DeploymentConfigSchema().load(config)
 
+    def should_create(self, asset_type: assets.AssetType, asset_name: str) -> bool:
+        """Determine if an asset should be created.
+
+        Args:
+            asset_type (assets.AssetType): Asset type.
+            asset_name (str): Asset name.
+
+        Returns:
+            bool: True if the asset should be created.
+        """
+        return any(n in {"*", asset_name} for n in self.create.get(asset_type, []))
+
 
 class TagsSchema(Schema):
     """Tags schema."""
 
     add = fields.Dict(fields.Str(), fields.Str())
     replace = fields.Dict(fields.Str(), fields.Str())
     delete = fields.List(fields.Str())
```

### Comparing `azureml-assets-1.1.0/azureml/assets/environment/build.py` & `azureml-assets-1.2.0/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.2.0/azureml/assets/environment/pin_image_versions.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,33 @@
 
     Returns:
         HTTPResponse: Response from urlopen.
     """
     return urlopen(request)
 
 
+def get_manifest(tag: str, hostname: str, repo: str):
+    """Retrieve manifest for an image.
+
+    Args:
+        tag (str): Tag for the image.
+        hostname (str): Hostname of the container registry.
+        repo (str): Repository of the image.
+
+    Returns:
+        HTTPResponse: Response from _urlopen_with_retries.
+    """
+    encoded_tag = urllib.parse.quote(tag, safe="")
+    request = Request(f"https://{hostname}/v2/{repo}/manifests/{encoded_tag}",
+                      method="HEAD",
+                      headers={'Accept': "application/vnd.docker.distribution.manifest.v2+json"})
+
+    return _urlopen_with_retries(request)
+
+
 def _get_latest_tag_or_digest(image: str, tags: List[str]) -> Tuple[str, str]:
     """Get latest tag or digest for an image.
 
     Args:
         image (str): Full image name, including hostname of the container registry.
         tags (List[str]): List of tags for the image.
 
@@ -49,21 +68,16 @@
     (hostname, repo) = image.split("/", 1)
 
     # Find another tag corresponding to latest
     latest_tag = None
     latest_digest = None
     for tag in tags:
         # Retrieve digest
-        encoded_tag = urllib.parse.quote(tag, safe="")
-        request = Request(f"https://{hostname}/v2/{repo}/manifests/{encoded_tag}",
-                          method="HEAD",
-                          headers={'Accept': "application/vnd.docker.distribution.manifest.v2+json"})
-
         try:
-            response = _urlopen_with_retries(request)
+            response = get_manifest(tag, hostname, repo)
         except Exception as e:
             raise Exception(f"Failed to retrieve manifest for {repo}:{tag}: {e}")
 
         digest = response.info()['Docker-Content-Digest']
 
         if tag == LATEST_TAG:
             # Store latest digest for comparison
@@ -111,15 +125,15 @@
         if LATEST_TAG not in tags:
             raise Exception(f"{image} does not have a {LATEST_TAG} tag")
 
         # Insert latest at the beginning to ensure we get its digest first
         tags_sorted.insert(0, LATEST_TAG)
 
         # Find another tag corresponding to latest, or default to digest
-        latest_tag, latest_digest = _get_latest_tag_or_digest(image, tags)
+        latest_tag, latest_digest = _get_latest_tag_or_digest(image, tags_sorted)
 
     # Return tag or digest
     if latest_tag is not None:
         return f":{latest_tag}"
     else:
         logger.log_warning(f"Using digest for {image} because a non-{LATEST_TAG} was not found")
         return f"@{latest_digest}"
```

### Comparing `azureml-assets-1.1.0/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.2.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.2.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.2.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.2.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/model/utils.py` & `azureml-assets-1.2.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/tag_released_assets.py` & `azureml-assets-1.2.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/update_assets.py` & `azureml-assets-1.2.0/azureml/assets/update_assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,39 @@
         bool: True if the tag exists, False otherwise
     """
     # Check git repo for version-specific tag
     repo = Repo(release_directory_root)
     return asset_config.full_name in repo.tags
 
 
+def get_latest_release_tag_version(asset_config: assets.AssetConfig, release_directory_root: Path) -> str:
+    """Check repo to see if an asset's previous version was released if a latest tag exists.
+
+    Args:
+        asset_config (assets.AssetConfig): Asset config
+        release_directory_root (Path): Release branch location
+
+    Returns:
+        str: Latest version found, or None if asset is not an environment or no tags not found
+    """
+    repo = Repo(release_directory_root)
+    tags = [t for t in repo.tags if t.name.startswith(f"{asset_config.partial_name}/")]
+
+    if not tags:
+        # No releases
+        return None
+
+    # Get the latest tag
+    ordered_tags = sorted(tags, key=lambda t: t.commit.authored_datetime)
+    latest_tag = ordered_tags[-1].name
+    _, _, latest_version = assets.AssetConfig.parse_full_name(latest_tag)
+
+    return latest_version
+
+
 def update_asset(asset_config: assets.AssetConfig,
                  release_directory_root: Path,
                  copy_only: bool,
                  skip_unreleased: bool,
                  output_directory_root: Path = None) -> str:
     """Update asset to prepare for release.
```

### Comparing `azureml-assets-1.1.0/azureml/assets/update_spec.py` & `azureml-assets-1.2.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/util/__init__.py` & `azureml-assets-1.2.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/util/logger.py` & `azureml-assets-1.2.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/util/template.py` & `azureml-assets-1.2.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/util/util.py` & `azureml-assets-1.2.0/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/azureml/assets/validate_assets.py` & `azureml-assets-1.2.0/azureml/assets/validate_assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 import azureml.assets as assets
 import azureml.assets.util as util
 from azureml.assets import PublishLocation, PublishVisibility
 from azureml.assets.config import ValidationException
 from azureml.assets.util import logger
 
-ERROR_TEMPLATE = "Validation of {asset} failed: {error}"
-WARNING_TEMPLATE = "Warning during validation of {asset}: {warning}"
+ERROR_TEMPLATE = "Validation of {file} failed: {error}"
+WARNING_TEMPLATE = "Warning during validation of {file}: {warning}"
 
 # Common naming convention
 NAMING_CONVENTION_URL = "https://github.com/Azure/azureml-assets/wiki/Asset-naming-convention"
 INVALID_STRINGS = ["microsoft", ["azureml", "azure"], "aml"]
 COMMON_NAME_PATTERN = re.compile(r"^[a-z][a-z0-9_.-]{0,254}$")
 
 # Asset config convention
@@ -50,36 +50,36 @@
     f"(?:-(?:{GPU_DRIVER_VERSION}|gpu))?",
 ]))
 
 # Image naming convention
 IMAGE_NAME_PATTERN = re.compile(r"^azureml/curated/(.+)")
 
 
-def _log_error(asset_config: assets.AssetConfig, error: str) -> None:
+def _log_error(file: Path, error: str) -> None:
     """Log error.
 
     Args:
-        asset_config (AssetConfig): Asset config.
+        file (Path): File with an issue.
         error (str): Error message.
     """
     logger.log_error(ERROR_TEMPLATE.format(
-        asset=asset_config.spec_with_path,
+        file=file.as_posix(),
         error=error
     ))
 
 
-def _log_warning(asset_config: assets.AssetConfig, warning: str) -> None:
+def _log_warning(file: Path, warning: str) -> None:
     """Log warning.
 
     Args:
-        asset_config (AssetConfig): Asset config.
+        file (Path): File with an issue.
         warning (str): Warning message.
     """
     logger.log_warning(WARNING_TEMPLATE.format(
-        asset=asset_config.spec_with_path,
+        file=file.as_posix(),
         warning=warning
     ))
 
 
 def validate_environment_name(asset_config: assets.AssetConfig) -> int:
     """Validate environment name.
 
@@ -90,56 +90,60 @@
         int: Number of errors.
     """
     error_count = 0
     asset_name = asset_config.name
 
     # Check for invalid characters
     if not ENVIRONMENT_NAME_PATTERN.match(asset_name):
-        _log_error(asset_config, "Name contains invalid characters")
+        _log_error(asset_config.file_name_with_path, "Name contains invalid characters")
         error_count += 1
 
     # Check for invalid strings
     for invalid_string in INVALID_ENVIRONMENT_STRINGS:
         if invalid_string in asset_name:
-            _log_error(asset_config, f"Name '{asset_name}' contains invalid string '{invalid_string}'")
+            _log_error(asset_config.file_name_with_path,
+                       f"Name '{asset_name}' contains invalid string '{invalid_string}'")
             error_count += 1
 
     # Check for missing frameworks and version
     frameworks_found = [f for f in FRAMEWORKS if f in asset_name]
     if len(frameworks_found) == 0:
-        _log_warning(asset_config, f"Name '{asset_name}' is missing framework")
+        _log_warning(asset_config.file_name_with_path, f"Name '{asset_name}' is missing framework")
     else:
         # Check framework version
         if not FRAMEWORK_VERSION_PATTERN.search(asset_name):
-            _log_error(asset_config, f"Name '{asset_name}' is missing framework version")
+            _log_error(asset_config.file_name_with_path, f"Name '{asset_name}' is missing framework version")
             error_count += 1
 
     # Check operating system and version
     if (OPERATING_SYSTEM_PATTERN.search(asset_name) and
             not OPERATING_SYSTEM_VERSION_PATTERN.search(asset_name)):
-        _log_error(asset_config, f"Name '{asset_name}' is missing operating system version")
+        _log_error(asset_config.file_name_with_path,
+                   f"Name '{asset_name}' is missing operating system version")
         error_count += 1
 
     # Check python version
     if PYTHON_VERSION_PATTERN.search(asset_name):
-        _log_warning(asset_config, f"Name '{asset_name}' should only contain Python version if absolutely necessary")
+        _log_warning(asset_config.file_name_with_path,
+                     f"Name '{asset_name}' should only contain Python version if absolutely necessary")
 
     # Check GPU driver and version
     gpu_drivers_found = [f for f in GPU_DRIVERS if f in asset_name]
     if gpu_drivers_found:
         if not GPU_DRIVER_VERSION_PATTERN.search(asset_name):
-            _log_error(asset_config, f"Name '{asset_name}' is missing GPU driver version")
+            _log_error(asset_config.file_name_with_path, f"Name '{asset_name}' is missing GPU driver version")
             error_count += 1
         if "gpu" in asset_name:
-            _log_error(asset_config, f"Name '{asset_name}' should not contain both GPU driver and 'gpu'")
+            _log_error(asset_config.file_name_with_path,
+                       f"Name '{asset_name}' should not contain both GPU driver and 'gpu'")
             error_count += 1
 
     # Check for ordering
     if frameworks_found and not ENVIRONMENT_NAME_FULL_PATTERN.search(asset_name):
-        _log_error(asset_config, f"Name '{asset_name}' elements are out of order")
+        _log_error(asset_config.file_name_with_path, f"Name '{asset_name}' elements are out of order")
         error_count += 1
 
     return error_count
 
 
 def validate_image_publishing(asset_config: assets.AssetConfig,
                               environment_config: assets.EnvironmentConfig = None) -> int:
@@ -156,43 +160,43 @@
     asset_name = asset_config.name
     environment_config = environment_config or asset_config.extra_config_as_object()
 
     # Check image name
     if (match := IMAGE_NAME_PATTERN.match(environment_config.image_name)) is not None:
         # Ensure image name matches environment name
         if match.group(1) != asset_name:
-            _log_error(asset_config,
+            _log_error(environment_config.file_name_with_path,
                        f"Image name '{environment_config.image_name}' should be 'azureml/curated/{asset_name}'")
             error_count += 1
     else:
-        _log_error(asset_config,
+        _log_error(environment_config.file_name_with_path,
                    f"Image name '{environment_config.image_name}' should match pattern azureml/curated/<env_name>")
         error_count += 1
 
     # Check build context
     if not environment_config.context_dir_with_path.exists():
-        _log_error(asset_config,
+        _log_error(environment_config.file_name_with_path,
                    f"Build context directory '{environment_config.context_dir}' not found")
         error_count += 1
     if not environment_config.dockerfile_with_path.exists():
-        _log_error(asset_config,
+        _log_error(environment_config.file_name_with_path,
                    f"Dockerfile '{environment_config.dockerfile}' not found")
         error_count += 1
 
     # Check publishing info
     if not environment_config.publish_enabled:
-        _log_error(asset_config, "Image publishing information is not specified")
+        _log_error(environment_config.file_name_with_path, "Image publishing information is not specified")
         error_count += 1
 
     # Check publishing details
     if environment_config.publish_location != PublishLocation.MCR:
-        _log_error(asset_config, "Image publishing location should be 'mcr'")
+        _log_error(environment_config.file_name_with_path, "Image publishing location should be 'mcr'")
         error_count += 1
     if environment_config.publish_visibility != PublishVisibility.PUBLIC:
-        _log_warning(asset_config, "Image publishing visibility should be 'public'")
+        _log_warning(environment_config.file_name_with_path, "Image publishing visibility should be 'public'")
 
     return error_count
 
 
 def validate_name(asset_config: assets.AssetConfig) -> int:
     """Validate asset name.
 
@@ -203,27 +207,28 @@
         int: Number of errors.
     """
     error_count = 0
     asset_name = asset_config.name
 
     # Check against generic naming pattern
     if not COMMON_NAME_PATTERN.match(asset_name):
-        _log_error(asset_config, f"Name '{asset_name}' contains invalid characters")
+        _log_error(asset_config.file_name_with_path, f"Name '{asset_name}' contains invalid characters")
         error_count += 1
 
     # Check for invalid strings
     invalid_strings = INVALID_STRINGS + [asset_config.type.value]
     for string_group in invalid_strings:
         # Coerce into a list
         string_group_list = string_group if isinstance(string_group, list) else [string_group]
 
         for invalid_string in string_group_list:
             if invalid_string in asset_name:
                 # Complain only about the first matching string
-                _log_error(asset_config, f"Name '{asset_name}' contains invalid string '{invalid_string}'")
+                _log_error(asset_config.file_name_with_path,
+                           f"Name '{asset_name}' contains invalid string '{invalid_string}'")
                 error_count += 1
                 break
 
     # Validate environment name
     if asset_config.type == assets.AssetType.ENVIRONMENT:
         error_count += validate_environment_name(asset_config)
 
@@ -236,15 +241,15 @@
     Args:
         asset_config (AssetConfig): Asset config.
 
     Returns:
         int: Number of errors.
     """
     if not asset_config.categories:
-        _log_error(asset_config, "Categories not found")
+        _log_error(asset_config.file_name_with_path, "Categories not found")
         return 1
     return 0
 
 
 def validate_assets(input_dirs: List[Path],
                     asset_config_filename: str,
                     changed_files: List[Path] = None,
@@ -263,79 +268,100 @@
 
     Raises:
         ValidationException: If validation fails.
 
     Returns:
         bool: True if assets were successfully validated, otherwise False.
     """
+    # Gather list of just changed assets, for later filtering
+    changed_assets = util.find_asset_config_files(input_dirs, asset_config_filename, changed_files) if changed_files else None  # noqa: E501
+
     # Find assets under input dirs
     asset_count = 0
     error_count = 0
     asset_dirs = defaultdict(list)
     image_names = defaultdict(list)
-    for asset_config_path in util.find_asset_config_files(input_dirs, asset_config_filename, changed_files):
+    for asset_config_path in util.find_asset_config_files(input_dirs, asset_config_filename):
         asset_count += 1
+        # Errors only "count" if changed_files was None or the asset was changed
+        validate_this = changed_assets is None or asset_config_path in changed_assets
+
         # Load config
         try:
             asset_config = assets.AssetConfig(asset_config_path)
         except Exception as e:
-            logger.log_error(f"Validation of {asset_config_path} failed: {e}")
-            error_count += 1
+            if validate_this:
+                _log_error(asset_config_path, e)
+                error_count += 1
+            else:
+                _log_warning(asset_config_path, e)
             continue
-        asset_dirs[f"{asset_config.type.value} {asset_config.name}"].append(asset_config_path)
 
-        # Validate name
-        if check_names:
-            error_count += validate_name(asset_config)
-
-        # Validate categories
-        if check_categories:
-            error_count += validate_categories(asset_config)
+        # Populate dictionary of asset names to asset config paths
+        asset_dirs[f"{asset_config.type.value} {asset_config.name}"].append(asset_config_path)
 
-        # Validate specific asset types
+        # Populate dictionary of image names to asset config paths
+        environment_config = None
         if asset_config.type == assets.AssetType.ENVIRONMENT:
             try:
                 environment_config = asset_config.extra_config_as_object()
 
                 # Store fully qualified image name
                 image_name = environment_config.image_name
                 if environment_config.publish_location:
                     image_name = f"{environment_config.publish_location.value}/{image_name}"
                 image_names[image_name].append(asset_config.file_path)
+            except Exception as e:
+                if validate_this:
+                    _log_error(environment_config.file_name_with_path, e)
+                    error_count += 1
+                else:
+                    _log_warning(environment_config.file_name_with_path, e)
+
+        # Checks for changed assets only, or all assets if changed_files was None
+        if validate_this:
+            # Validate name
+            if check_names:
+                error_count += validate_name(asset_config)
+
+            # Validate categories
+            if check_categories:
+                error_count += validate_categories(asset_config)
 
-                # Check image name
+            # Validate specific asset types
+            if environment_config is not None:
                 if check_images:
+                    # Check image name
                     error_count += validate_image_publishing(asset_config, environment_config)
-            except Exception as e:
-                logger.log_error(f"Validation of {asset_config.extra_config_with_path} failed: {e}")
-                error_count += 1
 
-        # Validate spec
-        try:
-            spec = asset_config.spec_as_object()
+            # Validate spec
+            try:
+                spec = asset_config.spec_as_object()
 
-            # Ensure name and version aren't inconsistent
-            if not assets.Config._contains_template(spec.name) and asset_config.name != spec.name:
-                raise ValidationException(f"Asset and spec name mismatch: {asset_config.name} != {spec.name}")
-            if not assets.Config._contains_template(spec.version) and asset_config.version != spec.version:
-                raise ValidationException(f"Asset and spec version mismatch: {asset_config.version} != {spec.version}")
-        except Exception as e:
-            logger.log_error(f"Validation of {asset_config.spec_with_path} failed: {e}")
-            error_count += 1
+                # Ensure name and version aren't inconsistent
+                if not assets.Config._contains_template(spec.name) and asset_config.name != spec.name:
+                    raise ValidationException(f"Asset and spec name mismatch: {asset_config.name} != {spec.name}")
+                if not assets.Config._contains_template(spec.version) and asset_config.version != spec.version:
+                    raise ValidationException(f"Asset and spec version mismatch: {asset_config.version} != {spec.version}")  # noqa: E501
+            except Exception as e:
+                _log_error(spec.file_name_with_path, e)
+                error_count += 1
 
     # Ensure unique assets
     for type_and_name, dirs in asset_dirs.items():
         if len(dirs) > 1:
-            logger.log_error(f"{type_and_name} found in multiple asset YAMLs: {dirs}")
+            dirs_str = [d.as_posix() for d in dirs]
+            logger.log_error(f"{type_and_name} found in multiple asset YAMLs: {dirs_str}")
             error_count += 1
 
     # Ensure unique image names
     for image_name, dirs in image_names.items():
         if len(dirs) > 1:
-            logger.log_error(f"{image_name} found in multiple assets: {dirs}")
+            dirs_str = [d.as_posix() for d in dirs]
+            logger.log_error(f"{image_name} found in multiple assets: {dirs_str}")
             error_count += 1
 
     logger.print(f"Found {error_count} error(s) in {asset_count} asset(s)")
     return error_count == 0
 
 
 if __name__ == '__main__':
```

### Comparing `azureml-assets-1.1.0/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.2.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.1.0
+Version: 1.2.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.1.0/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.2.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.1.0/setup.py` & `azureml-assets-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.1.0",
+   version="1.2.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

