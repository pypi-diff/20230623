# Comparing `tmp/django-partitioned-audit-1.0.2.tar.gz` & `tmp/django-partitioned-audit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-partitioned-audit-1.0.2.tar", last modified: Fri Jun 23 11:04:58 2023, max compression
+gzip compressed data, was "django-partitioned-audit-1.0.3.tar", last modified: Fri Jun 23 11:14:14 2023, max compression
```

## Comparing `django-partitioned-audit-1.0.2.tar` & `django-partitioned-audit-1.0.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      496 2023-06-23 11:04:25.000000 django-partitioned-audit-1.0.2/.bumpversion.cfg
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      102 2023-06-23 10:21:10.000000 django-partitioned-audit-1.0.2/.gitignore
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1721 2023-06-23 09:24:58.000000 django-partitioned-audit-1.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      375 2023-06-15 08:58:25.000000 django-partitioned-audit-1.0.2/.pylintrc
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1510 2023-06-15 05:52:04.000000 django-partitioned-audit-1.0.2/LICENSE
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     5865 2023-06-23 11:03:17.000000 django-partitioned-audit-1.0.2/Makefile
--rw-rw-r--   0 horacio   (1000) horacio   (1000)    14510 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/PKG-INFO
--rw-rw-r--   0 horacio   (1000) horacio   (1000)    13371 2023-06-23 10:47:57.000000 django-partitioned-audit-1.0.2/README.rst
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)       81 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1143 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/admin.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      155 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/apps.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit/management/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/management/__init__.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit/management/commands/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/management/commands/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     5455 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/management/commands/manage_partition_tables.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      984 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/0001_initial.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1989 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/0002_trigger_audit_entry_creator_func_v2.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-14 07:42:31.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1418 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/models.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2966 2023-06-23 09:18:01.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_info.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2997 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_base.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     5062 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_plan.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1834 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_time_range.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3011 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/time_range_partitioning.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3373 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/signals.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      278 2023-06-15 09:25:46.000000 django-partitioned-audit-1.0.2/django_partitioned_audit/utils.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)    14510 2023-06-23 11:04:58.000000 django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/PKG-INFO
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3086 2023-06-23 11:04:58.000000 django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/SOURCES.txt
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        1 2023-06-23 11:04:58.000000 django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/dependency_links.txt
--rw-rw-r--   0 horacio   (1000) horacio   (1000)       25 2023-06-23 11:04:58.000000 django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/top_level.txt
--rw-rw-r--   0 horacio   (1000) horacio   (1000)       99 2023-06-23 10:10:50.000000 django-partitioned-audit-1.0.2/pyproject.toml
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      211 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/pytest.ini
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1058 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/setup.cfg
--rw-rw-r--   0 horacio   (1000) horacio   (1000)       38 2023-06-14 07:42:31.000000 django-partitioned-audit-1.0.2/setup.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/app_django/
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/app_django/app/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/app/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      586 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/app_django/app/admin.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      174 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/apps.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.633821 django-partitioned-audit-1.0.2/tests/app_django/app/management/
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/app_django/app/management/commands/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     4013 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/app_django/app/management/commands/stresstest.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1314 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/app_django/app/management/commands/update_customer.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/app_django/app/migrations/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      568 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/app/migrations/0001_initial.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      786 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/migrations/0002_invoice_product.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/app/migrations/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      451 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/models.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.633821 django-partitioned-audit-1.0.2/tests/app_django/app/templates/
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.637821 django-partitioned-audit-1.0.2/tests/app_django/app/templates/app/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      271 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/app/templates/app/customer_confirm_delete.html
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/app/templates/app/customer_form.html
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/templates/app/invoice_form.html
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/templates/app/product_form.html
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1374 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/app/views.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/tests/app_django/config/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/config/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      389 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/config/asgi.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      521 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1618 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings_boilerplate.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings_postgres12.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings_postgres13.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings_postgres14.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.2/tests/app_django/config/settings_postgres15.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      652 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/config/tox_settings.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      582 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_django/config/urls.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      389 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/config/wsgi.py
--rwxrwxr-x   0 horacio   (1000) horacio   (1000)      626 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.2/tests/app_django/manage.py
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/tests/app_install_test/
-drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:04:58.641821 django-partitioned-audit-1.0.2/tests/app_install_test/app_install_test_config/
--rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_install_test/app_install_test_config/__init__.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      581 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/app_install_test/app_install_test_config/settings.py
--rwxrwxr-x   0 horacio   (1000) horacio   (1000)      643 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.2/tests/app_install_test/manage.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3396 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/conftest.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1309 2023-06-23 09:47:22.000000 django-partitioned-audit-1.0.2/tests/docker-compose.yml
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      292 2023-06-23 10:30:28.000000 django-partitioned-audit-1.0.2/tests/requirements.in
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3839 2023-06-23 10:30:36.000000 django-partitioned-audit-1.0.2/tests/requirements.txt
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2066 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_audit_events_creation.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2259 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_concurrent.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3357 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_examples_on_readme.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     5966 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_management_commands.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1386 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_non_standard_pk.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2017 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_info.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     3022 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_base.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     2442 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_create.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     6558 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_simulate.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     6172 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_time_range.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     7551 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_time_range_plan.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1917 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.2/tests/test_partition_manager_truncate_63.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)     1971 2023-06-23 09:50:20.000000 django-partitioned-audit-1.0.2/tests/test_testing_app_without_audit.py
--rw-rw-r--   0 horacio   (1000) horacio   (1000)      449 2023-06-23 08:17:07.000000 django-partitioned-audit-1.0.2/tox.ini
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      496 2023-06-23 11:14:12.000000 django-partitioned-audit-1.0.3/.bumpversion.cfg
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      102 2023-06-23 10:21:10.000000 django-partitioned-audit-1.0.3/.gitignore
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1721 2023-06-23 09:24:58.000000 django-partitioned-audit-1.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      375 2023-06-15 08:58:25.000000 django-partitioned-audit-1.0.3/.pylintrc
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1510 2023-06-15 05:52:04.000000 django-partitioned-audit-1.0.3/LICENSE
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     6130 2023-06-23 11:13:37.000000 django-partitioned-audit-1.0.3/Makefile
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)    14316 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/PKG-INFO
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)    13177 2023-06-23 11:13:42.000000 django-partitioned-audit-1.0.3/README.rst
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)       81 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1143 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/admin.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      155 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/apps.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit/management/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/management/__init__.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit/management/commands/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/management/commands/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     5455 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/management/commands/manage_partition_tables.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      984 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/0001_initial.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1989 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/0002_trigger_audit_entry_creator_func_v2.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-14 07:42:31.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1418 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/models.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2966 2023-06-23 09:18:01.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_info.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2997 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_base.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     5062 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_plan.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1834 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_time_range.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3011 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/time_range_partitioning.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3373 2023-06-23 09:23:18.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/signals.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      278 2023-06-15 09:25:46.000000 django-partitioned-audit-1.0.3/django_partitioned_audit/utils.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)    14316 2023-06-23 11:14:14.000000 django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/PKG-INFO
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3086 2023-06-23 11:14:14.000000 django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/SOURCES.txt
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        1 2023-06-23 11:14:14.000000 django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/dependency_links.txt
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)       25 2023-06-23 11:14:14.000000 django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/top_level.txt
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)       99 2023-06-23 10:10:50.000000 django-partitioned-audit-1.0.3/pyproject.toml
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      211 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/pytest.ini
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1058 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/setup.cfg
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)       38 2023-06-14 07:42:31.000000 django-partitioned-audit-1.0.3/setup.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/tests/
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/tests/app_django/
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_django/app/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/app/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      586 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/app_django/app/admin.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      174 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/apps.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.464311 django-partitioned-audit-1.0.3/tests/app_django/app/management/
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_django/app/management/commands/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     4013 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/app_django/app/management/commands/stresstest.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1314 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/app_django/app/management/commands/update_customer.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_django/app/migrations/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      568 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/app/migrations/0001_initial.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      786 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/migrations/0002_invoice_product.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/app/migrations/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      451 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/models.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.468311 django-partitioned-audit-1.0.3/tests/app_django/app/templates/
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_django/app/templates/app/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      271 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/app/templates/app/customer_confirm_delete.html
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/app/templates/app/customer_form.html
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/templates/app/invoice_form.html
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      216 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/templates/app/product_form.html
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1374 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/app/views.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_django/config/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/config/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      389 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/config/asgi.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      521 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1618 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings_boilerplate.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings_postgres12.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings_postgres13.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings_postgres14.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      481 2023-06-23 09:25:39.000000 django-partitioned-audit-1.0.3/tests/app_django/config/settings_postgres15.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      652 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/config/tox_settings.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      582 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_django/config/urls.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      389 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/config/wsgi.py
+-rwxrwxr-x   0 horacio   (1000) horacio   (1000)      626 2023-06-19 12:19:35.000000 django-partitioned-audit-1.0.3/tests/app_django/manage.py
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_install_test/
+drwxrwxr-x   0 horacio   (1000) horacio   (1000)        0 2023-06-23 11:14:14.472311 django-partitioned-audit-1.0.3/tests/app_install_test/app_install_test_config/
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)        0 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_install_test/app_install_test_config/__init__.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      581 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/app_install_test/app_install_test_config/settings.py
+-rwxrwxr-x   0 horacio   (1000) horacio   (1000)      643 2023-06-19 14:27:17.000000 django-partitioned-audit-1.0.3/tests/app_install_test/manage.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3396 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/conftest.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1309 2023-06-23 09:47:22.000000 django-partitioned-audit-1.0.3/tests/docker-compose.yml
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      292 2023-06-23 10:30:28.000000 django-partitioned-audit-1.0.3/tests/requirements.in
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3839 2023-06-23 10:30:36.000000 django-partitioned-audit-1.0.3/tests/requirements.txt
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2066 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_audit_events_creation.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2259 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_concurrent.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3357 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_examples_on_readme.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     5966 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_management_commands.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1386 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_non_standard_pk.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2017 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_info.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     3022 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_base.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     2442 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_create.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     6558 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_simulate.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     6172 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_time_range.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     7551 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_time_range_plan.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1917 2023-06-23 09:23:39.000000 django-partitioned-audit-1.0.3/tests/test_partition_manager_truncate_63.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)     1971 2023-06-23 09:50:20.000000 django-partitioned-audit-1.0.3/tests/test_testing_app_without_audit.py
+-rw-rw-r--   0 horacio   (1000) horacio   (1000)      449 2023-06-23 08:17:07.000000 django-partitioned-audit-1.0.3/tox.ini
```

### Comparing `django-partitioned-audit-1.0.2/.pre-commit-config.yaml` & `django-partitioned-audit-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/LICENSE` & `django-partitioned-audit-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/Makefile` & `django-partitioned-audit-1.0.3/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -157,7 +157,14 @@
 
 bumpversion-patch: build-test-recreate build-test-run tox-some
 	$(VENVDIR)/bin/bumpversion --commit --tag release
 	$(MAKE) build-package
 	$(MAKE) build-upload
 	$(VENVDIR)/bin/bumpversion --commit --no-tag patch
 	# git push origin && git push origin --tags
