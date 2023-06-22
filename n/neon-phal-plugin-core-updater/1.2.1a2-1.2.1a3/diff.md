# Comparing `tmp/neon-phal-plugin-core-updater-1.2.1a2.tar.gz` & `tmp/neon-phal-plugin-core-updater-1.2.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-core-updater-1.2.1a2.tar", last modified: Fri Jun 16 00:00:19 2023, max compression
+gzip compressed data, was "neon-phal-plugin-core-updater-1.2.1a3.tar", last modified: Thu Jun 22 21:41:20 2023, max compression
```

## Comparing `neon-phal-plugin-core-updater-1.2.1a2.tar` & `neon-phal-plugin-core-updater-1.2.1a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 00:00:19.000000 neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 00:00:19.826461 neon-phal-plugin-core-updater-1.2.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-16 00:00:12.000000 neon-phal-plugin-core-updater-1.2.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:41:20.189082 neon-phal-plugin-core-updater-1.2.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 21:41:16.000000 neon-phal-plugin-core-updater-1.2.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-22 21:41:20.189082 neon-phal-plugin-core-updater-1.2.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-22 21:41:16.000000 neon-phal-plugin-core-updater-1.2.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:41:20.189082 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-22 21:41:16.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:41:20.189082 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 21:41:20.000000 neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:41:20.189082 neon-phal-plugin-core-updater-1.2.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-22 21:41:16.000000 neon-phal-plugin-core-updater-1.2.1a3/setup.py
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/LICENSE.md` & `neon-phal-plugin-core-updater-1.2.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/PKG-INFO` & `neon-phal-plugin-core-updater-1.2.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.2.1a2
+Version: 1.2.1a3
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/README.md` & `neon-phal-plugin-core-updater-1.2.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater/__init__.py` & `neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,16 +94,20 @@
         """
         LOG.debug(f"Checking for update. current={self._installed_version}")
         update_alpha = message.data.get("include_prerelease")
         new_version = None
         latest_version = None
         if self.pypi_ref:
             releases = self._get_pypi_releases()
-        elif self.github_ref:
+        elif self.github_ref and update_alpha:
+            # Get list of latest GH Releases
             releases = self._get_github_releases()
+        elif self.github_ref:
+            # Only need the "latest" GH Release
+            releases = [self._get_latest_github_release()]
         else:
             LOG.error("No remote reference to check for updates")
             releases = []
 
         for release in releases:
             if 'a' in release and not update_alpha:
                 # Ignore an alpha release
@@ -115,15 +119,15 @@
             else:
                 latest_version = latest_version or release
                 new_version = new_version or release
 
         if new_version:
             LOG.info(f"Found newer version: {new_version}")
         if not latest_version and self.github_ref:
-            LOG.info("No release found; get 'latest'")
+            LOG.warning("No release found; get 'latest'")
             latest_version = self._get_latest_github_release()
         LOG.info(f"Got latest version: {latest_version}")
         if message:
             self.bus.emit(message.response({"new_version": new_version,
                                             "latest_version": latest_version,
                                             "installed_version": self._installed_version,
                                             "github_ref": self.github_ref,
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/neon_phal_plugin_core_updater.egg-info/PKG-INFO` & `neon-phal-plugin-core-updater-1.2.1a3/neon_phal_plugin_core_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.2.1a2
+Version: 1.2.1a3
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-core-updater-1.2.1a2/setup.py` & `neon-phal-plugin-core-updater-1.2.1a3/setup.py`

 * *Files identical despite different names*

