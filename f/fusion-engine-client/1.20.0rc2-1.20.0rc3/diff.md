# Comparing `tmp/fusion-engine-client-1.20.0rc2.tar.gz` & `tmp/fusion-engine-client-1.20.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc2.tar", last modified: Wed Jun  7 03:33:19 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc3.tar", last modified: Fri Jun 23 03:46:41 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc2.tar` & `fusion-engine-client-1.20.0rc3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.800689 fusion-engine-client-1.20.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    14038 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.788689 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110311 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.792688 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56695 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.792688 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.784688 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 03:33:19.000000 fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:33:19.800689 fusion-engine-client-1.20.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:33:19.796688 fusion-engine-client-1.20.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-07 03:32:42.000000 fusion-engine-client-1.20.0rc2/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.043105 fusion-engine-client-1.20.0rc3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.043105 fusion-engine-client-1.20.0rc3/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.047104 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113032 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56695 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26227 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35636 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.051104 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.047104 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 03:46:41.000000 fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:41.055105 fusion-engine-client-1.20.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-23 03:45:50.000000 fusion-engine-client-1.20.0rc3/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc2/PKG-INFO` & `fusion-engine-client-1.20.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc2
+Version: 1.20.0rc3
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc2/README.md` & `fusion-engine-client-1.20.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/bin/p1_extract` & `fusion-engine-client-1.20.0rc3/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/bin/p1_print` & `fusion-engine-client-1.20.0rc3/bin/p1_print`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import sys
 
 # Add the Python root directory (fusion-engine-client/python/) to the import search path to enable FusionEngine imports
 # if this application is being run directly out of the repository and is not installed as a pip package.
 root_dir = os.path.normpath(os.path.join(os.path.dirname(__file__), '..'))
 sys.path.insert(0, root_dir)
 
-root_dir = os.path.normpath(os.path.join(os.path.dirname(__file__), '..'))
-sys.path.append(root_dir)
 
 from fusion_engine_client.messages import *
 from fusion_engine_client.parsers import MixedLogReader
 from fusion_engine_client.utils import trace as logging
 from fusion_engine_client.utils.argument_parser import ArgumentParser, ExtendedBooleanAction
 from fusion_engine_client.utils.log import locate_log, DEFAULT_LOG_BASE_DIR
 from fusion_engine_client.utils.time_range import TimeRange
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1762,14 +1762,48 @@
                     name='Corrected Heading Solution Type'
                 ),
                 row=3, col=1
             )
 
         self._add_figure(name='heading_measurement', figure=fig, title='Measurements: Heading')
 
+    def plot_system_status_profiling(self):
+        """!
+        @brief Plot system status profiling data.
+        """
+        if self.output_dir is None:
+            return
+
+        # Read the data.
+        result = self.reader.read(message_types=[SystemStatusMessage], remove_nan_times=False, **self.params)
+        data = result[SystemStatusMessage.MESSAGE_TYPE]
+
+        if len(data.p1_time) == 0:
+            self.logger.info('No system status data available. Skipping plot.')
+            return
+
+        # Setup the figure.
+        figure = make_subplots(rows=1, cols=1, print_grid=False, shared_xaxes=True,
+                               subplot_titles=['GNSS Temperature'])
+
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
+        for i in range(1):
+            figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
+        figure['layout']['yaxis1'].update(title="Temp (deg C)")
+
+        # Plot the data.
+        time = data.p1_time - float(self.t0)
+        figure.add_trace(go.Scattergl(x=time, y=data.gnss_temperature_degc, customdata=data.p1_time,
+                                      name='GNSS Temperature',
+                                      hovertemplate='Time: %{x:.3f} sec (%{customdata:.3f} sec)',
+                                      mode='markers', line={'color': 'red'}),
+                         1, 1)
+
+        self._add_figure(name="profile_system_status", figure=figure, title="Profiling: System Status")
+
     def plot_events(self):
         """!
         @brief Generate a table of event notifications.
         """
         if self.output_dir is None:
             return
 
@@ -1936,31 +1970,61 @@
             # If the first pose is pretty close to t0, we'll assume the approximation is reasonably accurate and not
             # bother reporting it.
             t0_is_approx = dt_p1_sec > 10.0
         else:
             t0_gps = Timestamp()
             t0_is_approx = False
 
+        # Find the _processed_ t0, i.e., the first P1 and system times within the requested time range.
+        params = copy.deepcopy(self.params)
+        params['max_messages'] = 1
+        params['return_in_order'] = True
+
+        result = self.reader.read(message_types=None, require_p1_time=True, **params)
+        if len(result.messages) > 0:
+            processed_t0 = result.messages[0].get_p1_time()
+        else:
+            processed_t0 = Timestamp()
+
+        result = self.reader.read(message_types=None, require_system_time=True, **params)
+        if len(result.messages) > 0:
+            processed_system_t0 = result.messages[0].get_system_time_sec()
+        else:
+            processed_system_t0 = None
+
         # Create a table with log times and durations.
         descriptions = [
-            'Start Time',
+            'Log Start Time',
             '',
             '',
-            'Processed Duration',
             'Total Log Duration',
+            '',
+            'Processed Start Time',
+            '',
+            '',
+            'Processed Duration',
         ]
         times = [
+            # Log summary.
             str(self.reader.t0),
             system_time_to_str(self.reader.get_system_t0(), is_seconds=True).replace(' time', ':'),
             # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
             self._gps_sec_to_string(t0_gps) \
                 .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
                 .replace('<brbak>', '<br>'),
-            '%.1f seconds' % processing_duration_sec,
             log_duration_sec,
+            '',
+            # Processed data summary.
+            str(processed_t0),
+            system_time_to_str(processed_system_t0, is_seconds=True).replace(' time', ':'),
+            # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
+            self._gps_sec_to_string(t0_gps) \
+                .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
+                .replace('<brbak>', '<br>'),
+            '%.1f seconds' % processing_duration_sec,
         ]
         time_table = _data_to_table(['Description', 'Time'], [descriptions, times])
 
         # Create a table with the types and counts of each FusionEngine message type in the log.
         message_types, message_counts = np.unique(reduced_index['type'], return_counts=True)
         message_types = [MessageType.get_type_string(t) for t in message_types]
 
@@ -2107,20 +2171,16 @@
         if np.isnan(gps_time_sec):
             return "GPS: N/A<br>UTC: N/A"
         else:
             SECS_PER_WEEK = 7 * 24 * 3600.0
             week = int(gps_time_sec / SECS_PER_WEEK)
             tow_sec = gps_time_sec - week * SECS_PER_WEEK
             utc_time = gpstime.fromgps(gps_time_sec)
-
-            utc_time_str = utc_time.strftime('%Y-%m-%d %H:%M:%S')
-            utc_time_str += ('%.03f' % (utc_time.microsecond * 1e-6))[1:]
-
             return "GPS: %d:%.3f (%.3f sec)<br>UTC: %s" %\
-                   (week, tow_sec, gps_time_sec, utc_time_str)
+                   (week, tow_sec, gps_time_sec, datetime_to_string(utc_time, decimals=3))
 
     @classmethod
     def _get_measurement_time(cls, data, time_source: SystemTimeSource) -> np.ndarray:
         if time_source == SystemTimeSource.P1_TIME:
             return data.p1_time
         else:
             return data.measurement_time
@@ -2272,15 +2332,17 @@
     # Read pose data from the file.
     analyzer = Analyzer(file=input_path, output_dir=output_dir, ignore_index=options.ignore_index,
                         prefix=options.prefix + '.' if options.prefix is not None else '',
                         time_range=time_range,
                         truncate_long_logs=options.truncate and options.plot is None)
 
     if options.plot is None:
+        analyzer.plot_events()
         analyzer.plot_time_scale()
+
         analyzer.plot_solution_type()
         analyzer.plot_pose()
         analyzer.plot_pose_displacement()
         analyzer.plot_relative_position()
         analyzer.plot_map(mapbox_token=options.mapbox_token)
         analyzer.plot_calibration()
         analyzer.plot_gnss_cn0()
@@ -2292,15 +2354,15 @@
         # LG69T-AH), separate from other sensor measurements controlled by --measurements.
         analyzer.plot_heading_measurements()
 
         if options.measurements:
             analyzer.plot_imu()
             analyzer.plot_wheel_data()
 
-        analyzer.plot_events()
+        analyzer.plot_system_status_profiling()
     else:
         if len(options.plot) == 0:
             _logger.error('No plot names specified.')
             sys.exit(1)
 
         # Convert the user patterns into regex. The user is allowed to specify wildcards to match multiple figures.
         functions = set()
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/analysis/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,27 +319,30 @@
         #
         # We also disable numpy conversion and time alignment, since those features assume the data is being returned as
         # a dict separated by message type.
         if return_in_order:
             ignore_cache = True
             return_numpy = False
             time_align = TimeAlignmentMode.NONE
+            empty_result = MessageData(None, None)
+        else:
+            empty_result = {}
 
         # Parse the message types argument into a list of MessageType elements.
         if message_types is None:
             pass
         elif isinstance(message_types, MessageType):
             message_types = set((message_types,))
         elif MessagePayload.is_subclass(message_types):
             message_types = set((message_types.get_type(),))
-        else:
+        elif len(message_types) > 0:
             message_types = set([(t.get_type() if MessagePayload.is_subclass(t) else t) for t in message_types
                                  if t is not None])
             if len(message_types) == 0:
-                message_types = None
+                return empty_result
 
         # If the message type list is empty, read all messages.
         if message_types is None or len(message_types) == 0:
             message_types = list(message_type_to_class.keys())
 
         # If any of the requested types were already read from the file for the requested parameters, skip them.
         if ignore_cache:
@@ -393,38 +396,49 @@
             return result
 
         # Reset the filter criteria for the reader.
         if self.reader is None:
             raise IOError("File not open.")
         else:
             self.reader.rewind()
+            self.reader.clear_filters()
             self.reader.set_generate_index(self._generate_index and not disable_index_generation)
             self.reader.set_show_progress(show_progress)
             self.reader.set_max_bytes(max_bytes)
 
         # If we need to establish t0 (either P1 time or system time), we will wait to apply the user's filter criteria.
         # We can get t0 from any message type.
         reader_max_messages_applied = False
         if self.t0 is None or (self.system_t0 is None and system_time_messages_requested):
             logger.debug('Establishing t0. Postponing reader filter setup.')
             filters_applied = False
         else:
             filters_applied = True
 
-            self.reader.filter_in_place(message_types, clear_existing=True)
-            self.reader.filter_in_place(time_range, clear_existing=False)
+            self.reader.filter_in_place(time_range)
+            self.reader.filter_in_place(message_types)
+
+            # If the user is requiring (valid) P1 timestamps, filter to those now.
+            if require_p1_time and not system_time_messages_requested:
+                self.reader.filter_out_invalid_p1_times()
 
             # If the user requested max messages, tell the reader to return max N results. The reader only supports this
             # if it has an index file, so we still check for N ourselves below.
-            if max_messages is not None and self.reader.have_index():
+            #
+            # Additionally, if the caller requires the results to have (valid) system timestamps, we'll skip this here
+            # since we need to decode the messages to see if they have valid timestamps. The index only stores P1 time,
+            # not system time. The read_next() call below will apply this condition and only return messages with valid
+            # system time.
+            if (max_messages is not None and self.reader.have_index() and
+                not (require_system_time and system_time_messages_requested)):
                 reader_max_messages_applied = True
                 if max_messages >= 0:
-                    self.reader.filter_in_place(slice(None, max_messages), clear_existing=False)
+                    self.reader.filter_in_place(slice(None, max_messages))
                 else:
-                    self.reader.filter_in_place(slice(max_messages, None), clear_existing=False)
+                    self.reader.filter_in_place(slice(max_messages, None))
 
         # When the user requests max_messages < 0, they would like the _last_ N messages in the file. If the reader does
         # not have an index file, so we can't do a slice above, we will create a circular buffer and store the last N
         # messages we see.
         if max_messages is not None and max_messages < 0 and not reader_max_messages_applied:
             newest_messages = deque(maxlen=abs(max_messages))
         else:
@@ -436,16 +450,16 @@
                      (num_total, num_total - num_needed, 'N/A' if max_messages is None else str(max_messages),
                       str(time_range)))
 
         message_count = 0
         while True:
             try:
                 header, payload, message_bytes = \
-                    self.reader.read_next(require_p1_time=require_p1_time and filters_applied,
-                                          require_system_time=require_system_time and filters_applied)
+                    self.reader.read_next(require_p1_time=require_p1_time,
+                                          require_system_time=require_system_time)
             except StopIteration:
                 break
 
             message_size_bytes = header.get_message_size()
             message_offset_bytes = self.reader.get_bytes_read() - message_size_bytes
 
             # Unsupported/unrecognized message type.
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/configuration.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     EXPORT_DATA = 13111
     PLATFORM_STORAGE_DATA = 13113
 
     SET_MESSAGE_RATE = 13220
     GET_MESSAGE_RATE = 13221
     MESSAGE_RATE_RESPONSE = 13222
 
+    LBAND_FRAME = 14000
+
     RESERVED = 20000
 
     @classmethod
     def get_type_string(cls, value, include_value=True, raise_on_unrecognized=False):
         try:
             return cls(value, raise_on_unrecognized=True).to_string(include_value=include_value)
         except (KeyError, ValueError) as e:
@@ -209,18 +211,18 @@
 def is_response(message_type: MessageType) -> bool:
     return message_type in RESPONSE_MESSAGES
 
 
 class MessageHeader:
     INVALID_SOURCE_ID = 0xFFFFFFFF
 
-    _SYNC0 = 0x2E  # '.'
-    _SYNC1 = 0x31  # '1'
+    SYNC0 = 0x2E  # '.'
+    SYNC1 = 0x31  # '1'
 
-    SYNC = bytes((_SYNC0, _SYNC1))
+    SYNC = bytes((SYNC0, SYNC1))
 
     _FORMAT = '<BB2xIBBHIII'
     _SIZE: int = struct.calcsize(_FORMAT)
 
     _MAX_EXPECTED_SIZE_BYTES = (1 << 24)
 
     def __init__(self, message_type: MessageType = MessageType.INVALID):
@@ -283,15 +285,15 @@
         @return A `bytes` object containing the serialized message, or the size of the serialized content (in bytes).
         """
         # If the payload is specified, set the CRC and payload length, and then append the payload to the returned
         # result.
         if payload is not None:
             self.calculate_crc(payload)
 
-        args = (MessageHeader._SYNC0, MessageHeader._SYNC1, self.crc, self.protocol_version, self.message_version,
+        args = (MessageHeader.SYNC0, MessageHeader.SYNC1, self.crc, self.protocol_version, self.message_version,
                 int(self.message_type), self.sequence_number, self.payload_size_bytes, self.source_identifier)
         if buffer is None:
             buffer = struct.pack(MessageHeader._FORMAT, *args)
             if payload is not None:
                 buffer += payload
         else:
             struct.pack_into(MessageHeader._FORMAT, buffer, offset, *args)
@@ -300,36 +302,37 @@
                 buffer[offset:offset + len(payload)] = payload
 
         if return_buffer:
             return buffer
         else:
             return self.calcsize()
 
-    def unpack(self, buffer: bytes, offset: int = 0, validate_crc: bool = False,
+    def unpack(self, buffer: bytes, offset: int = 0, validate_sync: bool = False, validate_crc: bool = False,
                warn_on_unrecognized: bool = True) -> int:
         """!
         @brief Deserialize a message header and validate its sync bytes and CRC.
 
         @note
         If CRC validation is enabled, the complete message payload is assumed to follow the header in `buffer`.
 
         @param buffer A byte buffer containing a serialized message.
         @param offset The offset into the buffer (in bytes) at which the message header begins.
+        @param validate_sync If `True`, validate the sync bytes contained in the data buffer.
         @param validate_crc If `True`, validate the deserialized CRC against the data in the buffer.
         @param warn_on_unrecognized If `True`, print a warning if the message type is not listed in @ref MessageType.
 
         @return The size of the serialized header (in bytes).
         """
         (sync0, sync1,
          self.crc, self.protocol_version,
          self.message_version, message_type_int,
          self.sequence_number, self.payload_size_bytes, self.source_identifier) = \
             struct.unpack_from(MessageHeader._FORMAT, buffer, offset)
 
-        if sync0 != MessageHeader._SYNC0 or sync1 != MessageHeader._SYNC1:
+        if validate_sync and (sync0 != MessageHeader.SYNC0 or sync1 != MessageHeader.SYNC1):
             raise ValueError('Received invalid sync bytes. [sync0=0x%02x, sync1=0x%02x]' % (sync0, sync1))
 
         # Validate the CRC, assuming the message payload follows in the buffer.
         if validate_crc:
             self.validate_crc(buffer, offset)
 
         try:
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/device.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import math
 
 from construct import (Struct, Int16sl, Padding)
+import numpy as np
 
 from ..utils.construct_utils import FixedPointAdapter, construct_message_to_string
 from .defs import *
 
 
 class SystemStatusMessage(MessagePayload):
     """!
     @brief System status message.
     """
     MESSAGE_TYPE = MessageType.SYSTEM_STATUS
     MESSAGE_VERSION = 0
 
-    SystemStatusMessageConstruct = Struct(
+    Construct = Struct(
         "p1_time" / TimestampConstruct,
         "gnss_temperature_degc" / FixedPointAdapter(2 ** -7, Int16sl, invalid=0x7FFF),
         Padding(118),
     )
 
     def __init__(self):
         self.p1_time = Timestamp()
         self.gnss_temperature_degc = math.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         values = vars(self)
-        packed_data = self.SystemStatusMessageConstruct.build(values)
+        packed_data = self.Construct.build(values)
         return PackedDataToBuffer(packed_data, buffer, offset, return_buffer)
 
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
-        parsed = self.SystemStatusMessageConstruct.parse(buffer[offset:])
+        parsed = self.Construct.parse(buffer[offset:])
         self.__dict__.update(parsed)
         del self.__dict__['_io']
         return parsed._io.tell()
 
+    @classmethod
+    def calcsize(cls) -> int:
+        return cls.Construct.sizeof()
+
     def __repr__(self):
         result = super().__repr__()[:-1]
         result += f', gnss_temperature={self.gnss_temperature_degc:.1f} deg C]'
         return result
 
     def __str__(self):
-        string = 'System Status Message @ %s\n' % str(self.p1_time)
-        string += f'  GNSS Temperature: %.1f deg C' % self.gnss_temperature_degc
-        return string
-
-    def calcsize(self) -> int:
-        return self.SystemStatusMessageConstruct.sizeof()
+        return f"""\
+System Status Message @ %{self.p1_time}
+  GNSS Temperature: {self.gnss_temperature_degc:.1f} deg C"""
+
+    @classmethod
+    def to_numpy(cls, messages):
+        result = {
+            'p1_time': np.array([float(m.p1_time) for m in messages]),
+            'gnss_temperature_degc': np.array([m.gnss_temperature_degc for m in messages]),
+        }
+        return result
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,30 +104,34 @@
         self.solution_type = SolutionType(solution_type_int)
 
         return offset - initial_offset
 
     def __repr__(self):
         lla_str = '(%.6f, %.6f, %.3f)' % tuple(self.lla_deg)
         if self.gps_time:
-            gps_str = f'{str(self.gps_time).replace("GPS: ", "")}'
+            gps_str = f'{str(self.gps_time).replace("GPS: ", "")} ' \
+                      f'({datetime_to_string(self.gps_time.as_utc())} UTC)'
         else:
             gps_str = 'None'
 
         result = super().__repr__()[:-1]
         result += f', gps_time={gps_str}, solution_type={self.solution_type}, position={lla_str}]'
         return result
 
     def __str__(self):
         string = 'Pose Message @ %s\n' % str(self.p1_time)
         string += '  Solution type: %s\n' % self.solution_type.name
         if self.gps_time:
-            gps_str = f'{str(self.gps_time).replace("GPS: ", "")} ({str(self.gps_time.as_gps())})'
+            gps_str = f'{str(self.gps_time).replace("GPS: ", "")}'
+            utc_str = f'{datetime_to_string(self.gps_time.as_utc())}'
         else:
             gps_str = 'None'
+            utc_str = 'None'
         string += '  GPS time: %s\n' % gps_str
+        string += '  UTC time: %s\n' % utc_str
         string += '  Position (LLA): %.6f, %.6f, %.3f (deg, deg, m)\n' % tuple(self.lla_deg)
         string += '  Attitude (YPR): %.2f, %.2f, %.2f (deg, deg, deg)\n' % tuple(self.ypr_deg)
         string += '  Velocity (Body): %.2f, %.2f, %.2f (m/s, m/s, m/s)\n' % tuple(self.velocity_body_mps)
         string += '  Position std (ENU): %.2f, %.2f, %.2f (m, m, m)\n' % tuple(self.position_std_enu_m)
         string += '  Attitude std (YPR): %.2f, %.2f, %.2f (deg, deg, deg)\n' % tuple(self.ypr_std_deg)
         string += '  Velocity std (Body): %.2f, %.2f, %.2f (m/s, m/s, m/s)\n' % tuple(self.velocity_std_body_mps)
         string += '  Geoid undulation: %.2f m\n' % self.undulation_m
@@ -329,15 +333,16 @@
             self.corrections_age_sec = np.nan
             self.baseline_distance_m = np.nan
 
         return offset - initial_offset
 
     def __repr__(self):
         if self.gps_time:
-            gps_str = f'{str(self.gps_time).replace("GPS: ", "")}'
+            gps_str = f'{str(self.gps_time).replace("GPS: ", "")} ' \
+                      f'({datetime_to_string(self.gps_time.as_utc())} UTC)'
         else:
             gps_str = 'None'
         if self.reference_station_id != GNSSInfoMessage.INVALID_REFERENCE_STATION:
             station_str = str(self.reference_station_id)
         else:
             station_str = 'None'
 
@@ -345,18 +350,23 @@
         result += f', gps_time={gps_str}, num_svs={self.num_svs}, station={station_str}, ' \
                   f'age={self.corrections_age_sec:.1f} sec, baseline={self.baseline_distance_m * 1e-3:.1f} km]'
         return result
 
     def __str__(self):
         string = 'GNSS Info Message @ %s\n' % str(self.p1_time)
         if self.gps_time:
-            gps_str = f'{str(self.gps_time).replace("GPS: ", "")} ({str(self.gps_time.as_gps())})'
+            gps_str = f'{str(self.gps_time).replace("GPS: ", "")}'
         else:
             gps_str = 'None'
         string += '  GPS time: %s\n' % gps_str
+        if self.utc_time:
+            utc_str = f'{datetime_to_string(self.gps_time.as_utc())}'
+        else:
+            utc_str = 'None'
+        string += '  UTC time: %s\n' % utc_str
         string += '  UTC leap second: %s\n' % \
                   (self.leap_second if self.leap_second != GNSSInfoMessage.INVALID_LEAP_SECOND else 'unknown')
         string += '  # SVs used: %d\n' % self.num_svs
         string += ('  Reference station: %s\n' %
                    (str(self.reference_station_id)
                     if self.reference_station_id != GNSSInfoMessage.INVALID_REFERENCE_STATION
                     else 'none'))
@@ -852,15 +862,15 @@
             message=self,
             title=f'RelativeENUPosition @ {self.p1_time}',
             fields=['gps_time', 'solution_type', 'reference_station_id', 'relative_position_enu_m',
                     'position_std_enu_m'])
 
     @classmethod
     def calcsize(cls) -> int:
-        return cls.GetConfigMessageConstruct.sizeof()
+        return cls.Construct.sizeof()
 
     @classmethod
     def to_numpy(cls, messages: Sequence['RelativeENUPositionMessage']):
         result = {
             'p1_time': np.array([float(m.p1_time) for m in messages]),
             'gps_time': np.array([float(m.gps_time) for m in messages]),
             'solution_type': np.array([int(m.solution_type) for m in messages], dtype=int),
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/messages/timestamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union
 
 from datetime import datetime, timedelta, timezone
 import math
 import struct
 
 from construct import Adapter, Struct, Int32ul
+from gpstime import gpstime
 import numpy as np
 
 
 SECONDS_PER_WEEK = 7 * 24 * 3600.0
 
 GPS_POSIX_EPOCH = datetime(1980, 1, 6, tzinfo=timezone.utc)
 GPS_POSIX_EPOCH_SEC = GPS_POSIX_EPOCH.timestamp()
@@ -18,14 +19,24 @@
 # Used to distinguish between:
 # - P1 timestamps (0 at time of boot) vs GPS timestamps (referenced to 1/6/1980)
 # - System CPU/MCU monotonic timestamps (0 at time of boot) vs POSIX timestamps (referenced to 1/1/1970)
 Y2K_POSIX_SEC = datetime(2000, 1, 1, tzinfo=timezone.utc).timestamp()
 Y2K_GPS_SEC = (Y2K_POSIX_SEC - GPS_POSIX_EPOCH_SEC) + 13
 
 
+def datetime_to_string(time: datetime, decimals=3) -> str:
+    if time is None:
+        return 'None'
+    else:
+        time_str = time.strftime('%Y-%m-%d %H:%M:%S')
+        if decimals > 0:
+            time_str += (('%%.0%df' % decimals) % (time.microsecond * 1e-6))[1:]
+        return time_str
+
+
 def is_gps_time(value_sec: Union[float, np.ndarray]) -> Union[bool, np.ndarray]:
     """!
     @brief Test if a timestamp (or list of timestamps) is large enough to be presumed a GPS time (>2000/1/1).
 
     @param value_sec A timestamp or `ndarray` array of timestamps (in seconds).
 
     @return `True` if the timestamp appears to be a GPS timestamp.
@@ -49,14 +60,20 @@
 
     def as_gps(self) -> datetime:
         if self.is_gps():
             return GPS_POSIX_EPOCH + timedelta(seconds=self.seconds)
         else:
             return None
 
+    def as_utc(self) -> datetime:
+        if self.is_gps():
+            return gpstime.fromgps(self.seconds)
+        else:
+            return None
+
     def get_week_tow(self) -> (int, float):
         if self.is_gps():
             week = int(self.seconds / SECONDS_PER_WEEK)
             tow_sec = self.seconds - week * SECONDS_PER_WEEK
             return week, tow_sec
         else:
             return np.nan, np.nan
@@ -134,14 +151,17 @@
         if self.is_gps():
             return 'GPS: %d:%.3f (%.3f sec)' % (*self.get_week_tow(), self.seconds)
         else:
             return 'P1: %.3f sec' % self.seconds
 
 
 def system_time_to_str(system_time, is_seconds=False):
+    if system_time is None:
+        return 'None'
+
     if is_seconds:
         system_time_sec = system_time
     else:
         system_time_sec = system_time * 1e-9
 
     # Note: We're assuming no Point One device will ever operate before 2000/1/1, even in simulation, and that no
     # device will be running for 30 years continuously and have a system time > (2000 - 1970) seconds.
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

```diff
@@ -140,19 +140,19 @@
             # Message must be at least long enough for header.
             if len(self._buffer) < MessageHeader.calcsize():
                 break
             # Looking for a valid header.
             elif self._header is None:
                 # Explicitly check for the first two sync bytes to be a bit more efficient than doing it inside the @ref
                 # MessageHeader.unpack() with an exception.
