# Comparing `tmp/django-glue-0.2.6.tar.gz` & `tmp/django-glue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.2.6.tar", last modified: Thu Nov 10 06:35:23 2022, max compression
+gzip compressed data, was "django-glue-0.3.0.tar", last modified: Thu Jun 22 22:14:13 2023, max compression
```

## Comparing `django-glue-0.2.6.tar` & `django-glue-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.747420 django-glue-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-10 06:35:14.000000 django-glue-0.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-10 06:35:14.000000 django-glue-0.2.6/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-11-10 06:35:14.000000 django-glue-0.2.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-10 06:35:14.000000 django-glue-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-11-10 06:35:23.747420 django-glue-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-11-10 06:35:14.000000 django-glue-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (121)    10807 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/json.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.739420 django-glue-0.2.6/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.739420 django-glue-0.2.6/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/static/django_glue/js/ajax.js
--rw-r--r--   0 runner    (1001) docker     (121)    39713 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/static/django_glue/js/alpine.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    20763 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/static/django_glue/js/axios.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/static/django_glue/js/csrf.js
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/static/django_glue/js/django_glue.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.739420 django-glue-0.2.6/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/templates/django_glue/django_glue.html
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/templates/django_glue/django_glue_core.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-10 06:35:14.000000 django-glue-0.2.6/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.743420 django-glue-0.2.6/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-10 06:35:23.000000 django-glue-0.2.6/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-10 06:35:14.000000 django-glue-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-10 06:35:23.747420 django-glue-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-11-10 06:35:14.000000 django-glue-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.747420 django-glue-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:23.747420 django-glue-0.2.6/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-10 06:35:14.000000 django-glue-0.2.6/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 22:14:02.000000 django-glue-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 22:14:02.000000 django-glue-0.3.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 22:14:02.000000 django-glue-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 22:14:02.000000 django-glue-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 22:14:13.025857 django-glue-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-22 22:14:02.000000 django-glue-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_response.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 22:14:02.000000 django-glue-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 22:14:13.025857 django-glue-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-22 22:14:02.000000 django-glue-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/wsgi.py
```

### Comparing `django-glue-0.2.6/CHANGELOG.md` & `django-glue-0.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Changelog for Django Glue
 
 ## 0.3.0
 
 #### Features
-- You can now glue methods.
-
+- You can now glue django model methods (this works on both model objects and query sets).
+- Now works with all javascript not just alpine.
 
 #### Changes
-- Clean up internal functions to more efficient.
+- Clean up internal functions to more efficient and secure.
+- Remove Alpine.js and return to vanilla so that people can use their own libraries.
+- Complete overhaul of the server side and front end code.
 
 ## 0.2.6
 
 #### Bugs
 - Fixed issue with building context dictionaries on non glue views.
 
 ## 0.2.5
```

### Comparing `django-glue-0.2.6/LICENSE.md` & `django-glue-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.2.6/PKG-INFO` & `django-glue-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.2.6
+Version: 0.3.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
-Author: Nathan Johnson & Wesley Howery
+Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE.md
 
 # django-glue
 
 We built Django Glue to help solve the problem of fluid interactions between the front and back ends of a Django application.
 Our end goal is to bring as much front end power to the Django framework as possible while remaining pythonic.
```

### Comparing `django-glue-0.2.6/README.md` & `django-glue-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.2.6/django_glue/middleware.py` & `django-glue-0.3.0/django_glue/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from django.urls import resolve
 
-from django_glue.glue import clean_glue_session
+from django_glue.sessions import GlueSession, GlueKeepLiveSession
 
 
 class GlueMiddleware(object):
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
         response = self.get_response(request)
         return response
 
-    def process_view(self, request, view_func, view_args, view_kwargs):
+    @staticmethod
+    def process_view(request, view_func, view_args, view_kwargs):
         current_url = resolve(request.path_info).url_name
 
         if current_url != 'django_glue_handler':
-            clean_glue_session(request)
+            glue_session = GlueSession(request)
+            glue_keep_live_session = GlueKeepLiveSession(request)
+
+            glue_session.clean(glue_keep_live_session.clean_and_get_expired_unique_name_set())
 
         return None
```

### Comparing `django-glue-0.2.6/django_glue/templatetags/django_glue.py` & `django-glue-0.3.0/django_glue/templatetags/django_glue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import logging, json
+import json
 
 from django import template
-from django.template.defaultfilters import stringfilter
 from django.utils.safestring import mark_safe
 
 from django_glue.conf import settings
 
 register = template.Library()
 
 
 @register.inclusion_tag('django_glue/django_glue.html', takes_context=True)
 def glue_init(context):
     return context
 
 
