# Comparing `tmp/switch_api-0.4.5.tar.gz` & `tmp/switch_api-0.4.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.4.5.tar", last modified: Thu Jun  8 04:05:26 2023, max compression
+gzip compressed data, was "switch_api-0.4.6b2.tar", last modified: Fri Jun 23 06:58:17 2023, max compression
```

## Comparing `switch_api-0.4.5.tar` & `switch_api-0.4.6b2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.083871 switch_api-0.4.5/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-08 04:05:07.000000 switch_api-0.4.5/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)    26519 2023-06-08 04:05:07.000000 switch_api-0.4.5/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-08 04:05:07.000000 switch_api-0.4.5/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-06-08 04:05:07.000000 switch_api-0.4.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    27793 2023-06-08 04:05:26.083871 switch_api-0.4.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-06-08 04:05:07.000000 switch_api-0.4.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-06-08 04:05:07.000000 switch_api-0.4.5/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-08 04:05:26.083871 switch_api-0.4.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-06-08 04:05:07.000000 switch_api-0.4.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16873 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/email/
--rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/email/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4638 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/email/email_sender.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7519 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2970 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    89676 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.083871 switch_api-0.4.5/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    27793 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1600 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    26549 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27825 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1352 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16873 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4638 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7519 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2970 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3225 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    89676 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27825 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1600 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.4.5/HISTORY.md` & `switch_api-0.4.6b2/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # History
 
+## 0.4.6b1
+- Will be removed
+
 ## 0.4.5
 
 ### Added
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
```

### Comparing `switch_api-0.4.5/LICENCE` & `switch_api-0.4.6b2/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/PKG-INFO` & `switch_api-0.4.6b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_api
-Version: 0.4.5
+Version: 0.4.6b2
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,17 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.4.6b1
+- Will be removed
+
 ## 0.4.5
 
 ### Added
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
```

### Comparing `switch_api-0.4.5/README.md` & `switch_api-0.4.6b2/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/setup.py` & `switch_api-0.4.6b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.4.5",
+    version="0.4.6-beta2",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus', 'msal>=1.11.0'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Other Audience',
```

### Comparing `switch_api-0.4.5/switch_api/__init__.py` & `switch_api-0.4.6b2/switch_api/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.4.5"
+__version__ = "0.4.6-beta2"
```

### Comparing `switch_api-0.4.5/switch_api/_authentication/_authentication.py` & `switch_api-0.4.6b2/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.4.6b2/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/_utils/_constants.py` & `switch_api-0.4.6b2/switch_api/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/_utils/_platform.py` & `switch_api-0.4.6b2/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/_utils/_utils.py` & `switch_api-0.4.6b2/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/analytics/__init__.py` & `switch_api-0.4.6b2/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/analytics/analytics.py` & `switch_api-0.4.6b2/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/cache/cache.py` & `switch_api-0.4.6b2/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/dataset/__init__.py` & `switch_api-0.4.6b2/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/dataset/dataset.py` & `switch_api-0.4.6b2/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/email/email_sender.py` & `switch_api-0.4.6b2/switch_api/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/error_handlers/__init__.py` & `switch_api-0.4.6b2/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/error_handlers/error_handlers.py` & `switch_api-0.4.6b2/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/extensions/__init__.py` & `switch_api-0.4.6b2/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/extensions/extensions.py` & `switch_api-0.4.6b2/switch_api/extensions/extensions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/extensions/field_meta.py` & `switch_api-0.4.6b2/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/extensions/helpers.py` & `switch_api-0.4.6b2/switch_api/extensions/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/extensions/pipeline.py` & `switch_api-0.4.6b2/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/initialize.py` & `switch_api-0.4.6b2/switch_api/initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 
     Returns
     -------
     ApiInputs
         Returns the ApiInputs namedtuple that is required as an input to other functions.
     """
 
+    logger.info('My demo change')
+
     try:
         uuid.UUID(api_project_id)
     except:
-        sw.logger.error(f"Invalid value provided '{api_project_id}'- please provide a valid api_project_id. ")
+        logger.error(f"Invalid value provided '{api_project_id}'- please provide a valid api_project_id. ")
         return False
 
     creds = get_switch_credentials(environment, api_project_id)
 
     logger.info("Successfully initialized.")
     api_base_url = f"https://{creds.api_endpoint}/api/1.0"
     # api_base_url = f"https://localhost:5001/api/1.0"
```

### Comparing `switch_api-0.4.5/switch_api/integration/__init__.py` & `switch_api-0.4.6b2/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/integration/_utils.py` & `switch_api-0.4.6b2/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/integration/helpers.py` & `switch_api-0.4.6b2/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/integration/integration.py` & `switch_api-0.4.6b2/switch_api/integration/integration.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/pipeline/__init__.py` & `switch_api-0.4.6b2/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/pipeline/automation.py` & `switch_api-0.4.6b2/switch_api/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/pipeline/definitions.py` & `switch_api-0.4.6b2/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/pipeline/pipeline.py` & `switch_api-0.4.6b2/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/platform_insights/__init__.py` & `switch_api-0.4.6b2/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api/platform_insights/platform_insights.py` & `switch_api-0.4.6b2/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.5/switch_api.egg-info/PKG-INFO` & `switch_api-0.4.6b2/switch_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-api
-Version: 0.4.5
+Version: 0.4.6b2
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,17 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.4.6b1
+- Will be removed
+
 ## 0.4.5
 
 ### Added
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
```

### Comparing `switch_api-0.4.5/switch_api.egg-info/SOURCES.txt` & `switch_api-0.4.6b2/switch_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

