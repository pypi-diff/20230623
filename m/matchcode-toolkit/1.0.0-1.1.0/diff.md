# Comparing `tmp/matchcode-toolkit-1.0.0.tar.gz` & `tmp/matchcode-toolkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchcode-toolkit-1.0.0.tar", last modified: Tue Jun  6 00:49:10 2023, max compression
+gzip compressed data, was "matchcode-toolkit-1.1.0.tar", last modified: Fri Jun 23 01:01:05 2023, max compression
```

## Comparing `matchcode-toolkit-1.0.0.tar` & `matchcode-toolkit-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/
--rw-rw-r--   0 jono      (1000) jono      (1000)      104 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/AUTHORS.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)       69 2023-06-06 00:27:30.000000 matchcode-toolkit-1.0.0/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      217 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/NOTICE
--rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2516 2023-06-06 00:27:30.000000 matchcode-toolkit-1.0.0/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/apache-2.0.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)      923 2023-06-06 00:36:13.000000 matchcode-toolkit-1.0.0/pyproject.toml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1356 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)       92 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/setup.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.751959 matchcode-toolkit-1.0.0/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/src/matchcode_toolkit/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     4315 2023-06-06 00:18:09.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2023-06-06 00:27:30.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/src/matchcode_toolkit/pipelines/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-06-06 00:47:57.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/pipelines/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2443 2023-06-05 22:22:33.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1427 2023-05-05 21:13:22.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit/plugin_fingerprint.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/
--rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)      764 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      222 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-03-07 02:11:31.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 jono      (1000) jono      (1000)      165 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       18 2023-06-06 00:49:10.000000 matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4948 2023-06-06 00:18:36.000000 matchcode-toolkit-1.0.0/tests/test_fingerprinting.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.751959 matchcode-toolkit-1.0.0/tests/testfiles/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-06 00:49:10.755959 matchcode-toolkit-1.0.0/tests/testfiles/fingerprinting/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2023-04-13 19:04:55.000000 matchcode-toolkit-1.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      104 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/AUTHORS.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      306 2023-06-23 00:59:25.000000 matchcode-toolkit-1.1.0/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      217 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/NOTICE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2516 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.0/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/apache-2.0.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)      923 2023-06-23 01:01:01.000000 matchcode-toolkit-1.1.0/pyproject.toml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1356 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)       92 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/setup.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/matchcode_toolkit/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4815 2023-06-22 23:11:27.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-06-06 00:47:57.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2461 2023-06-22 19:21:36.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2023-06-22 19:21:32.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/plugin_fingerprint.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)      764 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      222 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-03-07 02:11:31.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 jono      (1000) jono      (1000)      165 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       18 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4975 2023-06-22 19:21:39.000000 matchcode-toolkit-1.1.0/tests/test_fingerprinting.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/tests/testfiles/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
```

### Comparing `matchcode-toolkit-1.0.0/NOTICE` & `matchcode-toolkit-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.0.0/PKG-INFO` & `matchcode-toolkit-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 1.0.0
+Version: 1.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `matchcode-toolkit-1.0.0/README.rst` & `matchcode-toolkit-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.0.0/apache-2.0.LICENSE` & `matchcode-toolkit-1.1.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.0.0/pyproject.toml` & `matchcode-toolkit-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "matchcode-toolkit"
-version = "1.0.0"
+version = "1.1.0"
 
 [build-system]
 requires = ["setuptools >= 50", "wheel", "setuptools_scm[toml] >= 6"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # this is used populated when creating a git archive
```

### Comparing `matchcode-toolkit-1.0.0/setup.cfg` & `matchcode-toolkit-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = matchcode-toolkit
-version = 1.0.0
+version = 1.1.0
 license = Apache-2.0
 description = matchcode-toolkit
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 author = nexB. Inc. and others
 author_email = info@aboutcode.org
```

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit/fingerprinting.py` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit/fingerprinting.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,38 +65,57 @@
         else:
             rounded_child_size = int(child.size / 10) * 10
         path_feature = str(rounded_child_size) + child_subpath
         features.append(path_feature)
     return _create_directory_fingerprint(features)
 
 
-def compute_directory_fingerprints(codebase):
+def _compute_directory_fingerprints(directory, codebase):
     """
-    Compute fingerprints for a directory from `codebase`
+    Compute fingerprints for `directory` from `codebase`
     """
-    for resource in codebase.walk(topdown=False):
-        if resource.is_file or not resource.path:
-            continue
-        children = [r for r in resource.walk(codebase) if r.is_file]
-        if len(children) == 1:
-            continue
+    children = [r for r in directory.walk(codebase) if r.is_file]
+    if len(children) == 1:
+        return
+
+    directory_content_fingerprint = create_content_fingerprint(children)
+    if hasattr(directory, 'directory_content_fingerprint'):
+        directory.directory_content_fingerprint = directory_content_fingerprint
+    else:
+        directory.extra_data['directory_content'] = directory_content_fingerprint
+
+    directory_structure_fingerprint = create_structure_fingerprint(directory, children)
+    if hasattr(directory, 'directory_structure_fingerprint'):
+        directory.directory_structure_fingerprint = directory_structure_fingerprint
+    else:
+        directory.extra_data['directory_structure'] = directory_structure_fingerprint
 
-        directory_content_fingerprint = create_content_fingerprint(children)
-        if hasattr(resource, 'directory_content_fingerprint'):
-            resource.directory_content_fingerprint = directory_content_fingerprint
-        else:
-            resource.extra_data['directory_content'] = directory_content_fingerprint
+    directory.save(codebase)
+    return directory
 