+
+bumpversion-patch-quick: build-test-recreate build-test-run tox-latest
+	$(VENVDIR)/bin/bumpversion --commit --tag release
+	$(MAKE) build-package
+	$(MAKE) build-upload
+	$(VENVDIR)/bin/bumpversion --commit --no-tag patch
+	# git push origin && git push origin --tags
```

### Comparing `django-partitioned-audit-1.0.2/PKG-INFO` & `django-partitioned-audit-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-partitioned-audit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Keep audit log based on PostgreSql triggers and partitioned tables
 Home-page: https://gitlab.com/hgdeoro/django-partitioned-audit
 Author: Horacio G. de Oro
 Author-email: hgdeoro@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -34,15 +34,15 @@
 
 * Only PostgreSql supported.
 * Models to audit are configured in ``AppConfig``
 * Triggers are applied automatically when running ``python manage.py migrate``
 * The whole row is saved by the trigger by using PostgreSql's ``row_to_json()``
 * The audit table is partitioned
 * Management command `manage_partition_tables` creates required partitions
-  * there are 3 partition strategies: one per month, one per week, one per day.
+* There are 3 partition strategies: one partition per month, one per week, one per day.
 
 Quick start
 -----------
 
 1. Add "django_partitioned_audit" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
@@ -86,18 +86,14 @@
 Security of audit entries
 +++++++++++++++++++++++++
 
 DBA should correctly configure permissions, in a way that the user used to
 connect to the database from Django has permissions to INSERT rows in the
 ``trigger_audit_entries`` table, but NO permissions to UPDATE / DELETE them.
 
