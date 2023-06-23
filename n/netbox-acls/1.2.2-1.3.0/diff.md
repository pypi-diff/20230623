# Comparing `tmp/netbox-acls-1.2.2.tar.gz` & `tmp/netbox-acls-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-acls-1.2.2.tar", last modified: Wed Jan 25 20:25:41 2023, max compression
+gzip compressed data, was "netbox-acls-1.3.0.tar", last modified: Fri Jun 23 19:04:11 2023, max compression
```

## Comparing `netbox-acls-1.2.2.tar` & `netbox-acls-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.136528 netbox-acls-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-01-25 20:25:41.136528 netbox-acls-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/forms/bulk_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/forms/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23478 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/migrations/0002_alter_accesslist_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/migrations/0003_netbox_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/models/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/models/access_list_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/models/access_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.128528 netbox-acls-1.2.2/netbox_acls/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls/templates/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/inc/view_tab.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.136528 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/accesslist.html
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/accesslist_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclextendedrule.html
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclinterfaceassignment.html
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclinterfaceassignment_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclstandardrule.html
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/netbox_acls/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:25:41.132528 netbox-acls-1.2.2/netbox_acls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-01-25 20:25:41.000000 netbox-acls-1.2.2/netbox_acls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-01-25 20:25:41.000000 netbox-acls-1.2.2/netbox_acls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:25:41.000000 netbox-acls-1.2.2/netbox_acls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:25:40.000000 netbox-acls-1.2.2/netbox_acls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-25 20:25:41.000000 netbox-acls-1.2.2/netbox_acls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:25:41.136528 netbox-acls-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-25 20:25:27.000000 netbox-acls-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.011162 netbox-acls-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-23 19:04:11.011162 netbox-acls-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/forms/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/forms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/graphql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/migrations/0002_alter_accesslist_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/migrations/0003_netbox_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/models/access_list_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/models/access_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.003162 netbox-acls-1.3.0/netbox_acls/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls/templates/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/inc/view_tab.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.011162 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/accesslist.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/accesslist_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclextendedrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclinterfaceassignment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclinterfaceassignment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclstandardrule.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.011162 netbox-acls-1.3.0/netbox_acls/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/netbox_acls/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:04:11.007162 netbox-acls-1.3.0/netbox_acls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-23 19:04:10.000000 netbox-acls-1.3.0/netbox_acls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-23 19:04:10.000000 netbox-acls-1.3.0/netbox_acls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:04:10.000000 netbox-acls-1.3.0/netbox_acls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:04:10.000000 netbox-acls-1.3.0/netbox_acls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 19:04:10.000000 netbox-acls-1.3.0/netbox_acls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:04:11.011162 netbox-acls-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-23 19:03:59.000000 netbox-acls-1.3.0/setup.py
```

### Comparing `netbox-acls-1.2.2/LICENSE.txt` & `netbox-acls-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/PKG-INFO` & `netbox-acls-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-acls
-Version: 1.2.2
-Summary: A NetBox plugin for Access List management
-Home-page: https://github.com/ryanmerolle/netbox-acls
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # NetBox Access Lists Plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin for Access List management.
 
 ## Features
 
 This plugin provides the following models:
@@ -47,14 +37,15 @@
 Each Plugin Version listed below has been tested with its corresponding NetBox Version.
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
 |      3.2       |     1.0.1      |
 |      3.3       |     1.1.0      |
 |      3.4       |     1.2.2      |
+|      3.5       |     1.3.0      |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 You can install with pip:
```

### Comparing `netbox-acls-1.2.2/netbox_acls/api/nested_serializers.py` & `netbox-acls-1.3.0/netbox_acls/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/api/serializers.py` & `netbox-acls-1.3.0/netbox_acls/api/serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Serializers control the translation of client data to and from Python objects,
 while Django itself handles the database abstraction.
 """
 
 from django.contrib.contenttypes.models import ContentType
-from django.core.exceptions import ObjectDoesNotExist
-from drf_yasg.utils import swagger_serializer_method
+from drf_spectacular.utils import extend_schema_field
 from ipam.api.serializers import NestedPrefixSerializer
 from netbox.api.fields import ContentTypeField
 from netbox.api.serializers import NetBoxModelSerializer
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from rest_framework import serializers
 from utilities.api import get_serializer_for_model
 
@@ -28,21 +27,17 @@
     "ACLStandardRuleSerializer",
     "ACLExtendedRuleSerializer",
 ]
 
 # Sets a standard error message for ACL rules with an action of remark, but no remark set.
 error_message_no_remark = "Action is set to remark, you MUST add a remark."
 # Sets a standard error message for ACL rules with an action of remark, but no source_prefix is set.
-error_message_action_remark_source_prefix_set = (
-    "Action is set to remark, Source Prefix CANNOT be set."
-)
+error_message_action_remark_source_prefix_set = "Action is set to remark, Source Prefix CANNOT be set."
 # Sets a standard error message for ACL rules with an action not set to remark, but no remark is set.
-error_message_remark_without_action_remark = (
-    "CANNOT set remark unless action is set to remark."
-)
+error_message_remark_without_action_remark = "CANNOT set remark unless action is set to remark."
 # Sets a standard error message for ACL rules no associated to an ACL of the same type.
 error_message_acl_type = "Provided parent Access List is not of right type."
 
 
 class AccessListSerializer(NetBoxModelSerializer):
     """
     Defines the serializer for the django AccessList model & associates it to a view.
