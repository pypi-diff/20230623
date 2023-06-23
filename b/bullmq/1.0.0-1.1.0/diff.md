# Comparing `tmp/bullmq-1.0.0.tar.gz` & `tmp/bullmq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.0.0.tar", last modified: Wed Jun 21 21:59:15 2023, max compression
+gzip compressed data, was "bullmq-1.1.0.tar", last modified: Fri Jun 23 19:17:12 2023, max compression
```

## Comparing `bullmq-1.0.0.tar` & `bullmq-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:59:15.298702 bullmq-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-21 21:59:15.298702 bullmq-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-21 21:57:19.000000 bullmq-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:59:15.290701 bullmq-1.0.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 21:59:13.000000 bullmq-1.0.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:59:15.298702 bullmq-1.0.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-21 21:58:48.000000 bullmq-1.0.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:59:15.298702 bullmq-1.0.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-21 21:57:19.000000 bullmq-1.0.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:59:15.294702 bullmq-1.0.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-21 21:59:15.000000 bullmq-1.0.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-21 21:59:15.000000 bullmq-1.0.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:59:15.000000 bullmq-1.0.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 21:59:15.000000 bullmq-1.0.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 21:59:15.000000 bullmq-1.0.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 21:59:15.298702 bullmq-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 21:57:19.000000 bullmq-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 19:17:12.299510 bullmq-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-23 19:15:56.000000 bullmq-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.287510 bullmq-1.1.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 19:17:08.000000 bullmq-1.1.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-23 19:16:39.000000 bullmq-1.1.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.299510 bullmq-1.1.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-23 19:15:56.000000 bullmq-1.1.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:17:12.287510 bullmq-1.1.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 19:17:12.000000 bullmq-1.1.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 19:17:12.299510 bullmq-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-23 19:15:56.000000 bullmq-1.1.0/setup.py
```

### Comparing `bullmq-1.0.0/PKG-INFO` & `bullmq-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.0.0
+Version: 1.1.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.0.0/README.md` & `bullmq-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/backoffs.py` & `bullmq-1.1.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/addJob-9.lua` & `bullmq-1.1.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.1.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.1.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.1.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/drain-4.lua` & `bullmq-1.1.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.1.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.1.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/getState-8.lua` & `bullmq-1.1.0/bullmq/commands/getState-8.lua`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     KEYS[3] 'delayed' key
     KEYS[4] 'active' key
     KEYS[5] 'wait' key
     KEYS[6] 'paused' key
     KEYS[7] 'waiting-children' key
     KEYS[8] 'prioritized' key
     ARGV[1] job id
-    ARGV[2] job key
   Output:
     'completed'
     'failed'
     'delayed'
     'active'
     'prioritized'
     'waiting'
```

### Comparing `bullmq-1.0.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.1.0/bullmq/commands/getStateV2-8.lua`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     KEYS[3] 'delayed' key
     KEYS[4] 'active' key
     KEYS[5] 'wait' key
     KEYS[6] 'paused' key
     KEYS[7] 'waiting-children' key
     KEYS[8] 'prioritized' key
     ARGV[1] job id
-    ARGV[2] job key
   Output:
     'completed'
     'failed'
     'delayed'
     'active'
     'waiting'
     'waiting-children'
```

### Comparing `bullmq-1.0.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.1.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.1.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 local token = ARGV[2]
 local lockKey = KEYS[4]
 local lockToken = rcall("GET", lockKey)
 local pttl = rcall("PTTL", KEYS[7])
 if lockToken == token and pttl > 0 then
   local removed = rcall("LREM", KEYS[1], 1, jobId)
   if (removed > 0) then
-    local target, paused = getTargetQueueList(KEYS[6], KEYS[2], KEYS[5])
+    local target = getTargetQueueList(KEYS[6], KEYS[2], KEYS[5])
     rcall("SREM", KEYS[3], jobId)
     local priority = tonumber(rcall("HGET", ARGV[3], "priority")) or 0
     if priority > 0 then
       pushBackJobWithPriority(KEYS[8], priority, jobId)
     else
       rcall("RPUSH", target, jobId)
     end