-If security is not important and you just want to avoid deleting the audit
-entries by accident, a solution could be
-https://docs.djangoproject.com/en/3.1/topics/db/multi-db/#automatic-database-routing
-
 
 How it works
 ------------
 
 #. A trigger is executed with each insert/update/delete operation
 
    * the database trigger is created by ``python manage.py migrate``.
```

### Comparing `django-partitioned-audit-1.0.2/README.rst` & `django-partitioned-audit-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 * Only PostgreSql supported.
 * Models to audit are configured in ``AppConfig``
 * Triggers are applied automatically when running ``python manage.py migrate``
 * The whole row is saved by the trigger by using PostgreSql's ``row_to_json()``
 * The audit table is partitioned
 * Management command `manage_partition_tables` creates required partitions
-  * there are 3 partition strategies: one per month, one per week, one per day.
+* There are 3 partition strategies: one partition per month, one per week, one per day.
 
 Quick start
 -----------
 
 1. Add "django_partitioned_audit" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
@@ -58,18 +58,14 @@
 Security of audit entries
 +++++++++++++++++++++++++
 
 DBA should correctly configure permissions, in a way that the user used to
 connect to the database from Django has permissions to INSERT rows in the
 ``trigger_audit_entries`` table, but NO permissions to UPDATE / DELETE them.
 