@@ -77,15 +72,15 @@
             "tags",
             "custom_fields",
             "created",
             "last_updated",
             "rule_count",
         )
 
-    @swagger_serializer_method(serializer_or_field=serializers.DictField)
+    @extend_schema_field(serializers.DictField())
     def get_assigned_object(self, obj):
         serializer = get_serializer_for_model(
             obj.assigned_object,
             prefix=NESTED_SERIALIZER_PREFIX,
         )
         context = {"request": self.context["request"]}
         return serializer(obj.assigned_object, context=context).data
@@ -94,35 +89,16 @@
         """
         Validates api inputs before processing:
           - Check that the GFK object is valid.
           - Check if Access List has no existing rules before change the Access List's type.
         """
         error_message = {}
 
-        # Check that the GFK object is valid.
-        if "assigned_object_type" in data and "assigned_object_id" in data:
-            # TODO: This can removed after https://github.com/netbox-community/netbox/issues/10221 is fixed.
-            try:
-                assigned_object = data[  # noqa: F841
-                    "assigned_object_type"
-                ].get_object_for_this_type(
-                    id=data["assigned_object_id"],
-                )
-            except ObjectDoesNotExist:
-                # Sets a standard error message for invalid GFK
-                error_message_invalid_gfk = f"Invalid assigned_object {data['assigned_object_type']} ID {data['assigned_object_id']}"
-                error_message["assigned_object_type"] = [error_message_invalid_gfk]
-                error_message["assigned_object_id"] = [error_message_invalid_gfk]
-
         # Check if Access List has no existing rules before change the Access List's type.
-        if (
-            self.instance
-            and self.instance.type != data.get("type")
-            and self.instance.rule_count > 0
-        ):
+        if self.instance and self.instance.type != data.get("type") and self.instance.rule_count > 0:
             error_message["type"] = [
                 "This ACL has ACL rules associated, CANNOT change ACL type.",
             ]
 
         if error_message:
             raise serializers.ValidationError(error_message)
 
@@ -160,15 +136,15 @@
             "comments",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
 
-    @swagger_serializer_method(serializer_or_field=serializers.DictField)
+    @extend_schema_field(serializers.DictField())
     def get_assigned_object(self, obj):
         serializer = get_serializer_for_model(
             obj.assigned_object,
             prefix=NESTED_SERIALIZER_PREFIX,
         )
         context = {"request": self.context["request"]}
         return serializer(obj.assigned_object, context=context).data
@@ -178,48 +154,23 @@
         Validate the AccessList django model's inputs before allowing it to update the instance.
           - Check that the GFK object is valid.
           - Check that the associated interface's parent host has the selected ACL defined.
         """
         error_message = {}
         acl_host = data["access_list"].assigned_object
 
-        # Check that the GFK object is valid.
-        if "assigned_object_type" in data and "assigned_object_id" in data:
-            # TODO: This can removed after https://github.com/netbox-community/netbox/issues/10221 is fixed.
-            try:
-                assigned_object = data[  # noqa: F841
-                    "assigned_object_type"
-                ].get_object_for_this_type(
-                    id=data["assigned_object_id"],
-                )
-            except ObjectDoesNotExist:
-                # Sets a standard error message for invalid GFK
-                error_message_invalid_gfk = f"Invalid assigned_object {data['assigned_object_type']} ID {data['assigned_object_id']}"
-                error_message["assigned_object_type"] = [error_message_invalid_gfk]
-                error_message["assigned_object_id"] = [error_message_invalid_gfk]
-
         if data["assigned_object_type"].model == "interface":
-            interface_host = (
-                data["assigned_object_type"]
-                .get_object_for_this_type(id=data["assigned_object_id"])
-                .device
-            )
+            interface_host = data["assigned_object_type"].get_object_for_this_type(id=data["assigned_object_id"]).device
         elif data["assigned_object_type"].model == "vminterface":
-            interface_host = (
-                data["assigned_object_type"]
-                .get_object_for_this_type(id=data["assigned_object_id"])
-                .virtual_machine
-            )
+            interface_host = data["assigned_object_type"].get_object_for_this_type(id=data["assigned_object_id"]).virtual_machine
         else:
             interface_host = None
         # Check that the associated interface's parent host has the selected ACL defined.
         if acl_host != interface_host:
-            error_acl_not_assigned_to_host = (
-                "Access List not present on the selected interface's host."
-            )
+            error_acl_not_assigned_to_host = "Access List not present on the selected interface's host."
             error_message["access_list"] = [error_acl_not_assigned_to_host]
             error_message["assigned_object_id"] = [error_acl_not_assigned_to_host]
 
         if error_message:
             raise serializers.ValidationError(error_message)
 
         return super().validate(data)
```

### Comparing `netbox-acls-1.2.2/netbox_acls/api/views.py` & `netbox-acls-1.3.0/netbox_acls/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/choices.py` & `netbox-acls-1.3.0/netbox_acls/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/filtersets.py` & `netbox-acls-1.3.0/netbox_acls/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/forms/bulk_edit.py` & `netbox-acls-1.3.0/netbox_acls/forms/bulk_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 
 # from dcim.models import Device, Region, Site, SiteGroup, VirtualChassis
 # from django import forms
 # from django.core.exceptions import ValidationError
 # from django.utils.safestring import mark_safe
 # from netbox.forms import NetBoxModelBulkEditForm
-# from utilities.forms import (
+# from utilities.forms.utils import add_blank_choice
+# from utilities.forms.fields import (
 #     ChoiceField,
 #     DynamicModelChoiceField,
 #     StaticSelect,
-#     add_blank_choice,
 # )
 # from virtualization.models import VirtualMachine
 
 # from ..choices import ACLActionChoices, ACLTypeChoices
 # from ..models import AccessList
```

### Comparing `netbox-acls-1.2.2/netbox_acls/forms/filtersets.py` & `netbox-acls-1.3.0/netbox_acls/forms/filtersets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Defines each django model's GUI filter/search options.
 """
 
 from dcim.models import Device, Interface, Region, Site, SiteGroup, VirtualChassis
 from django import forms
 from ipam.models import Prefix
 from netbox.forms import NetBoxModelFilterSetForm