-                if self._buffer[0] != MessageHeader._SYNC0:
+                if self._buffer[0] != MessageHeader.SYNC0:
                     self._buffer.pop(0)
                     self._bytes_processed += 1
                     continue
-                if self._buffer[1] != MessageHeader._SYNC1:
+                elif self._buffer[1] != MessageHeader.SYNC1:
                     self._buffer.pop(0)
                     self._bytes_processed += 1
                     continue
 
                 # Possible header found. Decode it and wait for the payload.
                 self._header = MessageHeader()
                 self._header.unpack(self._buffer, warn_on_unrecognized=False)
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/file_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,16 @@
         @param stop The P1 time at the end of the desired time range (exclusive).
         @param hint A hint indicating how to handle entries that do not have P1 time (`nan` timestamps):
                - `all_nans` - Return _all_ elements with nan timestamps in addition to entries within the time range,
                  including nan elements outside the time range
                - `include_nans` - Include nan elements within the requested time range (default)
                - `remove_nans` - Do not return nan elements; remove elements falling within the requested time range
         @param time_range A @ref TimeRange object to use instead of `start` and `stop`.
+
+        @return Returns a _copy_ of this class, limited to the requested range.
         """
         if hint is None:
             hint = 'include_nans'
 
         # If the caller provided a TimeRange object, use that to set start/stop.
         if time_range is not None:
             if start is not None or stop is not None:
@@ -327,16 +329,17 @@
         elif self.t0 is None:
             raise IndexError('No P1 timestamps present in index. Cannot apply time bounds.')
         else:
             # Note: The index stores only the integer part of the timestamp.
 
             # If self._data['time'] ends _before_ `start``, use 0 as start_idx. If self._data['time'] ends _after_
             # `end`, use len(self._data['time']) as end_idx.
-            start_idx = find_first(self._data['time'] >= np.floor(start)) if start is not None else 0
-            end_idx = find_first(self._data['time'] >= stop) if stop is not None else len(self._data)
+            with np.errstate(invalid='ignore'):
+                start_idx = find_first(self._data['time'] >= np.floor(start)) if start is not None else 0
+                end_idx = find_first(self._data['time'] >= stop) if stop is not None else len(self._data)
 
             if start_idx < 0:
                 start_idx = 0
 
             if end_idx < 0:
                 end_idx = len(self._data['time'])
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         self.return_payload = return_payload
         self.return_bytes = return_bytes
         self.return_offset = return_offset
 
         self._original_time_range = copy.deepcopy(time_range)
         self.time_range = copy.deepcopy(self._original_time_range)
 
+        self.remove_invalid_p1_time = False
+
         if message_types is None:
             self.message_types = None
         elif isinstance(message_types, MessageType):
             self.message_types = set((message_types,))
         elif MessagePayload.is_subclass(message_types):
             self.message_types = set((message_types.get_type(),))
         else:
@@ -116,15 +118,15 @@
         else:
             if os.path.exists(self.index_path):
                 try:
                     self.logger.debug("Loading index file '%s'." % self.index_path)
                     self._original_index = file_index.FileIndex(index_path=self.index_path, data_path=input_path,
                                                                 delete_on_error=generate_index)
                     self.index = self._original_index[self.message_types][self.time_range]
-                    self.filtered_message_types = len(np.unique(self._original_index.type)) !=\
+                    self.filtered_message_types = len(np.unique(self._original_index.type)) != \
                                                   len(np.unique(self.index.type))
                 except ValueError as e:
                     self.logger.error("Error loading index file: %s" % str(e))
             else:
                 self.logger.debug("No index file found @ '%s'." % self.index_path)
 
         self.index_builder = None
@@ -257,15 +259,16 @@
             try:
                 header = MessageHeader()
                 header.unpack(data, warn_on_unrecognized=False)
 
                 # Check if the payload is too big. If so, we most likely found an invalid header -- message sync bytes
                 # occurring randomly in non-FusionEngine binary data in the file.
                 if header.payload_size_bytes > MessageHeader._MAX_EXPECTED_SIZE_BYTES:
-                    raise ValueError('Payload size (%d) too large.' % header.payload_size_bytes)
+                    raise ValueError('Payload size (%d) too large. [message_type=%s]' %
+                                     (header.payload_size_bytes, header.get_type_string()))
 
                 # Read and validate the payload.
                 #
                 # Note here that we can read < payload_size_bytes under 2 circumstances:
                 # 1. We reached EOF unexpectedly: we found a valid message header but the file doesn't contain the
                 #    complete message.
                 # 2. We found an invalid header but its (bogus) payload length, while not large enough to trigger the
@@ -276,15 +279,16 @@
                 #
                 # If the CRC fails, either because we found an invalid header or because a valid message got corrupted,
                 # validate_crc() will raise a ValueError and we will skip forward in the same manner.
                 payload_bytes = self.input_file.read(header.payload_size_bytes)
                 read_len += len(payload_bytes)
                 self.total_bytes_read += len(payload_bytes)
                 if len(payload_bytes) != header.payload_size_bytes:
-                    raise ValueError('Not enough data - likely not a valid FusionEngine header.')
+                    raise ValueError('Not enough data - likely not a valid FusionEngine header. [message_type=%s]' %
+                                     header.get_type_string())
 
                 data += payload_bytes
                 header.validate_crc(data)
 
                 message_length_bytes = MessageHeader.calcsize() + header.payload_size_bytes
                 if self.logger.isEnabledFor(logging.getTraceLevel(depth=1)):
                     self.logger.trace('Read %s message @ %d (0x%x). [length=%d B, sequence=%d, # messages=%d]' %
@@ -333,30 +337,35 @@
                     if require_p1_time and (payload is None or payload.get_p1_time() is None):
                         self.logger.trace("Skipping %s message. P1 time requested." % header.get_type_string())
                         continue
                     elif require_system_time and (payload is None or payload.get_system_time_ns() is None):
                         self.logger.trace("Skipping %s message. System time requested." % header.get_type_string())
                         continue
 
+                # Extract P1 time if available.
+                p1_time = payload.get_p1_time() if payload is not None else Timestamp()
+
                 # Add this message to the index file.
                 if self.index_builder is not None and generate_index:
-                    p1_time = payload.get_p1_time() if payload is not None else None
                     self.index_builder.append(message_type=header.message_type, offset_bytes=start_offset_bytes,
                                               p1_time=p1_time)
 
                 # Now, if this message is not in the user-specified filter criteria, skip it.
                 #
                 # If we have an index available, this is implied by the index (we won't seek to messages that don't meet
                 # the criteria at all), so we do not need to do this check. Further, self.message_types and
                 # self.time_range are _only_ valid if we are _not_ using an index, so this may end up incorrectly
                 # filtering out some messages as unwanted.
                 if self.index is None:
                     if self.message_types is not None and header.message_type not in self.message_types:
                         self.logger.trace("Message type not requested. Skipping.", depth=1)
                         continue
+                    elif self.remove_invalid_p1_time and not p1_time:
+                        self.logger.trace("Message does not have valid P1 time. Skipping.", depth=1)
+                        continue
                     elif self.time_range is not None and not self.time_range.is_in_range(payload):
                         if self.time_range.in_range_started() and (self.index_builder is None or not generate_index):
                             self.logger.debug("End of time range reached. Finished processing.")
                             break
                         else:
                             self.logger.trace("Message not in time range. Skipping.", depth=1)
                             continue
@@ -388,14 +397,16 @@
         # If we are creating an index file, save it now.
         if self.index_builder is not None and generate_index:
             self.logger.debug("Saving index file as '%s'." % self.index_path)
             self._original_index = self.index_builder.save(self.index_path, self.input_file.name)
             self.index_builder = None
 
             self.index = self._original_index[self.message_types][self.time_range]
+            if self.remove_invalid_p1_time:
+                self.index = self.index.get_time_range(hint='remove_nans')
             self.message_types = None
             self.time_range = None
             self.next_index_elem = len(self.index)
 
         # Finished iterating.
         if force_eof:
             return
@@ -413,22 +424,22 @@
                     if self.total_bytes_read + 1 >= self.max_bytes:
                         self.logger.debug('Max read length exceeded (%d B).' % self.max_bytes)
                         return False
 
                     byte0 = self.input_file.read(1)[0]
                     self.total_bytes_read += 1
                     while True:
-                        if byte0 == MessageHeader._SYNC0:
+                        if byte0 == MessageHeader.SYNC0:
                             if self.total_bytes_read + 1 >= self.max_bytes:
                                 self.logger.debug('Max read length exceeded (%d B).' % self.max_bytes)
                                 return False
 
                             byte1 = self.input_file.read(1)[0]
                             self.total_bytes_read += 1
-                            if byte1 == MessageHeader._SYNC1:
+                            if byte1 == MessageHeader.SYNC1:
                                 self.input_file.seek(-2, os.SEEK_CUR)
                                 self.total_bytes_read -= 2
                                 if self.logger.isEnabledFor(logging.getTraceLevel(depth=3)):
                                     self.logger.trace('Sync bytes found @ %d (0x%x).' %
                                                       (self.total_bytes_read, self.total_bytes_read),
                                                       depth=3)
                                 return True
@@ -464,27 +475,32 @@
             self.logger.log(logging.INFO if show_progress else logging.DEBUG,
                             'Processed %d/%d bytes (%.1f%%). [elapsed=%.1f sec, rate=%.1f MB/s]' %
                             (self.total_bytes_read, file_size,
                              100.0 if file_size == 0 else 100.0 * float(self.total_bytes_read) / file_size,
                              elapsed_sec, (self.total_bytes_read / elapsed_sec / 1e6) if elapsed_sec > 0 else np.nan))
             self.last_print_bytes = self.total_bytes_read
 
+    def clear_filters(self):
+        self.filter_in_place(key=None, clear_existing=True)
+
     def filter_in_place(self, key, clear_existing: bool = False):
         """!
         @brief Limit the returned messages by type or time.
 
         @warning
         This operator modifies this class in-place.
 
         @param key One of the following:
                - An individual @ref MessageType to be returned
                - An iterable listing one or more @ref MessageType%s to be returned
                - A `slice` specifying the start/end of the desired absolute (P1) or relative time range
                - A @ref TimeRange object
         @param clear_existing If `True`, clear any previous filter criteria.
