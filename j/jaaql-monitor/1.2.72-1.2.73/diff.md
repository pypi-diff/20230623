# Comparing `tmp/jaaql-monitor-1.2.72.tar.gz` & `tmp/jaaql-monitor-1.2.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.72.tar", last modified: Tue Jun 20 10:10:37 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.73.tar", last modified: Fri Jun 23 18:07:57 2023, max compression
```

## Comparing `jaaql-monitor-1.2.72.tar` & `jaaql-monitor-1.2.73.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.806904 jaaql-monitor-1.2.72/
--rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/LICENSE.txt
--rw-rw-rw-   0        0        0     1454 2023-06-20 10:10:37.805905 jaaql-monitor-1.2.72/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.803906 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1454 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.804906 jaaql-monitor-1.2.72/monitor/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/monitor/__init__.py
--rw-rw-rw-   0        0        0    31684 2023-06-20 10:10:21.000000 jaaql-monitor-1.2.72/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-20 10:10:28.000000 jaaql-monitor-1.2.72/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:10:37.807905 jaaql-monitor-1.2.72/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.636523 jaaql-monitor-1.2.73/
+-rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/LICENSE.txt
+-rw-rw-rw-   0        0        0     1454 2023-06-23 18:07:57.635523 jaaql-monitor-1.2.73/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.634523 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1454 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 18:07:57.000000 jaaql-monitor-1.2.73/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 18:07:57.635523 jaaql-monitor-1.2.73/monitor/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/monitor/__init__.py
+-rw-rw-rw-   0        0        0    31823 2023-06-23 18:07:46.000000 jaaql-monitor-1.2.73/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-23 18:07:49.000000 jaaql-monitor-1.2.73/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:07:57.636523 jaaql-monitor-1.2.73/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.73/setup.py
```

### Comparing `jaaql-monitor-1.2.72/LICENSE.txt` & `jaaql-monitor-1.2.73/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.72/PKG-INFO` & `jaaql-monitor-1.2.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.72
+Version: 1.2.73
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.72/README.md` & `jaaql-monitor-1.2.73/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.72/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.73/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.72
+Version: 1.2.73
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.72/monitor/main.py` & `jaaql-monitor-1.2.73/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,22 +707,26 @@
             state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]).decode(), b64d(content_split[1]).decode(),
                                                                        b64d(content_split[2]).decode(), db, state.override_url)
 
     deal_with_input(state, file_content)
 
 
 def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]],
-               override_url: str):
+               override_url: str, folder_name: str = None):
     args = [ARGS__single_query[0]]
 
     for config in configs:
         args.append(ARGS__config[0])
         args.append(config[0])
         args.append(config[1])
 
+    if folder_name is not None:
+        args.append(ARGS__folder_config[0])
+        args.append(folder_name)
+
     for encoded_config in encoded_configs:
         args.append(ARGS__encoded_config[0])
         args.append(encoded_config[0])
         db_part = ""
         if encoded_config[4]:
             db_part = ":" + b64e(encoded_config[4].encode()).decode()
         args.append(b64e(encoded_config[1].encode()).decode() + ":" + b64e(encoded_config[2].encode()).decode() + ":" +
```

### Comparing `jaaql-monitor-1.2.72/setup.py` & `jaaql-monitor-1.2.73/setup.py`

 * *Files identical despite different names*

