# Comparing `tmp/openedx-events-8.0.1.tar.gz` & `tmp/openedx-events-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-8.0.1.tar", last modified: Thu Jun  1 21:09:17 2023, max compression
+gzip compressed data, was "openedx-events-8.2.0.tar", last modified: Fri Jun 23 13:07:01 2023, max compression
```

## Comparing `openedx-events-8.0.1.tar` & `openedx-events-8.2.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.056703 openedx-events-8.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     8998 2023-06-01 21:09:12.000000 openedx-events-8.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-01 21:09:12.000000 openedx-events-8.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-01 21:09:12.000000 openedx-events-8.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15024 2023-06-01 21:09:17.056703 openedx-events-8.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-06-01 21:09:12.000000 openedx-events-8.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5655 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.056703 openedx-events-8.0.1/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/management/commands/consume_events.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.056703 openedx-events-8.0.1/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-06-01 21:09:12.000000 openedx-events-8.0.1/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.052703 openedx-events-8.0.1/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15024 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 21:09:17.000000 openedx-events-8.0.1/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.056703 openedx-events-8.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-01 21:09:12.000000 openedx-events-8.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-01 21:09:17.056703 openedx-events-8.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-06-01 21:09:12.000000 openedx-events-8.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 21:09:17.056703 openedx-events-8.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-01 21:09:12.000000 openedx-events-8.0.1/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-23 13:06:56.000000 openedx-events-8.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-23 13:06:56.000000 openedx-events-8.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-23 13:06:56.000000 openedx-events-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-06-23 13:07:01.404430 openedx-events-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-23 13:06:56.000000 openedx-events-8.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9087 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-23 13:06:56.000000 openedx-events-8.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-23 13:07:01.404430 openedx-events-8.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-06-23 13:06:56.000000 openedx-events-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-23 13:06:56.000000 openedx-events-8.2.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-8.0.1/CHANGELOG.rst` & `openedx-events-8.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,26 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.2.0] - 2023-06-08
+--------------------
+Changed
+~~~~~~~
+* Added new USER_NOTIFICATION_REQUESTED event.
+
+[8.1.0] - 2023-06-06
+--------------------
+Added
+~~~~~
+* Store current versions of Avro schemas and add test to ensure valid evolution
+
 [8.0.1] - 2023-05-16
 --------------------
 Changed
 ~~~~~~~
 * Fixed event_type of XBLOCK_SKILL_VERIFIED signal
 
 [8.0.0] - 2023-05-16
```

### Comparing `openedx-events-8.0.1/LICENSE.txt` & `openedx-events-8.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/PKG-INFO` & `openedx-events-8.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.0.1
+Version: 8.2.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -161,15 +161,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-events
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-events.svg
     :target: https://pypi.python.org/pypi/openedx-events/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-events/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-events/actions
@@ -206,14 +206,26 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.2.0] - 2023-06-08
+--------------------
+Changed
+~~~~~~~
+* Added new USER_NOTIFICATION_REQUESTED event.
+
+[8.1.0] - 2023-06-06
+--------------------
+Added
+~~~~~
+* Store current versions of Avro schemas and add test to ensure valid evolution
+
 [8.0.1] - 2023-05-16
 --------------------
 Changed
 ~~~~~~~
 * Fixed event_type of XBLOCK_SKILL_VERIFIED signal
 
 [8.0.0] - 2023-05-16
```

### Comparing `openedx-events-8.0.1/README.rst` & `openedx-events-8.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-events
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-events.svg
     :target: https://pypi.python.org/pypi/openedx-events/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-events/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-events/actions
```

### Comparing `openedx-events-8.0.1/openedx_events/content_authoring/data.py` & `openedx-events-8.2.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/content_authoring/signals.py` & `openedx-events-8.2.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/data.py` & `openedx-events-8.2.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/__init__.py` & `openedx-events-8.2.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/schema.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/serializer.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from openedx_events.event_bus.avro.custom_serializers import BaseCustomTypeAvroSerializer
 from openedx_events.event_bus.avro.deserializer import AvroSignalDeserializer
 from openedx_events.event_bus.avro.serializer import AvroSignalSerializer
 from openedx_events.event_bus.avro.types import PYTHON_TYPE_TO_AVRO_MAPPING
 from openedx_events.tooling import OpenEdxPublicSignal
 
 
-def create_simple_signal(data_dict):
+def create_simple_signal(data_dict, event_type="simple.signal"):
     """
     Create a basic OpenEdxPublicSignal with init_data = data_dict.
 
     Arguments:
         data_dict: Description of attributes passed to the signal
+        event_type: A custom event type string. Defaults to 'simple.signal'
     """
     return OpenEdxPublicSignal(
-        event_type="simple.signal",
+        event_type=event_type,
         data=data_dict
     )
 
 
 # Useful simple attr classes
 @attr.s(auto_attribs=True)
 class SimpleAttrs:
