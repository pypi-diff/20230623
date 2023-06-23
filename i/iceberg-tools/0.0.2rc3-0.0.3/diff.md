# Comparing `tmp/iceberg_tools-0.0.2rc3.tar.gz` & `tmp/iceberg_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg_tools-0.0.2rc3.tar", last modified: Fri May 26 23:16:19 2023, max compression
+gzip compressed data, was "iceberg_tools-0.0.3.tar", last modified: Fri Jun 23 21:40:11 2023, max compression
```

## Comparing `iceberg_tools-0.0.2rc3.tar` & `iceberg_tools-0.0.3.tar`

### file list

```diff
@@ -1,77 +1,84 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.065983 iceberg_tools-0.0.2rc3/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2940 2023-05-26 23:16:19.065744 iceberg_tools-0.0.2rc3/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2023-05-26 23:14:20.000000 iceberg_tools-0.0.2rc3/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.021742 iceberg_tools-0.0.2rc3/iceberg_tools/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 16:19:26.000000 iceberg_tools-0.0.2rc3/iceberg_tools/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.034784 iceberg_tools-0.0.2rc3/iceberg_tools/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142      482 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6024 2023-05-26 23:00:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/data.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5048 2023-05-26 23:02:49.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/schema.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.036178 iceberg_tools-0.0.2rc3/iceberg_tools/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-25 15:58:53.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.036641 iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/
--rw-r--r--   0 walsbr   (320923486) 1971611142    13714 2023-05-26 19:23:29.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-05-25 19:18:02.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/pfb.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3530 2023-05-26 23:02:01.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/report.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.037595 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142    26369 2023-05-26 21:11:37.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-05-23 18:08:13.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/oid_lookup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.039401 iceberg_tools-0.0.2rc3/iceberg_tools/schema/
--rw-r--r--   0 walsbr   (320923486) 1971611142    11116 2023-05-26 16:55:34.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1348 2023-05-13 22:22:19.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/bmeg.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    20425 2023-05-26 15:19:47.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4157 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-05-25 15:57:02.000000 iceberg_tools-0.0.2rc3/iceberg_tools/util.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.027235 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2940 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2263 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-26 23:16:19.066059 iceberg_tools-0.0.2rc3/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5751 2023-05-26 23:06:27.000000 iceberg_tools-0.0.2rc3/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.008616 iceberg_tools-0.0.2rc3/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.039748 iceberg_tools-0.0.2rc3/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:03.000000 iceberg_tools-0.0.2rc3/tests/integration/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.058505 iceberg_tools-0.0.2rc3/tests/integration/bmeg/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-05-15 20:39:46.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      967 2023-05-15 20:24:40.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-05-15 20:39:22.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_load_granular_reference.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2736 2023-05-15 20:39:04.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-05-15 20:38:41.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_invalid_edges.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-05-15 20:24:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_lathe_lint.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      662 2023-05-15 20:38:23.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_negative_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-05-23 20:22:18.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-05-15 20:38:10.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_spot_check_embedded_type.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-05-15 20:37:50.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_edge_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      888 2023-05-15 20:37:28.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_yaml_anonymous_schemas.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.060159 iceberg_tools-0.0.2rc3/tests/integration/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-23 23:15:41.000000 iceberg_tools-0.0.2rc3/tests/integration/data/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      305 2023-05-26 22:58:19.000000 iceberg_tools-0.0.2rc3/tests/integration/data/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5374 2023-05-26 22:55:04.000000 iceberg_tools-0.0.2rc3/tests/integration/data/test_pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.063699 iceberg_tools-0.0.2rc3/tests/integration/gen3/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 18:03:42.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      616 2023-05-18 20:08:55.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-05-15 20:20:57.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_codeable_concept.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      451 2023-05-15 20:17:07.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_embedded_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-14 12:07:10.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_identifiers.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-05-12 18:57:49.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_individual_yaml.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-05-12 18:56:56.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_keys.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-05-23 19:23:34.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_primitive.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-05-15 20:06:10.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_quantities.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-05-18 20:10:27.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_research_study_has_project.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      155 2023-05-24 00:59:54.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1832 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_medication.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1744 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_task.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-05-18 20:08:09.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_task.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.064178 iceberg_tools-0.0.2rc3/tests/integration/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-26 14:08:42.000000 iceberg_tools-0.0.2rc3/tests/integration/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1080 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/simplifier/test_simplify.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.065384 iceberg_tools-0.0.2rc3/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:24.000000 iceberg_tools-0.0.2rc3/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-05-15 20:40:27.000000 iceberg_tools-0.0.2rc3/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 iceberg_tools-0.0.2rc3/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/unit/test_schema.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.287735 iceberg_tools-0.0.3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3070 2023-06-23 21:40:11.287465 iceberg_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2337 2023-06-23 21:38:25.000000 iceberg_tools-0.0.3/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.213880 iceberg_tools-0.0.3/iceberg_tools/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.224734 iceberg_tools-0.0.3/iceberg_tools/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      510 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5947 2023-06-23 21:37:38.000000 iceberg_tools-0.0.3/iceberg_tools/cli/data.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4902 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/cli/schema.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.229253 iceberg_tools-0.0.3/iceberg_tools/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.229629 iceberg_tools-0.0.3/iceberg_tools/data/migrator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13714 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/migrator/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/pfb.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3530 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/report.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.230927 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    29385 2023-06-11 13:19:39.000000 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/oid_lookup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.232754 iceberg_tools-0.0.3/iceberg_tools/graph/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      212 2023-06-23 21:26:39.000000 iceberg_tools-0.0.3/iceberg_tools/graph/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.240782 iceberg_tools-0.0.3/iceberg_tools/schema/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11282 2023-06-02 23:22:12.000000 iceberg_tools-0.0.3/iceberg_tools/schema/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.249711 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:09:01.000000 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3629 2023-06-02 23:24:05.000000 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/binding_lookup.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1349 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/schema/graph.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    24435 2023-06-09 19:07:39.000000 iceberg_tools-0.0.3/iceberg_tools/schema/simplified.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4355 2023-06-09 13:56:59.000000 iceberg_tools-0.0.3/iceberg_tools/schema/simplified_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/util.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.219869 iceberg_tools-0.0.3/iceberg_tools.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3070 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2610 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-23 21:40:11.287800 iceberg_tools-0.0.3/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5748 2023-06-23 21:39:15.000000 iceberg_tools-0.0.3/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.210299 iceberg_tools-0.0.3/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.250716 iceberg_tools-0.0.3/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/integration/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.252777 iceberg_tools-0.0.3/tests/integration/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      305 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.254346 iceberg_tools-0.0.3/tests/integration/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1296 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/simplifier/test_simplify.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5605 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/test_pfb.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.281854 iceberg_tools-0.0.3/tests/integration/graph/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      972 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_edge_load_granular_reference.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2743 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_edge_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_invalid_edges.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_lathe_lint.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      663 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_negative_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_schema_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_spot_check_embedded_type.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_trivial_edge_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      889 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_yaml_anonymous_schemas.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.285752 iceberg_tools-0.0.3/tests/integration/simplified/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      665 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_codeable_concept.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      378 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_embedded_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_identifiers.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_individual_yaml.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_keys.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_primitive.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_quantities.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_research_study_has_project.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      216 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1830 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_medication.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1742 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_task.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      665 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_specimen_plucked_properties.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_task.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.287042 iceberg_tools-0.0.3/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/unit/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11142 2023-06-09 18:29:35.000000 iceberg_tools-0.0.3/tests/unit/test_simplify.py
```

### Comparing `iceberg_tools-0.0.2rc3/PKG-INFO` & `iceberg_tools-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg_tools
-Version: 0.0.2rc3
+Version: 0.0.3
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
@@ -48,41 +48,42 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   generate  Generate from FHIR resources.
   compile   Create aggregated json file from individual yaml schemas
-  publish   Copy dictionary to s3 (note:aws cli dependency)
 
 $ iceberg data
 
 Usage: iceberg data [OPTIONS] COMMAND [ARGS]...
 
   Project data (ResearchStudy, ResearchSubjects, Patient, etc.).
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  simplify       Renders Gen3 friendly flattened records.
-  validate       Check FHIR data for validity and ACED conventions.
-  validate-gen3  Check Gen3 data for validity and ACED conventions.
-  pfb            Write simplified FHIR files to a PFB.
-  migrate        Migrate from FHIR R4B to R5.0.
+  simplify             Renders PFB friendly flattened records.
+  validate             Check FHIR data for validity and conventions.
+  validate-simplified  Check simplified data for validity and conventions.
+  pfb                  Write simplified FHIR files to a PFB.
+  migrate              Migrate from FHIR R4B to R5.0.
+  report               Aggregate avro pfb files into a cytoscape tsv.
 
 ```
 
 > Note: `pfb_fhir` and `iceberg` are synonymous in this context.
 
 ## Examples
 
 The commands:
 ```commandline