-from utilities.forms import (
+from utilities.forms.fields import (
     ChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     TagFilterField,
-    add_blank_choice,
 )
+from utilities.forms.utils import add_blank_choice
 from virtualization.models import VirtualMachine, VMInterface
 
 from ..choices import (
     ACLActionChoices,
     ACLAssignmentDirectionChoices,
     ACLProtocolChoices,
     ACLRuleActionChoices,
```

### Comparing `netbox-acls-1.2.2/netbox_acls/forms/models.py` & `netbox-acls-1.3.0/netbox_acls/forms/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dcim.models import Device, Interface, Region, Site, SiteGroup, VirtualChassis
 from django import forms
 from django.contrib.contenttypes.models import ContentType
 from django.utils.safestring import mark_safe
 from ipam.models import Prefix
 from netbox.forms import NetBoxModelForm
-from utilities.forms import CommentField, DynamicModelChoiceField
+from utilities.forms.fields import CommentField, DynamicModelChoiceField
 from virtualization.models import (
     Cluster,
     ClusterGroup,
     ClusterType,
     VirtualMachine,
     VMInterface,
 )
@@ -35,53 +35,48 @@
 # Sets a standard mark_safe help_text value to be used by the various classes
 help_text_acl_rule_logic = mark_safe(
     "<b>*Note:</b> CANNOT be set if action is set to remark.",
 )
 # Sets a standard help_text value to be used by the various classes for acl action
 help_text_acl_action = "Action the rule will take (remark, deny, or allow)."
 # Sets a standard help_text value to be used by the various classes for acl index
-help_text_acl_rule_index = (
-    "Determines the order of the rule in the ACL processing. AKA Sequence Number."
-)
+help_text_acl_rule_index = "Determines the order of the rule in the ACL processing. AKA Sequence Number."
 
 # Sets a standard error message for ACL rules with an action of remark, but no remark set.
 error_message_no_remark = "Action is set to remark, you MUST add a remark."
 # Sets a standard error message for ACL rules with an action of remark, but no source_prefix is set.
-error_message_action_remark_source_prefix_set = (
-    "Action is set to remark, Source Prefix CANNOT be set."
-)
+error_message_action_remark_source_prefix_set = "Action is set to remark, Source Prefix CANNOT be set."
 # Sets a standard error message for ACL rules with an action not set to remark, but no remark is set.
-error_message_remark_without_action_remark = (
-    "CANNOT set remark unless action is set to remark."
-)
+error_message_remark_without_action_remark = "CANNOT set remark unless action is set to remark."
 
 
 class AccessListForm(NetBoxModelForm):
     """
     GUI form to add or edit an AccessList.
     Requires a device, a name, a type, and a default_action.
     """
 
     # Device selector
     region = DynamicModelChoiceField(
         queryset=Region.objects.all(),
         required=False,
+        initial_params={
+            "sites": "$site",
+        },
     )
     site_group = DynamicModelChoiceField(
         queryset=SiteGroup.objects.all(),
         required=False,
         label="Site Group",
+        initial_params={"sites": "$site"},
     )
     site = DynamicModelChoiceField(
         queryset=Site.objects.all(),
         required=False,
-        query_params={
-            "region_id": "$region",
-            "group_id": "$site_group",
-        },
+        query_params={"region_id": "$region", "group_id": "$site_group"},
     )
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         required=False,
         query_params={
             "region_id": "$region",
             "group_id": "$site_group",
@@ -97,40 +92,32 @@
     )
 
     # Virtual Machine selector
     cluster_type = DynamicModelChoiceField(
         queryset=ClusterType.objects.all(),
         required=False,
     )
-
     cluster_group = DynamicModelChoiceField(
         queryset=ClusterGroup.objects.all(),
         required=False,
-        query_params={
-            "type_id": "$cluster_type",
-        },
+        query_params={"type_id": "$cluster_type"},
     )
-
     cluster = DynamicModelChoiceField(
         queryset=Cluster.objects.all(),
         required=False,
-        query_params={
-            "type_id": "$cluster_type",
-            "group_id": "$cluster_group",
-        },
+        query_params={"type_id": "$cluster_type", "group_id": "$cluster_group"},
     )
 
     virtual_machine = DynamicModelChoiceField(
         queryset=VirtualMachine.objects.all(),
         required=False,
-        label="Virtual Machine",
         query_params={
+            "cluster_id": "$cluster",
             "cluster_type_id": "$cluster_type",
             "cluster_group_id": "$cluster_group",
-            "cluster_id": "$cluster",
         },
     )
 
     comments = CommentField()
 
     class Meta:
         model = AccessList
@@ -152,27 +139,40 @@
             "name": "The name uniqueness per device is case insensitive.",
             "type": mark_safe(
                 "<b>*Note:</b> CANNOT be changed if ACL Rules are assoicated to this Access List.",
             ),
         }
 
     def __init__(self, *args, **kwargs):
-
         # Initialize helper selectors
         instance = kwargs.get("instance")
         initial = kwargs.get("initial", {}).copy()
         if instance:
-            if type(instance.assigned_object) is Device:
+            if isinstance(instance.assigned_object, Device):
                 initial["device"] = instance.assigned_object
-            elif type(instance.assigned_object) is VirtualChassis:
-                initial["virtual_chassis"] = instance.assigned_object
-            elif type(instance.assigned_object) is VirtualMachine:
+                if instance.assigned_object.site:
+                    initial["site"] = instance.assigned_object.site
+                    if instance.assigned_object.site.group:
+                        initial["site_group"] = instance.assigned_object.site.group
+
+                    if instance.assigned_object.site.region:
+                        initial["region"] = instance.assigned_object.site.region
+            elif isinstance(instance.assigned_object, VirtualMachine):
                 initial["virtual_machine"] = instance.assigned_object
-        kwargs["initial"] = initial
+                if instance.assigned_object.cluster:
+                    initial["cluster"] = instance.assigned_object.cluster
+                    if instance.assigned_object.cluster.group:
+                        initial["cluster_group"] = instance.assigned_object.cluster.group
+
+                    if instance.assigned_object.cluster.type:
+                        initial["cluster_type"] = instance.assigned_object.cluster.type
+            elif isinstance(instance.assigned_object, VirtualChassis):
+                initial["virtual_chassis"] = instance.assigned_object
 
+        kwargs["initial"] = initial
         super().__init__(*args, **kwargs)
 
     def clean(self):
         """
         Validates form inputs before submitting:
           - Check if more than one host type selected.
           - Check if no hosts selected.
@@ -186,21 +186,17 @@
         name = cleaned_data.get("name")
         acl_type = cleaned_data.get("type")
         device = cleaned_data.get("device")
         virtual_chassis = cleaned_data.get("virtual_chassis")
         virtual_machine = cleaned_data.get("virtual_machine")
 
         # Check if more than one host type selected.
-        if (
-            (device and virtual_chassis)
-            or (device and virtual_machine)
-            or (virtual_chassis and virtual_machine)
-        ):
+        if (device and virtual_chassis) or (device and virtual_machine) or (virtual_chassis and virtual_machine):
             raise forms.ValidationError(
-                "Access Lists must be assigned to one host (either a device, virtual chassis or virtual machine) at a time.",
+                "Access Lists must be assigned to one host at a time. Either a device, virtual chassis or virtual machine."
             )
         # Check if no hosts selected.
         if not device and not virtual_chassis and not virtual_machine:
             raise forms.ValidationError(
                 "Access Lists must be assigned to a device, virtual chassis or virtual machine.",
             )
 
@@ -217,48 +213,38 @@
             host_type = "virtual_chassis"
             existing_acls = AccessList.objects.filter(
                 name=name,
                 virtual_chassis=virtual_chassis,
             ).exists()
 
         # Check if duplicate entry.
-        if (
-            "name" in self.changed_data or host_type in self.changed_data
-        ) and existing_acls:
-            error_same_acl_name = (
-                "An ACL with this name is already associated to this host."
-            )
+        if ("name" in self.changed_data or host_type in self.changed_data) and existing_acls:
+            error_same_acl_name = "An ACL with this name is already associated to this host."
             error_message |= {
                 host_type: [error_same_acl_name],
                 "name": [error_same_acl_name],
             }
-        if self.instance.pk:
-            # Check if Access List has no existing rules before change the Access List's type.
-            if (
-                acl_type == ACLTypeChoices.TYPE_EXTENDED
-                and self.instance.aclstandardrules.exists()
-            ) or (
-                acl_type == ACLTypeChoices.TYPE_STANDARD
-                and self.instance.aclextendedrules.exists()
-            ):
-                error_message["type"] = [
-                    "This ACL has ACL rules associated, CANNOT change ACL type.",
-                ]
+        # Check if Access List has no existing rules before change the Access List's type.
+        if self.instance.pk and (
+            (acl_type == ACLTypeChoices.TYPE_EXTENDED and self.instance.aclstandardrules.exists())
+            or (acl_type == ACLTypeChoices.TYPE_STANDARD and self.instance.aclextendedrules.exists())
+        ):
+            error_message["type"] = [
+                "This ACL has ACL rules associated, CANNOT change ACL type.",
+            ]
 
         if error_message:
             raise forms.ValidationError(error_message)
 
         return cleaned_data
 
     def save(self, *args, **kwargs):
         # Set assigned object
         self.instance.assigned_object = (
-            self.cleaned_data.get("device")
-            or self.cleaned_data.get("virtual_chassis")
-            or self.cleaned_data.get("virtual_machine")
+            self.cleaned_data.get("device") or self.cleaned_data.get("virtual_chassis") or self.cleaned_data.get("virtual_machine")
         )
 
         return super().save(*args, **kwargs)
 
 
 class ACLInterfaceAssignmentForm(NetBoxModelForm):
     """
@@ -311,15 +297,14 @@
         help_text=mark_safe(
             "<b>*Note:</b> Access List must be present on the device already.",
         ),
     )
     comments = CommentField()
 
     def __init__(self, *args, **kwargs):
