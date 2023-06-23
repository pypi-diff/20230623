# Comparing `tmp/radiens-1.0.4.tar.gz` & `tmp/radiens-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiens-1.0.4.tar", last modified: Wed Feb 22 07:00:10 2023, max compression
+gzip compressed data, was "radiens-1.0.5.tar", last modified: Fri Jun 23 21:50:16 2023, max compression
```

## Comparing `radiens-1.0.4.tar` & `radiens-1.0.5.tar`

### file list

```diff
@@ -1,54 +1,108 @@
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.410982 radiens-1.0.4/
--rw-r--r--   0 akelly     (502) staff       (20)     1068 2023-02-15 20:28:22.000000 radiens-1.0.4/LICENSE
--rw-r--r--   0 akelly     (502) staff       (20)      759 2023-02-22 07:00:10.410834 radiens-1.0.4/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)      156 2023-02-15 20:28:22.000000 radiens-1.0.4/README.md
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.405955 radiens-1.0.4/radiens/
--rw-r--r--   0 akelly     (502) staff       (20)      182 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    13160 2023-02-22 06:46:07.000000 radiens-1.0.4/radiens/allego_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.407050 radiens-1.0.4/radiens/api/
--rw-r--r--   0 akelly     (502) staff       (20)       10 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/api/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    22268 2023-02-22 06:24:20.000000 radiens-1.0.4/radiens/api/api_allego.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.407300 radiens-1.0.4/radiens/api/api_utils/
--rw-r--r--   0 akelly     (502) staff       (20)       49 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/api/api_utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     2217 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/api/api_utils/response_parsers.py
--rw-r--r--   0 akelly     (502) staff       (20)     2549 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/api/api_videre.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.407556 radiens-1.0.4/radiens/auth/
--rw-r--r--   0 akelly     (502) staff       (20)       83 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/auth/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     3278 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/auth/interceptors.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.407936 radiens-1.0.4/radiens/exceptions/
--rw-r--r--   0 akelly     (502) staff       (20)      112 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/exceptions/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)      816 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/exceptions/grpc_error.py
--rw-r--r--   0 akelly     (502) staff       (20)      136 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/exceptions/scan_for_server_error.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.410065 radiens-1.0.4/radiens/grpc/
--rw-r--r--   0 akelly     (502) staff       (20)       14 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/grpc/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    28587 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/allegoserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   139617 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/allegoserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    21648 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/biointerface_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/biointerface_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    68877 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/common_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/common_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     8040 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/datasource_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/datasource_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     5354 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/radiens_dev_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/radiens_dev_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    11714 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/radiensserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   151415 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/radiensserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    22177 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/spikesorter_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2023-02-22 06:24:45.000000 radiens-1.0.4/radiens/grpc/spikesorter_pb2_grpc.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.410307 radiens-1.0.4/radiens/signal_group/
--rw-r--r--   0 akelly     (502) staff       (20)     6885 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/signal_group/SignalGroup.py
--rw-r--r--   0 akelly     (502) staff       (20)       20 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/signal_group/__init__.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.410640 radiens-1.0.4/radiens/utils/
--rw-r--r--   0 akelly     (502) staff       (20)       14 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     4277 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/utils/config.py
--rw-r--r--   0 akelly     (502) staff       (20)     4089 2023-02-22 06:24:20.000000 radiens-1.0.4/radiens/utils/constants.py
--rw-r--r--   0 akelly     (502) staff       (20)       22 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens/version.py
--rw-r--r--   0 akelly     (502) staff       (20)     7052 2023-02-15 20:28:22.000000 radiens-1.0.4/radiens/videre_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-02-22 07:00:10.406674 radiens-1.0.4/radiens.egg-info/
--rw-r--r--   0 akelly     (502) staff       (20)      759 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens.egg-info/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)     1233 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens.egg-info/SOURCES.txt
--rw-r--r--   0 akelly     (502) staff       (20)        1 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens.egg-info/dependency_links.txt
--rw-r--r--   0 akelly     (502) staff       (20)       49 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens.egg-info/requires.txt
--rw-r--r--   0 akelly     (502) staff       (20)        8 2023-02-22 07:00:10.000000 radiens-1.0.4/radiens.egg-info/top_level.txt
--rw-r--r--   0 akelly     (502) staff       (20)       38 2023-02-22 07:00:10.411029 radiens-1.0.4/setup.cfg
--rw-r--r--   0 akelly     (502) staff       (20)     1257 2023-02-22 06:24:20.000000 radiens-1.0.4/setup.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.949265 radiens-1.0.5/
+-rw-r--r--   0 akelly     (502) staff       (20)     1068 2023-04-19 19:30:07.000000 radiens-1.0.5/LICENSE
+-rw-r--r--   0 akelly     (502) staff       (20)      610 2023-06-23 21:50:16.949051 radiens-1.0.5/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)      156 2023-04-26 15:20:22.000000 radiens-1.0.5/README.md
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.932307 radiens-1.0.5/radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)      372 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    15861 2023-06-23 21:49:21.000000 radiens-1.0.5/radiens/allego_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.933626 radiens-1.0.5/radiens/api/
+-rw-r--r--   0 akelly     (502) staff       (20)       10 2023-04-19 19:30:07.000000 radiens-1.0.5/radiens/api/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24215 2023-06-23 21:46:19.000000 radiens-1.0.5/radiens/api/api_allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4346 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/api/api_curate.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.934011 radiens-1.0.5/radiens/api/api_utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       19 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/api/api_utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12083 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/api/api_utils/protocols.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11040 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/api/api_utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9202 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/api/api_videre.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.934280 radiens-1.0.5/radiens/auth/
+-rw-r--r--   0 akelly     (502) staff       (20)       83 2023-04-19 19:30:07.000000 radiens-1.0.5/radiens/auth/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3278 2023-04-19 19:30:07.000000 radiens-1.0.5/radiens/auth/interceptors.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.936762 radiens-1.0.5/radiens/cli/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8519 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6359 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/file_sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1890 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/main.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11856 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/signal_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5952 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/signals.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8181 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1813 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5391 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/cli/videre.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.937112 radiens-1.0.5/radiens/common/
+-rw-r--r--   0 akelly     (502) staff       (20)       16 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/common/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1450 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/common/constants.py
+-rw-r--r--   0 akelly     (502) staff       (20)    31922 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/curate_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.937545 radiens-1.0.5/radiens/exceptions/
+-rw-r--r--   0 akelly     (502) staff       (20)      117 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/exceptions/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)      813 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/exceptions/grpc_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)      138 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/exceptions/scan_for_server_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14187 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/file_sys_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.940724 radiens-1.0.5/radiens/grpc_radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)       22 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/grpc_radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    30662 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/allegoserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   153371 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/allegoserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    21909 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/biointerface_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/biointerface_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    75678 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/common_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/common_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8186 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/datasource_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/datasource_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5328 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/radiens_dev_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/radiens_dev_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12488 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/radiensserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   162939 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/radiensserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    22386 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/spikesorter_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2023-06-23 20:06:53.000000 radiens-1.0.5/radiens/grpc_radiens/spikesorter_pb2_grpc.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.943446 radiens-1.0.5/radiens/lib/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1479 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/_obsolete_bokeh_graphics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6168 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/lib/allego_lib.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1479 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/bokeh_graphics.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14572 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/channel_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)      169 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/corelib.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9860 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/dataset_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3611 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/fsys.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.943856 radiens-1.0.5/radiens/lib/graphics/
+-rw-r--r--   0 akelly     (502) staff       (20)       18 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/__init__.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.946001 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/
+-rw-r--r--   0 akelly     (502) staff       (20)       20 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5913 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/dash_datasets.py
+-rw-r--r--   0 akelly     (502) staff       (20)    13168 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/dash_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5197 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/dash_psd.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5197 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/dash_snapshot.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11253 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/lib.py
+-rw-r--r--   0 akelly     (502) staff       (20)      485 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/_obsolete_dashboards/mock_stdout.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.948249 radiens-1.0.5/radiens/lib/graphics/dashboards/
+-rw-r--r--   0 akelly     (502) staff       (20)       20 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9745 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/_obsolete_dash_sig_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5197 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/dash_psd.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10473 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/dash_sig_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5197 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/dash_snapshot.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10399 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/dash_t_range.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4960 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/dashboards/lib.py
+-rw-r--r--   0 akelly     (502) staff       (20)    17060 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/graphics/graphics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1472 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/selector_tables.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10892 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/sig_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4416 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/signals_snapshot.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7459 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10661 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/lib/spikes.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24918 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/metrics_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9249 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/signals_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14749 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8122 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/spikes_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.948817 radiens-1.0.5/radiens/utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       14 2023-04-19 19:30:07.000000 radiens-1.0.5/radiens/utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6982 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/utils/config.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6953 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/utils/constants.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8430 2023-06-08 19:08:16.000000 radiens-1.0.5/radiens/utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)       22 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens/version.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9694 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/videre_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     2937 2023-06-23 19:35:00.000000 radiens-1.0.5/radiens/workspace_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2023-06-23 21:50:16.933087 radiens-1.0.5/radiens.egg-info/
+-rw-r--r--   0 akelly     (502) staff       (20)      610 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)     2998 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/SOURCES.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        1 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/dependency_links.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       49 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/entry_points.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       49 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/requires.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        8 2023-06-23 21:50:16.000000 radiens-1.0.5/radiens.egg-info/top_level.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       38 2023-06-23 21:50:16.949337 radiens-1.0.5/setup.cfg
+-rw-r--r--   0 akelly     (502) staff       (20)     1362 2023-06-08 19:08:16.000000 radiens-1.0.5/setup.py
```

### Comparing `radiens-1.0.4/LICENSE` & `radiens-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `radiens-1.0.4/radiens/api/api_allego.py` & `radiens-1.0.5/radiens/api/api_allego.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,47 @@
+import warnings
+from pprint import pprint
+
 import grpc
 import numpy as np
 import pandas as pd
-import warnings
+from radiens.api.api_utils.util import (parse_stim_param_resp,
+                                        stim_params_dict_to_req)
+from radiens.common.constants import DEFAULT_STIM_PARAMS
 from radiens.exceptions.grpc_error import handle_grpc_error
-from radiens.grpc import (allegoserver_pb2, allegoserver_pb2_grpc,
-                          common_pb2, spikesorter_pb2)
-from radiens.signal_group.SignalGroup import SignalGroup
+from radiens.grpc_radiens import (allegoserver_pb2, allegoserver_pb2_grpc,
+                                  biointerface_pb2, common_pb2, datasource_pb2,
+                                  spikesorter_pb2)
+from radiens.lib.allego_lib import AllegoState
+from radiens.lib.channel_metadata import ChannelMetadata
+from radiens.lib.sig_metrics import SignalMetrics, SignalMetricsStatus
+from radiens.lib.spike_sorter import Dashboard, SorterState
+from radiens.lib.spikes import SpikesMetadata, SpikesSet
 from radiens.utils.config import new_server_channel
-from radiens.utils.constants import (DOUT_MODE_OUT, PORT_, PRIMARY_CACHE_STREAM_GROUP_ID, PORT_ENUM,
-                                     HEADSTAGE_ALIAS, PROBE_ALIAS, SYSTEM_MODE, SYSTEM_MODE_DECODE,
-                                     APPS_, SPK_SORTER_, SPK_SORTER_STATE_DECODE)
+from radiens.utils.constants import (APPS_, DOUT_MODE_OUT, HEADSTAGE_ALIAS,
+                                     PORT_, PORT_ENUM,
+                                     PRIMARY_CACHE_STREAM_GROUP_ID,
+                                     PROBE_ALIAS, SPIKE_SORTER_ID,
+                                     SPK_SORTER_STATE_DECODE, SYSTEM_MODE,
+                                     SYSTEM_MODE_DECODE)
 
 CLIENT_NAME = 'Allego'
 
 # ====== life cycle ======
 
 
 def restart(addr, mode: str):
     if mode not in SYSTEM_MODE.keys():
         raise ValueError('invalid system type {}'.format(mode))
 
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
-            stub.Restart(allegoserver_pb2.RestartRequest(mode=SYSTEM_MODE[mode]))
+            stub.Restart(allegoserver_pb2.RestartRequest(
+                mode=SYSTEM_MODE[mode]))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 # ====== workspace ======
 
 
 def workspace_save(addr, is_force_overwrite=True, tags='', notes=''):
@@ -74,101 +88,67 @@
         try:
             stub.WorkspaceControl(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
 def workspace_current(addr):
-    req = common_pb2.GetWorkspaceRequest(cmd=common_pb2.GET_WSPACE_Current, appMask=common_pb2.Allego)
+    req = common_pb2.GetWorkspaceRequest(
+        cmd=common_pb2.GET_WSPACE_Current, appMask=common_pb2.Allego)
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             resp = stub.GetWorkspace(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        d = {'ID': [], 'app': [], 'last_used': [], 'last_modified': [], 'is_modified': [], 'notes': [], 'tags': []}
+        d = {'ID': [], 'app': [], 'last_used': [], 'last_modified': [],
+             'is_modified': [], 'notes': [], 'tags': []}
         for _, v in resp.workspaceDesc.items():
             d['ID'].append(v.iD)
             d['app'].append(APPS_[v.app])
             d['last_used'].append(v.timestampLastUsed)
             d['last_modified'].append(v.timestampModified)
             d['is_modified'].append(v.isModified)
             d['tags'].append(v.annotation.tags)
             d['notes'].append(v.annotation.notes)
         return pd.DataFrame(d)
 
 
 def workspace_list(addr):
-    req = common_pb2.GetWorkspaceRequest(cmd=common_pb2.GET_WSPACE_List, appMask=common_pb2.Allego)
+    req = common_pb2.GetWorkspaceRequest(
+        cmd=common_pb2.GET_WSPACE_List, appMask=common_pb2.Allego)
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             resp = stub.GetWorkspace(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        d = {'ID': [], 'app': [], 'last_used': [], 'last_modified': [], 'is_modified': [], 'notes': [], 'tags': []}
+        d = {'ID': [], 'app': [], 'last_used': [], 'last_modified': [],
+             'is_modified': [], 'notes': [], 'tags': []}
         for _, v in resp.workspaceDesc.items():
             d['ID'].append(v.iD)
             d['app'].append(APPS_[v.app])
             d['last_used'].append(v.timestampLastUsed)
             d['last_modified'].append(v.timestampModified)
             d['is_modified'].append(v.isModified)
             d['tags'].append(v.annotation.tags)
             d['notes'].append(v.annotation.notes)
         return pd.DataFrame(d)
 
 # ====== getters ======
 
 
-def get_config(addr):
-    cfg = {}
+def get_stream_loop_dur_ms(addr) -> float:
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             res = stub.GetConfig(common_pb2.StandardRequest())
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        else:
-            cable_dict = {}
-            for p in ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L']:
-                try:
-                    cable_dict[p] = eval('res.cableLengths.{}'.format(p))
-                except AttributeError:
-                    pass
-            cfg = {'system_server_port': res.allegoCoreServerPort,
-                   'base_samp_freq': res.baseSampFreq,
-                   'stream_loop_dur_ms': res.streamLoopDurMs,
-                   'headstage_cable_lens': cable_dict,
-                   'backbone_mode': SYSTEM_MODE_DECODE[res.backboneMode]}
-
-        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
-        try:
-            res = stub.GetConfigRecording(common_pb2.StandardRequest())
-        except grpc.RpcError as ex:
-            handle_grpc_error(ex, CLIENT_NAME)
-        else:
-            cfg['base_filename'] = res.baseFileName
-            cfg['filepath'] = res.baseFilePath
-
-        return cfg
-
-
-def get_ports(addr):
-    req = common_pb2.SignalGroupIDRequest()
-    req.streamGroupId = PRIMARY_CACHE_STREAM_GROUP_ID
-    with new_server_channel(addr) as chan:
-        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
-        try:
-            res = stub.ListSensorSpecs(req)
-        except grpc.RpcError as ex:
-            handle_grpc_error(ex, CLIENT_NAME)
-        ports = {}
-        for _, v in enumerate(res.ports):
-            ports[PORT_ENUM[v.port]] = v.channelCount
-        return ports
+        return res.streamLoopDurMs
 
 
 def get_sensors(addr):
     req = common_pb2.SignalGroupIDRequest()
     req.streamGroupId = PRIMARY_CACHE_STREAM_GROUP_ID
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
@@ -181,69 +161,60 @@
             hstages[v.name.strip('hstg__')] = v.channelCount
         probes = {}
         for _, v in enumerate(res.probes):
             probes[v.name.strip('probe__')] = v.channelCount
         return {'headstages': hstages, 'probes': probes}
 
 
-def get_status(addr):
+def get_cfg_status(addr):
     with new_server_channel(addr) as chan:
-        AllegoCoreStub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
-            res = AllegoCoreStub.GetStatus(common_pb2.StandardRequest())
+            res = stub.GetConfigAndStatus(common_pb2.StandardRequest())
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        else:
-            return {'streaming': {'mode': 'on' if res.streaming.streamMode == 1 else 'off',
-                                  'time_range': [res.streaming.primaryCacheTRange[0], res.streaming.primaryCacheTRange[1]],
-                                  'hardware_memory': res.streaming.hardwareMemoryLevel},
-                    'recording': {'mode': 'on' if res.recording.recordMode == 1 else 'off',
-                                  'active_filename': res.recording.activeFileName,
-                                  'duration': res.recording.duration,
-                                  'error': res.recording.error}}
+        return AllegoState(res)
 
 
 def get_signal_group(addr, stream_group_id=None):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             req = common_pb2.SignalGroupIDRequest()
             req.streamGroupId = stream_group_id
 
             raw = stub.GetSignalGroup(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        else:
-            return SignalGroup(raw)
+        return ChannelMetadata(raw)
 
 
 def get_signals(addr, stream_group_id: str, samp_freq: float):
-    sigarray = []
-    time_range = []
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.Pcache1Stub(chan)
         req = common_pb2.GetSignalsRequest(streamGroupId=stream_group_id)
         req.params.timeWindow = 1
         req.params.spacing = 0
         req.params.magnitude = -1
         req.params.plotWidthPoints = samp_freq
         req.params.gpioOnTop = False
         req.params.auxMagnitude = -1
         req.params.componentID = 'allego_python_client'
+        req.params.resampleType = common_pb2.ResampleRoutine.NAIVE
 
         try:
             raw = stub.GetSignals(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        else:
-            sigarray = np.frombuffer(raw.data, dtype=np.float32)
-            sigarray = np.reshape(sigarray, (raw.shape[0], raw.shape[1]))
-            time_range = [raw.timeRange[0], raw.timeRange[1]]
 
-            return sigarray, time_range
+        sigarray = np.frombuffer(raw.data, dtype=np.float32)
+        sigarray = np.reshape(sigarray, (raw.shape[0], raw.shape[1]))
+        time_range = [raw.timeRange[0], raw.timeRange[1]]
+
+        return sigarray, time_range
 
 
 def get_digital_out_states(addr):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             res = stub.GetDIOReg(common_pb2.StandardRequest())
@@ -252,16 +223,57 @@
         else:
             return {
                 'digital_outs_mode': DOUT_MODE_OUT[res.mode],
                 'states': [{'chan_idx': i.ntvChanIdx, 'state': i.manualState} for i in res.doutChanRegisters]
             }
 
 
+def get_dac_register(addr):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            res = stub.GetDACReg(common_pb2.StandardRequest())
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        ch = []
+        for chan in res.analogOutChannels:
+            ch.append({'amp_ntv_chan_idx': chan.PriNtvChanIdx,
+                       'aout_ntv_chan_idx': chan.AnalogOutNtvChanIdx,
+                       'stream': chan.Stream,
+                       'stream_offset_idx': chan.StreamOffsetIdx})
+        return {
+            'dac': ch,
+            'gain': res.gain,
+            'high_pass': {'enable': res.highpassReg.enable,
+                          'cutoff_freq': res.highpassReg.cutoffFreq}}
+
+
+def get_stim_params(addr):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            resp = stub.GetStimParams(common_pb2.StandardRequest())
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+    return parse_stim_param_resp(resp)
+
 # ======= setters ========
 
+
+def set_dac_high_pass(addr, enable: bool, cutoff_freq: float):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            stub.SetDACHighPass(allegoserver_pb2.DACHighPassRegister(enable=enable,
+                                                                     cutoffFreq=cutoff_freq))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return get_dac_register(addr)
+
+
 def set_digital_out_manual(addr, dout1_state: bool, dout2_state: bool):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
 
         req1 = allegoserver_pb2.DIOModeManualRequest()
         req1.chanIdx = 0
         req1.state = dout1_state
@@ -277,59 +289,115 @@
             handle_grpc_error(ex, CLIENT_NAME)
 
 
 def set_fs(addr, fs: int):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
-            stub.SetConfigCore(allegoserver_pb2.SetConfigCoreRequest(sampFreq=float(fs)))
+            stub.SetConfigCore(
+                allegoserver_pb2.SetConfigCoreRequest(sampFreq=float(fs)))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
 def set_sensor(addr, port: str, hstage: str, probe: str):
-    connected_ports = get_ports(addr)
-    if port not in connected_ports.keys():
+    status = get_cfg_status(addr)
+    if port not in status.port_num_channels.keys():
         raise ValueError('port {} is not valid or is connected'.format(port))
     pb_port = PORT_[port]
 
     sensors = get_sensors(addr)
     if hstage in HEADSTAGE_ALIAS.keys():
         pb_hstage = 'hstg__{}'.format(HEADSTAGE_ALIAS[hstage])
     elif hstage in sensors['headstages'].keys():
         pb_hstage = 'hstg__{}'.format(hstage)
     else:
-        raise ValueError('headstage {} is not an alias nor an available headstage ID'.format(hstage))
+        raise ValueError(
+            'headstage {} is not an alias nor an available headstage ID'.format(hstage))
 
     if probe in PROBE_ALIAS.keys():
         pb_probe = 'probe__{}'.format(PROBE_ALIAS[probe])
     elif probe in sensors['probes'].keys():
         pb_probe = 'probe__{}'.format(probe)
     else:
-        raise ValueError('probe {} is not an alias nor an available probe ID'.format(hstage))
+        raise ValueError(
+            'probe {} is not an alias nor an available probe ID'.format(hstage))
 
-    port_num_chan = connected_ports[port]
     hstg_num_chan = sensors['headstages'][pb_hstage.strip('hstg__')]
     probe_num_chan = sensors['probes'][pb_probe.strip('probe__')]
-    if port_num_chan != hstg_num_chan:
+    if status.port_num_channels[port] != hstg_num_chan:
         warnings.warn('port {} number of channels={} does not match headstage number of channels={}'.format(
-                      connected_ports[port], port_num_chan, hstg_num_chan))
+                      port, status.port_num_channels[port], hstg_num_chan))
     if hstg_num_chan != probe_num_chan:
         warnings.warn('headstage {} number of channels={} does not match probe number of channels={}'.format(
                       sensors['headstages'][pb_hstage.strip('hstg__')], hstg_num_chan, probe_num_chan))
 
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             stub.SetSensor(common_pb2.SetSensorRequest(streamGroupId=PRIMARY_CACHE_STREAM_GROUP_ID,
                                                        port=pb_port, headstageId=pb_hstage, probeId=pb_probe))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
+def set_manual_stim_trigger(addr, trigger: int, trigger_on: bool):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            stub.ManualStimTrigger(allegoserver_pb2.ManualStimTriggerRequest(
+                trigger=trigger, triggerOn=trigger_on))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+
+
+def set_stim_step(addr, stim_step_enum: int):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            stub.SetStimStep(allegoserver_pb2.StimStepMessage(
+                stimStep=stim_step_enum))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+
+
+def set_stim_params(addr, stim_params_req: dict):
+    with new_server_channel(addr) as chan:
+        if 'stim_sys_chan_idx' not in stim_params_req:
+            raise KeyError(
+                "Required key stim_sys_chan_idx not found in request.")
+        stim_sys_chan_idx = stim_params_req['stim_sys_chan_idx']
+
+        curr_params = None
+        stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+        try:
+            curr_params_raw = stub.GetStimParams(common_pb2.StandardRequest())
+            curr_params = parse_stim_param_resp(curr_params_raw)
+        except grpc.RpcError as ex:
+            warnings.warn(
+                "can't retrieve any current stim parameters. Continuing with assuming defaults for parameters unspecified in request")
+
+        curr_chan_params = None
+        if curr_params is None or curr_params == {}:
+            curr_chan_params = DEFAULT_STIM_PARAMS
+        else:
+            curr_chan_params = curr_params[stim_sys_chan_idx]
+
+        for param, val in curr_chan_params.items():
+            if param not in stim_params_req:
+                stim_params_req[param] = val
+
+        req = stim_params_dict_to_req(stim_params_req)
+        try:
+            stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
+            stub.SetStimParams(req)
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+
+
 def set_stream_state(addr, state: int):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             stub.SetStreamState(allegoserver_pb2.SetStreamRequest(mode=state))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
@@ -340,21 +408,22 @@
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             stub.SetRecordState(allegoserver_pb2.SetRecordRequest(mode=state))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
-def set_recording_config(addr, filename: str, filepath: str, index: int, time_stamp: str):
+def set_recording_config(addr, filename: str, filepath: str, index: int, time_stamp: bool):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.AllegoCoreStub(chan)
         try:
             stub.SetConfigRecording(allegoserver_pb2.ConfigRecording(baseFileName=filename,
                                                                      baseFilePath=filepath,
-                                                                     datasource_idx=index,
+                                                                     dataSourceIdx=int(
+                                                                         index),
                                                                      timeStamp=time_stamp))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
 def set_time_to_cache_head(addr, stream_group_id=None):
     with new_server_channel(addr) as chan:
@@ -362,117 +431,184 @@
         req = common_pb2.SignalGroupIDRequest()
         req.streamGroupId = stream_group_id
         try:
             stub.SetTimeRangeToHead(req)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
-# ====== spike sorter ======
+# ==========================
+# ====== KPIs ==============
+# ==========================
+
+
+def set_kpi_params(addr, dsource_id,  req):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Kpi1Stub(chan)
+        try:
+            stub.SetKpiParam(req)
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+
 
+def get_kpi_status(addr):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Kpi1Stub(chan)
+        try:
+            resp = stub.GetKpiStatus(common_pb2.GetKpiStatusRequest(
+                streamGroupId=PRIMARY_CACHE_STREAM_GROUP_ID))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return SignalMetricsStatus(resp)
+
+
+def get_kpi_metrics(addr, req):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Kpi1Stub(chan)
+        try:
+            resp = stub.KpiGetMetrics(req)
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return SignalMetrics(PRIMARY_CACHE_STREAM_GROUP_ID, resp)
+
+
+def get_kpi_params(addr):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Kpi1Stub(chan)
+        try:
+            resp = stub.GetKpiParam(datasource_pb2.DataSourceRequest(
+                dsourceID=[PRIMARY_CACHE_STREAM_GROUP_ID]))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        p = {'ntv_idx': [], 'chan_enabled': [], 'thr_activated': [], 'thr': [], 'thr_sd': [], 'thr_wdw': [],
+             'shadow': [], 'weak_thr_activated': [],  'weak_thr': [], 'weak_thr_sd': [], 'thr_wdw_pts': [], 'shadow_pts': []}
+        for v in resp.rec:
+            p['ntv_idx'].append(v.ntvChanIdx)
+            p['chan_enabled'].append(v.isEnabled)
+            p['thr_activated'].append(v.isSetThr)
+            p['thr'].append(np.array(v.thr))
+            p['thr_sd'].append(np.array(v.thrSd))
+            p['thr_wdw'].append(np.around(np.array(v.thrWdw) * 1000.0, 5))
+            p['shadow'].append(np.around(np.array(v.shadow) * 1000.0, 5))
+            p['weak_thr_activated'].append(np.array(v.isSetWeakThr))
+            p['weak_thr'].append(np.array(v.weakThr))
+            p['weak_thr_sd'].append(np.array(v.weakThrSd))
+            p['thr_wdw_pts'].append(v.thrWdwPts)
+            p['shadow_pts'].append(v.shadowPts)
+        return pd.DataFrame(p)
+
+# ==========================
+# ====== spike sorter ======
+# ==========================
 
-def sorter_cmd(addr, cmd: str):
-    if cmd not in SPK_SORTER_.keys():
-        raise ValueError('invalid spike sorter command={}, valid commands are {}'.format(cmd, list(SPK_SORTER_.keys())))
 
+def sorter_cmd(addr, cmd):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
         try:
             stub.SpikeSorterCommand(spikesorter_pb2.SpikeSorterCommandRequest(
-                cmd=SPK_SORTER_[cmd], subCmd=spikesorter_pb2.SORTER_SUBCMD_NULL, spikeSorterID=''))
+                cmd=cmd, subCmd=spikesorter_pb2.SORTER_SUBCMD_NULL, spikeSorterID=''))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+
+
+def sorter_set_params(addr, msg):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
+        try:
+            stub.SpikeSorterSetParams(msg)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
 
 
 def sorter_get_params(addr):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
         try:
-            resp = stub.SpikeSorterGetParam(spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
+            resp = stub.SpikeSorterGetParam(
+                spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        p = {'ntv_chan_idx': [], 'chan_enabled?': [], 'thr_set?': [], 'use_sd?': [], 'thr': [], 'thr_sd': [], 'thr_wdw': [], 'peak_wdw': [],
-             'shadow': [], 'weak_thr': [], 'thr_wdw_pts': [], 'peak_wdw_pts': [], 'shadow_pts': []}
+        p = {'ntv_idx': [], 'chan_enabled': [], 'thr_activated': [], 'thr': [], 'thr_sd': [], 'thr_wdw': [],
+             'shadow': [], 'weak_thr': [], 'thr_wdw_pts': [], 'shadow_pts': []}
         for v in resp.rec:
-            p['ntv_chan_idx'].append(v.ntvChanIdx)
-            p['chan_enabled?'].append(v.isEnabled)
-            p['thr_set?'].append(v.isSetThr)
-            p['use_sd?'].append(v.isSD)
+            p['ntv_idx'].append(v.ntvChanIdx)
+            p['chan_enabled'].append(v.isEnabled)
+            p['thr_activated'].append(v.isSetThr)
             p['thr'].append(np.array(v.thr))
             p['thr_sd'].append(np.array(v.thrSd))
             p['thr_wdw'].append(np.around(np.array(v.thrWdw) * 1000.0, 5))
-            p['peak_wdw'].append(np.around(np.array(v.peakWdw) * 1000.0, 5))
             p['shadow'].append(np.around(np.array(v.shadow) * 1000.0, 5))
             p['weak_thr'].append(np.array(v.weakThr))
             p['thr_wdw_pts'].append(v.thrWdwPts)
-            p['peak_wdw_pts'].append(v.peakWdwPts)
             p['shadow_pts'].append(v.shadowPts)
         return pd.DataFrame(p)
 
 
 def sorter_get_state(addr):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
         try:
-            resp = stub.SpikeSorterGetState(spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
+            resp = stub.SpikeSorterGetState(
+                spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return SorterState(resp)
+
+
+def sorter_get_raster_data(addr, msg):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
+        try:
+            resp = stub.SpikeSorterGetRasterData(msg)
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-        return {'sorter': SPK_SORTER_STATE_DECODE[resp.sys], 'msg': resp.msg,
-                'time_initialize': resp.initializeTime, 'time_start': resp.sessionStartTime, 'time_stop': resp.sessionStopTime}
+
+        sigarray = np.frombuffer(resp.GPIOData, dtype=np.float32)
+        sigarray = np.reshape(sigarray, (resp.GPIOShape[0], resp.GPIOShape[1]))
+        return {'time_range': resp.timeRange, 'timestamp_range': resp.timeStampRange,
+                'spikes': {'ntv_chan_idx': resp.spikeTimestampsByChannel.ntvChanIdx,
+                           'timestamps': resp.spikeTimestampsByChannel.spikeTimestamps,
+                           'labels': resp.spikeTimestampsByChannellabels},
+                'gpio_data': sigarray}
 
 
 def sorter_get_dashboard(addr):
     with new_server_channel(addr) as chan:
         stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
         try:
-            resp = stub.SpikeSorterGetDashboard(spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
+            resp = stub.SpikeSorterGetDashboard(
+                spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=''))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+    return Dashboard(resp)
+
+
+def get_spikes(addr, req):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
+        try:
+            resp = stub.BiointerfaceGetSpikesDense(req)
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return SpikesSet(resp)
+
+
+def get_neurons(addr, req):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
+        try:
+            resp = stub.BiointerfaceGetNeurons(
+                biointerface_pb2.BiointerfaceGetNeuronsRequest(req))
+        except grpc.RpcError as ex:
+            handle_grpc_error(ex, CLIENT_NAME)
+        return resp
+
+
+def get_spikes_spec(addr):
+    with new_server_channel(addr) as chan:
+        stub = allegoserver_pb2_grpc.Neurons1Stub(chan)
+        try:
+            resp = stub.SpikesGetSpec(
+                spikesorter_pb2.SpikeSorterStandardRequest(spikeSorterID=SPIKE_SORTER_ID))
         except grpc.RpcError as ex:
             handle_grpc_error(ex, CLIENT_NAME)
-    sum_stats = []
-    sum_stats.append(pd.DataFrame({'stat': ['probe-snr', 'probe-noise', 'probe-units'],
-                                   'port': ['all', 'all', 'all'],
-                                   'N': [resp.siteStats.snr[11], resp.siteStats.noise[11], resp.siteStats.neuronYield[11]],
-                                   'mean': [resp.siteStats.snr[0], resp.siteStats.noise[0], resp.siteStats.neuronYield[0]],
-                                   'sd': [resp.siteStats.snr[1], resp.siteStats.noise[1], resp.siteStats.neuronYield[1]],
-                                   'min': [resp.siteStats.snr[3], resp.siteStats.noise[3], resp.siteStats.neuronYield[3]],
-                                   'max': [resp.siteStats.snr[4], resp.siteStats.noise[4], resp.siteStats.neuronYield[4]],
-                                   'median': [resp.siteStats.snr[6], resp.siteStats.noise[6], resp.siteStats.neuronYield[6]],
-                                   'mode': [np.NaN, np.NaN, resp.siteStats.neuronYield[2]],
-                                   'mode_cnt': [np.NaN, np.NaN, resp.siteStats.neuronYield[5]],
-                                   'q25': [resp.siteStats.snr[7], resp.siteStats.noise[7], resp.siteStats.neuronYield[7]],
-                                   'q75': [resp.siteStats.snr[8], resp.siteStats.noise[8], resp.siteStats.neuronYield[8]],
-                                   'skew': [resp.siteStats.snr[9], resp.siteStats.noise[9], resp.siteStats.neuronYield[9]],
-                                   'kurtosis': [resp.siteStats.snr[10], resp.siteStats.noise[10], resp.siteStats.neuronYield[10]],
-                                   }))
-    for k in resp.portStats:
-        v = resp.portStats[k]
-        sum_stats.append(pd.DataFrame({'stat': ['port-snr', 'port-noise', 'port-units'],
-                                       'port': [PORT_ENUM[k], PORT_ENUM[k], PORT_ENUM[k]],
-                                       'N': [v.snr[11], v.noise[11], v.neuronYield[11]],
-                                       'mean': [v.snr[0], v.noise[0], v.neuronYield[0]],
-                                       'sd': [v.snr[1], v.noise[1], v.neuronYield[1]],
-                                       'min': [v.snr[3], v.noise[3], v.neuronYield[3]],
-                                       'max': [v.snr[4], v.noise[4], v.neuronYield[4]],
-                                       'median': [v.snr[6], v.noise[6], v.neuronYield[6]],
-                                       'mode': [np.NaN, np.NaN, v.neuronYield[2]],
-                                       'mode_cnt': [np.NaN, np.NaN, v.neuronYield[5]],
-                                       'q25': [v.snr[7], v.noise[7], v.neuronYield[7]],
-                                       'q75': [v.snr[8], v.noise[8], v.neuronYield[8]],
-                                       'skew': [v.snr[9], v.noise[9], v.neuronYield[9]],
-                                       'kurtosis': [v.snr[10], v.noise[10], v.neuronYield[10]],
-                                       }))
-    df_sum_stats = pd.concat(sum_stats, axis=0)
-    return {'enabled_ports': resp.enabledPorts, 'general': {'sorter': SPK_SORTER_STATE_DECODE[resp.general.state.sys],
-                                                            'msg': resp.general.state.msg,
-                                                            'time_range': np.array(resp.general.timeRange),
-                                                            'num_sites_total': resp.general.numTotalSites,
-                                                            'num_sites_enabled': resp.general.numEnabledSites,
-                                                            'num_sites_active': resp.general.numActiveSites,
-                                                            'num_units': resp.general.numNeurons,
-                                                            'probe_yield_mean': resp.general.probeYield,
-                                                            'site_yield_mean': resp.general.siteYield,
-                                                            'num_spikes_processed': resp.general.numSpikesProcessed,
-                                                            'num_spikes_labeled': resp.general.numSpikesLabeled,
-                                                            'sort_efficiency': resp.general.sortEfficiency,
-                                                            'spikes_file_path': resp.general.sinkDesc.path,
-                                                            'spikes_file_base_name': resp.general.sinkDesc.baseName,
-                                                            },
-            'summary_stats': df_sum_stats}
+        return SpikesMetadata(resp)
```

### Comparing `radiens-1.0.4/radiens/auth/interceptors.py` & `radiens-1.0.5/radiens/auth/interceptors.py`

 * *Files identical despite different names*

### Comparing `radiens-1.0.4/radiens/exceptions/grpc_error.py` & `radiens-1.0.5/radiens/exceptions/grpc_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from grpc import RpcError, StatusCode
+from grpc import (RpcError, StatusCode)
 
 
 class RpcException(Exception):
     def __init__(self, message, status_code):
         self.message = message
-        self.code_msg = ". Error code: {}".format(status_code.value[0]) 
+        self.code_msg = ". Error code: {}".format(status_code.value[0])
+
     def __str__(self):
         return self.message + self.code_msg
 
 
-
-
 def handle_grpc_error(ex: RpcError, client_name):
     status_code = ex.code()
     if status_code == StatusCode.UNAVAILABLE:
         raise RpcException("Confirm {} is running".format(client_name), status_code) from None
     if status_code == StatusCode.UNAUTHENTICATED:
         raise RpcException("Invalid authentication", status_code) from None
     if status_code == StatusCode.RESOURCE_EXHAUSTED:
         raise RpcException("Data too big. Try smaller chunks", status_code)
     else:
         raise RpcError(ex) from None
