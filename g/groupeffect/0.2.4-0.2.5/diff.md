# Comparing `tmp/groupeffect-0.2.4.tar.gz` & `tmp/groupeffect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.2.4.tar", last modified: Wed Jun 21 14:16:12 2023, max compression
+gzip compressed data, was "groupeffect-0.2.5.tar", last modified: Fri Jun 23 21:13:49 2023, max compression
```

## Comparing `groupeffect-0.2.4.tar` & `groupeffect-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/
--rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.4/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4308 2023-06-21 14:16:12.649204 groupeffect-0.2.4/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     3016 2023-06-21 12:58:29.000000 groupeffect-0.2.4/README.md
--rw-rw-r--   0 root         (0) root         (0)      190 2023-06-21 14:16:12.000000 groupeffect-0.2.4/VERSION.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.4/groupeffect/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.4/groupeffect/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.4/groupeffect/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5531 2023-06-21 13:14:58.000000 groupeffect-0.2.4/groupeffect/management/commands/effect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/configuration/
--rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/management/configuration/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/management/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/management/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-21 13:10:11.000000 groupeffect-0.2.4/groupeffect/management/tasks/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect/templates/groupeffect/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/
--rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/database.txt
--rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/serializers.txt
--rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/tests.txt
--rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/urls.txt
--rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/default/views.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.649204 groupeffect-0.2.4/groupeffect/templates/groupeffect/web/
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.4/groupeffect/templates/groupeffect/web/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:16:12.645204 groupeffect-0.2.4/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4308 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      812 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-21 14:16:12.000000 groupeffect-0.2.4/groupeffect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1269 2023-06-21 14:16:12.649204 groupeffect-0.2.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      417 2023-06-21 13:09:18.000000 groupeffect-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/
+-rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.5/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9013 2023-06-23 21:13:49.579946 groupeffect-0.2.5/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     7721 2023-06-23 21:10:22.000000 groupeffect-0.2.5/README.md
+-rw-rw-r--   0 root         (0) root         (0)      190 2023-06-23 21:13:49.000000 groupeffect-0.2.5/VERSION.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.575946 groupeffect-0.2.5/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.5/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.575946 groupeffect-0.2.5/groupeffect/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.5/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/groupeffect/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.5/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6429 2023-06-23 21:11:39.000000 groupeffect-0.2.5/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/groupeffect/management/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/management/configuration/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/groupeffect/management/tasks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/management/tasks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9779 2023-06-23 20:50:12.000000 groupeffect-0.2.5/groupeffect/management/tasks/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.575946 groupeffect-0.2.5/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.575946 groupeffect-0.2.5/groupeffect/templates/groupeffect/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/database.txt
+-rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/serializers.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/tests.txt
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/urls.txt
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/default/views.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.579946 groupeffect-0.2.5/groupeffect/templates/groupeffect/web/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.5/groupeffect/templates/groupeffect/web/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:13:49.575946 groupeffect-0.2.5/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9013 2023-06-23 21:13:49.000000 groupeffect-0.2.5/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-23 21:13:49.000000 groupeffect-0.2.5/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:13:49.000000 groupeffect-0.2.5/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-23 21:13:49.000000 groupeffect-0.2.5/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1269 2023-06-23 21:13:49.579946 groupeffect-0.2.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      417 2023-06-21 13:09:18.000000 groupeffect-0.2.5/setup.py
```

### Comparing `groupeffect-0.2.4/LICENSE` & `groupeffect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.4/groupeffect/management/commands/effect.py` & `groupeffect-0.2.5/groupeffect/management/commands/effect.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,17 +60,35 @@
         "args": ["-n", "--name"],
         "kwargs": {
             "nargs": "?",
             "help": "Name value",
         },
     },
     {
+        "key": "model",
+        "value": "Namespace",
+        "args": ["-mo", "--model"],
+        "kwargs": {
+            "nargs": "?",
+            "help": "Model name",
+        },
+    },
+    {
+        "key": "schema",
+        "value": "default",
+        "args": ["-sc", "--schema"],
+        "kwargs": {
+            "nargs": "?",
+            "help": "Schema name",
+        },
+    },
+    {
         "key": "service",
         "value": "api",
-        "args": ["-s", "--service-name"],
+        "args": ["-s", "--service"],
         "kwargs": {
             "nargs": "?",
             "help": "Service name",
         },
     },
     {
         "key": "path",
@@ -86,14 +104,24 @@
         "value": "api",
         "args": ["-pf", "--prefix"],
         "kwargs": {
             "nargs": "?",
             "help": "Prefix for something",
         },
     },
+    {
+        "key": "argument",
+        "value": "argument",
+        "args": ["-a", "--argument"],
+        "kwargs": {
+            "nargs": "?",
+            "help": "Argument for something",
+            "action": "append",
+        },
+    },
 ]
 
 
 class Configurator:
     def __init__(self, options=None) -> None:
         self.success = []
         self.errors = []
@@ -113,29 +141,41 @@
 
             self.config_file = os.getenv(
                 "GROUPEFFECT_CONFIG_JSON_FILE_PATH",
                 default,
             )
         self.read_config_json()
 
-        self.tasks = []
+        self.tasks = [
+            import_string("groupeffect.management.tasks.default.DefaultTask"),
+            import_string("groupeffect.management.tasks.default.CreateAppTask"),
+            import_string(
+                "groupeffect.management.tasks.default.CreateConfigurationJsonFileTask"
+            ),
+        ]
         try:
-            self.tasks += [
+            self.tasks = [
                 import_string(i) for i in settings.GROUPEFFECT_MANAGEMENT_TASKS
             ]
-        except Exception as e:
-            self.errors.append(e)
-        try:
-            self.tasks += [
-                import_string("groupeffect.management.tasks.default.DefaultTask"),
-                import_string("groupeffect.management.tasks.default.CreateAppTask"),
-                import_string(
-                    "groupeffect.management.tasks.default.CreateConfigurationJsonFileTask"
-                ),
-            ]
+            self.success.append(
+                """
+You changed the default tasks they are no longer available.
+If you want to keep the default tasks.
+you can add:
+
+    groupeffect.management.tasks.default.DefaultTask,
+    groupeffect.management.tasks.default.CreateAppTask,
+    groupeffect.management.tasks.default.CreateConfigurationJsonFileTask,
+
+to:
+
+GROUPEFFECT_MANAGEMENT_TASKS
+
+"""
+            )
         except Exception as e:
             self.errors.append(e)
 
         if not self.tasks:
             self.errors.append("No tasks found")
 
     def read_config_json(self):
```

### Comparing `groupeffect-0.2.4/groupeffect/templates/groupeffect/web/api.html` & `groupeffect-0.2.5/groupeffect/templates/groupeffect/web/api.html`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.4/groupeffect.egg-info/SOURCES.txt` & `groupeffect-0.2.5/groupeffect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.4/setup.cfg` & `groupeffect-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = groupeffect
-version = 0.2.4
+version = 0.2.5
 description = A Django app for fast api development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Groupeffect/groupeffect-pypi
 author = Amir Yousefi
 author_email = groupeffect.public@gmail.com
 license = MIT
```