-
         # Initialize helper selectors
         instance = kwargs.get("instance")
         initial = kwargs.get("initial", {}).copy()
         if instance:
             if type(instance.assigned_object) is Interface:
                 initial["interface"] = instance.assigned_object
                 initial["device"] = "device"
@@ -363,23 +348,23 @@
         access_list = cleaned_data.get("access_list")
         direction = cleaned_data.get("direction")
         interface = cleaned_data.get("interface")
         vminterface = cleaned_data.get("vminterface")
 
         # Check if both interface and vminterface are set.
         if interface and vminterface:
-            error_too_many_interfaces = "Access Lists must be assigned to one type of interface at a time (VM interface or physical interface)"
+            error_too_many_interfaces = (
+                "Access Lists must be assigned to one type of interface at a time (VM interface or physical interface)"
+            )
             error_message |= {
                 "interface": [error_too_many_interfaces],
                 "vminterface": [error_too_many_interfaces],
             }
         elif not (interface or vminterface):
-            error_no_interface = (
-                "An Access List assignment but specify an Interface or VM Interface."
-            )
+            error_no_interface = "An Access List assignment but specify an Interface or VM Interface."
             error_message |= {
                 "interface": [error_no_interface],
                 "vminterface": [error_no_interface],
             }
         else:
             if interface:
                 assigned_object = interface
