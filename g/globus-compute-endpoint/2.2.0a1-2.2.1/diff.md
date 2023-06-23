# Comparing `tmp/globus-compute-endpoint-2.2.0a1.tar.gz` & `tmp/globus-compute-endpoint-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.2.0a1.tar", last modified: Wed Jun 21 18:53:29 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.2.1.tar", last modified: Fri Jun 23 01:03:56 2023, max compression
```

## Comparing `globus-compute-endpoint-2.2.0a1.tar` & `globus-compute-endpoint-2.2.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.026301 globus-compute-endpoint-2.2.0a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       83 2023-06-21 18:50:46.000000 globus-compute-endpoint-2.2.0a1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-21 18:53:29.026365 globus-compute-endpoint-2.2.0a1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a1/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.013800 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.016674 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.017964 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)      117 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.yaml
--rw-r--r--   0 lei        (501) staff       (20)     3448 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.018912 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.019230 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.020508 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/
--rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/helper.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/process_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.020639 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024293 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8499 2023-06-21 18:50:27.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024472 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024964 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.025667 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-06-21 18:52:01.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.014518 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     3152 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      344 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-21 18:53:29.026607 globus-compute-endpoint-2.2.0a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3685 2023-06-21 18:51:52.000000 globus-compute-endpoint-2.2.0a1/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.026116 globus-compute-endpoint-2.2.0a1/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.0a1/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.558050 globus-compute-endpoint-2.2.1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       83 2023-06-21 21:23:44.000000 globus-compute-endpoint-2.2.1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1838 2023-06-23 01:03:56.558134 globus-compute-endpoint-2.2.1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.1/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.544078 globus-compute-endpoint-2.2.1/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.547356 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.548441 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)      117 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-r--r--   0 lei        (501) staff       (20)     3447 2023-06-23 00:56:17.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.549176 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.549558 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.550769 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/
+-rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/helper.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/process_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.550911 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.555338 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8499 2023-06-21 18:50:27.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.555614 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.556322 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.557235 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      804 2023-06-23 00:59:13.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.544803 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1838 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     3152 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      342 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-23 01:03:56.558447 globus-compute-endpoint-2.2.1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3683 2023-06-23 00:59:09.000000 globus-compute-endpoint-2.2.1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.557776 globus-compute-endpoint-2.2.1/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.1/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.2.0a1/LICENSE` & `globus-compute-endpoint-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/PKG-INFO` & `globus-compute-endpoint-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.0a1/PyPI.md` & `globus-compute-endpoint-2.2.1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     type: type = Field(default=HighThroughputExecutor, const=True)
     provider: ProviderModel
     strategy: t.Optional[StrategyModel]
     address: t.Optional[t.Union[str, AddressModel]]
 
     _validate_provider = _validate_params("provider")
     _validate_strategy = _validate_params("strategy")
-    _validate_strategy = _validate_params("address")
+    _validate_address = _validate_params("address")
 
     class Config:
         extra = "allow"
 
 
 class ConfigModel(BaseModel):
     engine: EngineModel
```

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/process_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.0a1"
+__version__ = "2.2.1"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/setup.py` & `globus-compute-endpoint-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.2.0a1",
+    "globus-compute-sdk==2.2.1",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.2.0a1/tests/conftest.py` & `globus-compute-endpoint-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a1/tests/utils.py` & `globus-compute-endpoint-2.2.1/tests/utils.py`

 * *Files identical despite different names*