-
-
-
```

### Comparing `radiens-1.0.4/radiens/grpc/allegoserver_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/allegoserver_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,46 +13,48 @@
 
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"4\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"r\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"g\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"^\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"5\n\x10TriggerModeState\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.TriggerMode\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\x80\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x82\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*O\n\x0bTriggerMode\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0c\n\x08T_DOUT_0\x10\x02\x12\x0c\n\x08T_DOUT_1\x10\x03\x12\n\n\x06T_NONE\x10\x04*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01\x32\xe2%\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetTriggerMode\x12\x18.allego.TriggerModeState\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x45\n\x0eGetTriggerMode\x12\x17.allego.StandardRequest\x1a\x18.allego.TriggerModeState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe2\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12H\n\x15GetHDSnapshotFromHead\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\xd8\x01\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x32\xc2\t\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x65\n\x17SpikeSorterGetDashboard\x12\".allego.SpikeSorterStandardRequest\x1a$.allego.SpikeSorterGetDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12m\n\x1a\x42iointerfaceGetSpikesDense\x12$.allego.BiointerfaceGetSpikesRequest\x1a\'.allego.BiointerfaceSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12p\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"4\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"r\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"g\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"9\n\x13\x44\x41\x43HighPassRegister\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\x12\x12\n\ncutoffFreq\x18\x02 \x02(\x01\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"\x90\x01\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\x12\x30\n\x0bhighpassReg\x18\x03 \x02(\x0b\x32\x1b.allego.DACHighPassRegister\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"5\n\x10TriggerModeState\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.TriggerMode\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\x99\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\x12\x17\n\x0f\x66irmwareVersion\x18\x11 \x02(\t\"%\n\x12\x46lashSinapsRequest\x12\x0f\n\x07\x62itfile\x18\x01 \x02(\t\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08\"5\n\x0fStimStepMessage\x12\"\n\x08stimStep\x18\x01 \x02(\x0e\x32\x10.allego.StimStep*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x82\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*O\n\x0bTriggerMode\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0c\n\x08T_DOUT_0\x10\x02\x12\x0c\n\x08T_DOUT_1\x10\x03\x12\n\n\x06T_NONE\x10\x04*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01*\x90\x02\n\x08StimStep\x12\x13\n\x0fStimStepSizeMin\x10\x00\x12\x14\n\x10StimStepSize10nA\x10\x01\x12\x14\n\x10StimStepSize20nA\x10\x02\x12\x14\n\x10StimStepSize50nA\x10\x03\x12\x15\n\x11StimStepSize100nA\x10\x04\x12\x15\n\x11StimStepSize200nA\x10\x05\x12\x15\n\x11StimStepSize500nA\x10\x06\x12\x13\n\x0fStimStepSize1uA\x10\x07\x12\x13\n\x0fStimStepSize2uA\x10\x08\x12\x13\n\x0fStimStepSize5uA\x10\t\x12\x14\n\x10StimStepSize10uA\x10\n\x12\x13\n\x0fStimStepSizeMax\x10\x0b\x32\xbc(\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0eSetDACHighPass\x12\x1b.allego.DACHighPassRegister\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetTriggerMode\x12\x18.allego.TriggerModeState\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12?\n\x0bSetStimStep\x12\x17.allego.StimStepMessage\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0bGetStimStep\x12\x17.allego.StandardRequest\x1a\x17.allego.StimStepMessage\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x45\n\x0eGetTriggerMode\x12\x17.allego.StandardRequest\x1a\x18.allego.TriggerModeState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12\x42\n\x0b\x46lashSinaps\x12\x1a.allego.FlashSinapsRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe4\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12J\n\x15GetHDSnapshotFromHead\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8d\x04\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12I\n\x12SetKpiUpdatePeriod\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x32\xb6\t\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x65\n\x17SpikeSorterGetDashboard\x12\".allego.SpikeSorterStandardRequest\x1a$.allego.SpikeSorterGetDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12\x61\n\x1a\x42iointerfaceGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12p\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'allegoserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _STIMPARAMSREPLY_PARAMSENTRY._options = None
   _STIMPARAMSREPLY_PARAMSENTRY._serialized_options = b'8\001'
-  _STREAMMODE._serialized_start=6284
-  _STREAMMODE._serialized_end=6317
-  _RECORDMODE._serialized_start=6319
-  _RECORDMODE._serialized_end=6352
-  _BACKBONEMODE._serialized_start=6355
-  _BACKBONEMODE._serialized_end=6869
-  _DIOMODE._serialized_start=6871
-  _DIOMODE._serialized_end=6915
-  _TRIGGERMODE._serialized_start=6917
-  _TRIGGERMODE._serialized_end=6996
-  _ALLEGOHALMODE._serialized_start=6998
-  _ALLEGOHALMODE._serialized_end=7111
-  _STIMSHAPE._serialized_start=7113
-  _STIMSHAPE._serialized_end=7200
-  _STIMPOLARITY._serialized_start=7202
-  _STIMPOLARITY._serialized_end=7254
-  _STIMTRIGGEREDGEORLEVEL._serialized_start=7256
-  _STIMTRIGGEREDGEORLEVEL._serialized_end=7307
-  _STIMTRIGGERHIGHORLOW._serialized_start=7309
-  _STIMTRIGGERHIGHORLOW._serialized_end=7356
-  _STIMPULSEORTRAIN._serialized_start=7358
-  _STIMPULSEORTRAIN._serialized_end=7411
+  _STREAMMODE._serialized_start=6513
+  _STREAMMODE._serialized_end=6546
+  _RECORDMODE._serialized_start=6548
+  _RECORDMODE._serialized_end=6581
+  _BACKBONEMODE._serialized_start=6584
+  _BACKBONEMODE._serialized_end=7098
+  _DIOMODE._serialized_start=7100
+  _DIOMODE._serialized_end=7144
+  _TRIGGERMODE._serialized_start=7146
+  _TRIGGERMODE._serialized_end=7225
+  _ALLEGOHALMODE._serialized_start=7227
+  _ALLEGOHALMODE._serialized_end=7340
+  _STIMSHAPE._serialized_start=7342
+  _STIMSHAPE._serialized_end=7429
+  _STIMPOLARITY._serialized_start=7431
+  _STIMPOLARITY._serialized_end=7483
+  _STIMTRIGGEREDGEORLEVEL._serialized_start=7485
+  _STIMTRIGGEREDGEORLEVEL._serialized_end=7536
+  _STIMTRIGGERHIGHORLOW._serialized_start=7538
+  _STIMTRIGGERHIGHORLOW._serialized_end=7585
+  _STIMPULSEORTRAIN._serialized_start=7587
+  _STIMPULSEORTRAIN._serialized_end=7640
+  _STIMSTEP._serialized_start=7643
+  _STIMSTEP._serialized_end=7915
   _RESTARTREQUEST._serialized_start=101
   _RESTARTREQUEST._serialized_end=153
   _SETPROFILEREQUEST._serialized_start=155
   _SETPROFILEREQUEST._serialized_end=213
   _LOGSYSTEMREQUEST._serialized_start=216
   _LOGSYSTEMREQUEST._serialized_end=577
   _LOGSYSTEMREQUEST_LOGSYSTEMMODE._serialized_start=377
@@ -87,74 +89,80 @@
   _DIOMODEMANUALREQUEST._serialized_end=2195
   _DIGITALOUTCHANNELREGISTER._serialized_start=2197
   _DIGITALOUTCHANNELREGISTER._serialized_end=2312
   _DIGITALOUTREGISTER._serialized_start=2314
   _DIGITALOUTREGISTER._serialized_end=2427
   _DACGAINREQUEST._serialized_start=2429
   _DACGAINREQUEST._serialized_end=2459
-  _ANALOGOUTCHANNELREGISTER._serialized_start=2461
-  _ANALOGOUTCHANNELREGISTER._serialized_end=2580
-  _ANALOGOUTREGISTER._serialized_start=2582
-  _ANALOGOUTREGISTER._serialized_end=2676
-  _SERIALNUMBER._serialized_start=2678
-  _SERIALNUMBER._serialized_end=2711
-  _SETSIMPORTSREQUEST._serialized_start=2714
-  _SETSIMPORTSREQUEST._serialized_end=2843
-  _SETSIMPORTSREQUEST_SIMPORT._serialized_start=2789
-  _SETSIMPORTSREQUEST_SIMPORT._serialized_end=2843
-  _SETMUXCHANNELREQUEST._serialized_start=2845
-  _SETMUXCHANNELREQUEST._serialized_end=2884
-  _SETPOTVOLTAGEREQUEST._serialized_start=2886
-  _SETPOTVOLTAGEREQUEST._serialized_end=2925
-  _GETADCLEVELREPLY._serialized_start=2927
-  _GETADCLEVELREPLY._serialized_end=2960
-  _SETPOTRANGEREQUEST._serialized_start=2962
-  _SETPOTRANGEREQUEST._serialized_end=2997
-  _SETPOTMODEREQUEST._serialized_start=2999
-  _SETPOTMODEREQUEST._serialized_end=3032
-  _SETPOTCELLENABLEREQUEST._serialized_start=3034
-  _SETPOTCELLENABLEREQUEST._serialized_end=3075
-  _READWIREOUTREQUEST._serialized_start=3077
-  _READWIREOUTREQUEST._serialized_end=3121
-  _READWIREOUTREPLY._serialized_start=3123
-  _READWIREOUTREPLY._serialized_end=3163
-  _LOGSYSCONFIGREPLY._serialized_start=3166
-  _LOGSYSCONFIGREPLY._serialized_end=3493
-  _PORTINFO._serialized_start=3495
-  _PORTINFO._serialized_end=3584
-  _LOGSYSSTATUSREPLY._serialized_start=3586
-  _LOGSYSSTATUSREPLY._serialized_end=3685
-  _RECORDERSTATUS._serialized_start=3688
-  _RECORDERSTATUS._serialized_end=3874
-  _SYSTEMSTATUS._serialized_start=3877
-  _SYSTEMSTATUS._serialized_end=4283
-  _LOGSYSPCACHEREPLY._serialized_start=4286
-  _LOGSYSPCACHEREPLY._serialized_end=4630
-  _TRIGGERMODESTATE._serialized_start=4632
-  _TRIGGERMODESTATE._serialized_end=4685
-  _LOADALLMOSIREQUEST._serialized_start=4687
-  _LOADALLMOSIREQUEST._serialized_end=4729
-  _TRANSMITMOSIREQUEST._serialized_start=4731
-  _TRANSMITMOSIREQUEST._serialized_end=4752
-  _DUMPMISOREQUEST._serialized_start=4754
-  _DUMPMISOREQUEST._serialized_end=4807
-  _SINAPSSTATUSREGISTERS._serialized_start=4810
-  _SINAPSSTATUSREGISTERS._serialized_end=5194
-  _HALDASHBOARD._serialized_start=5196
-  _HALDASHBOARD._serialized_end=5247
-  _STIMPARAMS._serialized_start=5250
-  _STIMPARAMS._serialized_end=6078
-  _STIMPARAMSREPLY._serialized_start=6081
-  _STIMPARAMSREPLY._serialized_end=6218
-  _STIMPARAMSREPLY_PARAMSENTRY._serialized_start=6153
-  _STIMPARAMSREPLY_PARAMSENTRY._serialized_end=6218
-  _MANUALSTIMTRIGGERREQUEST._serialized_start=6220
-  _MANUALSTIMTRIGGERREQUEST._serialized_end=6282
-  _ALLEGOCORE._serialized_start=7414
-  _ALLEGOCORE._serialized_end=12248
-  _PCACHE1._serialized_start=12251
-  _PCACHE1._serialized_end=12605
-  _KPI1._serialized_start=12608
-  _KPI1._serialized_end=12824
-  _NEURONS1._serialized_start=12827
-  _NEURONS1._serialized_end=14045
+  _DACHIGHPASSREGISTER._serialized_start=2461
+  _DACHIGHPASSREGISTER._serialized_end=2518
+  _ANALOGOUTCHANNELREGISTER._serialized_start=2520
+  _ANALOGOUTCHANNELREGISTER._serialized_end=2639
+  _ANALOGOUTREGISTER._serialized_start=2642
+  _ANALOGOUTREGISTER._serialized_end=2786
+  _SERIALNUMBER._serialized_start=2788
+  _SERIALNUMBER._serialized_end=2821
+  _SETSIMPORTSREQUEST._serialized_start=2824
+  _SETSIMPORTSREQUEST._serialized_end=2953
+  _SETSIMPORTSREQUEST_SIMPORT._serialized_start=2899
+  _SETSIMPORTSREQUEST_SIMPORT._serialized_end=2953
+  _SETMUXCHANNELREQUEST._serialized_start=2955
+  _SETMUXCHANNELREQUEST._serialized_end=2994
+  _SETPOTVOLTAGEREQUEST._serialized_start=2996
+  _SETPOTVOLTAGEREQUEST._serialized_end=3035
+  _GETADCLEVELREPLY._serialized_start=3037
+  _GETADCLEVELREPLY._serialized_end=3070
+  _SETPOTRANGEREQUEST._serialized_start=3072
+  _SETPOTRANGEREQUEST._serialized_end=3107
+  _SETPOTMODEREQUEST._serialized_start=3109
+  _SETPOTMODEREQUEST._serialized_end=3142
+  _SETPOTCELLENABLEREQUEST._serialized_start=3144
+  _SETPOTCELLENABLEREQUEST._serialized_end=3185
+  _READWIREOUTREQUEST._serialized_start=3187
+  _READWIREOUTREQUEST._serialized_end=3231
+  _READWIREOUTREPLY._serialized_start=3233
+  _READWIREOUTREPLY._serialized_end=3273
+  _LOGSYSCONFIGREPLY._serialized_start=3276
+  _LOGSYSCONFIGREPLY._serialized_end=3603
+  _PORTINFO._serialized_start=3605
+  _PORTINFO._serialized_end=3694
+  _LOGSYSSTATUSREPLY._serialized_start=3696
+  _LOGSYSSTATUSREPLY._serialized_end=3795
+  _RECORDERSTATUS._serialized_start=3798
+  _RECORDERSTATUS._serialized_end=3984
+  _SYSTEMSTATUS._serialized_start=3987
+  _SYSTEMSTATUS._serialized_end=4393
+  _LOGSYSPCACHEREPLY._serialized_start=4396
+  _LOGSYSPCACHEREPLY._serialized_end=4740
+  _TRIGGERMODESTATE._serialized_start=4742
+  _TRIGGERMODESTATE._serialized_end=4795
+  _LOADALLMOSIREQUEST._serialized_start=4797
+  _LOADALLMOSIREQUEST._serialized_end=4839
+  _TRANSMITMOSIREQUEST._serialized_start=4841
+  _TRANSMITMOSIREQUEST._serialized_end=4862
+  _DUMPMISOREQUEST._serialized_start=4864
+  _DUMPMISOREQUEST._serialized_end=4917
+  _SINAPSSTATUSREGISTERS._serialized_start=4920
+  _SINAPSSTATUSREGISTERS._serialized_end=5329
+  _FLASHSINAPSREQUEST._serialized_start=5331
+  _FLASHSINAPSREQUEST._serialized_end=5368
+  _HALDASHBOARD._serialized_start=5370
+  _HALDASHBOARD._serialized_end=5421
+  _STIMPARAMS._serialized_start=5424
+  _STIMPARAMS._serialized_end=6252
+  _STIMPARAMSREPLY._serialized_start=6255
+  _STIMPARAMSREPLY._serialized_end=6392
+  _STIMPARAMSREPLY_PARAMSENTRY._serialized_start=6327
+  _STIMPARAMSREPLY_PARAMSENTRY._serialized_end=6392
+  _MANUALSTIMTRIGGERREQUEST._serialized_start=6394
+  _MANUALSTIMTRIGGERREQUEST._serialized_end=6456
+  _STIMSTEPMESSAGE._serialized_start=6458
+  _STIMSTEPMESSAGE._serialized_end=6511
+  _ALLEGOCORE._serialized_start=7918
+  _ALLEGOCORE._serialized_end=13098
+  _PCACHE1._serialized_start=13101
+  _PCACHE1._serialized_end=13457
+  _KPI1._serialized_start=13460
+  _KPI1._serialized_end=13985
+  _NEURONS1._serialized_start=13988
+  _NEURONS1._serialized_end=15194
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/allegoserver_pb2_grpc.py` & `radiens-1.0.5/radiens/grpc_radiens/allegoserver_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,19 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SetDACOff = channel.unary_unary(
                 '/allego.AllegoCore/SetDACOff',
                 request_serializer=common__pb2.DACOffRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
+        self.SetDACHighPass = channel.unary_unary(
+                '/allego.AllegoCore/SetDACHighPass',
+                request_serializer=allegoserver__pb2.DACHighPassRegister.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
         self.SetSimPorts = channel.unary_unary(
                 '/allego.AllegoCore/SetSimPorts',
                 request_serializer=allegoserver__pb2.SetSimPortsRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SetMuxChannel = channel.unary_unary(
                 '/allego.AllegoCore/SetMuxChannel',
@@ -154,14 +159,24 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetStimParams = channel.unary_unary(
                 '/allego.AllegoCore/GetStimParams',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=allegoserver__pb2.StimParamsReply.FromString,
                 )
+        self.SetStimStep = channel.unary_unary(
+                '/allego.AllegoCore/SetStimStep',
+                request_serializer=allegoserver__pb2.StimStepMessage.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
+        self.GetStimStep = channel.unary_unary(
+                '/allego.AllegoCore/GetStimStep',
+                request_serializer=common__pb2.StandardRequest.SerializeToString,
+                response_deserializer=allegoserver__pb2.StimStepMessage.FromString,
+                )
         self.ManualStimTrigger = channel.unary_unary(
                 '/allego.AllegoCore/ManualStimTrigger',
                 request_serializer=allegoserver__pb2.ManualStimTriggerRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetConfig = channel.unary_unary(
                 '/allego.AllegoCore/GetConfig',
@@ -239,14 +254,19 @@
                 response_deserializer=common__pb2.ListSensorSpecsReply.FromString,
                 )
         self.GetSignalGroupIDs = channel.unary_unary(
                 '/allego.AllegoCore/GetSignalGroupIDs',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=common__pb2.GetSignalGroupIDsReply.FromString,
                 )
+        self.GetSorterIDMap = channel.unary_unary(
+                '/allego.AllegoCore/GetSorterIDMap',
+                request_serializer=common__pb2.StandardRequest.SerializeToString,
+                response_deserializer=common__pb2.GetSorterIDMapReply.FromString,
+                )
         self.GetSpikeSorterIDs = channel.unary_unary(
                 '/allego.AllegoCore/GetSpikeSorterIDs',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.GetSpikeSorterIDsReply.FromString,
                 )
         self.GetSignalGroup = channel.unary_unary(
                 '/allego.AllegoCore/GetSignalGroup',
@@ -319,14 +339,19 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetSinapsStatusRegisters = channel.unary_unary(
                 '/allego.AllegoCore/GetSinapsStatusRegisters',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=allegoserver__pb2.SinapsStatusRegisters.FromString,
                 )
+        self.FlashSinaps = channel.unary_unary(
+                '/allego.AllegoCore/FlashSinaps',
+                request_serializer=allegoserver__pb2.FlashSinapsRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
         self.GetOrCreateEventViewer = channel.unary_unary(
                 '/allego.AllegoCore/GetOrCreateEventViewer',
                 request_serializer=common__pb2.EventViewerID.SerializeToString,
                 response_deserializer=common__pb2.EventViewerConfig.FromString,
                 )
         self.UpdateEventViewer = channel.unary_unary(
                 '/allego.AllegoCore/UpdateEventViewer',
@@ -465,14 +490,20 @@
 
     def SetDACOff(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetDACHighPass(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SetSimPorts(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetMuxChannel(self, request, context):
@@ -525,14 +556,26 @@
 
     def GetStimParams(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetStimStep(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetStimStep(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ManualStimTrigger(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetConfig(self, request, context):
@@ -629,14 +672,20 @@
 
     def GetSignalGroupIDs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetSorterIDMap(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetSpikeSorterIDs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSignalGroup(self, request, context):
@@ -727,14 +776,20 @@
 
     def GetSinapsStatusRegisters(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def FlashSinaps(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetOrCreateEventViewer(self, request, context):
         """EventViewer
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -858,14 +913,19 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SetDACOff': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDACOff,
                     request_deserializer=common__pb2.DACOffRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
+            'SetDACHighPass': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetDACHighPass,
+                    request_deserializer=allegoserver__pb2.DACHighPassRegister.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
             'SetSimPorts': grpc.unary_unary_rpc_method_handler(
                     servicer.SetSimPorts,
                     request_deserializer=allegoserver__pb2.SetSimPortsRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SetMuxChannel': grpc.unary_unary_rpc_method_handler(
                     servicer.SetMuxChannel,
@@ -908,14 +968,24 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetStimParams': grpc.unary_unary_rpc_method_handler(
                     servicer.GetStimParams,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=allegoserver__pb2.StimParamsReply.SerializeToString,
             ),
+            'SetStimStep': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetStimStep,
+                    request_deserializer=allegoserver__pb2.StimStepMessage.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
+            'GetStimStep': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetStimStep,
+                    request_deserializer=common__pb2.StandardRequest.FromString,
+                    response_serializer=allegoserver__pb2.StimStepMessage.SerializeToString,
+            ),
             'ManualStimTrigger': grpc.unary_unary_rpc_method_handler(
                     servicer.ManualStimTrigger,
                     request_deserializer=allegoserver__pb2.ManualStimTriggerRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetConfig': grpc.unary_unary_rpc_method_handler(
                     servicer.GetConfig,
@@ -993,14 +1063,19 @@
                     response_serializer=common__pb2.ListSensorSpecsReply.SerializeToString,
             ),
             'GetSignalGroupIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSignalGroupIDs,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=common__pb2.GetSignalGroupIDsReply.SerializeToString,
             ),
+            'GetSorterIDMap': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSorterIDMap,
+                    request_deserializer=common__pb2.StandardRequest.FromString,
+                    response_serializer=common__pb2.GetSorterIDMapReply.SerializeToString,
+            ),
             'GetSpikeSorterIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSpikeSorterIDs,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=spikesorter__pb2.GetSpikeSorterIDsReply.SerializeToString,
             ),
             'GetSignalGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSignalGroup,
@@ -1073,14 +1148,19 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetSinapsStatusRegisters': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSinapsStatusRegisters,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=allegoserver__pb2.SinapsStatusRegisters.SerializeToString,
             ),
+            'FlashSinaps': grpc.unary_unary_rpc_method_handler(
+                    servicer.FlashSinaps,
+                    request_deserializer=allegoserver__pb2.FlashSinapsRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
             'GetOrCreateEventViewer': grpc.unary_unary_rpc_method_handler(
                     servicer.GetOrCreateEventViewer,
                     request_deserializer=common__pb2.EventViewerID.FromString,
                     response_serializer=common__pb2.EventViewerConfig.SerializeToString,
             ),
             'UpdateEventViewer': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdateEventViewer,
@@ -1420,14 +1500,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetDACOff',
             common__pb2.DACOffRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SetDACHighPass(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetDACHighPass',
+            allegoserver__pb2.DACHighPassRegister.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SetSimPorts(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1590,14 +1687,48 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetStimParams',
             common__pb2.StandardRequest.SerializeToString,
             allegoserver__pb2.StimParamsReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SetStimStep(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetStimStep',
+            allegoserver__pb2.StimStepMessage.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetStimStep(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetStimStep',
+            common__pb2.StandardRequest.SerializeToString,
+            allegoserver__pb2.StimStepMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ManualStimTrigger(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1879,14 +2010,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetSignalGroupIDs',
             common__pb2.StandardRequest.SerializeToString,
             common__pb2.GetSignalGroupIDsReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetSorterIDMap(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetSorterIDMap',
+            common__pb2.StandardRequest.SerializeToString,
+            common__pb2.GetSorterIDMapReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetSpikeSorterIDs(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2151,14 +2299,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetSinapsStatusRegisters',
             common__pb2.StandardRequest.SerializeToString,
             allegoserver__pb2.SinapsStatusRegisters.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def FlashSinaps(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/FlashSinaps',
+            allegoserver__pb2.FlashSinapsRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetOrCreateEventViewer(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2276,16 +2441,16 @@
         self.GetHDSnapshot = channel.unary_unary(
                 '/allego.Pcache1/GetHDSnapshot',
                 request_serializer=common__pb2.HDSnapshotRequest.SerializeToString,
                 response_deserializer=common__pb2.HDSnapshot.FromString,
                 )
         self.GetHDSnapshotFromHead = channel.unary_unary(
                 '/allego.Pcache1/GetHDSnapshotFromHead',
-                request_serializer=common__pb2.HDSnapshotRequest.SerializeToString,
-                response_deserializer=common__pb2.HDSnapshot.FromString,
+                request_serializer=common__pb2.HDSnapshotRequest2.SerializeToString,
+                response_deserializer=common__pb2.HDSnapshot2.FromString,
                 )
         self.GetSignals = channel.unary_unary(
                 '/allego.Pcache1/GetSignals',
                 request_serializer=common__pb2.GetSignalsRequest.SerializeToString,
                 response_deserializer=common__pb2.RawSignals.FromString,
                 )
         self.SetTimeRangeToHead = channel.unary_unary(
@@ -2342,16 +2507,16 @@
             'GetHDSnapshot': grpc.unary_unary_rpc_method_handler(
                     servicer.GetHDSnapshot,
                     request_deserializer=common__pb2.HDSnapshotRequest.FromString,
                     response_serializer=common__pb2.HDSnapshot.SerializeToString,
             ),
             'GetHDSnapshotFromHead': grpc.unary_unary_rpc_method_handler(
                     servicer.GetHDSnapshotFromHead,
-                    request_deserializer=common__pb2.HDSnapshotRequest.FromString,
-                    response_serializer=common__pb2.HDSnapshot.SerializeToString,
+                    request_deserializer=common__pb2.HDSnapshotRequest2.FromString,
+                    response_serializer=common__pb2.HDSnapshot2.SerializeToString,
             ),
             'GetSignals': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSignals,
                     request_deserializer=common__pb2.GetSignalsRequest.FromString,
                     response_serializer=common__pb2.RawSignals.SerializeToString,
             ),
             'SetTimeRangeToHead': grpc.unary_unary_rpc_method_handler(
@@ -2413,16 +2578,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/allego.Pcache1/GetHDSnapshotFromHead',
-            common__pb2.HDSnapshotRequest.SerializeToString,
-            common__pb2.HDSnapshot.FromString,
+            common__pb2.HDSnapshotRequest2.SerializeToString,
+            common__pb2.HDSnapshot2.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetSignals(request,
             target,
             options=(),
@@ -2479,14 +2644,34 @@
                 response_deserializer=common__pb2.KpiBundlePacketMetrics.FromString,
                 )
         self.GetKpiStatus = channel.unary_unary(
                 '/allego.Kpi1/GetKpiStatus',
                 request_serializer=common__pb2.GetKpiStatusRequest.SerializeToString,
                 response_deserializer=common__pb2.KpiStatusReply.FromString,
                 )
+        self.SetKpiParam = channel.unary_unary(
+                '/allego.Kpi1/SetKpiParam',
+                request_serializer=common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
+        self.GetKpiParam = channel.unary_unary(
+                '/allego.Kpi1/GetKpiParam',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.FromString,
+                )
+        self.SetKpiUpdatePeriod = channel.unary_unary(
+                '/allego.Kpi1/SetKpiUpdatePeriod',
+                request_serializer=common__pb2.SetKpiParamRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
+        self.SetKpiPacketDur = channel.unary_unary(
+                '/allego.Kpi1/SetKpiPacketDur',
+                request_serializer=common__pb2.SetKpiParamRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
 
 
 class Kpi1Servicer(object):
     """The Kpi1 service definition.
     This is interface for getting data from the KPI stream service
     """
 
@@ -2504,14 +2689,38 @@
 
     def GetKpiStatus(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetKpiParam(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetKpiParam(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetKpiUpdatePeriod(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetKpiPacketDur(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_Kpi1Servicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Healthcheck': grpc.unary_unary_rpc_method_handler(
                     servicer.Healthcheck,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
@@ -2522,14 +2731,34 @@
                     response_serializer=common__pb2.KpiBundlePacketMetrics.SerializeToString,
             ),
             'GetKpiStatus': grpc.unary_unary_rpc_method_handler(
                     servicer.GetKpiStatus,
                     request_deserializer=common__pb2.GetKpiStatusRequest.FromString,
                     response_serializer=common__pb2.KpiStatusReply.SerializeToString,
             ),
+            'SetKpiParam': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetKpiParam,
+                    request_deserializer=common__pb2.SpikeSorterSetParamsRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
+            'GetKpiParam': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKpiParam,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.SerializeToString,
+            ),
+            'SetKpiUpdatePeriod': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetKpiUpdatePeriod,
+                    request_deserializer=common__pb2.SetKpiParamRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
+            'SetKpiPacketDur': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetKpiPacketDur,
+                    request_deserializer=common__pb2.SetKpiParamRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'allego.Kpi1', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -2585,14 +2814,82 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/allego.Kpi1/GetKpiStatus',
             common__pb2.GetKpiStatusRequest.SerializeToString,
             common__pb2.KpiStatusReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def SetKpiParam(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Kpi1/SetKpiParam',
+            common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetKpiParam(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Kpi1/GetKpiParam',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            spikesorter__pb2.GetSpikeSorterParamCommandReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetKpiUpdatePeriod(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Kpi1/SetKpiUpdatePeriod',
+            common__pb2.SetKpiParamRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetKpiPacketDur(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Kpi1/SetKpiPacketDur',
+            common__pb2.SetKpiParamRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class Neurons1Stub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
@@ -2637,16 +2934,16 @@
         self.SpikeSorterGetRasterData = channel.unary_unary(
                 '/allego.Neurons1/SpikeSorterGetRasterData',
                 request_serializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.SpikeSorterRasterDataReply.FromString,
                 )
         self.BiointerfaceGetSpikesDense = channel.unary_unary(
                 '/allego.Neurons1/BiointerfaceGetSpikesDense',
-                request_serializer=biointerface__pb2.BiointerfaceGetSpikesRequest.SerializeToString,
-                response_deserializer=biointerface__pb2.BiointerfaceSpikeDataDenseReply.FromString,
+                request_serializer=biointerface__pb2.SpikesGetSpikesRequest.SerializeToString,
+                response_deserializer=biointerface__pb2.SpikesSpikeDataDenseReply.FromString,
                 )
         self.BiointerfaceGetNeurons = channel.unary_unary(
                 '/allego.Neurons1/BiointerfaceGetNeurons',
                 request_serializer=biointerface__pb2.BiointerfaceGetNeuronsRequest.SerializeToString,
                 response_deserializer=biointerface__pb2.BiointerfaceGetNeuronsReply.FromString,
                 )
         self.BiointerfaceSeekEndSpikeTimestamps = channel.unary_unary(
@@ -2788,16 +3085,16 @@
             'SpikeSorterGetRasterData': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterGetRasterData,
                     request_deserializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.FromString,
                     response_serializer=spikesorter__pb2.SpikeSorterRasterDataReply.SerializeToString,
             ),
             'BiointerfaceGetSpikesDense': grpc.unary_unary_rpc_method_handler(
                     servicer.BiointerfaceGetSpikesDense,
-                    request_deserializer=biointerface__pb2.BiointerfaceGetSpikesRequest.FromString,
-                    response_serializer=biointerface__pb2.BiointerfaceSpikeDataDenseReply.SerializeToString,
+                    request_deserializer=biointerface__pb2.SpikesGetSpikesRequest.FromString,
+                    response_serializer=biointerface__pb2.SpikesSpikeDataDenseReply.SerializeToString,
             ),
             'BiointerfaceGetNeurons': grpc.unary_unary_rpc_method_handler(
                     servicer.BiointerfaceGetNeurons,
                     request_deserializer=biointerface__pb2.BiointerfaceGetNeuronsRequest.FromString,
                     response_serializer=biointerface__pb2.BiointerfaceGetNeuronsReply.SerializeToString,
             ),
             'BiointerfaceSeekEndSpikeTimestamps': grpc.unary_unary_rpc_method_handler(
@@ -2969,16 +3266,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/allego.Neurons1/BiointerfaceGetSpikesDense',
-            biointerface__pb2.BiointerfaceGetSpikesRequest.SerializeToString,
-            biointerface__pb2.BiointerfaceSpikeDataDenseReply.FromString,
+            biointerface__pb2.SpikesGetSpikesRequest.SerializeToString,
+            biointerface__pb2.SpikesSpikeDataDenseReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BiointerfaceGetNeurons(request,
             target,
             options=(),
```

### Comparing `radiens-1.0.4/radiens/grpc/biointerface_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/biointerface_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,134 +10,134 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x62iointerface.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\"!\n\x0cSpikesStdReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\"\x14\n\x12SpikesNewLoadReply\"<\n\x0fSpikesRenameReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x16\n\x0eisForceReplace\x18\x02 \x01(\x08\"\x13\n\x11SpikesGetIDsReply\"\xa3\x04\n\x0fSpikesSpecReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x12\n\ndatasetUID\x18\x02 \x02(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x02(\t\x12\x15\n\rprovenanceUID\x18\x04 \x03(\t\x12\x12\n\npersistDur\x18\x06 \x02(\x01\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x10\n\x08numSites\x18\x08 \x02(\x03\x12\x11\n\tsizeBytes\x18\t \x02(\x03\x12\x1d\n\x15\x65nabledSiteNtvChanIdx\x18\n \x03(\x05\x12\x11\n\ttimeRange\x18\x0b \x03(\x01\x12\x16\n\x0etimestampRange\x18\x0c \x03(\x03\x12\x15\n\rwallTimeStart\x18\r \x02(\t\x12$\n\x04site\x18\x0e \x03(\x0b\x32\x16.allego.SpikesSiteSpec\x12*\n\tsiteStats\x18\x11 \x01(\x0b\x32\x17.allego.SpikesSiteStats\x12\x31\n\tsensorExt\x18\x12 \x01(\x0b\x32\x1e.allego.SensorExtendedMetadata\x12(\n\x07project\x18\x13 \x01(\x0b\x32\x17.allego.ProjectMetadata\x12)\n\x07\x62ioType\x18\x14 \x02(\x0e\x32\x18.allego.BiointerfaceType\x12\x17\n\x0freqNumNeighbors\x18\x15 \x01(\x03\x12\x1c\n\x14neighborhoodRadiusUm\x18\x16 \x01(\x01\"\xc5\x04\n\x0eSpikesSiteSpec\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12,\n\x08neighbor\x18\x02 \x02(\x0b\x32\x1a.allego.NeighborDescriptor\x12\x11\n\tisEnabled\x18\x03 \x02(\x08\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x11\n\tsizeBytes\x18\x06 \x02(\x03\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x08 \x02(\t\x12\x11\n\ttimeRange\x18\t \x03(\x01\x12\x16\n\x0etimestampRange\x18\n \x03(\x03\x12\x16\n\x0espikeTimeRange\x18\x0b \x03(\x01\x12\x1b\n\x13spikeTimestampRange\x18\x0c \x03(\x03\x12\x1c\n\x14spikeTimeRangeMemory\x18\r \x03(\x01\x12!\n\x19spikeTimestampRangeMemory\x18\x0e \x03(\x03\x12\x1c\n\x14spikeCountSiteMemory\x18\x0f \x01(\x03\x12\x16\n\x0espikeCountSite\x18\x10 \x03(\x01\x12\x15\n\rspikeRateSite\x18\x11 \x03(\x01\x12\x14\n\x0cnoiseLevelSd\x18\x12 \x02(\x01\x12\x0f\n\x07snrSite\x18\x13 \x02(\x01\x12(\n\x06neuron\x18\x14 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x12\n\nnumNeurons\x18\x15 \x01(\x05\x12*\n\x07\x63ompLen\x18\x16 \x02(\x0b\x32\x19.allego.SpikeComponentLen\"!\n\x10SpikeLabelRecord\x12\r\n\x05label\x18\x01 \x03(\x05\"\x9a\x02\n\x0bSpikeMatrix\x12\x11\n\tnumSpikes\x18\x01 \x02(\x03\x12\x17\n\x0ftimestampsBytes\x18\x02 \x02(\x0c\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12\x15\n\rwaveformBytes\x18\x04 \x01(\x0c\x12\x13\n\x0bwaveformLen\x18\x05 \x01(\x05\x12\x15\n\rfeaturesBytes\x18\x06 \x01(\x0c\x12\x13\n\x0b\x66\x65\x61turesLen\x18\x07 \x01(\x05\x12\x16\n\x0e\x66\x65\x61tures2Bytes\x18\x08 \x01(\x0c\x12\x14\n\x0c\x66\x65\x61tures2Len\x18\t \x01(\x05\x12\x13\n\x0bzscoreBytes\x18\n \x01(\x0c\x12\x11\n\tzscoreLen\x18\x0b \x01(\x05\x12\x0f\n\x07siteIdx\x18\x0c \x01(\x05\x12\x10\n\x08spikePos\x18\r \x03(\x05\"}\n\x0eSpikeMatrixSet\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x0f\n\x07siteIdx\x18\x02 \x03(\x05\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08sampFreq\x18\x04 \x02(\x01\x12#\n\x06spkMtx\x18\x05 \x03(\x0b\x32\x13.allego.SpikeMatrix\"\x93\x01\n\x14NeuronSpikeMatrixSet\x12\x0e\n\x06labels\x18\x01 \x03(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x0f\n\x07siteIdx\x18\x03 \x03(\x05\x12#\n\x06spkMtx\x18\x04 \x03(\x0b\x32\x13.allego.SpikeMatrix\x12\x16\n\x0etimestampRange\x18\x05 \x03(\x03\x12\x0b\n\x03uID\x18\x06 \x02(\t\"\xa7\x02\n\x1c\x42iointerfaceGetSpikesRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\'\n\x04mode\x18\x02 \x02(\x0e\x32\x19.allego.NeuronsSignalMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x11\n\ttimeStart\x18\x04 \x02(\x01\x12\x10\n\x08timeStop\x18\x05 \x02(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\x12\x1b\n\x13maxSpikesPerChannel\x18\x07 \x02(\x05\x12\x33\n\tspikeComp\x18\x08 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x11\n\tspkSortID\x18\t \x01(\t\"\x99\x01\n\x1a\x42iointerfaceGetHistRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12%\n\x04mode\x18\x02 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12-\n\x0bspikeLabels\x18\x04 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x90\x01\n%BiointerfaceGetSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x8b\x01\n BiointerfaceSpikeTimestampsReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\"S\n)BiointerfaceSeekEndSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x13\n\x0b\x63omponentID\x18\x02 \x02(\t\"Y\n\x1d\x42iointerfaceGetNeuronsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\"\xe4\x02\n\x1b\x42iointerfaceGetNeuronsReply\x12;\n\x04site\x18\x01 \x03(\x0b\x32-.allego.BiointerfaceGetNeuronsReply.SiteEntry\x1a\x36\n\x0eSpikeRateChunk\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x11\n\tspikeRate\x18\x02 \x03(\x01\x1av\n\x07NeuronL\x12(\n\x06neuron\x18\x01 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x41\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\x32.allego.BiointerfaceGetNeuronsReply.SpikeRateChunk\x1aX\n\tSiteEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.allego.BiointerfaceGetNeuronsReply.NeuronL:\x02\x38\x01\"\x87\x02\n\x0fSpikesSiteStats\x12\x17\n\x0fspikeCountStats\x18\t \x03(\x01\x12\x1e\n\x16labeledSpikeCountStats\x18\n \x03(\x01\x12 \n\x18unlabeledSpikeCountStats\x18\x0b \x03(\x01\x12\x16\n\x0espikeRateStats\x18\x0c \x03(\x01\x12\x1d\n\x15labeledSpikeRateStats\x18\r \x03(\x01\x12\x1f\n\x17unlabeledSpikeRateStats\x18\x0e \x03(\x01\x12\x16\n\x0esiteNoiseStats\x18\x0f \x03(\x01\x12\x14\n\x0csiteSnrStats\x18\x10 \x03(\x01\x12\x13\n\x0bneuronStats\x18\x11 \x03(\x01\"f\n\x11SpikeComponentLen\x12\x10\n\x08waveform\x18\x01 \x02(\x05\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x02(\x05\x12\x10\n\x08\x66\x65\x61ture2\x18\x03 \x02(\x05\x12\x0e\n\x06zscore\x18\x04 \x02(\x05\x12\x0c\n\x04nbrs\x18\x05 \x03(\x05\"\xa8\x01\n\x12NeighborDescriptor\x12\x0e\n\x06radius\x18\x01 \x02(\x01\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x10\n\x08\x64istance\x18\x03 \x03(\x01\x12\x10\n\x08thetaDeg\x18\x04 \x03(\x01\x12\x0e\n\x06phiDeg\x18\x05 \x03(\x01\x12\x0b\n\x03num\x18\x06 \x02(\x05\x12\x14\n\x0cSiteCenterUm\x18\x07 \x03(\x01\x12\x17\n\x0fSiteCenterTcsUm\x18\x08 \x03(\x01\"\xf3\x01\n\x10NeuronDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\x16\n\x0esiteNtvChanIdx\x18\x02 \x02(\x05\x12\x12\n\nspikeLabel\x18\x03 \x02(\t\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x12\n\nspikeCount\x18\x06 \x02(\x03\x12\x11\n\tspikeRate\x18\x07 \x02(\x01\x12\x16\n\x0emeanAbsPeakWfm\x18\x08 \x01(\x01\x12\x0b\n\x03snr\x18\t \x01(\x01\x12\x30\n\x08metaData\x18\n \x01(\x0b\x32\x1e.allego.NeuronExtendedMetadata\"\x86\x01\n\x16NeuronExtendedMetadata\x12\x18\n\x10neuronCatalogUID\x18\x01 \x01(\t\x12\x13\n\x0b\x65nsembleUID\x18\x02 \x01(\t\x12\x17\n\x0f\x66uncAssemblyUID\x18\x03 \x03(\t\x12\x12\n\ndatasetUID\x18\x04 \x01(\t\x12\x10\n\x08probeUID\x18\x05 \x01(\t\"\x8b\x01\n\x10NeuronStatistics\x12\x1a\n\x12WaveformAvgAbsAmpl\x18\x01 \x02(\x01\x12\x0b\n\x03Snr\x18\x02 \x02(\x01\x12\x12\n\nspikeCount\x18\x03 \x02(\x03\x12\x14\n\x0c\x61vgSpikeRate\x18\x04 \x02(\x01\x12$\n\x04isih\x18\x05 \x01(\x0b\x32\x16.allego.NeuronHistData\"|\n\x0fSpikeDescriptor\x12\x11\n\ttimestamp\x18\x01 \x02(\x03\x12\r\n\x05label\x18\x02 \x02(\t\x12\x10\n\x08waveform\x18\x03 \x03(\x02\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\x02\x12\x13\n\x0b\x64\x65\x63\x46\x65\x61tures\x18\x05 \x03(\x01\x12\x0e\n\x06zscore\x18\x06 \x03(\x02\"g\n\tSpikeData\x12&\n\x05spike\x18\x01 \x03(\x0b\x32\x17.allego.SpikeDescriptor\x12\x18\n\x10waveformMaxValue\x18\x02 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x03 \x02(\x02\"1\n\rSpikeTimeData\x12\x11\n\tspikeTime\x18\x01 \x03(\x01\x12\r\n\x05label\x18\x02 \x03(\x05\"Q\n\x12SpikeTimestampData\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x02 \x03(\x03\x12\x0e\n\x06labels\x18\x03 \x03(\x05\"\xb6\x02\n\x17SpikeTemplateDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\r\n\x05label\x18\x02 \x02(\t\x12\x11\n\tnumSpikes\x18\x03 \x02(\x03\x12\x10\n\x08waveform\x18\x04 \x02(\x0c\x12\x12\n\nwaveformSd\x18\x05 \x02(\x0c\x12\x13\n\x0blenWaveform\x18\x06 \x02(\x03\x12\x10\n\x08\x66\x65\x61tures\x18\x07 \x02(\x0c\x12\x12\n\nfeaturesSd\x18\x08 \x02(\x0c\x12\x13\n\x0blenFeatures\x18\t \x02(\x03\x12\x11\n\tfeatures2\x18\n \x02(\x0c\x12\x13\n\x0b\x66\x65\x61tures2Sd\x18\x0b \x02(\x0c\x12\x14\n\x0clenFeatures2\x18\x0c \x02(\x03\x12\x0e\n\x06zscore\x18\r \x02(\x0c\x12\x10\n\x08zscoreSd\x18\x0e \x02(\x0c\x12\x11\n\tlenZscore\x18\x0f \x02(\x03\"[\n\x12SiteSpikeTemplates\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x31\n\x08template\x18\x02 \x03(\x0b\x32\x1f.allego.SpikeTemplateDescriptor\"\x97\x01\n\x1f\x42iointerfaceSpikeTemplatesReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12(\n\x04site\x18\x05 \x03(\x0b\x32\x1a.allego.SiteSpikeTemplates\"@\n\x14\x42iointerfaceMetaData\x12(\n\x0bsignalGroup\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\"\xd6\x01\n\x1a\x42iointerfaceSpikeDataReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x03(\x03\x12\x12\n\nntvChanIdx\x18\x05 \x03(\x05\x12\x1f\n\x04site\x18\x06 \x03(\x0b\x32\x11.allego.SpikeData\x12.\n\x08metaData\x18\x07 \x01(\x0b\x32\x1c.allego.BiointerfaceMetaData\"y\n\x1fSpikeDataDenseChannelDescriptor\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0e\n\x06labels\x18\x02 \x03(\x05\x12\x18\n\x10waveformMaxValue\x18\x03 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x04 \x02(\x02\"\xb6\x01\n\x1f\x42iointerfaceSpikeDataDenseReply\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x17\n\x0fwaveformNPoints\x18\x02 \x02(\x05\x12\x14\n\x0ctotalNSpikes\x18\x03 \x02(\x05\x12\x43\n\x12\x63hannelDescriptors\x18\x04 \x03(\x0b\x32\'.allego.SpikeDataDenseChannelDescriptor\x12\x0c\n\x04\x64\x61ta\x18\x05 \x02(\x0c\"\x8a\x01\n\x17GroupSpikeTimeDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12#\n\x04site\x18\x05 \x03(\x0b\x32\x15.allego.SpikeTimeData\"v\n\x16\x42iointerfaceSpiketrain\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12$\n\x04site\x18\x04 \x03(\x0b\x32\x16.allego.SiteSpiketrain\"p\n\x0eSiteSpiketrain\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\"\n\x06neuron\x18\x02 \x03(\x0b\x32\x12.allego.Spiketrain\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12\x14\n\x0cnumNeighbors\x18\x04 \x02(\x05\"\x8b\x02\n\nSpiketrain\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12\r\n\x05label\x18\x02 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x03 \x03(\x03\x12\x14\n\x0cwaveformData\x18\x05 \x03(\x02\x12\x15\n\rwaveformShape\x18\x06 \x03(\x05\x12\x13\n\x0b\x66\x65\x61tureData\x18\x07 \x03(\x02\x12\x14\n\x0c\x66\x65\x61tureShape\x18\x08 \x03(\x05\x12\x12\n\nzscoreData\x18\t \x03(\x02\x12\x13\n\x0bzscoreShape\x18\n \x03(\x05\x12,\n\nneuronDesc\x18\x0f \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x14\n\x0cnumNeighbors\x18\x11 \x02(\x05\"\xb6\x01\n\x0eNeuronHistData\x12\x13\n\x0b\x62inWidthSec\x18\x01 \x02(\x01\x12\x15\n\rhistTimeRange\x18\x02 \x03(\x01\x12%\n\x04mode\x18\x03 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x14\n\x0cnumRefEvents\x18\x04 \x02(\x03\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\x12\x1a\n\x12numProcessedSpikes\x18\x06 \x02(\x03\x12\x0c\n\x04hist\x18\x07 \x03(\x01\"\x9d\x01\n\x0cSiteHistData\x12\x14\n\x0csitePosProbe\x18\x01 \x03(\x01\x12\x14\n\x0csitePosBrain\x18\x02 \x03(\x01\x12(\n\x06neuron\x18\x03 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12$\n\x04hist\x18\x04 \x03(\x0b\x32\x16.allego.NeuronHistData\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\"\x8b\x01\n\x19\x42iointerfaceHistDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12\"\n\x04site\x18\x05 \x03(\x0b\x32\x14.allego.SiteHistData\"\xb4\x01\n\x17\x42iointerfaceSaveRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x11\n\ttimeRange\x18\x04 \x03(\x01\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x1e\n\x16includeNeuronTemplates\x18\x06 \x02(\x08\"\xac\x01\n\x17\x42iointerfaceLoadRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x13\n\x0buidFragment\x18\x04 \x02(\t\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x14\n\x0c\x66orceReplace\x18\x06 \x02(\x08\"\x95\x01\n\x19\x42iointerfaceSaveLoadReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x0b\n\x03uid\x18\x04 \x02(\t\x12\x1c\n\x14\x62iointerfaceMetaFile\x18\x05 \x02(\t\x12\x1a\n\x12neuronTemplateFile\x18\x06 \x02(\t\"2\n\x17\x42iointerfaceGetIDsReply\x12\x17\n\x0f\x62iointerfaceIDs\x18\x01 \x03(\t\"\xef\x01\n\x16\x42iointerfaceVizRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x35\n\x07vizType\x18\x02 \x02(\x0e\x32$.allego.BiointerfaceVizRequest.VType\x12\x12\n\nnumSamples\x18\x03 \x02(\x05\x12\x14\n\x0cisYAutoScale\x18\x04 \x02(\x08\x12\x0c\n\x04yLim\x18\x05 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x06 \x01(\t\x12\x12\n\nisAutoOpen\x18\x07 \x01(\x08\"/\n\x05VType\x12\x15\n\x11VIZ_BIO_TEMPLATES\x10\x00\x12\x0f\n\x0bVIZ_BIO_DEV\x10\x01\"2\n\x14\x42iointerfaceVizReply\x12\x1a\n\x12pngPathAndFileName\x18\x01 \x01(\t*T\n\x10\x42iointerfaceType\x12\x13\n\x0f\x42IO_SPIKETRAINS\x10\x00\x12\x14\n\x10\x42IO_SPIKES_CACHE\x10\x01\x12\x15\n\x11\x42IO_SPIKES_STREAM\x10\x02* \n\x12SpikesImportSchema\x12\n\n\x06NI_SIM\x10\x00*@\n\x13\x42iointerfaceCommand\x12\x13\n\x0f\x42IO_CMD_SAVE_ON\x10\x00\x12\x14\n\x10\x42IO_CMD_SAVE_OFF\x10\x01*J\n\x11\x42iointerfaceState\x12\x0f\n\x0b\x42IO_SAVE_ON\x10\x00\x12\x10\n\x0c\x42IO_SAVE_OFF\x10\x01\x12\x12\n\x0e\x42IO_CONFIGURED\x10\x02*X\n\x11NeuronsSignalMode\x12\n\n\x06Spikes\x10\x00\x12\x13\n\x0fSpikeTimestamps\x10\x01\x12\x0e\n\nSpikeTimes\x10\x02\x12\x12\n\x0eSpikeWaveforms\x10\x03*q\n\x18SpikeDescriptorComponent\x12\x0e\n\nCTimestamp\x10\x00\x12\n\n\x06\x43Label\x10\x01\x12\r\n\tCWaveform\x10\x02\x12\x0c\n\x08\x43\x46\x65\x61ture\x10\x03\x12\x0f\n\x0b\x43\x44\x65\x63\x46\x65\x61ture\x10\x04\x12\x0b\n\x07\x43Zscore\x10\x05*S\n\x0fHistScalingMode\x12\x0c\n\x08\x41sSpikes\x10\x00\x12\x0f\n\x0b\x41sSpikeRate\x10\x01\x12\n\n\x06\x41sNorm\x10\x02\x12\n\n\x06\x41sProb\x10\x03\x12\t\n\x05\x41sRaw\x10\x04\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x62iointerface.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\"!\n\x0cSpikesStdReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\"\x14\n\x12SpikesNewLoadReply\"<\n\x0fSpikesRenameReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x16\n\x0eisForceReplace\x18\x02 \x01(\x08\"\x13\n\x11SpikesGetIDsReply\"\x87\x05\n\x0fSpikesSpecReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x12\n\ndatasetUID\x18\x02 \x02(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x02(\t\x12\x15\n\rprovenanceUID\x18\x04 \x03(\t\x12\x12\n\npersistDur\x18\x06 \x02(\x01\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x10\n\x08numSites\x18\x08 \x02(\x03\x12\x11\n\tsizeBytes\x18\t \x02(\x03\x12\x1d\n\x15\x65nabledSiteNtvChanIdx\x18\n \x03(\x05\x12\x11\n\ttimeRange\x18\x0b \x03(\x01\x12\x16\n\x0etimestampRange\x18\x0c \x03(\x03\x12\x15\n\rwallTimeStart\x18\r \x02(\t\x12$\n\x04site\x18\x0e \x03(\x0b\x32\x16.allego.SpikesSiteSpec\x12*\n\tsiteStats\x18\x11 \x01(\x0b\x32\x17.allego.SpikesSiteStats\x12\x31\n\tsensorExt\x18\x12 \x01(\x0b\x32\x1e.allego.SensorExtendedMetadata\x12(\n\x07project\x18\x13 \x01(\x0b\x32\x17.allego.ProjectMetadata\x12)\n\x07\x62ioType\x18\x14 \x02(\x0e\x32\x18.allego.BiointerfaceType\x12\x17\n\x0freqNumNeighbors\x18\x15 \x01(\x03\x12\x1c\n\x14neighborhoodRadiusUm\x18\x16 \x01(\x01\x12\x1d\n\x02tR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\x12\x1f\n\x02sG\x18\x18 \x01(\x0b\x32\x13.allego.SignalGroup\x12\"\n\x07spikeTR\x18\x19 \x01(\x0b\x32\x11.allego.TimeRange\"\x88\x05\n\x0eSpikesSiteSpec\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12,\n\x08neighbor\x18\x02 \x02(\x0b\x32\x1a.allego.NeighborDescriptor\x12\x11\n\tisEnabled\x18\x03 \x02(\x08\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x11\n\tsizeBytes\x18\x06 \x02(\x03\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x08 \x02(\t\x12\x11\n\ttimeRange\x18\t \x03(\x01\x12\x16\n\x0etimestampRange\x18\n \x03(\x03\x12\x16\n\x0espikeTimeRange\x18\x0b \x03(\x01\x12\x1b\n\x13spikeTimestampRange\x18\x0c \x03(\x03\x12\x1c\n\x14spikeTimeRangeMemory\x18\r \x03(\x01\x12!\n\x19spikeTimestampRangeMemory\x18\x0e \x03(\x03\x12\x1c\n\x14spikeCountSiteMemory\x18\x0f \x01(\x03\x12\x16\n\x0espikeCountSite\x18\x10 \x03(\x01\x12\x15\n\rspikeRateSite\x18\x11 \x03(\x01\x12\x14\n\x0cnoiseLevelSd\x18\x12 \x02(\x01\x12\x0f\n\x07snrSite\x18\x13 \x02(\x01\x12(\n\x06neuron\x18\x14 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x12\n\nnumNeurons\x18\x15 \x01(\x05\x12*\n\x07\x63ompLen\x18\x16 \x02(\x0b\x32\x19.allego.SpikeComponentLen\x12\x1d\n\x02tR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\x12\"\n\x07spikeTR\x18\x18 \x01(\x0b\x32\x11.allego.TimeRange\"!\n\x10SpikeLabelRecord\x12\r\n\x05label\x18\x01 \x03(\x05\"\x9a\x02\n\x0bSpikeMatrix\x12\x11\n\tnumSpikes\x18\x01 \x02(\x03\x12\x17\n\x0ftimestampsBytes\x18\x02 \x02(\x0c\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12\x15\n\rwaveformBytes\x18\x04 \x01(\x0c\x12\x13\n\x0bwaveformLen\x18\x05 \x01(\x05\x12\x15\n\rfeaturesBytes\x18\x06 \x01(\x0c\x12\x13\n\x0b\x66\x65\x61turesLen\x18\x07 \x01(\x05\x12\x16\n\x0e\x66\x65\x61tures2Bytes\x18\x08 \x01(\x0c\x12\x14\n\x0c\x66\x65\x61tures2Len\x18\t \x01(\x05\x12\x13\n\x0bzscoreBytes\x18\n \x01(\x0c\x12\x11\n\tzscoreLen\x18\x0b \x01(\x05\x12\x0f\n\x07siteIdx\x18\x0c \x01(\x05\x12\x10\n\x08spikePos\x18\r \x03(\x05\"}\n\x0eSpikeMatrixSet\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x0f\n\x07siteIdx\x18\x02 \x03(\x05\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08sampFreq\x18\x04 \x02(\x01\x12#\n\x06spkMtx\x18\x05 \x03(\x0b\x32\x13.allego.SpikeMatrix\"\x93\x01\n\x14NeuronSpikeMatrixSet\x12\x0e\n\x06labels\x18\x01 \x03(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x0f\n\x07siteIdx\x18\x03 \x03(\x05\x12#\n\x06spkMtx\x18\x04 \x03(\x0b\x32\x13.allego.SpikeMatrix\x12\x16\n\x0etimestampRange\x18\x05 \x03(\x03\x12\x0b\n\x03uID\x18\x06 \x02(\t\"\xa1\x02\n\x16SpikesGetSpikesRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\'\n\x04mode\x18\x02 \x02(\x0e\x32\x19.allego.NeuronsSignalMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x11\n\ttimeStart\x18\x04 \x02(\x01\x12\x10\n\x08timeStop\x18\x05 \x02(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\x12\x1b\n\x13maxSpikesPerChannel\x18\x07 \x02(\x05\x12\x33\n\tspikeComp\x18\x08 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x11\n\tspkSortID\x18\t \x01(\t\"\x99\x01\n\x1a\x42iointerfaceGetHistRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12%\n\x04mode\x18\x02 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12-\n\x0bspikeLabels\x18\x04 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x90\x01\n%BiointerfaceGetSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x8b\x01\n BiointerfaceSpikeTimestampsReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\"S\n)BiointerfaceSeekEndSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x13\n\x0b\x63omponentID\x18\x02 \x02(\t\"Y\n\x1d\x42iointerfaceGetNeuronsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\"\xe4\x02\n\x1b\x42iointerfaceGetNeuronsReply\x12;\n\x04site\x18\x01 \x03(\x0b\x32-.allego.BiointerfaceGetNeuronsReply.SiteEntry\x1a\x36\n\x0eSpikeRateChunk\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x11\n\tspikeRate\x18\x02 \x03(\x01\x1av\n\x07NeuronL\x12(\n\x06neuron\x18\x01 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x41\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\x32.allego.BiointerfaceGetNeuronsReply.SpikeRateChunk\x1aX\n\tSiteEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.allego.BiointerfaceGetNeuronsReply.NeuronL:\x02\x38\x01\"\x87\x02\n\x0fSpikesSiteStats\x12\x17\n\x0fspikeCountStats\x18\t \x03(\x01\x12\x1e\n\x16labeledSpikeCountStats\x18\n \x03(\x01\x12 \n\x18unlabeledSpikeCountStats\x18\x0b \x03(\x01\x12\x16\n\x0espikeRateStats\x18\x0c \x03(\x01\x12\x1d\n\x15labeledSpikeRateStats\x18\r \x03(\x01\x12\x1f\n\x17unlabeledSpikeRateStats\x18\x0e \x03(\x01\x12\x16\n\x0esiteNoiseStats\x18\x0f \x03(\x01\x12\x14\n\x0csiteSnrStats\x18\x10 \x03(\x01\x12\x13\n\x0bneuronStats\x18\x11 \x03(\x01\"f\n\x11SpikeComponentLen\x12\x10\n\x08waveform\x18\x01 \x02(\x05\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x02(\x05\x12\x10\n\x08\x66\x65\x61ture2\x18\x03 \x02(\x05\x12\x0e\n\x06zscore\x18\x04 \x02(\x05\x12\x0c\n\x04nbrs\x18\x05 \x03(\x05\"\xa8\x01\n\x12NeighborDescriptor\x12\x0e\n\x06radius\x18\x01 \x02(\x01\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x10\n\x08\x64istance\x18\x03 \x03(\x01\x12\x10\n\x08thetaDeg\x18\x04 \x03(\x01\x12\x0e\n\x06phiDeg\x18\x05 \x03(\x01\x12\x0b\n\x03num\x18\x06 \x02(\x05\x12\x14\n\x0cSiteCenterUm\x18\x07 \x03(\x01\x12\x17\n\x0fSiteCenterTcsUm\x18\x08 \x03(\x01\"\xf3\x01\n\x10NeuronDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\x16\n\x0esiteNtvChanIdx\x18\x02 \x02(\x05\x12\x12\n\nspikeLabel\x18\x03 \x02(\t\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x12\n\nspikeCount\x18\x06 \x02(\x03\x12\x11\n\tspikeRate\x18\x07 \x02(\x01\x12\x16\n\x0emeanAbsPeakWfm\x18\x08 \x01(\x01\x12\x0b\n\x03snr\x18\t \x01(\x01\x12\x30\n\x08metaData\x18\n \x01(\x0b\x32\x1e.allego.NeuronExtendedMetadata\"\x86\x01\n\x16NeuronExtendedMetadata\x12\x18\n\x10neuronCatalogUID\x18\x01 \x01(\t\x12\x13\n\x0b\x65nsembleUID\x18\x02 \x01(\t\x12\x17\n\x0f\x66uncAssemblyUID\x18\x03 \x03(\t\x12\x12\n\ndatasetUID\x18\x04 \x01(\t\x12\x10\n\x08probeUID\x18\x05 \x01(\t\"\x8b\x01\n\x10NeuronStatistics\x12\x1a\n\x12WaveformAvgAbsAmpl\x18\x01 \x02(\x01\x12\x0b\n\x03Snr\x18\x02 \x02(\x01\x12\x12\n\nspikeCount\x18\x03 \x02(\x03\x12\x14\n\x0c\x61vgSpikeRate\x18\x04 \x02(\x01\x12$\n\x04isih\x18\x05 \x01(\x0b\x32\x16.allego.NeuronHistData\"|\n\x0fSpikeDescriptor\x12\x11\n\ttimestamp\x18\x01 \x02(\x03\x12\r\n\x05label\x18\x02 \x02(\t\x12\x10\n\x08waveform\x18\x03 \x03(\x02\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\x02\x12\x13\n\x0b\x64\x65\x63\x46\x65\x61tures\x18\x05 \x03(\x01\x12\x0e\n\x06zscore\x18\x06 \x03(\x02\"g\n\tSpikeData\x12&\n\x05spike\x18\x01 \x03(\x0b\x32\x17.allego.SpikeDescriptor\x12\x18\n\x10waveformMaxValue\x18\x02 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x03 \x02(\x02\"1\n\rSpikeTimeData\x12\x11\n\tspikeTime\x18\x01 \x03(\x01\x12\r\n\x05label\x18\x02 \x03(\x05\"Q\n\x12SpikeTimestampData\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x02 \x03(\x03\x12\x0e\n\x06labels\x18\x03 \x03(\x05\"\xb6\x02\n\x17SpikeTemplateDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\r\n\x05label\x18\x02 \x02(\t\x12\x11\n\tnumSpikes\x18\x03 \x02(\x03\x12\x10\n\x08waveform\x18\x04 \x02(\x0c\x12\x12\n\nwaveformSd\x18\x05 \x02(\x0c\x12\x13\n\x0blenWaveform\x18\x06 \x02(\x03\x12\x10\n\x08\x66\x65\x61tures\x18\x07 \x02(\x0c\x12\x12\n\nfeaturesSd\x18\x08 \x02(\x0c\x12\x13\n\x0blenFeatures\x18\t \x02(\x03\x12\x11\n\tfeatures2\x18\n \x02(\x0c\x12\x13\n\x0b\x66\x65\x61tures2Sd\x18\x0b \x02(\x0c\x12\x14\n\x0clenFeatures2\x18\x0c \x02(\x03\x12\x0e\n\x06zscore\x18\r \x02(\x0c\x12\x10\n\x08zscoreSd\x18\x0e \x02(\x0c\x12\x11\n\tlenZscore\x18\x0f \x02(\x03\"[\n\x12SiteSpikeTemplates\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x31\n\x08template\x18\x02 \x03(\x0b\x32\x1f.allego.SpikeTemplateDescriptor\"\x97\x01\n\x1f\x42iointerfaceSpikeTemplatesReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12(\n\x04site\x18\x05 \x03(\x0b\x32\x1a.allego.SiteSpikeTemplates\"@\n\x14\x42iointerfaceMetaData\x12(\n\x0bsignalGroup\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\"\xd6\x01\n\x1a\x42iointerfaceSpikeDataReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x03(\x03\x12\x12\n\nntvChanIdx\x18\x05 \x03(\x05\x12\x1f\n\x04site\x18\x06 \x03(\x0b\x32\x11.allego.SpikeData\x12.\n\x08metaData\x18\x07 \x01(\x0b\x32\x1c.allego.BiointerfaceMetaData\"y\n\x1fSpikeDataDenseChannelDescriptor\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0e\n\x06labels\x18\x02 \x03(\x05\x12\x18\n\x10waveformMaxValue\x18\x03 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x04 \x02(\x02\"\xb0\x01\n\x19SpikesSpikeDataDenseReply\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x17\n\x0fwaveformNPoints\x18\x02 \x02(\x05\x12\x14\n\x0ctotalNSpikes\x18\x03 \x02(\x05\x12\x43\n\x12\x63hannelDescriptors\x18\x04 \x03(\x0b\x32\'.allego.SpikeDataDenseChannelDescriptor\x12\x0c\n\x04\x64\x61ta\x18\x05 \x02(\x0c\"\x8a\x01\n\x17GroupSpikeTimeDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12#\n\x04site\x18\x05 \x03(\x0b\x32\x15.allego.SpikeTimeData\"v\n\x16\x42iointerfaceSpiketrain\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12$\n\x04site\x18\x04 \x03(\x0b\x32\x16.allego.SiteSpiketrain\"p\n\x0eSiteSpiketrain\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\"\n\x06neuron\x18\x02 \x03(\x0b\x32\x12.allego.Spiketrain\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12\x14\n\x0cnumNeighbors\x18\x04 \x02(\x05\"\x8b\x02\n\nSpiketrain\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12\r\n\x05label\x18\x02 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x03 \x03(\x03\x12\x14\n\x0cwaveformData\x18\x05 \x03(\x02\x12\x15\n\rwaveformShape\x18\x06 \x03(\x05\x12\x13\n\x0b\x66\x65\x61tureData\x18\x07 \x03(\x02\x12\x14\n\x0c\x66\x65\x61tureShape\x18\x08 \x03(\x05\x12\x12\n\nzscoreData\x18\t \x03(\x02\x12\x13\n\x0bzscoreShape\x18\n \x03(\x05\x12,\n\nneuronDesc\x18\x0f \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x14\n\x0cnumNeighbors\x18\x11 \x02(\x05\"\xb6\x01\n\x0eNeuronHistData\x12\x13\n\x0b\x62inWidthSec\x18\x01 \x02(\x01\x12\x15\n\rhistTimeRange\x18\x02 \x03(\x01\x12%\n\x04mode\x18\x03 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x14\n\x0cnumRefEvents\x18\x04 \x02(\x03\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\x12\x1a\n\x12numProcessedSpikes\x18\x06 \x02(\x03\x12\x0c\n\x04hist\x18\x07 \x03(\x01\"\x9d\x01\n\x0cSiteHistData\x12\x14\n\x0csitePosProbe\x18\x01 \x03(\x01\x12\x14\n\x0csitePosBrain\x18\x02 \x03(\x01\x12(\n\x06neuron\x18\x03 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12$\n\x04hist\x18\x04 \x03(\x0b\x32\x16.allego.NeuronHistData\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\"\x8b\x01\n\x19\x42iointerfaceHistDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12\"\n\x04site\x18\x05 \x03(\x0b\x32\x14.allego.SiteHistData\"\xb4\x01\n\x17\x42iointerfaceSaveRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x11\n\ttimeRange\x18\x04 \x03(\x01\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x1e\n\x16includeNeuronTemplates\x18\x06 \x02(\x08\"\xac\x01\n\x17\x42iointerfaceLoadRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x13\n\x0buidFragment\x18\x04 \x02(\t\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x14\n\x0c\x66orceReplace\x18\x06 \x02(\x08\"\x95\x01\n\x19\x42iointerfaceSaveLoadReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x0b\n\x03uid\x18\x04 \x02(\t\x12\x1c\n\x14\x62iointerfaceMetaFile\x18\x05 \x02(\t\x12\x1a\n\x12neuronTemplateFile\x18\x06 \x02(\t\"2\n\x17\x42iointerfaceGetIDsReply\x12\x17\n\x0f\x62iointerfaceIDs\x18\x01 \x03(\t\"\xef\x01\n\x16\x42iointerfaceVizRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x35\n\x07vizType\x18\x02 \x02(\x0e\x32$.allego.BiointerfaceVizRequest.VType\x12\x12\n\nnumSamples\x18\x03 \x02(\x05\x12\x14\n\x0cisYAutoScale\x18\x04 \x02(\x08\x12\x0c\n\x04yLim\x18\x05 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x06 \x01(\t\x12\x12\n\nisAutoOpen\x18\x07 \x01(\x08\"/\n\x05VType\x12\x15\n\x11VIZ_BIO_TEMPLATES\x10\x00\x12\x0f\n\x0bVIZ_BIO_DEV\x10\x01\"2\n\x14\x42iointerfaceVizReply\x12\x1a\n\x12pngPathAndFileName\x18\x01 \x01(\t*T\n\x10\x42iointerfaceType\x12\x13\n\x0f\x42IO_SPIKETRAINS\x10\x00\x12\x14\n\x10\x42IO_SPIKES_CACHE\x10\x01\x12\x15\n\x11\x42IO_SPIKES_STREAM\x10\x02* \n\x12SpikesImportSchema\x12\n\n\x06NI_SIM\x10\x00*@\n\x13\x42iointerfaceCommand\x12\x13\n\x0f\x42IO_CMD_SAVE_ON\x10\x00\x12\x14\n\x10\x42IO_CMD_SAVE_OFF\x10\x01*J\n\x11\x42iointerfaceState\x12\x0f\n\x0b\x42IO_SAVE_ON\x10\x00\x12\x10\n\x0c\x42IO_SAVE_OFF\x10\x01\x12\x12\n\x0e\x42IO_CONFIGURED\x10\x02*X\n\x11NeuronsSignalMode\x12\n\n\x06Spikes\x10\x00\x12\x13\n\x0fSpikeTimestamps\x10\x01\x12\x0e\n\nSpikeTimes\x10\x02\x12\x12\n\x0eSpikeWaveforms\x10\x03*q\n\x18SpikeDescriptorComponent\x12\x0e\n\nCTimestamp\x10\x00\x12\n\n\x06\x43Label\x10\x01\x12\r\n\tCWaveform\x10\x02\x12\x0c\n\x08\x43\x46\x65\x61ture\x10\x03\x12\x0f\n\x0b\x43\x44\x65\x63\x46\x65\x61ture\x10\x04\x12\x0b\n\x07\x43Zscore\x10\x05*S\n\x0fHistScalingMode\x12\x0c\n\x08\x41sSpikes\x10\x00\x12\x0f\n\x0b\x41sSpikeRate\x10\x01\x12\n\n\x06\x41sNorm\x10\x02\x12\n\n\x06\x41sProb\x10\x03\x12\t\n\x05\x41sRaw\x10\x04\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'biointerface_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._options = None
   _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_options = b'8\001'
-  _BIOINTERFACETYPE._serialized_start=7763
-  _BIOINTERFACETYPE._serialized_end=7847
-  _SPIKESIMPORTSCHEMA._serialized_start=7849
-  _SPIKESIMPORTSCHEMA._serialized_end=7881
-  _BIOINTERFACECOMMAND._serialized_start=7883
-  _BIOINTERFACECOMMAND._serialized_end=7947
-  _BIOINTERFACESTATE._serialized_start=7949
-  _BIOINTERFACESTATE._serialized_end=8023
-  _NEURONSSIGNALMODE._serialized_start=8025
-  _NEURONSSIGNALMODE._serialized_end=8113
-  _SPIKEDESCRIPTORCOMPONENT._serialized_start=8115
-  _SPIKEDESCRIPTORCOMPONENT._serialized_end=8228
-  _HISTSCALINGMODE._serialized_start=8230
-  _HISTSCALINGMODE._serialized_end=8313
+  _BIOINTERFACETYPE._serialized_start=7918
+  _BIOINTERFACETYPE._serialized_end=8002
+  _SPIKESIMPORTSCHEMA._serialized_start=8004
+  _SPIKESIMPORTSCHEMA._serialized_end=8036
+  _BIOINTERFACECOMMAND._serialized_start=8038
+  _BIOINTERFACECOMMAND._serialized_end=8102
+  _BIOINTERFACESTATE._serialized_start=8104
+  _BIOINTERFACESTATE._serialized_end=8178
+  _NEURONSSIGNALMODE._serialized_start=8180
+  _NEURONSSIGNALMODE._serialized_end=8268
+  _SPIKEDESCRIPTORCOMPONENT._serialized_start=8270
+  _SPIKEDESCRIPTORCOMPONENT._serialized_end=8383
+  _HISTSCALINGMODE._serialized_start=8385
+  _HISTSCALINGMODE._serialized_end=8468
   _SPIKESSTDREQ._serialized_start=44
   _SPIKESSTDREQ._serialized_end=77
   _SPIKESNEWLOADREPLY._serialized_start=79
   _SPIKESNEWLOADREPLY._serialized_end=99
   _SPIKESRENAMEREQ._serialized_start=101
   _SPIKESRENAMEREQ._serialized_end=161
   _SPIKESGETIDSREPLY._serialized_start=163
   _SPIKESGETIDSREPLY._serialized_end=182
   _SPIKESSPECREPLY._serialized_start=185
-  _SPIKESSPECREPLY._serialized_end=732
-  _SPIKESSITESPEC._serialized_start=735
-  _SPIKESSITESPEC._serialized_end=1316
-  _SPIKELABELRECORD._serialized_start=1318
-  _SPIKELABELRECORD._serialized_end=1351
-  _SPIKEMATRIX._serialized_start=1354
-  _SPIKEMATRIX._serialized_end=1636
-  _SPIKEMATRIXSET._serialized_start=1638
-  _SPIKEMATRIXSET._serialized_end=1763
-  _NEURONSPIKEMATRIXSET._serialized_start=1766
-  _NEURONSPIKEMATRIXSET._serialized_end=1913
-  _BIOINTERFACEGETSPIKESREQUEST._serialized_start=1916
-  _BIOINTERFACEGETSPIKESREQUEST._serialized_end=2211
-  _BIOINTERFACEGETHISTREQUEST._serialized_start=2214
-  _BIOINTERFACEGETHISTREQUEST._serialized_end=2367
-  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_start=2370
-  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_end=2514
-  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_start=2517
-  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_end=2656
-  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_start=2658
-  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_end=2741
-  _BIOINTERFACEGETNEURONSREQUEST._serialized_start=2743
-  _BIOINTERFACEGETNEURONSREQUEST._serialized_end=2832
-  _BIOINTERFACEGETNEURONSREPLY._serialized_start=2835
-  _BIOINTERFACEGETNEURONSREPLY._serialized_end=3191
-  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_start=2927
-  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_end=2981
-  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_start=2983
-  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_end=3101
-  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_start=3103
-  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_end=3191
-  _SPIKESSITESTATS._serialized_start=3194
-  _SPIKESSITESTATS._serialized_end=3457
-  _SPIKECOMPONENTLEN._serialized_start=3459
-  _SPIKECOMPONENTLEN._serialized_end=3561
-  _NEIGHBORDESCRIPTOR._serialized_start=3564
-  _NEIGHBORDESCRIPTOR._serialized_end=3732
-  _NEURONDESCRIPTOR._serialized_start=3735
-  _NEURONDESCRIPTOR._serialized_end=3978
-  _NEURONEXTENDEDMETADATA._serialized_start=3981
-  _NEURONEXTENDEDMETADATA._serialized_end=4115
-  _NEURONSTATISTICS._serialized_start=4118
-  _NEURONSTATISTICS._serialized_end=4257
-  _SPIKEDESCRIPTOR._serialized_start=4259
-  _SPIKEDESCRIPTOR._serialized_end=4383
-  _SPIKEDATA._serialized_start=4385
-  _SPIKEDATA._serialized_end=4488
-  _SPIKETIMEDATA._serialized_start=4490
-  _SPIKETIMEDATA._serialized_end=4539
-  _SPIKETIMESTAMPDATA._serialized_start=4541
-  _SPIKETIMESTAMPDATA._serialized_end=4622
-  _SPIKETEMPLATEDESCRIPTOR._serialized_start=4625
-  _SPIKETEMPLATEDESCRIPTOR._serialized_end=4935
-  _SITESPIKETEMPLATES._serialized_start=4937
-  _SITESPIKETEMPLATES._serialized_end=5028
-  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_start=5031
-  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_end=5182
-  _BIOINTERFACEMETADATA._serialized_start=5184
-  _BIOINTERFACEMETADATA._serialized_end=5248
-  _BIOINTERFACESPIKEDATAREPLY._serialized_start=5251
-  _BIOINTERFACESPIKEDATAREPLY._serialized_end=5465
-  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_start=5467
-  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_end=5588
-  _BIOINTERFACESPIKEDATADENSEREPLY._serialized_start=5591
-  _BIOINTERFACESPIKEDATADENSEREPLY._serialized_end=5773
-  _GROUPSPIKETIMEDATAREPLY._serialized_start=5776
-  _GROUPSPIKETIMEDATAREPLY._serialized_end=5914
-  _BIOINTERFACESPIKETRAIN._serialized_start=5916
-  _BIOINTERFACESPIKETRAIN._serialized_end=6034
-  _SITESPIKETRAIN._serialized_start=6036
-  _SITESPIKETRAIN._serialized_end=6148
-  _SPIKETRAIN._serialized_start=6151
-  _SPIKETRAIN._serialized_end=6418
-  _NEURONHISTDATA._serialized_start=6421
-  _NEURONHISTDATA._serialized_end=6603
-  _SITEHISTDATA._serialized_start=6606
-  _SITEHISTDATA._serialized_end=6763
-  _BIOINTERFACEHISTDATAREPLY._serialized_start=6766
-  _BIOINTERFACEHISTDATAREPLY._serialized_end=6905
-  _BIOINTERFACESAVEREQUEST._serialized_start=6908
-  _BIOINTERFACESAVEREQUEST._serialized_end=7088
-  _BIOINTERFACELOADREQUEST._serialized_start=7091
-  _BIOINTERFACELOADREQUEST._serialized_end=7263
-  _BIOINTERFACESAVELOADREPLY._serialized_start=7266
-  _BIOINTERFACESAVELOADREPLY._serialized_end=7415
-  _BIOINTERFACEGETIDSREPLY._serialized_start=7417
-  _BIOINTERFACEGETIDSREPLY._serialized_end=7467
-  _BIOINTERFACEVIZREQUEST._serialized_start=7470
-  _BIOINTERFACEVIZREQUEST._serialized_end=7709
-  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_start=7662
-  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_end=7709
-  _BIOINTERFACEVIZREPLY._serialized_start=7711
-  _BIOINTERFACEVIZREPLY._serialized_end=7761
+  _SPIKESSPECREPLY._serialized_end=832
+  _SPIKESSITESPEC._serialized_start=835
+  _SPIKESSITESPEC._serialized_end=1483
+  _SPIKELABELRECORD._serialized_start=1485
+  _SPIKELABELRECORD._serialized_end=1518
+  _SPIKEMATRIX._serialized_start=1521
+  _SPIKEMATRIX._serialized_end=1803
+  _SPIKEMATRIXSET._serialized_start=1805
+  _SPIKEMATRIXSET._serialized_end=1930
+  _NEURONSPIKEMATRIXSET._serialized_start=1933
+  _NEURONSPIKEMATRIXSET._serialized_end=2080
+  _SPIKESGETSPIKESREQUEST._serialized_start=2083
+  _SPIKESGETSPIKESREQUEST._serialized_end=2372
+  _BIOINTERFACEGETHISTREQUEST._serialized_start=2375
+  _BIOINTERFACEGETHISTREQUEST._serialized_end=2528
+  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_start=2531
+  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_end=2675
+  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_start=2678
+  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_end=2817
+  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_start=2819
+  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_end=2902
+  _BIOINTERFACEGETNEURONSREQUEST._serialized_start=2904
+  _BIOINTERFACEGETNEURONSREQUEST._serialized_end=2993
+  _BIOINTERFACEGETNEURONSREPLY._serialized_start=2996
+  _BIOINTERFACEGETNEURONSREPLY._serialized_end=3352
+  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_start=3088
+  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_end=3142
+  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_start=3144
+  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_end=3262
+  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_start=3264
+  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_end=3352
+  _SPIKESSITESTATS._serialized_start=3355
+  _SPIKESSITESTATS._serialized_end=3618
+  _SPIKECOMPONENTLEN._serialized_start=3620
+  _SPIKECOMPONENTLEN._serialized_end=3722
+  _NEIGHBORDESCRIPTOR._serialized_start=3725
+  _NEIGHBORDESCRIPTOR._serialized_end=3893
+  _NEURONDESCRIPTOR._serialized_start=3896
+  _NEURONDESCRIPTOR._serialized_end=4139
+  _NEURONEXTENDEDMETADATA._serialized_start=4142
+  _NEURONEXTENDEDMETADATA._serialized_end=4276
+  _NEURONSTATISTICS._serialized_start=4279
+  _NEURONSTATISTICS._serialized_end=4418
+  _SPIKEDESCRIPTOR._serialized_start=4420
+  _SPIKEDESCRIPTOR._serialized_end=4544
+  _SPIKEDATA._serialized_start=4546
+  _SPIKEDATA._serialized_end=4649
+  _SPIKETIMEDATA._serialized_start=4651
+  _SPIKETIMEDATA._serialized_end=4700
+  _SPIKETIMESTAMPDATA._serialized_start=4702
+  _SPIKETIMESTAMPDATA._serialized_end=4783
+  _SPIKETEMPLATEDESCRIPTOR._serialized_start=4786
+  _SPIKETEMPLATEDESCRIPTOR._serialized_end=5096
+  _SITESPIKETEMPLATES._serialized_start=5098
+  _SITESPIKETEMPLATES._serialized_end=5189
+  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_start=5192
+  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_end=5343
+  _BIOINTERFACEMETADATA._serialized_start=5345
+  _BIOINTERFACEMETADATA._serialized_end=5409
+  _BIOINTERFACESPIKEDATAREPLY._serialized_start=5412
+  _BIOINTERFACESPIKEDATAREPLY._serialized_end=5626
+  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_start=5628
+  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_end=5749
+  _SPIKESSPIKEDATADENSEREPLY._serialized_start=5752
+  _SPIKESSPIKEDATADENSEREPLY._serialized_end=5928
+  _GROUPSPIKETIMEDATAREPLY._serialized_start=5931
+  _GROUPSPIKETIMEDATAREPLY._serialized_end=6069
+  _BIOINTERFACESPIKETRAIN._serialized_start=6071
+  _BIOINTERFACESPIKETRAIN._serialized_end=6189
+  _SITESPIKETRAIN._serialized_start=6191
+  _SITESPIKETRAIN._serialized_end=6303
+  _SPIKETRAIN._serialized_start=6306
+  _SPIKETRAIN._serialized_end=6573
+  _NEURONHISTDATA._serialized_start=6576
+  _NEURONHISTDATA._serialized_end=6758
+  _SITEHISTDATA._serialized_start=6761
+  _SITEHISTDATA._serialized_end=6918
+  _BIOINTERFACEHISTDATAREPLY._serialized_start=6921
+  _BIOINTERFACEHISTDATAREPLY._serialized_end=7060
+  _BIOINTERFACESAVEREQUEST._serialized_start=7063
+  _BIOINTERFACESAVEREQUEST._serialized_end=7243
+  _BIOINTERFACELOADREQUEST._serialized_start=7246
+  _BIOINTERFACELOADREQUEST._serialized_end=7418
+  _BIOINTERFACESAVELOADREPLY._serialized_start=7421
+  _BIOINTERFACESAVELOADREPLY._serialized_end=7570
+  _BIOINTERFACEGETIDSREPLY._serialized_start=7572
+  _BIOINTERFACEGETIDSREPLY._serialized_end=7622
+  _BIOINTERFACEVIZREQUEST._serialized_start=7625
+  _BIOINTERFACEVIZREQUEST._serialized_end=7864
+  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_start=7817
+  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_end=7864
+  _BIOINTERFACEVIZREPLY._serialized_start=7866
+  _BIOINTERFACEVIZREPLY._serialized_end=7916
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/common_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/common_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,466 +7,513 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\"9\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\"\x11\n\x0fStandardRequest\"\x1f\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"\xc6\x02\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xe0\x01\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\ntimeWindow\x18\x02 \x02(\x01\x12\x0f\n\x07spacing\x18\x03 \x02(\x01\x12\x11\n\tmagnitude\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x14\n\x0c\x61uxMagnitude\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\"<\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"S\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\xf9\x05\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\xc2\x02\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x01(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x01(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\x92\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"k\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x02(\t\x12\x13\n\x0bheadstageId\x18\x04 \x02(\t\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"}\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"W\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x94\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12)\n\nbundleName\x18\x04 \x01(\x0e\x32\x15.allego.KpiBundleName\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"\x88\x01\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\x12#\n\x04name\x18\x04 \x01(\x0e\x32\x15.allego.KpiBundleName\"\x90\x01\n\x19SetKpiUpdatePeriodRequest\x12!\n\x05stype\x18\x01 \x02(\x0e\x32\x12.allego.SignalType\x12\x15\n\rstreamGroupId\x18\x02 \x01(\t\x12\x14\n\x0cupdatePeriod\x18\x03 \x02(\x01\x12#\n\x04name\x18\x04 \x01(\x0e\x32\x15.allego.KpiBundleName\"\xd2\x02\n\x16SetKpiThresholdRequest\x12!\n\x05stype\x18\x01 \x02(\x0e\x32\x12.allego.SignalType\x12\x15\n\rstreamGroupId\x18\x02 \x01(\t\x12\x13\n\x0bisUpdatePos\x18\x03 \x02(\x08\x12\x12\n\nisClearPos\x18\x04 \x02(\x08\x12\x0f\n\x07isSdPos\x18\x05 \x02(\x08\x12\x10\n\x08levelPos\x18\x06 \x02(\x01\x12\x13\n\x0bisUpdateNeg\x18\x07 \x02(\x08\x12\x12\n\nisClearNeg\x18\x08 \x02(\x08\x12\x0f\n\x07isSdNeg\x18\t \x02(\x08\x12\x10\n\x08levelNeg\x18\n \x02(\x01\x12\x16\n\nntvChanIdx\x18\x0b \x03(\x05\x42\x02\x10\x01\x12)\n\x07thrName\x18\x0c \x01(\x0e\x32\x18.allego.KpiThresholdName\x12#\n\x04name\x18\r \x01(\x0e\x32\x15.allego.KpiBundleName\"\xd2\x01\n\x18SetKpiEventDetectRequest\x12!\n\x05stype\x18\x01 \x02(\x0e\x32\x12.allego.SignalType\x12\x15\n\rstreamGroupId\x18\x02 \x01(\t\x12\x15\n\risEventDetect\x18\x03 \x02(\x08\x12\x16\n\nntvChanIdx\x18\x04 \x03(\x05\x42\x02\x10\x01\x12)\n\x07thrName\x18\x05 \x01(\x0e\x32\x18.allego.KpiThresholdName\x12\x10\n\x08isPosThr\x18\x06 \x01(\x08\x12\x10\n\x08isNegThr\x18\x07 \x01(\x08\"\xa5\x01\n\x18SetKpiEventShadowRequest\x12!\n\x05stype\x18\x01 \x02(\x0e\x32\x12.allego.SignalType\x12\x15\n\rstreamGroupId\x18\x02 \x01(\t\x12\x0e\n\x06shadow\x18\x03 \x02(\x01\x12\x16\n\nntvChanIdx\x18\x04 \x03(\x05\x42\x02\x10\x01\x12\'\n\x07wdwName\x18\x05 \x01(\x0e\x32\x16.allego.KpiWindowdName\"\xb6\x01\n\x18SetKpiEventWindowRequest\x12!\n\x05stype\x18\x01 \x02(\x0e\x32\x12.allego.SignalType\x12\x15\n\rstreamGroupId\x18\x02 \x01(\t\x12\x0e\n\x06preThr\x18\x03 \x02(\x01\x12\x0f\n\x07postThr\x18\x04 \x02(\x01\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12\'\n\x07wdwName\x18\x06 \x01(\x0e\x32\x16.allego.KpiWindowdName\"Q\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12#\n\x04name\x18\x03 \x01(\x0e\x32\x15.allego.KpiBundleName\"\xa3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x03(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x02(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x02(\t\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"3\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\xd9\x05\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"O\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"V\n\x0eWrangleRequest\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.WrangleMode\x12!\n\x04spec\x18\x02 \x02(\x0b\x32\x13.allego.WrangleSpec\"Y\n\x0bWrangleSpec\x12%\n\x06import\x18\x01 \x03(\x0b\x32\x15.allego.WrangleImport\x12#\n\x05merge\x18\x02 \x03(\x0b\x32\x14.allego.WrangleMerge\"H\n\rWrangleImport\x12\x37\n\x0cvexSpikesSim\x18\x01 \x01(\x0b\x32!.allego.WrangleImportVexSpikesSim\"g\n\x19WrangleImportVexSpikesSim\x12\'\n\x06source\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x13\n\x0bisOverwrite\x18\x02 \x01(\x08\x12\x0c\n\x04note\x18\x03 \x01(\t\"C\n\x0fWrangleFileDesc\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12\x10\n\x08\x66ileType\x18\x03 \x01(\t\"H\n\x0cWrangleMerge\x12\x38\n\rvexSpikesView\x18\x01 \x01(\x0b\x32!.allego.WrangleMergeVexSpikesView\"\xaf\x02\n\x19WrangleMergeVexSpikesView\x12*\n\tsourceVex\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12*\n\tsourceBio\x18\x02 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x33\n\x04view\x18\x03 \x03(\x0b\x32%.allego.WrangleMergeVexSpikesViewSpec\x12\x0c\n\x04note\x18\x04 \x01(\t\x12\x18\n\x10isBandpassFilter\x18\x05 \x01(\x08\x12\x1a\n\x12\x62\x61ndpassFilterSpec\x18\x06 \x03(\x01\x12\x13\n\x0bisOverwrite\x18\x07 \x01(\x08\x12\x15\n\rspikeWindowMs\x18\x08 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\t \x01(\x01\"\xc0\x01\n\x1dWrangleMergeVexSpikesViewSpec\x12(\n\x07sinkBio\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x1c\n\x14siteNeighborRadiusUm\x18\x02 \x01(\x01\x12\x1b\n\x13reqNumSiteNeighbors\x18\x03 \x01(\x05\x12\x15\n\rspikeWindowMs\x18\x04 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\x05 \x01(\x01\x12\x0c\n\x04note\x18\x06 \x01(\t\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields*\x85\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*+\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\x96\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xfd\x05\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*\x97\x01\n\rKpiBundleName\x12\t\n\x05Kpi_A\x10\x00\x12\t\n\x05Kpi_B\x10\x01\x12\t\n\x05Kpi_C\x10\x02\x12\t\n\x05Kpi_D\x10\x03\x12\x0c\n\x08Kpi_Aux0\x10\x04\x12\x0c\n\x08Kpi_Aux1\x10\x05\x12\x12\n\x0eKpi_Datasource\x10\x06\x12\t\n\x05Kpi_E\x10\x07\x12\t\n\x05Kpi_F\x10\x08\x12\t\n\x05Kpi_G\x10\t\x12\t\n\x05Kpi_H\x10\n*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*B\n\x10KpiThresholdName\x12\x11\n\rKpi_Thr_Event\x10\x00\x12\x1b\n\x17Kpi_Thr_Artifact_Reject\x10\x01*@\n\x0eKpiWindowdName\x12\x11\n\rKpi_Wdw_Event\x10\x00\x12\x1b\n\x17Kpi_Wdw_Artifact_Reject\x10\x01*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\xf0\x01\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*Z\n\x0bWrangleMode\x12*\n&WRANGLE_MODE_IMPORT_NNX_VEX_SPIKES_SIM\x10\x00\x12\x1f\n\x1bWRANGLE_MODE_MERGE_FIT_VIEW\x10\x01*\xd7\x03\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x16\n\x12GPIO_CHANNEL_COUNT\x10\x05\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\x1a\x1fgoogle/protobuf/timestamp.proto\"9\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\"!\n\x0fStandardRequest\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"/\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\x96\x01\n\x12HDSnapshotRequest2\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x01(\x0e\x32\x18.allego.TimeRangeSelMode\x12#\n\x06sigSel\x18\x04 \x01(\x0b\x32\x13.allego.SigSelector\"L\n\x15RadiensPyGraphicsArgs\x12\x12\n\ngraphicsID\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0f\n\x07\x66igSize\x18\x03 \x03(\x03\"\xdd\x02\n\nPSDRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x02(\x0e\x32\x18.allego.TimeRangeSelMode\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\x12\x12\n\nresampleFs\x18\x06 \x01(\x01\x12&\n\x07wdwType\x18\x07 \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\x08 \x01(\x0e\x32\x12.allego.PSDScaling\x12\x11\n\tfreqRange\x18\t \x03(\x01\x12\x14\n\x0c\x63ollapseFreq\x18\n \x01(\x08\x12\x11\n\tdeltaFreq\x18\x0b \x01(\x01\x12\x0c\n\x04path\x18\r \x01(\t\x12\x13\n\x0bisReturnPSD\x18\x0e \x01(\x08\"\xa1\x02\n\x03PSD\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x1d\n\x02tR\x18\x05 \x02(\x0b\x32\x11.allego.TimeRange\x12 \n\x03psd\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x0c\n\x04\x66req\x18\x07 \x03(\x01\x12\x14\n\x0c\x66reqBinWidth\x18\x08 \x02(\x01\x12\x11\n\tfreqRange\x18\x0b \x03(\x01\x12&\n\x07wdwType\x18\t \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\n \x01(\x0e\x32\x12.allego.PSDScaling\"e\n\x18RadiensPyGraphicsRequest\x12\x1c\n\x07psdData\x18\x01 \x01(\x0b\x32\x0b.allego.PSD\x12+\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x1d.allego.RadiensPyGraphicsArgs\"^\n\x0bSigSelector\x12\x12\n\nampNtvIdxs\x18\x01 \x03(\x03\x12\x12\n\nainNtvIdxs\x18\x02 \x03(\x03\x12\x12\n\ndinNtvIdxs\x18\x03 \x03(\x03\x12\x13\n\x0b\x64outNtvIdxs\x18\x04 \x03(\x03\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"@\n\x0bHDSnapshot2\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1e\n\x04sigs\x18\x02 \x02(\x0b\x32\x10.allego.Signals2\"\xc6\x02\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xe0\x01\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\ntimeWindow\x18\x02 \x02(\x01\x12\x0f\n\x07spacing\x18\x03 \x02(\x01\x12\x11\n\tmagnitude\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x14\n\x0c\x61uxMagnitude\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\"[\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\x12\x1d\n\x02tR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\"\xe7\x01\n\x08Signals2\x12\x1f\n\x02sG\x18\x01 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12%\n\x03\x61mp\x18\x03 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x61in\x18\x04 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x64in\x18\x05 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12&\n\x04\x64out\x18\x06 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"d\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\x12\x0f\n\x07\x64irList\x18\x03 \x03(\t\"\x1c\n\x07SortMap\x12\x11\n\tsorterIds\x18\x01 \x03(\t\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xa0\x01\n\x13GetSorterIDMapReply\x12\x43\n\x0csigToSortMap\x18\x01 \x03(\x0b\x32-.allego.GetSorterIDMapReply.SigToSortMapEntry\x1a\x44\n\x11SigToSortMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.allego.SortMap:\x02\x38\x01\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\xf9\x05\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\xee\x02\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\n \x01(\x05\x12\x10\n\x08numSites\x18\x0b \x02(\x05\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x03(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\xa5\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\x12\x11\n\tpropagate\x18\x07 \x01(\x08\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"T\n\x14SliceSignalGroupSpec\x12\x0e\n\x06sortBy\x18\x01 \x02(\t\x12\r\n\x05\x64\x65lim\x18\x02 \x02(\t\x12\x1d\n\x02tR\x18\x03 \x01(\x0b\x32\x11.allego.TimeRange\"X\n\x17SliceSignalGroupRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\"\x88\x01\n\x15SliceSignalGroupReply\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07outcome\x18\x04 \x02(\t\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\x85\x01\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x01(\t\x12\x13\n\x0bheadstageId\x18\x04 \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"\x90\x01\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorIdx\x18\x04 \x01(\x05\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"\x85\x01\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\x12,\n\x08wallTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x9d\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12\x0e\n\x06isPlot\x18\x04 \x01(\x08\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x14\n\x0cisReturnData\x18\x06 \x01(\x08\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"c\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\":\n\x12SetKpiParamRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\x01\",\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"\'\n\x12KpiStandardRequest\x12\x11\n\tdsourceID\x18\x02 \x03(\t\"\xba\x01\n\rKpiFileStatus\x12,\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1b.allego.KpiFileStatus.State\x1a{\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x12\n\ndsourceUID\x18\x03 \x01(\t\x12 \n\x05kpiTR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x05 \x01(\t\"\xc7\x04\n\x0eKpiFileStatus2\x12>\n\x07\x64source\x18\x01 \x03(\x0b\x32-.allego.KpiFileStatus2.KpiDatasourceStateSpec\x1a\xe9\x01\n\tKPI_State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x17\n\x0f\x66ilePathAndName\x18\x04 \x01(\t\x12 \n\x05kpiTR\x18\x05 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0cpacketDurSec\x18\x06 \x01(\x01\x12\x0e\n\x06numAmp\x18\x07 \x01(\x03\x12\x18\n\x10\x62ytesInBundlePkt\x18\x08 \x01(\x03\x12\x12\n\nnumPackets\x18\t \x01(\x03\x12\x12\n\ndatasetUID\x18\n \x01(\t\x1aq\n\x10\x44\x61tasource_State\x12\x17\n\x0f\x66ilePathAndName\x18\x01 \x01(\t\x12\x1d\n\x02TR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x11\n\tdsourceID\x18\x04 \x01(\t\x1a\x95\x01\n\x16KpiDatasourceStateSpec\x12\x37\n\x06source\x18\x01 \x02(\x0b\x32\'.allego.KpiFileStatus2.Datasource_State\x12-\n\x03kpi\x18\x02 \x02(\x0b\x32 .allego.KpiFileStatus2.KPI_State\x12\x13\n\x0bisSprinting\x18\x03 \x02(\x08\"\xfd\x01\n\x0fKpiFileMetadata\x12.\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1d.allego.KpiFileMetadata.State\x1a\xb9\x01\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\ndsourceUID\x18\x02 \x01(\t\x12\x11\n\tpacketDur\x18\x03 \x01(\x01\x12\x0c\n\x04nAMP\x18\x04 \x01(\x03\x12\x1b\n\x13\x62ytesInBundlePacket\x18\x05 \x01(\x03\x12\x12\n\nnumPackets\x18\x06 \x01(\x03\x12 \n\x05kpiTR\x18\x07 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x08 \x01(\t\"\xd3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x01(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x01(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x01(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x01(\t\x12\x1d\n\x02tR\x18\x10 \x01(\x0b\x32\x11.allego.TimeRange\x12\x0f\n\x07numSigs\x18\x11 \x01(\x03\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"/\n\x10RadixMatrixBytes\x12\x0c\n\x04\x64\x61ta\x18\x01 \x02(\x0c\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"3\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\xd9\x05\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"{\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x14\n\x0cincrementSec\x18\x04 \x01(\x01\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"?\n\tKpiParams\x12\x32\n\x03rec\x18\x01 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"W\n\x0eWrangleRequest\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.WrangleMode\x12\"\n\x04spec\x18\x02 \x02(\x0b\x32\x14.allego.WrangleMerge\"Y\n\x0bWrangleSpec\x12%\n\x06import\x18\x01 \x03(\x0b\x32\x15.allego.WrangleImport\x12#\n\x05merge\x18\x02 \x03(\x0b\x32\x14.allego.WrangleMerge\"H\n\rWrangleImport\x12\x37\n\x0cvexSpikesSim\x18\x01 \x01(\x0b\x32!.allego.WrangleImportVexSpikesSim\"g\n\x19WrangleImportVexSpikesSim\x12\'\n\x06source\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x13\n\x0bisOverwrite\x18\x02 \x01(\x08\x12\x0c\n\x04note\x18\x03 \x01(\t\"C\n\x0fWrangleFileDesc\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12\x10\n\x08\x66ileType\x18\x03 \x01(\t\"H\n\x0cWrangleMerge\x12\x38\n\rvexSpikesView\x18\x01 \x01(\x0b\x32!.allego.WrangleMergeVexSpikesView\"\xaf\x02\n\x19WrangleMergeVexSpikesView\x12*\n\tsourceVex\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12*\n\tsourceBio\x18\x02 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x33\n\x04view\x18\x03 \x03(\x0b\x32%.allego.WrangleMergeVexSpikesViewSpec\x12\x0c\n\x04note\x18\x04 \x01(\t\x12\x18\n\x10isBandpassFilter\x18\x05 \x01(\x08\x12\x1a\n\x12\x62\x61ndpassFilterSpec\x18\x06 \x03(\x01\x12\x13\n\x0bisOverwrite\x18\x07 \x01(\x08\x12\x15\n\rspikeWindowMs\x18\x08 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\t \x01(\x01\"\xc0\x01\n\x1dWrangleMergeVexSpikesViewSpec\x12(\n\x07sinkBio\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x1c\n\x14siteNeighborRadiusUm\x18\x02 \x01(\x01\x12\x1b\n\x13reqNumSiteNeighbors\x18\x03 \x01(\x05\x12\x15\n\rspikeWindowMs\x18\x04 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\x05 \x01(\x01\x12\x0c\n\x04note\x18\x06 \x01(\t\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields\"\xa5\x01\n\x17\x44\x61shboardCommandRequest\x12\'\n\x08\x64\x61shType\x18\x01 \x01(\x0e\x32\x15.allego.DashboardType\x12\x32\n\x04\x61rgs\x18\x02 \x01(\x0b\x32$.allego.DashboardCommandRequest.Args\x1a-\n\x04\x41rgs\x12%\n\x03\x63md\x18\x01 \x02(\x0e\x32\x18.allego.DashboardCommand\"]\n\x13SelTableSignalGroup\x12\r\n\x05index\x18\x01 \x02(\t\x12\x15\n\rcriterionDesc\x18\x02 \x02(\t\x12\x0f\n\x07ntvIdxs\x18\x03 \x03(\x03\x12\x0f\n\x07numSigs\x18\x04 \x02(\x03\"?\n\x13SelectorTablesReply\x12(\n\x03sig\x18\x01 \x03(\x0b\x32\x1b.allego.SelTableSignalGroup*\x85\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*+\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\xae\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06\x12\x16\n\x12RADIENS_DASHBOARDS\x10\x07*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*C\n\rPSDWindowType\x12\x0f\n\x0bHAMMING_p01\x10\x00\x12\x0f\n\x0bHAMMING_p05\x10\x01\x12\x10\n\x0cPASS_THROUGH\x10\x02*/\n\nPSDScaling\x12\x10\n\x0cPSD_SPECTRUM\x10\x00\x12\x0f\n\x0bPSD_DENSITY\x10\x01*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xa1\x06\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#\x12\"\n\x1eKPI_MAX_MIN_DIFF_ABS_AMPLIFIED\x10$*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\xf0\x01\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*\x83\x01\n\x0bWrangleMode\x12*\n&WRANGLE_MODE_IMPORT_NNX_VEX_SPIKES_SIM\x10\x00\x12\x1f\n\x1bWRANGLE_MODE_MERGE_FIT_VIEW\x10\x01\x12\'\n#WRANGLE_MODE_IMPORT_KILOSORT_SPIKES\x10\x02*\x86\x04\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x16\n\x12GPIO_CHANNEL_COUNT\x10\x05\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x12\x19\n\x15SPIKE_SORTER_WARNINGS\x10\x18\x12\x12\n\x0eSTIM_STEP_SIZE\x10\x19*\x1b\n\rDashboardType\x12\n\n\x06\x44\x41SH_1\x10\x00*N\n\x10\x44\x61shboardCommand\x12\x11\n\rDASH_CMD_OPEN\x10\x00\x12\x12\n\x0e\x44\x41SH_CMD_CLOSE\x10\x01\x12\x13\n\x0f\x44\x41SH_CMD_UPDATE\x10\x02\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._options = None
   _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._serialized_options = b'8\001'
   _SERVERSPEC_SERVICEENTRY._options = None
   _SERVERSPEC_SERVICEENTRY._serialized_options = b'8\001'
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._options = None
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_options = b'8\001'
   _SIGNALGROUPUNITS_UNITSENTRY._options = None
   _SIGNALGROUPUNITS_UNITSENTRY._serialized_options = b'8\001'
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._options = None
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _SETKPITHRESHOLDREQUEST.fields_by_name['ntvChanIdx']._options = None
-  _SETKPITHRESHOLDREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _SETKPIEVENTDETECTREQUEST.fields_by_name['ntvChanIdx']._options = None
-  _SETKPIEVENTDETECTREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _SETKPIEVENTSHADOWREQUEST.fields_by_name['ntvChanIdx']._options = None
-  _SETKPIEVENTSHADOWREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _SETKPIEVENTWINDOWREQUEST.fields_by_name['ntvChanIdx']._options = None
-  _SETKPIEVENTWINDOWREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _RADIXFILETYPES._serialized_start=21688
-  _RADIXFILETYPES._serialized_end=21949
-  _SIGNALTYPE._serialized_start=21951
-  _SIGNALTYPE._serialized_end=22000
-  _RESAMPLEROUTINE._serialized_start=22002
-  _RESAMPLEROUTINE._serialized_end=22045
-  _PORT._serialized_start=22047
-  _PORT._serialized_end=22109
-  _WORKSPACEAPP._serialized_start=22111
-  _WORKSPACEAPP._serialized_end=22161
-  _WORKSPACECOMMANDS._serialized_start=22164
-  _WORKSPACECOMMANDS._serialized_end=22324
-  _GETWORKSPACECOMMANDS._serialized_start=22326
-  _GETWORKSPACECOMMANDS._serialized_end=22393
-  _RADIENSSERVERTYPE._serialized_start=22395
-  _RADIENSSERVERTYPE._serialized_end=22451
-  _GRPCSERVICETYPE._serialized_start=22454
-  _GRPCSERVICETYPE._serialized_end=22604
-  _DEVDATASETTYPE._serialized_start=22606
-  _DEVDATASETTYPE._serialized_end=22669
-  _DATASOURCESORT._serialized_start=22671
-  _DATASOURCESORT._serialized_end=22759
-  _SIGNALGROUPTYPE._serialized_start=22761
-  _SIGNALGROUPTYPE._serialized_end=22807
-  _DSPTYPE._serialized_start=22810
-  _DSPTYPE._serialized_end=22939
-  _FILTERSTAGE._serialized_start=22941
-  _FILTERSTAGE._serialized_end=22998
-  _FEATURELICENSE._serialized_start=23001
-  _FEATURELICENSE._serialized_end=23340
-  _KPIMETRICSMODE._serialized_start=23342
-  _KPIMETRICSMODE._serialized_end=23437
-  _KPIMETRICSENUM._serialized_start=23440
-  _KPIMETRICSENUM._serialized_end=24205
-  _KPIMETRICSSTATSENUM._serialized_start=24208
-  _KPIMETRICSSTATSENUM._serialized_end=24347
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=24350
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=24670
-  _KPIBUNDLENAME._serialized_start=24673
-  _KPIBUNDLENAME._serialized_end=24824
-  _TIMERANGESELMODE._serialized_start=24826
-  _TIMERANGESELMODE._serialized_end=24896
-  _KPITHRESHOLDNAME._serialized_start=24898
-  _KPITHRESHOLDNAME._serialized_end=24964
-  _KPIWINDOWDNAME._serialized_start=24966
-  _KPIWINDOWDNAME._serialized_end=25030
-  _OUTFITTERCOMPONENTTYPE._serialized_start=25032
-  _OUTFITTERCOMPONENTTYPE._serialized_end=25110
-  _WORLDNODELABEL._serialized_start=25112
-  _WORLDNODELABEL._serialized_end=25237
-  _WORLDEDGELABEL._serialized_start=25239
-  _WORLDEDGELABEL._serialized_end=25278
-  _WORLDEDGEDIRECTION._serialized_start=25280
-  _WORLDEDGEDIRECTION._serialized_end=25376
-  _USERROLETYPE._serialized_start=25379
-  _USERROLETYPE._serialized_end=25538
-  _MANAGENODECMD._serialized_start=25540
-  _MANAGENODECMD._serialized_end=25611
-  _WORLDQUERYCMD._serialized_start=25614
-  _WORLDQUERYCMD._serialized_end=25846
-  _TRANSFORMNODETYPE._serialized_start=25849
-  _TRANSFORMNODETYPE._serialized_end=26089
-  _SPIKESORTERPARAMCOMMAND._serialized_start=26092
-  _SPIKESORTERPARAMCOMMAND._serialized_end=26315
-  _WRANGLEMODE._serialized_start=26317
-  _WRANGLEMODE._serialized_end=26407
-  _STATUSPOLLFIELDS._serialized_start=26410
-  _STATUSPOLLFIELDS._serialized_end=26881
-  _RADIXENVIRONMENT._serialized_start=24
-  _RADIXENVIRONMENT._serialized_end=81
-  _STANDARDREQUEST._serialized_start=83
-  _STANDARDREQUEST._serialized_end=100
-  _STANDARDREPLY._serialized_start=102
-  _STANDARDREPLY._serialized_end=133
-  _DACOFFREQUEST._serialized_start=135
-  _DACOFFREQUEST._serialized_end=173
-  _WORKSPACEDESCRIPTOR._serialized_start=176
-  _WORKSPACEDESCRIPTOR._serialized_end=362
-  _WORKSPACECONTROLREQUEST._serialized_start=365
-  _WORKSPACECONTROLREQUEST._serialized_end=549
-  _GETWORKSPACEREQUEST._serialized_start=552
-  _GETWORKSPACEREQUEST._serialized_end=763
-  _GETWORKSPACEREPLY._serialized_start=766
-  _GETWORKSPACEREPLY._serialized_end=937
-  _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._serialized_start=856
-  _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._serialized_end=937
-  _GETRADIENSSERVERSREQUEST._serialized_start=939
-  _GETRADIENSSERVERSREQUEST._serialized_end=1035
-  _SERVERSPEC._serialized_start=1038
-  _SERVERSPEC._serialized_end=1317
-  _SERVERSPEC_GRPCSERVICE._serialized_start=1179
-  _SERVERSPEC_GRPCSERVICE._serialized_end=1206
-  _SERVERSPEC_SPAWNEDPROCESS._serialized_start=1208
-  _SERVERSPEC_SPAWNEDPROCESS._serialized_end=1237
-  _SERVERSPEC_SERVICEENTRY._serialized_start=1239
-  _SERVERSPEC_SERVICEENTRY._serialized_end=1317
-  _RADIENSSERVERSREPLY._serialized_start=1319
-  _RADIENSSERVERSREPLY._serialized_end=1425
-  _SIGNALGROUPIDREQUEST._serialized_start=1427
-  _SIGNALGROUPIDREQUEST._serialized_end=1472
-  _SIGNALMAP._serialized_start=1475
-  _SIGNALMAP._serialized_end=1671
-  _GPIOCHANNELCOUNT._serialized_start=1673
-  _GPIOCHANNELCOUNT._serialized_end=1734
-  _PORTCHANNELCOUNT._serialized_start=1736
-  _PORTCHANNELCOUNT._serialized_end=1804
-  _SETPORTREQUEST._serialized_start=1806
-  _SETPORTREQUEST._serialized_end=1887
-  _HDSNAPSHOTREQUEST._serialized_start=1890
-  _HDSNAPSHOTREQUEST._serialized_end=2244
-  _HDSNAPSHOTREQUEST_SELECTEDSIGNALS._serialized_start=2206
-  _HDSNAPSHOTREQUEST_SELECTEDSIGNALS._serialized_end=2244
-  _HDSNAPSHOTMETA._serialized_start=2246
-  _HDSNAPSHOTMETA._serialized_end=2339
-  _HDSNAPSHOT._serialized_start=2342
-  _HDSNAPSHOT._serialized_end=2629
-  _GETSIGNALSREQUEST._serialized_start=2632
-  _GETSIGNALSREQUEST._serialized_end=2958
-  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_start=2734
-  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_end=2958
-  _RAWSIGNALS._serialized_start=2960
-  _RAWSIGNALS._serialized_end=3020
-  _LISTSENSORSPECSREPLY._serialized_start=3023
-  _LISTSENSORSPECSREPLY._serialized_end=3284
-  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_start=3226
-  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_end=3284
-  _LISTDATASOURCESREQUEST._serialized_start=3286
-  _LISTDATASOURCESREQUEST._serialized_end=3369
-  _GETSIGNALGROUPIDSREPLY._serialized_start=3371
-  _GETSIGNALGROUPIDSREPLY._serialized_end=3433
-  _DATASOURCE._serialized_start=3436
-  _DATASOURCE._serialized_end=3611
-  _FILEDESCRIPTOR._serialized_start=3613
-  _FILEDESCRIPTOR._serialized_end=3724
-  _TIMESPEC._serialized_start=3727
-  _TIMESPEC._serialized_end=3935
-  _TIMESPEC_TIMERANGEL._serialized_start=3849
-  _TIMESPEC_TIMERANGEL._serialized_end=3880
-  _TIMESPEC_TIMESTAMPRANGEL._serialized_start=3882
-  _TIMESPEC_TIMESTAMPRANGEL._serialized_end=3923
-  _SIGNALSPEC._serialized_start=3938
-  _SIGNALSPEC._serialized_end=4128
-  _SIGNALSPEC_SITENUML._serialized_start=4054
-  _SIGNALSPEC_SITENUML._serialized_end=4081
-  _SIGNALSPEC_NTVCHANIDXL._serialized_start=4083
-  _SIGNALSPEC_NTVCHANIDXL._serialized_end=4116
-  _CHANNELRECORD._serialized_start=4131
-  _CHANNELRECORD._serialized_end=4892
-  _XYCOORD._serialized_start=4894
-  _XYCOORD._serialized_end=4925
-  _XYZCOORD._serialized_start=4927
-  _XYZCOORD._serialized_end=4970
-  _SENSOR._serialized_start=4973
-  _SENSOR._serialized_end=5295
-  _SENSOR_WIREFRAME._serialized_start=5186
-  _SENSOR_WIREFRAME._serialized_end=5295
-  _SENSORPORTSPEC._serialized_start=5298
-  _SENSORPORTSPEC._serialized_end=5578
-  _SIGNALGROUPUNITS._serialized_start=5580
-  _SIGNALGROUPUNITS._serialized_end=5696
-  _SIGNALGROUPUNITS_UNITSENTRY._serialized_start=5652
-  _SIGNALGROUPUNITS_UNITSENTRY._serialized_end=5696
-  _SIGNALGROUP._serialized_start=5699
-  _SIGNALGROUP._serialized_end=5955
-  _CREATESIGNALGROUPREQUEST._serialized_start=5958
-  _CREATESIGNALGROUPREQUEST._serialized_end=6093
-  _SUBOPSORT._serialized_start=6095
-  _SUBOPSORT._serialized_end=6210
-  _SUBOPSORT_SORTFIELD._serialized_start=6151
-  _SUBOPSORT_SORTFIELD._serialized_end=6210
-  _UPDATESIGNALGROUPREQUEST._serialized_start=6213
-  _UPDATESIGNALGROUPREQUEST._serialized_end=6615
-  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_start=6496
-  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_end=6562
-  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_start=6564
-  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_end=6599
-  _LICENSESTATUS._serialized_start=6617
-  _LICENSESTATUS._serialized_end=6632
-  _SETDSPGROUPREQUEST._serialized_start=6634
-  _SETDSPGROUPREQUEST._serialized_end=6751
-  _DSPPARAMS._serialized_start=6754
-  _DSPPARAMS._serialized_end=7124
-  _DSPPARAMS_FREQSPECBAND._serialized_start=7063
-  _DSPPARAMS_FREQSPECBAND._serialized_end=7112
-  _DSPGROUP._serialized_start=7127
-  _DSPGROUP._serialized_end=7260
-  _SETSENSORREQUEST._serialized_start=7262
-  _SETSENSORREQUEST._serialized_end=7369
-  _SENSORPOSITIONTCS._serialized_start=7371
-  _SENSORPOSITIONTCS._serialized_end=7480
-  _SETSENSORPOSITIONTCSREQUEST._serialized_start=7482
-  _SETSENSORPOSITIONTCSREQUEST._serialized_end=7607
-  _SITEPOSITIONTCS._serialized_start=7609
-  _SITEPOSITIONTCS._serialized_end=7679
-  _SETSITEPOSITIONSTCSREQUEST._serialized_start=7681
-  _SETSITEPOSITIONSTCSREQUEST._serialized_end=7808
-  _FEATURESTARTSTOPREQUEST._serialized_start=7810
-  _FEATURESTARTSTOPREQUEST._serialized_end=7899
-  _PRIVACYREPLY._serialized_start=7901
-  _PRIVACYREPLY._serialized_end=7934
-  _SETPRIVACYREQUEST._serialized_start=7936
-  _SETPRIVACYREQUEST._serialized_end=7974
-  _DENSEMATRIX._serialized_start=7976
-  _DENSEMATRIX._serialized_end=8031
-  _KPIMETRICID._serialized_start=8033
-  _KPIMETRICID._serialized_end=8122
-  _TIMERANGE._serialized_start=8124
-  _TIMERANGE._serialized_end=8211
-  _BUNDLEREQ._serialized_start=8213
-  _BUNDLEREQ._serialized_end=8326
-  _KPIMETRICSREQ._serialized_start=8329
-  _KPIMETRICSREQ._serialized_end=8477
-  _KPIMETRICSDATA._serialized_start=8480
-  _KPIMETRICSDATA._serialized_end=8867
-  _KPIMETRICSDATA_METRICSTATS._serialized_start=8802
-  _KPIMETRICSDATA_METRICSTATS._serialized_end=8867
-  _KPIBUNDLEPACKETMETRICS._serialized_start=8869
-  _KPIBUNDLEPACKETMETRICS._serialized_end=8988
-  _KPIMETRICS._serialized_start=8990
-  _KPIMETRICS._serialized_end=9073
-  _KPICONTROLREQUEST._serialized_start=9076
-  _KPICONTROLREQUEST._serialized_end=9212
-  _SETKPIUPDATEPERIODREQUEST._serialized_start=9215
-  _SETKPIUPDATEPERIODREQUEST._serialized_end=9359
-  _SETKPITHRESHOLDREQUEST._serialized_start=9362
-  _SETKPITHRESHOLDREQUEST._serialized_end=9700
-  _SETKPIEVENTDETECTREQUEST._serialized_start=9703
-  _SETKPIEVENTDETECTREQUEST._serialized_end=9913
-  _SETKPIEVENTSHADOWREQUEST._serialized_start=9916
-  _SETKPIEVENTSHADOWREQUEST._serialized_end=10081
-  _SETKPIEVENTWINDOWREQUEST._serialized_start=10084
-  _SETKPIEVENTWINDOWREQUEST._serialized_end=10266
-  _GETKPISTATUSREQUEST._serialized_start=10268
-  _GETKPISTATUSREQUEST._serialized_end=10349
-  _KPISTATUSREPLY._serialized_start=10352
-  _KPISTATUSREPLY._serialized_end=10643
-  _SIGKPIPARAMRECORD._serialized_start=10646
-  _SIGKPIPARAMRECORD._serialized_end=11004
-  _ANNOTATEBUNDLE._serialized_start=11006
-  _ANNOTATEBUNDLE._serialized_end=11080
-  _PROJECTMETADATA._serialized_start=11082
-  _PROJECTMETADATA._serialized_end=11175
-  _SENSOREXTENDEDMETADATA._serialized_start=11177
-  _SENSOREXTENDEDMETADATA._serialized_end=11228
-  _GONUMMATRIXLIST._serialized_start=11230
-  _GONUMMATRIXLIST._serialized_end=11267
-  _RADIXMATRIXLIST._serialized_start=11269
-  _RADIXMATRIXLIST._serialized_end=11323
-  _RADIXMATRIX._serialized_start=11325
-  _RADIXMATRIX._serialized_end=11367
-  _RADIXSIGNALSLIST._serialized_start=11369
-  _RADIXSIGNALSLIST._serialized_end=11425
-  _RADIXSIGNALS._serialized_start=11428
-  _RADIXSIGNALS._serialized_end=11597
-  _VECTORSTRING._serialized_start=11599
-  _VECTORSTRING._serialized_end=11624
-  _VECTORFLOAT64._serialized_start=11626
-  _VECTORFLOAT64._serialized_end=11652
-  _VECTORSLICEFLOAT64._serialized_start=11654
-  _VECTORSLICEFLOAT64._serialized_end=11725
-  _LOGSYSKPISTATUSREPLY._serialized_start=11728
-  _LOGSYSKPISTATUSREPLY._serialized_end=12078
-  _KPICACHE._serialized_start=12081
-  _KPICACHE._serialized_end=12461
-  _LOGSYSKPITAILREPLY._serialized_start=12464
-  _LOGSYSKPITAILREPLY._serialized_end=12842
-  _KPIPORTINFO._serialized_start=12844
-  _KPIPORTINFO._serialized_end=12895
-  _KPITAILROWS._serialized_start=12898
-  _KPITAILROWS._serialized_end=13270
-  _WAREHOUSEHEALTHCHECKSPEC._serialized_start=13272
-  _WAREHOUSEHEALTHCHECKSPEC._serialized_end=13314
-  _OUTFITTERGETDEVICEREQUEST._serialized_start=13316
-  _OUTFITTERGETDEVICEREQUEST._serialized_end=13356
-  _SENSORCOMPREQUEST._serialized_start=13359
-  _SENSORCOMPREQUEST._serialized_end=13517
-  _REGISTERSENSORCOMPREQUEST._serialized_start=13519
-  _REGISTERSENSORCOMPREQUEST._serialized_end=13641
-  _SAVESENSORCOMPINSTANCEREQUEST._serialized_start=13644
-  _SAVESENSORCOMPINSTANCEREQUEST._serialized_end=13790
-  _PROBEDESC._serialized_start=13792
-  _PROBEDESC._serialized_end=13830
-  _HEADSTAGEDESC._serialized_start=13832
-  _HEADSTAGEDESC._serialized_end=13874
-  _GETSENSORCOMPREPLY._serialized_start=13876
-  _GETSENSORCOMPREPLY._serialized_end=13972
-  _PROBESPEC._serialized_start=13974
-  _PROBESPEC._serialized_end=14094
-  _HEADSTAGESPEC._serialized_start=14097
-  _HEADSTAGESPEC._serialized_end=14233
-  _PROBEMODEL._serialized_start=14236
-  _PROBEMODEL._serialized_end=14826
-  _PROBEMODEL_PROBESITEDESC._serialized_start=14473
-  _PROBEMODEL_PROBESITEDESC._serialized_end=14695
-  _PROBEMODEL_PROBEWIREFRAME._serialized_start=14697
-  _PROBEMODEL_PROBEWIREFRAME._serialized_end=14791
-  _PROBEMODEL_PROBEPTXY._serialized_start=14793
-  _PROBEMODEL_PROBEPTXY._serialized_end=14826
-  _PROBEMETADATA._serialized_start=14828
-  _PROBEMETADATA._serialized_end=14923
-  _HEADSTAGEMODEL._serialized_start=14926
-  _HEADSTAGEMODEL._serialized_end=15058
-  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_start=15007
-  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_end=15058
-  _HEADSTAGEMETADATA._serialized_start=15060
-  _HEADSTAGEMETADATA._serialized_end=15079
-  _USERPROFILE._serialized_start=15081
-  _USERPROFILE._serialized_end=15134
-  _GETCURRENTPROFILEREPLY._serialized_start=15136
-  _GETCURRENTPROFILEREPLY._serialized_end=15202
-  _GETALLPROFILESREPLY._serialized_start=15204
-  _GETALLPROFILESREPLY._serialized_end=15268
-  _SETCURRENTPROFILEREQUEST._serialized_start=15270
-  _SETCURRENTPROFILEREQUEST._serialized_end=15315
-  _MANAGENODEORGPAYLOAD._serialized_start=15318
-  _MANAGENODEORGPAYLOAD._serialized_end=15454
-  _MANAGENODEORGREQUEST._serialized_start=15456
-  _MANAGENODEORGREQUEST._serialized_end=15561
-  _MANAGENODEORGREPLY._serialized_start=15563
-  _MANAGENODEORGREPLY._serialized_end=15646
-  _MANAGENODELABPAYLOAD._serialized_start=15649
-  _MANAGENODELABPAYLOAD._serialized_end=15811
-  _MANAGENODELABREQUEST._serialized_start=15813
-  _MANAGENODELABREQUEST._serialized_end=15918
-  _MANAGENODELABREPLY._serialized_start=15920
-  _MANAGENODELABREPLY._serialized_end=16003
-  _MANAGENODEUSERPAYLOAD._serialized_start=16006
-  _MANAGENODEUSERPAYLOAD._serialized_end=16159
-  _MANAGENODEUSERREQUEST._serialized_start=16161
-  _MANAGENODEUSERREQUEST._serialized_end=16268
-  _MANAGENODEUSERREPLY._serialized_start=16270
-  _MANAGENODEUSERREPLY._serialized_end=16355
-  _CATALOGPROBEPAYLOAD._serialized_start=16357
-  _CATALOGPROBEPAYLOAD._serialized_end=16411
-  _PROBENODEREQUEST._serialized_start=16413
-  _PROBENODEREQUEST._serialized_end=16506
-  _PROBENODEREPLY._serialized_start=16508
-  _PROBENODEREPLY._serialized_end=16563
-  _PROBEPAYLOAD._serialized_start=16565
-  _PROBEPAYLOAD._serialized_end=16612
-  _EDGEPAYLOAD._serialized_start=16615
-  _EDGEPAYLOAD._serialized_end=16908
-  _EDGEPAYLOAD_GENERICNODE._serialized_start=16818
-  _EDGEPAYLOAD_GENERICNODE._serialized_end=16908
-  _WORLDEDGEREQUEST._serialized_start=16910
-  _WORLDEDGEREQUEST._serialized_end=16966
-  _WORLDEDGEREPLY._serialized_start=16968
-  _WORLDEDGEREPLY._serialized_end=16984
-  _QUERYWORLDREQUEST._serialized_start=16986
-  _QUERYWORLDREQUEST._serialized_end=17055
-  _QUERYWORLDREC._serialized_start=17058
-  _QUERYWORLDREC._serialized_end=17288
-  _QUERYWORLDREPLY._serialized_start=17290
-  _QUERYWORLDREPLY._serialized_end=17347
-  _HIGHLOWPASSTRANSFORMPARAMS._serialized_start=17349
-  _HIGHLOWPASSTRANSFORMPARAMS._serialized_end=17396
-  _BANDTRANSFORMPARAMS._serialized_start=17398
-  _BANDTRANSFORMPARAMS._serialized_end=17464
-  _NOTCHTRANSFORMPARAMS._serialized_start=17466
-  _NOTCHTRANSFORMPARAMS._serialized_end=17536
-  _CARTRANSFORMPARAMS._serialized_start=17538
-  _CARTRANSFORMPARAMS._serialized_end=17558
-  _VIRTUALREFTRANSFORMPARAMS._serialized_start=17560
-  _VIRTUALREFTRANSFORMPARAMS._serialized_end=17610
-  _PAIREDREFTRANSFORMPARAMS._serialized_start=17612
-  _PAIREDREFTRANSFORMPARAMS._serialized_end=17687
-  _DATASOURCESINKTRANSFORMPARAMS._serialized_start=17689
-  _DATASOURCESINKTRANSFORMPARAMS._serialized_end=17794
-  _SLICETIMETRANSFORMPARAMS._serialized_start=17796
-  _SLICETIMETRANSFORMPARAMS._serialized_end=17858
-  _SLICECHANNELSTRANSFORMPARAMS._serialized_start=17860
-  _SLICECHANNELSTRANSFORMPARAMS._serialized_end=17911
-  _DOWNSAMPLETRANSFORMPARAMS._serialized_start=17913
-  _DOWNSAMPLETRANSFORMPARAMS._serialized_end=17962
-  _POSITION._serialized_start=17964
-  _POSITION._serialized_end=17996
-  _TRANSFORMNODE._serialized_start=17999
-  _TRANSFORMNODE._serialized_end=18728
-  _TRANSFORMEDGE._serialized_start=18730
-  _TRANSFORMEDGE._serialized_end=18789
-  _PROTOCOL._serialized_start=18791
-  _PROTOCOL._serialized_end=18907
-  _PROTOCOLREQUEST._serialized_start=18909
-  _PROTOCOLREQUEST._serialized_end=18946
-  _RENAMEPROTOCOLREQUEST._serialized_start=18948
-  _RENAMEPROTOCOLREQUEST._serialized_end=19014
-  _GETALLPROTOCOLSREPLY._serialized_start=19016
-  _GETALLPROTOCOLSREPLY._serialized_end=19075
-  _APPLYPROTOCOLPROGRESS._serialized_start=19077
-  _APPLYPROTOCOLPROGRESS._serialized_end=19156
-  _SPIKESORTERSETPARAMREQUEST._serialized_start=19159
-  _SPIKESORTERSETPARAMREQUEST._serialized_end=19313
-  _SPIKESORTERSETPARAMSREQUEST._serialized_start=19315
-  _SPIKESORTERSETPARAMSREQUEST._serialized_end=19396
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=19399
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=19694
-  _WRANGLEREQUEST._serialized_start=19696
-  _WRANGLEREQUEST._serialized_end=19782
-  _WRANGLESPEC._serialized_start=19784
-  _WRANGLESPEC._serialized_end=19873
-  _WRANGLEIMPORT._serialized_start=19875
-  _WRANGLEIMPORT._serialized_end=19947
-  _WRANGLEIMPORTVEXSPIKESSIM._serialized_start=19949
-  _WRANGLEIMPORTVEXSPIKESSIM._serialized_end=20052
-  _WRANGLEFILEDESC._serialized_start=20054
-  _WRANGLEFILEDESC._serialized_end=20121
-  _WRANGLEMERGE._serialized_start=20123
-  _WRANGLEMERGE._serialized_end=20195
-  _WRANGLEMERGEVEXSPIKESVIEW._serialized_start=20198
-  _WRANGLEMERGEVEXSPIKESVIEW._serialized_end=20501
-  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_start=20504
-  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_end=20696
-  _DACSTREAMREQUEST._serialized_start=20698
-  _DACSTREAMREQUEST._serialized_end=20772
-  _EVENTVIEWERCONFIG._serialized_start=20775
-  _EVENTVIEWERCONFIG._serialized_end=20997
-  _EVENTVIEWERID._serialized_start=20999
-  _EVENTVIEWERID._serialized_end=21060
-  _GETEVENTVIEWEREVENTREQUEST._serialized_start=21062
-  _GETEVENTVIEWEREVENTREQUEST._serialized_end=21130
-  _EVENTVIEWEREVENTDESC._serialized_start=21132
-  _EVENTVIEWEREVENTDESC._serialized_end=21221
-  _EVENTVIEWEREVENT._serialized_start=21224
-  _EVENTVIEWEREVENT._serialized_end=21367
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=21369
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=21466
-  _LISTEVENTVIEWERSREPLY._serialized_start=21468
-  _LISTEVENTVIEWERSREPLY._serialized_end=21536
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=21538
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=21589
-  _STATUSPOLLFIELDSTOUPDATE._serialized_start=21591
-  _STATUSPOLLFIELDSTOUPDATE._serialized_end=21685
+  _RADIXFILETYPES._serialized_start=24387
+  _RADIXFILETYPES._serialized_end=24648
+  _SIGNALTYPE._serialized_start=24650
+  _SIGNALTYPE._serialized_end=24699
+  _RESAMPLEROUTINE._serialized_start=24701
+  _RESAMPLEROUTINE._serialized_end=24744
+  _PORT._serialized_start=24746
+  _PORT._serialized_end=24808
+  _WORKSPACEAPP._serialized_start=24810
+  _WORKSPACEAPP._serialized_end=24860
+  _WORKSPACECOMMANDS._serialized_start=24863
+  _WORKSPACECOMMANDS._serialized_end=25023
+  _GETWORKSPACECOMMANDS._serialized_start=25025
+  _GETWORKSPACECOMMANDS._serialized_end=25092
+  _RADIENSSERVERTYPE._serialized_start=25094
+  _RADIENSSERVERTYPE._serialized_end=25150
+  _GRPCSERVICETYPE._serialized_start=25153
+  _GRPCSERVICETYPE._serialized_end=25327
+  _DEVDATASETTYPE._serialized_start=25329
+  _DEVDATASETTYPE._serialized_end=25392
+  _PSDWINDOWTYPE._serialized_start=25394
+  _PSDWINDOWTYPE._serialized_end=25461
+  _PSDSCALING._serialized_start=25463
+  _PSDSCALING._serialized_end=25510
+  _DATASOURCESORT._serialized_start=25512
+  _DATASOURCESORT._serialized_end=25600
+  _SIGNALGROUPTYPE._serialized_start=25602
+  _SIGNALGROUPTYPE._serialized_end=25648
+  _DSPTYPE._serialized_start=25651
+  _DSPTYPE._serialized_end=25780
+  _FILTERSTAGE._serialized_start=25782
+  _FILTERSTAGE._serialized_end=25839
+  _FEATURELICENSE._serialized_start=25842
+  _FEATURELICENSE._serialized_end=26181
+  _KPIMETRICSMODE._serialized_start=26183
+  _KPIMETRICSMODE._serialized_end=26278
+  _KPIMETRICSENUM._serialized_start=26281
+  _KPIMETRICSENUM._serialized_end=27082
+  _KPIMETRICSSTATSENUM._serialized_start=27085
+  _KPIMETRICSSTATSENUM._serialized_end=27224
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=27227
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=27547
+  _TIMERANGESELMODE._serialized_start=27549
+  _TIMERANGESELMODE._serialized_end=27619
+  _OUTFITTERCOMPONENTTYPE._serialized_start=27621
+  _OUTFITTERCOMPONENTTYPE._serialized_end=27699
+  _WORLDNODELABEL._serialized_start=27701
+  _WORLDNODELABEL._serialized_end=27826
+  _WORLDEDGELABEL._serialized_start=27828
+  _WORLDEDGELABEL._serialized_end=27867
+  _WORLDEDGEDIRECTION._serialized_start=27869
+  _WORLDEDGEDIRECTION._serialized_end=27965
+  _USERROLETYPE._serialized_start=27968
+  _USERROLETYPE._serialized_end=28127
+  _MANAGENODECMD._serialized_start=28129
+  _MANAGENODECMD._serialized_end=28200
+  _WORLDQUERYCMD._serialized_start=28203
+  _WORLDQUERYCMD._serialized_end=28435
+  _TRANSFORMNODETYPE._serialized_start=28438
+  _TRANSFORMNODETYPE._serialized_end=28678
+  _SPIKESORTERPARAMCOMMAND._serialized_start=28681
+  _SPIKESORTERPARAMCOMMAND._serialized_end=28904
+  _WRANGLEMODE._serialized_start=28907
+  _WRANGLEMODE._serialized_end=29038
+  _STATUSPOLLFIELDS._serialized_start=29041
+  _STATUSPOLLFIELDS._serialized_end=29559
+  _DASHBOARDTYPE._serialized_start=29561
+  _DASHBOARDTYPE._serialized_end=29588
+  _DASHBOARDCOMMAND._serialized_start=29590
+  _DASHBOARDCOMMAND._serialized_end=29668
+  _RADIXENVIRONMENT._serialized_start=57
+  _RADIXENVIRONMENT._serialized_end=114
+  _STANDARDREQUEST._serialized_start=116
+  _STANDARDREQUEST._serialized_end=149
+  _STANDARDREPLY._serialized_start=151
+  _STANDARDREPLY._serialized_end=198
+  _DACOFFREQUEST._serialized_start=200
+  _DACOFFREQUEST._serialized_end=238
+  _WORKSPACEDESCRIPTOR._serialized_start=241
+  _WORKSPACEDESCRIPTOR._serialized_end=427
+  _WORKSPACECONTROLREQUEST._serialized_start=430
+  _WORKSPACECONTROLREQUEST._serialized_end=614
+  _GETWORKSPACEREQUEST._serialized_start=617
+  _GETWORKSPACEREQUEST._serialized_end=828
+  _GETWORKSPACEREPLY._serialized_start=831
+  _GETWORKSPACEREPLY._serialized_end=1002
+  _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._serialized_start=921
+  _GETWORKSPACEREPLY_WORKSPACEDESCENTRY._serialized_end=1002
+  _GETRADIENSSERVERSREQUEST._serialized_start=1004
+  _GETRADIENSSERVERSREQUEST._serialized_end=1100
+  _SERVERSPEC._serialized_start=1103
+  _SERVERSPEC._serialized_end=1382
+  _SERVERSPEC_GRPCSERVICE._serialized_start=1244
+  _SERVERSPEC_GRPCSERVICE._serialized_end=1271
+  _SERVERSPEC_SPAWNEDPROCESS._serialized_start=1273
+  _SERVERSPEC_SPAWNEDPROCESS._serialized_end=1302
+  _SERVERSPEC_SERVICEENTRY._serialized_start=1304
+  _SERVERSPEC_SERVICEENTRY._serialized_end=1382
+  _RADIENSSERVERSREPLY._serialized_start=1384
+  _RADIENSSERVERSREPLY._serialized_end=1490
+  _SIGNALGROUPIDREQUEST._serialized_start=1492
+  _SIGNALGROUPIDREQUEST._serialized_end=1537
+  _SIGNALMAP._serialized_start=1540
+  _SIGNALMAP._serialized_end=1736
+  _GPIOCHANNELCOUNT._serialized_start=1738
+  _GPIOCHANNELCOUNT._serialized_end=1799
+  _PORTCHANNELCOUNT._serialized_start=1801
+  _PORTCHANNELCOUNT._serialized_end=1869
+  _SETPORTREQUEST._serialized_start=1871
+  _SETPORTREQUEST._serialized_end=1952
+  _HDSNAPSHOTREQUEST._serialized_start=1955
+  _HDSNAPSHOTREQUEST._serialized_end=2309
+  _HDSNAPSHOTREQUEST_SELECTEDSIGNALS._serialized_start=2271
+  _HDSNAPSHOTREQUEST_SELECTEDSIGNALS._serialized_end=2309
+  _HDSNAPSHOTREQUEST2._serialized_start=2312
+  _HDSNAPSHOTREQUEST2._serialized_end=2462
+  _RADIENSPYGRAPHICSARGS._serialized_start=2464
+  _RADIENSPYGRAPHICSARGS._serialized_end=2540
+  _PSDREQUEST._serialized_start=2543
+  _PSDREQUEST._serialized_end=2892
+  _PSD._serialized_start=2895
+  _PSD._serialized_end=3184
+  _RADIENSPYGRAPHICSREQUEST._serialized_start=3186
+  _RADIENSPYGRAPHICSREQUEST._serialized_end=3287
+  _SIGSELECTOR._serialized_start=3289
+  _SIGSELECTOR._serialized_end=3383
+  _HDSNAPSHOTMETA._serialized_start=3385
+  _HDSNAPSHOTMETA._serialized_end=3478
+  _HDSNAPSHOT._serialized_start=3481
+  _HDSNAPSHOT._serialized_end=3768
+  _HDSNAPSHOT2._serialized_start=3770
+  _HDSNAPSHOT2._serialized_end=3834
+  _GETSIGNALSREQUEST._serialized_start=3837
+  _GETSIGNALSREQUEST._serialized_end=4163
+  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_start=3939
+  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_end=4163
+  _RAWSIGNALS._serialized_start=4165
+  _RAWSIGNALS._serialized_end=4256
+  _SIGNALS2._serialized_start=4259
+  _SIGNALS2._serialized_end=4490
+  _LISTSENSORSPECSREPLY._serialized_start=4493
+  _LISTSENSORSPECSREPLY._serialized_end=4754
+  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_start=4696
+  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_end=4754
+  _LISTDATASOURCESREQUEST._serialized_start=4756
+  _LISTDATASOURCESREQUEST._serialized_end=4856
+  _SORTMAP._serialized_start=4858
+  _SORTMAP._serialized_end=4886
+  _GETSIGNALGROUPIDSREPLY._serialized_start=4888
+  _GETSIGNALGROUPIDSREPLY._serialized_end=4950
+  _GETSORTERIDMAPREPLY._serialized_start=4953
+  _GETSORTERIDMAPREPLY._serialized_end=5113
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_start=5045
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_end=5113
+  _DATASOURCE._serialized_start=5116
+  _DATASOURCE._serialized_end=5291
+  _FILEDESCRIPTOR._serialized_start=5293
+  _FILEDESCRIPTOR._serialized_end=5404
+  _TIMESPEC._serialized_start=5407
+  _TIMESPEC._serialized_end=5615
+  _TIMESPEC_TIMERANGEL._serialized_start=5529
+  _TIMESPEC_TIMERANGEL._serialized_end=5560
+  _TIMESPEC_TIMESTAMPRANGEL._serialized_start=5562
+  _TIMESPEC_TIMESTAMPRANGEL._serialized_end=5603
+  _SIGNALSPEC._serialized_start=5618
+  _SIGNALSPEC._serialized_end=5808
+  _SIGNALSPEC_SITENUML._serialized_start=5734
+  _SIGNALSPEC_SITENUML._serialized_end=5761
+  _SIGNALSPEC_NTVCHANIDXL._serialized_start=5763
+  _SIGNALSPEC_NTVCHANIDXL._serialized_end=5796
+  _CHANNELRECORD._serialized_start=5811
+  _CHANNELRECORD._serialized_end=6572
+  _XYCOORD._serialized_start=6574
+  _XYCOORD._serialized_end=6605
+  _XYZCOORD._serialized_start=6607
+  _XYZCOORD._serialized_end=6650
+  _SENSOR._serialized_start=6653
+  _SENSOR._serialized_end=7019
+  _SENSOR_WIREFRAME._serialized_start=6910
+  _SENSOR_WIREFRAME._serialized_end=7019
+  _SENSORPORTSPEC._serialized_start=7022
+  _SENSORPORTSPEC._serialized_end=7302
+  _SIGNALGROUPUNITS._serialized_start=7304
+  _SIGNALGROUPUNITS._serialized_end=7420
+  _SIGNALGROUPUNITS_UNITSENTRY._serialized_start=7376
+  _SIGNALGROUPUNITS_UNITSENTRY._serialized_end=7420
+  _SIGNALGROUP._serialized_start=7423
+  _SIGNALGROUP._serialized_end=7679
+  _CREATESIGNALGROUPREQUEST._serialized_start=7682
+  _CREATESIGNALGROUPREQUEST._serialized_end=7817
+  _SUBOPSORT._serialized_start=7819
+  _SUBOPSORT._serialized_end=7934
+  _SUBOPSORT_SORTFIELD._serialized_start=7875
+  _SUBOPSORT_SORTFIELD._serialized_end=7934
+  _UPDATESIGNALGROUPREQUEST._serialized_start=7937
+  _UPDATESIGNALGROUPREQUEST._serialized_end=8358
+  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_start=8239
+  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_end=8305
+  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_start=8307
+  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_end=8342
+  _SLICESIGNALGROUPSPEC._serialized_start=8360
+  _SLICESIGNALGROUPSPEC._serialized_end=8444
+  _SLICESIGNALGROUPREQUEST._serialized_start=8446
+  _SLICESIGNALGROUPREQUEST._serialized_end=8534
+  _SLICESIGNALGROUPREPLY._serialized_start=8537
+  _SLICESIGNALGROUPREPLY._serialized_end=8673
+  _LICENSESTATUS._serialized_start=8675
+  _LICENSESTATUS._serialized_end=8690
+  _SETDSPGROUPREQUEST._serialized_start=8692
+  _SETDSPGROUPREQUEST._serialized_end=8809
+  _DSPPARAMS._serialized_start=8812
+  _DSPPARAMS._serialized_end=9182
+  _DSPPARAMS_FREQSPECBAND._serialized_start=9121
+  _DSPPARAMS_FREQSPECBAND._serialized_end=9170
+  _DSPGROUP._serialized_start=9185
+  _DSPGROUP._serialized_end=9318
+  _SETSENSORREQUEST._serialized_start=9321
+  _SETSENSORREQUEST._serialized_end=9454
+  _SENSORPOSITIONTCS._serialized_start=9456
+  _SENSORPOSITIONTCS._serialized_end=9565
+  _SETSENSORPOSITIONTCSREQUEST._serialized_start=9568
+  _SETSENSORPOSITIONTCSREQUEST._serialized_end=9712
+  _SITEPOSITIONTCS._serialized_start=9714
+  _SITEPOSITIONTCS._serialized_end=9784
+  _SETSITEPOSITIONSTCSREQUEST._serialized_start=9786
+  _SETSITEPOSITIONSTCSREQUEST._serialized_end=9913
+  _FEATURESTARTSTOPREQUEST._serialized_start=9915
+  _FEATURESTARTSTOPREQUEST._serialized_end=10004
+  _PRIVACYREPLY._serialized_start=10006
+  _PRIVACYREPLY._serialized_end=10039
+  _SETPRIVACYREQUEST._serialized_start=10041
+  _SETPRIVACYREQUEST._serialized_end=10079
+  _DENSEMATRIX._serialized_start=10081
+  _DENSEMATRIX._serialized_end=10136
+  _KPIMETRICID._serialized_start=10138
+  _KPIMETRICID._serialized_end=10227
+  _TIMERANGE._serialized_start=10230
+  _TIMERANGE._serialized_end=10363
+  _BUNDLEREQ._serialized_start=10365
+  _BUNDLEREQ._serialized_end=10478
+  _KPIMETRICSREQ._serialized_start=10481
+  _KPIMETRICSREQ._serialized_end=10638
+  _KPIMETRICSDATA._serialized_start=10641
+  _KPIMETRICSDATA._serialized_end=11028
+  _KPIMETRICSDATA_METRICSTATS._serialized_start=10963
+  _KPIMETRICSDATA_METRICSTATS._serialized_end=11028
+  _KPIBUNDLEPACKETMETRICS._serialized_start=11030
+  _KPIBUNDLEPACKETMETRICS._serialized_end=11149
+  _KPIMETRICS._serialized_start=11151
+  _KPIMETRICS._serialized_end=11234
+  _KPICONTROLREQUEST._serialized_start=11236
+  _KPICONTROLREQUEST._serialized_end=11335
+  _SETKPIPARAMREQUEST._serialized_start=11337
+  _SETKPIPARAMREQUEST._serialized_end=11395
+  _GETKPISTATUSREQUEST._serialized_start=11397
+  _GETKPISTATUSREQUEST._serialized_end=11441
+  _KPISTANDARDREQUEST._serialized_start=11443
+  _KPISTANDARDREQUEST._serialized_end=11482
+  _KPIFILESTATUS._serialized_start=11485
+  _KPIFILESTATUS._serialized_end=11671
+  _KPIFILESTATUS_STATE._serialized_start=11548
+  _KPIFILESTATUS_STATE._serialized_end=11671
+  _KPIFILESTATUS2._serialized_start=11674
+  _KPIFILESTATUS2._serialized_end=12257
+  _KPIFILESTATUS2_KPI_STATE._serialized_start=11757
+  _KPIFILESTATUS2_KPI_STATE._serialized_end=11990
+  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_start=11992
+  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_end=12105
+  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_start=12108
+  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_end=12257
+  _KPIFILEMETADATA._serialized_start=12260
+  _KPIFILEMETADATA._serialized_end=12513
+  _KPIFILEMETADATA_STATE._serialized_start=12328
+  _KPIFILEMETADATA_STATE._serialized_end=12513
+  _KPISTATUSREPLY._serialized_start=12516
+  _KPISTATUSREPLY._serialized_end=12855
+  _SIGKPIPARAMRECORD._serialized_start=12858
+  _SIGKPIPARAMRECORD._serialized_end=13216
+  _ANNOTATEBUNDLE._serialized_start=13218
+  _ANNOTATEBUNDLE._serialized_end=13292
+  _PROJECTMETADATA._serialized_start=13294
+  _PROJECTMETADATA._serialized_end=13387
+  _SENSOREXTENDEDMETADATA._serialized_start=13389
+  _SENSOREXTENDEDMETADATA._serialized_end=13440
+  _GONUMMATRIXLIST._serialized_start=13442
+  _GONUMMATRIXLIST._serialized_end=13479
+  _RADIXMATRIXLIST._serialized_start=13481
+  _RADIXMATRIXLIST._serialized_end=13535
+  _RADIXMATRIX._serialized_start=13537
+  _RADIXMATRIX._serialized_end=13579
+  _RADIXMATRIXBYTES._serialized_start=13581
+  _RADIXMATRIXBYTES._serialized_end=13628
+  _RADIXSIGNALSLIST._serialized_start=13630
+  _RADIXSIGNALSLIST._serialized_end=13686
+  _RADIXSIGNALS._serialized_start=13689
+  _RADIXSIGNALS._serialized_end=13858
+  _VECTORSTRING._serialized_start=13860
+  _VECTORSTRING._serialized_end=13885
+  _VECTORFLOAT64._serialized_start=13887
+  _VECTORFLOAT64._serialized_end=13913
+  _VECTORSLICEFLOAT64._serialized_start=13915
+  _VECTORSLICEFLOAT64._serialized_end=13986
+  _LOGSYSKPISTATUSREPLY._serialized_start=13989
+  _LOGSYSKPISTATUSREPLY._serialized_end=14339
+  _KPICACHE._serialized_start=14342
+  _KPICACHE._serialized_end=14722
+  _LOGSYSKPITAILREPLY._serialized_start=14725
+  _LOGSYSKPITAILREPLY._serialized_end=15103
+  _KPIPORTINFO._serialized_start=15105
+  _KPIPORTINFO._serialized_end=15156
+  _KPITAILROWS._serialized_start=15159
+  _KPITAILROWS._serialized_end=15531
+  _WAREHOUSEHEALTHCHECKSPEC._serialized_start=15533
+  _WAREHOUSEHEALTHCHECKSPEC._serialized_end=15575
+  _OUTFITTERGETDEVICEREQUEST._serialized_start=15577
+  _OUTFITTERGETDEVICEREQUEST._serialized_end=15617
+  _SENSORCOMPREQUEST._serialized_start=15620
+  _SENSORCOMPREQUEST._serialized_end=15778
+  _REGISTERSENSORCOMPREQUEST._serialized_start=15780
+  _REGISTERSENSORCOMPREQUEST._serialized_end=15902
+  _SAVESENSORCOMPINSTANCEREQUEST._serialized_start=15905
+  _SAVESENSORCOMPINSTANCEREQUEST._serialized_end=16051
+  _PROBEDESC._serialized_start=16053
+  _PROBEDESC._serialized_end=16091
+  _HEADSTAGEDESC._serialized_start=16093
+  _HEADSTAGEDESC._serialized_end=16135
+  _GETSENSORCOMPREPLY._serialized_start=16137
+  _GETSENSORCOMPREPLY._serialized_end=16233
+  _PROBESPEC._serialized_start=16235
+  _PROBESPEC._serialized_end=16355
+  _HEADSTAGESPEC._serialized_start=16358
+  _HEADSTAGESPEC._serialized_end=16494
+  _PROBEMODEL._serialized_start=16497
+  _PROBEMODEL._serialized_end=17087
+  _PROBEMODEL_PROBESITEDESC._serialized_start=16734
+  _PROBEMODEL_PROBESITEDESC._serialized_end=16956
+  _PROBEMODEL_PROBEWIREFRAME._serialized_start=16958
+  _PROBEMODEL_PROBEWIREFRAME._serialized_end=17052
+  _PROBEMODEL_PROBEPTXY._serialized_start=17054
+  _PROBEMODEL_PROBEPTXY._serialized_end=17087
+  _PROBEMETADATA._serialized_start=17089
+  _PROBEMETADATA._serialized_end=17184
+  _HEADSTAGEMODEL._serialized_start=17187
+  _HEADSTAGEMODEL._serialized_end=17319
+  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_start=17268
+  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_end=17319
+  _HEADSTAGEMETADATA._serialized_start=17321
+  _HEADSTAGEMETADATA._serialized_end=17340
+  _USERPROFILE._serialized_start=17342
+  _USERPROFILE._serialized_end=17395
+  _GETCURRENTPROFILEREPLY._serialized_start=17397
+  _GETCURRENTPROFILEREPLY._serialized_end=17463
+  _GETALLPROFILESREPLY._serialized_start=17465
+  _GETALLPROFILESREPLY._serialized_end=17529
+  _SETCURRENTPROFILEREQUEST._serialized_start=17531
+  _SETCURRENTPROFILEREQUEST._serialized_end=17576
+  _MANAGENODEORGPAYLOAD._serialized_start=17579
+  _MANAGENODEORGPAYLOAD._serialized_end=17715
+  _MANAGENODEORGREQUEST._serialized_start=17717
+  _MANAGENODEORGREQUEST._serialized_end=17822
+  _MANAGENODEORGREPLY._serialized_start=17824
+  _MANAGENODEORGREPLY._serialized_end=17907
+  _MANAGENODELABPAYLOAD._serialized_start=17910
+  _MANAGENODELABPAYLOAD._serialized_end=18072
+  _MANAGENODELABREQUEST._serialized_start=18074
+  _MANAGENODELABREQUEST._serialized_end=18179
+  _MANAGENODELABREPLY._serialized_start=18181
+  _MANAGENODELABREPLY._serialized_end=18264
+  _MANAGENODEUSERPAYLOAD._serialized_start=18267
+  _MANAGENODEUSERPAYLOAD._serialized_end=18420
+  _MANAGENODEUSERREQUEST._serialized_start=18422
+  _MANAGENODEUSERREQUEST._serialized_end=18529
+  _MANAGENODEUSERREPLY._serialized_start=18531
+  _MANAGENODEUSERREPLY._serialized_end=18616
+  _CATALOGPROBEPAYLOAD._serialized_start=18618
+  _CATALOGPROBEPAYLOAD._serialized_end=18672
+  _PROBENODEREQUEST._serialized_start=18674
+  _PROBENODEREQUEST._serialized_end=18767
+  _PROBENODEREPLY._serialized_start=18769
+  _PROBENODEREPLY._serialized_end=18824
+  _PROBEPAYLOAD._serialized_start=18826
+  _PROBEPAYLOAD._serialized_end=18873
+  _EDGEPAYLOAD._serialized_start=18876
+  _EDGEPAYLOAD._serialized_end=19169
+  _EDGEPAYLOAD_GENERICNODE._serialized_start=19079
+  _EDGEPAYLOAD_GENERICNODE._serialized_end=19169
+  _WORLDEDGEREQUEST._serialized_start=19171
+  _WORLDEDGEREQUEST._serialized_end=19227
+  _WORLDEDGEREPLY._serialized_start=19229
+  _WORLDEDGEREPLY._serialized_end=19245
+  _QUERYWORLDREQUEST._serialized_start=19247
+  _QUERYWORLDREQUEST._serialized_end=19316
+  _QUERYWORLDREC._serialized_start=19319
+  _QUERYWORLDREC._serialized_end=19549
+  _QUERYWORLDREPLY._serialized_start=19551
+  _QUERYWORLDREPLY._serialized_end=19608
+  _HIGHLOWPASSTRANSFORMPARAMS._serialized_start=19610
+  _HIGHLOWPASSTRANSFORMPARAMS._serialized_end=19657
+  _BANDTRANSFORMPARAMS._serialized_start=19659
+  _BANDTRANSFORMPARAMS._serialized_end=19725
+  _NOTCHTRANSFORMPARAMS._serialized_start=19727
+  _NOTCHTRANSFORMPARAMS._serialized_end=19797
+  _CARTRANSFORMPARAMS._serialized_start=19799
+  _CARTRANSFORMPARAMS._serialized_end=19819
+  _VIRTUALREFTRANSFORMPARAMS._serialized_start=19821
+  _VIRTUALREFTRANSFORMPARAMS._serialized_end=19871
+  _PAIREDREFTRANSFORMPARAMS._serialized_start=19873
+  _PAIREDREFTRANSFORMPARAMS._serialized_end=19948
+  _DATASOURCESINKTRANSFORMPARAMS._serialized_start=19950
+  _DATASOURCESINKTRANSFORMPARAMS._serialized_end=20055
+  _SLICETIMETRANSFORMPARAMS._serialized_start=20057
+  _SLICETIMETRANSFORMPARAMS._serialized_end=20119
+  _SLICECHANNELSTRANSFORMPARAMS._serialized_start=20121
+  _SLICECHANNELSTRANSFORMPARAMS._serialized_end=20172
+  _DOWNSAMPLETRANSFORMPARAMS._serialized_start=20174
+  _DOWNSAMPLETRANSFORMPARAMS._serialized_end=20223
+  _POSITION._serialized_start=20225
+  _POSITION._serialized_end=20257
+  _TRANSFORMNODE._serialized_start=20260
+  _TRANSFORMNODE._serialized_end=20989
+  _TRANSFORMEDGE._serialized_start=20991
+  _TRANSFORMEDGE._serialized_end=21050
+  _PROTOCOL._serialized_start=21052
+  _PROTOCOL._serialized_end=21168
+  _PROTOCOLREQUEST._serialized_start=21170
+  _PROTOCOLREQUEST._serialized_end=21207
+  _RENAMEPROTOCOLREQUEST._serialized_start=21209
+  _RENAMEPROTOCOLREQUEST._serialized_end=21275
+  _GETALLPROTOCOLSREPLY._serialized_start=21277
+  _GETALLPROTOCOLSREPLY._serialized_end=21336
+  _APPLYPROTOCOLPROGRESS._serialized_start=21338
+  _APPLYPROTOCOLPROGRESS._serialized_end=21461
+  _SPIKESORTERSETPARAMREQUEST._serialized_start=21464
+  _SPIKESORTERSETPARAMREQUEST._serialized_end=21618
+  _SPIKESORTERSETPARAMSREQUEST._serialized_start=21620
+  _SPIKESORTERSETPARAMSREQUEST._serialized_end=21701
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=21704
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=21999
+  _KPIPARAMS._serialized_start=22001
+  _KPIPARAMS._serialized_end=22064
+  _WRANGLEREQUEST._serialized_start=22066
+  _WRANGLEREQUEST._serialized_end=22153
+  _WRANGLESPEC._serialized_start=22155
+  _WRANGLESPEC._serialized_end=22244
+  _WRANGLEIMPORT._serialized_start=22246
+  _WRANGLEIMPORT._serialized_end=22318
+  _WRANGLEIMPORTVEXSPIKESSIM._serialized_start=22320
+  _WRANGLEIMPORTVEXSPIKESSIM._serialized_end=22423
+  _WRANGLEFILEDESC._serialized_start=22425
+  _WRANGLEFILEDESC._serialized_end=22492
+  _WRANGLEMERGE._serialized_start=22494
+  _WRANGLEMERGE._serialized_end=22566
+  _WRANGLEMERGEVEXSPIKESVIEW._serialized_start=22569
+  _WRANGLEMERGEVEXSPIKESVIEW._serialized_end=22872
+  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_start=22875
+  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_end=23067
+  _DACSTREAMREQUEST._serialized_start=23069
+  _DACSTREAMREQUEST._serialized_end=23143
+  _EVENTVIEWERCONFIG._serialized_start=23146
+  _EVENTVIEWERCONFIG._serialized_end=23368
+  _EVENTVIEWERID._serialized_start=23370
+  _EVENTVIEWERID._serialized_end=23431
+  _GETEVENTVIEWEREVENTREQUEST._serialized_start=23433
+  _GETEVENTVIEWEREVENTREQUEST._serialized_end=23501
+  _EVENTVIEWEREVENTDESC._serialized_start=23503
+  _EVENTVIEWEREVENTDESC._serialized_end=23592
+  _EVENTVIEWEREVENT._serialized_start=23595
+  _EVENTVIEWEREVENT._serialized_end=23738
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=23740
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=23837
+  _LISTEVENTVIEWERSREPLY._serialized_start=23839
+  _LISTEVENTVIEWERSREPLY._serialized_end=23907
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=23909
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=23960
+  _STATUSPOLLFIELDSTOUPDATE._serialized_start=23962
+  _STATUSPOLLFIELDSTOUPDATE._serialized_end=24056
+  _DASHBOARDCOMMANDREQUEST._serialized_start=24059
+  _DASHBOARDCOMMANDREQUEST._serialized_end=24224
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_start=24179
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_end=24224
+  _SELTABLESIGNALGROUP._serialized_start=24226
+  _SELTABLESIGNALGROUP._serialized_end=24319
+  _SELECTORTABLESREPLY._serialized_start=24321
+  _SELECTORTABLESREPLY._serialized_end=24384
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/datasource_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/datasource_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,58 +11,58 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61tasource.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x11\x44\x61taSourceRequest\x12\x11\n\tdsourceID\x18\x01 \x03(\t\x12\x14\n\x0crenameDsrcID\x18\x02 \x01(\t\"\xae\x01\n\x18\x44\x61taSourceSetSaveRequest\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12\x11\n\tdsourceID\x18\x03 \x01(\t\x12\x0b\n\x03uID\x18\x04 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x0f\n\x07isForce\x18\x06 \x01(\x08\x12\x17\n\x0fisBackgroundKPI\x18\x07 \x01(\x08\"%\n\x11\x44\x61taSourceIDReply\x12\x10\n\x08sortedID\x18\x01 \x03(\t\"\x95\x01\n\x16\x44\x61taSourceSetSaveReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12(\n\x06status\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus\x12\r\n\x05niIDs\x18\x03 \x03(\t\x12/\n\x0f\x61ssociatedDsrcs\x18\x04 \x03(\x0b\x32\x16.allego.FileDescriptor\"\xae\x01\n\x13\x44\x61taSourceStatusMap\x12\x39\n\x07\x64source\x18\x01 \x03(\x0b\x32(.allego.DataSourceStatusMap.DsourceEntry\x12\x12\n\norderedIDs\x18\x02 \x03(\t\x1aH\n\x0c\x44sourceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus:\x02\x38\x01\"\xa1\x03\n\x1f\x43opyRemoveDataSourceFileRequest\x12\x45\n\x04many\x18\x01 \x01(\x0b\x32\x35.allego.CopyRemoveDataSourceFileRequest.MultipleFilesH\x00\x12>\n\x03one\x18\x02 \x01(\x0b\x32/.allego.CopyRemoveDataSourceFileRequest.OneFileH\x00\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\x1at\n\rMultipleFiles\x12#\n\x03src\x18\x01 \x03(\x0b\x32\x16.allego.FileDescriptor\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12,\n\x0c\x64\x65stFileType\x18\x03 \x01(\x0e\x32\x16.allego.RadixFileTypes\x1aT\n\x07OneFile\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptorB\x06\n\x04\x64\x65sc\"\xf8\x02\n\x15\x44\x61taSourceFileSetStat\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x1b\n\x13numBytesPrimaryData\x18\x02 \x02(\x03\x12\x18\n\x10numBytesMetaData\x18\x03 \x02(\x03\x12\x10\n\x08numBytes\x18\x04 \x02(\x03\x12\x16\n\x0eisMetadataFile\x18\x05 \x02(\x08\x12-\n\ttimeStamp\x18\x06 \x02(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bnumChannels\x18\x07 \x02(\x05\x12\x13\n\x0b\x64urationSec\x18\x08 \x02(\x01\x12\x12\n\ndatasetUID\x18\t \x02(\t\x12\x17\n\x0f\x64\x61tasetChecksum\x18\n \x01(\t\x12\x19\n\x11\x64\x61tasetProvenance\x18\x0b \x03(\t\x12\x12\n\nsampleRate\x18\x0c \x02(\x05\x12\x37\n\x0e\x62\x61\x63kgroundProc\x18\r \x01(\x0b\x32\x1f.allego.BackgroundProcessStatus\"\x82\x02\n\rCpRmMvLsReply\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x12\n\nnumDsource\x18\x02 \x02(\x05\x12\x10\n\x08numBytes\x18\x03 \x02(\x03\x12\x10\n\x08\x64\x65stPath\x18\x04 \x02(\t\x12\x35\n\x07\x64source\x18\x05 \x03(\x0b\x32$.allego.CpRmMvLsReply.DataSourceInfo\x12\x0b\n\x03msg\x18\x06 \x01(\t\x1a\x63\n\x0e\x44\x61taSourceInfo\x12$\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12+\n\x04stat\x18\x02 \x02(\x0b\x32\x1d.allego.DataSourceFileSetStat\"y\n\x17\x42\x61\x63kgroundProcessStatus\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x16\n\x0e\x65lapsedTimeSec\x18\x03 \x01(\x01\x12#\n\x1b\x65stimatedCompletionWallTime\x18\x04 \x01(\t\"\x8b\x01\n\x19MoveDataSourceFileRequest\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x02(\x0b\x32\x16.allego.FileDescriptor\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\"\xc5\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x02(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\"\xbf\x01\n\x10\x44\x61taSourceParams\x12\x12\n\nsampleFreq\x18\x01 \x02(\x01\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12%\n\x04type\x18\x05 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x35\n\x0e\x64\x61tasourceType\x18\x06 \x01(\x0e\x32\x1d.allego.RadiensDatasourceType\x12\x14\n\x0c\x64\x61tasourceID\x18\x07 \x01(\t\".\n\x10ImpedanceRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\"\x85\x01\n\tImpedance\x12\x34\n\nimpedances\x18\x01 \x03(\x0b\x32 .allego.Impedance.ImpedanceValue\x1a\x42\n\x0eImpedanceValue\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0c\n\x04zMag\x18\x02 \x02(\x01\x12\x0e\n\x06zPhase\x18\x03 \x02(\x01*0\n\x15RadiensDatasourceType\x12\x07\n\x03\x41NY\x10\x00\x12\x0e\n\nTIMESERIES\x10\x01\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61tasource.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x11\x44\x61taSourceRequest\x12\x11\n\tdsourceID\x18\x01 \x03(\t\x12\x14\n\x0crenameDsrcID\x18\x02 \x01(\t\"\xc7\x01\n\x18\x44\x61taSourceSetSaveRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x01(\t\x12\x11\n\tdsourceID\x18\x03 \x01(\t\x12\x0b\n\x03uID\x18\x04 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x01(\x0e\x32\x16.allego.RadixFileTypes\x12\x0f\n\x07isForce\x18\x06 \x01(\x08\x12\x17\n\x0fisBackgroundKPI\x18\x07 \x01(\x08\x12\x17\n\x0fparentDsourceID\x18\x08 \x01(\t\"%\n\x11\x44\x61taSourceIDReply\x12\x10\n\x08sortedID\x18\x01 \x03(\t\"\x95\x01\n\x16\x44\x61taSourceSetSaveReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12(\n\x06status\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus\x12\r\n\x05niIDs\x18\x03 \x03(\t\x12/\n\x0f\x61ssociatedDsrcs\x18\x04 \x03(\x0b\x32\x16.allego.FileDescriptor\"\xae\x01\n\x13\x44\x61taSourceStatusMap\x12\x39\n\x07\x64source\x18\x01 \x03(\x0b\x32(.allego.DataSourceStatusMap.DsourceEntry\x12\x12\n\norderedIDs\x18\x02 \x03(\t\x1aH\n\x0c\x44sourceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus:\x02\x38\x01\"\xa1\x03\n\x1f\x43opyRemoveDataSourceFileRequest\x12\x45\n\x04many\x18\x01 \x01(\x0b\x32\x35.allego.CopyRemoveDataSourceFileRequest.MultipleFilesH\x00\x12>\n\x03one\x18\x02 \x01(\x0b\x32/.allego.CopyRemoveDataSourceFileRequest.OneFileH\x00\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\x1at\n\rMultipleFiles\x12#\n\x03src\x18\x01 \x03(\x0b\x32\x16.allego.FileDescriptor\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12,\n\x0c\x64\x65stFileType\x18\x03 \x01(\x0e\x32\x16.allego.RadixFileTypes\x1aT\n\x07OneFile\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptorB\x06\n\x04\x64\x65sc\"\xf8\x02\n\x15\x44\x61taSourceFileSetStat\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x1b\n\x13numBytesPrimaryData\x18\x02 \x02(\x03\x12\x18\n\x10numBytesMetaData\x18\x03 \x02(\x03\x12\x10\n\x08numBytes\x18\x04 \x02(\x03\x12\x16\n\x0eisMetadataFile\x18\x05 \x02(\x08\x12-\n\ttimeStamp\x18\x06 \x02(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bnumChannels\x18\x07 \x02(\x05\x12\x13\n\x0b\x64urationSec\x18\x08 \x02(\x01\x12\x12\n\ndatasetUID\x18\t \x02(\t\x12\x17\n\x0f\x64\x61tasetChecksum\x18\n \x01(\t\x12\x19\n\x11\x64\x61tasetProvenance\x18\x0b \x03(\t\x12\x12\n\nsampleRate\x18\x0c \x02(\x05\x12\x37\n\x0e\x62\x61\x63kgroundProc\x18\r \x01(\x0b\x32\x1f.allego.BackgroundProcessStatus\"\x82\x02\n\rCpRmMvLsReply\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x12\n\nnumDsource\x18\x02 \x02(\x05\x12\x10\n\x08numBytes\x18\x03 \x02(\x03\x12\x10\n\x08\x64\x65stPath\x18\x04 \x02(\t\x12\x35\n\x07\x64source\x18\x05 \x03(\x0b\x32$.allego.CpRmMvLsReply.DataSourceInfo\x12\x0b\n\x03msg\x18\x06 \x01(\t\x1a\x63\n\x0e\x44\x61taSourceInfo\x12$\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12+\n\x04stat\x18\x02 \x02(\x0b\x32\x1d.allego.DataSourceFileSetStat\"y\n\x17\x42\x61\x63kgroundProcessStatus\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x16\n\x0e\x65lapsedTimeSec\x18\x03 \x01(\x01\x12#\n\x1b\x65stimatedCompletionWallTime\x18\x04 \x01(\t\"\x8b\x01\n\x19MoveDataSourceFileRequest\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x02(\x0b\x32\x16.allego.FileDescriptor\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\"\xfa\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x01(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\x12\x1d\n\x02tR\x18\x11 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0ckpiDsourceID\x18\x12 \x01(\t\"\xbf\x01\n\x10\x44\x61taSourceParams\x12\x12\n\nsampleFreq\x18\x01 \x02(\x01\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12%\n\x04type\x18\x05 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x35\n\x0e\x64\x61tasourceType\x18\x06 \x01(\x0e\x32\x1d.allego.RadiensDatasourceType\x12\x14\n\x0c\x64\x61tasourceID\x18\x07 \x01(\t\".\n\x10ImpedanceRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\"\x85\x01\n\tImpedance\x12\x34\n\nimpedances\x18\x01 \x03(\x0b\x32 .allego.Impedance.ImpedanceValue\x1a\x42\n\x0eImpedanceValue\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0c\n\x04zMag\x18\x02 \x02(\x01\x12\x0e\n\x06zPhase\x18\x03 \x02(\x01*0\n\x15RadiensDatasourceType\x12\x07\n\x03\x41NY\x10\x00\x12\x0e\n\nTIMESERIES\x10\x01\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'datasource_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _DATASOURCESTATUSMAP_DSOURCEENTRY._options = None
   _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_options = b'8\001'
-  _RADIENSDATASOURCETYPE._serialized_start=2713
-  _RADIENSDATASOURCETYPE._serialized_end=2761
+  _RADIENSDATASOURCETYPE._serialized_start=2791
+  _RADIENSDATASOURCETYPE._serialized_end=2839
   _DATASOURCEREQUEST._serialized_start=75
   _DATASOURCEREQUEST._serialized_end=135
   _DATASOURCESETSAVEREQUEST._serialized_start=138
-  _DATASOURCESETSAVEREQUEST._serialized_end=312
-  _DATASOURCEIDREPLY._serialized_start=314
-  _DATASOURCEIDREPLY._serialized_end=351
-  _DATASOURCESETSAVEREPLY._serialized_start=354
-  _DATASOURCESETSAVEREPLY._serialized_end=503
-  _DATASOURCESTATUSMAP._serialized_start=506
-  _DATASOURCESTATUSMAP._serialized_end=680
-  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_start=608
-  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_end=680
-  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_start=683
-  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_end=1100
-  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_start=890
-  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_end=1006
-  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_start=1008
-  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_end=1092
-  _DATASOURCEFILESETSTAT._serialized_start=1103
-  _DATASOURCEFILESETSTAT._serialized_end=1479
-  _CPRMMVLSREPLY._serialized_start=1482
-  _CPRMMVLSREPLY._serialized_end=1740
-  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_start=1641
-  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_end=1740
-  _BACKGROUNDPROCESSSTATUS._serialized_start=1742
-  _BACKGROUNDPROCESSSTATUS._serialized_end=1863
-  _MOVEDATASOURCEFILEREQUEST._serialized_start=1866
-  _MOVEDATASOURCEFILEREQUEST._serialized_end=2005
-  _DATASOURCESTATUS._serialized_start=2008
-  _DATASOURCESTATUS._serialized_end=2333
-  _DATASOURCEPARAMS._serialized_start=2336
-  _DATASOURCEPARAMS._serialized_end=2527
-  _IMPEDANCEREQUEST._serialized_start=2529
-  _IMPEDANCEREQUEST._serialized_end=2575
-  _IMPEDANCE._serialized_start=2578
-  _IMPEDANCE._serialized_end=2711
-  _IMPEDANCE_IMPEDANCEVALUE._serialized_start=2645
-  _IMPEDANCE_IMPEDANCEVALUE._serialized_end=2711
+  _DATASOURCESETSAVEREQUEST._serialized_end=337
+  _DATASOURCEIDREPLY._serialized_start=339
+  _DATASOURCEIDREPLY._serialized_end=376
+  _DATASOURCESETSAVEREPLY._serialized_start=379
+  _DATASOURCESETSAVEREPLY._serialized_end=528
+  _DATASOURCESTATUSMAP._serialized_start=531
+  _DATASOURCESTATUSMAP._serialized_end=705
+  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_start=633
+  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_end=705
+  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_start=708
+  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_end=1125
+  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_start=915
+  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_end=1031
+  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_start=1033
+  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_end=1117
+  _DATASOURCEFILESETSTAT._serialized_start=1128
+  _DATASOURCEFILESETSTAT._serialized_end=1504
+  _CPRMMVLSREPLY._serialized_start=1507
+  _CPRMMVLSREPLY._serialized_end=1765
+  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_start=1666
+  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_end=1765
+  _BACKGROUNDPROCESSSTATUS._serialized_start=1767
+  _BACKGROUNDPROCESSSTATUS._serialized_end=1888
+  _MOVEDATASOURCEFILEREQUEST._serialized_start=1891
+  _MOVEDATASOURCEFILEREQUEST._serialized_end=2030
+  _DATASOURCESTATUS._serialized_start=2033
+  _DATASOURCESTATUS._serialized_end=2411
+  _DATASOURCEPARAMS._serialized_start=2414
+  _DATASOURCEPARAMS._serialized_end=2605
+  _IMPEDANCEREQUEST._serialized_start=2607
+  _IMPEDANCEREQUEST._serialized_end=2653
+  _IMPEDANCE._serialized_start=2656
+  _IMPEDANCE._serialized_end=2789
+  _IMPEDANCE_IMPEDANCEVALUE._serialized_start=2723
+  _IMPEDANCE_IMPEDANCEVALUE._serialized_end=2789
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/radiens_dev_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/radiens_dev_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11radiens_dev.proto\x12\x06\x61llego\"\xc0\x01\n\x14SpkSortTrainerNewReq\x12\x33\n\x07\x64\x61taset\x18\x01 \x02(\x0b\x32\".allego.SpkSortTrainerDatasetParam\x12=\n\x08training\x18\x02 \x02(\x0b\x32+.allego.SpkSortTrainerNetworkTrainingParams\x12\x34\n\x05store\x18\x03 \x02(\x0b\x32%.allego.SpkSortTrainerStoreDescriptor\"l\n\x1cSpkSortTrainerDeleteModelReq\x12\x35\n\x07release\x18\x01 \x01(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x15\n\risDeleteNamed\x18\x02 \x01(\x08\"\xb6\x03\n\x1aSpkSortTrainerDatasetParam\x12\x14\n\x0c\x62ioPathTrain\x18\x01 \x03(\t\x12\x18\n\x10\x62ioBaseNameTrain\x18\x02 \x03(\t\x12\x19\n\x11\x62ioPathValidation\x18\x03 \x03(\t\x12\x1d\n\x15\x62ioBaseNameValidation\x18\x04 \x03(\t\x12\x13\n\x0b\x62ioPathTest\x18\x05 \x03(\t\x12\x17\n\x0f\x62ioBaseNameTest\x18\x06 \x03(\t\x12\x14\n\x0cnumNeighbors\x18\x07 \x02(\x05\x12\x10\n\x08radiusUm\x18\x08 \x02(\x01\x12\x19\n\x11maxNumSamplesTest\x18\t \x02(\x03\x12\x1a\n\x12networkMaskingFrac\x18\n \x02(\x01\x12 \n\x18networkInitWeightsStdDev\x18\x0b \x02(\x01\x12\x1d\n\x15networkInitBiasStdDev\x18\x0c \x02(\x01\x12\x17\n\x0fnetworkL1lambda\x18\r \x02(\x01\x12*\n\"networkHiddenLayerShapeRelInputDim\x18\x0e \x03(\x01\x12\x1b\n\x13networkNumFeatures2\x18\x0f \x02(\x05\"\xbd\x01\n#SpkSortTrainerNetworkTrainingParams\x12\x11\n\tnumEpochs\x18\x01 \x02(\x05\x12\x15\n\rminibatchSize\x18\x02 \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x03 \x02(\x03\x12\r\n\x05\x61lpha\x18\x04 \x02(\x01\x12\x11\n\talphaBias\x18\x05 \x02(\x01\x12\x18\n\x10\x65rrorTolPretrain\x18\x06 \x02(\x01\x12\x19\n\x11numSamplesTestMSE\x18\x07 \x02(\x05\"\x87\x02\n\x1dSpkSortTrainerStoreDescriptor\x12\x13\n\x0b\x62rainRegion\x18\x01 \x02(\t\x12\x36\n\x0bnetworkSize\x18\x02 \x02(\x0e\x32!.allego.SpkSortTrainerNetworkSize\x12\x39\n\nnbrPattern\x18\x03 \x02(\x0e\x32%.allego.SpkSortTrainerNeighborPattern\x12\x11\n\tnetworkID\x18\x04 \x02(\t\x12\x14\n\x0cnumNeighbors\x18\x05 \x02(\x05\x12\x35\n\x07release\x18\x06 \x02(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\"(\n\x18SpkSortTrainerSetModeReq\x12\x0c\n\x04mode\x18\x01 \x02(\x05\"\x81\x01\n\x14SpkSortTrainerCmdReq\x12;\n\x03\x63md\x18\x01 \x02(\x0e\x32..allego.SpkSortTrainerCmdReq.SpkSortTrainerCmd\",\n\x11SpkSortTrainerCmd\x12\n\n\x06\x43MD_ON\x10\x00\x12\x0b\n\x07\x43MD_OFF\x10\x01\",\n\x19SpkSortTrainerStatusReply\x12\x0f\n\x07msgJson\x18\x01 \x02(\x0c*\x81\x01\n\x19SpkSortTrainerNetworkSize\x12\x14\n\x10SST_SIZE_DEFAULT\x10\x00\x12\x10\n\x0cSST_SIZE_ARB\x10\x01\x12\x12\n\x0eSST_SIZE_SMALL\x10\x02\x12\x14\n\x10SST_SIZE_NOMINAL\x10\x03\x12\x12\n\x0eSST_SIZE_LARGE\x10\x04*\xa1\x01\n\x1dSpkSortTrainerNeighborPattern\x12\x17\n\x13SST_PATTERN_DEFAULT\x10\x00\x12\x13\n\x0fSST_PATTERN_ARB\x10\x01\x12\x14\n\x10SST_PATTERN_DIST\x10\x02\x12\x1d\n\x19SST_PATTERN_SPATIAL_TIGHT\x10\x03\x12\x1d\n\x19SST_PATTERN_SPATIAL_LOOSE\x10\x04*\xe3\x01\n\x1cSpkSortTrainerNetworkRelease\x12\x17\n\x13SST_NET_RELEASE_ANY\x10\x00\x12\x17\n\x13SST_NET_RELEASE_DEV\x10\x01\x12\x1b\n\x17SST_NET_RELEASE_DEV_MOD\x10\x02\x12\x18\n\x14SST_NET_RELEASE_PROD\x10\x03\x12\x1c\n\x18SST_NET_RELEASE_PROD_MOD\x10\x04\x12\x1b\n\x17SST_NET_RELEASE_SANDBOX\x10\x05\x12\x1f\n\x1bSST_NET_RELEASE_SANDBOX_MOD\x10\x06\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11radiens_dev.proto\x12\x06\x61llego\"\xc0\x01\n\x14SpkSortTrainerNewReq\x12\x33\n\x07\x64\x61taset\x18\x01 \x02(\x0b\x32\".allego.SpkSortTrainerDatasetParam\x12=\n\x08training\x18\x02 \x02(\x0b\x32+.allego.SpkSortTrainerNetworkTrainingParams\x12\x34\n\x05store\x18\x03 \x02(\x0b\x32%.allego.SpkSortTrainerStoreDescriptor\"l\n\x1cSpkSortTrainerDeleteModelReq\x12\x35\n\x07release\x18\x01 \x01(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x15\n\risDeleteNamed\x18\x02 \x01(\x08\"\xb0\x03\n\x1aSpkSortTrainerDatasetParam\x12\x13\n\x0bniPathTrain\x18\x01 \x03(\t\x12\x17\n\x0fniBaseNameTrain\x18\x02 \x03(\t\x12\x18\n\x10niPathValidation\x18\x03 \x03(\t\x12\x1c\n\x14niBaseNameValidation\x18\x04 \x03(\t\x12\x12\n\nniPathTest\x18\x05 \x03(\t\x12\x16\n\x0eniBaseNameTest\x18\x06 \x03(\t\x12\x14\n\x0cnumNeighbors\x18\x07 \x02(\x05\x12\x10\n\x08radiusUm\x18\x08 \x02(\x01\x12\x19\n\x11maxNumSamplesTest\x18\t \x02(\x03\x12\x1a\n\x12networkMaskingFrac\x18\n \x02(\x01\x12 \n\x18networkInitWeightsStdDev\x18\x0b \x02(\x01\x12\x1d\n\x15networkInitBiasStdDev\x18\x0c \x02(\x01\x12\x17\n\x0fnetworkL1lambda\x18\r \x02(\x01\x12*\n\"networkHiddenLayerShapeRelInputDim\x18\x0e \x03(\x01\x12\x1b\n\x13networkNumFeatures2\x18\x0f \x02(\x05\"\xbd\x01\n#SpkSortTrainerNetworkTrainingParams\x12\x11\n\tnumEpochs\x18\x01 \x02(\x05\x12\x15\n\rminibatchSize\x18\x02 \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x03 \x02(\x03\x12\r\n\x05\x61lpha\x18\x04 \x02(\x01\x12\x11\n\talphaBias\x18\x05 \x02(\x01\x12\x18\n\x10\x65rrorTolPretrain\x18\x06 \x02(\x01\x12\x19\n\x11numSamplesTestMSE\x18\x07 \x02(\x05\"\x87\x02\n\x1dSpkSortTrainerStoreDescriptor\x12\x13\n\x0b\x62rainRegion\x18\x01 \x02(\t\x12\x36\n\x0bnetworkSize\x18\x02 \x02(\x0e\x32!.allego.SpkSortTrainerNetworkSize\x12\x39\n\nnbrPattern\x18\x03 \x02(\x0e\x32%.allego.SpkSortTrainerNeighborPattern\x12\x11\n\tnetworkID\x18\x04 \x02(\t\x12\x14\n\x0cnumNeighbors\x18\x05 \x02(\x05\x12\x35\n\x07release\x18\x06 \x02(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\"(\n\x18SpkSortTrainerSetModeReq\x12\x0c\n\x04mode\x18\x01 \x02(\x05\"\x81\x01\n\x14SpkSortTrainerCmdReq\x12;\n\x03\x63md\x18\x01 \x02(\x0e\x32..allego.SpkSortTrainerCmdReq.SpkSortTrainerCmd\",\n\x11SpkSortTrainerCmd\x12\n\n\x06\x43MD_ON\x10\x00\x12\x0b\n\x07\x43MD_OFF\x10\x01\",\n\x19SpkSortTrainerStatusReply\x12\x0f\n\x07msgJson\x18\x01 \x02(\x0c*\x81\x01\n\x19SpkSortTrainerNetworkSize\x12\x14\n\x10SST_SIZE_DEFAULT\x10\x00\x12\x10\n\x0cSST_SIZE_ARB\x10\x01\x12\x12\n\x0eSST_SIZE_SMALL\x10\x02\x12\x14\n\x10SST_SIZE_NOMINAL\x10\x03\x12\x12\n\x0eSST_SIZE_LARGE\x10\x04*\xa1\x01\n\x1dSpkSortTrainerNeighborPattern\x12\x17\n\x13SST_PATTERN_DEFAULT\x10\x00\x12\x13\n\x0fSST_PATTERN_ARB\x10\x01\x12\x14\n\x10SST_PATTERN_DIST\x10\x02\x12\x1d\n\x19SST_PATTERN_SPATIAL_TIGHT\x10\x03\x12\x1d\n\x19SST_PATTERN_SPATIAL_LOOSE\x10\x04*\xe3\x01\n\x1cSpkSortTrainerNetworkRelease\x12\x17\n\x13SST_NET_RELEASE_ANY\x10\x00\x12\x17\n\x13SST_NET_RELEASE_DEV\x10\x01\x12\x1b\n\x17SST_NET_RELEASE_DEV_MOD\x10\x02\x12\x18\n\x14SST_NET_RELEASE_PROD\x10\x03\x12\x1c\n\x18SST_NET_RELEASE_PROD_MOD\x10\x04\x12\x1b\n\x17SST_NET_RELEASE_SANDBOX\x10\x05\x12\x1f\n\x1bSST_NET_RELEASE_SANDBOX_MOD\x10\x06\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'radiens_dev_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
-  _SPKSORTTRAINERNETWORKSIZE._serialized_start=1454
-  _SPKSORTTRAINERNETWORKSIZE._serialized_end=1583
-  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_start=1586
-  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_end=1747
-  _SPKSORTTRAINERNETWORKRELEASE._serialized_start=1750
-  _SPKSORTTRAINERNETWORKRELEASE._serialized_end=1977
+  _SPKSORTTRAINERNETWORKSIZE._serialized_start=1448
+  _SPKSORTTRAINERNETWORKSIZE._serialized_end=1577
+  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_start=1580
+  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_end=1741
+  _SPKSORTTRAINERNETWORKRELEASE._serialized_start=1744
+  _SPKSORTTRAINERNETWORKRELEASE._serialized_end=1971
   _SPKSORTTRAINERNEWREQ._serialized_start=30
   _SPKSORTTRAINERNEWREQ._serialized_end=222
   _SPKSORTTRAINERDELETEMODELREQ._serialized_start=224
   _SPKSORTTRAINERDELETEMODELREQ._serialized_end=332
   _SPKSORTTRAINERDATASETPARAM._serialized_start=335
-  _SPKSORTTRAINERDATASETPARAM._serialized_end=773
-  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_start=776
-  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_end=965
-  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_start=968
-  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_end=1231
-  _SPKSORTTRAINERSETMODEREQ._serialized_start=1233
-  _SPKSORTTRAINERSETMODEREQ._serialized_end=1273
-  _SPKSORTTRAINERCMDREQ._serialized_start=1276
-  _SPKSORTTRAINERCMDREQ._serialized_end=1405
-  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_start=1361
-  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_end=1405
-  _SPKSORTTRAINERSTATUSREPLY._serialized_start=1407
-  _SPKSORTTRAINERSTATUSREPLY._serialized_end=1451
+  _SPKSORTTRAINERDATASETPARAM._serialized_end=767
+  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_start=770
+  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_end=959
+  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_start=962
+  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_end=1225
+  _SPKSORTTRAINERSETMODEREQ._serialized_start=1227
+  _SPKSORTTRAINERSETMODEREQ._serialized_end=1267
+  _SPKSORTTRAINERCMDREQ._serialized_start=1270
+  _SPKSORTTRAINERCMDREQ._serialized_end=1399
+  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_start=1355
+  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_end=1399
+  _SPKSORTTRAINERSTATUSREPLY._serialized_start=1401
+  _SPKSORTTRAINERSTATUSREPLY._serialized_end=1445
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/radiensserver_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/radiensserver_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 from . import radiens_dev_pb2 as radiens__dev__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec2\xca/\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12>\n\nInitialize\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12>\n\x08KpiClear\x12\x19.allego.KpiControlRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0cKpiCalculate\x12\x19.allego.KpiControlRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12P\n\x12SetKpiUpdatePeriod\x12!.allego.SetKpiUpdatePeriodRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x0fSetKpiThreshold\x12\x1e.allego.SetKpiThresholdRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11SetKpiEventDetect\x12 .allego.SetKpiEventDetectRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11SetKpiEventShadow\x12 .allego.SetKpiEventShadowRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11SetKpiEventWindow\x12 .allego.SetKpiEventWindowRequest\x1a\x15.allego.StandardReply\"\x00\x12U\n\x10SpikesSaveToFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1d.allego.DataSourceFileSetStat\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12g\n\x14SpikesGetSpikesDense\x12$.allego.BiointerfaceGetSpikesRequest\x1a\'.allego.BiointerfaceSpikeDataDenseReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12p\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x15.allego.StandardReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\xf9\x06\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x65\n\x17SpikeSorterGetDashboard\x12\".allego.SpikeSorterStandardRequest\x1a$.allego.SpikeSorterGetDashboardReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x32\xb7\x04\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec2\x96\x32\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12>\n\nInitialize\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0fGetHDSnapshotPy\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12+\n\x06GetPSD\x12\x12.allego.PSDRequest\x1a\x0b.allego.PSD\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12M\n\x11GetSelectorTables\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.SelectorTablesReply\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12P\n\x1aGetDataSourceKpiFileStatus\x12\x19.allego.DataSourceRequest\x1a\x15.allego.KpiFileStatus\"\x00\x12R\n\x1bGetDataSourceKpiFileStatus2\x12\x19.allego.DataSourceRequest\x1a\x16.allego.KpiFileStatus2\"\x00\x12\x46\n\x0eGetKpiMetadata\x12\x19.allego.DataSourceRequest\x1a\x17.allego.KpiFileMetadata\"\x00\x12?\n\x08KpiClear\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0cKpiCalculate\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x10SpikesSaveToFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1d.allego.DataSourceFileSetStat\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12[\n\x14SpikesGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12p\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x15.allego.StandardReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\xf9\x06\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x65\n\x17SpikeSorterGetDashboard\x12\".allego.SpikeSorterStandardRequest\x1a$.allego.SpikeSorterGetDashboardReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x32\xae\x01\n\nDashboards\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12L\n\x10\x43ommandDashboard\x12\x1f.allego.DashboardCommandRequest\x1a\x15.allego.StandardReply\"\x00\x32\xb7\x04\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'radiensserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _RADIENSHEALTHCHECKREQUEST._serialized_start=121
   _RADIENSHEALTHCHECKREQUEST._serialized_end=196
   _RADIENSHEALTHCHECKSPEC._serialized_start=198
   _RADIENSHEALTHCHECKSPEC._serialized_end=291
   _RADIENSCORE._serialized_start=294
-  _RADIENSCORE._serialized_end=6384
-  _RADIENSSPIKESORTER1._serialized_start=6387
-  _RADIENSSPIKESORTER1._serialized_end=7276
-  _RADIENSDEV1._serialized_start=7279
-  _RADIENSDEV1._serialized_end=7846
+  _RADIENSCORE._serialized_end=6716
+  _RADIENSSPIKESORTER1._serialized_start=6719
+  _RADIENSSPIKESORTER1._serialized_end=7608
+  _DASHBOARDS._serialized_start=7611
+  _DASHBOARDS._serialized_end=7785
+  _RADIENSDEV1._serialized_start=7788
+  _RADIENSDEV1._serialized_end=8355
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/radiens/grpc/radiensserver_pb2_grpc.py` & `radiens-1.0.5/radiens/grpc_radiens/radiensserver_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,19 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetSignalGroupIDs = channel.unary_unary(
                 '/allego.RadiensCore/GetSignalGroupIDs',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=common__pb2.GetSignalGroupIDsReply.FromString,
                 )
+        self.GetSorterIDMap = channel.unary_unary(
+                '/allego.RadiensCore/GetSorterIDMap',
+                request_serializer=common__pb2.StandardRequest.SerializeToString,
+                response_deserializer=common__pb2.GetSorterIDMapReply.FromString,
+                )
         self.GetSpikeSorterIDs = channel.unary_unary(
                 '/allego.RadiensCore/GetSpikeSorterIDs',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.GetSpikeSorterIDsReply.FromString,
                 )
         self.GetSignalGroup = channel.unary_unary(
                 '/allego.RadiensCore/GetSignalGroup',
@@ -185,29 +190,44 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SetDACOff = channel.unary_unary(
                 '/allego.RadiensCore/SetDACOff',
                 request_serializer=common__pb2.DACOffRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
+        self.GetHDSnapshotPy = channel.unary_unary(
+                '/allego.RadiensCore/GetHDSnapshotPy',
+                request_serializer=common__pb2.HDSnapshotRequest2.SerializeToString,
+                response_deserializer=common__pb2.HDSnapshot2.FromString,
+                )
         self.GetHDSnapshot = channel.unary_unary(
                 '/allego.RadiensCore/GetHDSnapshot',
                 request_serializer=common__pb2.HDSnapshotRequest.SerializeToString,
                 response_deserializer=common__pb2.HDSnapshot.FromString,
                 )
+        self.GetPSD = channel.unary_unary(
+                '/allego.RadiensCore/GetPSD',
+                request_serializer=common__pb2.PSDRequest.SerializeToString,
+                response_deserializer=common__pb2.PSD.FromString,
+                )
         self.SetDSPGroup = channel.unary_unary(
                 '/allego.RadiensCore/SetDSPGroup',
                 request_serializer=common__pb2.SetDSPGroupRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetDSPGroup = channel.unary_unary(
                 '/allego.RadiensCore/GetDSPGroup',
                 request_serializer=common__pb2.SignalGroupIDRequest.SerializeToString,
                 response_deserializer=common__pb2.DSPGroup.FromString,
                 )
+        self.GetSelectorTables = channel.unary_unary(
+                '/allego.RadiensCore/GetSelectorTables',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=common__pb2.SelectorTablesReply.FromString,
+                )
         self.ListDataSource = channel.unary_unary(
                 '/allego.RadiensCore/ListDataSource',
                 request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
                 response_deserializer=datasource__pb2.DataSourceStatusMap.FromString,
                 )
         self.ListDataSourceIDs = channel.unary_unary(
                 '/allego.RadiensCore/ListDataSourceIDs',
@@ -225,58 +245,63 @@
                 response_deserializer=datasource__pb2.DataSourceIDReply.FromString,
                 )
         self.RenameDataSource = channel.unary_unary(
                 '/allego.RadiensCore/RenameDataSource',
                 request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
                 response_deserializer=datasource__pb2.DataSourceIDReply.FromString,
                 )
+        self.GetDataSourceKpiFileStatus = channel.unary_unary(
+                '/allego.RadiensCore/GetDataSourceKpiFileStatus',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=common__pb2.KpiFileStatus.FromString,
+                )
+        self.GetDataSourceKpiFileStatus2 = channel.unary_unary(
+                '/allego.RadiensCore/GetDataSourceKpiFileStatus2',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=common__pb2.KpiFileStatus2.FromString,
+                )
+        self.GetKpiMetadata = channel.unary_unary(
+                '/allego.RadiensCore/GetKpiMetadata',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=common__pb2.KpiFileMetadata.FromString,
+                )
         self.KpiClear = channel.unary_unary(
                 '/allego.RadiensCore/KpiClear',
-                request_serializer=common__pb2.KpiControlRequest.SerializeToString,
+                request_serializer=common__pb2.KpiStandardRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.KpiCalculate = channel.unary_unary(
                 '/allego.RadiensCore/KpiCalculate',
-                request_serializer=common__pb2.KpiControlRequest.SerializeToString,
+                request_serializer=common__pb2.KpiStandardRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.GetKpiStatus = channel.unary_unary(
                 '/allego.RadiensCore/GetKpiStatus',
                 request_serializer=common__pb2.GetKpiStatusRequest.SerializeToString,
                 response_deserializer=common__pb2.KpiStatusReply.FromString,
                 )
         self.KpiGetMetrics = channel.unary_unary(
                 '/allego.RadiensCore/KpiGetMetrics',
                 request_serializer=common__pb2.KpiMetricsReq.SerializeToString,
                 response_deserializer=common__pb2.KpiBundlePacketMetrics.FromString,
                 )
-        self.SetKpiUpdatePeriod = channel.unary_unary(
-                '/allego.RadiensCore/SetKpiUpdatePeriod',
-                request_serializer=common__pb2.SetKpiUpdatePeriodRequest.SerializeToString,
-                response_deserializer=common__pb2.StandardReply.FromString,
-                )
-        self.SetKpiThreshold = channel.unary_unary(
-                '/allego.RadiensCore/SetKpiThreshold',
-                request_serializer=common__pb2.SetKpiThresholdRequest.SerializeToString,
-                response_deserializer=common__pb2.StandardReply.FromString,
-                )
-        self.SetKpiEventDetect = channel.unary_unary(
-                '/allego.RadiensCore/SetKpiEventDetect',
-                request_serializer=common__pb2.SetKpiEventDetectRequest.SerializeToString,
+        self.SetKpiPacketDur = channel.unary_unary(
+                '/allego.RadiensCore/SetKpiPacketDur',
+                request_serializer=common__pb2.SetKpiParamRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
-        self.SetKpiEventShadow = channel.unary_unary(
-                '/allego.RadiensCore/SetKpiEventShadow',
-                request_serializer=common__pb2.SetKpiEventShadowRequest.SerializeToString,
+        self.SetKpiParam = channel.unary_unary(
+                '/allego.RadiensCore/SetKpiParam',
+                request_serializer=common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
-        self.SetKpiEventWindow = channel.unary_unary(
-                '/allego.RadiensCore/SetKpiEventWindow',
-                request_serializer=common__pb2.SetKpiEventWindowRequest.SerializeToString,
-                response_deserializer=common__pb2.StandardReply.FromString,
+        self.GetKpiParam = channel.unary_unary(
+                '/allego.RadiensCore/GetKpiParam',
+                request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
+                response_deserializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.FromString,
                 )
         self.SpikesSaveToFile = channel.unary_unary(
                 '/allego.RadiensCore/SpikesSaveToFile',
                 request_serializer=datasource__pb2.DataSourceSetSaveRequest.SerializeToString,
                 response_deserializer=datasource__pb2.DataSourceFileSetStat.FromString,
                 )
         self.SpikesSetFromFile = channel.unary_unary(
@@ -307,16 +332,16 @@
         self.SpikesGetRasterData = channel.unary_unary(
                 '/allego.RadiensCore/SpikesGetRasterData',
                 request_serializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.SpikeSorterRasterDataReply.FromString,
                 )
         self.SpikesGetSpikesDense = channel.unary_unary(
                 '/allego.RadiensCore/SpikesGetSpikesDense',
-                request_serializer=biointerface__pb2.BiointerfaceGetSpikesRequest.SerializeToString,
-                response_deserializer=biointerface__pb2.BiointerfaceSpikeDataDenseReply.FromString,
+                request_serializer=biointerface__pb2.SpikesGetSpikesRequest.SerializeToString,
+                response_deserializer=biointerface__pb2.SpikesSpikeDataDenseReply.FromString,
                 )
         self.SpikesDeleteIDs = channel.unary_unary(
                 '/allego.RadiensCore/SpikesDeleteIDs',
                 request_serializer=datasource__pb2.DataSourceRequest.SerializeToString,
                 response_deserializer=datasource__pb2.DataSourceIDReply.FromString,
                 )
         self.BiointerfaceGetNeurons = channel.unary_unary(
@@ -600,14 +625,20 @@
 
     def GetSignalGroupIDs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetSorterIDMap(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetSpikeSorterIDs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSignalGroup(self, request, context):
@@ -636,32 +667,50 @@
 
     def SetDACOff(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetHDSnapshotPy(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetHDSnapshot(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetPSD(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SetDSPGroup(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetDSPGroup(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetSelectorTables(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListDataSource(self, request, context):
         """data source functions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -685,64 +734,70 @@
 
     def RenameDataSource(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def KpiClear(self, request, context):
-        """time series data source KPI functions
-        """
+    def GetDataSourceKpiFileStatus(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def KpiCalculate(self, request, context):
+    def GetDataSourceKpiFileStatus2(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetKpiStatus(self, request, context):
+    def GetKpiMetadata(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def KpiGetMetrics(self, request, context):
+    def KpiClear(self, request, context):
+        """time series data source KPI functions
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def KpiCalculate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetKpiUpdatePeriod(self, request, context):
+    def GetKpiStatus(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetKpiThreshold(self, request, context):
+    def KpiGetMetrics(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetKpiEventDetect(self, request, context):
+    def SetKpiPacketDur(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetKpiEventShadow(self, request, context):
+    def SetKpiParam(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetKpiEventWindow(self, request, context):
+    def GetKpiParam(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SpikesSaveToFile(self, request, context):
         """===================
@@ -1055,14 +1110,19 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetSignalGroupIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSignalGroupIDs,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=common__pb2.GetSignalGroupIDsReply.SerializeToString,
             ),
+            'GetSorterIDMap': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSorterIDMap,
+                    request_deserializer=common__pb2.StandardRequest.FromString,
+                    response_serializer=common__pb2.GetSorterIDMapReply.SerializeToString,
+            ),
             'GetSpikeSorterIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSpikeSorterIDs,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=spikesorter__pb2.GetSpikeSorterIDsReply.SerializeToString,
             ),
             'GetSignalGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSignalGroup,
@@ -1085,29 +1145,44 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SetDACOff': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDACOff,
                     request_deserializer=common__pb2.DACOffRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
+            'GetHDSnapshotPy': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetHDSnapshotPy,
+                    request_deserializer=common__pb2.HDSnapshotRequest2.FromString,
+                    response_serializer=common__pb2.HDSnapshot2.SerializeToString,
+            ),
             'GetHDSnapshot': grpc.unary_unary_rpc_method_handler(
                     servicer.GetHDSnapshot,
                     request_deserializer=common__pb2.HDSnapshotRequest.FromString,
                     response_serializer=common__pb2.HDSnapshot.SerializeToString,
             ),
+            'GetPSD': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPSD,
+                    request_deserializer=common__pb2.PSDRequest.FromString,
+                    response_serializer=common__pb2.PSD.SerializeToString,
+            ),
             'SetDSPGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDSPGroup,
                     request_deserializer=common__pb2.SetDSPGroupRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetDSPGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.GetDSPGroup,
                     request_deserializer=common__pb2.SignalGroupIDRequest.FromString,
                     response_serializer=common__pb2.DSPGroup.SerializeToString,
             ),
+            'GetSelectorTables': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSelectorTables,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=common__pb2.SelectorTablesReply.SerializeToString,
+            ),
             'ListDataSource': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDataSource,
                     request_deserializer=datasource__pb2.DataSourceRequest.FromString,
                     response_serializer=datasource__pb2.DataSourceStatusMap.SerializeToString,
             ),
             'ListDataSourceIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDataSourceIDs,
@@ -1125,58 +1200,63 @@
                     response_serializer=datasource__pb2.DataSourceIDReply.SerializeToString,
             ),
             'RenameDataSource': grpc.unary_unary_rpc_method_handler(
                     servicer.RenameDataSource,
                     request_deserializer=datasource__pb2.DataSourceRequest.FromString,
                     response_serializer=datasource__pb2.DataSourceIDReply.SerializeToString,
             ),
+            'GetDataSourceKpiFileStatus': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDataSourceKpiFileStatus,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=common__pb2.KpiFileStatus.SerializeToString,
+            ),
+            'GetDataSourceKpiFileStatus2': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDataSourceKpiFileStatus2,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=common__pb2.KpiFileStatus2.SerializeToString,
+            ),
+            'GetKpiMetadata': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKpiMetadata,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=common__pb2.KpiFileMetadata.SerializeToString,
+            ),
             'KpiClear': grpc.unary_unary_rpc_method_handler(
                     servicer.KpiClear,
-                    request_deserializer=common__pb2.KpiControlRequest.FromString,
+                    request_deserializer=common__pb2.KpiStandardRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'KpiCalculate': grpc.unary_unary_rpc_method_handler(
                     servicer.KpiCalculate,
-                    request_deserializer=common__pb2.KpiControlRequest.FromString,
+                    request_deserializer=common__pb2.KpiStandardRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'GetKpiStatus': grpc.unary_unary_rpc_method_handler(
                     servicer.GetKpiStatus,
                     request_deserializer=common__pb2.GetKpiStatusRequest.FromString,
                     response_serializer=common__pb2.KpiStatusReply.SerializeToString,
             ),
             'KpiGetMetrics': grpc.unary_unary_rpc_method_handler(
                     servicer.KpiGetMetrics,
                     request_deserializer=common__pb2.KpiMetricsReq.FromString,
                     response_serializer=common__pb2.KpiBundlePacketMetrics.SerializeToString,
             ),
-            'SetKpiUpdatePeriod': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetKpiUpdatePeriod,
-                    request_deserializer=common__pb2.SetKpiUpdatePeriodRequest.FromString,
-                    response_serializer=common__pb2.StandardReply.SerializeToString,
-            ),
-            'SetKpiThreshold': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetKpiThreshold,
-                    request_deserializer=common__pb2.SetKpiThresholdRequest.FromString,
-                    response_serializer=common__pb2.StandardReply.SerializeToString,
-            ),
-            'SetKpiEventDetect': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetKpiEventDetect,
-                    request_deserializer=common__pb2.SetKpiEventDetectRequest.FromString,
+            'SetKpiPacketDur': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetKpiPacketDur,
+                    request_deserializer=common__pb2.SetKpiParamRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
-            'SetKpiEventShadow': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetKpiEventShadow,
-                    request_deserializer=common__pb2.SetKpiEventShadowRequest.FromString,
+            'SetKpiParam': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetKpiParam,
+                    request_deserializer=common__pb2.SpikeSorterSetParamsRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
-            'SetKpiEventWindow': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetKpiEventWindow,
-                    request_deserializer=common__pb2.SetKpiEventWindowRequest.FromString,
-                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            'GetKpiParam': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKpiParam,
+                    request_deserializer=datasource__pb2.DataSourceRequest.FromString,
+                    response_serializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.SerializeToString,
             ),
             'SpikesSaveToFile': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikesSaveToFile,
                     request_deserializer=datasource__pb2.DataSourceSetSaveRequest.FromString,
                     response_serializer=datasource__pb2.DataSourceFileSetStat.SerializeToString,
             ),
             'SpikesSetFromFile': grpc.unary_unary_rpc_method_handler(
@@ -1207,16 +1287,16 @@
             'SpikesGetRasterData': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikesGetRasterData,
                     request_deserializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.FromString,
                     response_serializer=spikesorter__pb2.SpikeSorterRasterDataReply.SerializeToString,
             ),
             'SpikesGetSpikesDense': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikesGetSpikesDense,
-                    request_deserializer=biointerface__pb2.BiointerfaceGetSpikesRequest.FromString,
-                    response_serializer=biointerface__pb2.BiointerfaceSpikeDataDenseReply.SerializeToString,
+                    request_deserializer=biointerface__pb2.SpikesGetSpikesRequest.FromString,
+                    response_serializer=biointerface__pb2.SpikesSpikeDataDenseReply.SerializeToString,
             ),
             'SpikesDeleteIDs': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikesDeleteIDs,
                     request_deserializer=datasource__pb2.DataSourceRequest.FromString,
                     response_serializer=datasource__pb2.DataSourceIDReply.SerializeToString,
             ),
             'BiointerfaceGetNeurons': grpc.unary_unary_rpc_method_handler(
@@ -1792,14 +1872,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetSignalGroupIDs',
             common__pb2.StandardRequest.SerializeToString,
             common__pb2.GetSignalGroupIDsReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetSorterIDMap(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetSorterIDMap',
+            common__pb2.StandardRequest.SerializeToString,
+            common__pb2.GetSorterIDMapReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetSpikeSorterIDs(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1894,14 +1991,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetDACOff',
             common__pb2.DACOffRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetHDSnapshotPy(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetHDSnapshotPy',
+            common__pb2.HDSnapshotRequest2.SerializeToString,
+            common__pb2.HDSnapshot2.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetHDSnapshot(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1911,14 +2025,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetHDSnapshot',
             common__pb2.HDSnapshotRequest.SerializeToString,
             common__pb2.HDSnapshot.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetPSD(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetPSD',
+            common__pb2.PSDRequest.SerializeToString,
+            common__pb2.PSD.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SetDSPGroup(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1945,14 +2076,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetDSPGroup',
             common__pb2.SignalGroupIDRequest.SerializeToString,
             common__pb2.DSPGroup.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetSelectorTables(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetSelectorTables',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            common__pb2.SelectorTablesReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListDataSource(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2030,167 +2178,184 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/RenameDataSource',
             datasource__pb2.DataSourceRequest.SerializeToString,
             datasource__pb2.DataSourceIDReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def KpiClear(request,
+    def GetDataSourceKpiFileStatus(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiClear',
-            common__pb2.KpiControlRequest.SerializeToString,
-            common__pb2.StandardReply.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetDataSourceKpiFileStatus',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            common__pb2.KpiFileStatus.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def KpiCalculate(request,
+    def GetDataSourceKpiFileStatus2(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiCalculate',
-            common__pb2.KpiControlRequest.SerializeToString,
-            common__pb2.StandardReply.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetDataSourceKpiFileStatus2',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            common__pb2.KpiFileStatus2.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetKpiStatus(request,
+    def GetKpiMetadata(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetKpiStatus',
-            common__pb2.GetKpiStatusRequest.SerializeToString,
-            common__pb2.KpiStatusReply.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetKpiMetadata',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            common__pb2.KpiFileMetadata.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def KpiGetMetrics(request,
+    def KpiClear(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiGetMetrics',
-            common__pb2.KpiMetricsReq.SerializeToString,
-            common__pb2.KpiBundlePacketMetrics.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiClear',
+            common__pb2.KpiStandardRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetKpiUpdatePeriod(request,
+    def KpiCalculate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiUpdatePeriod',
-            common__pb2.SetKpiUpdatePeriodRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiCalculate',
+            common__pb2.KpiStandardRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetKpiThreshold(request,
+    def GetKpiStatus(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiThreshold',
-            common__pb2.SetKpiThresholdRequest.SerializeToString,
-            common__pb2.StandardReply.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetKpiStatus',
+            common__pb2.GetKpiStatusRequest.SerializeToString,
+            common__pb2.KpiStatusReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetKpiEventDetect(request,
+    def KpiGetMetrics(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiEventDetect',
-            common__pb2.SetKpiEventDetectRequest.SerializeToString,
-            common__pb2.StandardReply.FromString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/KpiGetMetrics',
+            common__pb2.KpiMetricsReq.SerializeToString,
+            common__pb2.KpiBundlePacketMetrics.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetKpiEventShadow(request,
+    def SetKpiPacketDur(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiEventShadow',
-            common__pb2.SetKpiEventShadowRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiPacketDur',
+            common__pb2.SetKpiParamRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetKpiEventWindow(request,
+    def SetKpiParam(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiEventWindow',
-            common__pb2.SetKpiEventWindowRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SetKpiParam',
+            common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetKpiParam(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/GetKpiParam',
+            datasource__pb2.DataSourceRequest.SerializeToString,
+            spikesorter__pb2.GetSpikeSorterParamCommandReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SpikesSaveToFile(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2313,16 +2478,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensCore/SpikesGetSpikesDense',
-            biointerface__pb2.BiointerfaceGetSpikesRequest.SerializeToString,
-            biointerface__pb2.BiointerfaceSpikeDataDenseReply.FromString,
+            biointerface__pb2.SpikesGetSpikesRequest.SerializeToString,
+            biointerface__pb2.SpikesSpikeDataDenseReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SpikesDeleteIDs(request,
             target,
             options=(),
@@ -3003,14 +3168,108 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikesGetSpec',
             spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
             biointerface__pb2.SpikesSpecReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
+class DashboardsStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.Healthcheck = channel.unary_unary(
+                '/allego.Dashboards/Healthcheck',
+                request_serializer=radiensserver__pb2.RadiensHealthcheckRequest.SerializeToString,
+                response_deserializer=radiensserver__pb2.RadiensHealthcheckSpec.FromString,
+                )
+        self.CommandDashboard = channel.unary_unary(
+                '/allego.Dashboards/CommandDashboard',
+                request_serializer=common__pb2.DashboardCommandRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
+
+
+class DashboardsServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def Healthcheck(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CommandDashboard(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_DashboardsServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'Healthcheck': grpc.unary_unary_rpc_method_handler(
+                    servicer.Healthcheck,
+                    request_deserializer=radiensserver__pb2.RadiensHealthcheckRequest.FromString,
+                    response_serializer=radiensserver__pb2.RadiensHealthcheckSpec.SerializeToString,
+            ),
+            'CommandDashboard': grpc.unary_unary_rpc_method_handler(
+                    servicer.CommandDashboard,
+                    request_deserializer=common__pb2.DashboardCommandRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'allego.Dashboards', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class Dashboards(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def Healthcheck(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Dashboards/Healthcheck',
+            radiensserver__pb2.RadiensHealthcheckRequest.SerializeToString,
+            radiensserver__pb2.RadiensHealthcheckSpec.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CommandDashboard(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Dashboards/CommandDashboard',
+            common__pb2.DashboardCommandRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
 class RadiensDev1Stub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
```

### Comparing `radiens-1.0.4/radiens/grpc/spikesorter_pb2.py` & `radiens-1.0.5/radiens/grpc_radiens/spikesorter_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import biointerface_pb2 as biointerface__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11spikesorter.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x12\x62iointerface.proto\"\x84\x02\n\x18SpikeSorterLaunchRequest\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12&\n\x06source\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptor\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x01(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x01(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12%\n\x04mode\x18\x07 \x01(\x0e\x32\x17.allego.SpikeSorterMode\x12\x0c\n\x04seed\x18\x08 \x01(\x03\x12\x10\n\x08isAutoOn\x18\t \x01(\x08\"\x8a\x01\n\x19SpikeSorterCommandRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\'\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1a.allego.SpikeSorterCommand\x12-\n\x06subCmd\x18\x03 \x02(\x0e\x32\x1d.allego.SpikeSorterSubCommand\"\xcf\x01\n\x10SpikeSorterState\x12+\n\x03sys\x18\x01 \x02(\x0e\x32\x1e.allego.SpikeSorterStateSystem\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\x12\n\nlaunchTime\x18\x04 \x01(\t\x12\x16\n\x0einitializeTime\x18\x05 \x01(\t\x12\x18\n\x10sessionStartTime\x18\x06 \x01(\t\x12\x17\n\x0fsessionStopTime\x18\x07 \x01(\t\x12\x0c\n\x04isOn\x18\x08 \x01(\x08\"\x81\x01\n\x0cSpkSortIOreq\x12#\n\x04type\x18\x01 \x02(\x0e\x32\x15.allego.SpkSortIOtype\x12\'\n\x06target\x18\x02 \x02(\x0e\x32\x17.allego.SpkSortIOtarget\x12#\n\x04mode\x18\x03 \x02(\x0e\x32\x15.allego.SpkSortIOmode\"i\n\x16SpikeSorterLaunchReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x0b\n\x03msg\x18\x03 \x01(\t\"0\n\x16GetSpikeSorterIDsReply\x12\x16\n\x0espikeSorterIDs\x18\x01 \x03(\t\"\xa1\x01\n\x1fSpikeSorterGetRasterDataRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x12\n\ntimeWindow\x18\x03 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x04 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x05 \x02(\t\x12\x11\n\ttimeRange\x18\x06 \x03(\x01\"\xaa\x01\n\x1aSpikeSorterRasterDataReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\x12\x10\n\x08GPIOData\x18\x05 \x02(\x0c\x12\x11\n\tGPIOShape\x18\x06 \x03(\x05\"3\n\x1aSpikeSorterStandardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\"\x86\x03\n\x12SpikeSorterDynamic\x12\x11\n\tisEnabled\x18\x01 \x01(\x08\x12\x43\n\x0fupdatePeriodSec\x18\x02 \x01(\x0b\x32*.allego.SpikeSorterDynamic.UpdatePeriodSec\x12\x35\n\x08\x63riteria\x18\x03 \x01(\x0b\x32#.allego.SpikeSorterDynamic.Criteria\x1a\xa0\x01\n\x08\x43riteria\x12\x31\n\x06\x64\x65tect\x18\x01 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12\x30\n\x05train\x18\x02 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12/\n\x04sort\x18\x03 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x1a>\n\x0fUpdatePeriodSec\x12\x0e\n\x06\x64\x65tect\x18\x01 \x01(\x01\x12\r\n\x05train\x18\x02 \x01(\x01\x12\x0c\n\x04sort\x18\x03 \x01(\x01\"\xc5\x01\n\x1cSpikeSorterSetDynamicRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x42\n\x07variant\x18\x02 \x03(\x0b\x32\x31.allego.SpikeSorterSetDynamicRequest.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"\xd8\x01\n\x1aSpikeSorterGetDynamicReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x15\n\rrootVariantID\x18\x02 \x02(\t\x12@\n\x07variant\x18\x03 \x03(\x0b\x32/.allego.SpikeSorterGetDynamicReply.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"l\n\x1fGetSpikeSorterParamCommandReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x32\n\x03rec\x18\x02 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"3\n\x12\x43lusterMapOutliers\x12\x0c\n\x04mild\x18\x01 \x03(\x01\x12\x0f\n\x07\x65xtreme\x18\x02 \x03(\x01\"9\n\x13\x43lusterMapQuartiles\x12\n\n\x02q1\x18\x01 \x02(\x01\x12\n\n\x02q2\x18\x02 \x02(\x01\x12\n\n\x02q3\x18\x03 \x02(\x01\"\x83\x01\n\x0f\x43lusterMapStats\x12\x16\n\x0e\x63\x65ntroidCenter\x18\x01 \x03(\x01\x12\x12\n\ncentroidSd\x18\x02 \x03(\x01\x12\x16\n\x0e\x63\x65ntroidSdNorm\x18\x03 \x02(\x01\x12\x19\n\x11intraCentroidDist\x18\x04 \x03(\x01\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\"f\n\x10\x43lusterMapRecord\x12\r\n\x05label\x18\x01 \x02(\x05\x12&\n\x05stats\x18\x03 \x02(\x0b\x32\x17.allego.ClusterMapStats\x12\x1b\n\x13numSpikesTrainCache\x18\x04 \x02(\x03\"\xa8\x01\n\x13SpikeSortSiteStatus\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x15\n\rorderedLabels\x18\x02 \x03(\x05\x12)\n\x07\x63luster\x18\x03 \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x11\n\tnumSpikes\x18\x04 \x03(\x03\x12\x0c\n\x04zeta\x18\x05 \x03(\x01\x12\x1a\n\x12\x61ggregateSpikeRate\x18\x06 \x02(\x01\"\x8f\x01\n\x14SpikeSortPhaseStatus\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\nchunkIndex\x18\x02 \x02(\x03\x12\x14\n\x0cupdatePeriod\x18\x03 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x04 \x02(\x01\x12\x12\n\nisComplete\x18\x05 \x02(\x08\x12\x18\n\x10\x66ractionComplete\x18\x06 \x02(\x01\"*\n\x13SpikeSortNbrIdxList\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\xf2\x02\n\x16SpikeSorterStatusReply\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x10\n\x08sampFreq\x18\x05 \x02(\x01\x12\x19\n\x11\x65nabledNtvChanIdx\x18\x06 \x03(\x05\x12+\n\x05phase\x18\x07 \x03(\x0b\x32\x1c.allego.SpikeSortPhaseStatus\x12\x30\n\x0b\x65nabledSite\x18\x08 \x03(\x0b\x32\x1b.allego.SpikeSortSiteStatus\x12\x12\n\nprobeYield\x18\t \x02(\x01\x12\x11\n\tsortStats\x18\n \x03(\x01\x12\x1b\n\x13\x64\x61tasourceTimeRange\x18\x0c \x03(\x01\x12\x1d\n\x15\x62iointerfaceTimeRange\x18\r \x03(\x01\x12\x12\n\nnumNeurons\x18\x0f \x02(\x03\"R\n\x1eSpikeSorterStatusVariantsReply\x12\x30\n\x08variants\x18\x01 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\xfd\x02\n\x19SpikeSorterClassifierSpec\x12\r\n\x05\x61lpha\x18\x01 \x02(\x01\x12\x11\n\talphaBias\x18\x02 \x02(\x01\x12\x16\n\x0e\x64imOutputLayer\x18\x03 \x02(\x05\x12\x16\n\x0e\x65rrorTolerance\x18\x04 \x02(\x01\x12\x19\n\x11hiddenLayerFactor\x18\x05 \x02(\x01\x12\n\n\x02iD\x18\x06 \x02(\t\x12\x16\n\x0einitBiasStdDev\x18\x07 \x02(\x01\x12\x18\n\x10initWeightStdDev\x18\x08 \x02(\x01\x12\x11\n\tisMasking\x18\t \x02(\x08\x12\x10\n\x08l1lambda\x18\n \x02(\x01\x12\x15\n\rminibatchSize\x18\x0b \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x0c \x02(\x05\x12\x11\n\tnumEpochs\x18\r \x02(\x05\x12\x19\n\x11numSamplesTestMSE\x18\x0e \x02(\x05\x12\x1b\n\x13numConcurrentModels\x18\x0f \x02(\x05\x12\x17\n\x0flabelNoiseLevel\x18\x10 \x02(\x01\"u\n\x16SpikeSorterVariantSpec\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x14\n\x0csiteConfigID\x18\x02 \x02(\t\x12\x39\n\x0e\x63lassifierSpec\x18\x03 \x02(\x0b\x32!.allego.SpikeSorterClassifierSpec\"\xcc\x01\n\x0fSpikeSorterSpec\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x02 \x02(\t\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x02(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x02(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12\x0c\n\x04seed\x18\x08 \x02(\x03\"\xc2\x01\n\x19SpikeSorterGetConfigReply\x12%\n\x04spec\x18\x01 \x02(\x0b\x32\x17.allego.SpikeSorterSpec\x12\x16\n\x0e\x61IupdatePeriod\x18\x02 \x02(\x01\x12\x19\n\x11orderedVariantIDs\x18\x03 \x03(\t\x12\x15\n\rrootVariantID\x18\x04 \x02(\t\x12\x34\n\x0csorterStatus\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\x90\x02\n\x15SpikeSorterVizRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\tvariantID\x18\x02 \x02(\t\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x13\n\x0bspikeLabels\x18\x04 \x03(\x05\x12\x34\n\x07vizType\x18\x05 \x02(\x0e\x32#.allego.SpikeSorterVizRequest.VType\x12\x14\n\x0cisYAutoScale\x18\x06 \x02(\x08\x12\x0c\n\x04yLim\x18\x07 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x08 \x02(\t\x12\x11\n\tnumSpikes\x18\t \x02(\x05\"\'\n\x05VType\x12\x1e\n\x1aVIZ_SPIKESORT_TRAIN_SPIKES\x10\x00\"\xc2\x05\n\x1cSpikeSorterGetDashboardReply\x12\"\n\x0c\x65nabledPorts\x18\x01 \x03(\x0e\x32\x0c.allego.Port\x12\x37\n\x07general\x18\x02 \x02(\x0b\x32&.allego.SpikeSorterDashboardGeneralRec\x12\x33\n\tsiteStats\x18\x03 \x02(\x0b\x32 .allego.IndicoDashboardSiteStats\x12\x46\n\tportStats\x18\x04 \x03(\x0b\x32\x33.allego.SpikeSorterGetDashboardReply.PortStatsEntry\x12\x46\n\tsitePanel\x18\x05 \x03(\x0b\x32\x33.allego.SpikeSorterGetDashboardReply.SitePanelEntry\x12J\n\x0bneuronPanel\x18\x06 \x03(\x0b\x32\x35.allego.SpikeSorterGetDashboardReply.NeuronPanelEntry\x12*\n\x02\x61I\x18\x07 \x01(\x0b\x32\x1e.allego.SpikeSorterDashboardAI\x1aR\n\x0ePortStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .allego.IndicoDashboardPortStats:\x02\x38\x01\x1aW\n\x0eSitePanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.allego.IndicoDashboardSiteIndicators:\x02\x38\x01\x1a[\n\x10NeuronPanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.allego.IndicoDashboardNeuronIndicators:\x02\x38\x01\"\xac\x03\n\x1eSpikeSorterDashboardGeneralRec\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x10\n\x08sorterID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\x12\x15\n\rnumTotalSites\x18\x06 \x02(\x03\x12\x17\n\x0fnumEnabledSites\x18\x07 \x02(\x03\x12\x16\n\x0enumActiveSites\x18\x08 \x02(\x03\x12\x12\n\nnumNeurons\x18\t \x02(\x03\x12\x12\n\nprobeYield\x18\n \x02(\x01\x12\x11\n\tsiteYield\x18\x0b \x02(\x01\x12\x1a\n\x12numSpikesProcessed\x18\x0c \x02(\x03\x12\x18\n\x10numSpikesLabeled\x18\r \x02(\x03\x12\x16\n\x0esortEfficiency\x18\x0e \x02(\x01\x12(\n\x08sinkDesc\x18\x0f \x02(\x0b\x32\x16.allego.FileDescriptor\"\xd5\x01\n\x16SpikeSorterDashboardAI\x12\x0c\n\x04\x62\x65ta\x18\x01 \x02(\x01\x12\"\n\x1a\x65stimatedReaderCompleteSec\x18\x02 \x02(\x01\x12\x1a\n\x12interSessionDurSec\x18\x03 \x02(\x01\x12\x19\n\x11interSessionStart\x18\x04 \x02(\t\x12\x15\n\rsessionDurSec\x18\x05 \x02(\x01\x12\x14\n\x0csessionStart\x18\x06 \x02(\t\x12\x12\n\nsessionIdx\x18\x07 \x02(\x03\x12\x11\n\tstartTime\x18\x08 \x02(\t\"_\n\x18IndicoDashboardSiteStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x12\n\nnumNeurons\x18\x04 \x02(\x03\"\x90\x01\n\x18IndicoDashboardPortStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x04 \x02(\x01\x12\x17\n\x0fnumEnabledSites\x18\x05 \x02(\x03\x12\x12\n\nnumNeurons\x18\x06 \x02(\x03\"\xd9\x01\n\x1dIndicoDashboardSiteIndicators\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\r\n\x05noise\x18\x03 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x04 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x05 \x03(\x01\x12\x11\n\tspikeRate\x18\x06 \x03(\x01\x12\x11\n\tposProbeX\x18\x07 \x03(\x01\x12\x11\n\tposProbeY\x18\x08 \x03(\x01\x12\x11\n\tposProbeZ\x18\t \x03(\x01\x12\x0f\n\x07siteNum\x18\n \x03(\x05\"\xb1\x01\n\x1fIndicoDashboardNeuronIndicators\x12\x10\n\x08neuronID\x18\x01 \x03(\t\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\x11\n\tspikeRate\x18\x03 \x03(\x01\x12\x11\n\tposProbeX\x18\x04 \x03(\x01\x12\x11\n\tposProbeY\x18\x05 \x03(\x01\x12\x11\n\tposProbeZ\x18\x06 \x03(\x01\x12\x0f\n\x07siteNum\x18\x07 \x03(\x05\x12\x12\n\nspikeLabel\x18\x08 \x03(\x05\"\xa7\x02\n\x1cSpikeSorterDashboardSiteDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x10\n\x08posProbe\x18\x03 \x03(\x01\x12\x10\n\x08posBrain\x18\x04 \x03(\x01\x12\x0e\n\x06snrMax\x18\x05 \x02(\x01\x12\x0e\n\x06snrMin\x18\x06 \x02(\x01\x12\x12\n\nnoiseLevel\x18\x07 \x02(\x01\x12\x12\n\nnumNeurons\x18\x08 \x02(\x03\x12/\n\rindicoCluster\x18\n \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x1c\n\x14pileWaveformMinValue\x18\r \x02(\x02\x12\x1c\n\x14pileWaveformMaxValue\x18\x0e \x02(\x02\"\xd2\x01\n\x1eSpikeSorterDashboardNeuronDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12&\n\x04\x64\x65sc\x18\x02 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x0b\n\x03snr\x18\x05 \x02(\x01\x12\x0f\n\x07IsihMax\x18\x06 \x02(\x01\x12\x15\n\rIsihArgmaxSec\x18\x07 \x02(\x01\x12\x15\n\rIsihArgmaxIdx\x18\x08 \x02(\x03\x12\x10\n\x08IsihMean\x18\t \x02(\x01\x12\x0e\n\x06IsihSd\x18\n \x02(\x01\"\xfa\x01\n SpikeSorterDashboardNeuronDetail\x12&\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x18\n\x10templateWaveform\x18\x02 \x03(\x02\x12\x1a\n\x12templateSdWaveform\x18\x03 \x03(\x02\x12\x18\n\x10pileWaveformData\x18\x04 \x03(\x02\x12\x1e\n\x16numSamplesPileWaveform\x18\x05 \x02(\x05\x12\x18\n\x10numPileWaveforms\x18\x06 \x02(\x05\x12$\n\x04isih\x18\x0b \x02(\x0b\x32\x16.allego.NeuronHistData\"\xa9\x01\n\x1eSpikeSorterDashboardSiteDetail\x12\x32\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32$.allego.SpikeSorterDashboardSiteDesc\x12\x19\n\x11orderedSpikeLabel\x18\x02 \x03(\x05\x12\x38\n\x06neuron\x18\x03 \x03(\x0b\x32(.allego.SpikeSorterDashboardNeuronDetail*\x80\x01\n\x0fSpikeSorterType\x12\x0f\n\x0bSORTER_NULL\x10\x00\x12\x15\n\x11SORTER_VEX_STREAM\x10\x01\x12\x18\n\x14SORTER_SPIKES_STREAM\x10\x02\x12\x13\n\x0fSORTER_VEX_FILE\x10\x03\x12\x16\n\x12SORTER_SPIKES_FILE\x10\x04*\xb0\x01\n\x12SpikeSorterCommand\x12\x11\n\rSORTER_CMD_ON\x10\x00\x12\x12\n\x0eSORTER_CMD_OFF\x10\x01\x12\x19\n\x15SORTER_CMD_CLEAR_SORT\x10\x02\x12\x15\n\x11SORTER_CMD_REBASE\x10\x04\x12\x13\n\x0fSORTER_CMD_INIT\x10\x07\x12\x17\n\x13SORTER_CMD_LOCALIZE\x10\x08\x12\x13\n\x0fSORTER_CMD_SORT\x10\t*/\n\x15SpikeSorterSubCommand\x12\x16\n\x12SORTER_SUBCMD_NULL\x10\x00*@\n\x0fSpikeSorterMode\x12\x16\n\x12SORTER_MODE_STREAM\x10\x00\x12\x15\n\x11SORTER_MODE_BATCH\x10\x01*I\n\x16SpikeSorterStateSystem\x12\n\n\x06SYS_ON\x10\x00\x12\x0b\n\x07SYS_OFF\x10\x01\x12\x16\n\x12SYS_NOT_CONFIGURED\x10\x02*f\n\rSpkSortIOtype\x12\x17\n\x13SPK_SORT_IO_NETWORK\x10\x00\x12\x17\n\x13SPK_SORT_IO_TRAINER\x10\x01\x12#\n\x1fSPK_SORT_IO_NETWORK_AND_TRAINER\x10\x02*>\n\x0fSpkSortIOtarget\x12\x14\n\x10SPK_SORT_IO_FSYS\x10\x00\x12\x15\n\x11SPK_SORT_IO_CLOUD\x10\x01*;\n\rSpkSortIOmode\x12\x14\n\x10SPK_SORT_IO_SAVE\x10\x00\x12\x14\n\x10SPK_SORT_IO_LOAD\x10\x01*u\n\x19SpikeSorterCriterionLevel\x12\x10\n\x0cSORTER_LEAST\x10\x00\x12\x0f\n\x0bSORTER_LESS\x10\x01\x12\x13\n\x0fSORTER_BALANCED\x10\x02\x12\x0f\n\x0bSORTER_MORE\x10\x03\x12\x0f\n\x0bSORTER_MOST\x10\x04*\x84\x01\n\x07SS_STAT\x12\x08\n\x04MEAN\x10\x00\x12\x06\n\x02SD\x10\x01\x12\x08\n\x04MODE\x10\x02\x12\x07\n\x03MIN\x10\x03\x12\x07\n\x03MAX\x10\x04\x12\x0e\n\nMODE_COUNT\x10\x05\x12\n\n\x06MEDIAN\x10\x06\x12\x07\n\x03Q25\x10\x07\x12\x07\n\x03Q75\x10\x08\x12\x08\n\x04SKEW\x10\t\x12\x0c\n\x08KURTOSIS\x10\n\x12\x05\n\x01N\x10\x0b\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11spikesorter.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x12\x62iointerface.proto\"\xbc\x02\n\x18SpikeSorterLaunchRequest\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12&\n\x06source\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptor\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x01(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x01(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12%\n\x04mode\x18\x07 \x01(\x0e\x32\x17.allego.SpikeSorterMode\x12\x0c\n\x04seed\x18\x08 \x01(\x03\x12\x10\n\x08isAutoOn\x18\t \x01(\x08\x12\x12\n\nnbrPattern\x18\n \x01(\x05\x12\x11\n\tnetworkID\x18\x0b \x01(\t\x12\x0f\n\x07release\x18\x0c \x01(\x03\"\x8a\x01\n\x19SpikeSorterCommandRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\'\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1a.allego.SpikeSorterCommand\x12-\n\x06subCmd\x18\x03 \x02(\x0e\x32\x1d.allego.SpikeSorterSubCommand\"\x86\x02\n\x10SpikeSorterState\x12+\n\x03sys\x18\x01 \x02(\x0e\x32\x1e.allego.SpikeSorterStateSystem\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\x12\n\nlaunchTime\x18\x04 \x01(\t\x12\x16\n\x0einitializeTime\x18\x05 \x01(\t\x12\x18\n\x10sessionStartTime\x18\x06 \x01(\t\x12\x17\n\x0fsessionStopTime\x18\x07 \x01(\t\x12\x0c\n\x04isOn\x18\x08 \x01(\x08\x12\x1a\n\x12kernelErrorMessage\x18\t \x01(\t\x12\x19\n\x11kernelWarnMessage\x18\n \x01(\t\"\x81\x01\n\x0cSpkSortIOreq\x12#\n\x04type\x18\x01 \x02(\x0e\x32\x15.allego.SpkSortIOtype\x12\'\n\x06target\x18\x02 \x02(\x0e\x32\x17.allego.SpkSortIOtarget\x12#\n\x04mode\x18\x03 \x02(\x0e\x32\x15.allego.SpkSortIOmode\"i\n\x16SpikeSorterLaunchReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x0b\n\x03msg\x18\x03 \x01(\t\"0\n\x16GetSpikeSorterIDsReply\x12\x16\n\x0espikeSorterIDs\x18\x01 \x03(\t\"\xa1\x01\n\x1fSpikeSorterGetRasterDataRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x12\n\ntimeWindow\x18\x03 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x04 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x05 \x02(\t\x12\x11\n\ttimeRange\x18\x06 \x03(\x01\"\xaa\x01\n\x1aSpikeSorterRasterDataReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\x12\x10\n\x08GPIOData\x18\x05 \x02(\x0c\x12\x11\n\tGPIOShape\x18\x06 \x03(\x05\"3\n\x1aSpikeSorterStandardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\"\x86\x03\n\x12SpikeSorterDynamic\x12\x11\n\tisEnabled\x18\x01 \x01(\x08\x12\x43\n\x0fupdatePeriodSec\x18\x02 \x01(\x0b\x32*.allego.SpikeSorterDynamic.UpdatePeriodSec\x12\x35\n\x08\x63riteria\x18\x03 \x01(\x0b\x32#.allego.SpikeSorterDynamic.Criteria\x1a\xa0\x01\n\x08\x43riteria\x12\x31\n\x06\x64\x65tect\x18\x01 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12\x30\n\x05train\x18\x02 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12/\n\x04sort\x18\x03 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x1a>\n\x0fUpdatePeriodSec\x12\x0e\n\x06\x64\x65tect\x18\x01 \x01(\x01\x12\r\n\x05train\x18\x02 \x01(\x01\x12\x0c\n\x04sort\x18\x03 \x01(\x01\"\xc5\x01\n\x1cSpikeSorterSetDynamicRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x42\n\x07variant\x18\x02 \x03(\x0b\x32\x31.allego.SpikeSorterSetDynamicRequest.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"\xd8\x01\n\x1aSpikeSorterGetDynamicReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x15\n\rrootVariantID\x18\x02 \x02(\t\x12@\n\x07variant\x18\x03 \x03(\x0b\x32/.allego.SpikeSorterGetDynamicReply.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"l\n\x1fGetSpikeSorterParamCommandReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x32\n\x03rec\x18\x02 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"3\n\x12\x43lusterMapOutliers\x12\x0c\n\x04mild\x18\x01 \x03(\x01\x12\x0f\n\x07\x65xtreme\x18\x02 \x03(\x01\"9\n\x13\x43lusterMapQuartiles\x12\n\n\x02q1\x18\x01 \x02(\x01\x12\n\n\x02q2\x18\x02 \x02(\x01\x12\n\n\x02q3\x18\x03 \x02(\x01\"\x83\x01\n\x0f\x43lusterMapStats\x12\x16\n\x0e\x63\x65ntroidCenter\x18\x01 \x03(\x01\x12\x12\n\ncentroidSd\x18\x02 \x03(\x01\x12\x16\n\x0e\x63\x65ntroidSdNorm\x18\x03 \x02(\x01\x12\x19\n\x11intraCentroidDist\x18\x04 \x03(\x01\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\"f\n\x10\x43lusterMapRecord\x12\r\n\x05label\x18\x01 \x02(\x05\x12&\n\x05stats\x18\x03 \x02(\x0b\x32\x17.allego.ClusterMapStats\x12\x1b\n\x13numSpikesTrainCache\x18\x04 \x02(\x03\"\xa8\x01\n\x13SpikeSortSiteStatus\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x15\n\rorderedLabels\x18\x02 \x03(\x05\x12)\n\x07\x63luster\x18\x03 \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x11\n\tnumSpikes\x18\x04 \x03(\x03\x12\x0c\n\x04zeta\x18\x05 \x03(\x01\x12\x1a\n\x12\x61ggregateSpikeRate\x18\x06 \x02(\x01\"\x8f\x01\n\x14SpikeSortPhaseStatus\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\nchunkIndex\x18\x02 \x02(\x03\x12\x14\n\x0cupdatePeriod\x18\x03 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x04 \x02(\x01\x12\x12\n\nisComplete\x18\x05 \x02(\x08\x12\x18\n\x10\x66ractionComplete\x18\x06 \x02(\x01\"*\n\x13SpikeSortNbrIdxList\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\xf2\x02\n\x16SpikeSorterStatusReply\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x10\n\x08sampFreq\x18\x05 \x02(\x01\x12\x19\n\x11\x65nabledNtvChanIdx\x18\x06 \x03(\x05\x12+\n\x05phase\x18\x07 \x03(\x0b\x32\x1c.allego.SpikeSortPhaseStatus\x12\x30\n\x0b\x65nabledSite\x18\x08 \x03(\x0b\x32\x1b.allego.SpikeSortSiteStatus\x12\x12\n\nprobeYield\x18\t \x02(\x01\x12\x11\n\tsortStats\x18\n \x03(\x01\x12\x1b\n\x13\x64\x61tasourceTimeRange\x18\x0c \x03(\x01\x12\x1d\n\x15\x62iointerfaceTimeRange\x18\r \x03(\x01\x12\x12\n\nnumNeurons\x18\x0f \x02(\x03\"R\n\x1eSpikeSorterStatusVariantsReply\x12\x30\n\x08variants\x18\x01 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\xfd\x02\n\x19SpikeSorterClassifierSpec\x12\r\n\x05\x61lpha\x18\x01 \x02(\x01\x12\x11\n\talphaBias\x18\x02 \x02(\x01\x12\x16\n\x0e\x64imOutputLayer\x18\x03 \x02(\x05\x12\x16\n\x0e\x65rrorTolerance\x18\x04 \x02(\x01\x12\x19\n\x11hiddenLayerFactor\x18\x05 \x02(\x01\x12\n\n\x02iD\x18\x06 \x02(\t\x12\x16\n\x0einitBiasStdDev\x18\x07 \x02(\x01\x12\x18\n\x10initWeightStdDev\x18\x08 \x02(\x01\x12\x11\n\tisMasking\x18\t \x02(\x08\x12\x10\n\x08l1lambda\x18\n \x02(\x01\x12\x15\n\rminibatchSize\x18\x0b \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x0c \x02(\x05\x12\x11\n\tnumEpochs\x18\r \x02(\x05\x12\x19\n\x11numSamplesTestMSE\x18\x0e \x02(\x05\x12\x1b\n\x13numConcurrentModels\x18\x0f \x02(\x05\x12\x17\n\x0flabelNoiseLevel\x18\x10 \x02(\x01\"u\n\x16SpikeSorterVariantSpec\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x14\n\x0csiteConfigID\x18\x02 \x02(\t\x12\x39\n\x0e\x63lassifierSpec\x18\x03 \x02(\x0b\x32!.allego.SpikeSorterClassifierSpec\"\xcc\x01\n\x0fSpikeSorterSpec\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x02 \x02(\t\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x02(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x02(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12\x0c\n\x04seed\x18\x08 \x02(\x03\"\xc2\x01\n\x19SpikeSorterGetConfigReply\x12%\n\x04spec\x18\x01 \x02(\x0b\x32\x17.allego.SpikeSorterSpec\x12\x16\n\x0e\x61IupdatePeriod\x18\x02 \x02(\x01\x12\x19\n\x11orderedVariantIDs\x18\x03 \x03(\t\x12\x15\n\rrootVariantID\x18\x04 \x02(\t\x12\x34\n\x0csorterStatus\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\x90\x02\n\x15SpikeSorterVizRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\tvariantID\x18\x02 \x02(\t\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x13\n\x0bspikeLabels\x18\x04 \x03(\x05\x12\x34\n\x07vizType\x18\x05 \x02(\x0e\x32#.allego.SpikeSorterVizRequest.VType\x12\x14\n\x0cisYAutoScale\x18\x06 \x02(\x08\x12\x0c\n\x04yLim\x18\x07 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x08 \x02(\t\x12\x11\n\tnumSpikes\x18\t \x02(\x05\"\'\n\x05VType\x12\x1e\n\x1aVIZ_SPIKESORT_TRAIN_SPIKES\x10\x00\"\xc2\x05\n\x1cSpikeSorterGetDashboardReply\x12\"\n\x0c\x65nabledPorts\x18\x01 \x03(\x0e\x32\x0c.allego.Port\x12\x37\n\x07general\x18\x02 \x02(\x0b\x32&.allego.SpikeSorterDashboardGeneralRec\x12\x33\n\tsiteStats\x18\x03 \x02(\x0b\x32 .allego.IndicoDashboardSiteStats\x12\x46\n\tportStats\x18\x04 \x03(\x0b\x32\x33.allego.SpikeSorterGetDashboardReply.PortStatsEntry\x12\x46\n\tsitePanel\x18\x05 \x03(\x0b\x32\x33.allego.SpikeSorterGetDashboardReply.SitePanelEntry\x12J\n\x0bneuronPanel\x18\x06 \x03(\x0b\x32\x35.allego.SpikeSorterGetDashboardReply.NeuronPanelEntry\x12*\n\x02\x61I\x18\x07 \x01(\x0b\x32\x1e.allego.SpikeSorterDashboardAI\x1aR\n\x0ePortStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .allego.IndicoDashboardPortStats:\x02\x38\x01\x1aW\n\x0eSitePanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.allego.IndicoDashboardSiteIndicators:\x02\x38\x01\x1a[\n\x10NeuronPanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.allego.IndicoDashboardNeuronIndicators:\x02\x38\x01\"\xac\x03\n\x1eSpikeSorterDashboardGeneralRec\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x10\n\x08sorterID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\x12\x15\n\rnumTotalSites\x18\x06 \x02(\x03\x12\x17\n\x0fnumEnabledSites\x18\x07 \x02(\x03\x12\x16\n\x0enumActiveSites\x18\x08 \x02(\x03\x12\x12\n\nnumNeurons\x18\t \x02(\x03\x12\x12\n\nprobeYield\x18\n \x02(\x01\x12\x11\n\tsiteYield\x18\x0b \x02(\x01\x12\x1a\n\x12numSpikesProcessed\x18\x0c \x02(\x03\x12\x18\n\x10numSpikesLabeled\x18\r \x02(\x03\x12\x16\n\x0esortEfficiency\x18\x0e \x02(\x01\x12(\n\x08sinkDesc\x18\x0f \x02(\x0b\x32\x16.allego.FileDescriptor\"\xd5\x01\n\x16SpikeSorterDashboardAI\x12\x0c\n\x04\x62\x65ta\x18\x01 \x02(\x01\x12\"\n\x1a\x65stimatedReaderCompleteSec\x18\x02 \x02(\x01\x12\x1a\n\x12interSessionDurSec\x18\x03 \x02(\x01\x12\x19\n\x11interSessionStart\x18\x04 \x02(\t\x12\x15\n\rsessionDurSec\x18\x05 \x02(\x01\x12\x14\n\x0csessionStart\x18\x06 \x02(\t\x12\x12\n\nsessionIdx\x18\x07 \x02(\x03\x12\x11\n\tstartTime\x18\x08 \x02(\t\"_\n\x18IndicoDashboardSiteStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x12\n\nnumNeurons\x18\x04 \x02(\x03\"\x90\x01\n\x18IndicoDashboardPortStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x04 \x02(\x01\x12\x17\n\x0fnumEnabledSites\x18\x05 \x02(\x03\x12\x12\n\nnumNeurons\x18\x06 \x02(\x03\"\xd9\x01\n\x1dIndicoDashboardSiteIndicators\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\r\n\x05noise\x18\x03 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x04 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x05 \x03(\x01\x12\x11\n\tspikeRate\x18\x06 \x03(\x01\x12\x11\n\tposProbeX\x18\x07 \x03(\x01\x12\x11\n\tposProbeY\x18\x08 \x03(\x01\x12\x11\n\tposProbeZ\x18\t \x03(\x01\x12\x0f\n\x07siteNum\x18\n \x03(\x05\"\xb1\x01\n\x1fIndicoDashboardNeuronIndicators\x12\x10\n\x08neuronID\x18\x01 \x03(\t\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\x11\n\tspikeRate\x18\x03 \x03(\x01\x12\x11\n\tposProbeX\x18\x04 \x03(\x01\x12\x11\n\tposProbeY\x18\x05 \x03(\x01\x12\x11\n\tposProbeZ\x18\x06 \x03(\x01\x12\x0f\n\x07siteNum\x18\x07 \x03(\x05\x12\x12\n\nspikeLabel\x18\x08 \x03(\x05\"\xa7\x02\n\x1cSpikeSorterDashboardSiteDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x10\n\x08posProbe\x18\x03 \x03(\x01\x12\x10\n\x08posBrain\x18\x04 \x03(\x01\x12\x0e\n\x06snrMax\x18\x05 \x02(\x01\x12\x0e\n\x06snrMin\x18\x06 \x02(\x01\x12\x12\n\nnoiseLevel\x18\x07 \x02(\x01\x12\x12\n\nnumNeurons\x18\x08 \x02(\x03\x12/\n\rindicoCluster\x18\n \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x1c\n\x14pileWaveformMinValue\x18\r \x02(\x02\x12\x1c\n\x14pileWaveformMaxValue\x18\x0e \x02(\x02\"\xd2\x01\n\x1eSpikeSorterDashboardNeuronDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12&\n\x04\x64\x65sc\x18\x02 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x0b\n\x03snr\x18\x05 \x02(\x01\x12\x0f\n\x07IsihMax\x18\x06 \x02(\x01\x12\x15\n\rIsihArgmaxSec\x18\x07 \x02(\x01\x12\x15\n\rIsihArgmaxIdx\x18\x08 \x02(\x03\x12\x10\n\x08IsihMean\x18\t \x02(\x01\x12\x0e\n\x06IsihSd\x18\n \x02(\x01\"\xfa\x01\n SpikeSorterDashboardNeuronDetail\x12&\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x18\n\x10templateWaveform\x18\x02 \x03(\x02\x12\x1a\n\x12templateSdWaveform\x18\x03 \x03(\x02\x12\x18\n\x10pileWaveformData\x18\x04 \x03(\x02\x12\x1e\n\x16numSamplesPileWaveform\x18\x05 \x02(\x05\x12\x18\n\x10numPileWaveforms\x18\x06 \x02(\x05\x12$\n\x04isih\x18\x0b \x02(\x0b\x32\x16.allego.NeuronHistData\"\xa9\x01\n\x1eSpikeSorterDashboardSiteDetail\x12\x32\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32$.allego.SpikeSorterDashboardSiteDesc\x12\x19\n\x11orderedSpikeLabel\x18\x02 \x03(\x05\x12\x38\n\x06neuron\x18\x03 \x03(\x0b\x32(.allego.SpikeSorterDashboardNeuronDetail*\x80\x01\n\x0fSpikeSorterType\x12\x0f\n\x0bSORTER_NULL\x10\x00\x12\x15\n\x11SORTER_VEX_STREAM\x10\x01\x12\x18\n\x14SORTER_SPIKES_STREAM\x10\x02\x12\x13\n\x0fSORTER_VEX_FILE\x10\x03\x12\x16\n\x12SORTER_SPIKES_FILE\x10\x04*\xb0\x01\n\x12SpikeSorterCommand\x12\x11\n\rSORTER_CMD_ON\x10\x00\x12\x12\n\x0eSORTER_CMD_OFF\x10\x01\x12\x19\n\x15SORTER_CMD_CLEAR_SORT\x10\x02\x12\x15\n\x11SORTER_CMD_REBASE\x10\x04\x12\x13\n\x0fSORTER_CMD_INIT\x10\x07\x12\x17\n\x13SORTER_CMD_LOCALIZE\x10\x08\x12\x13\n\x0fSORTER_CMD_SORT\x10\t*/\n\x15SpikeSorterSubCommand\x12\x16\n\x12SORTER_SUBCMD_NULL\x10\x00*@\n\x0fSpikeSorterMode\x12\x16\n\x12SORTER_MODE_STREAM\x10\x00\x12\x15\n\x11SORTER_MODE_BATCH\x10\x01*I\n\x16SpikeSorterStateSystem\x12\n\n\x06SYS_ON\x10\x00\x12\x0b\n\x07SYS_OFF\x10\x01\x12\x16\n\x12SYS_NOT_CONFIGURED\x10\x02*f\n\rSpkSortIOtype\x12\x17\n\x13SPK_SORT_IO_NETWORK\x10\x00\x12\x17\n\x13SPK_SORT_IO_TRAINER\x10\x01\x12#\n\x1fSPK_SORT_IO_NETWORK_AND_TRAINER\x10\x02*>\n\x0fSpkSortIOtarget\x12\x14\n\x10SPK_SORT_IO_FSYS\x10\x00\x12\x15\n\x11SPK_SORT_IO_CLOUD\x10\x01*;\n\rSpkSortIOmode\x12\x14\n\x10SPK_SORT_IO_SAVE\x10\x00\x12\x14\n\x10SPK_SORT_IO_LOAD\x10\x01*u\n\x19SpikeSorterCriterionLevel\x12\x10\n\x0cSORTER_LEAST\x10\x00\x12\x0f\n\x0bSORTER_LESS\x10\x01\x12\x13\n\x0fSORTER_BALANCED\x10\x02\x12\x0f\n\x0bSORTER_MORE\x10\x03\x12\x0f\n\x0bSORTER_MOST\x10\x04*\x84\x01\n\x07SS_STAT\x12\x08\n\x04MEAN\x10\x00\x12\x06\n\x02SD\x10\x01\x12\x08\n\x04MODE\x10\x02\x12\x07\n\x03MIN\x10\x03\x12\x07\n\x03MAX\x10\x04\x12\x0e\n\nMODE_COUNT\x10\x05\x12\n\n\x06MEDIAN\x10\x06\x12\x07\n\x03Q25\x10\x07\x12\x07\n\x03Q75\x10\x08\x12\x08\n\x04SKEW\x10\t\x12\x0c\n\x08KURTOSIS\x10\n\x12\x05\n\x01N\x10\x0b\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spikesorter_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -29,120 +29,120 @@
   _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_options = b'8\001'
   _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._options = None
   _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._serialized_options = b'8\001'
   _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._options = None
   _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._serialized_options = b'8\001'
   _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._options = None
   _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._serialized_options = b'8\001'
-  _SPIKESORTERTYPE._serialized_start=7565
-  _SPIKESORTERTYPE._serialized_end=7693
-  _SPIKESORTERCOMMAND._serialized_start=7696
-  _SPIKESORTERCOMMAND._serialized_end=7872
-  _SPIKESORTERSUBCOMMAND._serialized_start=7874
-  _SPIKESORTERSUBCOMMAND._serialized_end=7921
-  _SPIKESORTERMODE._serialized_start=7923
-  _SPIKESORTERMODE._serialized_end=7987
-  _SPIKESORTERSTATESYSTEM._serialized_start=7989
-  _SPIKESORTERSTATESYSTEM._serialized_end=8062
-  _SPKSORTIOTYPE._serialized_start=8064
-  _SPKSORTIOTYPE._serialized_end=8166
-  _SPKSORTIOTARGET._serialized_start=8168
-  _SPKSORTIOTARGET._serialized_end=8230
-  _SPKSORTIOMODE._serialized_start=8232
-  _SPKSORTIOMODE._serialized_end=8291
-  _SPIKESORTERCRITERIONLEVEL._serialized_start=8293
-  _SPIKESORTERCRITERIONLEVEL._serialized_end=8410
-  _SS_STAT._serialized_start=8413
-  _SS_STAT._serialized_end=8545
+  _SPIKESORTERTYPE._serialized_start=7676
+  _SPIKESORTERTYPE._serialized_end=7804
+  _SPIKESORTERCOMMAND._serialized_start=7807
+  _SPIKESORTERCOMMAND._serialized_end=7983
+  _SPIKESORTERSUBCOMMAND._serialized_start=7985
+  _SPIKESORTERSUBCOMMAND._serialized_end=8032
+  _SPIKESORTERMODE._serialized_start=8034
+  _SPIKESORTERMODE._serialized_end=8098
+  _SPIKESORTERSTATESYSTEM._serialized_start=8100
+  _SPIKESORTERSTATESYSTEM._serialized_end=8173
+  _SPKSORTIOTYPE._serialized_start=8175
+  _SPKSORTIOTYPE._serialized_end=8277
+  _SPKSORTIOTARGET._serialized_start=8279
+  _SPKSORTIOTARGET._serialized_end=8341
+  _SPKSORTIOMODE._serialized_start=8343
+  _SPKSORTIOMODE._serialized_end=8402
+  _SPIKESORTERCRITERIONLEVEL._serialized_start=8404
+  _SPIKESORTERCRITERIONLEVEL._serialized_end=8521
+  _SS_STAT._serialized_start=8524
+  _SS_STAT._serialized_end=8656
   _SPIKESORTERLAUNCHREQUEST._serialized_start=64
-  _SPIKESORTERLAUNCHREQUEST._serialized_end=324
-  _SPIKESORTERCOMMANDREQUEST._serialized_start=327
-  _SPIKESORTERCOMMANDREQUEST._serialized_end=465
-  _SPIKESORTERSTATE._serialized_start=468
-  _SPIKESORTERSTATE._serialized_end=675
-  _SPKSORTIOREQ._serialized_start=678
-  _SPKSORTIOREQ._serialized_end=807
-  _SPIKESORTERLAUNCHREPLY._serialized_start=809
-  _SPIKESORTERLAUNCHREPLY._serialized_end=914
-  _GETSPIKESORTERIDSREPLY._serialized_start=916
-  _GETSPIKESORTERIDSREPLY._serialized_end=964
-  _SPIKESORTERGETRASTERDATAREQUEST._serialized_start=967
-  _SPIKESORTERGETRASTERDATAREQUEST._serialized_end=1128
-  _SPIKESORTERRASTERDATAREPLY._serialized_start=1131
-  _SPIKESORTERRASTERDATAREPLY._serialized_end=1301
-  _SPIKESORTERSTANDARDREQUEST._serialized_start=1303
-  _SPIKESORTERSTANDARDREQUEST._serialized_end=1354
-  _SPIKESORTERDYNAMIC._serialized_start=1357
-  _SPIKESORTERDYNAMIC._serialized_end=1747
-  _SPIKESORTERDYNAMIC_CRITERIA._serialized_start=1523
-  _SPIKESORTERDYNAMIC_CRITERIA._serialized_end=1683
-  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_start=1685
-  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_end=1747
-  _SPIKESORTERSETDYNAMICREQUEST._serialized_start=1750
-  _SPIKESORTERSETDYNAMICREQUEST._serialized_end=1947
-  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_start=1873
-  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_end=1947
-  _SPIKESORTERGETDYNAMICREPLY._serialized_start=1950
-  _SPIKESORTERGETDYNAMICREPLY._serialized_end=2166
-  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_start=1873
-  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_end=1947
-  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_start=2168
-  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_end=2276
-  _CLUSTERMAPOUTLIERS._serialized_start=2278
-  _CLUSTERMAPOUTLIERS._serialized_end=2329
-  _CLUSTERMAPQUARTILES._serialized_start=2331
-  _CLUSTERMAPQUARTILES._serialized_end=2388
-  _CLUSTERMAPSTATS._serialized_start=2391
-  _CLUSTERMAPSTATS._serialized_end=2522
-  _CLUSTERMAPRECORD._serialized_start=2524
-  _CLUSTERMAPRECORD._serialized_end=2626
-  _SPIKESORTSITESTATUS._serialized_start=2629
-  _SPIKESORTSITESTATUS._serialized_end=2797
-  _SPIKESORTPHASESTATUS._serialized_start=2800
-  _SPIKESORTPHASESTATUS._serialized_end=2943
-  _SPIKESORTNBRIDXLIST._serialized_start=2945
-  _SPIKESORTNBRIDXLIST._serialized_end=2987
-  _SPIKESORTERSTATUSREPLY._serialized_start=2990
-  _SPIKESORTERSTATUSREPLY._serialized_end=3360
-  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_start=3362
-  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_end=3444
-  _SPIKESORTERCLASSIFIERSPEC._serialized_start=3447
-  _SPIKESORTERCLASSIFIERSPEC._serialized_end=3828
-  _SPIKESORTERVARIANTSPEC._serialized_start=3830
-  _SPIKESORTERVARIANTSPEC._serialized_end=3947
-  _SPIKESORTERSPEC._serialized_start=3950
-  _SPIKESORTERSPEC._serialized_end=4154
-  _SPIKESORTERGETCONFIGREPLY._serialized_start=4157
-  _SPIKESORTERGETCONFIGREPLY._serialized_end=4351
-  _SPIKESORTERVIZREQUEST._serialized_start=4354
-  _SPIKESORTERVIZREQUEST._serialized_end=4626
-  _SPIKESORTERVIZREQUEST_VTYPE._serialized_start=4587
-  _SPIKESORTERVIZREQUEST_VTYPE._serialized_end=4626
-  _SPIKESORTERGETDASHBOARDREPLY._serialized_start=4629
-  _SPIKESORTERGETDASHBOARDREPLY._serialized_end=5335
-  _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._serialized_start=5071
-  _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._serialized_end=5153
-  _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._serialized_start=5155
-  _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._serialized_end=5242
-  _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._serialized_start=5244
-  _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._serialized_end=5335
-  _SPIKESORTERDASHBOARDGENERALREC._serialized_start=5338
-  _SPIKESORTERDASHBOARDGENERALREC._serialized_end=5766
-  _SPIKESORTERDASHBOARDAI._serialized_start=5769
-  _SPIKESORTERDASHBOARDAI._serialized_end=5982
-  _INDICODASHBOARDSITESTATS._serialized_start=5984
-  _INDICODASHBOARDSITESTATS._serialized_end=6079
-  _INDICODASHBOARDPORTSTATS._serialized_start=6082
-  _INDICODASHBOARDPORTSTATS._serialized_end=6226
-  _INDICODASHBOARDSITEINDICATORS._serialized_start=6229
-  _INDICODASHBOARDSITEINDICATORS._serialized_end=6446
-  _INDICODASHBOARDNEURONINDICATORS._serialized_start=6449
-  _INDICODASHBOARDNEURONINDICATORS._serialized_end=6626
-  _SPIKESORTERDASHBOARDSITEDESC._serialized_start=6629
-  _SPIKESORTERDASHBOARDSITEDESC._serialized_end=6924
-  _SPIKESORTERDASHBOARDNEURONDESC._serialized_start=6927
-  _SPIKESORTERDASHBOARDNEURONDESC._serialized_end=7137
-  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_start=7140
-  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_end=7390
-  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_start=7393
-  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_end=7562
+  _SPIKESORTERLAUNCHREQUEST._serialized_end=380
+  _SPIKESORTERCOMMANDREQUEST._serialized_start=383
+  _SPIKESORTERCOMMANDREQUEST._serialized_end=521
+  _SPIKESORTERSTATE._serialized_start=524
+  _SPIKESORTERSTATE._serialized_end=786
+  _SPKSORTIOREQ._serialized_start=789
+  _SPKSORTIOREQ._serialized_end=918
+  _SPIKESORTERLAUNCHREPLY._serialized_start=920
+  _SPIKESORTERLAUNCHREPLY._serialized_end=1025
+  _GETSPIKESORTERIDSREPLY._serialized_start=1027
+  _GETSPIKESORTERIDSREPLY._serialized_end=1075
+  _SPIKESORTERGETRASTERDATAREQUEST._serialized_start=1078
+  _SPIKESORTERGETRASTERDATAREQUEST._serialized_end=1239
+  _SPIKESORTERRASTERDATAREPLY._serialized_start=1242
+  _SPIKESORTERRASTERDATAREPLY._serialized_end=1412
+  _SPIKESORTERSTANDARDREQUEST._serialized_start=1414
+  _SPIKESORTERSTANDARDREQUEST._serialized_end=1465
+  _SPIKESORTERDYNAMIC._serialized_start=1468
+  _SPIKESORTERDYNAMIC._serialized_end=1858
+  _SPIKESORTERDYNAMIC_CRITERIA._serialized_start=1634
+  _SPIKESORTERDYNAMIC_CRITERIA._serialized_end=1794
+  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_start=1796
+  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_end=1858
+  _SPIKESORTERSETDYNAMICREQUEST._serialized_start=1861
+  _SPIKESORTERSETDYNAMICREQUEST._serialized_end=2058
+  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_start=1984
+  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_end=2058
+  _SPIKESORTERGETDYNAMICREPLY._serialized_start=2061
+  _SPIKESORTERGETDYNAMICREPLY._serialized_end=2277
+  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_start=1984
+  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_end=2058
+  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_start=2279
+  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_end=2387
+  _CLUSTERMAPOUTLIERS._serialized_start=2389
+  _CLUSTERMAPOUTLIERS._serialized_end=2440
+  _CLUSTERMAPQUARTILES._serialized_start=2442
+  _CLUSTERMAPQUARTILES._serialized_end=2499
+  _CLUSTERMAPSTATS._serialized_start=2502
+  _CLUSTERMAPSTATS._serialized_end=2633
+  _CLUSTERMAPRECORD._serialized_start=2635
+  _CLUSTERMAPRECORD._serialized_end=2737
+  _SPIKESORTSITESTATUS._serialized_start=2740
+  _SPIKESORTSITESTATUS._serialized_end=2908
+  _SPIKESORTPHASESTATUS._serialized_start=2911
+  _SPIKESORTPHASESTATUS._serialized_end=3054
+  _SPIKESORTNBRIDXLIST._serialized_start=3056
+  _SPIKESORTNBRIDXLIST._serialized_end=3098
+  _SPIKESORTERSTATUSREPLY._serialized_start=3101
+  _SPIKESORTERSTATUSREPLY._serialized_end=3471
+  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_start=3473
+  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_end=3555
+  _SPIKESORTERCLASSIFIERSPEC._serialized_start=3558
+  _SPIKESORTERCLASSIFIERSPEC._serialized_end=3939
+  _SPIKESORTERVARIANTSPEC._serialized_start=3941
+  _SPIKESORTERVARIANTSPEC._serialized_end=4058
+  _SPIKESORTERSPEC._serialized_start=4061
+  _SPIKESORTERSPEC._serialized_end=4265
+  _SPIKESORTERGETCONFIGREPLY._serialized_start=4268
+  _SPIKESORTERGETCONFIGREPLY._serialized_end=4462
+  _SPIKESORTERVIZREQUEST._serialized_start=4465
+  _SPIKESORTERVIZREQUEST._serialized_end=4737
+  _SPIKESORTERVIZREQUEST_VTYPE._serialized_start=4698
+  _SPIKESORTERVIZREQUEST_VTYPE._serialized_end=4737
+  _SPIKESORTERGETDASHBOARDREPLY._serialized_start=4740
+  _SPIKESORTERGETDASHBOARDREPLY._serialized_end=5446
+  _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._serialized_start=5182
+  _SPIKESORTERGETDASHBOARDREPLY_PORTSTATSENTRY._serialized_end=5264
+  _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._serialized_start=5266
+  _SPIKESORTERGETDASHBOARDREPLY_SITEPANELENTRY._serialized_end=5353
+  _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._serialized_start=5355
+  _SPIKESORTERGETDASHBOARDREPLY_NEURONPANELENTRY._serialized_end=5446
+  _SPIKESORTERDASHBOARDGENERALREC._serialized_start=5449
+  _SPIKESORTERDASHBOARDGENERALREC._serialized_end=5877
+  _SPIKESORTERDASHBOARDAI._serialized_start=5880
+  _SPIKESORTERDASHBOARDAI._serialized_end=6093
+  _INDICODASHBOARDSITESTATS._serialized_start=6095
+  _INDICODASHBOARDSITESTATS._serialized_end=6190
+  _INDICODASHBOARDPORTSTATS._serialized_start=6193
+  _INDICODASHBOARDPORTSTATS._serialized_end=6337
+  _INDICODASHBOARDSITEINDICATORS._serialized_start=6340
+  _INDICODASHBOARDSITEINDICATORS._serialized_end=6557
+  _INDICODASHBOARDNEURONINDICATORS._serialized_start=6560
+  _INDICODASHBOARDNEURONINDICATORS._serialized_end=6737
+  _SPIKESORTERDASHBOARDSITEDESC._serialized_start=6740
+  _SPIKESORTERDASHBOARDSITEDESC._serialized_end=7035
+  _SPIKESORTERDASHBOARDNEURONDESC._serialized_start=7038
+  _SPIKESORTERDASHBOARDNEURONDESC._serialized_end=7248
+  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_start=7251
+  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_end=7501
+  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_start=7504
+  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_end=7673
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-1.0.4/setup.py` & `radiens-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from setuptools import find_packages, setup
 
 metadata = {}
 with open('radiens/version.py', 'r') as f:
-      exec(f.read(), None, metadata)
+    exec(f.read(), None, metadata)
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
-      _reqs = f.read().split('\n')
-      install_requires = [r for r in _reqs if r]
+    _reqs = f.read().split('\n')
+    install_requires = [r for r in _reqs if r]
 
 setup(name='radiens',
       version=metadata['__version__'],
       description='provides python API to RADIENS analytics platform',
-      long_description=long_description,      
+      long_description=long_description,
       long_description_content_type="text/markdown",
       author='NeuroNexus',
       author_email='dkipke@neuronexus.com',
       license='MIT',
-      license_files = ('LICENSE',),
+      license_files=('LICENSE',),
       url='http://neuronexus.github.io',
       classifiers=[
-            'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3.7',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'License :: OSI Approved :: MIT License',
+          'Operating System :: OS Independent',
+          #   'Programming Language :: Python :: 3.7',
+          #   'Programming Language :: Python :: 3.8',
+          #   'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'License :: OSI Approved :: MIT License',
       ],
       packages=find_packages(exclude=('radiens_obs', 'tests')),
       include_package_data=True,
-      python_requires='>=3.7',
+      python_requires='>=3.10',
       install_requires=install_requires,
+      entry_points={
+          'console_scripts': ['radiens=radiens.cli.main:cli',
+                              ]},
+
       )
```