-        directory_structure_fingerprint = create_structure_fingerprint(resource, children)
-        if hasattr(resource, 'directory_structure_fingerprint'):
-            resource.directory_structure_fingerprint = directory_structure_fingerprint
-        else:
-            resource.extra_data['directory_structure'] = create_structure_fingerprint(resource, children)
 
-        resource.save(codebase)
+def compute_directory_fingerprints(directory, codebase):
+    """
+    Recursivly compute fingerprints for `directory` from `codebase`
+    """
+    for resource in directory.walk(codebase, topdown=False):
+        if resource.is_file:
+            continue
+        _ = _compute_directory_fingerprints(resource, codebase)
+    return directory
+
+
+def compute_codebase_directory_fingerprints(codebase):
+    """
+    Compute fingerprints for directories from `codebase`
+    """
+    for resource in codebase.walk(topdown=False):
+        if resource.is_file or not resource.path:
+            continue
+        _ = _compute_directory_fingerprints(resource, codebase)
     return codebase
 
 
 def split_fingerprint(directory_fingerprint):
     """
     Given a string `directory_fingerprint`, return the indexed elements count as
     an integer and the bah128 fingerprint string
```

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit/halohash.py` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit/halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # OR CONDITIONS OF ANY KIND, either express or implied. No content created from
 # ScanCode.io should be considered or used as legal advice. Consult an Attorney
 # for any legal advice.
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
-from matchcode_toolkit.fingerprinting import compute_directory_fingerprints
+from matchcode_toolkit.fingerprinting import compute_codebase_directory_fingerprints
 
 from scanpipe.pipelines.scan_package import ScanPackage
 from scanpipe.pipes.codebase import ProjectCodebase
 
 
 class ScanAndFingerprintPackage(ScanPackage):
     """
@@ -59,8 +59,8 @@
     ]
 
     def fingerprint_codebase(self):
         """
         Compute directory fingerprints for matching purposes
         """
         project_codebase = ProjectCodebase(self.project)
-        compute_directory_fingerprints(project_codebase)
+        compute_codebase_directory_fingerprints(project_codebase)
```

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit/plugin_fingerprint.py` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit/plugin_fingerprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
 
 import attr
 
 from commoncode.cliutils import PluggableCommandLineOption
 from commoncode.cliutils import POST_SCAN_GROUP
-from matchcode_toolkit.fingerprinting import compute_directory_fingerprints
+from matchcode_toolkit.fingerprinting import compute_codebase_directory_fingerprints
 from plugincode.post_scan import post_scan_impl
 from plugincode.post_scan import PostScanPlugin
 
 
 @post_scan_impl
 class Fingerprint(PostScanPlugin):
     resource_attributes = dict(
@@ -37,8 +37,8 @@
         )
     ]
 
     def is_enabled(self, fingerprint, **kwargs):
         return fingerprint
 
     def process_codebase(self, codebase, **kwargs):
-        codebase = compute_directory_fingerprints(codebase)
+        codebase = compute_codebase_directory_fingerprints(codebase)
```

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/PKG-INFO` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 1.0.0
+Version: 1.1.0
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `matchcode-toolkit-1.0.0/src/matchcode_toolkit.egg-info/SOURCES.txt` & `matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.0.0/tests/test_fingerprinting.py` & `matchcode-toolkit-1.1.0/tests/test_fingerprinting.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 
 from commoncode.resource import VirtualCodebase
 from commoncode.testcase import FileBasedTesting
 
 from matchcode_toolkit.fingerprinting import _create_directory_fingerprint
 from matchcode_toolkit.fingerprinting import _get_resource_subpath
-from matchcode_toolkit.fingerprinting import compute_directory_fingerprints
+from matchcode_toolkit.fingerprinting import compute_codebase_directory_fingerprints
 from matchcode_toolkit.fingerprinting import create_content_fingerprint
 from matchcode_toolkit.fingerprinting import create_halohash_chunks
 from matchcode_toolkit.fingerprinting import create_structure_fingerprint
 from matchcode_toolkit.fingerprinting import split_fingerprint
 
 
 class Resource():
@@ -91,17 +91,17 @@
         expected_chunk3 = bytearray(b'\xb0\xfbG\xed')
         expected_chunk4 = bytearray(b'Y\x0b\\S')
         self.assertEqual(chunk1, expected_chunk1)
         self.assertEqual(chunk2, expected_chunk2)
         self.assertEqual(chunk3, expected_chunk3)
         self.assertEqual(chunk4, expected_chunk4)
 
-    def test_compute_directory_fingerprints(self):
+    def test_compute_codebase_directory_fingerprints(self):
         scan_loc = self.get_test_loc('abbrev-1.0.3-i.json')
         vc = VirtualCodebase(location=scan_loc)
-        vc = compute_directory_fingerprints(vc)
+        vc = compute_codebase_directory_fingerprints(vc)
         directory_content = vc.root.extra_data['directory_content']
         directory_structure = vc.root.extra_data['directory_structure']
         expected_directory_content = '0000000346ce04751a3c98f00086f16a91d9790b'
         expected_directory_structure = '000000034f9bf110673bdf06197cd514a799a66c'
         self.assertEqual(expected_directory_content, directory_content)
         self.assertEqual(expected_directory_structure, directory_structure)
```

### Comparing `matchcode-toolkit-1.0.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json` & `matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json`

 * *Files identical despite different names*