-@register.inclusion_tag('django_glue/django_glue_core.html', takes_context=True)
-def glue_init_core(context):
-    return context
-
-
 @register.simple_tag(takes_context=True)
 def glue_context_data_str(context):
     return mark_safe(str(json.dumps(context[settings.DJANGO_GLUE_CONTEXT_NAME])))
 
 
 @register.simple_tag(takes_context=True)
 def glue_context_keep_live_str(context):
@@ -44,11 +38,11 @@
     def __init__(self, unique_name, field):
         self.unique_name = unique_name
         self.field = field
 
     def render(self, context):
         html_attr_str = ''
 
-        for key, val in context[settings.DJANGO_GLUE_CONTEXT_NAME][self.unique_name]['fields'][self.field]['html_attr'].items():
+        for key, val in context[settings.DJANGO_GLUE_CONTEXT_NAME]['context'][self.unique_name]['fields'][self.field]['html_attr'].items():
             html_attr_str = f'{key}="{val}" '
 
         return html_attr_str
```

### Comparing `django-glue-0.2.6/django_glue/utils.py` & `django-glue-0.3.0/django_glue/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+import inspect
 import logging, pickle, base64, json
+from typing import Optional, Callable
 
-from django.core import exceptions, serializers
-from django.core.serializers.json import DjangoJSONEncoder
+from django.core import exceptions
 
-from django_glue.conf import settings
-
-
-def camel_to_snake(string):
-    return ''.join(['_' + c.lower() if c.isupper() else c for c in string]).lstrip('_')
+from django_glue.core.utils import serialize_object_to_json
+from django_glue.data_classes import GlueModelFieldData
 
 
 def decode_query_set_from_str(query_set_string):
     query = pickle.loads(base64.b64decode(query_set_string))
     decoded_query_set = query.model.objects.all()
     decoded_query_set.query = query
     return decoded_query_set
@@ -35,96 +33,83 @@
     return form_field.widget_attrs(form_field.widget)
 
 
 def generate_field_dict(model_object, fields, exclude):
     fields_dict = dict()
 
     model = type(model_object)
-    json_model = json.loads(serialize_object_to_json(model_object, fields, exclude))[0]
+    json_model = json.loads(serialize_object_to_json(model_object))[0]
 
     for field in model._meta.fields:
         try:
             if field_name_included(field.name, fields, exclude):
                 if hasattr(field, 'get_internal_type'):
                     if field.name == 'id':
                         field_value = json_model['pk']
                         field_attr = ''
                     else:
                         field_value = json_model['fields'][field.name]
                         field_attr = generate_field_attr_dict(field)
 
-                    fields_dict[field.name] = {
-                        'type': field.get_internal_type(),
-                        'value': field_value,
-                        'html_attr': field_attr,
-                    }
+                    fields_dict[field.name] = GlueModelFieldData(
+                        type=field.get_internal_type(),
+                        value=field_value,
+                        html_attr=field_attr,
+                    ).to_dict()
 
         except:
-            raise f'Invalid field or exclude for model type {model.__class__.__name__}'
+            raise f'Field "{field.name}" is invalid field or exclude for model type "{model.__class__.__name__}"'
 
     return fields_dict
 
 
+def generate_method_list(model_object, methods: tuple) -> list:
+    methods_list = list()
+
+    model = type(model_object)
+
+    if methods[0] != '__none__':
+        for method in methods:
+            if hasattr(model_object, method):
+                methods_list.append(method)
+            else:
+                raise f'Method "{method}" is invalid for model type "{model.__class__.__name__}"'
+
+    return methods_list
+
+
 def generate_simple_field_dict(model_object, fields, exclude):
     fields_dict = generate_field_dict(model_object, fields, exclude)
     simple_fields_dict = {}
 
     for key, val in fields_dict.items():
         simple_fields_dict[key] = val['value']
 
     return simple_fields_dict
 
 
 def get_fields_from_model(model):
     return [field for field in model._meta.fields]
 
 