```

### Comparing `bullmq-1.0.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.1.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.1.0/bullmq/commands/moveToActive-10.lua`

 * *Files 2% similar despite different names*

```diff
@@ -96,47 +96,24 @@
     keys[10] pc priority counter
     opts - token - lock token
     opts - lockDuration
     opts - limiter
 ]]
 -- Includes
 --[[
-  Function to add job considering priority.
-]]
--- Includes
---[[
-  Function priority marker to wait if needed
-  in order to wake up our workers and to respect priority
-  order as much as possible
-]]
-local function addPriorityMarkerIfNeeded(waitKey)
-  local waitLen = rcall("LLEN", waitKey)
-  if waitLen == 0 then
-    rcall("LPUSH", waitKey, "0:0")
-  end
-end
-local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
-  local prioCounter = rcall("INCR", priorityCounterKey)
-  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
-  rcall("ZADD", prioritizedKey, score, jobId)
-  if not paused then
-    addPriorityMarkerIfNeeded(waitKey)
-  end
-end
---[[
   Function to push back job considering priority in front of same prioritized jobs.
 ]]
 local function pushBackJobWithPriority(prioritizedKey, priority, jobId)
   -- in order to put it at front of same prioritized jobs
   -- we consider prioritized counter as 0
   local score = priority * 0x100000000
   rcall("ZADD", prioritizedKey, score, jobId)
 end
 local function prepareJobForProcessing(keys, keyPrefix, targetKey, jobId, processedOn,
-    maxJobs, expireTime, paused, opts)
+    maxJobs, expireTime, opts)
   local jobKey = keyPrefix .. jobId
   -- Check if we need to perform rate limiting.
   if maxJobs then
     local rateLimiterKey = keys[6];
     -- check if we exceeded rate limit, we need to remove the job and return expireTime
     if expireTime > 0 then
       -- remove from active queue and add back to the wait list
@@ -170,14 +147,37 @@
 --[[
   Updates the delay set, by moving delayed jobs that should
   be processed now to "wait".
      Events:
       'waiting'
 ]]
 -- Includes
+--[[
+  Function to add job considering priority.
+]]
+-- Includes
+--[[
+  Function priority marker to wait if needed
+  in order to wake up our workers and to respect priority
+  order as much as possible
+]]
+local function addPriorityMarkerIfNeeded(waitKey)
+  local waitLen = rcall("LLEN", waitKey)
+  if waitLen == 0 then
+    rcall("LPUSH", waitKey, "0:0")
+  end
+end
+local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
+  local prioCounter = rcall("INCR", priorityCounterKey)
+  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
+  rcall("ZADD", prioritizedKey, score, jobId)
+  if not paused then
+    addPriorityMarkerIfNeeded(waitKey)
+  end
+end
 -- Try to get as much as 1000 jobs at once
 local function promoteDelayedJobs(delayedKey, waitKey, targetKey, prioritizedKey,
                                   eventStreamKey, prefix, timestamp, paused, priorityCounterKey)
     local jobs = rcall("ZRANGEBYSCORE", delayedKey, 0, (timestamp + 1) * 0x1000, "LIMIT", 0, 1000)
     if (#jobs > 0) then
         rcall("ZREM", delayedKey, unpack(jobs))
         for _, jobId in ipairs(jobs) do
@@ -233,26 +233,25 @@
     -- another script puts a new maker in wait, we need to check again.
     if jobId and string.sub(jobId, 1, 2) == "0:" then
       rcall("LREM", KEYS[2], 1, jobId)
       jobId = rcall("RPOPLPUSH", KEYS[1], KEYS[2])
     end
   end
   if jobId then
-    -- this script is not really moving, it is preparing the job for processing
-    return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, paused, opts)
+    return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, opts)
   else
     jobId = moveJobFromPriorityToActive(KEYS[3], KEYS[2], KEYS[10])
     if jobId then
-      return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, paused, opts)
+      return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, opts)
     end
   end
 else
   jobId = moveJobFromPriorityToActive(KEYS[3], KEYS[2], KEYS[10])
   if jobId then
-    return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, paused, opts)
+    return prepareJobForProcessing(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, opts)
   end
 end
 -- Return the timestamp for the next delayed job if any.
 local nextTimestamp = getNextDelayedTimestamp(KEYS[7])
 if (nextTimestamp ~= nil) then
   return { 0, 0, 0, nextTimestamp }
 end
