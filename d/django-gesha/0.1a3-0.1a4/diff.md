# Comparing `tmp/django-gesha-0.1a3.tar.gz` & `tmp/django-gesha-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gesha-0.1a3.tar", last modified: Sat May 20 05:09:16 2023, max compression
+gzip compressed data, was "django-gesha-0.1a4.tar", last modified: Thu Jun 22 22:42:57 2023, max compression
```

## Comparing `django-gesha-0.1a3.tar` & `django-gesha-0.1a4.tar`

### file list

```diff
@@ -1,91 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.963458 django-gesha-0.1a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 05:09:05.000000 django-gesha-0.1a3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-20 05:09:05.000000 django-gesha-0.1a3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-20 05:09:05.000000 django-gesha-0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-20 05:09:16.975458 django-gesha-0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-20 05:09:05.000000 django-gesha-0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/django_gesha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 05:09:16.000000 django-gesha-0.1a3/django_gesha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/assets/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/settings.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-20 05:09:05.000000 django-gesha-0.1a3/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/gesha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.967458 django-gesha-0.1a3/gesha/static/gesha/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/static/gesha/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/gesha/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/templatetags/gesha.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gesha/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-20 05:09:05.000000 django-gesha-0.1a3/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.971458 django-gesha-0.1a3/js_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/context.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/converters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_src/urls.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/js_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/context.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/converters.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/helpers.ts
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/main.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-20 05:09:05.000000 django-gesha-0.1a3/js_tests/urls.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-20 05:09:05.000000 django-gesha-0.1a3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-20 05:09:05.000000 django-gesha-0.1a3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-20 05:09:05.000000 django-gesha-0.1a3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-20 05:09:05.000000 django-gesha-0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 05:09:16.975458 django-gesha-0.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/management/commands/printtestpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/test_project/fake/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/fake/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-20 05:09:05.000000 django-gesha-0.1a3/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:16.975458 django-gesha-0.1a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_jscontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 05:09:05.000000 django-gesha-0.1a3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.839611 django-gesha-0.1a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 22:42:47.000000 django-gesha-0.1a4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 22:42:47.000000 django-gesha-0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-22 22:42:57.847611 django-gesha-0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-22 22:42:47.000000 django-gesha-0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.839611 django-gesha-0.1a4/django_gesha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/assets/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/settings.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/stylesheets/extra.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/gesha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/gesha/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/static/gesha/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/templatetags/gesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/context.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/converters.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/urls.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/converters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/urls.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/context.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/converters.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/main.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/urls.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 22:42:47.000000 django-gesha-0.1a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   349273 2023-06-22 22:42:47.000000 django-gesha-0.1a4/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-22 22:42:47.000000 django-gesha-0.1a4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-22 22:42:47.000000 django-gesha-0.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:42:57.847611 django-gesha-0.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/fake/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/test_project/fake/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/commands/printtestpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/test_project/fake/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_package_versions_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_project_views_generate_correct_HTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tsconfig.json
```

### Comparing `django-gesha-0.1a3/.github/workflows/python-publish.yml` & `django-gesha-0.1a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/.gitignore` & `django-gesha-0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/LICENSE` & `django-gesha-0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/PKG-INFO` & `django-gesha-0.1a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a3
+Version: 0.1a4
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
 Project-URL: Source, https://github.com/ely-as/django-gesha
 Keywords: django,javascript,typescript