```

### Comparing `openedx-events-8.0.1/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-8.2.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/exceptions.py` & `openedx-events-8.2.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/learning/data.py` & `openedx-events-8.2.0/openedx_events/learning/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -231,7 +231,29 @@
         verified_skills (List[int]): list of verified skill ids.
         ignored_skills (List[int]): list of ignored skill ids.
     """
 
     usage_key = attr.ib(type=UsageKey)
     verified_skills = attr.ib(type=List[int], factory=list)
     ignored_skills = attr.ib(type=List[int], factory=list)
+
+
+@attr.s(frozen=True)
+class UserNotificationData:
+    """
+    Attributes defined for Open edX User Notification data object.
+
+    Arguments:
+        user_ids (List(int)): identifier of the user to which the notification belongs.
+        notification_type (str): type of the notification.
+        context (dict): additional structured information about the context in
+                        which this topic is used, such as the section, subsection etc.
+        content_url (str): url of the content.
+        app_name (str): name of the app.
+    """
+
+    user_ids = attr.ib(type=List[int])
+    notification_type = attr.ib(type=str)
+    content_url = attr.ib(type=str)
+    app_name = attr.ib(type=str)
+    course_key = attr.ib(type=CourseKey)
+    context = attr.ib(type=dict, factory=dict)
```

### Comparing `openedx-events-8.0.1/openedx_events/learning/signals.py` & `openedx-events-8.2.0/openedx_events/learning/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from openedx_events.learning.data import (
     CertificateData,
     CohortData,
     CourseDiscussionConfigurationData,
     CourseEnrollmentData,
     PersistentCourseGradeData,
     UserData,
+    UserNotificationData,
     XBlockSkillVerificationData,
 )
 from openedx_events.tooling import OpenEdxPublicSignal
 
 # .. event_type: org.openedx.learning.student.registration.completed.v1
 # .. event_name: STUDENT_REGISTRATION_COMPLETED
 # .. event_description: emitted when the user registration process in the LMS is completed.
@@ -157,7 +158,20 @@
 # .. event_data: XBlockSkillVerificationData
 XBLOCK_SKILL_VERIFIED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.xblock.skill.verified.v1",
     data={
         "xblock_info": XBlockSkillVerificationData,
     }
 )
+
+# .. event_type: org.openedx.learning.user.notification.requested.v1
+# .. event_name: USER_NOTIFICATION
+# .. event_description: Can be fired from apps to send user notifications.
+# .. event_data: UserNotificationSendListData
+# Warning: This event is currently incompatible with the event bus, list/dict cannot be serialized yet
+#
+USER_NOTIFICATION_REQUESTED = OpenEdxPublicSignal(
+    event_type="org.openedx.learning.user.notification.requested.v1",
+    data={
+        "notification_data": UserNotificationData,
+    }
+)
```

### Comparing `openedx-events-8.0.1/openedx_events/management/commands/consume_events.py` & `openedx-events-8.2.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/tests/test_consume_events_command.py` & `openedx-events-8.2.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/tests/test_tooling.py` & `openedx-events-8.2.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/tests/utils.py` & `openedx-events-8.2.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events/tooling.py` & `openedx-events-8.2.0/openedx_events/tooling.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 
 from openedx_events.data import EventsMetadata
 from openedx_events.exceptions import SenderValidationError
 from openedx_events.utils import format_responses
 
 log = getLogger(__name__)
 
+# If a signal is explicitly not for use with the event bus, add it to this list
+#  and document why in the event's annotations
+KNOWN_UNSERIALIZABLE_SIGNALS = [
+    "org.openedx.learning.discussions.configuration.changed.v1",
+    "org.openedx.content_authoring.course.certificate_config.changed.v1",
+    "org.openedx.content_authoring.course.certificate_config.deleted.v1",
+    "org.openedx.learning.user.notification.requested.v1"
+]
+
 
 class OpenEdxPublicSignal(Signal):
     """
     Standardized Django Signals used to create Open edX events.
     """
 
     _mapping = {}
```

### Comparing `openedx-events-8.0.1/openedx_events/utils.py` & `openedx-events-8.2.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.0.1/openedx_events.egg-info/PKG-INFO` & `openedx-events-8.2.0/openedx_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.0.1
+Version: 8.2.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -161,15 +161,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-events
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-events.svg
     :target: https://pypi.python.org/pypi/openedx-events/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-events/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-events/actions
@@ -206,14 +206,26 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.2.0] - 2023-06-08
+--------------------
+Changed
+~~~~~~~
+* Added new USER_NOTIFICATION_REQUESTED event.
+
+[8.1.0] - 2023-06-06
+--------------------
+Added
+~~~~~
+* Store current versions of Avro schemas and add test to ensure valid evolution
+
 [8.0.1] - 2023-05-16
 --------------------
 Changed
 ~~~~~~~
 * Fixed event_type of XBLOCK_SKILL_VERIFIED signal
 
 [8.0.0] - 2023-05-16
```

### Comparing `openedx-events-8.0.1/openedx_events.egg-info/SOURCES.txt` & `openedx-events-8.2.0/openedx_events.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -35,13 +35,15 @@
 openedx_events/event_bus/tests/test_loader.py
 openedx_events/learning/__init__.py
 openedx_events/learning/data.py
 openedx_events/learning/signals.py
 openedx_events/management/__init__.py
 openedx_events/management/commands/__init__.py
 openedx_events/management/commands/consume_events.py
+openedx_events/management/commands/generate_avro_schemas.py
 openedx_events/tests/__init__.py
 openedx_events/tests/test_consume_events_command.py
+openedx_events/tests/test_generate_avro_schemas.py
 openedx_events/tests/test_tooling.py
 openedx_events/tests/utils.py
 requirements/base.in
 tests/test_openedx_events.py
```

### Comparing `openedx-events-8.0.1/setup.py` & `openedx-events-8.2.0/setup.py`

 * *Files identical despite different names*

