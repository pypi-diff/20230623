# Comparing `tmp/ovos-phal-plugin-ipgeo-0.0.2a3.tar.gz` & `tmp/ovos-phal-plugin-ipgeo-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.2a3.tar", last modified: Wed Jun 21 16:30:34 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-ipgeo-0.0.2a4.tar", last modified: Wed Jun 21 19:37:47 2023, max compression
```

## Comparing `ovos-phal-plugin-ipgeo-0.0.2a3.tar` & `ovos-phal-plugin-ipgeo-0.0.2a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:30:34.106608 ovos-phal-plugin-ipgeo-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 16:30:15.000000 ovos-phal-plugin-ipgeo-0.0.2a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 16:30:34.106608 ovos-phal-plugin-ipgeo-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 16:30:15.000000 ovos-phal-plugin-ipgeo-0.0.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:30:34.106608 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-21 16:30:15.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:30:27.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:30:34.106608 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 16:30:34.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:30:33.000000 ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 16:30:15.000000 ovos-phal-plugin-ipgeo-0.0.2a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:30:34.106608 ovos-phal-plugin-ipgeo-0.0.2a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-21 16:30:15.000000 ovos-phal-plugin-ipgeo-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:47.086730 ovos-phal-plugin-ipgeo-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 19:37:47.086730 ovos-phal-plugin-ipgeo-0.0.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:47.082730 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:47.086730 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:47.000000 ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:37:47.086730 ovos-phal-plugin-ipgeo-0.0.2a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-06-21 19:37:36.000000 ovos-phal-plugin-ipgeo-0.0.2a4/setup.py
```

### Comparing `ovos-phal-plugin-ipgeo-0.0.2a3/ovos_phal_plugin_ipgeo/__init__.py` & `ovos-phal-plugin-ipgeo-0.0.2a4/ovos_phal_plugin_ipgeo/__init__.py`

 * *Files identical despite different names*

