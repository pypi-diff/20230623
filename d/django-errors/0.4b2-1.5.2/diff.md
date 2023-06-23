# Comparing `tmp/django_errors-0.4b2.tar.gz` & `tmp/django-errors-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_errors-0.4b2.tar", last modified: Sun Jan 17 09:36:28 2021, max compression
+gzip compressed data, was "django-errors-1.5.2.tar", last modified: Fri Jun 23 18:51:42 2023, max compression
```

## Comparing `django_errors-0.4b2.tar` & `django-errors-1.5.2.tar`

### file list

```diff
@@ -1,66 +1,89 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2021-01-17 09:35:46.000000 django_errors-0.4b2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      247 2021-01-17 09:35:46.000000 django_errors-0.4b2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3491 2021-01-17 09:36:28.000000 django_errors-0.4b2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2021-01-17 09:35:46.000000 django_errors-0.4b2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/apps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/cn/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/cn/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/cn/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     1893 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/de/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/de/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/en/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/en/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     1893 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/es/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/es/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/fr/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     1939 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/it/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/it/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1487 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2373 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/lt/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      484 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/ru/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2017 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/templates/errors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      804 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/templates/errors/400.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      535 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/templates/errors/403.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/templates/errors/404.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/templates/errors/500.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors/tests/__pycache__/
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2021-01-17 09:35:55.000000 django_errors-0.4b2/django_errors/tests/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)      541 2021-01-17 09:35:55.000000 django_errors-0.4b2/django_errors/tests/__pycache__/test_settings.cpython-37.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2486 2021-01-17 09:35:55.000000 django_errors-0.4b2/django_errors/tests/__pycache__/tests.cpython-37.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)      416 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/tests/test_settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2102 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/tests/tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1605 2021-01-17 09:35:46.000000 django_errors-0.4b2/django_errors/views.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3491 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-17 09:35:50.000000 django_errors-0.4b2/django_errors.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-01-17 09:36:28.000000 django_errors-0.4b2/django_errors.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2021-01-17 09:36:28.000000 django_errors-0.4b2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2021-01-17 09:35:46.000000 django_errors-0.4b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.473109 django-errors-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 18:51:23.000000 django-errors-1.5.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-23 18:51:23.000000 django-errors-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 18:51:23.000000 django-errors-1.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 18:51:23.000000 django-errors-1.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-23 18:51:23.000000 django-errors-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-23 18:51:23.000000 django-errors-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-23 18:51:42.473109 django-errors-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-23 18:51:23.000000 django-errors-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-23 18:51:23.000000 django-errors-1.5.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 18:51:23.000000 django-errors-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.465109 django-errors-1.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 18:51:23.000000 django-errors-1.5.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 18:51:23.000000 django-errors-1.5.2/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 18:51:42.473109 django-errors-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 18:51:23.000000 django-errors-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.465109 django-errors-1.5.2/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/cn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.457110 django-errors-1.5.2/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.469109 django-errors-1.5.2/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.461109 django-errors-1.5.2/src/django_errors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.473109 django-errors-1.5.2/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-23 18:51:23.000000 django-errors-1.5.2/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.465109 django-errors-1.5.2/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-23 18:51:42.000000 django-errors-1.5.2/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 18:51:42.000000 django-errors-1.5.2/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:51:42.000000 django-errors-1.5.2/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:51:41.000000 django-errors-1.5.2/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 18:51:42.000000 django-errors-1.5.2/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 18:51:42.000000 django-errors-1.5.2/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:42.473109 django-errors-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:51:23.000000 django-errors-1.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-23 18:51:23.000000 django-errors-1.5.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-23 18:51:23.000000 django-errors-1.5.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 18:51:23.000000 django-errors-1.5.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-23 18:51:23.000000 django-errors-1.5.2/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 18:51:23.000000 django-errors-1.5.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django_errors-0.4b2/LICENSE` & `django-errors-1.5.2/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2016, DLRSP
+Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `django_errors-0.4b2/PKG-INFO` & `django-errors-1.5.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,68 @@
-Metadata-Version: 2.1
-Name: django_errors
-Version: 0.4b2
-Summary: Wrapper Views for common errors
-Home-page: https://github.com/DLRSP/django-errors
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
-License: MIT
-Description: # django-errors [![PyPi license](https://img.shields.io/pypi/l/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
-        
-        ## Pypi [![PyPi status](https://img.shields.io/pypi/status/django-errors.svg)](https://pypi.python.org/pypi/django_errors) [![PyPi version](https://img.shields.io/pypi/v/django-errors.svg)](https://pypi.python.org/pypi/django_errors) [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors) [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors) [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors) [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
-        
-        ```shell
-        pip install django-errors
-        ```
-        
-        ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
-        
-        ## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-errors?branch=master) [![travis-ci.org](https://travis-ci.org/DLRSP/django-errors.svg?branch=master)](https://travis-ci.org/DLRSP/django-errors) [![circleci.com](https://circleci.com/gh/DLRSP/django-errors.svg?style=shield&circle-token=b2c2b63556f8dfc17f9058adfbaae1fd16b3bc01)](https://circleci.com/gh/DLRSP/django-errors)
-        
-        ## Configurations
-        
-        1. modify `settings.py` by adding the app to `INSTALLED_APPS`:
-        ```python
-        INSTALLED_APPS = [
-            # ...
-            "django_errors",
-            # ...
-        ]
-        ```
-        
-        2. Finally, modify your project `urls.py` with handlers for all errors:
-        ```python
-        # ...other imports...
-        from django_errors import views as errors_views
-        
-        urlpatterns = [
-            # ...other urls...
-        ]
-        
-        handler400 = errors_views.custom_400
-        """ Handle 400 error """
-        
-        handler403 = errors_views.custom_403
-        """ Handle 403 error """
-        
-        handler404 = errors_views.custom_404
-        """ Handle 404 error """
-        
-        handler500 = errors_views.custom_500
-        """ Handle 500 error """
-        ```
-        
-        ## Run Example Project
-        
-        ```shell
-        cd example
-        python manage.py runserver
-        ```
-        
-        Now browser the app @ http://127.0.0.1:8000
-        
-        ## About Landing Page Errors
-        http://www.onextrapixel.com/2011/03/09/the-secret-of-a-successful-error-page-with-35-amazing-404-page-designs/
-        http://www.onextrapixel.com/2011/10/21/applying-defensive-design-for-the-web/
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP
-Description-Content-Type: text/markdown
+# django-errors [![PyPi license](https://img.shields.io/pypi/l/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+[![PyPi version](https://img.shields.io/pypi/v/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-errors?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/master) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+
+## Check Demo Project
+* Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
+
+## Requirements
+-   Python 3.8+ supported.
+-   Django 3.2+ supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-errors
+```
+
+2. modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = [
+    # ...
+    "django_errors",
+    # ...
+]
+```
+
+3. Finally, modify your project `urls.py` with handlers for all errors:
+```python
+# ...other imports...
+from django_errors import views as errors_views
+
+urlpatterns = [
+    # ...other urls...
+]
+
+handler400 = errors_views.custom_400
+""" Handle 400 error """
+
+handler403 = errors_views.custom_403
+""" Handle 403 error """
+
+handler404 = errors_views.custom_404
+""" Handle 404 error """
+
+handler500 = errors_views.custom_500
+""" Handle 500 error """
+```
+
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-errors https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django_errors-0.4b2/django_errors/locale/it/LC_MESSAGES/django.mo` & `django-errors-1.5.2/src/django_errors/locale/it/LC_MESSAGES/django.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,44 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-01-04 16:15+0100\n"
 "PO-Revision-Date: 2016-01-04 16:15+0100\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.6\n"
 
-msgid "An app to manage errors page ..."
-msgstr "Una app per gestire le pagine di errorre ..."
-
 msgid "Bad Request"
 msgstr "Brutta Richiesta"
 
-msgid "Details"
-msgstr "Details"
-
-msgid "I'm sorry, an error has occurred with the application."
-msgstr "Mi dispiace, si è verificato un errore con il programma."
-
-msgid "I'm sorry, we don't have a page with that URL."
-msgstr "Mi dispiace, non abbiamo una pagina con questo URL."
-
 msgid "Internal Server Error"
 msgstr "Errore Interno del Server"
 
+msgid "Method Not Allowed"
+msgstr "Metodo non consentito"
+
 msgid "Page Not Found"
 msgstr "Pagina non trovata"
 
 msgid "Permission Denied"
 msgstr "Permesso Negato"
 
-msgid "Server Error"
-msgstr "Errore del Server "
+msgid "Sorry, an error has occurred with the application."
+msgstr "Scusa, si è verificato un errore con il programma."
+
+msgid "Sorry, the used method is not allowed for the page with that URL."
+msgstr "Scusa, il metodo usato non è consentito per la pagina con questo URL."
 
-msgid "The browser SHOULD NOT repeat the request without modifications."
-msgstr "Il browser NON DEVE ripetere la richiesta senza modifiche."
+msgid "Sorry, we don't have a page with that URL."
+msgstr "Scusa, non abbiamo una pagina con questo URL."
 
 msgid ""
 "The request could not be understood by the server due to malformed syntax."
 msgstr ""
 "La richiesta non può essere compresa dal server a causa di sintassi errata."
 
 msgid "You don't have permissions to see this page!"
```