-If security is not important and you just want to avoid deleting the audit
-entries by accident, a solution could be
-https://docs.djangoproject.com/en/3.1/topics/db/multi-db/#automatic-database-routing
-
 
 How it works
 ------------
 
 #. A trigger is executed with each insert/update/delete operation
 
    * the database trigger is created by ``python manage.py migrate``.
```

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/admin.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/admin.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/management/commands/manage_partition_tables.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/management/commands/manage_partition_tables.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/0001_initial.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/migrations/0002_trigger_audit_entry_creator_func_v2.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/migrations/0002_trigger_audit_entry_creator_func_v2.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/models.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/models.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_info.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_info.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_base.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_base.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_plan.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_plan.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/partition_manager_time_range.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/partition_manager_time_range.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/partitions/time_range_partitioning.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/partitions/time_range_partitioning.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit/signals.py` & `django-partitioned-audit-1.0.3/django_partitioned_audit/signals.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/PKG-INFO` & `django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-partitioned-audit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Keep audit log based on PostgreSql triggers and partitioned tables
 Home-page: https://gitlab.com/hgdeoro/django-partitioned-audit
 Author: Horacio G. de Oro
 Author-email: hgdeoro@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -34,15 +34,15 @@
 
 * Only PostgreSql supported.
 * Models to audit are configured in ``AppConfig``
 * Triggers are applied automatically when running ``python manage.py migrate``
 * The whole row is saved by the trigger by using PostgreSql's ``row_to_json()``
 * The audit table is partitioned
 * Management command `manage_partition_tables` creates required partitions
-  * there are 3 partition strategies: one per month, one per week, one per day.
+* There are 3 partition strategies: one partition per month, one per week, one per day.
 
 Quick start
 -----------
 
 1. Add "django_partitioned_audit" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
@@ -86,18 +86,14 @@
 Security of audit entries
 +++++++++++++++++++++++++
 
 DBA should correctly configure permissions, in a way that the user used to
 connect to the database from Django has permissions to INSERT rows in the
 ``trigger_audit_entries`` table, but NO permissions to UPDATE / DELETE them.
 
-If security is not important and you just want to avoid deleting the audit
-entries by accident, a solution could be
-https://docs.djangoproject.com/en/3.1/topics/db/multi-db/#automatic-database-routing
-
 
 How it works
 ------------
 
 #. A trigger is executed with each insert/update/delete operation
 
    * the database trigger is created by ``python manage.py migrate``.
```