-pfb_fhir data simplify  tests/fixtures/simplify/study/ tmp/simplified
+pfb_fhir schema generate simplified
+pfb_fhir data simplify --schema_path  iceberg/schemas/simplified/simplified-fhir.json tests/fixtures/simplify/study/ tmp/simplified
 pfb_fhir data pfb tmp/simplified/ tmp/study.pfb
 tree tmp
 
 ```
 
 Will generate the following output:
 ```commandline
```

### Comparing `iceberg_tools-0.0.2rc3/README.md` & `iceberg_tools-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,41 +29,42 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   generate  Generate from FHIR resources.
   compile   Create aggregated json file from individual yaml schemas
-  publish   Copy dictionary to s3 (note:aws cli dependency)
 
 $ iceberg data
 
 Usage: iceberg data [OPTIONS] COMMAND [ARGS]...
 
   Project data (ResearchStudy, ResearchSubjects, Patient, etc.).
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  simplify       Renders Gen3 friendly flattened records.
-  validate       Check FHIR data for validity and ACED conventions.
-  validate-gen3  Check Gen3 data for validity and ACED conventions.
-  pfb            Write simplified FHIR files to a PFB.
-  migrate        Migrate from FHIR R4B to R5.0.
+  simplify             Renders PFB friendly flattened records.
+  validate             Check FHIR data for validity and conventions.
+  validate-simplified  Check simplified data for validity and conventions.
+  pfb                  Write simplified FHIR files to a PFB.
+  migrate              Migrate from FHIR R4B to R5.0.
+  report               Aggregate avro pfb files into a cytoscape tsv.
 
 ```
 
 > Note: `pfb_fhir` and `iceberg` are synonymous in this context.
 
 ## Examples
 
 The commands:
 ```commandline
-pfb_fhir data simplify  tests/fixtures/simplify/study/ tmp/simplified
+pfb_fhir schema generate simplified
+pfb_fhir data simplify --schema_path  iceberg/schemas/simplified/simplified-fhir.json tests/fixtures/simplify/study/ tmp/simplified
 pfb_fhir data pfb tmp/simplified/ tmp/study.pfb
 tree tmp
 
 ```
 
 Will generate the following output:
 ```commandline
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/cli/data.py` & `iceberg_tools-0.0.3/iceberg_tools/cli/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import logging
 import pathlib
 import threading
-import uuid
 
 import click
 import yaml
 from fhir.resources import FHIRAbstractModel  # noqa
 from yaml import SafeLoader
 
 from iceberg_tools.data.report import aggregate_edges
 from iceberg_tools.data.migrator import migrate_directory
 from iceberg_tools.data.pfb import SimplePFBWriter
 from iceberg_tools.data.simplifier import cli as simplifier
-from iceberg_tools.schema.gen3_validator import directory_reader as gen3_directory_reader
+from iceberg_tools.schema.simplified_validator import directory_reader as simplified_directory_reader
 from iceberg_tools.util import NaturalOrderGroup, directory_reader
 
 LINKS = threading.local()
 CLASSES = threading.local()
 IDENTIFIER_LIST_SIZE = 8
 
-ACED_NAMESPACE = uuid.uuid3(uuid.NAMESPACE_DNS, 'aced-ipd.org')
 logger = logging.getLogger(__name__)
 
 
 @click.group(name="data", cls=NaturalOrderGroup)
 def cli():
     """Project data (ResearchStudy, ResearchSubjects, Patient, etc.)."""
     pass
@@ -33,15 +31,15 @@
 
 
 @cli.command('validate')
 @click.argument('path')
 @click.option('--pattern', required=True, default="*.*", show_default=True,
               help='File name pattern')
 def _validate(path, pattern):
-    """Check FHIR data for validity and ACED conventions.
+    """Check FHIR data for validity and conventions.
 
     PATH: Path to FHIR files.
     """
     ok = True
     for result in directory_reader(pathlib.Path(path), pattern):
         if result.exception:
             ok = False
@@ -50,29 +48,29 @@
             print('\tresource_id:', result.resource_id)
             msg = str(result.exception).replace('\n', '\n\t\t')
             print('\texception:', msg)
     if ok:
         print('OK, all resources pass')
 
 
-@cli.command('validate-gen3')
+@cli.command('validate-simplified')
 @click.argument('path')
 @click.option('--schema_path', required=True,
-              default='iceberg/schemas/gen3/aced.json',
+              default='iceberg/schemas/simplified/simplified-fhir.json',
               show_default=True,
-              help='Path to gen3 schema json, a file path or url'
+              help='Path to simplified schema json, a file path or url'
               )
-def _validate_gen3(path, schema_path):
+def _validate_simplified(path, schema_path):
 
-    """Check Gen3 data for validity and ACED conventions.
+    """Check simplified data for validity and conventions.
 
-    PATH: Path to Gen3 ndjson files.
+    PATH: Path to simplified ndjson files.
     """
     ok = True
-    for result in gen3_directory_reader(pathlib.Path(path), schema_path):
+    for result in simplified_directory_reader(pathlib.Path(path), schema_path):
         if result.exception:
             ok = False
             print('file:', result.path)
             print('\toffset:', result.offset)
             print('\tresource_id:', result.resource_id)
             msg = str(result.exception).replace('\n', '\n\t\t')
             print('\texception:', msg)
@@ -80,17 +78,17 @@
         print('OK, all resources pass')
 
 
 @cli.command('pfb')
 @click.argument('path')
 @click.argument('output_path')
 @click.option('--schema_path', required=True,
-              default='iceberg/schemas/gen3/aced.json',
+              default='iceberg/schemas/simplified/simplified-fhir.json',
               show_default=True,
-              help='Path to gen3 schema json, a file path or url'
+              help='Path to simplified schema json, a file path or url'
               )
 @click.option('--config_path',
               default='config.yaml',
               show_default=True,
               help='Path to config file.')
 def pfb(path, output_path, schema_path, config_path):
 
@@ -99,17 +97,16 @@
     \b
     PATH: Directory path to simplified FHIR ndjson files.
     OUTPUT_PATH: File path where to write the PFB.
     """
     path = pathlib.Path(path)
     output_path = pathlib.Path(output_path)
     config_path = pathlib.Path(config_path)
-    assert output_path.is_dir(), f"Path {output_path} is not a directory"
     assert config_path.is_file(), f"Path {config_path} is not a file"
-    assert path.is_file(), f"Path {path} is not a file"
+    assert path.is_dir(), f"Path {path} is not a directory"
 
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
     dependency_order = gen3_config['dependency_order']
 
     pfb_writer = SimplePFBWriter(schema_path=schema_path,
                                  output_path=output_path,
@@ -160,15 +157,15 @@
 
 
 @cli.command()
 @click.argument('path')
 @click.argument('output_path')
 @click.option('--pattern', default='**/*.avro', help='Search pattern', show_default=True)
 def report(path: str,  output_path: str,  pattern: str):
-    """Aggregate avro pfb files into a cytoscape friendly tsv.
+    """Aggregate avro pfb files into a cytoscape tsv.
 
     \b
     PATH: Directory path to search for pfb files
     OUTPUT_PATH: Directory path to write the report TSVs
     """
     assert pathlib.Path(path).is_dir(), f"Path {path} is not a directory"
     assert pathlib.Path(output_path).is_dir(), f"Path {output_path} is not a directory"
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/__init__.py` & `iceberg_tools-0.0.3/iceberg_tools/data/migrator/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/data/pfb.py` & `iceberg_tools-0.0.3/iceberg_tools/data/pfb.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/data/report.py` & `iceberg_tools-0.0.3/iceberg_tools/data/report.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/__init__.py` & `iceberg_tools-0.0.3/iceberg_tools/data/simplifier/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import decimal
 import importlib
 import logging
 import pathlib
 import threading
+import uuid
 from typing import Dict, List
 
 import click
 import inflection
 import orjson
 import requests
 import yaml
+
 from fhir.resources import FHIRAbstractModel  # noqa
 from fhir.resources.attachment import Attachment
 from fhir.resources.codeableconcept import CodeableConcept
 from fhir.resources.codeablereference import CodeableReference
 from fhir.resources.coding import Coding
 from fhir.resources.core.utils import is_primitive_type
 from fhir.resources.documentreference import DocumentReferenceContent, DocumentReference