@@ -397,17 +382,15 @@
             assigned_object_type_id = ContentType.objects.get_for_model(
                 assigned_object,
             ).pk
             access_list_host = AccessList.objects.get(pk=access_list.pk).assigned_object
 
             # Check that an interface's parent device/virtual_machine is assigned to the Access List.
             if access_list_host != host:
-                error_acl_not_assigned_to_host = (
-                    "Access List not present on selected host."
-                )
+                error_acl_not_assigned_to_host = "Access List not present on selected host."
                 error_message |= {
                     "access_list": [error_acl_not_assigned_to_host],
                     assigned_object_type: [error_acl_not_assigned_to_host],
                     host_type: [error_acl_not_assigned_to_host],
                 }
             # Check for duplicate entry.
             if ACLInterfaceAssignment.objects.filter(
@@ -424,17 +407,15 @@
                 }
             # Check that the interface does not have an existing ACL applied in the direction already.
             if ACLInterfaceAssignment.objects.filter(
                 assigned_object_id=assigned_object_id,
                 assigned_object_type=assigned_object_type_id,
                 direction=direction,
             ).exists():
-                error_interface_already_assigned = (
-                    "Interfaces can only have 1 Access List assigned in each direction."
-                )
+                error_interface_already_assigned = "Interfaces can only have 1 Access List assigned in each direction."
                 error_message |= {
                     "direction": [error_interface_already_assigned],
                     assigned_object_type: [error_interface_already_assigned],
                 }
 
         if error_message:
             raise forms.ValidationError(error_message)
```

### Comparing `netbox-acls-1.2.2/netbox_acls/graphql.py` & `netbox-acls-1.3.0/netbox_acls/graphql/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 """
 Define the object types and queries availble via the graphql api.
 """
 
-from graphene import ObjectType
-from netbox.graphql.fields import ObjectField, ObjectListField
 from netbox.graphql.types import NetBoxObjectType
 
-from . import filtersets, models
+from .. import filtersets, models
 
 __all__ = (
     "AccessListType",
     "ACLInterfaceAssignmentType",
     "ACLExtendedRuleType",
     "ACLStandardRuleType",
 )
 