-def process_and_save_form_values(model_object, form_values_dict, fields, exclude):
-    logging.warning(f'{model_object = }')
-
-    try:
-        for key, val in form_values_dict.items():
-            if key != 'id':
-                if field_name_included(key, fields, exclude):
-                    model_object.__dict__[key] = val
-
-        model_object.full_clean()
-        model_object.save()
-        logging.warning(f'{model_object = }')
-
-    except exceptions.ValidationError as e:
-        logging.warning(f'Validation Failed {e = }')
-        return {
-            'type': 'error',
-            'message_dict': e.message_dict
-        }
-
-    else:
-        logging.warning(f'Validation Successful')
-        return {
-            'type': 'success',
-        }
-
-
-def process_and_save_field_value(model_object, field_name, value, fields, exclude):
-    logging.warning(f'{field_name = } {value = }')
-    try:
-        if field_name_included(field_name, fields, exclude):
-            model_object.__dict__[field_name] = value
-            model_object.full_clean()
-            model_object.save()
-
-    except exceptions.ValidationError as e:
-        logging.warning(f'Validation Failed {e = }')
-        return {
-            'type': 'error',
-            'message_dict': e.message_dict
-        }
-
-    else:
-        return {
-            'type': 'success',
-        }
-
+def check_valid_method_kwargs(method: Callable, kwargs: Optional[dict]):
+    for kwarg in kwargs:
+        if kwarg not in inspect.signature(method).parameters.keys():
+            return False
+    return True
+
+
+def type_set_method_kwargs(method: Callable, kwargs: Optional[dict]) -> dict:
+    type_set_kwargs = {}
+
+    # This is a dict consisting of all kwargs and there type annotations (If they have type annotations)
+    annotations = inspect.getfullargspec(method).annotations
+
+    for kwarg in kwargs:
+        if kwarg in annotations:
+            # Converts the kwarg to match the type specified in on the methods kwargs
+            type_set_kwargs[kwarg] = inspect.getfullargspec(method).annotations[kwarg](kwargs[kwarg])
+        else:
+            # If there is not a type annotation, the value remains the same
+            type_set_kwargs[kwarg] = kwargs[kwarg]
 
-def serialize_object_to_json(model_object, fields, exclude):
-    return serializers.serialize('json', [model_object, ])
+    return type_set_kwargs
```

### Comparing `django-glue-0.2.6/django_glue.egg-info/PKG-INFO` & `django-glue-0.3.0/django_glue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.2.6
+Version: 0.3.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
-Author: Nathan Johnson & Wesley Howery
+Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE.md
 
 # django-glue
 
 We built Django Glue to help solve the problem of fluid interactions between the front and back ends of a Django application.
 Our end goal is to bring as much front end power to the Django framework as possible while remaining pythonic.
```

### Comparing `django-glue-0.2.6/django_glue.egg-info/SOURCES.txt` & `django-glue-0.3.0/django_glue.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 django_glue/__init__.py
 django_glue/conf.py
 django_glue/context_processors.py
+django_glue/data_classes.py
+django_glue/enums.py
 django_glue/glue.py
 django_glue/handlers.py
-django_glue/json.py
 django_glue/middleware.py
+django_glue/responses.py
+django_glue/sessions.py
 django_glue/settings.py
 django_glue/urls.py
 django_glue/utils.py
 django_glue/views.py
 django_glue.egg-info/PKG-INFO
 django_glue.egg-info/SOURCES.txt
 django_glue.egg-info/dependency_links.txt
 django_glue.egg-info/not-zip-safe
 django_glue.egg-info/requires.txt
 django_glue.egg-info/top_level.txt
-django_glue/migrations/__init__.py
-django_glue/static/django_glue/js/ajax.js
-django_glue/static/django_glue/js/alpine.min.js
-django_glue/static/django_glue/js/axios.min.js
-django_glue/static/django_glue/js/csrf.js
-django_glue/static/django_glue/js/django_glue.js
+django_glue/core/__init__.py
+django_glue/core/utils.py
+django_glue/services/__init__.py
+django_glue/services/model_objects.py
+django_glue/services/query_sets.py
+django_glue/services/services.py
+django_glue/static/django_glue/js/django_glue_ajax.js
+django_glue/static/django_glue/js/django_glue_csrf.js
+django_glue/static/django_glue/js/django_glue_model_object.js
+django_glue/static/django_glue/js/django_glue_query_set.js
+django_glue/static/django_glue/js/django_glue_response.js
 django_glue/templates/django_glue/django_glue.html
-django_glue/templates/django_glue/django_glue_core.html
 django_glue/templatetags/__init__.py
 django_glue/templatetags/django_glue.py
 tests/__init__.py
 tests/admin.py
 tests/manage.py
 tests/models.py
 tests/settings.py
```

### Comparing `django-glue-0.2.6/setup.py` & `django-glue-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,27 +13,25 @@
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords=["glue", "django", "backend", "frontend", "javascript", "active server pages"],
-    author="Nathan Johnson & Wesley Howery",
+    author="Nathan Johnson, Austin Sauer & Wesley Howery",
     author_email="info@stratusadv.com",
     url="https://github.com/stratusadv/django-glue",
     license="MIT",
     packages=find_packages(exclude=["docs"]),
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     install_requires="django>=3.2",
 )
```

### Comparing `django-glue-0.2.6/tests/manage.py` & `django-glue-0.3.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.2.6/tests/migrations/0001_initial.py` & `django-glue-0.3.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.2.6/tests/models.py` & `django-glue-0.3.0/tests/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from django.db import models
 from django.utils.timezone import now
 