@@ -32,14 +34,58 @@
 
 LOGGED_ALREADY = []
 logger = logging.getLogger(__name__)
 
 # create a local instance
 THREAD_LOCAL = threading.local()
 
+ICEBERG_NAMESPACE = uuid.uuid3(uuid.NAMESPACE_DNS, 'ICEBERG')
+
+class Getter:
+    """A getter for a FHIR resource."""
+
+    def __init__(self, path: str):
+        """Initialize Getter."""
+        self.path_str = 'this.' + path
+
+    def _traverse_path(self, resource: FHIRAbstractModel, path_to_search: str = None):
+        """Traverse the path, return the last element ,traverse 1st element in list."""
+        target = resource
+        path_to_search = path_to_search or str(self.path_str)
+        path_to_search = path_to_search.replace('this.', '')
+        for path in path_to_search.split('.'):
+            _ = f"this.{path}"
+            _ = eval(_, {}, {'this': target})
+            if _ is None:
+                break
+            if isinstance(_, list):
+                target = _[0]
+            else:
+                target = _
+        return _
+
+    def get(self, resource: FHIRAbstractModel):
+        """Get the value from the resource, including extensions."""
+        if 'extension' in self.path_str:
+            prefix, extension_name = self.path_str.split('.extension.')
+            val = self._traverse_path(resource, path_to_search=prefix)
+            if val:
+                extension_list = getattr(val, 'extension', None)
+                for extension in extension_list or []:
+                    if extension_name in extension.url:
+                        return extension.dict()['__value__']
+            return None
+
+        return self._traverse_path(resource)
+
+
+def _get_nested_object(resource: FHIRAbstractModel, path: str):
+    """Pluck a value from a resource, using path."""
+    return Getter(path).get(resource)
+
 
 def _simple_coding_dict(self: Coding, *args, **kwargs):
     """MonkeyPatch replacement for dict(), render Coding."""
     display = self.display
     if not display:
         display = self.code
     return [
@@ -186,90 +232,91 @@
     return document_reference_content
 
 
 def _simple_document_reference_dict(self: DocumentReference, *args, **kwargs):
     """MonkeyPatch replacement for dict(), render DocumentReference."""
     # defaults
     document_reference = _simple_resource_dict(self)
-    # # sub-resource
-    # _render_sub_resources(document_reference, self)
-
     return document_reference
 
 
 def _simple_task_dict(self: Task, *args, **kwargs):
     """MonkeyPatch replacement for dict(), render Observation."""
     task = _simple_resource_dict(self)
     # go through outputs to collect references
     for _ in self.output:
         _.dict()
     return task
 
 
 def _render_sub_resources(resource: FHIRAbstractModel) -> dict:
     """Render sub-resources with keys "{sub_resource}_{if list index}_{property_name}: simple_value" """
-    config = {
-        'DocumentReference': {
-            'lists': {
-                'content': {'limit': 1, 'properties': ['contentType', 'md5', 'size', 'url']}
-            },
-            'scalars': {}
-        },
-        'Patient': {
-            'lists': {
-                'address': {'limit': 1, 'properties': ['postalCode']}
-            },
-            'scalars': {}
-        }
-    }
+
+    # read config
+    nested_objects = THREAD_LOCAL.nested_objects
     # render lists to scalar
     simplified = {}
-    if resource.resource_type not in config:
+
+    if resource.resource_type not in nested_objects:
         return simplified
 
-    lists = config[resource.resource_type].get('lists', {})
-    scalars = config[resource.resource_type].get('scalars', {})
+    paths = nested_objects[resource.resource_type]
+    for path in paths:
+        nested_object_value = _get_nested_object(resource=resource, path=path)
+        nested_object_name = '_'.join(path.split('.'))
+
+        # # fyi:resource.schema() caches results
+        # parent_property_name = path.split('.')[0]
+        # parent_property_schema = resource.schema()['properties'][parent_property_name]
+
+        is_array = nested_object_value is not None and isinstance(nested_object_value, list)
+
+        if is_array and nested_object_value is not None:
+
+            count = 0
+            for item in nested_object_value:
+                _ = item.dict()
+
+                # only add index in name if > 0
+                separator = '_'
+
+                value = _['__value__']
+                name = _.get('__name__', None)
+                if name:
+                    name = separator + name
+                else:
+                    name = ''
+
+                if f"{nested_object_name}{name}" not in simplified:
+                    simplified[f"{nested_object_name}{name}"] = []
+                simplified[f"{nested_object_name}{name}"].append(value)
 
-    # add values to simplified resource
+                count += 1
 
-    # lists
-    for resource_property_name in lists:  # sub_resource's property name
-        assert hasattr(resource, resource_property_name), f"{resource.resource_type} has no property named {resource_property_name}"
-        resource_property = getattr(resource, resource_property_name)
-        if not resource_property:
-            continue
-        limit = lists[resource_property_name].get('limit', 1)
-        properties = lists[resource_property_name].get('properties', [])
-        count = 0
-        for item in resource_property:
-            _ = item.dict()
-            # only add index in name if > 0
-            separator = '_'
-            if count > 0:
-                separator = f"_{count}_"
-            for k, v in _.items():
-                if k in properties:
-                    simplified[f"{resource_property_name}{separator}{k}"] = v
-            count += 1
-            if count == limit:
-                break
-            # warn if data had more than limit
-            if len(resource.content) > limit:
-                logger.warning(f"{resource.resource_type}/{resource.id} {resource_property_name}"
-                               f" had {len(resource.content)} items limit was {limit}")
-
-    # scalars
-    for resource_property_name in scalars:  # sub_resource's property name
-        assert hasattr(resource, resource_property_name), f"{resource.resource_type} has no property named {resource_property_name}"
-        resource_property = getattr(resource, resource_property_name)
-        if not resource_property:
-            continue
-        _ = resource_property.dict()
-        for k, v in _.items():
-            simplified[f"{resource_property_name}_{k}"] = v
+        else:
+            # scalar
+            if nested_object_value is not None:
+                if hasattr(nested_object_value, 'dict'):
+                    name_value_list = nested_object_value.dict()
+                    if not isinstance(name_value_list, list):
+                        name_value_list = [name_value_list]
+                    for item in name_value_list:
+                        value = item['__value__']
+                        name = item.get('__name__', None)
+                        if name:
+                            name = '_' + name
+                        else:
+                            name = ''
+                        if isinstance(value, list):
+                            value = value[0]
+                        simplified[f"{nested_object_name}{name}"] = value
+                else:
+                    if isinstance(nested_object_value, list):
+                        nested_object_value = nested_object_value[0]
+                    simplified[f"{nested_object_name}"] = nested_object_value
 
     return simplified
 
 
 def _simple_resource_dict(self: FHIRAbstractModel, *args, **kwargs):
     """MonkeyPatch replacement for dict(), render generic Resource."""
     # override this with a specialization
@@ -312,47 +359,65 @@
 def _render_extensions(self: FHIRAbstractModel, *args, **kwargs) -> Dict:
     """Utility, create a dict of the extensions in a resource."""
     extensions = {}
     if hasattr(self, 'extension') and self.extension:
         for extension in self.extension:
             ext_dict = extension.dict()
             if ext_dict:
-                ext_val_as_list = ext_dict['__value__']
-                if not isinstance(ext_dict['__value__'], list):
-                    ext_val_as_list = [ext_dict['__value__']]
-                ext_name = ext_dict['__name__']
-                for item in ext_val_as_list:
-                    # more than one name
-                    compound_name = ext_name
-
-                    if not isinstance(item, dict):
-                        extensions[compound_name] = item
-                        continue
-
-                    if '__name__' in item:
-                        compound_name = f"{compound_name}_{item['__name__']}"
-                    compound_name = compound_name.replace('-', '_')
-
-                    if compound_name not in extensions:
-                        extensions[compound_name] = []
+                _populate_extensions(ext_dict, extensions)
+            else:
+                parent_name = extension.url.split('/')[-1].replace('-', '_')
+                for child_extension in extension.extension:
+                    ext_dict = child_extension.dict()
+                    if ext_dict:
+                        _populate_extensions(ext_dict, extensions, parent_name)
 
-                    if '__value__' in item:
-                        extensions[compound_name].extend(item['__value__'])
-                    else:
-                        for k, v in item.items():
-                            extensions[f"{compound_name}_{k}"] = v
-
-                    # if only one value, make it scalar
-                    if len(extensions[compound_name]) == 1:
-                        extensions[compound_name] = extensions[compound_name][0]
     # cleanup no data
     extensions = {k: v for k, v in extensions.items() if (v is not None and v != [])}
     return extensions
 
 
+def _populate_extensions(ext_dict, extensions, parent_name=None):
+    """Utility, populate extensions dict with values from a single extension."""
+    ext_val_as_list = ext_dict['__value__']
+    if not isinstance(ext_dict['__value__'], list):
+        ext_val_as_list = [ext_dict['__value__']]
+    ext_name = ext_dict['__name__']
+    if parent_name:
+        ext_name = f"{parent_name}_{ext_name}"
+
+    compound_name = None
+    for item in ext_val_as_list:
+        # more than one name
+        compound_name = ext_name
+
+        if not isinstance(item, dict):
+            extensions[compound_name] = item
+            continue
+
+        if '__name__' in item and item['__name__'] != ext_name:
+            compound_name = f"{compound_name}_{item['__name__']}"
+        compound_name = compound_name.replace('-', '_')
+
+        compound_name = compound_name.replace('_text', '')
+
+        if compound_name not in extensions:
+            extensions[compound_name] = []
+
+        if '__value__' in item:
+            extensions[compound_name].append(item['__value__'])
+        else:
+            for k, v in item.items():
+                extensions[f"{compound_name}_{k}"] = v
+
+    # if only one value, make it scalar
+    if isinstance(extensions[compound_name], list) and len(extensions[compound_name]) == 1:
+        extensions[compound_name] = extensions[compound_name][0]
+
+
 def _render_codings(self: FHIRAbstractModel, *args, **kwargs) -> Dict:
     """Utility, create a dict of the codings in a resource."""
     codings = {}
     alias_maps = self.get_alias_mapping()
     for prop_name in self.elements_sequence():
         field_key = alias_maps[prop_name]
         v = self.__dict__.get(field_key, None)
@@ -427,20 +492,20 @@
 
 def _gen3_scaffolding_document_reference(simplified: dict, resource: FHIRAbstractModel) -> dict:
     """Add Gen3 boiler plate"""
 
     if simplified['resourceType'] != 'DocumentReference':
         return simplified
 
-    if 'content_url' not in simplified:
-        logger.warning(f"Missing content_url in simplified {simplified['resourceType']} {simplified['id']}")
+    if 'content_attachment_url' not in simplified:
+        logger.debug(f"Missing content_attachment_url in simplified {simplified['resourceType']} {simplified['id']}")
         suffix = None
         file_name = None
     else:
-        content_url = pathlib.Path(simplified['content_url'])
+        content_url = pathlib.Path(simplified['content_attachment_url'])
         suffix = content_url.suffix
         file_name = content_url.name
 
     if suffix:
         suffix = suffix.replace('.', '')
     simplified['data_type'] = suffix
     if suffix in ['csv']:
@@ -453,43 +518,43 @@
         simplified['data_format'] = 'log'
     if suffix in ['m']:
         simplified['data_format'] = 'matlab'
     if suffix in ['sh']:
         simplified['data_format'] = 'script'
 
     simplified['file_name'] = file_name
-    if 'content_md5' in simplified:
-        simplified['md5sum'] = simplified['content_md5']
+    if 'content_attachment_extension_md5' in simplified:
+        simplified['md5sum'] = simplified['content_attachment_extension_md5']
     if 'content_size' in simplified:
-        simplified['file_size'] = simplified['content_size']
+        simplified['file_size'] = simplified['content_attachment_size']
     simplified['object_id'] = simplified['id']
 
     return simplified
 
 
 def _gen3_references(simplified: dict, resource: FHIRAbstractModel) -> dict:
 
     pass
 
 
 def _ensure_dialect(simplified: dict, resource: FHIRAbstractModel, dialect: str) -> dict:
     """Enforce dialect rules, update simplified dict.
-    In practice, it toggles between GEN3 and plain FHIR.
-    Gen3 dialect injects Gen3 properties and harvests edges.
+    In practice, it toggles between PFB and plain FHIR.
+    PFB dialect injects Gen3 properties and harvests edges.
     """
-    if dialect != 'GEN3':
+    if dialect != 'PFB':
         return simplified
     simplified = _gen3_scaffolding_document_reference(simplified, resource)
     return simplified
 
 
-def _render_dialect(simplified: dict, references: List[str], dialect: str, schemas: dict, limit_links: dict) -> dict:
-    """Render as Gen3 record ready for import
+def _render_dialect(simplified: dict, references: List[str], dialect: str, schemas: dict, limit_links: dict = {}) -> dict:
+    """Render as PFB record ready for import
     """
-    if dialect != 'GEN3':
+    if dialect != 'PFB':
         return simplified
 
     labels = [_['title'] for _ in schemas.values() if 'title' in _]
 
     permitted_destinations = None
     if simplified['resourceType'] in limit_links:
         permitted_destinations = limit_links[simplified['resourceType']]
@@ -505,36 +570,54 @@
         if permitted_destinations is not None and label not in permitted_destinations:
             continue
         gen3_links.append({"dst_id": id_, "dst_name": inflection.underscore(label)})
 
     return {'id': simplified['id'], 'name': inflection.underscore(simplified['resourceType']), 'relations': gen3_links, 'object': simplified}
 
 
-def simplify(resource: FHIRAbstractModel, dialect: str) -> (Dict, List[str]):
-    """Create a Gen3 friendly resource. Returns simplified resource and associated references."""
-    # most of the heavy lifting done in dict() overrides
+def new_id(transform_ids, id_):
+    """Create a new UUID based on the original id and the seed."""
+    _study_uuid = uuid.uuid5(ICEBERG_NAMESPACE, transform_ids)
+    return str(uuid.uuid5(_study_uuid, id_))
+
+
+def simplify(resource: FHIRAbstractModel, dialect: str, nested_objects: dict = {}, transform_ids=None) -> (Dict, List[str]):
+    """Create a PFB friendly resource. Returns simplified resource and associated references.
+    Most of the heavy lifting done in dict() overrides of FHIRAbstractModel.dict()
+    """
+    # filled in by _simple_reference_dict
     THREAD_LOCAL.references = []
+    # read by _render_sub_resources
+    THREAD_LOCAL.nested_objects = nested_objects
     simplified = resource.dict()
     # cleanup goes here...
     simplified = _ensure_dialect(simplified, resource, dialect)
+    if transform_ids:
+        simplified['id'] = new_id(transform_ids, simplified['id'])
+        transformed_references = []
+        for reference in THREAD_LOCAL.references:
+            type_, id_ = reference.split('/')
+            id_ = new_id(transform_ids, id_)
+            transformed_references.append(f"{type_}/{id_}")
+        THREAD_LOCAL.references = transformed_references
     return simplified, THREAD_LOCAL.references
 
 
 def check_simplified_schemas(simplified: dict, schemas: dict):
     """Compare simplified fields vs schema."""
     resource_type = inflection.underscore(simplified['resourceType'])
     assert resource_type in schemas, f"{resource_type} not in schemas"
     extra_fields = [k for k in simplified if k not in schemas[resource_type]['properties']]
     assert len(extra_fields) == 0, ('extra_fields_not_in_schema', resource_type, extra_fields)
 
 
 def _default_json_serializer(obj):
     """JSON Serializer, render decimal and bytes types."""
     if isinstance(obj, decimal.Decimal):
-        return str(obj)
+        return float(obj)
     if isinstance(obj, bytes):
         return obj.decode()
 
     raise TypeError
 
 
 class SimplifierContextManager:
@@ -542,52 +625,58 @@
     def __enter__(self):
         # print("Monkey patching FHIR", file=sys.stderr)
         self.orig_resource_dict = FHIRAbstractModel.dict
         self.orig_coding_dict = Coding.dict
         self.orig_identifier_dict = Identifier.dict
         self.orig_reference_dict = Reference.dict
         self.orig_extension_dict = Extension.dict
+
         self.orig_attachment_dict = Attachment.dict
         self.orig_document_reference_content_dict = DocumentReferenceContent.dict
-        # self.orig_document_reference_dict = DocumentReference.dict
+
         self.orig_observation_dict = Observation.dict
         self.orig_codeable_concept_dict = CodeableConcept.dict
         self.orig_codeable_reference_dict = CodeableReference.dict
+
         self.orig_task_dict = Task.dict
 
         FHIRAbstractModel.dict = _simple_resource_dict
         Coding.dict = _simple_coding_dict
         Identifier.dict = _simple_identifier_dict
         Reference.dict = _simple_reference_dict
         Extension.dict = _simple_extension_dict
-        Attachment.dict = _simple_attachment_dict
-        DocumentReferenceContent.dict = _simple_document_reference_content_dict
-        # DocumentReference.dict = _simple_document_reference_dict
+
+        # Attachment.dict = _simple_attachment_dict
+        # DocumentReferenceContent.dict = _simple_document_reference_content_dict
+
         Observation.dict = _simple_observation_dict
         CodeableConcept.dict = _simple_codeable_concept_dict
         CodeableReference.dict = _simple_codeable_reference_dict
-        Task.dict = _simple_task_dict
+
+        Task.dict = _simple_task_dict    # TODO - do we still need this?
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         # print("Restoring original FHIR classes", file=sys.stderr)
         FHIRAbstractModel.dict = self.orig_resource_dict
         Coding.dict = self.orig_coding_dict
         Identifier.dict = self.orig_identifier_dict
         Reference.dict = self.orig_reference_dict
         Extension.dict = self.orig_extension_dict
+
         Attachment.dict = self.orig_attachment_dict
         DocumentReferenceContent.dict = self.orig_document_reference_content_dict
-        # DocumentReference.dict = self.orig_document_reference_dict
+
         Observation.dict = self.orig_observation_dict
         CodeableConcept.dict = self.orig_codeable_concept_dict
         CodeableReference.dict = self.orig_codeable_reference_dict
+
         Task.dict = self.orig_task_dict
 
 
-def simplify_directory(input_path, pattern, output_path, schema_path, dialect, config_path):
+def simplify_directory(input_path, pattern, output_path, schema_path, dialect, config_path, transform_ids=None):
     """Reads directory of FHIR, renders simple, data frame friendly flattened records."""
 
     input_path = pathlib.Path(input_path)
     assert input_path.is_dir(), f"{input_path} not a directory"
     dialect = dialect.upper()
 
     if pathlib.Path(schema_path).is_file():
@@ -596,26 +685,27 @@
     else:
         schemas = requests.get(schema_path).json()
     assert schemas, f"No schema found at {schema_path}"
 
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
     limit_links = gen3_config['limit_links']
+    nested_objects = gen3_config['nested_objects']
 
     with SimplifierContextManager():
         with EmitterContextManager(output_path) as emitter:
             for parse_result in directory_reader(directory_path=input_path, pattern=pattern,
                                                  validate=False):
                 if parse_result.exception is not None:
                     if 'resourceType' not in str(parse_result.exception):
                         logger.error(f"{parse_result.path} has exception {parse_result.exception}")
                     continue
                 resource = parse_result.resource
 
-                simplified, references = simplify(resource, dialect)
+                simplified, references = simplify(resource, dialect, nested_objects, transform_ids)
                 try:
                     check_simplified_schemas(simplified, schemas)
                 except (TypeError, AssertionError) as e:
                     _debug_once(str(e))
 
                 assert simplified, ("Should have simplified", resource.resource_type, resource.id)
                 all_ok = all([validate_simplified_value(_) for _ in simplified.values()])
@@ -645,32 +735,36 @@
 
 @click.command('simplify')
 @click.argument('path')
 @click.argument('output_path')
 @click.option('--pattern', required=True, default="**/*.*", show_default=True,
               help='File name pattern')
 @click.option('--schema_path', required=True,
-              default='https://aced-public.s3.us-west-2.amazonaws.com/aced.json',
               show_default=True,
-              help='Path to gen3 schema json.  (Accepts file path for schema development)'
+              help='Path to simplified schema json.  (Accepts url or file path)'
               )
 @click.option('--dialect',
-              default='GEN3',
-              type=click.Choice(['FHIR', 'GEN3'], case_sensitive=False),
-              help='GEN3: adds common properties, FHIR: passthrough'
+              default='PFB',
+              type=click.Choice(['FHIR', 'PFB'], case_sensitive=False),
+              help='PFB: adds common properties, FHIR: passthrough'
               )
 @click.option('--config_path',
               default='config.yaml',
               show_default=True,
               help='Path to config file.')
-def cli(path, pattern, output_path, schema_path, dialect, config_path):
-    """Renders Gen3 friendly flattened records.
+@click.option('--transform_ids',
+              default=None,
+              show_default=True,
+              help='Transform ids based on this seed')
+
+def cli(path, pattern, output_path, schema_path, dialect, config_path, transform_ids):
+    """Renders PFB friendly flattened records.
 
     PATH: Path containing bundles (*.json) or resources (*.ndjson)
     OUTPUT_PATH: Path where simplified resources will be stored
     """
-    simplify_directory(path, pattern, output_path, schema_path, dialect, config_path)
+    simplify_directory(path, pattern, output_path, schema_path, dialect, config_path, transform_ids)
 
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO)
     cli()
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/oid_lookup.py` & `iceberg_tools-0.0.3/iceberg_tools/data/simplifier/oid_lookup.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/schema/__init__.py` & `iceberg_tools-0.0.3/iceberg_tools/schema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 from typing import List
 
 import inflection
 import orjson
 from fhir.resources.core.utils.common import get_fhir_type_name
 from fhir.resources.fhirprimitiveextension import FHIRPrimitiveExtension
 