-#
-# Object types
-#
-
 
 class AccessListType(NetBoxObjectType):
     """
     Defines the object type for the django model AccessList.
     """
 
     class Meta:
@@ -74,30 +68,7 @@
         """
         Associates the filterset, fields, and model for the django model ACLStandardRule.
         """
 
         model = models.ACLStandardRule
         fields = "__all__"
         filterset_class = filtersets.ACLStandardRuleFilterSet
-
-
-#
-# Queries
-#
-
-
-class Query(ObjectType):
-    """
-    Defines the queries availible to this plugin via the graphql api.
-    """
-
-    access_list = ObjectField(AccessListType)
-    access_list_list = ObjectListField(AccessListType)
-
-    acl_extended_rule = ObjectField(ACLExtendedRuleType)
-    acl_extended_rule_list = ObjectListField(ACLExtendedRuleType)
-
-    acl_standard_rule = ObjectField(ACLStandardRuleType)
-    acl_standard_rule_list = ObjectListField(ACLStandardRuleType)
-
-
-schema = Query
```

### Comparing `netbox-acls-1.2.2/netbox_acls/migrations/0001_initial.py` & `netbox-acls-1.3.0/netbox_acls/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,11 +278,13 @@
             options={
                 "ordering": ("access_list", "index"),
                 "unique_together": {("access_list", "index")},
                 "verbose_name": "ACL Extended Rule",
             },
         ),
         # migrations.AddConstraint(
-        #    model_name='accesslist',
-        #    constraint=models.UniqueConstraint(fields=('assigned_object_type', 'assigned_object_id'), name='accesslist_assigned_object'),
+        #     model_name="accesslist",
+        #     constraint=models.UniqueConstraint(
+        #         fields=("assigned_object_type", "assigned_object_id"), name="accesslist_assigned_object"
+        #     ),
         # ),
     ]
```

### Comparing `netbox-acls-1.2.2/netbox_acls/migrations/0002_alter_accesslist_options_and_more.py` & `netbox-acls-1.3.0/netbox_acls/migrations/0002_alter_accesslist_options_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.core.validators
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         ("netbox_acls", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
```

### Comparing `netbox-acls-1.2.2/netbox_acls/migrations/0003_netbox_acls.py` & `netbox-acls-1.3.0/netbox_acls/migrations/0003_netbox_acls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 # Generated by Django 4.1.5 on 2023-01-25 20:08
 
 import utilities.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("netbox_acls", "0002_alter_accesslist_options_and_more"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="accesslist",
             name="custom_field_data",
             field=models.JSONField(
-                blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
+                blank=True,
+                default=dict,
+                encoder=utilities.json.CustomFieldJSONEncoder,
             ),
         ),
         migrations.AlterField(
             model_name="aclextendedrule",
             name="custom_field_data",
             field=models.JSONField(
-                blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
+                blank=True,
+                default=dict,
+                encoder=utilities.json.CustomFieldJSONEncoder,
             ),
         ),
         migrations.AlterField(
             model_name="aclinterfaceassignment",
             name="custom_field_data",
             field=models.JSONField(
-                blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
+                blank=True,
+                default=dict,
+                encoder=utilities.json.CustomFieldJSONEncoder,
             ),
         ),
         migrations.AlterField(
             model_name="aclstandardrule",
             name="custom_field_data",
             field=models.JSONField(
-                blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
+                blank=True,
+                default=dict,
+                encoder=utilities.json.CustomFieldJSONEncoder,
             ),
         ),
     ]
```

### Comparing `netbox-acls-1.2.2/netbox_acls/models/access_list_rules.py` & `netbox-acls-1.3.0/netbox_acls/models/access_list_rules.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/models/access_lists.py` & `netbox-acls-1.3.0/netbox_acls/models/access_lists.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/navigation.py` & `netbox-acls-1.3.0/netbox_acls/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/tables.py` & `netbox-acls-1.3.0/netbox_acls/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/inc/view_tab.html` & `netbox-acls-1.3.0/netbox_acls/templates/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/accesslist.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/accesslist.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 {% block content %}
     <div class="row mb-3">
         <div class="col col-md-6">
             <div class="card">
                 <h5 class="card-header">Access List</h5>
                 <div class="card-body">
                     <table class="table table-hover attr-table">
+                        <caption>Access List</caption>
                         <tr>
                             <th scope="row">Type</th>
                             <td>{{ object.get_type_display }}</td>
                         </tr>
                         <tr>
                             <th scope="row">Default Action</th>
                             <td>{% badge object.get_default_action_display bg_color=object.get_default_action_color %}</td>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
 {% block extra_controls %} {% if perms.netbox_acls.change_policy %} {% if
 object.type == 'extended' %}
 {%_elif_object.type_==_'standard'_%}_{%_endif_%}__Rule_{%_endif_%}_{%_endblock
 extra_controls_%}_{%_block_content_%}
 **_Access_List_**