+from django_glue.data_classes import GlueJsonResponseData
+
 
 class TestModel(models.Model):
     first_name = models.CharField(max_length=32)
     last_name = models.CharField(max_length=32)
     description = models.TextField()
     favorite_number = models.IntegerField()
     anniversary_datetime = models.DateTimeField(default=now)
     birth_date = models.DateField(default=now)
     weight_lbs = models.DecimalField(max_digits=7, decimal_places=3)
 
     def __str__(self):
         return f'{self.first_name} {self.last_name}'
 
-    def django_glue_create(self, request):
-        pass
-
-    def django_glue_update(self, request):
-        pass
-
-    def django_glue_delete(self, request):
-        self.delete()
+    def is_lighter_than(self, check_weight: float) -> bool:
+        if self.weight_lbs < check_weight:
+            return True
+        return False
 
-    def django_glue_view(self, request):
-        pass
+    def get_full_name(self):
+        return f'{self.first_name} {self.last_name}'
 
 
 class BigTestModel(models.Model):
     big_integer_field = models.BigIntegerField()
     binary_field = models.BinaryField()
     boolean_field = models.BooleanField()
     char_field = models.CharField(max_length=8)
@@ -51,18 +49,9 @@
     time_field = models.TimeField()
     url_field = models.URLField()
     uuid_field = models.UUIDField()
 
     def __str__(self):
         return f'{self.char_field}'
 
-    def django_glue_create(self, request):
-        pass
-
-    def django_glue_update(self, request):
-        pass
 
-    def django_glue_delete(self, request):
-        self.delete()
 
-    def django_glue_view(self, request):
-        pass
```

### Comparing `django-glue-0.2.6/tests/settings.py` & `django-glue-0.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.2.6/tests/utils.py` & `django-glue-0.3.0/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 
 from tests.models import TestModel, BigTestModel
 
 FIRST_NAME_TUPLE = (
     'Fred',
     'Jane',
     'Janet',
+    'Austin',
     'Johnny',
     'Nathan',
     'Robert',
     'Ted',
+    'Wesley',
 )
 
 LAST_NAME_TUPLE = (
     'Doe',
-    'Hansen',
     'Johnson',
+    'Hansen',
     'Mancal',
     'Smith',
     'Waldern',
+    'Howery',
     'Wilson',
+    'Sauer',
 )
 
 DESCRIPTION_WORD_TUPLE = (
     'I',
     'a',
     'are'
     'artsy',
```

### Comparing `django-glue-0.2.6/tests/views.py` & `django-glue-0.3.0/tests/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,32 +4,52 @@
 
 from tests.models import TestModel
 from tests.utils import generate_randomized_test_model, generate_big_test_model
 from django_glue.glue import add_glue
 
 
 class TestView(TemplateView):
-    template_name = 'test.html'
+    template_name = 'page/test_glue_page.html'
 
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
         test_model_object = generate_randomized_test_model()
 
         logging.warning(f'Added TestModel object.')
 
-        add_glue(self.request, 'test_model_1', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime',))
+        add_glue(self.request, 'test_model_1', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'), methods=['is_lighter_than', 'get_full_name'])
         add_glue(self.request, 'test_model_2', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
         add_glue(self.request, 'test_model_3', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'))
         add_glue(self.request, 'test_model_4', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
         logging.warning('Added model object glue for TestModel Object in write mode')
 
-        add_glue(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'change', exclude=('birth_date', 'anniversary_datetime'))
+        add_glue(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('birth_date', 'anniversary_datetime'), methods=['is_lighter_than', 'get_full_name'])
         add_glue(self.request, 'test_query_2', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'add', exclude=('birth_date', 'anniversary_datetime'))
-        add_glue(self.request, 'test_query_3', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('birth_date', 'anniversary_datetime'))
+        add_glue(self.request, 'test_query_3', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'change', exclude=('birth_date', 'anniversary_datetime'))
         logging.warning('Added model query set glue for TestModel Object in read mode')
 
         big_test_model_object = generate_big_test_model()
 
         logging.warning(f'Added BigTestModel object.')
 
         return context_data
+
+
+class OtherView(TemplateView):
+    template_name = 'page/other_glue_page.html'
+    def get_context_data(self, **kwargs):
+        context_data = super().get_context_data(**kwargs)
+
+        other_test_model_object = generate_randomized_test_model()
+
+        logging.warning(f'Added Other TestModel object.')
+
+        add_glue(self.request, 'other_test_model_1', other_test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime',))
+
+        logging.warning('Added model object glue for Other TestModel Object in write mode')
+
+        return context_data
+
+def benchmark_run_view(request):
+    # this view should take an integer that determines how many glue connections to make.
+    pass
```