+from iceberg_tools.schema.fhir_resources.binding_lookup import create_fhir_definitions_lookup
+
+
+logger = logging.getLogger(__name__)
+
 path = pathlib.Path("~/.iceberg").expanduser()
 path.mkdir(parents=True, exist_ok=True)
 path = path / "element_bindings.sqlite"
 if not path.is_file():
-    print("Please see resources/fhir/README.md first.")
+    create_fhir_definitions_lookup()
+if not path.is_file():
+    logger.error(f"Unable to find fhir bindings at {path}")
     exit(2)
 
 ELEMENT_DB = sqlite3.connect(path)
-BASE_URI = 'http://bmeg.io/schema/0.0.2'
-
-logger = logging.getLogger(__name__)
+BASE_URI = 'http://graph-fhir.io/schema/0.0.2'
 
 
 def _find_fhir_classes(gen3_config, log_stats=True) -> List[type]:
     """Based on config, expand dependencies."""
 
     class_names = [c for c in gen3_config['dependency_order'] if not c.startswith('_')]
     class_names = [c for c in class_names if c not in ['Program', 'Project']]
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/schema/bmeg.py` & `iceberg_tools-0.0.3/iceberg_tools/schema/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 
             assert 'title' in schema, schema
             schema['$id'] = f"{base_uri}/{schema['title']}"
 
             schemas['$defs'][schema['title']] = schema
             schemas['anyOf'].append({'$ref': f"{base_uri}/{schema['title']}"})
 