+                                        Access_List
 Type_____{{_object.get_type_display_}}
          {%_badge
 Default__object.get_default_action_display
 Action___bg_color=object.get_default_action_color
          %}
          {_________________________________________{
 Rules____{_________________________________________{
```

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/accesslist_edit.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/accesslist_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclextendedrule.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclextendedrule.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">ACL Extended Rule</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
+            <caption>ACL Extended Rule</caption>
             <tr>
               <th scope="row">Access List</th>
               <td>
                 <a href="{{ object.access_list.get_absolute_url }}">{{ object.access_list }}</a>
               </td>
             </tr>
             <tr>
@@ -28,14 +29,15 @@
       {% include 'inc/panels/tags.html' %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Details</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
+            <caption>Details</caption>
             <tr>
               <th scope="row">Remark</th>
               <td>{{ object.get_remark_display|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Protocol</th>
               <td>{{ object.get_protocol_display|placeholder }}</td>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 {% extends 'generic/object.html' %} {% block content %}
 ** ACL Extended Rule **
+               ACL Extended Rule
 Access List {{_object.access_list_}}
 Description {{ object.description|placeholder }}
 Index       {{ object.index }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %}
 ** Details **
+                                   Details
 Remark             {{ object.get_remark_display|placeholder }}
 Protocol           {{ object.get_protocol_display|placeholder }}
 Source Prefix      {% if object.source_prefix %} {{_object.source_prefix_}} {%
                    else %} {{ ''|placeholder }} {% endif %}
 Source Ports       {{ object.source_ports|join:", "|placeholder }}
                    {% if object.destination_prefix %} {
 Destination Prefix {_object.destination_prefix_}} {% else %} {{ ''|placeholder
```

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclinterfaceassignment.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclinterfaceassignment.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">ACL Interface Assignment</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
+            <caption>Host</caption>
             <tr>
               <th scope="row">Host</th>
               <td>
                 {% if object.assigned_object.device %}
                 <a href="{{ object.assigned_object.device.get_absolute_url }}">{{ object.assigned_object.device|placeholder }}</a>
                 {% else %}
                 <a href="{{ object.assigned_object.virtual_machine.get_absolute_url }}">{{ object.assigned_object.virtual_machine|placeholder }}</a>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
 {% block content %}
 ** ACL Interface Assignment **
+                                     Host
             {% if object.assigned_object.device %} {
 Host        {_object.assigned_object.device|placeholder_}} {% else %} {
             {_object.assigned_object.virtual_machine|placeholder_}} {% endif %}
 Interface   {{_object.assigned_object_}}
 Access List {{_object.access_list_}}
 Direction   {% badge object.get_direction_display
             bg_color=object.get_direction_color %}
```

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclinterfaceassignment_edit.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclinterfaceassignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-acls-1.2.2/netbox_acls/templates/netbox_acls/aclstandardrule.html` & `netbox-acls-1.3.0/netbox_acls/templates/netbox_acls/aclstandardrule.html`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">ACL Standard Rule</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
+            <caption>ACL Standard Rule</caption>
             <tr>
               <th scope="row">Access List</th>
               <td>
                 <a href="{{ object.access_list.get_absolute_url }}">{{ object.access_list }}</a>
               </td>
             </tr>
             <tr>
@@ -28,14 +29,15 @@
       {% include 'inc/panels/tags.html' %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Details</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
+            <caption>Details</caption>
             <tr>
               <th scope="row">Remark</th>
               <td>{{ object.get_remark_display|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Protocol</th>
               <td>{{ object.get_protocol_display|placeholder }}</td>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 {% extends 'generic/object.html' %} {% block content %}
 ** ACL Standard Rule **
+               ACL Standard Rule
 Access List {{_object.access_list_}}
 Index       {{ object.index }}
 Description {{ object.description|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %}
 ** Details **
+                                   Details
 Remark        {{ object.get_remark_display|placeholder }}
 Protocol      {{ object.get_protocol_display|placeholder }}
 Source Prefix {% if object.source_prefix %} {{_object.source_prefix_}} {% else
               %} {{ ''|placeholder }} {% endif %}
 Action        {% badge object.get_action_display
               bg_color=object.get_action_color %}
 {% endblock content %}
```

### Comparing `netbox-acls-1.2.2/netbox_acls/urls.py` & `netbox-acls-1.3.0/netbox_acls/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Map Views to URLs.
 """
 
 from django.urls import include, path
 from utilities.urls import get_model_urls
 
-from . import models, views
+from . import views
 
 urlpatterns = (
     # Access Lists
     path("access-lists/", views.AccessListListView.as_view(), name="accesslist_list"),
     path(
         "access-lists/add/",
         views.AccessListEditView.as_view(),
@@ -43,15 +43,19 @@
         name="aclinterfaceassignment_list",
     ),
     path(
         "interface-assignments/add/",
         views.ACLInterfaceAssignmentEditView.as_view(),
         name="aclinterfaceassignment_add",
     ),
-    # path('interface-assignments/edit/', views.ACLInterfaceAssignmentBulkEditView.as_view(), name='aclinterfaceassignment_bulk_edit'),
+    # path(
+    #    "interface-assignments/edit/",
+    #    views.ACLInterfaceAssignmentBulkEditView.as_view(),
+    #    name="aclinterfaceassignment_bulk_edit"
+    # ),
     path(
         "interface-assignments/delete/",
         views.ACLInterfaceAssignmentBulkDeleteView.as_view(),
         name="aclinterfaceassignment_bulk_delete",
     ),
     path(
         "interface-assignments/<int:pk>/",
```

### Comparing `netbox-acls-1.2.2/netbox_acls/views.py` & `netbox-acls-1.3.0/netbox_acls/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     Defines the view for the AccessLists django model.
     """
 
     queryset = models.AccessList.objects.prefetch_related("tags")
 
     def get_extra_context(self, request, instance):
         """
-        Depending on the Access List type, the list view will return the required ACL Rule using the previous defined tables in tables.py.
+        Depending on the Access List type, the list view will return
+        the required ACL Rule using the previous defined tables in tables.py.
         """
 
         if instance.type == choices.ACLTypeChoices.TYPE_EXTENDED:
             table = tables.ACLExtendedRuleTable(instance.aclextendedrules.all())
         elif instance.type == choices.ACLTypeChoices.TYPE_STANDARD:
             table = tables.ACLStandardRuleTable(instance.aclstandardrules.all())
         else:
@@ -223,16 +224,15 @@
 
     def get_extra_addanother_params(self, request):
         """
         Returns a dictionary of additional parameters to be passed to the "Add Another" button.
         """
 
         return {
-            "access_list": request.GET.get("access_list")
-            or request.POST.get("access_list"),
+            "access_list": request.GET.get("access_list") or request.POST.get("access_list"),
             "direction": request.GET.get("direction") or request.POST.get("direction"),
         }
 
 
 @register_model_view(models.ACLInterfaceAssignment, "delete")
 class ACLInterfaceAssignmentDeleteView(generic.ObjectDeleteView):
     """
@@ -356,16 +356,15 @@
 
     def get_extra_addanother_params(self, request):
         """
         Returns a dictionary of additional parameters to be passed to the "Add Another" button.
         """
 
         return {
-            "access_list": request.GET.get("access_list")
-            or request.POST.get("access_list"),
+            "access_list": request.GET.get("access_list") or request.POST.get("access_list"),
         }
 
 
 @register_model_view(models.ACLStandardRule, "delete")
 class ACLStandardRuleDeleteView(generic.ObjectDeleteView):
     """
     Defines delete view for the ACLStandardRules django model.
@@ -439,16 +438,15 @@
 
     def get_extra_addanother_params(self, request):
         """
         Returns a dictionary of additional parameters to be passed to the "Add Another" button.
         """
 
         return {
-            "access_list": request.GET.get("access_list")
-            or request.POST.get("access_list"),
+            "access_list": request.GET.get("access_list") or request.POST.get("access_list"),
         }
 
 
 @register_model_view(models.ACLExtendedRule, "delete")
 class ACLExtendedRuleDeleteView(generic.ObjectDeleteView):
     """
     Defines delete view for the ACLExtendedRules django model.
```

### Comparing `netbox-acls-1.2.2/netbox_acls.egg-info/SOURCES.txt` & `netbox-acls-1.3.0/netbox_acls.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 netbox_acls/__init__.py
 netbox_acls/choices.py
 netbox_acls/constants.py
 netbox_acls/filtersets.py
-netbox_acls/graphql.py
 netbox_acls/navigation.py
 netbox_acls/tables.py
 netbox_acls/urls.py
 netbox_acls/version.py
 netbox_acls/views.py
 netbox_acls.egg-info/PKG-INFO
 netbox_acls.egg-info/SOURCES.txt
@@ -22,21 +22,26 @@
 netbox_acls/api/serializers.py
 netbox_acls/api/urls.py
 netbox_acls/api/views.py
 netbox_acls/forms/__init__.py
 netbox_acls/forms/bulk_edit.py
 netbox_acls/forms/filtersets.py
 netbox_acls/forms/models.py
+netbox_acls/graphql/__init__.py
+netbox_acls/graphql/schema.py
+netbox_acls/graphql/types.py
 netbox_acls/migrations/0001_initial.py
 netbox_acls/migrations/0002_alter_accesslist_options_and_more.py
 netbox_acls/migrations/0003_netbox_acls.py
 netbox_acls/migrations/__init__.py
 netbox_acls/models/__init__.py
 netbox_acls/models/access_list_rules.py
 netbox_acls/models/access_lists.py
 netbox_acls/templates/inc/view_tab.html
 netbox_acls/templates/netbox_acls/accesslist.html
 netbox_acls/templates/netbox_acls/accesslist_edit.html
 netbox_acls/templates/netbox_acls/aclextendedrule.html
 netbox_acls/templates/netbox_acls/aclinterfaceassignment.html
 netbox_acls/templates/netbox_acls/aclinterfaceassignment_edit.html
-netbox_acls/templates/netbox_acls/aclstandardrule.html
+netbox_acls/templates/netbox_acls/aclstandardrule.html
+netbox_acls/tests/__init__.py
+netbox_acls/tests/test_api.py
```

