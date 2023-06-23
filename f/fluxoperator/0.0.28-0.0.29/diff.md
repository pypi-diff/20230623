# Comparing `tmp/fluxoperator-0.0.28.tar.gz` & `tmp/fluxoperator-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.28.tar", last modified: Wed Jun 21 05:22:20 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.29.tar", last modified: Fri Jun 23 19:56:51 2023, max compression
```

## Comparing `fluxoperator-0.0.28.tar` & `fluxoperator-0.0.29.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.681672 fluxoperator-0.0.28/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2005 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13616 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1529 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6151 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.28/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1266 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2005 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13678 2023-06-23 19:56:45.000000 fluxoperator-0.0.29/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.189840 fluxoperator-0.0.29/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1529 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8718 2023-06-23 19:56:45.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.189840 fluxoperator-0.0.29/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6151 2023-06-21 05:22:14.000000 fluxoperator-0.0.29/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.29/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-23 19:56:51.197841 fluxoperator-0.0.29/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1266 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.28/PKG-INFO` & `fluxoperator-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.28
+Version: 0.0.29
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.28/fluxoperator/__init__.py` & `fluxoperator-0.0.29/fluxoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/api_client.py` & `fluxoperator-0.0.29/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/client.py` & `fluxoperator-0.0.29/fluxoperator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 class FluxMiniCluster:
     """
     A MiniCluster is a small class to hold Metadata about a minicluster!
 
     Each MiniCluster holds it's own controller for the Flux Operator.
     """
 
-    def __init__(self):
+    def __init__(self, **kwargs):
         """
         Create a persistent client to interact with a MiniCluster
 
         This currently assumes the namespace exists.
         """
         self.times = {}
         self.metadata = None
         self._pods = None
         self._broker_pod = None
-        self.ctrl = FluxOperator()
+        self.ctrl = FluxOperator(**kwargs)
 
     def load(self, metadata):
         """
         Load minicluster metadata
         """
         self.metadata = metadata
         self._broker_pod = None
@@ -206,21 +206,21 @@
         )
         if print_result:
             print(res, end="")
         return res
 
 
 class FluxOperator:
-    def __init__(self, namespace=None):
+    def __init__(self, namespace=None, **kwargs):
         """
         Create a persistent client to interact with a MiniCluster
 
         This currently assumes the namespace exists.
         """
-        self._core_v1 = None
+        self._core_v1 = kwargs.get('core_v1_api')
         self.namespace = namespace
 
     @property
     def core_v1(self):
         """
         Instantiate a core_v1 api (if not done yet)
 
@@ -380,15 +380,15 @@
         retry_seconds=1,
         quiet=False,
     ):
         """
         Wait for all pods to be running or completed (or in a specific set of states)
         """
         namespace = namespace or self.namespace
-        states = states or ["Running", "Succeeded"]
+        states = states or ["Running", "Succeeded", "Completed"]
         if not isinstance(states, list):
             states = [states]
 
         # We don't have a size - get from cluster
         if not size:
             time.sleep(10)
             pod_list = self.get_pods(name=name, namespace=namespace)
```

### Comparing `fluxoperator-0.0.28/fluxoperator/configuration.py` & `fluxoperator-0.0.29/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/decorator.py` & `fluxoperator-0.0.29/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/exceptions.py` & `fluxoperator-0.0.29/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/__init__.py` & `fluxoperator-0.0.29/fluxoperator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/commands.py` & `fluxoperator-0.0.29/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.29/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.29/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.29/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.29/fluxoperator/models/flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.29/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.29/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.29/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,50 +29,78 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'completed': 'bool',
         'conditions': 'list[V1Condition]',
         'jobid': 'str',
         'maximum_size': 'int',
         'selector': 'str',
         'size': 'int'
     }
 
     attribute_map = {
+        'completed': 'completed',
         'conditions': 'conditions',
         'jobid': 'jobid',
         'maximum_size': 'maximumSize',
         'selector': 'selector',
         'size': 'size'
     }
 
-    def __init__(self, conditions=None, jobid='', maximum_size=0, selector='', size=0, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, completed=False, conditions=None, jobid='', maximum_size=0, selector='', size=0, local_vars_configuration=None):  # noqa: E501
         """MiniClusterStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._completed = None
         self._conditions = None
         self._jobid = None
         self._maximum_size = None
         self._selector = None
         self._size = None
         self.discriminator = None
 
+        if completed is not None:
+            self.completed = completed
         if conditions is not None:
             self.conditions = conditions
         self.jobid = jobid
         self.maximum_size = maximum_size
         self.selector = selector
         self.size = size
 
     @property
+    def completed(self):
+        """Gets the completed of this MiniClusterStatus.  # noqa: E501
+
+        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
+
+        :return: The completed of this MiniClusterStatus.  # noqa: E501
+        :rtype: bool
+        """
+        return self._completed
+
+    @completed.setter
+    def completed(self, completed):
+        """Sets the completed of this MiniClusterStatus.
+
+        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
+
+        :param completed: The completed of this MiniClusterStatus.  # noqa: E501
+        :type completed: bool
+        """
+
+        self._completed = completed
+
+    @property
     def conditions(self):
         """Gets the conditions of this MiniClusterStatus.  # noqa: E501
 
         conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
         :return: The conditions of this MiniClusterStatus.  # noqa: E501
         :rtype: list[V1Condition]
```

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/network.py` & `fluxoperator-0.0.29/fluxoperator/models/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.29/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/models/security_context.py` & `fluxoperator-0.0.29/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/resource/network.py` & `fluxoperator-0.0.29/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/resource/pods.py` & `fluxoperator-0.0.29/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator/rest.py` & `fluxoperator-0.0.29/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.29/fluxoperator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.28
+Version: 0.0.29
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.28/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.29/fluxoperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/setup.py` & `fluxoperator-0.0.29/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.28",
+        version="0.0.29",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.28/test/test_commands.py` & `fluxoperator-0.0.29/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_container_resources.py` & `fluxoperator-0.0.29/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_container_volume.py` & `fluxoperator-0.0.29/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_flux_restful.py` & `fluxoperator-0.0.29/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_flux_spec.py` & `fluxoperator-0.0.29/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_flux_user.py` & `fluxoperator-0.0.29/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_life_cycle.py` & `fluxoperator-0.0.29/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_logging_spec.py` & `fluxoperator-0.0.29/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster.py` & `fluxoperator-0.0.29/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.29/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_container.py` & `fluxoperator-0.0.29/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.29/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_list.py` & `fluxoperator-0.0.29/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.29/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_status.py` & `fluxoperator-0.0.29/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_user.py` & `fluxoperator-0.0.29/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.29/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_network.py` & `fluxoperator-0.0.29/test/test_network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_pod_spec.py` & `fluxoperator-0.0.29/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.28/test/test_security_context.py` & `fluxoperator-0.0.29/test/test_security_context.py`

 * *Files identical despite different names*