-    path = output_path / pathlib.Path("aced-bmeg.json")
+    path = output_path / pathlib.Path("graph-fhir.json")
     with open(path, "w") as fp:
         json.dump(schemas, fp, indent=2)
 
     return path
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3.py` & `iceberg_tools-0.0.3/iceberg_tools/schema/simplified.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 FHIR_PRIMITIVES_TO_JSON_SCHEMA = {
     "boolean": 'boolean',
     "string": 'string',
     "base64Binary": 'string',
     "code": 'string',
     "id": 'string',
-    "decimal": 'string',
+    "decimal": 'number',
     "integer": 'number',
     "unsignedInt": 'number',
     "positiveInt": 'number',
     "uri": 'string',
     "oid": 'string',
     "uuid": 'string',
     "canonical": 'string',
@@ -51,51 +51,53 @@
             continue
         summary[schema['title']] = {'total_property_counts': len(schema['properties'])}
     stats_table = '\n  '.join(sorted([f'{k}: {v}' for k, v in summary.items()]))
     return '  ' + stats_table
 
 
 def _simplify_schemas(gen3_config, gen3_fixtures, schemas, log_stats=True):
-    """Make the schema Gen3 (data-frame) friendly."""
+    """Make the schema PFB (data-frame) friendly."""
 
     # extract expected configurations
     config_categories = gen3_config['categories']
     ignored_properties = gen3_config['ignored_properties']
     dependency_order = gen3_config['dependency_order']
     extra_properties = gen3_config['extra_properties']
     renamed_properties = gen3_config['renamed_properties']
     limit_links = gen3_config['limit_links']
     extensions = gen3_config['extensions']
-
-    # delete vertices we don't want
-    vertices_to_delete = set(schemas.keys()) - set(dependency_order)
-    for k in vertices_to_delete:
-        del schemas[k]
+    nested_objects = gen3_config['nested_objects']
 
     _remove_required_flag(schemas)
 
     _ensure_description(schemas)
     _add_extra_properties(schemas, extra_properties)
     _rename_properties(schemas, renamed_properties)
+    _add_plucked_properties(schemas, nested_objects)
 
     _add_gen3_schema_scaffolding(config_categories, schemas)
     _add_extensions(extensions, schemas)
 
     # do this before _remove_ignored_properties since we have dummy references in extra_properties
     _simplify_references(schemas, dependency_order, limit_links)
     _remove_ignored_properties(ignored_properties, schemas)
     _simplify_identifiers(schemas)
     _simplify_codeable_concepts(schemas)
     _simplify_quantities(schemas)
 
     _simplify_embedded_types(schemas)
 
+    # delete vertices we don't want
+    vertices_to_delete = set(schemas.keys()) - set(dependency_order)
+    for k in vertices_to_delete:
+        del schemas[k]
+
     _add_gen3_static_dependencies(gen3_fixtures, schemas)
 
-    # save gen3 schema in order
+    # save simplified schema in order
     dependency_order.extend(k for k in schemas if k not in dependency_order)
 
     # change to lowercase for gen3
     gen3_schema = {inflection.underscore(k).replace('.yaml', ''): schemas[k] for k in dependency_order if k in schemas}
 
     if log_stats:
         logger.info(f"Class statistics number of simplified objects:\n{_summarize_stats(gen3_schema)}")
@@ -171,14 +173,16 @@
                         property_['binding_version'] = version
                 property_name = f"{extension_name}_{element_name}"
                 if len(element_name) == 0:
                     property_name = extension_name
 
                 _add_term_def(property_)
                 _add_enum(property_)
+
+                property_name = property_name.replace('_text', '')
                 schema['properties'][property_name] = property_
             logger.info(f"Added extension: {extension_name}")
 
 
 def _add_gen3_schema_scaffolding(config_categories, schemas):
     """add gen3 boilerplate to individual schemas"""
     for k, schema in schemas.items():
@@ -197,18 +201,22 @@
             schema['id'] = inflection.underscore(schema['$id'])
             del schema['$id']
 
 
 def _simplify_identifiers(schemas: dict):
     """Transform identifiers to a list of strings"""
     for schema in schemas.values():
+
         if 'properties' not in schema:
             continue
         if 'identifier' not in schema['properties']:
             continue
+        if 'items' not in schema['properties']['identifier']:
+            continue
+
         schema['properties']['identifier']['items']['type'] = 'string'
         del schema['properties']['identifier']['items']['$ref']
 
         identifier_text_coding = copy.deepcopy(schema['properties']['identifier'])
         identifier_text_coding['description'] = "[system#code representation of identifier.text] " + identifier_text_coding['description']
         schema['properties']['identifier_text_coding'] = identifier_text_coding
 
@@ -328,30 +336,102 @@
 #         codings = _list_of_type(schema, 'Coding')
 #         if len(codings) > 0:
 #             print()
 #         codings = _scalar_of_type(schema, 'Coding')
 #         if len(codings) > 0:
 #             print()
 
-def _simplify_embedded_types(schemas):
-    """Any remaining embedded types are simply rendered as strings."""
-    # TODO - implement "PLUCK"
+def _add_plucked_properties(schemas: dict, nested_objects: dict):
+    """Add plucked properties to schemas
+
+    nested_objects: render child objects properties
+    """
+
     for schema in schemas.values():
+        plucked_properties = _plucked_properties(schema, schemas,  nested_objects)
+
+        if plucked_properties:
+            properties_with_plucked = set()
+            for plucked_property_source, plucked_property in plucked_properties.items():
+                for nested_property_name, nested_property in plucked_property['_nested_objects'].items():
+                    compound_property_name = f"{plucked_property_source}_{nested_property_name}"
+                    nested_property['description'] = f"[Plucked from {schema['title']}.{plucked_property_source}] {nested_property['description']}"
+                    schema['properties'][compound_property_name] = nested_property
+                    properties_with_plucked.add(plucked_property_source)
+            for _ in properties_with_plucked:
+                del schema['properties'][_]
+
+
+def _simplify_embedded_types(schemas: dict):
+    """Any remaining embedded types are simply rendered as strings.
+
+    """
+
+    for schema in schemas.values():
+
         lists_of_any = _list_of_any_type(schema)
         for name, property_ in lists_of_any.items():
             property_['description'] = f"[Text representation of {property_['items']['$ref'].replace('.yaml', '')}] {property_['description']}"
             property_['items']['type'] = 'string'
             del property_['items']['$ref']
         scalars_of_any = _scalar_of_any_type(schema)
         for name, property_ in scalars_of_any.items():
             property_['description'] = f"[Text representation of {property_['$ref'].replace('.yaml', '')}] {property_['description']}"
             property_['type'] = 'string'
             del property_['$ref']
 
 
+def _plucked_properties(schema, schemas, nested_objects) -> dict:
+    """Pluck properties tree from nested objects."""
+    plucked_properties = {}
+
+    if any([name == schema['title'] for name in nested_objects]):
+        for path in nested_objects[schema['title']]:
+            k = path.split('.')[0]
+            assert k in schema['properties']
+            plucked_properties[k] = schema['properties'][k]
+            if '_nested_objects' not in plucked_properties[k]:
+                plucked_properties[k]['_nested_objects'] = {}
+            _ = '.'.join(path.split('.')[1:])
+            plucked_properties[k]['_nested_objects'].update({_.replace('.', '_'): {}})
+
+    for k, v in plucked_properties.items():
+        if 'items' in v:
+            if '$ref' in v['items']:
+                for path in v['_nested_objects']:
+                    sub_schema_key = v['items']['$ref'].replace('.yaml', '')
+                    assert sub_schema_key in schemas, (sub_schema_key, schemas.keys())
+                    sub_schema = schemas[sub_schema_key]
+                    for sub_property_name in path.split('_'):
+                        if sub_schema['title'] == 'Extension':
+                            v['_nested_objects'][path] = {'description': 'Value of extension', 'type': 'string'}
+                            continue
+                        assert sub_property_name in sub_schema['properties'], (sub_property_name, sub_schema['title'])
+                        sub_property = sub_schema['properties'][sub_property_name]
+                        v['_nested_objects'][path] = sub_property
+                        if '$ref' in sub_property:
+                            sub_schema = schemas[sub_property['$ref'].replace('.yaml', '')]
+                        if '$ref' in sub_property.get('items', {}):
+                            sub_schema = schemas[sub_property['items']['$ref'].replace('.yaml', '')]
+        elif '$ref' in v:
+            sub_schema_key = v['$ref'].replace('.yaml', '')
+            assert sub_schema_key in schemas, (sub_schema_key, schemas.keys())
+            sub_schema = schemas[sub_schema_key]
+            for _ in v['_nested_objects']:
+                for sub_property_name in _.split('.'):
+                    sub_property = sub_schema['properties'][sub_property_name]
+                    v['_nested_objects'][sub_property_name] = sub_property
+                    if '$ref' in sub_property:
+                        sub_schema = schemas[sub_property['$ref'].replace('.yaml', '')]
+                    if '$ref' in sub_property.get('items', {}):
+                        sub_schema = schemas[sub_property['items']['$ref'].replace('.yaml', '')]
+
+    return plucked_properties
+
+
 def _ensure_description(schemas):
     """Every property has a description"""
     for schema in schemas.values():
         for name_, property_ in schema['properties'].items():
             if 'description' not in property_:
                 property_['description'] = property_.get('title', '')
 
@@ -400,17 +480,17 @@
                 links_to_add[name_] = property_
 
         links = []
         targets = {}
         delete_from_properties = []
         for name_, property_ in links_to_add.items():
             if 'enum_reference_types' not in property_:
-                logger.warning(
+                logger.info(
                     f"{schema['title']}.{name_} has no defined targets, "
-                    "i.e a Reference->Any.  Not supported by Gen3. Skipping."
+                    "i.e a Reference->Any.  Not supported by PFB. Skipping."
                 )
                 continue
 
             multiple_targets = len(property_['enum_reference_types']) > 1
             for reference_type in property_['enum_reference_types']:
                 # is the reference in scope
                 assert 'backref' in property_, (f"{schema['title']}_{name_}", property_)
@@ -420,29 +500,29 @@
                 if permitted_destinations and reference_type not in permitted_destinations:
                     logger.info(f"Edge destination suppressed: {schema['title']}.{name_} -> {reference_type}")
                     continue
 
                 target_type = inflection.underscore(reference_type)
                 label = f"{schema['title']}_{name_}_{reference_type}_{property_['backref']}"
                 if target_type in targets:
-                    logger.warning(f"{schema['title']} already has link to {target_type} via {targets[target_type]}. "
-                                   f"Therefore ignoring: {label}")
+                    logger.info(f"{schema['title']} already has link to {target_type} via {targets[target_type]}, "
+                                f"ignoring {schema['title']}.{name_}")
                     continue
                 link_name = name_
                 if multiple_targets:
                     link_name = f"{name_}_{reference_type}"
                 links.append({
                     'backref': property_['backref'],
                     'label': label,
                     'multiplicity': 'many_to_many',
                     'name': link_name,
                     'required': False,
                     'target_type': target_type
                 })
-                targets[target_type] = label
+                targets[target_type] = f"{schema['title']}.{name_}"
                 delete_from_properties.append(name_)
 
         # # remove link from property dict
         # for name_ in set(delete_from_properties):
         #     del schema['properties'][name_]
 
         schema['links'] = links
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3_validator.py` & `iceberg_tools-0.0.3/iceberg_tools/schema/simplified_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,83 +20,89 @@
 
 def log_once(msg):
     if msg not in LOGGED_ALREADY:
         logger.info(msg)
         LOGGED_ALREADY.append(msg)
 
 
-def _validate(gen3_resource: dict, schemas: dict):
-    """Ensure resource is valid for gen3 schema."""
+def validate(gen3_resource: dict, schemas: dict):
+    """Ensure resource is valid for simplified schema."""
     try:
-        resource = None
+        object_ = None
         for expected_property in ['id', 'relations', 'object']:
             assert expected_property in gen3_resource, f"{expected_property} not in {gen3_resource}"
 
-        resource = gen3_resource['object']
-        resource_type = resource['resourceType']
+        object_ = gen3_resource['object']
+        resource_type = object_['resourceType']
         key = inflection.underscore(resource_type)
         schema = schemas.get(key, schemas.get(f"{key}.yaml", None))
         assert schema, f"Could not find schema for {key}"
-        actual_keys = set(resource.keys())
+        actual_keys = set(object_.keys())
         expected_keys = set(schema['properties'].keys()).union(set([_['name'] for _ in schema['links']]))
         if not actual_keys.issubset(expected_keys):
             if not schema.get('additionalProperties', False):
                 assert False, f"Is not a subset {actual_keys - expected_keys} not expected"
             else:
                 for _ in actual_keys - expected_keys:
-                    msg = f"extra property: {resource_type}.{_} {type(resource[_]).__name__}"
+                    msg = f"extra property: {resource_type}.{_} {type(object_[_]).__name__}"
                     log_once(msg)
         if 'required' in schema:
             for _ in schema['required']:
-                assert _ in resource, f"{_} missing {resource}"
+                assert _ in object_, f"{_} missing {object_}"
         compiled_schema = COMPILED_SCHEMAS.get(key, None)
         if not compiled_schema:
             compiled_schema = fastjsonschema.compile(
                 schema,
                 formats={
                     'time': r'^(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?$',
                     'date': r'^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])?$',
                     'binary': r'^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$',
                     "date-time": r'^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?$',
                     "uri": r'\w+:(\/?\/?)[^\s]+',
                     "uuid": r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-5][0-9a-f]{3}-[089ab][0-9a-f]{3}-[0-9a-f]{12}$"
                 }
             )
             COMPILED_SCHEMAS[key] = compiled_schema
-        compiled_schema(resource)
-        return ParseResult(resource=resource, exception=None, path=None, resource_id=resource.get('id', None))
+        compiled_schema(object_)
+        return ParseResult(object=object_, resource=None, exception=None, path=None, resource_id=object_.get('id', None))
     except (ValidationError, AssertionError) as e:
-        if resource:
-            return ParseResult(resource=None, exception=e, path=None, resource_id=resource.get('id', None))
+        if object_:
+            return ParseResult(object=object_, resource=None, exception=e, path=None, resource_id=object_.get('id', None))
         else:
-            return ParseResult(resource=None, exception=e, path=None)
+            return ParseResult(object=object_, resource=None, exception=e, path=None)
 
 
 def directory_reader(
         directory_path: pathlib.Path,
         schema_path: str,
         pattern: str = '*.ndjson',
-        validate=True) -> Iterator[ParseResult]:
+        validate_=True) -> Iterator[ParseResult]:
     """Extract FHIR resources from directory"""
 
     assert directory_path.is_dir(), f"{directory_path.name} is not a directory"
 