```

### Comparing `bullmq-1.0.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.1.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.1.0/bullmq/commands/moveToFinished-13.lua`

 * *Files 2% similar despite different names*

```diff
@@ -141,47 +141,24 @@
     keys[10] pc priority counter
     opts - token - lock token
     opts - lockDuration
     opts - limiter
 ]]
 -- Includes
 --[[
-  Function to add job considering priority.
-]]
--- Includes
---[[
-  Function priority marker to wait if needed
-  in order to wake up our workers and to respect priority
-  order as much as possible
-]]
-local function addPriorityMarkerIfNeeded(waitKey)
-  local waitLen = rcall("LLEN", waitKey)
-  if waitLen == 0 then
-    rcall("LPUSH", waitKey, "0:0")
-  end
-end
-local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
-  local prioCounter = rcall("INCR", priorityCounterKey)
-  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
-  rcall("ZADD", prioritizedKey, score, jobId)
-  if not paused then
-    addPriorityMarkerIfNeeded(waitKey)
-  end
-end
---[[
   Function to push back job considering priority in front of same prioritized jobs.
 ]]
 local function pushBackJobWithPriority(prioritizedKey, priority, jobId)
   -- in order to put it at front of same prioritized jobs
   -- we consider prioritized counter as 0
   local score = priority * 0x100000000
   rcall("ZADD", prioritizedKey, score, jobId)
 end
 local function prepareJobForProcessing(keys, keyPrefix, targetKey, jobId, processedOn,
-    maxJobs, expireTime, paused, opts)
+    maxJobs, expireTime, opts)
   local jobKey = keyPrefix .. jobId
   -- Check if we need to perform rate limiting.
   if maxJobs then
     local rateLimiterKey = keys[6];
     -- check if we exceeded rate limit, we need to remove the job and return expireTime
     if expireTime > 0 then
       -- remove from active queue and add back to the wait list
@@ -240,14 +217,37 @@
 --[[
   Updates the delay set, by moving delayed jobs that should
   be processed now to "wait".
      Events:
       'waiting'
 ]]
 -- Includes
+--[[
+  Function to add job considering priority.
+]]
+-- Includes
+--[[
+  Function priority marker to wait if needed
+  in order to wake up our workers and to respect priority
+  order as much as possible
+]]
+local function addPriorityMarkerIfNeeded(waitKey)
+  local waitLen = rcall("LLEN", waitKey)
+  if waitLen == 0 then
+    rcall("LPUSH", waitKey, "0:0")
+  end
+end
+local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
+  local prioCounter = rcall("INCR", priorityCounterKey)
+  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
+  rcall("ZADD", prioritizedKey, score, jobId)
+  if not paused then
+    addPriorityMarkerIfNeeded(waitKey)
+  end
+end
 -- Try to get as much as 1000 jobs at once
 local function promoteDelayedJobs(delayedKey, waitKey, targetKey, prioritizedKey,
                                   eventStreamKey, prefix, timestamp, paused, priorityCounterKey)
     local jobs = rcall("ZRANGEBYSCORE", delayedKey, 0, (timestamp + 1) * 0x1000, "LIMIT", 0, 1000)
     if (#jobs > 0) then
         rcall("ZREM", delayedKey, unpack(jobs))
         for _, jobId in ipairs(jobs) do
@@ -575,23 +575,22 @@
         if paused then return {0, 0, 0, 0} end
         jobId = rcall("RPOPLPUSH", KEYS[1], KEYS[2])
         -- If jobId is special ID 0:delay, then there is no job to process
         if jobId then
             if string.sub(jobId, 1, 2) == "0:" then
                 rcall("LREM", KEYS[2], 1, jobId)
             else
-                -- this script is not really moving, it is preparing the job for processing
                 return prepareJobForProcessing(KEYS, ARGV[8], target, jobId, timestamp, maxJobs,
-                    expireTime, paused, opts)
+                    expireTime, opts)
             end
         else
             jobId = moveJobFromPriorityToActive(KEYS[3], KEYS[2], KEYS[10])
             if jobId then
                 return prepareJobForProcessing(KEYS, ARGV[8], target, jobId, timestamp, maxJobs,
-                    expireTime, paused, opts)
+                    expireTime, opts)
             end
         end
         -- Return the timestamp for the next delayed job if any.
         local nextTimestamp = getNextDelayedTimestamp(KEYS[7])
         if nextTimestamp ~= nil then
             -- The result is guaranteed to be positive, since the
             -- ZRANGEBYSCORE command would have return a job otherwise.
```

### Comparing `bullmq-1.0.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.1.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.1.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/pause-5.lua` & `bullmq-1.1.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/promote-7.lua` & `bullmq-1.1.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.1.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.1.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.1.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.1.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.1.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/event_emitter.py` & `bullmq-1.1.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/job.py` & `bullmq-1.1.0/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/queue.py` & `bullmq-1.1.0/bullmq/queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import asyncio
 from bullmq.redis_connection import RedisConnection
 from bullmq.types import QueueOptions, RetryJobsOptions, JobOptions
