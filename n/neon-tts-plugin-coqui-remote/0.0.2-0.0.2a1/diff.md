# Comparing `tmp/neon-tts-plugin-coqui-remote-0.0.2.tar.gz` & `tmp/neon-tts-plugin-coqui-remote-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.2.tar", last modified: Fri Jun 23 21:32:52 2023, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.2a1.tar", last modified: Fri Jun 23 21:05:24 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-remote-0.0.2.tar` & `neon-tts-plugin-coqui-remote-0.0.2a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:32:52.162940 neon-tts-plugin-coqui-remote-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-23 21:32:48.000000 neon-tts-plugin-coqui-remote-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-23 21:32:52.162940 neon-tts-plugin-coqui-remote-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-23 21:32:48.000000 neon-tts-plugin-coqui-remote-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:32:52.162940 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-23 21:32:48.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-23 21:32:48.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:32:52.162940 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:32:52.000000 neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:32:52.162940 neon-tts-plugin-coqui-remote-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-23 21:32:48.000000 neon-tts-plugin-coqui-remote-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:05:24.300132 neon-tts-plugin-coqui-remote-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-23 21:05:19.000000 neon-tts-plugin-coqui-remote-0.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-23 21:05:24.300132 neon-tts-plugin-coqui-remote-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-23 21:05:19.000000 neon-tts-plugin-coqui-remote-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:05:24.296132 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-23 21:05:19.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-23 21:05:19.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:05:24.300132 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:05:24.000000 neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:05:24.300132 neon-tts-plugin-coqui-remote-0.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-23 21:05:19.000000 neon-tts-plugin-coqui-remote-0.0.2a1/setup.py
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/LICENSE.md` & `neon-tts-plugin-coqui-remote-0.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.2a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.2
+Version: 0.0.2a1
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui-remote
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/README.md` & `neon-tts-plugin-coqui-remote-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote/__init__.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote/configs.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.2
+Version: 0.0.2a1
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui-remote
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.2/setup.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/setup.py`

 * *Files identical despite different names*

