# Comparing `tmp/remotemanager-0.7.0.tar.gz` & `tmp/remotemanager-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.7.0.tar", last modified: Fri Jun 16 11:23:06 2023, max compression
+gzip compressed data, was "remotemanager-0.7.1.tar", last modified: Fri Jun 23 06:58:09 2023, max compression
```

## Comparing `remotemanager-0.7.0.tar` & `remotemanager-0.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-16 11:23:06.694952 remotemanager-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-15 14:41:51.000000 remotemanager-0.7.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-15 14:41:51.000000 remotemanager-0.7.0/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.7.0/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.7.0/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25087 2023-06-16 10:42:35.000000 remotemanager-0.7.0/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50282 2023-06-15 12:40:25.000000 remotemanager-0.7.0/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22383 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2023-06-15 11:08:04.000000 remotemanager-0.7.0/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.7.0/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.7.0/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.7.0/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.7.0/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.7.0/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.7.0/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.7.0/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9283 2023-06-14 07:47:50.000000 remotemanager-0.7.0/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 11:23:06.694952 remotemanager-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.806987 remotemanager-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 06:58:09.806987 remotemanager-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.7.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-22 15:30:59.000000 remotemanager-0.7.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-22 15:30:59.000000 remotemanager-0.7.1/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.7.1/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.7.1/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.7.1/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25087 2023-06-16 10:42:35.000000 remotemanager-0.7.1/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50410 2023-06-22 14:49:18.000000 remotemanager-0.7.1/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22383 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-22 14:49:18.000000 remotemanager-0.7.1/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.7.1/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.7.1/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.7.1/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.7.1/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.7.1/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.7.1/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.7.1/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.802987 remotemanager-0.7.1/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.7.1/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.7.1/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9283 2023-06-14 07:47:50.000000 remotemanager-0.7.1/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.806987 remotemanager-0.7.1/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.7.1/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 06:58:09.798987 remotemanager-0.7.1/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-23 06:58:09.000000 remotemanager-0.7.1/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 06:58:09.806987 remotemanager-0.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.7.1/setup.py
```

### Comparing `remotemanager-0.7.0/LICENSE` & `remotemanager-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/PKG-INFO` & `remotemanager-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.7.0
+Version: 0.7.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.7.0/README.md` & `remotemanager-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/pyproject.toml` & `remotemanager-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.7.0/remotemanager/connection/cmd.py` & `remotemanager-0.7.1/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/computers/base.py` & `remotemanager-0.7.1/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/computers/example.py` & `remotemanager-0.7.1/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/computers/options.py` & `remotemanager-0.7.1/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/computers/parsers.py` & `remotemanager-0.7.1/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/testing_object.py` & `remotemanager-0.7.1/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/connection/url.py` & `remotemanager-0.7.1/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/dataset/dataset.py` & `remotemanager-0.7.1/remotemanager/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,16 @@
             command to exec any scripts with. Defaults to "bash"
         name (str):
             optional name for this dataset. Will be used for runscripts
         extra_files_send(list, str):
             extra files to send with this run
         extra_files_recv(list, str):
             extra files to retrieve with this run
+        skip (bool):
+            skip dataset creation if possible. Defaults True
         global_run_args:
             any further (unchanging) arguments to be passed to the runner(s)
     """
 
     _do_not_package = ["_database"]
 
     # DEV NOTE: arguments must be None for computer-url override to function
@@ -67,15 +69,15 @@
         script: str = None,
         name: str = None,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         verbose: int = None,
         add_newline: bool = True,
         block_reinit: bool = None,
-        skip: bool = False,
+        skip: bool = True,
         **global_run_args,
     ):
         self._verbose = Verbosity(verbose)
 
         self._logger.info("dataset initialised")
 
         self._function = Function(function)
@@ -115,18 +117,20 @@
 
         self.url = url
         self.transport = transport
         self.serialiser = serialiser
         self._submitter = None
 
         if block_reinit is not None:
-            warnings.warn("block_reinit is soon to be deprecated, use skip instead")
-            skip = block_reinit
+            warnings.warn(
+                "block_reinit is soon to be deprecated, " "use skip=False instead"
+            )
+            skip = not block_reinit
 
-        if skip:
+        if not skip:
             try:
                 os.remove(self.dbfile)
                 self._logger.warning(
                     f"deleted database file {self.dbfile}", silent=True
                 )
             except FileNotFoundError:
                 pass
```

### Comparing `remotemanager-0.7.0/remotemanager/dataset/dependency.py` & `remotemanager-0.7.1/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/dataset/runner.py` & `remotemanager-0.7.1/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/jupyter/magic.py` & `remotemanager-0.7.1/remotemanager/jupyter/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         self._logger.info(f"generated function string {fstr}")
         self._logger.info(f"Dataset args: {args}")
         self._logger.info(f"Function args: {fargs}")
 
         run_skip = args.pop("skip", True)
         # Build the runner and run
-        ds = Dataset(function=fstr, skip=False, **args)
+        ds = Dataset(function=fstr, skip=True, **args)
         ds.append_run(args=fargs)
         ds.run(skip=run_skip)
 
         for cmd in ds.run_cmds:
             if cmd.stderr:
                 raise RuntimeError(f"error detected in magic run: " f"{cmd.stderr}")
         Quiet.state = True
```

### Comparing `remotemanager-0.7.0/remotemanager/logging/__init__.py` & `remotemanager-0.7.1/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/logging/log.py` & `remotemanager-0.7.1/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/logging/utils.py` & `remotemanager-0.7.1/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/logging/verbosity.py` & `remotemanager-0.7.1/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/serialisation/__init__.py` & `remotemanager-0.7.1/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/serialisation/serial.py` & `remotemanager-0.7.1/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.7.1/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.7.1/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/storage/database.py` & `remotemanager-0.7.1/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/storage/function.py` & `remotemanager-0.7.1/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/storage/remotefunction.py` & `remotemanager-0.7.1/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/storage/sendablemixin.py` & `remotemanager-0.7.1/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/storage/trackedfile.py` & `remotemanager-0.7.1/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/transport/cp.py` & `remotemanager-0.7.1/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/transport/rsync.py` & `remotemanager-0.7.1/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/transport/scp.py` & `remotemanager-0.7.1/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/transport/transport.py` & `remotemanager-0.7.1/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/utils/__init__.py` & `remotemanager-0.7.1/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/utils/flags.py` & `remotemanager-0.7.1/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager/utils/version.py` & `remotemanager-0.7.1/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.7.0/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.7.1/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.7.0
+Version: 0.7.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.7.0/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.7.1/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

