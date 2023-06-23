# Comparing `tmp/cicada-0.5.1.tar.gz` & `tmp/cicada-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicada-0.5.1.tar", last modified: Mon Feb 27 16:00:16 2023, max compression
+gzip compressed data, was "cicada-0.6.0.tar", last modified: Fri Jun 23 12:35:25 2023, max compression
```

## Comparing `cicada-0.5.1.tar` & `cicada-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:16.539594 cicada-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-02-27 16:00:07.000000 cicada-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-02-27 16:00:16.539594 cicada-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-02-27 16:00:07.000000 cicada-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:16.535593 cicada-0.5.1/cicada/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:16.539594 cicada-0.5.1/cicada/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/archive_schedule_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/exec_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/exec_server_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/list_server_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/ping_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/register_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/show_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/spread_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/commands/upsert_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:16.539594 cicada-0.5.1/cicada/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/lib/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/lib/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-02-27 16:00:07.000000 cicada-0.5.1/cicada/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:00:16.535593 cicada-0.5.1/cicada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-27 16:00:16.000000 cicada-0.5.1/cicada.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 16:00:07.000000 cicada-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 16:00:16.539594 cicada-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-27 16:00:07.000000 cicada-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:25.863240 cicada-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-23 12:35:12.000000 cicada-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-23 12:35:25.863240 cicada-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-23 12:35:12.000000 cicada-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:25.859240 cicada-0.6.0/cicada/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:25.863240 cicada-0.6.0/cicada/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/archive_schedule_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/exec_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/exec_server_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/list_server_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/ping_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/register_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/show_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/spread_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/commands/upsert_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:25.863240 cicada-0.6.0/cicada/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/lib/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/lib/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-23 12:35:12.000000 cicada-0.6.0/cicada/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:25.859240 cicada-0.6.0/cicada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 12:35:25.000000 cicada-0.6.0/cicada.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 12:35:12.000000 cicada-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:35:25.863240 cicada-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-23 12:35:12.000000 cicada-0.6.0/setup.py
```

### Comparing `cicada-0.5.1/LICENSE` & `cicada-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/PKG-INFO` & `cicada-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cicada
-Version: 0.5.1
+Version: 0.6.0
 Summary: Lightweight, agent-based, distributed scheduler
 Home-page: https://github.com/transferwise/cicada
 Author: Wise
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cicada-0.5.1/README.md` & `cicada-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/cli.py` & `cicada-0.6.0/cicada/cli.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/archive_schedule_log.py` & `cicada-0.6.0/cicada/commands/archive_schedule_log.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/exec_schedule.py` & `cicada-0.6.0/cicada/commands/exec_schedule.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/exec_server_schedules.py` & `cicada-0.6.0/cicada/commands/exec_server_schedules.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/list_server_schedules.py` & `cicada-0.6.0/cicada/commands/list_server_schedules.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/register_server.py` & `cicada-0.6.0/cicada/commands/register_server.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/show_schedule.py` & `cicada-0.6.0/cicada/commands/show_schedule.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/spread_schedules.py` & `cicada-0.6.0/cicada/commands/spread_schedules.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/commands/upsert_schedule.py` & `cicada-0.6.0/cicada/commands/upsert_schedule.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/lib/postgres.py` & `cicada-0.6.0/cicada/lib/postgres.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada/lib/scheduler.py` & `cicada-0.6.0/cicada/lib/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         sqlquery = sqlquery + " ,schedule_group_id"
 
     sqlquery = sqlquery + ") VALUES ('" + str(schedule_details["schedule_id"]) + "'"
 
     if schedule_details["schedule_description"] is not None:
         sqlquery = sqlquery + " ,'" + str(schedule_details["schedule_description"]) + "'"
     if schedule_details["server_id"] is None:
-        sqlquery = sqlquery + " ,(SELECT MIN(server_id) FROM servers WHERE is_enabled=1)"
+        sqlquery = sqlquery + " ,(SELECT MAX(server_id) FROM servers WHERE is_enabled=1)"
     else:
         sqlquery = sqlquery + " ," + str(schedule_details["server_id"])
     if schedule_details["schedule_order"] is not None:
         sqlquery = sqlquery + " ," + str(schedule_details["schedule_order"])
     if schedule_details["is_async"] is not None:
         sqlquery = sqlquery + " ," + str(schedule_details["is_async"])
     if schedule_details["is_enabled"] is not None:
```

### Comparing `cicada-0.5.1/cicada/lib/utils.py` & `cicada-0.6.0/cicada/lib/utils.py`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/cicada.egg-info/PKG-INFO` & `cicada-0.6.0/cicada.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cicada
-Version: 0.5.1
+Version: 0.6.0
 Summary: Lightweight, agent-based, distributed scheduler
 Home-page: https://github.com/transferwise/cicada
 Author: Wise
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cicada-0.5.1/cicada.egg-info/SOURCES.txt` & `cicada-0.6.0/cicada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cicada-0.5.1/setup.py` & `cicada-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="cicada",
-    version="0.5.1",
+    version="0.6.0",
     description="Lightweight, agent-based, distributed scheduler",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Wise",
     url="https://github.com/transferwise/cicada",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     install_requires=[
         "psycopg2-binary==2.9.5",
         "pyyaml==6.0",
-        "croniter==1.3.8",
-        "tabulate==0.9.0",
-        "slack-sdk==3.19.5",
-        "backoff==2.2.1",
+        "croniter==1.3",
+        "tabulate==0.9",
+        "slack-sdk==3.19",
+        "backoff==2.2",
     ],
     extras_require={
         "dev": [
-            "pytest==7.2.0",
-            "pytest-cov==4.0.0",
-            "pytest-mock==3.10.0",
-            "black==22.12.0",
-            "flake8==6.0.0",
-            "freezegun==1.2.2",
+            "pytest==7.3",
+            "pytest-cov==4.0",
+            "pytest-mock==3.10",
+            "black==22.12",
+            "flake8==6.0",
+            "freezegun==1.2",
         ]
     },
     entry_points={"console_scripts": ["cicada=cicada.cli:main"]},
     packages=find_packages(include=["cicada", "cicada.*"]),
 )
```