+
+        @return A reference to this class.
         """
         # If we're reading using an index, determine the offset within the data file of the most recent message we have
         # read. Then below, after we filter the index down (or clear existing filtering), we'll locate the next entry to
         # be read in the file that meets the new criteria. That way we continue where we left off.
         #
         # If we're reading directly from the file without an index, we'll just pick up where the current seek is, so no
         # need to do anything special.
@@ -497,24 +513,25 @@
                 prev_offset_bytes = self.index.offset[self.next_index_elem - 1]
 
         # If requested, clear previous filter criteria.
         if clear_existing:
             if self.index is None:
                 self.message_types = copy.deepcopy(self._original_message_types)
                 self.time_range = copy.deepcopy(self._original_time_range)
+                self.remove_invalid_p1_time = False
             else:
                 self.index = self._original_index
 
         # No key specified (convenience case).
         if key is None:
             pass
         # If we have an index file available, reduce the index to the requested criteria.
         elif self.index is not None:
             self.index = self.index[key]
-            self.filtered_message_types = len(np.unique(self._original_index.type)) !=\
+            self.filtered_message_types = len(np.unique(self._original_index.type)) != \
                                           len(np.unique(self.index.type))
         # Otherwise, store the criteria and apply them while reading.
         else:
             # Return entries for a specific message type.
             if isinstance(key, MessageType):
                 self.message_types = set((key,))
                 self.filtered_message_types = True
@@ -567,14 +584,34 @@
                 if idx == 0 and self.index.offset[0] <= prev_offset_bytes:
                     self.next_index_elem = len(self.index)
                 else:
                     self.next_index_elem = idx
 
         return self
 
+    def filter_out_invalid_p1_times(self, clear_existing: bool = False):
+        """!
+        @brief Limit the returned messages, removing any messages that do not have valid P1 time.
+
+        @param clear_existing If `True`, clear any previous filter criteria.
+
+        @return A reference to this class.
+        """
+        self.filter_in_place(key=None, clear_existing=clear_existing)
+
+        # If we have an index file available, reduce the index to the requested criteria.
+        if self.index is not None:
+            self.index = self.index.get_time_range(hint='remove_nans')
+            self.filtered_message_types = len(np.unique(self._original_index.type)) != \
+                                          len(np.unique(self.index.type))
+        else:
+            self.remove_invalid_p1_time = True
+
+        return self
+
     def __iter__(self):
         return self
 
     def __next__(self):
         return self.next()
 
     @classmethod
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,20 +192,24 @@
 
     @return The path to the located file or a tuple containing:
             - The path to the located file.
             - The path to the located output directory. Only provided if `return_output_dir` is `True`.
             - The log ID string, or `None` if the requested file is not part of a FusionEngine log. Only provided if
               `return_log_id` is `True`.
     """