### Comparing `django_errors-0.4b2/django_errors/tests/tests.py` & `django-errors-1.5.2/tests/test_errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-"""Unit Tests for the Example module"""
-
-# pylint: disable=R0904, C0103
+"""Unit Tests for the module"""
+import logging
 
 from django.test import TestCase
 
-from django.core.exceptions import ObjectDoesNotExist
-import logging
-
-LOGGER = logging.getLogger(name='example')
+LOGGER = logging.getLogger(name="django-errors")
 
 
-class ExampleTestCase(TestCase):
-    """Test Case for Social Profile"""
+class ErrorsTestCase(TestCase):
+    """Test Case for django-errors"""
 
     def setUp(self):
         """Set up common assets for tests"""
-        LOGGER.debug("Example Tests setUp")
+        LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
-        LOGGER.debug("Example Tests tearDown")
+        LOGGER.debug("Tests tearDown")
 
     def test_400_urls(self):
         """Test the url of 400 page."""
         LOGGER.debug("400 Test Redirect URLs")
-        response = self.client.get('/400/', follow=True)
+        response = self.client.get("/test-400/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(400, response.status_code)
 
     def test_403_urls(self):
         """Test the url of 403 page."""
         LOGGER.debug("403 Test Redirect URLs")
-        response = self.client.get('/403/', follow=True)
+        response = self.client.get("/test-403/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(403, response.status_code)
 
     def test_404_urls(self):
         """Test the url of 404 page."""
         LOGGER.debug("404 Test URLs")
-        response = self.client.get('/404/', follow=True)
+        response = self.client.get("/test-404/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
 
+    def test_405_urls(self):
+        """Test the url of 404 page."""
+        LOGGER.debug("405 Test GET URLs with only POST")
+        response = self.client.get("/test-405/", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(405, response.status_code)
+
     def test_not_exist_urls(self):
         """Test that redirects kicking in when trying to go to 404 page."""
         LOGGER.debug("404 Test Redirect URLs")
-        response = self.client.get('/UrlShouldNotExist/', follow=True)
+        response = self.client.get("/UrlShouldNotExist/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(404, response.status_code)
 
     def test_500_urls(self):
         """Test the url of 500 page."""
         LOGGER.debug("500 Test Redirect URLs")
-        response = self.client.get('/500/', follow=True)
+        response = self.client.get("/test-500/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(500, response.status_code)
 
     # def test_X_redirect_urls(self):
     # """Test that redirects end urls"""
     # LOGGER.debug("Test X Redirect URLs")
     # response = self.client.get('/403/', follow=True)
```

