# Comparing `tmp/factro_client-0.9.0a1.tar.gz` & `tmp/factro_client-0.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factro_client-0.9.0a1.tar", last modified: Mon Jan 30 14:50:58 2023, max compression
+gzip compressed data, was "factro_client-0.9.1a1.tar", last modified: Wed Feb  1 10:10:39 2023, max compression
```

## Comparing `factro_client-0.9.0a1.tar` & `factro_client-0.9.1a1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.340180 factro_client-0.9.0a1/
--rw-r--r--   0 runner    (1001) docker     (116)      678 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      196 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client/controlling/
--rw-r--r--   0 runner    (1001) docker     (116)       64 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/controlling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7505 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/controlling/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client/core/
--rw-r--r--   0 runner    (1001) docker     (116)      105 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/client.py
--rw-r--r--   0 runner    (1001) docker     (116)      314 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2631 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1214 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/company_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1154 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/contact_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1533 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/package_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/project_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1676 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/task_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1283 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/user_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1293 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/core/helpers/work_record_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client/effort_estimation/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/effort_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9959 2023-01-30 14:50:49.000000 factro_client-0.9.0a1/factro_client/effort_estimation/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 14:50:58.336180 factro_client-0.9.0a1/factro_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      678 2023-01-30 14:50:58.000000 factro_client-0.9.0a1/factro_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      883 2023-01-30 14:50:58.000000 factro_client-0.9.0a1/factro_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-30 14:50:58.000000 factro_client-0.9.0a1/factro_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      101 2023-01-30 14:50:58.000000 factro_client-0.9.0a1/factro_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-01-30 14:50:58.000000 factro_client-0.9.0a1/factro_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-30 14:50:58.340180 factro_client-0.9.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1225 2023-01-30 14:50:57.000000 factro_client-0.9.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.240710 factro_client-0.9.1a1/
+-rw-r--r--   0 runner    (1001) docker     (116)      678 2023-02-01 10:10:39.240710 factro_client-0.9.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      196 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.236710 factro_client-0.9.1a1/factro_client/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.236710 factro_client-0.9.1a1/factro_client/controlling/
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/controlling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7708 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/controlling/client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.236710 factro_client-0.9.1a1/factro_client/core/
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)      314 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.240710 factro_client-0.9.1a1/factro_client/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2631 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1214 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/company_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1154 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/contact_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1533 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/package_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2010 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/project_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1676 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/task_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1283 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/user_handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1293 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/core/helpers/work_record_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.240710 factro_client-0.9.1a1/factro_client/effort_estimation/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/effort_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9959 2023-02-01 10:10:31.000000 factro_client-0.9.1a1/factro_client/effort_estimation/client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-01 10:10:39.236710 factro_client-0.9.1a1/factro_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      678 2023-02-01 10:10:39.000000 factro_client-0.9.1a1/factro_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      883 2023-02-01 10:10:39.000000 factro_client-0.9.1a1/factro_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-01 10:10:39.000000 factro_client-0.9.1a1/factro_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      101 2023-02-01 10:10:39.000000 factro_client-0.9.1a1/factro_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-01 10:10:39.000000 factro_client-0.9.1a1/factro_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-01 10:10:39.240710 factro_client-0.9.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1225 2023-02-01 10:10:38.000000 factro_client-0.9.1a1/setup.py
```

### Comparing `factro_client-0.9.0a1/PKG-INFO` & `factro_client-0.9.1a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factro_client
-Version: 0.9.0a1
+Version: 0.9.1a1
 Summary: A core api client for project management tool 'factro'.
 Home-page: https://github.com/5minds/factro_client
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: developers@5minds.de
 Keywords: client factro 5minds processcube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `factro_client-0.9.0a1/factro_client/controlling/client.py` & `factro_client-0.9.1a1/factro_client/controlling/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,38 +98,43 @@
         user = self._core_client.get_user_by_id(user_id)
         return user
 
     def query_controlling_data(self, from_date: str, to_date: str) -> List[ActivityRecording]:
 
         tz = get_localzone()
 
-        def is_billable(workrecord: WorkRecord, package: Package, project: Project) -> bool:
+        def is_billable(workrecord: WorkRecord, task: Task, package: Package, project: Project) -> bool:
             billable = workrecord.is_billable
 
             if workrecord.is_billable:
-                billable = package.custom_fields.get('abrechenbar', workrecord.is_billable) if package is not None else workrecord.is_billable
+
+                billable = task.custom_fields.get('abrechenbar', workrecord.is_billable) if task is not None else workrecord.is_billable
 
                 if billable:
-                    if project is not None and "abrechnungsart" in project.custom_fields.keys():
-                        billable = project.custom_fields.get('abrechnungsart') != 'keine_abrechnung'
+
+                    billable = package.custom_fields.get('abrechenbar', workrecord.is_billable) if package is not None else workrecord.is_billable
+
+                    if billable:
+                        if project is not None and "abrechnungsart" in project.custom_fields.keys():
+                            billable = project.custom_fields.get('abrechnungsart') != 'keine_abrechnung'
 
             return billable
 
         def make_datetime(date_string: str) -> datetime:
             d = datetime.strptime(date_string, '%Y-%m-%dT%H:%M:%S')
 
             return tz.localize(d).isoformat()
 
         def mapping(workrecord: WorkRecord, user: User, task: Task, package: Package, project: Project, company: Company, company_contact: Contact) -> ActivityRecording:
             activity_recording = ActivityRecording(
                 start_date = make_datetime(f"{workrecord.start_date}T{workrecord.start_time}"),
                 end_date = make_datetime(f"{workrecord.end_date}T{workrecord.end_time}"),
                 title = workrecord.title,
                 #is_billable = package.custom_fields.get('abrechenbar', workrecord.is_billable) if package is not None else workrecord.is_billable,
-                is_billable = is_billable(workrecord, package, project),
+                is_billable = is_billable(workrecord, task, package, project),
                 hours = workrecord.minutes_worked / 60,
                 description = workrecord.description,
                 driving_distance_km = 0,
                 task_number = task.number,
                 company_name = company.name if company is not None else '',
                 company_shortname = company.short_name if company is not None else '',
                 project_name = project.title,
```

### Comparing `factro_client-0.9.0a1/factro_client/core/client.py` & `factro_client-0.9.1a1/factro_client/core/client.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/base_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/base_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/company_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/company_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/contact_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/contact_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/package_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/package_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/project_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/project_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/task_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/task_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/user_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/user_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/core/helpers/work_record_handler.py` & `factro_client-0.9.1a1/factro_client/core/helpers/work_record_handler.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client/effort_estimation/client.py` & `factro_client-0.9.1a1/factro_client/effort_estimation/client.py`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/factro_client.egg-info/PKG-INFO` & `factro_client-0.9.1a1/factro_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factro-client
-Version: 0.9.0a1
+Version: 0.9.1a1
 Summary: A core api client for project management tool 'factro'.
 Home-page: https://github.com/5minds/factro_client
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: developers@5minds.de
 Keywords: client factro 5minds processcube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `factro_client-0.9.0a1/factro_client.egg-info/SOURCES.txt` & `factro_client-0.9.1a1/factro_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factro_client-0.9.0a1/setup.py` & `factro_client-0.9.1a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='factro_client',
-    version=setuptools.sic('0.9.0-alpha.1'),
+    version=setuptools.sic('0.9.1-alpha.1'),
     author="5Minds IT-Solutions GmbH & Co. KG",
     author_email="developers@5minds.de",
     description="A core api client for project management tool 'factro'.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="client factro 5minds processcube",
     url="https://github.com/5minds/factro_client",
```