-    if 'http' in schema_path:
-        schemas = requests.get(schema_path).json()
-    else:
-        schemas = DataDictionary(local_file=schema_path).schema
+    schemas = ensure_schema(schema_path)
 
     input_files = [_ for _ in directory_path.glob(pattern)]
     for input_file in input_files:
         logger.info(input_file)
         if not input_file.is_file():
             continue
         fp = _to_file(input_file)
         with fp:
             offset = 0
             for line in fp.readlines():
                 gen3_resource = orjson.loads(line)
-                parse_result = _validate(gen3_resource, schemas=schemas)
+                parse_result = validate(gen3_resource, schemas=schemas)
                 parse_result.path = input_file
                 parse_result.offset = offset
                 offset += 1
                 yield parse_result
+
+
+def ensure_schema(schema_path):
+    """Ensure schema is loaded, from either local file or URL."""
+    if 'http' in schema_path:
+        schemas = requests.get(schema_path).json()
+    else:
+        schemas = DataDictionary(local_file=schema_path).schema
+    return schemas
```

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools/util.py` & `iceberg_tools-0.0.3/iceberg_tools/util.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/PKG-INFO` & `iceberg_tools-0.0.3/iceberg_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-tools
-Version: 0.0.2rc3
+Version: 0.0.3
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
@@ -48,41 +48,42 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   generate  Generate from FHIR resources.
   compile   Create aggregated json file from individual yaml schemas
-  publish   Copy dictionary to s3 (note:aws cli dependency)
 
 $ iceberg data
 
 Usage: iceberg data [OPTIONS] COMMAND [ARGS]...
 
   Project data (ResearchStudy, ResearchSubjects, Patient, etc.).
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  simplify       Renders Gen3 friendly flattened records.
-  validate       Check FHIR data for validity and ACED conventions.
-  validate-gen3  Check Gen3 data for validity and ACED conventions.
-  pfb            Write simplified FHIR files to a PFB.
-  migrate        Migrate from FHIR R4B to R5.0.
+  simplify             Renders PFB friendly flattened records.
+  validate             Check FHIR data for validity and conventions.
+  validate-simplified  Check simplified data for validity and conventions.
+  pfb                  Write simplified FHIR files to a PFB.
+  migrate              Migrate from FHIR R4B to R5.0.
+  report               Aggregate avro pfb files into a cytoscape tsv.
 
 ```
 
 > Note: `pfb_fhir` and `iceberg` are synonymous in this context.
 
 ## Examples
 
 The commands:
 ```commandline
-pfb_fhir data simplify  tests/fixtures/simplify/study/ tmp/simplified
+pfb_fhir schema generate simplified
+pfb_fhir data simplify --schema_path  iceberg/schemas/simplified/simplified-fhir.json tests/fixtures/simplify/study/ tmp/simplified
 pfb_fhir data pfb tmp/simplified/ tmp/study.pfb
 tree tmp
 
 ```
 
 Will generate the following output:
 ```commandline
```

