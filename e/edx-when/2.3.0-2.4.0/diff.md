# Comparing `tmp/edx-when-2.3.0.tar.gz` & `tmp/edx-when-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-when-2.3.0.tar", last modified: Tue Feb 15 11:06:03 2022, max compression
+gzip compressed data, was "edx-when-2.4.0.tar", last modified: Fri Jun 23 13:52:41 2023, max compression
```

## Comparing `edx-when-2.3.0.tar` & `edx-when-2.4.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.950218 edx-when-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-02-15 11:05:56.000000 edx-when-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-02-15 11:05:56.000000 edx-when-2.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-02-15 11:05:56.000000 edx-when-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-02-15 11:05:56.000000 edx-when-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-02-15 11:06:03.950218 edx-when-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-02-15 11:05:56.000000 edx-when-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.946218 edx-when-2.3.0/edx_when/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    19535 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/field_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.950218 edx-when-2.3.0/edx_when/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0002_auto_20190318_1736.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0003_auto_20190402_1501.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0004_datepolicy_rel_date.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0005_auto_20190911_1056.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0006_drop_active_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0007_meta_tweaks.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/0008_courseversion_block_type.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.946218 edx-when-2.3.0/edx_when/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.950218 edx-when-2.3.0/edx_when/templates/edx_schedule/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/templates/edx_schedule/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-02-15 11:05:56.000000 edx-when-2.3.0/edx_when/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.950218 edx-when-2.3.0/edx_when.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-15 11:06:03.000000 edx-when-2.3.0/edx_when.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 11:06:03.950218 edx-when-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-15 11:05:56.000000 edx-when-2.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-02-15 11:05:56.000000 edx-when-2.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-02-15 11:06:03.950218 edx-when-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-02-15 11:05:56.000000 edx-when-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.690486 edx-when-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-23 13:52:36.000000 edx-when-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-06-23 13:52:36.000000 edx-when-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-06-23 13:52:36.000000 edx-when-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-23 13:52:36.000000 edx-when-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-06-23 13:52:41.690486 edx-when-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-06-23 13:52:36.000000 edx-when-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19535 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4821 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/field_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0002_auto_20190318_1736.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0003_auto_20190402_1501.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0004_datepolicy_rel_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0005_auto_20190911_1056.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0006_drop_active_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0007_meta_tweaks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0008_courseversion_block_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.682486 edx-when-2.4.0/edx_when/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/templates/edx_schedule/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/templates/edx_schedule/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-23 13:52:36.000000 edx-when-2.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-23 13:52:36.000000 edx-when-2.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-23 13:52:41.690486 edx-when-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-06-23 13:52:36.000000 edx-when-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.690486 edx-when-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    28200 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_xblock_services.py
```

### Comparing `edx-when-2.3.0/CHANGELOG.rst` & `edx-when-2.4.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[2.4.0] - 2023-06-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2
+
 [2.3.0] - 2022-02-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Added Django40 support
 * Dropped Django22, 30 and 31 support
 
 
 [2.2.2] - 2021-10-21
```

### Comparing `edx-when-2.3.0/LICENSE.txt` & `edx-when-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/PKG-INFO` & `edx-when-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: edx-when
-Version: 2.3.0
+Version: 2.4.0
 Summary: Your project description goes here
-Home-page: https://github.com/edx/edx-when
+Home-page: https://github.com/openedx/edx-when
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 edx-when
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
@@ -29,15 +30,15 @@
 Overview
 --------
 
 edx-when is designed to be the central source of dates for the LMS.
 This repository is deployed to PyPI and designed to be installed and imported by an installation of edx-platform.
 As part of being integrated into edx-platform, edx-when shares the **same** database as the rest of the platform.
 It is written to by Studio when a Course is published