+from bullmq.utils import extract_result
 from bullmq.scripts import Scripts
 from bullmq.job import Job
 
 
 class Queue:
     """
     Instantiate a Queue object
@@ -120,14 +122,36 @@
         responses = await self.scripts.getCounts(current_types)
         counts = {}
 
         for index, val in enumerate(responses):
             counts[current_types[index]] = val or 0
         return counts
 
+    async def getJobs(self, types, start=0, end=-1, asc:bool=False):
+        current_types = self.sanitizeJobTypes(types)
+        job_ids = await self.scripts.getRanges(current_types, start, end, asc)
+        tasks = [asyncio.create_task(Job.fromId(self, i)) for i in job_ids]   
+        job_set, _ = await asyncio.wait(tasks, return_when=asyncio.ALL_COMPLETED)
+        jobs = [extract_result(job_task) for job_task in job_set]
+        jobs_len = len(jobs)
+
+        # we filter `None` out to remove:
+        jobs = list(filter(lambda j: j is not None, jobs))
+
+        for index, job_id in enumerate(job_ids):
+            pivot_job = jobs[index]
+
+            for i in range(index,jobs_len):
+                current_job = jobs[i]
+                if current_job and current_job.id == job_id:
+                    jobs[index] = current_job
+                    jobs[i] = pivot_job
+
+        return jobs
+
     def sanitizeJobTypes(self, types):
         current_types = list(types)
 
         if len(types) > 0:
             sanitized_types = current_types.copy()
 
             try:
```

### Comparing `bullmq-1.0.0/bullmq/redis_connection.py` & `bullmq-1.1.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/scripts.py` & `bullmq-1.1.0/bullmq/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.redisConnection = redisConnection
         self.redisClient = redisConnection.conn
         self.commands = {
             "addJob": self.redisClient.register_script(self.getScript("addJob-9.lua")),
             "changePriority": self.redisClient.register_script(self.getScript("changePriority-5.lua")),
             "extendLock": self.redisClient.register_script(self.getScript("extendLock-2.lua")),
             "getCounts": self.redisClient.register_script(self.getScript("getCounts-1.lua")),
+            "getRanges": self.redisClient.register_script(self.getScript("getRanges-1.lua")),
             "getState": self.redisClient.register_script(self.getScript("getState-8.lua")),
             "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-8.lua")),
             "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
             "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-10.lua")),
             "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-13.lua")),
             "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
@@ -96,14 +97,59 @@
         packedOpts = msgpack.packb(job.opts)
 
         keys = self.getKeys(['wait', 'paused', 'meta', 'id',
                             'delayed', 'prioritized', 'completed', 'events', 'pc'])
 
         return self.commands["addJob"](keys=keys, args=[packedArgs, jsonData, packedOpts])
 
+    def getRangesArgs(self, types, start: int = 0, end: int = 1, asc: bool = False):
+        transformed_types = []
+        for type in types:
+            transformed_types.append("wait" if type == "waiting" else type)
+
+        keys = self.getKeys([''])
+        args = [start, end, "1" if asc else "0"] + transformed_types
+
+        return (keys, args)
+
+    async def getRanges(self, types, start: int = 0, end: int = 1, asc: bool = False):
+        commands = []
+
+        switcher = {
+            "completed": "zrange",
+            "delayed": "zrange",
+            "failed": "zrange",
+            "priority": "zrange",
+            "repeat": "zrange",
+            "waiting-children": "zrange",
+            "active": "lrange",
+            "paused": "lrange",
+            "wait": "lrange"
+        }
+        transformed_types = []
+        for type in types:
+            transformed_type = "wait" if type == "waiting" else type
+            transformed_types.append(transformed_type)
+            commands.append(switcher.get(transformed_type))
+
+        keys, args = self.getRangesArgs(transformed_types, start, end, asc)
+
+        responses = await self.commands["getRanges"](keys=keys, args=args)
+
+        results = []
+        for i, response in enumerate(responses):
+            result = response or []
+
+            if asc and commands[i] == "lrange":
+                results+=result.reverse()
+            else:
+                results+=result
+
+        return results
+
     def saveStacktraceArgs(self, job_id: str, stacktrace: str, failedReason: str):
         keys = [self.toKey(job_id)]
         args = [stacktrace, failedReason]
 
         return (keys, args)
 
     def retryJobArgs(self, job_id: str, lifo: bool, token: str):
@@ -186,27 +232,27 @@
         
         args = [priority, self.toKey(job_id), job_id, 1 if lifo else 0]
 
         result = await self.commands["changePriority"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
-                raise self.finishedErrors(result, job_id, 'updateData')
+                raise self.finishedErrors(result, job_id, 'changePriority', None)
         return None
 
     async def updateData(self, job_id: str, data):
         keys = [self.toKey(job_id)]
         data_json = json.dumps(data, separators=(',', ':'))
         args = [data_json]
 
         result = await self.commands["updateData"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
-                raise self.finishedErrors(result, job_id, 'updateData')
+                raise self.finishedErrors(result, job_id, 'updateData', None)
         return None
 
     async def reprocessJob(self, job: Job, state: str):
         keys = [self.toKey(job.id)]
         keys.append(self.keys['events'])
         keys.append(self.keys[state])
         keys.append(self.keys['wait'])
@@ -287,15 +333,15 @@
         keys = [self.toKey(job_id), self.keys['events']]
         progress_json = json.dumps(progress, separators=(',', ':'))
         args = [job_id, progress_json]
         result = await self.commands["updateProgress"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
-                raise self.finishedErrors(result, job_id, 'updateProgress')
+                raise self.finishedErrors(result, job_id, 'updateProgress', None)
         return None
 
     def moveToFinishedArgs(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext=True) -> list[Any] | None:
         timestamp = round(time.time() * 1000)
         metricsKey = self.toKey('metrics:' + target)
 
         keys = self.getKeys(['wait', 'active', 'prioritized', 'events',
@@ -369,16 +415,15 @@
     def moveStalledJobsToWait(self, maxStalledCount: int, stalledInterval: int):
         keys = self.getKeys(['stalled', 'wait', 'active', 'failed',
                             'stalled-check', 'meta', 'paused', 'events'])
         args = [maxStalledCount, self.keys[''], round(
             time.time() * 1000), stalledInterval]
         return self.commands["moveStalledJobsToWait"](keys, args)
 
-
-    def finishedErrors(code: int, jobId: str, command: str, state: str) -> TypeError:
+    def finishedErrors(self, code: int, jobId: str, command: str, state: str) -> TypeError:
         if code == ErrorCode.JobNotExist.value:
             return TypeError(f"Missing key for job {jobId}.{command}")
         elif code == ErrorCode.JobLockNotExist.value:
             return TypeError(f"Missing lock for job {jobId}.{command}")
         elif code == ErrorCode.JobNotInState.value:
             return TypeError(f"Job {jobId} is not in the state {state}.{command}")
         elif code == ErrorCode.JobPendingDependencies.value:
```

### Comparing `bullmq-1.0.0/bullmq/timer.py` & `bullmq-1.1.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/types/job_options.py` & `bullmq-1.1.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/types/worker_options.py` & `bullmq-1.1.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/bullmq/worker.py` & `bullmq-1.1.0/bullmq/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from uuid import uuid4
 from bullmq.scripts import Scripts
 from bullmq.redis_connection import RedisConnection
 from bullmq.event_emitter import EventEmitter
 from bullmq.job import Job
 from bullmq.timer import Timer
 from bullmq.types import WorkerOptions
-from bullmq.utils import isRedisVersionLowerThan
+from bullmq.utils import isRedisVersionLowerThan, extract_result
 
 import asyncio
 import traceback
 import time
 import math
 
 class Worker(EventEmitter):
@@ -191,18 +191,7 @@
     job_set, pending = await asyncio.wait(task_set, return_when=asyncio.FIRST_COMPLETED)
     jobs = [extract_result(job_task) for job_task in job_set]
     # we filter `None` out to remove:
     # a) an empty 'completed jobs' list; and
     # b) a failed extract_result
     jobs = list(filter(lambda j: j is not None, jobs))
     return jobs, pending
-
-
-def extract_result(job_task):
-    try:
-        return job_task.result()
-    except Exception as e:
-        if not str(e).startswith('Connection closed by server'):
-            # lets use a simple-but-effective error handling:
-            # print error message and ignore the job
-            print("ERROR:", e)
-            traceback.print_exc()
```

### Comparing `bullmq-1.0.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.1.0/bullmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.0.0
+Version: 1.1.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.0.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.1.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.0.0/setup.py` & `bullmq-1.1.0/setup.py`

 * *Files identical despite different names*