### Comparing `iceberg_tools-0.0.2rc3/setup.py` & `iceberg_tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='iceberg_tools',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2rc3',  # Required
+    version='0.0.3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='FHIR schemas tools for bioinformatics.',
     # Optional
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/__init__.py` & `iceberg_tools-0.0.3/tests/integration/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/conftest.py` & `iceberg_tools-0.0.3/tests/integration/graph/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
 import os
 import pathlib
 
 import pytest
 from jsonschema.validators import Draft202012Validator
 
-from tests.integration.bmeg import is_edge
+from tests.integration.graph import is_edge
 
 
 @pytest.fixture()
 def bmeg_dir():
-    """cd to bmeg dir"""
+    """cd to graph dir"""
     # setup
     cwd = os.getcwd()
-    os.chdir('iceberg/schemas/bmeg')
+    os.chdir('iceberg/schemas/graph')
     # run test
-    yield 'iceberg/schemas/bmeg'
+    yield 'iceberg/schemas/graph'
     # teardown
     os.chdir(cwd)
 
 
 @pytest.fixture()
 def fhir_schema(bmeg_dir):
-    fhir_schema = json.load(open("aced-bmeg.json"))
+    fhir_schema = json.load(open("graph-fhir.json"))
     Draft202012Validator.check_schema(fhir_schema)
     yield fhir_schema
 
 
 @pytest.fixture()
 def fhir_validator(fhir_schema):
     yield Draft202012Validator(fhir_schema)
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_load_granular_reference.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_edge_load_granular_reference.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_validator.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_edge_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 
 from jsonschema.exceptions import ValidationError
 
