# Comparing `tmp/io4edge_client-0.3.0.tar.gz` & `tmp/io4edge_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io4edge_client-0.3.0.tar", last modified: Wed Jan 18 07:48:44 2023, max compression
+gzip compressed data, was "io4edge_client-0.4.0.tar", last modified: Fri Jun 23 14:33:42 2023, max compression
```

## Comparing `io4edge_client-0.3.0.tar` & `io4edge_client-0.4.0.tar`

### file list

```diff
@@ -1,100 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/analogintypea/
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/analogintypea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/analogintypea/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    14800 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/analogInTypeA_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    35620 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/binaryIoTypeA_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.472860 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    35692 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/binaryIoTypeB_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    43224 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/binaryIoTypeC_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/canL2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/canL2/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/canL2/python/canL2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/canL2/python/canL2/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/canL2/python/canL2/v1alpha1/canL2_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/core_api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/
--rw-r--r--   0 runner    (1001) docker     (122)    28507 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/io4edge_core_api_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/any_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    37894 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/io4edge_functionblock_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/io4edge_inventory_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/motionSensor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/motionSensor/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/motionSensor/python/motionSensor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/motionSensor/python/motionSensor/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    17699 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/motionSensor/python/motionSensor/v1/motionSensor_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbDebug/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbDebug/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbDebug/python/mvbDebug/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    13601 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/mvbDebug_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    13869 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/mvbSniffer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    10715 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/telegram_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/templateInterface/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/templateInterface/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client/api/templateInterface/python/templateInterface/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (122)    19738 2023-01-18 07:48:35.000000 io4edge_client-0.3.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/templateInterface_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/base/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/base/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/base/socket_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/binaryiotypea/
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/binaryiotypea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/binaryiotypea/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/binaryiotypec/
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/binaryiotypec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/binaryiotypec/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/canl2/
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/canl2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/canl2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/functionblock/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/functionblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/functionblock/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/mvbsniffer/
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/mvbsniffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/mvbsniffer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/io4edge_client/util/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/util/any.py
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/io4edge_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 07:48:44.476861 io4edge_client-0.3.0/io4edge_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-01-18 07:48:44.000000 io4edge_client-0.3.0/io4edge_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-01-18 07:48:44.000000 io4edge_client-0.3.0/io4edge_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-18 07:48:44.000000 io4edge_client-0.3.0/io4edge_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-01-18 07:48:44.000000 io4edge_client-0.3.0/io4edge_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-01-18 07:48:44.000000 io4edge_client-0.3.0/io4edge_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-18 07:48:44.480861 io4edge_client-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-01-18 07:48:34.000000 io4edge_client-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/analogintypea/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/analogintypea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/analogintypea/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    14800 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/analogInTypeA_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35620 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/binaryIoTypeA_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.898976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35692 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/binaryIoTypeB_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    43224 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/binaryIoTypeC_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/canL2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/canL2/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/canL2/python/canL2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/canL2/python/canL2/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/canL2/python/canL2/v1alpha1/canL2_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/core_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/
+-rw-r--r--   0 runner    (1001) docker     (122)    28507 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/io4edge_core_api_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/any_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37894 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/io4edge_functionblock_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/io4edge_inventory_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/motionSensor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/motionSensor/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/motionSensor/python/motionSensor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/motionSensor/python/motionSensor/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    17699 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/motionSensor/python/motionSensor/v1/motionSensor_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbDebug/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbDebug/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbDebug/python/mvbDebug/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    13601 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/mvbDebug_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    13869 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/mvbSniffer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10715 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/telegram_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/templateInterface/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/templateInterface/python/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.902976 io4edge_client-0.4.0/io4edge_client/api/templateInterface/python/templateInterface/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (122)    19738 2023-06-23 14:33:29.000000 io4edge_client-0.4.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/templateInterface_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/base/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/base/socket_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/binaryiotypea/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypea/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client/binaryiotypeb/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypeb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypeb/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/io4edge_client/binaryiotypec/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6148 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/binaryiotypec/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/io4edge_client/canl2/
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/canl2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/canl2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/io4edge_client/functionblock/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/functionblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/functionblock/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/io4edge_client/mvbsniffer/
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/mvbsniffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/mvbsniffer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/io4edge_client/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/util/any.py
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/io4edge_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 14:33:42.906976 io4edge_client-0.4.0/io4edge_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-06-23 14:33:42.000000 io4edge_client-0.4.0/io4edge_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-23 14:33:42.000000 io4edge_client-0.4.0/io4edge_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 14:33:42.000000 io4edge_client-0.4.0/io4edge_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-23 14:33:42.000000 io4edge_client-0.4.0/io4edge_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-23 14:33:42.000000 io4edge_client-0.4.0/io4edge_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-23 14:33:42.910976 io4edge_client-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-06-23 14:33:27.000000 io4edge_client-0.4.0/setup.py
```

### Comparing `io4edge_client-0.3.0/PKG-INFO` & `io4edge_client-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: io4edge_client
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python library for io4edge devices
 Home-page: https://github.com/ci4rail/io4edge-client-python
 Author: Ci4Rail GmbH
 Author-email: engineering@ci4rail.com
 Project-URL: Source Code, https://github.com/ci4rail/io4edge-client-python.git
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -16,18 +16,18 @@
 [io4edge devices](https://docs.ci4rail.com/edge-solutions/io4edge/) are intelligent I/O devices invented by [Ci4Rail](https://www.ci4rail.com), connected to the host via network.
 
 This library provides support for the following function blocks within io4edge devices:
 * Analog In TypeA - IOU01, MIO01
 * Binary IO TypeA - IOU01, MIO01
 * CAN Layer2 - IOU03, MIO03, IOU04, MIO04, IOU06
 * MVB Sniffer - IOU03, MIO03
+* Binary IO TypeB - IOU06
 * Binary IO TypeC - IOU07
 
 Currently not supported, but will follow:
-* Binary IO TypeB - IOU06
 * Motion Sensor - CPU01UC
 
 Not planned: Support for io4edge management functions, such as firmware update. Please use io4edge-client-go for this.
 
 
 ## Installation
```

### Comparing `io4edge_client-0.3.0/README.md` & `io4edge_client-0.4.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 [io4edge devices](https://docs.ci4rail.com/edge-solutions/io4edge/) are intelligent I/O devices invented by [Ci4Rail](https://www.ci4rail.com), connected to the host via network.
 
 This library provides support for the following function blocks within io4edge devices:
 * Analog In TypeA - IOU01, MIO01
 * Binary IO TypeA - IOU01, MIO01
 * CAN Layer2 - IOU03, MIO03, IOU04, MIO04, IOU06
 * MVB Sniffer - IOU03, MIO03
+* Binary IO TypeB - IOU06
 * Binary IO TypeC - IOU07
 
 Currently not supported, but will follow:
-* Binary IO TypeB - IOU06
 * Motion Sensor - CPU01UC
 
 Not planned: Support for io4edge management functions, such as firmware update. Please use io4edge-client-go for this.
 
 
 ## Installation
```

### Comparing `io4edge_client-0.3.0/io4edge_client/analogintypea/client.py` & `io4edge_client-0.4.0/io4edge_client/analogintypea/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/analogInTypeA_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/analogInTypeA/python/analogInTypeA/v1alpha1/analogInTypeA_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/binaryIoTypeA_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeA/python/binaryIoTypeA/v1alpha1/binaryIoTypeA_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/binaryIoTypeB_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeB/python/binaryIoTypeB/v1alpha1/binaryIoTypeB_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/binaryIoTypeC_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/binaryIoTypeC/python/binaryIoTypeC/v1alpha1/binaryIoTypeC_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/canL2/python/canL2/v1alpha1/canL2_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/canL2/python/canL2/v1alpha1/canL2_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/io4edge_core_api_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/io4edge/python/core_api/v1alpha2/io4edge_core_api_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/any_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/google/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/io4edge_functionblock_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/io4edge/python/functionblock/v1alpha1/io4edge_functionblock_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/io4edge_inventory_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/io4edge/python/inventory/v1alpha1/io4edge_inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/motionSensor/python/motionSensor/v1/motionSensor_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/motionSensor/python/motionSensor/v1/motionSensor_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/mvbDebug_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/mvbDebug/python/mvbDebug/v1/mvbDebug_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/mvbSniffer_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/mvbSniffer_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/telegram_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/telegram_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/templateInterface_pb2.py` & `io4edge_client-0.4.0/io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/templateInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/base/client.py` & `io4edge_client-0.4.0/io4edge_client/base/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/base/socket_transport.py` & `io4edge_client-0.4.0/io4edge_client/base/socket_transport.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/binaryiotypea/client.py` & `io4edge_client-0.4.0/io4edge_client/binaryiotypea/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/binaryiotypec/client.py` & `io4edge_client-0.4.0/io4edge_client/binaryiotypec/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/canl2/client.py` & `io4edge_client-0.4.0/io4edge_client/canl2/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/functionblock/client.py` & `io4edge_client-0.4.0/io4edge_client/functionblock/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/mvbsniffer/client.py` & `io4edge_client-0.4.0/io4edge_client/mvbsniffer/client.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client/util/any.py` & `io4edge_client-0.4.0/io4edge_client/util/any.py`

 * *Files identical despite different names*

### Comparing `io4edge_client-0.3.0/io4edge_client.egg-info/PKG-INFO` & `io4edge_client-0.4.0/io4edge_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: io4edge-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python library for io4edge devices
 Home-page: https://github.com/ci4rail/io4edge-client-python
 Author: Ci4Rail GmbH
 Author-email: engineering@ci4rail.com
 Project-URL: Source Code, https://github.com/ci4rail/io4edge-client-python.git
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -16,18 +16,18 @@
 [io4edge devices](https://docs.ci4rail.com/edge-solutions/io4edge/) are intelligent I/O devices invented by [Ci4Rail](https://www.ci4rail.com), connected to the host via network.
 
 This library provides support for the following function blocks within io4edge devices:
 * Analog In TypeA - IOU01, MIO01
 * Binary IO TypeA - IOU01, MIO01
 * CAN Layer2 - IOU03, MIO03, IOU04, MIO04, IOU06
 * MVB Sniffer - IOU03, MIO03
+* Binary IO TypeB - IOU06
 * Binary IO TypeC - IOU07
 
 Currently not supported, but will follow:
-* Binary IO TypeB - IOU06
 * Motion Sensor - CPU01UC
 
 Not planned: Support for io4edge management functions, such as firmware update. Please use io4edge-client-go for this.
 
 
 ## Installation
```

### Comparing `io4edge_client-0.3.0/io4edge_client.egg-info/SOURCES.txt` & `io4edge_client-0.4.0/io4edge_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 io4edge_client/api/mvbSniffer/python/mvbSniffer/v1/telegram_pb2.py
 io4edge_client/api/templateInterface/python/templateInterface/v1alpha1/templateInterface_pb2.py
 io4edge_client/base/__init__.py
 io4edge_client/base/client.py
 io4edge_client/base/socket_transport.py
 io4edge_client/binaryiotypea/__init__.py
 io4edge_client/binaryiotypea/client.py
+io4edge_client/binaryiotypeb/__init__.py
+io4edge_client/binaryiotypeb/client.py
 io4edge_client/binaryiotypec/__init__.py
 io4edge_client/binaryiotypec/client.py
 io4edge_client/canl2/__init__.py
 io4edge_client/canl2/client.py
 io4edge_client/functionblock/__init__.py
 io4edge_client/functionblock/client.py
 io4edge_client/mvbsniffer/__init__.py
```

### Comparing `io4edge_client-0.3.0/setup.py` & `io4edge_client-0.4.0/setup.py`

 * *Files identical despite different names*

