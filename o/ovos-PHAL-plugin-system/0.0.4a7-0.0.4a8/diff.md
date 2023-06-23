# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a7.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a7.tar", last modified: Wed Jun 21 22:46:20 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a8.tar", last modified: Wed Jun 21 22:55:34 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a7.tar` & `ovos-PHAL-plugin-system-0.0.4a8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:55:34.000000 ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:55:34.549060 ovos-PHAL-plugin-system-0.0.4a8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-21 22:55:30.000000 ovos-PHAL-plugin-system-0.0.4a8/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a7
+Version: 0.0.4a8
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,16 @@
                 sid = message.data["skill_id"]
                 if sid not in reset_plugs:
                     reset_plugs.append(sid)
                 if all([s in reset_plugs for s in self.factory_reset_plugs]):
                     event.set()
 
             self.bus.on("system.factory.reset.phal.complete", on_done)
-            self.bus.emit(message.forward("system.factory.reset.phal"))
+            self.bus.emit(message.forward("system.factory.reset.phal",
+                                          message.data))
             event.wait(timeout=60)
             self.bus.remove("system.factory.reset.phal.complete", on_done)
 
         script = message.data.get("script", True)
         if script:
             script = os.path.expanduser(self.config.get("reset_script", ""))
             LOG.debug(f"Running reset script: {script}")
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a7
+Version: 0.0.4a8
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a8/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a7/setup.py` & `ovos-PHAL-plugin-system-0.0.4a8/setup.py`

 * *Files identical despite different names*