-from tests.integration.bmeg import edge_validator
+from tests.integration.graph import edge_validator
 
 
 def test_edge_validator(fhir_schema, fhir_validator, edge_schemas):
 
     for edge in edge_schemas:
         try:
             edge_validator(fhir_validator, {
@@ -41,15 +41,15 @@
     for edge in edge_schemas:
         if edge['destination_type'] == 'Resource' and len([e for e in edge_schemas if e['source_type'] == edge['source_type']]) == 1:
             print('  ', edge['source_type']+'.'+edge['source_property_name'], edge['destination_type'])
             needs_unresolved_primary = True
     if not needs_unresolved_primary:
         print('  None')
 
-    print('multi-edges (ie need `is_primary` manually set for uni-graphs (gen3)):')
+    print('multi-edges (ie need `is_primary` manually set for uni-graphs (simplified)):')
 
     edge_counts = defaultdict(dict)
     for edge in edge_schemas:
         if edge['destination_type'] not in edge_counts[edge['source_type']]:
             edge_counts[edge['source_type']][edge['destination_type']] = False
         if not edge_counts[edge['source_type']][edge['destination_type']]:
             edge_counts[edge['source_type']][edge['destination_type']] = edge['is_primary']
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_invalid_edges.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_invalid_edges.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_negative_trivial_vertex_load.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_negative_trivial_vertex_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import ValidationError
 
-from tests.integration.bmeg import is_edge
+from tests.integration.graph import is_edge
 
 
 def test_negative_trivial_schema_load(fhir_schema, fhir_validator):
     """a negative test - all should fail"""
 
     for vertex_name in fhir_schema['$defs']:
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_spot_check_embedded_type.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_spot_check_embedded_type.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_edge_load.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_trivial_edge_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_vertex_load.py` & `iceberg_tools-0.0.3/tests/integration/graph/test_trivial_vertex_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from jsonschema.exceptions import ValidationError, UnknownType
 
-from tests.integration.bmeg import is_edge
+from tests.integration.graph import is_edge
 
 
 def test_trivial_schema_load(fhir_schema, fhir_validator):
     """Ensure whole schema can load"""
     for vertex_name in fhir_schema['$defs']:
 
         if not is_edge(fhir_schema['$defs'][vertex_name]):
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/data/test_pfb.py` & `iceberg_tools-0.0.3/tests/integration/data/test_pfb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from iceberg_tools.data.pfb import SimplePFBWriter
 from iceberg_tools.data.simplifier import simplify_directory
 
 
 def test_studies(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/study/', '**/*.*', 'tmp/study/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/CohesiveDataSet.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/study/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
 def test_synthea(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/synthea', '**/*.*', 'tmp/synthea/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/Synthea.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/synthea/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
 def test_kf(caplog, dependency_order):
     """Ensure we can create a pfb file from a Kids first study."""
     simplify_directory('tests/fixtures/simplify/kf', '**/*.*', 'tmp/kf/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/KidsFirst.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/kf/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -53,17 +53,17 @@
         print(inspection.warnings)
 
 
 def test_ncpi(caplog, dependency_order):
     """Ensure we can create a pfb file from a NCPI IG examples."""
 
     simplify_directory('tests/fixtures/simplify/ncpi/examples-5.0', '*.*', 'tmp/ncpi/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/NCPI.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/ncpi/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -72,17 +72,17 @@
 
 
 def test_genomics_reporting(caplog, dependency_order):
     """Ensure we can create a pfb file from a Genomics Reporting IG examples."""
 
     simplify_directory('tests/fixtures/simplify/genomics-reporting/examples-5.0',
                        '*.*', 'tmp/genomics-reporting/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/GenomicsReporting.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/genomics-reporting/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -90,17 +90,17 @@
         print(inspection.warnings)
 
 
 def test_dbgap(caplog, dependency_order):
     """Ensure we can create a pfb file from dbGAP examples."""
 
     simplify_directory('tests/fixtures/simplify/dbgap/examples-5.0', '*.*', 'tmp/dbgap/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/dbGap.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/dbgap/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -108,17 +108,17 @@
         print(inspection.warnings)
 
 
 def test_anvil(caplog, dependency_order):
     """Ensure we can create a pfb file from AnVIL examples."""
 
     simplify_directory('tests/fixtures/simplify/anvil/fhir-5.0/', '**/*.*', 'tmp/anvil/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
+    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
                                  output_path='tmp/AnVIL.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/anvil/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/conftest.py` & `iceberg_tools-0.0.3/tests/integration/simplified/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 import os
 
 from dictionaryutils import DataDictionary
 
 
 @pytest.fixture()
-def gen3_dir():
-    """cd to gen3 dir"""
+def simplified_dir():
+    """cd to simplified dir"""
     # setup
     cwd = os.getcwd()
-    os.chdir('iceberg/schemas/gen3')
+    os.chdir('iceberg/schemas/simplified')
     # run test
-    yield 'iceberg/schemas/gen3_dir'
+    yield 'iceberg/schemas/simplified'
     # teardown
     os.chdir(cwd)
 
 
 @pytest.fixture()
-def data_dictionary_from_yaml(gen3_dir) -> DataDictionary:
+def data_dictionary_from_yaml(simplified_dir) -> DataDictionary:
     """Load the schema from individual yaml files."""
     yield DataDictionary(root_dir=os.getcwd())
 
 
 @pytest.fixture()
-def distribution_schema(gen3_dir) -> dict:
-    """Load the aced.json schema"""
-    yield json.load(open("aced.json"))
+def distribution_schema(simplified_dir) -> dict:
+    """Load the simplified-fhir schema"""
+    yield json.load(open("simplified-fhir.json"))
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_codeable_concept.py` & `iceberg_tools-0.0.3/tests/integration/simplified/test_codeable_concept.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_primitive.py` & `iceberg_tools-0.0.3/tests/integration/simplified/test_primitive.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_research_study_has_project.py` & `iceberg_tools-0.0.3/tests/integration/simplified/test_research_study_has_project.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_medication.py` & `iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_medication.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         "reason": [
             {"reference": {"reference": "Condition/83d3ecf0-0ce7-473c-ac31-1f4be6c5780d"}}]
     }
 
     medication_administration = MedicationAdministration(**medication_administration)
     with SimplifierContextManager():
 
-        simplified, references = simplify(medication_administration, dialect='GEN3')
-        rendered = _render_dialect(simplified, references, 'GEN3', schemas=distribution_schema)
+        simplified, references = simplify(medication_administration, dialect='PFB')
+        rendered = _render_dialect(simplified, references, 'PFB', schemas=distribution_schema)
 
         print(orjson.dumps(rendered, option=orjson.OPT_INDENT_2).decode())
 
         assert 'medication' in rendered['object'], "Should render CodeableReference codeable"
         assert len(rendered['relations']) > 0
         condition = next(iter([_ for _ in rendered['relations'] if _['dst_name'] == 'condition']), None)
         assert condition, "Should render Condition relation"
```

### Comparing `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_task.py` & `iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             {"type": {"coding": [{"code": "DocumentReference"}]},
              "valueReference": {"reference": "DocumentReference/64ca4c81-d466-5eb6-b57e-62238241c0e4"}}]
     }
 
     task = Task(**task)
     with SimplifierContextManager():
 
-        simplified, references = simplify(task, dialect='GEN3')
-        rendered = _render_dialect(simplified, references, 'GEN3', schemas=distribution_schema)
+        simplified, references = simplify(task, dialect='PFB')
+        rendered = _render_dialect(simplified, references, 'PFB', schemas=distribution_schema)
 
         print(orjson.dumps(rendered, option=orjson.OPT_INDENT_2).decode())
 
         assert len(rendered['relations']) > 0
         document_reference = next(iter([_ for _ in rendered['relations'] if _['dst_name'] == 'document_reference']), None)
         assert document_reference, "Should render DocumentReference relation"
```

### Comparing `iceberg_tools-0.0.2rc3/tests/unit/test_coding_conventions.py` & `iceberg_tools-0.0.3/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc3/tests/unit/test_schema.py` & `iceberg_tools-0.0.3/tests/unit/test_schema.py`

 * *Files identical despite different names*