-(via https://github.com/edx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
+(via https://github.com/openedx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
 and then the LMS reads from it in several locations.
 This repo contains start, end, and due dates for Courses and offers the
 functionality to have both absolute and relative dates.
 
 License
 -------
 
@@ -47,24 +48,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -76,16 +75,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/edx-when/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-when/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/edx-when/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-when/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-when/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-when?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-when/badge/?version=latest
@@ -93,15 +92,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-when.svg
-    :target: https://github.com/edx/edx-when/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-when/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -113,14 +112,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[2.4.0] - 2023-06-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2
+
 [2.3.0] - 2022-02-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Added Django40 support
 * Dropped Django22, 30 and 31 support
 
 
 [2.2.2] - 2021-10-21
@@ -202,9 +208,7 @@
 [0.1.0] - 2019-03-04
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `edx-when-2.3.0/README.rst` & `edx-when-2.4.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Overview
 --------
 
 edx-when is designed to be the central source of dates for the LMS.
 This repository is deployed to PyPI and designed to be installed and imported by an installation of edx-platform.
 As part of being integrated into edx-platform, edx-when shares the **same** database as the rest of the platform.
 It is written to by Studio when a Course is published
-(via https://github.com/edx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
+(via https://github.com/openedx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
 and then the LMS reads from it in several locations.
 This repo contains start, end, and due dates for Courses and offers the
 functionality to have both absolute and relative dates.
 
 License
 -------
 
@@ -25,24 +25,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -54,16 +52,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/edx-when/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-when/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/edx-when/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-when/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-when/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-when?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-when/badge/?version=latest
@@ -71,9 +69,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-when.svg
-    :target: https://github.com/edx/edx-when/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-when/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `edx-when-2.3.0/edx_when/admin.py` & `edx-when-2.4.0/edx_when/admin.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/api.py` & `edx-when-2.4.0/edx_when/api.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/field_data.py` & `edx-when-2.4.0/edx_when/field_data.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/migrations/0001_initial.py` & `edx-when-2.4.0/edx_when/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/migrations/0002_auto_20190318_1736.py` & `edx-when-2.4.0/edx_when/migrations/0002_auto_20190318_1736.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/migrations/0003_auto_20190402_1501.py` & `edx-when-2.4.0/edx_when/migrations/0003_auto_20190402_1501.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/migrations/0005_auto_20190911_1056.py` & `edx-when-2.4.0/edx_when/migrations/0005_auto_20190911_1056.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/migrations/0008_courseversion_block_type.py` & `edx-when-2.4.0/edx_when/migrations/0008_courseversion_block_type.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/models.py` & `edx-when-2.4.0/edx_when/models.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/templates/edx_schedule/base.html` & `edx-when-2.4.0/edx_when/templates/edx_schedule/base.html`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when/utils.py` & `edx-when-2.4.0/edx_when/utils.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/edx_when.egg-info/PKG-INFO` & `edx-when-2.4.0/edx_when.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: edx-when
-Version: 2.3.0
+Version: 2.4.0
 Summary: Your project description goes here
-Home-page: https://github.com/edx/edx-when
+Home-page: https://github.com/openedx/edx-when
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 edx-when
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
@@ -29,15 +30,15 @@
 Overview
 --------
 
 edx-when is designed to be the central source of dates for the LMS.
 This repository is deployed to PyPI and designed to be installed and imported by an installation of edx-platform.
 As part of being integrated into edx-platform, edx-when shares the **same** database as the rest of the platform.
 It is written to by Studio when a Course is published
-(via https://github.com/edx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
+(via https://github.com/openedx/edx-platform/blob/master/openedx/core/djangoapps/course_date_signals/handlers.py)
 and then the LMS reads from it in several locations.
 This repo contains start, end, and due dates for Courses and offers the
 functionality to have both absolute and relative dates.
 
 License
 -------
 
@@ -47,24 +48,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -76,16 +75,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/edx-when/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-when/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/edx-when/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-when/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-when/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-when?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-when/badge/?version=latest
@@ -93,15 +92,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-when.svg
     :target: https://pypi.python.org/pypi/edx-when/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-when.svg
-    :target: https://github.com/edx/edx-when/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-when/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -113,14 +112,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[2.4.0] - 2023-06-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2
+
 [2.3.0] - 2022-02-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Added Django40 support
 * Dropped Django22, 30 and 31 support
 
 
 [2.2.2] - 2021-10-21
@@ -202,9 +208,7 @@
 [0.1.0] - 2019-03-04
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `edx-when-2.3.0/edx_when.egg-info/SOURCES.txt` & `edx-when-2.4.0/edx_when.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -28,8 +28,11 @@
 edx_when/migrations/0005_auto_20190911_1056.py
 edx_when/migrations/0006_drop_active_index.py
 edx_when/migrations/0007_meta_tweaks.py
 edx_when/migrations/0008_courseversion_block_type.py
 edx_when/migrations/__init__.py
 edx_when/templates/edx_schedule/base.html
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_api.py
+tests/test_models.py
+tests/test_xblock_services.py
```

### Comparing `edx-when-2.3.0/requirements/constraints.txt` & `edx-when-2.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-when-2.3.0/setup.py` & `edx-when-2.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,30 +104,32 @@
     CHANGELOG = changelog_file.read()
 
 setup(
     name='edx-when',
     version=VERSION,
     description="""Your project description goes here""",
     long_description=README + '\n\n' + CHANGELOG,
+    long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/edx-when',
+    url='https://github.com/openedx/edx-when',
     packages=[
         'edx_when',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
```

