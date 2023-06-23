# Comparing `tmp/xcookie-0.1.0.tar.gz` & `tmp/xcookie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcookie-0.1.0.tar", last modified: Tue Jun 14 20:36:00 2022, max compression
+gzip compressed data, was "xcookie-0.2.0.tar", last modified: Fri Jun 23 20:55:57 2023, max compression
```

## Comparing `xcookie-0.1.0.tar` & `xcookie-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,49 @@
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2022-06-14 20:36:00.573524 xcookie-0.1.0/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2826 2022-06-14 20:36:00.573524 xcookie-0.1.0/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1964 2022-06-13 15:46:42.000000 xcookie-0.1.0/README.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      872 2022-06-13 15:46:42.000000 xcookie-0.1.0/pyproject.toml
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       38 2022-06-14 20:36:00.573524 xcookie-0.1.0/setup.cfg
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9344 2022-06-14 20:35:35.000000 xcookie-0.1.0/setup.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2022-06-14 20:36:00.573524 xcookie-0.1.0/xcookie/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      413 2022-06-14 20:00:21.000000 xcookie-0.1.0/xcookie/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2022-06-13 15:46:42.000000 xcookie-0.1.0/xcookie/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2022-06-13 15:46:42.000000 xcookie-0.1.0/xcookie/__main__.pyi
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    27149 2022-06-14 20:30:45.000000 xcookie-0.1.0/xcookie/main.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      981 2022-06-13 15:46:42.000000 xcookie-0.1.0/xcookie/main.pyi
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-13 15:46:42.000000 xcookie-0.1.0/xcookie/py.typed
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2022-06-14 20:36:00.573524 xcookie-0.1.0/xcookie.egg-info/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2826 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      333 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/SOURCES.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/dependency_links.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       51 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/entry_points.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2737 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/requires.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        8 2022-06-14 20:36:00.000000 xcookie-0.1.0/xcookie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:57.211356 xcookie-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-23 20:55:48.000000 xcookie-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-23 20:55:57.211356 xcookie-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-06-23 20:55:48.000000 xcookie-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-23 20:55:48.000000 xcookie-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 20:55:57.211356 xcookie-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9082 2023-06-23 20:55:48.000000 xcookie-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:57.207356 xcookie-0.2.0/xcookie/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:57.211356 xcookie-0.2.0/xcookie/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/common_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/docs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40615 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/readthedocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/builders/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/directive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50910 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:57.211356 xcookie-0.2.0/xcookie/rc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/conf_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/gitlab-ci.binpy.yml.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/gitlab-ci.purepy.yml.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/run_tests.binpy.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/run_tests.purepy.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/test_binaries.yml.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rc/tests.yml.in
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/rich_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/util_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-23 20:55:48.000000 xcookie-0.2.0/xcookie/vcs_remotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:55:57.207356 xcookie-0.2.0/xcookie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 20:55:57.000000 xcookie-0.2.0/xcookie.egg-info/top_level.txt
```

### Comparing `xcookie-0.1.0/xcookie/main.pyi` & `xcookie-0.2.0/xcookie/main.pyi`

 * *Files identical despite different names*

