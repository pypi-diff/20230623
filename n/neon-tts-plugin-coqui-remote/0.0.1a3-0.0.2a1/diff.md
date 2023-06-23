# Comparing `tmp/neon-tts-plugin-coqui-remote-0.0.1a3.tar.gz` & `tmp/neon-tts-plugin-coqui-remote-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a3.tar", last modified: Thu Jun 22 01:16:29 2023, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.2a1.tar", last modified: Fri Jun 23 21:05:24 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-remote-0.0.1a3.tar` & `neon-tts-plugin-coqui-remote-0.0.2a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.245917 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/setup.py
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

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/LICENSE.md` & `neon-tts-plugin-coqui-remote-0.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.2a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a3
+Version: 0.0.2a1
 Summary: A Coqui AI Remote TTS plugin for Neon
-Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
+Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui-remote
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
@@ -17,11 +17,13 @@
 [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
 TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
 
 ## Configuration
 ```yaml
 TTS:
   module: neon-tts-plugin-coqui-remote
+  neon-tts-plugin-coqui-remote:
+    url: "https://coqui.2022.us"
 ```
 ## Language Support
 See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
 support info.
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/__init__.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/configs.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.2a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a3
+Version: 0.0.2a1
 Summary: A Coqui AI Remote TTS plugin for Neon
-Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
+Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui-remote
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
@@ -17,11 +17,13 @@
 [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
 TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
 
 ## Configuration
 ```yaml
 TTS:
   module: neon-tts-plugin-coqui-remote
+  neon-tts-plugin-coqui-remote:
+    url: "https://coqui.2022.us"
 ```
 ## Language Support
 See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
 support info.
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a3/setup.py` & `neon-tts-plugin-coqui-remote-0.0.2a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,22 @@
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
 
 PLUGIN_ENTRY_POINT = 'neon-tts-plugin-coqui-remote = neon_tts_plugin_coqui_remote:CoquiRemoteTTS'
-CONFIG_ENTRY_POINT = 'neon-tts-plugin-coqui-remote.config = neon_tts_plugin_coqui.configs:tts_config'
+CONFIG_ENTRY_POINT = 'neon-tts-plugin-coqui-remote.config = neon_tts_plugin_coqui_remote.configs:tts_config'
 setup(
     name='neon-tts-plugin-coqui-remote',
     version=version,
     description='A Coqui AI Remote TTS plugin for Neon',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/NeonGeckoCom/neon-tts-plugin-coqui',
+    url='https://github.com/NeonGeckoCom/neon-tts-plugin-coqui-remote',
     author='Neongecko',
     author_email='developers@neon.ai',
     license='BSD-3.0',
     packages=find_packages(),
     install_requires=get_requirements("requirements.txt"),
     zip_safe=True,
     classifiers=[
```