### Comparing `django-partitioned-audit-1.0.2/django_partitioned_audit.egg-info/SOURCES.txt` & `django-partitioned-audit-1.0.3/django_partitioned_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/setup.cfg` & `django-partitioned-audit-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-partitioned-audit
-version = 1.0.2
+version = 1.0.3
 description = Keep audit log based on PostgreSql triggers and partitioned tables
 long_description = file: README.rst
 url = https://gitlab.com/hgdeoro/django-partitioned-audit
 author = Horacio G. de Oro
 author_email = hgdeoro@gmail.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/admin.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/admin.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/management/commands/stresstest.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/management/commands/stresstest.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/management/commands/update_customer.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/management/commands/update_customer.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/migrations/0001_initial.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/migrations/0002_invoice_product.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/migrations/0002_invoice_product.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/app/views.py` & `django-partitioned-audit-1.0.3/tests/app_django/app/views.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/config/settings.py` & `django-partitioned-audit-1.0.3/tests/app_django/config/settings.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/config/settings_boilerplate.py` & `django-partitioned-audit-1.0.3/tests/app_django/config/settings_boilerplate.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/config/tox_settings.py` & `django-partitioned-audit-1.0.3/tests/app_django/config/tox_settings.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/config/urls.py` & `django-partitioned-audit-1.0.3/tests/app_django/config/urls.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_django/manage.py` & `django-partitioned-audit-1.0.3/tests/app_django/manage.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_install_test/app_install_test_config/settings.py` & `django-partitioned-audit-1.0.3/tests/app_install_test/app_install_test_config/settings.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/app_install_test/manage.py` & `django-partitioned-audit-1.0.3/tests/app_install_test/manage.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/conftest.py` & `django-partitioned-audit-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/docker-compose.yml` & `django-partitioned-audit-1.0.3/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/requirements.txt` & `django-partitioned-audit-1.0.3/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_audit_events_creation.py` & `django-partitioned-audit-1.0.3/tests/test_audit_events_creation.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_concurrent.py` & `django-partitioned-audit-1.0.3/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_examples_on_readme.py` & `django-partitioned-audit-1.0.3/tests/test_examples_on_readme.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_management_commands.py` & `django-partitioned-audit-1.0.3/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_non_standard_pk.py` & `django-partitioned-audit-1.0.3/tests/test_non_standard_pk.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_info.py` & `django-partitioned-audit-1.0.3/tests/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_base.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_base.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_create.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_create.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_simulate.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_simulate.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_time_range.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_time_range.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_time_range_plan.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_time_range_plan.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_partition_manager_truncate_63.py` & `django-partitioned-audit-1.0.3/tests/test_partition_manager_truncate_63.py`

 * *Files identical despite different names*

### Comparing `django-partitioned-audit-1.0.2/tests/test_testing_app_without_audit.py` & `django-partitioned-audit-1.0.3/tests/test_testing_app_without_audit.py`

 * *Files identical despite different names*