@@ -60,14 +60,25 @@
   - [Reverse URLs](https://django-gesha.readthedocs.io/en/latest/user_guide/#reverse-urls)
     natively in JavaScript (equivalent to `reverse()` in Python and `{% url %}` in
     templates).
   - Written in TypeScript and fully-typed Python.
 
 ---
 
+## Getting started
+
+To install and set up **django-gesha** in an existing Django project, see:
+
+  - [Installation](https://django-gesha.readthedocs.io/en/latest/installation/)
+  - [User Guide](https://django-gesha.readthedocs.io/en/latest/user_guide/)
+
+Starting a new Django project? Consider using
+[**django-gesha-template**](https://github.com/ely-as/django-gesha-template), which is
+pre-configured with **django-gesha** and a pipeline for TypeScript integration.
+
 ## Contributing
 
 See [Contributing](https://django-gesha.readthedocs.io/en/latest/contributing/).
 
 ## License
 
 [MIT](https://github.com/ely-as/django-gesha/blob/main/LICENSE).
```

### Comparing `django-gesha-0.1a3/README.md` & `django-gesha-0.1a4/docs/index.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
-
-[**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
-**&nbsp;•&nbsp;**
-[**Issue Tracker**](https://github.com/ely-as/django-gesha/issues)
-**&nbsp;•&nbsp;**
-[**Source**](https://github.com/ely-as/django-gesha)
-
 ---
 
 JavaScript utilities for [Django](https://www.djangoproject.com/) projects.
 
 ---
 
 **Features:**
 
-  - [Add context](https://django-gesha.readthedocs.io/en/latest/user_guide/#add-context)
-    in Django views to be used in JavaScript functions.
-  - [Reverse URLs](https://django-gesha.readthedocs.io/en/latest/user_guide/#reverse-urls)
-    natively in JavaScript (equivalent to `reverse()` in Python and `{% url %}` in
-    templates).
+  - [Add context](user_guide/#add-context) in Django views to be used in JavaScript
+    functions.
+  - [Reverse URLs](user_guide/#reverse-urls) natively in JavaScript (equivalent to
+    `#!py reverse()` in Python and
+    <span style="white-space:nowrap;">`#!django {% url %}`</span> in templates).
   - Written in TypeScript and fully-typed Python.
 
 ---
 
-## Contributing
-
-See [Contributing](https://django-gesha.readthedocs.io/en/latest/contributing/).
-
-## License
-
-[MIT](https://github.com/ely-as/django-gesha/blob/main/LICENSE).
+[**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
+**&nbsp;•&nbsp;**
+[**Issue Tracker**](https://github.com/ely-as/django-gesha/issues)
+**&nbsp;•&nbsp;**
+[**Source**](https://github.com/ely-as/django-gesha)
```

### Comparing `django-gesha-0.1a3/django_gesha.egg-info/PKG-INFO` & `django-gesha-0.1a4/django_gesha.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a3
+Version: 0.1a4
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
 Project-URL: Source, https://github.com/ely-as/django-gesha
 Keywords: django,javascript,typescript
@@ -60,14 +60,25 @@
   - [Reverse URLs](https://django-gesha.readthedocs.io/en/latest/user_guide/#reverse-urls)
     natively in JavaScript (equivalent to `reverse()` in Python and `{% url %}` in
     templates).
   - Written in TypeScript and fully-typed Python.
 
 ---
 
+## Getting started
+
+To install and set up **django-gesha** in an existing Django project, see:
+
+  - [Installation](https://django-gesha.readthedocs.io/en/latest/installation/)
+  - [User Guide](https://django-gesha.readthedocs.io/en/latest/user_guide/)
+
+Starting a new Django project? Consider using
+[**django-gesha-template**](https://github.com/ely-as/django-gesha-template), which is
+pre-configured with **django-gesha** and a pipeline for TypeScript integration.
+
 ## Contributing
 
 See [Contributing](https://django-gesha.readthedocs.io/en/latest/contributing/).
 
 ## License
 
 [MIT](https://github.com/ely-as/django-gesha/blob/main/LICENSE).
```

### Comparing `django-gesha-0.1a3/django_gesha.egg-info/SOURCES.txt` & `django-gesha-0.1a4/django_gesha.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,24 +24,29 @@
 docs/index.md
 docs/installation.md
 docs/settings.md
 docs/user_guide.md
 docs/assets/favicon.svg
 docs/assets/logo.svg
 docs/stylesheets/extra.css
+docs/stylesheets/extra.min.css
 gesha/__init__.py
 gesha/conf.py
 gesha/mixins.py
 gesha/types.py
 gesha/urls.py
 gesha/views.py
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
 gesha/templatetags/__init__.py
 gesha/templatetags/gesha.py
+js_dist/context.d.ts
+js_dist/converters.d.ts
+js_dist/main.d.ts
+js_dist/urls.d.ts
 js_src/context.ts
 js_src/converters.ts
 js_src/main.ts
 js_src/urls.ts
 js_tests/context.spec.ts
 js_tests/converters.spec.ts
 js_tests/helpers.ts
@@ -57,12 +62,14 @@
 test_project/fake/views.py
 test_project/fake/wsgi.py
 test_project/fake/management/__init__.py
 test_project/fake/management/commands/__init__.py
 test_project/fake/management/commands/printtestpage.py
 test_project/fake/templates/test.html
 tests/__init__.py
+tests/conftest.py
 tests/test_conf.py
 tests/test_init.py
-tests/test_jscontext.py
 tests/test_package_json.py
+tests/test_package_versions_align.py
+tests/test_project_views_generate_correct_HTML.py
 tests/test_urls.py
```

### Comparing `django-gesha-0.1a3/docs/assets/favicon.svg` & `django-gesha-0.1a4/docs/assets/favicon.svg`

 * *Files 17% similar despite different names*

```diff
@@ -21,49 +21,57 @@
 00000140: 6e73 3a73 6572 6966 3d22 6874 7470 3a2f  ns:serif="http:/
 00000150: 2f77 7777 2e73 6572 6966 2e63 6f6d 2f22  /www.serif.com/"
 00000160: 2073 7479 6c65 3d22 6669 6c6c 2d72 756c   style="fill-rul
 00000170: 653a 6576 656e 6f64 643b 636c 6970 2d72  e:evenodd;clip-r
 00000180: 756c 653a 6576 656e 6f64 643b 7374 726f  ule:evenodd;stro
 00000190: 6b65 2d6c 696e 6563 6170 3a73 7175 6172  ke-linecap:squar
 000001a0: 653b 7374 726f 6b65 2d6d 6974 6572 6c69  e;stroke-miterli
-000001b0: 6d69 743a 312e 353b 223e 3c63 6972 636c  mit:1.5;"><circl
-000001c0: 6520 6378 3d22 3134 2e34 2220 6379 3d22  e cx="14.4" cy="
-000001d0: 3134 2e34 2220 723d 2231 342e 3136 2220  14.4" r="14.16" 
-000001e0: 7374 796c 653d 2266 696c 6c3a 2336 6634  style="fill:#6f4
-000001f0: 6533 373b 222f 3e3c 7061 7468 2064 3d22  e37;"/><path d="
-00000200: 4d37 2e33 3134 2c31 302e 3332 3263 2d30  M7.314,10.322c-0
-00000210: 2c2d 3020 2d31 2e37 3236 2c37 2e31 3737  ,-0 -1.726,7.177
-00000220: 202d 312e 3632 312c 392e 3032 3563 302e   -1.621,9.025c0.
-00000230: 3136 382c 322e 3934 2034 2e37 3937 2c32  168,2.94 4.797,2
-00000240: 2e39 3720 342e 3739 372c 322e 3937 6c37  .97 4.797,2.97l7
-00000250: 2e37 312c 2d30 2e30 3038 632d 302c 3020  .71,-0.008c-0,0 
-00000260: 322e 3636 332c 302e 3033 3720 332e 3831  2.663,0.037 3.81
-00000270: 332c 2d31 2e36 3632 6330 2e36 3635 2c2d  3,-1.662c0.665,-
-00000280: 302e 3938 3120 302e 3334 372c 2d33 2e31  0.981 0.347,-3.1
-00000290: 3120 302e 3334 372c 2d33 2e31 3163 2d30  1 0.347,-3.11c-0
-000002a0: 2c2d 3020 312e 3734 362c 2d30 2e30 3536  ,-0 1.746,-0.056
-000002b0: 2032 2e33 3037 2c2d 302e 3738 6331 2e31   2.307,-0.78c1.1
-000002c0: 3739 2c2d 312e 3532 2030 2e34 3332 2c2d  79,-1.52 0.432,-
-000002d0: 342e 3737 3120 2d31 2e34 3737 2c2d 342e  4.771 -1.477,-4.
-000002e0: 3739 3763 2d31 2e31 3631 2c2d 302e 3031  797c-1.161,-0.01
-000002f0: 3620 2d31 2e38 372c 2d30 2e30 3220 2d31  6 -1.87,-0.02 -1
-00000300: 2e38 372c 2d30 2e30 326c 2d30 2e38 3332  .87,-0.02l-0.832
-00000310: 2c2d 342e 3334 6c2d 3132 2e37 3037 2c30  ,-4.34l-12.707,0
-00000320: 2e30 316c 2d31 2e36 3338 2c30 2e37 3933  .01l-1.638,0.793
-00000330: 6c31 2e31 3731 2c31 2e39 3139 5a22 2073  l1.171,1.919Z" s
-00000340: 7479 6c65 3d22 6669 6c6c 3a6e 6f6e 653b  tyle="fill:none;
-00000350: 7374 726f 6b65 3a23 6666 663b 7374 726f  stroke:#fff;stro
-00000360: 6b65 2d77 6964 7468 3a32 7078 3b22 2f3e  ke-width:2px;"/>
-00000370: 3c70 6174 6820 643d 224d 372e 3739 392c  <path d="M7.799,
-00000380: 3139 2e34 3535 632d 302e 3439 322c 2d30  19.455c-0.492,-0
-00000390: 2e36 3034 2030 2e38 3633 2c2d 352e 3831  .604 0.863,-5.81
-000003a0: 3520 302e 3836 332c 2d35 2e38 3135 6c31  5 0.863,-5.815l1
-000003b0: 312e 3034 312c 302e 3035 6330 2c2d 3020  1.041,0.05c0,-0 
-000003c0: 302e 3633 342c 322e 3437 3620 302e 3834  0.634,2.476 0.84
-000003d0: 2c34 2e39 6330 2e31 3639 2c31 2e39 3935  ,4.9c0.169,1.995
-000003e0: 202d 322e 3637 362c 312e 3831 3220 2d32   -2.676,1.812 -2
-000003f0: 2e36 3736 2c31 2e38 3132 6c2d 362e 3636  .676,1.812l-6.66
-00000400: 2c2d 302e 3030 3163 2d30 2c30 202d 322e  ,-0.001c-0,0 -2.
-00000410: 3536 332c 302e 3039 3320 2d33 2e34 3038  563,0.093 -3.408
-00000420: 2c2d 302e 3934 365a 2220 7374 796c 653d  ,-0.946Z" style=
-00000430: 2266 696c 6c3a 2366 6666 3b22 2f3e 3c2f  "fill:#fff;"/></
-00000440: 7376 673e                                svg>
+000001b0: 6d69 743a 312e 353b 223e 3c70 6174 6820  mit:1.5;"><path 
+000001c0: 643d 224d 3238 2e38 2c37 2e32 632d 302c  d="M28.8,7.2c-0,
+000001d0: 2d33 2e39 3734 202d 332e 3232 362c 2d37  -3.974 -3.226,-7
+000001e0: 2e32 202d 372e 322c 2d37 2e32 6c2d 3134  .2 -7.2,-7.2l-14
+000001f0: 2e34 2c30 632d 332e 3937 342c 3020 2d37  .4,0c-3.974,0 -7
+00000200: 2e32 2c33 2e32 3236 202d 372e 322c 372e  .2,3.226 -7.2,7.
+00000210: 326c 2d30 2c31 342e 3463 2d30 2c33 2e39  2l-0,14.4c-0,3.9
+00000220: 3734 2033 2e32 3236 2c37 2e32 2037 2e32  74 3.226,7.2 7.2
+00000230: 2c37 2e32 6c31 342e 342c 2d30 6333 2e39  ,7.2l14.4,-0c3.9
+00000240: 3734 2c2d 3020 372e 322c 2d33 2e32 3236  74,-0 7.2,-3.226
+00000250: 2037 2e32 2c2d 372e 326c 2d30 2c2d 3134   7.2,-7.2l-0,-14
+00000260: 2e34 5a22 2073 7479 6c65 3d22 6669 6c6c  .4Z" style="fill
+00000270: 3a23 3666 3465 3337 3b22 2f3e 3c70 6174  :#6f4e37;"/><pat
+00000280: 6820 643d 224d 372e 3331 342c 3130 2e33  h d="M7.314,10.3
+00000290: 3232 632d 302c 2d30 202d 312e 3732 362c  22c-0,-0 -1.726,
+000002a0: 372e 3137 3720 2d31 2e36 3231 2c39 2e30  7.177 -1.621,9.0
+000002b0: 3235 6330 2e31 3638 2c32 2e39 3420 342e  25c0.168,2.94 4.
+000002c0: 3739 372c 322e 3937 2034 2e37 3937 2c32  797,2.97 4.797,2
+000002d0: 2e39 376c 372e 3731 2c2d 302e 3030 3863  .97l7.71,-0.008c
+000002e0: 2d30 2c30 2032 2e36 3633 2c30 2e30 3337  -0,0 2.663,0.037
+000002f0: 2033 2e38 3133 2c2d 312e 3636 3263 302e   3.813,-1.662c0.
+00000300: 3636 352c 2d30 2e39 3831 2030 2e33 3437  665,-0.981 0.347
+00000310: 2c2d 332e 3131 2030 2e33 3437 2c2d 332e  ,-3.11 0.347,-3.
+00000320: 3131 632d 302c 2d30 2031 2e37 3436 2c2d  11c-0,-0 1.746,-
+00000330: 302e 3035 3620 322e 3330 372c 2d30 2e37  0.056 2.307,-0.7
+00000340: 3863 312e 3137 392c 2d31 2e35 3220 302e  8c1.179,-1.52 0.
+00000350: 3433 322c 2d34 2e37 3731 202d 312e 3437  432,-4.771 -1.47
+00000360: 372c 2d34 2e37 3937 632d 312e 3136 312c  7,-4.797c-1.161,
+00000370: 2d30 2e30 3136 202d 312e 3837 2c2d 302e  -0.016 -1.87,-0.
+00000380: 3032 202d 312e 3837 2c2d 302e 3032 6c2d  02 -1.87,-0.02l-
+00000390: 302e 3833 322c 2d34 2e33 346c 2d31 322e  0.832,-4.34l-12.
+000003a0: 3730 372c 302e 3031 6c2d 312e 3633 382c  707,0.01l-1.638,
+000003b0: 302e 3739 336c 312e 3137 312c 312e 3931  0.793l1.171,1.91
+000003c0: 395a 2220 7374 796c 653d 2266 696c 6c3a  9Z" style="fill:
+000003d0: 6e6f 6e65 3b73 7472 6f6b 653a 2366 6666  none;stroke:#fff
+000003e0: 3b73 7472 6f6b 652d 7769 6474 683a 3270  ;stroke-width:2p
+000003f0: 783b 222f 3e3c 7061 7468 2064 3d22 4d37  x;"/><path d="M7
+00000400: 2e37 3939 2c31 392e 3435 3563 2d30 2e34  .799,19.455c-0.4
+00000410: 3932 2c2d 302e 3630 3420 302e 3836 332c  92,-0.604 0.863,
+00000420: 2d35 2e38 3135 2030 2e38 3633 2c2d 352e  -5.815 0.863,-5.
+00000430: 3831 356c 3131 2e30 3431 2c30 2e30 3563  815l11.041,0.05c
+00000440: 302c 2d30 2030 2e36 3334 2c32 2e34 3736  0,-0 0.634,2.476
+00000450: 2030 2e38 342c 342e 3963 302e 3136 392c   0.84,4.9c0.169,
+00000460: 312e 3939 3520 2d32 2e36 3736 2c31 2e38  1.995 -2.676,1.8
+00000470: 3132 202d 322e 3637 362c 312e 3831 326c  12 -2.676,1.812l
+00000480: 2d36 2e36 362c 2d30 2e30 3031 632d 302c  -6.66,-0.001c-0,
+00000490: 3020 2d32 2e35 3633 2c30 2e30 3933 202d  0 -2.563,0.093 -
+000004a0: 332e 3430 382c 2d30 2e39 3436 5a22 2073  3.408,-0.946Z" s
+000004b0: 7479 6c65 3d22 6669 6c6c 3a23 6666 663b  tyle="fill:#fff;
+000004c0: 222f 3e3c 2f73 7667 3e                   "/></svg>
```

### Comparing `django-gesha-0.1a3/docs/assets/logo.svg` & `django-gesha-0.1a4/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/docs/contributing.md` & `django-gesha-0.1a4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/docs/index.md` & `django-gesha-0.1a4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
+
+[**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
+**&nbsp;•&nbsp;**
+[**Issue Tracker**](https://github.com/ely-as/django-gesha/issues)
+**&nbsp;•&nbsp;**
+[**Source**](https://github.com/ely-as/django-gesha)
+
 ---
 
 JavaScript utilities for [Django](https://www.djangoproject.com/) projects.
 
 ---
 
 **Features:**
 
-  - [Add context](user_guide/#add-context) in Django views to be used in JavaScript
-    functions.
-  - [Reverse URLs](user_guide/#reverse-urls) natively in JavaScript (equivalent to
-    `#!py reverse()` in Python and
-    <span style="white-space:nowrap;">`#!django {% url %}`</span> in templates).
+  - [Add context](https://django-gesha.readthedocs.io/en/latest/user_guide/#add-context)
+    in Django views to be used in JavaScript functions.
+  - [Reverse URLs](https://django-gesha.readthedocs.io/en/latest/user_guide/#reverse-urls)
+    natively in JavaScript (equivalent to `reverse()` in Python and `{% url %}` in
+    templates).
   - Written in TypeScript and fully-typed Python.
 
 ---
 
-[**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
-**&nbsp;•&nbsp;**
-[**Issue Tracker**](https://github.com/ely-as/django-gesha/issues)
-**&nbsp;•&nbsp;**
-[**Source**](https://github.com/ely-as/django-gesha)
+## Getting started
+
+To install and set up **django-gesha** in an existing Django project, see:
+
+  - [Installation](https://django-gesha.readthedocs.io/en/latest/installation/)
+  - [User Guide](https://django-gesha.readthedocs.io/en/latest/user_guide/)
+
+Starting a new Django project? Consider using
+[**django-gesha-template**](https://github.com/ely-as/django-gesha-template), which is
+pre-configured with **django-gesha** and a pipeline for TypeScript integration.
+
+## Contributing
+
+See [Contributing](https://django-gesha.readthedocs.io/en/latest/contributing/).
+
+## License
+
+[MIT](https://github.com/ely-as/django-gesha/blob/main/LICENSE).
```

### Comparing `django-gesha-0.1a3/docs/settings.md` & `django-gesha-0.1a4/docs/settings.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## **django-gesha** Settings
 
 ---
 
-### <pre>**GESHA_ALLOWED_URL_PATTERNS**</pre>
+### <pre>**GESHA_ALLOWED_URL_NAMES**</pre>
 
 Default: `[]`
 
-A list of allowed patterns for use in [reversing URLs](../user_guide/#reverse-urls).
+A list of allowed URL names for use in [reversing URLs](../user_guide/#reverse-urls).
 Supports [Unix shell-style wildcards](https://docs.python.org/3/library/fnmatch.html)
 <span style="white-space:nowrap;">(`*`, `?`, `[seq]` and `[!seq]`)</span>. Example to
 match `login`, `logout` and all paths in the `myapp` namespace:
 
 ``` py
-GESHA_ALLOWED_URL_PATTERNS = ["log*", "myapp:*"]
+GESHA_ALLOWED_URL_NAMES = ["log*", "myapp:*"]
 ```
 
 The default setting (an empty list) disables all patterns.
 
 ---
```

### Comparing `django-gesha-0.1a3/docs/user_guide.md` & `django-gesha-0.1a4/docs/user_guide.md`

 * *Files 11% similar despite different names*

```diff
@@ -108,18 +108,18 @@
 
 ### Test JavaScript API
 
 You can test that the JavaScript API is available by opening the console on your
 browser:
 
 ``` js
->> console.log(django.context.myNumber)
+>> console.log(window.django.context.myNumber)
    5
 
->> console.log(django.context.myString)
+>> console.log(window.django.context.myString)
    "this is my string"
 ```
 
 ## Using the JavaScript API
 
 ### Add context
 
@@ -155,26 +155,26 @@
         return render(request, "myapp/home.html", context=context)
     ```
 
 ### Reverse URLs
 
 Reverse URLs in JavaScript using the following function:
 
-`#!ts django.urls.reverse(name: string, kwargs?: ReverseKwargs): string`
+`#!ts window.django.urls.reverse(name: string, kwargs?: ReverseKwargs): string`
 
   - `#!ts name: string` – The namespaced URL name.
   - `#!ts kwargs?: { [argName: string]: number | string }` – URL arguments.
 
 !!! example "Examples of URL reversing"
 
     ``` js
-    >> django.urls.reverse("myapp:home")
+    >> window.django.urls.reverse("myapp:home")
     "/"
 
-    >> django.reverse("myapp:page", { page: 5 })
+    >> window.django.reverse("myapp:page", { page: 5 })
     "/page/5/"
     ```
 
     ??? info "Equivalent code in Django"
 
         ``` py title="In Python"
         from django.urls import reverse
@@ -185,46 +185,46 @@
         ``` django title="In templates"
         {% url 'myapp:page' page=5 %}
         ```
 
 !!! tip
 
     To set the URLs available for reversing configure the
-    [`GESHA_ALLOWED_URL_PATTERNS`](../settings/#gesha_allowed_url_patterns) setting.
+    [`GESHA_ALLOWED_URL_NAMES`](../settings/#GESHA_ALLOWED_URL_NAMES) setting.
 
     These patterns can also be set in class-based views by overriding the
     `#!py get_allowed_url_patterns()` method, for example:
 
     ``` py
     class HomeView(gesha.JSContextMixin, TemplateView):
         ...
 
         def get_allowed_url_patterns(self):
             return ["myapp:home", "otherapp:*"]
     ```
 
 !!! tip
 
-    `#!js django.urls.reverse()` is aliased to `#!js django.reverse()`
+    `#!js window.django.urls.reverse()` is aliased to `#!js window.django.reverse()`
 
 #### Custom converters
 
 If you have
 [registered custom path converters](https://docs.djangoproject.com/en/stable/topics/http/urls/#registering-custom-path-converters)
 in your Django project, you can also register them using the JavaScript API, for
 example:
 
 !!! example "Example path converter registration"
 
     === "JavaScript"
 
         ``` js linenums="1"
-        const fourDigitYearConverter = new django.urls.Converter("yyyy", /[0-9]{4}/);
+        const fourDigitYearConverter = new window.django.urls.Converter("yyyy", /[0-9]{4}/);
 
-        django.urls.converters.register(fourDigitYearConverter);
+        window.django.urls.converters.register(fourDigitYearConverter);
         ```
 
     === "Python"
 
         ``` py linenums="1"
         class FourDigitYearConverter:
             regex = "[0-9]{4}"
@@ -234,25 +234,26 @@
 
             def to_url(self, value):
                 return "%04d" % value
         ```
 
 #### Handling errors
 
-`#!js django.reverse()` will throw a `#!js django.urls.NoReverseMatch` error if:
+`#!js window.django.reverse()` will throw a `#!js window.django.urls.NoReverseMatch`
+error if:
 
   - The name provided does not match any known URLs.
   - The URL requires args, but none were provided.
   - The URL received args, but their values failed validation.
 
 ??? example "Example JavaScript code which handles `#!js NoReverseMatch`"
 
     ``` js hl_lines="5" linenums="1"
     try {
-      django.urls.reverse("missing:path")
+      window.django.urls.reverse("missing:path")
     }
     catch(err) {
       if (err.name === "NoReverseMatch") {
         console.log("handle NoReverseMatch");
       } else {
         console.log("handle different error")
       }
```

### Comparing `django-gesha-0.1a3/gesha/mixins.py` & `django-gesha-0.1a4/gesha/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                 "paths": get_paths_dict(
                     self.get_urlconf(), self.get_allowed_url_patterns()
                 ),
             }
         }
 
     def get_allowed_url_patterns(self) -> Iterable[str]:
-        return get_setting("GESHA_ALLOWED_URL_PATTERNS")
+        return get_setting("GESHA_ALLOWED_URL_NAMES")
 
     def get_urlconf(self) -> types.URLConf | None:
         return None
 
     def get_context_data(self, **kwargs) -> dict:
         context = super().get_context_data(**kwargs)  # type: ignore[misc]
         js_context_key = get_setting("GESHA_JSCONTEXT_KEY")
```

### Comparing `django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js` & `django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map` & `django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/gesha/templatetags/gesha.py` & `django-gesha-0.1a4/gesha/templatetags/gesha.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/gesha/types.py` & `django-gesha-0.1a4/gesha/types.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/gesha/urls.py` & `django-gesha-0.1a4/gesha/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/gulpfile.js` & `django-gesha-0.1a4/gulpfile.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,56 +1,101 @@
-const {
-    dest,
-    series
-} = require("gulp");
+const gulp = require("gulp");
 const browserify = require("browserify");
 const buffer = require("vinyl-buffer");
+const cleanCSS = require('gulp-clean-css');
 const fancy_log = require("fancy-log");
+const rename = require("gulp-rename");
 const source = require("vinyl-source-stream");
 const sourcemaps = require("gulp-sourcemaps");
 const terser = require("gulp-terser");
+const ts = require('gulp-typescript');
 const tsify = require("tsify");
 const watchify = require("watchify");
 
 require('dotenv').config();
 
 const debug = (String(process.env.DEBUG).toLowerCase() === "true");
 const paths = {
-    entries: ["js_src/main.ts"],
-    dest: "gesha/static/gesha/dist/js",
-    outfile: "django-gesha.bundle.min.js"
+    bundle: {
+        entries: ["js_src/main.ts"],
+        dest: "gesha/static/gesha/dist/js",
+        outfile: "django-gesha.bundle.min.js"
+    },
+    types: {
+        dest: "js_dist"
+    },
+    docs_styles: {
+        src: ["docs/stylesheets/extra.css"],
+        dest: "docs/stylesheets/"
+    }
 };
+const tsProject = ts.createProject("tsconfig.json");
 
 var browserifyObj = browserify({
     basedir: ".",
     debug: debug,
-    entries: paths.entries,
+    entries: paths.bundle.entries,
     cache: {},
     packageCache: {},
 }).plugin(tsify)
 
-function bundle(cb) {
+function bundle() {
     return browserifyObj
         .bundle()
         .on("error", fancy_log)
-        .pipe(source(paths.outfile))
+        .pipe(source(paths.bundle.outfile))
         .pipe(buffer())
         .pipe(sourcemaps.init({
             loadMaps: true
         }))
         .pipe(terser({
             mangle: true
         }))
         .pipe(sourcemaps.write("./"))
-        .pipe(dest(paths.dest));
+        .pipe(gulp.dest(paths.bundle.dest));
 }
 
-function watch(cb) {
+async function clean() {
+    const {
+        deleteAsync
+    } = await import("del");
+    await deleteAsync(paths.types.dest);
+}
+
+function types() {
+    return tsProject.src()
+        .pipe(sourcemaps.init())
+        .pipe(ts({
+            declaration: true,
+            emitDeclarationOnly: true
+        }))
+        .pipe(sourcemaps.write())
+        .pipe(gulp.dest(paths.types.dest));
+}
+
+function docs_styles() {
+    return gulp.src(paths.docs_styles.src, {
+            sourcemaps: true
+        })
+        .pipe(cleanCSS())
+        .pipe(rename({
+            suffix: ".min"
+        }))
+        .pipe(gulp.dest(paths.docs_styles.dest));
+}
+
+const build = gulp.parallel(bundle, gulp.series(clean, types));
+
+function watch() {
     var watchedBrowserify = watchify(browserifyObj);
-    bundle();
-    watchedBrowserify.on("update", bundle);
+    build();
+    watchedBrowserify.on("update", build);
     watchedBrowserify.on("log", fancy_log);
+    gulp.watch(paths.docs_styles.src, docs_styles);
 }
 
-exports.build = bundle;
-exports.default = exports.build;
+exports.build = build;
+exports.clean = clean;
+exports.default = gulp.parallel(build, docs_styles);
+exports.docs_styles = docs_styles;
+exports.types = types;
 exports.watch = watch;
```

### Comparing `django-gesha-0.1a3/js_src/context.ts` & `django-gesha-0.1a4/js_src/context.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_src/converters.ts` & `django-gesha-0.1a4/js_src/converters.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_src/main.ts` & `django-gesha-0.1a4/js_src/main.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_src/urls.ts` & `django-gesha-0.1a4/js_src/urls.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_tests/converters.spec.ts` & `django-gesha-0.1a4/js_tests/converters.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_tests/helpers.ts` & `django-gesha-0.1a4/js_tests/helpers.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_tests/test.html` & `django-gesha-0.1a4/js_tests/test.html`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/js_tests/urls.spec.ts` & `django-gesha-0.1a4/js_tests/urls.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/mkdocs.yml` & `django-gesha-0.1a4/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   name: material
   palette:
     scheme: slate
     primary: gesha
     accent: amber
   features:
     - content.code.annotate
+    - navigation.footer
   logo: assets/logo.svg
   favicon: assets/favicon.svg
 markdown_extensions:
   - admonition
   - footnotes
   - pymdownx.details
   - pymdownx.highlight:
@@ -31,8 +32,8 @@
   - Home: index.md
   - Installation: installation.md
   - User Guide: user_guide.md
   - Settings: settings.md
   - Contributing: contributing.md
   - Changelog: changelog.md
 extra_css:
-  - stylesheets/extra.css
+  - stylesheets/extra.min.css
```

### Comparing `django-gesha-0.1a3/package-lock.json` & `django-gesha-0.1a4/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8981710373575348%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.0-alpha4', 'devDependencies': {'del': '^7.0.0', "*

 * *               "'gulp-clean-css': '^4.3.0', 'gulp-rename': '^2.0.0'}}, "*

 * *               "'node_modules/aggregate-error': OrderedDict([('version', '4.0.1'), ('resolved', "*

 * *               "'https://registry.npmjs.org/aggregate-error/-/aggregate-error-4.0.1.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-0poP0T7el6Vq3rstR8Mn4V/IQrpBLO6POkUSrN7RhyY+GF/InCFShQzsQ39T25gkHhLgSLByyAz+Kjb+c2L98w=='), "*

 * *           […]*

```diff
@@ -5,33 +5,36 @@
         "": {
             "devDependencies": {
                 "@types/jsdom": "^21.1.1",
                 "@types/mocha": "^10.0.1",
                 "@typescript-eslint/eslint-plugin": "^5.59.0",
                 "@typescript-eslint/parser": "^5.59.0",
                 "browserify": "^17.0.0",
+                "del": "^7.0.0",
                 "dotenv": "^16.0.3",
                 "eslint": "^8.38.0",
                 "fancy-log": "^2.0.0",
                 "gulp": "^4.0.0",
+                "gulp-clean-css": "^4.3.0",
+                "gulp-rename": "^2.0.0",
                 "gulp-sourcemaps": "^3.0.0",
                 "gulp-terser": "^2.1.0",
                 "gulp-typescript": "^6.0.0-alpha.1",
                 "jsdom": "^21.1.1",
                 "mocha": "^10.2.0",
                 "ts-node": "^10.9.1",
                 "tsify": "^5.0.4",
                 "typescript": "^5.0.4",
                 "vinyl-buffer": "^1.0.1",
                 "vinyl-source-stream": "^2.0.0",
                 "watchify": "^4.0.0"
             },
             "license": "MIT",
             "name": "django-gesha",
-            "version": "0.1.0-alpha3"
+            "version": "0.1.0-alpha4"
         },
         "node_modules/@cspotcode/source-map-support": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "0.3.9"
             },
             "dev": true,
             "engines": {
@@ -893,14 +896,30 @@
         },
         "node_modules/agent-base/node_modules/ms": {
             "dev": true,
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
+        "node_modules/aggregate-error": {
+            "dependencies": {
+                "clean-stack": "^4.0.0",
+                "indent-string": "^5.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-0poP0T7el6Vq3rstR8Mn4V/IQrpBLO6POkUSrN7RhyY+GF/InCFShQzsQ39T25gkHhLgSLByyAz+Kjb+c2L98w==",
+            "resolved": "https://registry.npmjs.org/aggregate-error/-/aggregate-error-4.0.1.tgz",
+            "version": "4.0.1"
+        },
         "node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "fast-json-stable-stringify": "^2.0.0",
                 "json-schema-traverse": "^0.4.1",
                 "uri-js": "^4.2.2"
             },
@@ -1865,14 +1884,62 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-avDYr0SB3DwO9zsMov0gKCESFYqCnE4hq/4z3TdUlukEy5t9C0YRq7HLrsN52NAcqXKaepeCD0n+B0arnVG3Hg==",
             "resolved": "https://registry.npmjs.org/is-descriptor/-/is-descriptor-0.1.6.tgz",
             "version": "0.1.6"
         },
+        "node_modules/clean-css": {
+            "dependencies": {
+                "source-map": "~0.6.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 4.0"
+            },
+            "integrity": "sha512-VcMWDN54ZN/DS+g58HYL5/n4Zrqe8vHJpGA8KdgUXFU4fuP/aHNw8eld9SyEIyabIMJX/0RaY/fplOo5hYLSFA==",
+            "resolved": "https://registry.npmjs.org/clean-css/-/clean-css-4.2.3.tgz",
+            "version": "4.2.3"
+        },
+        "node_modules/clean-css/node_modules/source-map": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
+            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
+            "version": "0.6.1"
+        },
+        "node_modules/clean-stack": {
+            "dependencies": {
+                "escape-string-regexp": "5.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-LYv6XPxoyODi36Dp976riBtSY27VmFo+MKqEU9QCCWyTrdEPDog+RWA7xQWHi6Vbp61j5c4cdzzX1NidnwtUWg==",
+            "resolved": "https://registry.npmjs.org/clean-stack/-/clean-stack-4.2.0.tgz",
+            "version": "4.2.0"
+        },
+        "node_modules/clean-stack/node_modules/escape-string-regexp": {
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-/veY75JbMK4j1yjvuUxuVsiS/hr/4iHs9FTT6cgTexxdE0Ly/glccBAkloH/DofkjRbZU3bnoj38mOmhkZ0lHw==",
+            "resolved": "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-5.0.0.tgz",
+            "version": "5.0.0"
+        },
         "node_modules/cliui": {
             "dependencies": {
                 "string-width": "^1.0.1",
                 "strip-ansi": "^3.0.1",
                 "wrap-ansi": "^2.0.0"
             },
             "dev": true,
@@ -2345,14 +2412,79 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-hsBd2qSVCRE+5PmNdHt1uzyrFu5d3RwmFDKzyNZMFq/EwDNJF7Ee5+D5oEKF0hU6LhtoUF1macFvOe4AskQC1Q==",
             "resolved": "https://registry.npmjs.org/defined/-/defined-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "node_modules/del": {
+            "dependencies": {
+                "globby": "^13.1.2",
+                "graceful-fs": "^4.2.10",
+                "is-glob": "^4.0.3",
+                "is-path-cwd": "^3.0.0",
+                "is-path-inside": "^4.0.0",
+                "p-map": "^5.5.0",
+                "rimraf": "^3.0.2",
+                "slash": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=14.16"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-tQbV/4u5WVB8HMJr08pgw0b6nG4RGt/tj+7Numvq+zqcvUFeMaIWWOUFltiU+6go8BSO2/ogsB4EasDaj0y68Q==",
+            "resolved": "https://registry.npmjs.org/del/-/del-7.0.0.tgz",
+            "version": "7.0.0"
+        },
+        "node_modules/del/node_modules/globby": {
+            "dependencies": {
+                "dir-glob": "^3.0.1",
+                "fast-glob": "^3.2.11",
+                "ignore": "^5.2.0",
+                "merge2": "^1.4.1",
+                "slash": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-jWsQfayf13NvqKUIL3Ta+CIqMnvlaIDFveWE/dpOZ9+3AMEJozsxDvKA02zync9UuvOM8rOXzsD5GqKP4OnWPQ==",
+            "resolved": "https://registry.npmjs.org/globby/-/globby-13.2.0.tgz",
+            "version": "13.2.0"
+        },
+        "node_modules/del/node_modules/is-path-inside": {
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-lJJV/5dYS+RcL8uQdBDW9c9uWFLLBNRyFhnAKXw5tVqLlKZ4RMGZKv+YQ/IA3OhD+RpbJa1LLFM1FQPGyIXvOA==",
+            "resolved": "https://registry.npmjs.org/is-path-inside/-/is-path-inside-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/del/node_modules/slash": {
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-3dOsAHXXUkQTpOYcoAxLIorMTp4gIQr5IW3iVb7A7lFIp0VHhnynm9izx6TssdrIcVIESAlVjtnO2K8bg+Coew==",
+            "resolved": "https://registry.npmjs.org/slash/-/slash-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "node_modules/delayed-stream": {
             "dev": true,
             "engines": {
                 "node": ">=0.4.0"
             },
             "integrity": "sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==",
             "resolved": "https://registry.npmjs.org/delayed-stream/-/delayed-stream-1.0.0.tgz",
@@ -3861,14 +3993,35 @@
             "engines": {
                 "node": ">= 0.10"
             },
             "integrity": "sha512-dvEs27SCZt2ibF29xYgmnwwCYZxdxhQ/+LFWlbAW8y7jt68L/65402Lz3+CKy0Ov4rOs+NERmDq7YlZaDqUIfA==",
             "resolved": "https://registry.npmjs.org/gulp/-/gulp-4.0.2.tgz",
             "version": "4.0.2"
         },
+        "node_modules/gulp-clean-css": {
+            "dependencies": {
+                "clean-css": "4.2.3",
+                "plugin-error": "1.0.1",
+                "through2": "3.0.1",
+                "vinyl-sourcemaps-apply": "0.2.1"
+            },
+            "dev": true,
+            "integrity": "sha512-mGyeT3qqFXTy61j0zOIciS4MkYziF2U594t2Vs9rUnpkEHqfu6aDITMp8xOvZcvdX61Uz3y1mVERRYmjzQF5fg==",
+            "resolved": "https://registry.npmjs.org/gulp-clean-css/-/gulp-clean-css-4.3.0.tgz",
+            "version": "4.3.0"
+        },
+        "node_modules/gulp-clean-css/node_modules/through2": {
+            "dependencies": {
+                "readable-stream": "2 || 3"
+            },
+            "dev": true,
+            "integrity": "sha512-M96dvTalPT3YbYLaKaCuwu+j06D/8Jfib0o/PxbVt6Amhv3dUAtW6rTV1jPgJSBG83I/e04Y6xkVdVhSRhi0ww==",
+            "resolved": "https://registry.npmjs.org/through2/-/through2-3.0.1.tgz",
+            "version": "3.0.1"
+        },
         "node_modules/gulp-cli": {
             "bin": {
                 "gulp": "bin/gulp.js"
             },
             "dependencies": {
                 "ansi-colors": "^1.0.1",
                 "archy": "^1.0.0",
@@ -3908,14 +4061,23 @@
             "engines": {
                 "node": ">= 0.10"
             },
             "integrity": "sha512-k9oEhlyc0FrVh25qYuSELjr8oxsCoc4/LEZfg2iJJrfEk/tZL9bCoJE47gqAvI2m/AUjluCS4+3I0eTx8n3AEw==",
             "resolved": "https://registry.npmjs.org/fancy-log/-/fancy-log-1.3.3.tgz",
             "version": "1.3.3"
         },
+        "node_modules/gulp-rename": {
+            "dev": true,
+            "engines": {
+                "node": ">=4"
+            },
+            "integrity": "sha512-97Vba4KBzbYmR5VBs9mWmK+HwIf5mj+/zioxfZhOKeXtx5ZjBk57KFlePf5nxq9QsTtFl0ejnHE3zTC9MHXqyQ==",
+            "resolved": "https://registry.npmjs.org/gulp-rename/-/gulp-rename-2.0.0.tgz",
+            "version": "2.0.0"
+        },
         "node_modules/gulp-sourcemaps": {
             "dependencies": {
                 "@gulp-sourcemaps/identity-map": "^2.0.1",
                 "@gulp-sourcemaps/map-sources": "^1.0.0",
                 "acorn": "^6.4.1",
                 "convert-source-map": "^1.0.0",
                 "css": "^3.0.0",
@@ -4378,14 +4540,26 @@
             "engines": {
                 "node": ">=0.8.19"
             },
             "integrity": "sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==",
             "resolved": "https://registry.npmjs.org/imurmurhash/-/imurmurhash-0.1.4.tgz",
             "version": "0.1.4"
         },
+        "node_modules/indent-string": {
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-m6FAo/spmsW2Ab2fU35JTYwtOKa2yAwXSwgjSv1TJzh4Mh7mC3lzAOVLBprb72XsTrgkEIsl7YrFNAiDiRhIGg==",
+            "resolved": "https://registry.npmjs.org/indent-string/-/indent-string-5.0.0.tgz",
+            "version": "5.0.0"
+        },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
             "dev": true,
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
@@ -4680,14 +4854,26 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-NOW9QQXMoZGg/oqnVNoNTTIFEIid1627WCffUBJEdMxYApq7mNE7CpzucIPc+ZQg25Phej7IJSmX3hO+oblOtQ==",
             "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-3.2.2.tgz",
             "version": "3.2.2"
         },
+        "node_modules/is-path-cwd": {
+            "dev": true,
+            "engines": {
+                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-kyiNFFLU0Ampr6SDZitD/DwUo4Zs1nSdnygUBqsu3LooL00Qvb5j+UnvApUn/TTj1J3OuE6BTdQ5rudKmU2ZaA==",
+            "resolved": "https://registry.npmjs.org/is-path-cwd/-/is-path-cwd-3.0.0.tgz",
+            "version": "3.0.0"
+        },
         "node_modules/is-path-inside": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-Fd4gABb+ycGAmKou8eMftCupSir5lRxqf4aD/vd0cD2qc4HL07OjCeuHMr8Ro4CoMaeCKDB0/ECBOVWjTwUvPQ==",
             "resolved": "https://registry.npmjs.org/is-path-inside/-/is-path-inside-3.0.3.tgz",
@@ -6342,14 +6528,29 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-LaNjtRWUBY++zB5nE/NwcaoMylSPk+S+ZHNB1TzdbMJMny6dynpAGt7X/tl/QYq3TIeE6nxHppbo2LGymrG5Pw==",
             "resolved": "https://registry.npmjs.org/p-locate/-/p-locate-5.0.0.tgz",
             "version": "5.0.0"
         },
+        "node_modules/p-map": {
+            "dependencies": {
+                "aggregate-error": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=12"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-VFqfGDHlx87K66yZrNdI4YGtD70IRyd+zSvgks6mzHPRNkoKy+9EKP4SFC77/vTTQYmRmti7dvqC+m5jBrBAcg==",
+            "resolved": "https://registry.npmjs.org/p-map/-/p-map-5.5.0.tgz",
+            "version": "5.5.0"
+        },
         "node_modules/pako": {
             "dev": true,
             "integrity": "sha512-4hLB8Py4zZce5s4yd9XzopqwVv/yGNhV1Bl8NTmCq1763HeK2+EwVTv+leGeL13Dnh2wfbqowVPXCIO0z4taYw==",
             "resolved": "https://registry.npmjs.org/pako/-/pako-1.0.11.tgz",
             "version": "1.0.11"
         },
         "node_modules/parent-module": {
@@ -9298,9 +9499,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0-alpha3"
+    "version": "0.1.0-alpha4"
 }
```

### Comparing `django-gesha-0.1a3/package.json` & `django-gesha-0.1a4/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8219063545150502%*

 * *Differences: {"'devDependencies'": "{'del': '^7.0.0', 'gulp-clean-css': '^4.3.0', 'gulp-rename': '^2.0.0'}",*

 * * "'directories'": "{'test': './js_tests'}",*

 * * "'main'": "'./gesha/static/gesha/dist/js/django-gesha.bundle.min.js'",*

 * * "'types'": "'./js_dist/main.d.ts'",*

 * * "'version'": "'0.1.0-alpha4'"}*

```diff
@@ -6,40 +6,44 @@
     "description": "JavaScript utilities for Django projects.",
     "devDependencies": {
         "@types/jsdom": "^21.1.1",
         "@types/mocha": "^10.0.1",
         "@typescript-eslint/eslint-plugin": "^5.59.0",
         "@typescript-eslint/parser": "^5.59.0",
         "browserify": "^17.0.0",
+        "del": "^7.0.0",
         "dotenv": "^16.0.3",
         "eslint": "^8.38.0",
         "fancy-log": "^2.0.0",
         "gulp": "^4.0.0",
+        "gulp-clean-css": "^4.3.0",
+        "gulp-rename": "^2.0.0",
         "gulp-sourcemaps": "^3.0.0",
         "gulp-terser": "^2.1.0",
         "gulp-typescript": "^6.0.0-alpha.1",
         "jsdom": "^21.1.1",
         "mocha": "^10.2.0",
         "ts-node": "^10.9.1",
         "tsify": "^5.0.4",
         "typescript": "^5.0.4",
         "vinyl-buffer": "^1.0.1",
         "vinyl-source-stream": "^2.0.0",
         "watchify": "^4.0.0"
     },
     "directories": {
-        "test": "js_tests"
+        "test": "./js_tests"
     },
     "homepage": "https://github.com/ely-as/django-gesha",
     "license": "MIT",
-    "main": "gesha/static/gesha/dist/js/django-gesha.bundle.min.js",
+    "main": "./gesha/static/gesha/dist/js/django-gesha.bundle.min.js",
     "name": "django-gesha",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/ely-as/django-gesha.git"
     },
     "scripts": {
         "lint": "eslint ./js_*/**/*.ts",
         "test": "mocha"
     },
-    "version": "0.1.0-alpha3"
+    "types": "./js_dist/main.d.ts",
+    "version": "0.1.0-alpha4"
 }
```

### Comparing `django-gesha-0.1a3/pyproject.toml` & `django-gesha-0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/test_project/fake/management/commands/printtestpage.py` & `django-gesha-0.1a4/test_project/fake/management/commands/printtestpage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/test_project/fake/settings.py` & `django-gesha-0.1a4/test_project/fake/settings.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/test_project/fake/urls.py` & `django-gesha-0.1a4/test_project/fake/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/test_project/fake/views.py` & `django-gesha-0.1a4/test_project/fake/views.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/test_project/manage.py` & `django-gesha-0.1a4/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/tests/test_jscontext.py` & `django-gesha-0.1a4/tests/test_project_views_generate_correct_HTML.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,52 @@
+"""
+Functional tests which confirm that the {% jscontext %} template tag is generating the
+correct HTML in conjunction with correctly configured views, and can also be modified by
+settings overrides.
+"""
 from __future__ import annotations
 
 import json
 from collections.abc import Iterator
 
 import django
 import pytest
 from bs4 import BeautifulSoup
 from django.test import Client, override_settings
 
 
 def request_soup(method: str, path: str) -> BeautifulSoup:
+    """Perform an HTTP request against the Django test client and return a
+    `BeautifulSoup` object.
+
+    This is a function (rather than a @pytest.fixture) so the output can be modified
+    using django.test.override_settings as a context manager.
+    """
     response = Client().generic(method, path)
     return BeautifulSoup(response.content, "lxml")
 
 
-paths_to_test_for_presence_of_valid_script_html: list[str] = [
+# defined in test_project/fake/urls.py
+paths_to_test: list[str] = [
     "/",  # tests JSContextMixin
     "/func-based/",  # tests create_js_context_data()
 ]
 
 if django.VERSION[:2] >= (3, 1):
-    paths_to_test_for_presence_of_valid_script_html += [
-        "/async/",  # tests async
-    ]
+    paths_to_test.append("/async/")
 
 
-@pytest.fixture(params=paths_to_test_for_presence_of_valid_script_html)
+@pytest.fixture(params=paths_to_test)
 def path(request: pytest.FixtureRequest) -> Iterator[str]:
     yield request.param
 
 
+# Tests for {% jscontext %} generating correct <script> elements
+
+
 def test_jscontext_tag_generates_script_html(path: str) -> None:
     soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     assert json_script
     js_context = json.loads(json_script.text)
     assert "myString" in js_context
 
@@ -43,30 +56,35 @@
 ) -> None:
     with override_settings(GESHA_JSCONTEXT_KEY="different_key"):
         soup = request_soup("GET", path)
     json_script = soup.find("script", id="different_key")
     assert json_script
 
 
-def test_paths_are_empty_by_default(path: str) -> None:
+# Tests for the JSON within the <script> elements
+
+
+def test_JSON_paths_are_empty_by_default(path: str) -> None:
     soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     js_context = json.loads(json_script.text)  # type: ignore[union-attr]
     assert js_context["_gesha"]["paths"] == {}
 
 
-def test_paths_are_empty_when_GESHA_ALLOWED_URL_PATTERNS_is_empty_list(
+def test_JSON_paths_are_empty_when_GESHA_ALLOWED_URL_NAMES_is_empty_list(
     path: str,
 ) -> None:
-    with override_settings(GESHA_ALLOWED_URL_PATTERNS=[]):
+    with override_settings(GESHA_ALLOWED_URL_NAMES=[]):
         soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     js_context = json.loads(json_script.text)  # type: ignore[union-attr]
     assert js_context["_gesha"]["paths"] == {}
 
 
-def test_paths_are_filtered_when_GESHA_ALLOWED_URL_PATTERNS_is_set(path: str) -> None:
-    with override_settings(GESHA_ALLOWED_URL_PATTERNS=["fake:test"]):
+def test_JSON_paths_are_filtered_when_GESHA_ALLOWED_URL_NAMES_is_set(
+    path: str,
+) -> None:
+    with override_settings(GESHA_ALLOWED_URL_NAMES=["fake:test"]):
         soup = request_soup("GET", path)
     json_script = soup.find("script", id="js_context_data")
     js_context = json.loads(json_script.text)  # type: ignore[union-attr]
     assert len(js_context["_gesha"]["paths"]) == 1
```

### Comparing `django-gesha-0.1a3/tests/test_urls.py` & `django-gesha-0.1a4/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a3/tox.ini` & `django-gesha-0.1a4/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tox]
 min_version = 4.0
 isolated_build = True
 envlist =
-    lint-test-type
+    static-test
 labels =
-    py3.8 = test-py38-django{22,30,31,32,40,41,42}
-    py3.9 = test-py39-django{22,30,31,32,40,41,42}
-    py3.10 = test-py310-django{32,40,41,42}
-    py3.11 = test-py311-django{41,42}, lint-type
+    # Used by .github/workflows/test.yml - envs to run for each py version
+    3.8 = test-py38-django{22,30,31,32,40,41,42}
+    3.9 = test-py39-django{22,30,31,32,40,41,42}
+    3.10 = test-py310-django{32,40,41,42}
+    3.11 = static, test-py311-django{41,42}
 
 [testenv]
 extras = test
 deps =
     django22: Django>=2.2,<2.3
     django30: Django>=3.0,<3.1
     django31: Django>=3.1,<3.2
@@ -25,13 +26,13 @@
     py38-django22: Django>=2.2.8
     py39-django22: Django>=2.2.17
     py39-django30: Django>=3.0.11
     py39-django31: Django>=3.1.3
     py310-django32: Django>=3.2.9
     py311-django41: Django>=4.1.3
 commands =
-    format: black {toxinidir} {posargs}
-    format: ruff check --select I --fix {toxinidir} {posargs}
-    lint: black {toxinidir} --check --diff {posargs}
-    lint: ruff check {toxinidir} {posargs}
-    test: pytest --cov={toxinidir} --cov-report=term --cov-report=xml {posargs}
-    type: mypy {posargs}
+    format: black {tox_root}
+    format: ruff check --fix-only {tox_root}
+    static: black {tox_root} --check --diff
+    static: ruff check {tox_root}
+    static: mypy
+    test: pytest --cov={tox_root} --cov-report=term --cov-report=xml
```