+    def _get_log_id(file_path):
+        parent_dir = os.path.dirname(os.path.abspath(input_path))
+        return os.path.basename(parent_dir)
+
     # Check if the input path is a file. If so, return it and set the output directory to its parent directory.
     if os.path.isfile(input_path) and check_exact_match:
         output_dir = os.path.dirname(input_path)
         if output_dir == "":
             output_dir = "."
-        log_id = None
+        log_id = _get_log_id(input_path)
     # If the input path is a directory, see if it's a P1 log. If it is not a directory, see if it pattern matches to a
     # log directory within `log_base_dir`. If so for either case, set the output directory to the log directory (note
     # that the .p1log may be contained within a subdirectory).
     else:
         if candidate_files is None:
             # No candidate files specified. Default to 'fusion_engine.p1log'.
             candidate_files = ['fusion_engine.p1log']
@@ -220,15 +224,15 @@
         def _search_directory(dir_path):
             for f in candidate_files:
                 if f is None:
                     continue
 
                 test_path = os.path.join(dir_path, f)
                 if os.path.exists(test_path):
-                    return test_path, dir_path, os.path.basename(dir_path)
+                    return test_path, dir_path, _get_log_id(test_path)
             return None, None, None
 
         if check_exact_match:
             dir_exists = os.path.isdir(input_path)
             if dir_exists:
                 matching_input_path, log_dir, log_id = _search_directory(input_path)
                 if matching_input_path is not None:
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/numpy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     @return First index of input array which is `True`. If all elements are `False`, returns -1.
     """
     if arr.dtype != bool:
         raise ValueError('Input array is not a boolean array.')
     elif len(arr) == 0:
         return -1
     else:
-        idx = np.argmax(arr)
+        idx = np.nanargmax(arr)
         if idx == 0 and not arr[0]:
             return -1
         else:
             return idx
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc3/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc2
+Version: 1.20.0rc3
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc2/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc3/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 fusion_engine_client/messages/__init__.py
 fusion_engine_client/messages/configuration.py
 fusion_engine_client/messages/control.py
 fusion_engine_client/messages/core.py
 fusion_engine_client/messages/defs.py
 fusion_engine_client/messages/device.py
 fusion_engine_client/messages/fault_control.py
+fusion_engine_client/messages/gnss_corrections.py
 fusion_engine_client/messages/measurement_details.py
 fusion_engine_client/messages/measurements.py
 fusion_engine_client/messages/ros.py
 fusion_engine_client/messages/signal_defs.py
 fusion_engine_client/messages/solution.py
 fusion_engine_client/messages/timestamp.py
 fusion_engine_client/parsers/__init__.py
```

### Comparing `fusion-engine-client-1.20.0rc2/setup.py` & `fusion-engine-client-1.20.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     raise RuntimeError("Unable to find version string.")
 
 
 version = find_version('fusion_engine_client', '__init__.py')
 
 tools_requirements = set([
     'argparse-formatter>=1.4',
-    'gpstime>=0.6.2',
     'scipy>=1.6.0',
 ])
 
 display_requirements = set([
     'colorama>=0.4.4',
     'palettable>=3.3.0',
     'plotly>=4.0.0',
@@ -75,14 +74,15 @@
     ],
     python_requires='>3.7',
     setup_requires=[
         'wheel>=0.36.2',
     ],
     install_requires=[
         'aenum>=3.1.1',
+        'gpstime>=0.6.2',
         'numpy>=1.16.0',
         'construct>=2.10.0',
     ],
     extras_require={
         'all': list(all_requirements),
         'dev': list(dev_requirements),
         'display': list(display_requirements),
```

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_config.py` & `fusion-engine-client-1.20.0rc3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc3/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc3/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc3/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc3/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc3/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc3/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc2/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc3/tests/test_time_range.py`

 * *Files identical despite different names*

