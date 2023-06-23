# Comparing `tmp/django_bg_task-0.0.1.tar.gz` & `tmp/django_bg_task-0.0.2.tar.gz`

## Comparing `django_bg_task-0.0.1.tar` & `django_bg_task-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.isort.cfg
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/ignore-spelling-words.txt
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/manage.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/mypy.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/apps.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/common.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/constants.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/handler.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/models.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/serializers.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/services.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/settings.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/urls.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/views.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0001_initial.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0002_alter_task_status.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0003_remove_task_task_id.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0004_alter_task_id.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0005_rename_arguments_task_args_and_more.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0006_remove_task_exception_task_failed_reason_and_more.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0007_alter_task_created_at_alter_task_failed_reason_and_more.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/0008_remove_task_identifier_task_identifiers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/django_task/migrations/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/LICENSE
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/README.md
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/manage.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/mypy.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/apps.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/common.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/constants.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/handler.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/models.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/serializers.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/services.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/settings.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/urls.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/views.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0001_initial.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0002_alter_task_status.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0003_remove_task_task_id.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0004_alter_task_id.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0005_rename_arguments_task_args_and_more.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0006_remove_task_exception_task_failed_reason_and_more.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0007_alter_task_created_at_alter_task_failed_reason_and_more.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0008_remove_task_identifier_task_identifiers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/__init__.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/README.md
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/PKG-INFO
```

### Comparing `django_bg_task-0.0.1/.pre-commit-config.yaml` & `django_bg_task-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/.pylintrc` & `django_bg_task-0.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/manage.py` & `django_bg_task-0.0.2/manage.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/.github/workflows/publish.yaml` & `django_bg_task-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/common.py` & `django_bg_task-0.0.2/django_task/common.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/handler.py` & `django_bg_task-0.0.2/django_task/handler.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/models.py` & `django_bg_task-0.0.2/django_task/models.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/services.py` & `django_bg_task-0.0.2/django_task/services.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/settings.py` & `django_bg_task-0.0.2/django_task/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from django.conf import settings
 
 # pylint: disable=invalid-name
 
-INSTALLED_APPS = ["task_manager"]
+INSTALLED_APPS = ["django_task"]
 
 
 class AppSettings:
     def __init__(self):
         self.app_settings = getattr(settings, "DRF_MISC_SETTINGS", {})
 
     @property
```

### Comparing `django_bg_task-0.0.1/django_task/views.py` & `django_bg_task-0.0.2/django_task/views.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0001_initial.py` & `django_bg_task-0.0.2/django_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0002_alter_task_status.py` & `django_bg_task-0.0.2/django_task/migrations/0002_alter_task_status.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0005_rename_arguments_task_args_and_more.py` & `django_bg_task-0.0.2/django_task/migrations/0005_rename_arguments_task_args_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0006_remove_task_exception_task_failed_reason_and_more.py` & `django_bg_task-0.0.2/django_task/migrations/0006_remove_task_exception_task_failed_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0007_alter_task_created_at_alter_task_failed_reason_and_more.py` & `django_bg_task-0.0.2/django_task/migrations/0007_alter_task_created_at_alter_task_failed_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/django_task/migrations/0008_remove_task_identifier_task_identifiers.py` & `django_bg_task-0.0.2/django_task/migrations/0008_remove_task_identifier_task_identifiers.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/.gitignore` & `django_bg_task-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/LICENSE` & `django_bg_task-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/README.md` & `django_bg_task-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.1/pyproject.toml` & `django_bg_task-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "django-bg-task"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension for managing background task with celery"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_bg_task-0.0.1/PKG-INFO` & `django_bg_task-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bg-task
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small Django DRF extension for managing background task with celery
 Project-URL: Homepage, https://github.com/abhishm20/django-task
 Project-URL: Bug Tracker, https://github.com/abhishm20/django-task/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

