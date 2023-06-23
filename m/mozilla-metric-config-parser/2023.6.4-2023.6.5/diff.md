# Comparing `tmp/mozilla-metric-config-parser-2023.6.4.tar.gz` & `tmp/mozilla-metric-config-parser-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2023.6.4.tar", last modified: Wed Jun 14 18:13:55 2023, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2023.6.5.tar", last modified: Fri Jun 23 21:21:06 2023, max compression
```

## Comparing `mozilla-metric-config-parser-2023.6.4.tar` & `mozilla-metric-config-parser-2023.6.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    27669 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9608 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    12463 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.439258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     4708 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    19957 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    14533 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 18:13:55.000000 mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-14 18:13:55.443258 mozilla-metric-config-parser-2023.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-14 18:13:46.000000 mozilla-metric-config-parser-2023.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.509301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    27669 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    14411 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.509301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    25190 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    14533 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/setup.py
```

### Comparing `mozilla-metric-config-parser-2023.6.4/LICENSE` & `mozilla-metric-config-parser-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/PKG-INFO` & `mozilla-metric-config-parser-2023.6.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/config.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/function.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,22 +62,23 @@
     Metric representation.
 
     Metrics are supersets of mozanalysis metrics with additional
     metadata required for analysis.
     """
 
     name: str
-    data_source: DataSource
-    select_expression: str
+    data_source: Optional[DataSource]
+    select_expression: Optional[str]
     friendly_name: Optional[str] = None
     description: Optional[str] = None
     bigger_is_better: bool = True
     analysis_bases: List[AnalysisBasis] = [AnalysisBasis.ENROLLMENTS, AnalysisBasis.EXPOSURES]
     type: str = "scalar"
     category: Optional[str] = None
+    depends_on: Optional[List[Summary]] = None
 
 
 @attr.s(auto_attribs=True)
 class MetricReference:
     name: str
 
     def resolve(
@@ -115,14 +116,15 @@
     data_source: Optional[DataSourceReference] = None
     friendly_name: Optional[str] = None
     description: Optional[str] = None
     bigger_is_better: bool = True
     analysis_bases: Optional[List[AnalysisBasis]] = None
     type: Optional[str] = None
     category: Optional[str] = None
+    depends_on: Optional[List[MetricReference]] = None
 
     @staticmethod
     def generate_select_expression(
         param_definitions: Dict[str, ParameterDefinition],
         select_expr_template: Union[str, jinja2.nodes.Template],
         configs: "ConfigCollection",
     ) -> str:
@@ -160,30 +162,66 @@
         self,
         spec: "DefinitionSpecSub",
         conf: Union["ExperimentConfiguration", "ProjectConfiguration"],
         configs: "ConfigCollection",
     ) -> List[Summary]:
         metric_summary = None
         metric = None
+        upstream_metrics = None
+
+        # check if metric depends on other metrics
+        if self.depends_on:
+            upstream_metrics = []
+            # resolve upstream metrics
+            for metric_ref in self.depends_on:
+                # check if upstream metric is defined externally as a "definition"
+                upstream_metric = configs.get_metric_definition(metric_ref.name, conf.app_name)
+
+                if upstream_metric is None:
+                    # check if upstream metric is part of the analysis spec
+                    upstream_metric = spec.metrics.definitions.get(metric_ref.name, None)
+
+                if upstream_metric is None:
+                    raise DefinitionNotFound(
+                        f"No definition found for referenced upstream metric {metric_ref}"
+                    )
+
+                upstream_metrics += upstream_metric.resolve(spec, conf, configs)
 
         if self.select_expression is None or self.data_source is None:
             # checks if a metric from mozanalysis was referenced
             metric_definition = configs.get_metric_definition(self.name, conf.app_name)
 
-            if metric_definition is None:
+            if metric_definition is None and upstream_metrics is None:
                 raise DefinitionNotFound(
                     f"No default definition found for referenced metric {self.name}"
                 )
-
-            metric_definition.analysis_bases = self.analysis_bases or [
-                AnalysisBasis.ENROLLMENTS,
-                AnalysisBasis.EXPOSURES,
-            ]
-            metric_definition.statistics = self.statistics
-            metric_summary = metric_definition.resolve(spec, conf, configs)
+            elif upstream_metrics:
+                metric = Metric(
+                    name=self.name,
+                    data_source=None,
+                    select_expression=None,
+                    friendly_name=dedent(self.friendly_name)
+                    if self.friendly_name
+                    else self.friendly_name,
+                    description=dedent(self.description) if self.description else self.description,
+                    bigger_is_better=self.bigger_is_better,
+                    analysis_bases=self.analysis_bases
+                    or [AnalysisBasis.ENROLLMENTS, AnalysisBasis.EXPOSURES],
+                    type=self.type or "scalar",
+                    category=self.category,
+                    depends_on=upstream_metrics,
+                )
+            elif metric_definition:
+                metric_definition.analysis_bases = self.analysis_bases or [
+                    AnalysisBasis.ENROLLMENTS,
+                    AnalysisBasis.EXPOSURES,
+                ]
+                metric_definition.statistics = self.statistics
+                metric_summary = metric_definition.resolve(spec, conf, configs)
         else:
             select_expression = self.generate_select_expression(
                 spec.parameters.definitions,
                 select_expr_template=self.select_expression,
                 configs=configs,
             )
 
@@ -196,14 +234,15 @@
                 else self.friendly_name,
                 description=dedent(self.description) if self.description else self.description,
                 bigger_is_better=self.bigger_is_better,
                 analysis_bases=self.analysis_bases
                 or [AnalysisBasis.ENROLLMENTS, AnalysisBasis.EXPOSURES],
                 type=self.type or "scalar",
                 category=self.category,
+                depends_on=upstream_metrics,
             )
 
         metrics_with_treatments = []
 
         if metric_summary:
             if self.statistics:
                 for statistic_name, params in self.statistics.items():
```

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/population.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/project.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import toml
 from cattrs.errors import ClassValidationError
 
 from metric_config_parser.analysis import AnalysisConfiguration, AnalysisSpec
 from metric_config_parser.data_source import DataSource
 from metric_config_parser.errors import InvalidConfigurationException
 from metric_config_parser.exposure_signal import AnalysisWindow, ExposureSignal
-from metric_config_parser.metric import AnalysisBasis, AnalysisPeriod
+from metric_config_parser.metric import (
+    AnalysisBasis,
+    AnalysisPeriod,
+    DefinitionNotFound,
+)
 from metric_config_parser.parameter import ParameterDefinition, ParameterSpec
 
 TEST_DIR = Path(__file__).parent
 DEFAULT_METRICS_CONFIG = TEST_DIR / "data" / "jetstream" / "defaults" / "firefox_desktop.toml"
 
 
 class TestAnalysisSpec:
@@ -564,7 +568,173 @@
         ),
     )
     def test__merge_param_raises(self, input):
         param_definition_1, param_definition_2 = input
 
         with pytest.raises(InvalidConfigurationException):
             AnalysisSpec._merge_param(param_definition_1, param_definition_2)
+
+    def test_depends_on_metric(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["spam", "ham", "spam_ham"]
+
+            [metrics.spam]
+            data_source = "main"
+            select_expression = "1"
+
+            [metrics.spam.statistics.bootstrap_mean]
+
+            [metrics.ham]
+            data_source = "main"
+            select_expression = "2"
+
+            [metrics.ham.statistics.bootstrap_mean]
+
+            [metrics.spam_ham]
+            depends_on = ["spam", "ham"]
+
+            [metrics.spam_ham.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+        cfg = spec.resolve(experiments[0], config_collection)
+
+        assert len(cfg.metrics[AnalysisPeriod.WEEK]) == 3
+
+        metric = [m for m in cfg.metrics[AnalysisPeriod.WEEK] if m.metric.name == "spam_ham"][
+            0
+        ].metric
+        assert metric.select_expression is None
+        assert metric.data_source is None
+        assert len(metric.depends_on) == 2
+
+        upstream_metrics = [m.metric.name for m in metric.depends_on]
+        assert "spam" in upstream_metrics
+        assert "ham" in upstream_metrics
+
+    def test_depends_on_definition(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["active_hours", "view_about_logins", "combined_metric"]
+
+            [metrics.combined_metric]
+            depends_on = ["active_hours", "view_about_logins"]
+
+            [metrics.combined_metric.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+        cfg = spec.resolve(experiments[0], config_collection)
+
+        assert len(cfg.metrics[AnalysisPeriod.WEEK]) == 3
+
+        metric = [
+            m for m in cfg.metrics[AnalysisPeriod.WEEK] if m.metric.name == "combined_metric"
+        ][0].metric
+        assert metric.select_expression is None
+        assert metric.data_source is None
+        assert len(metric.depends_on) == 2
+
+        upstream_metrics = [m.metric.name for m in metric.depends_on]
+        assert "active_hours" in upstream_metrics
+        assert "view_about_logins" in upstream_metrics
+
+    def test_non_existing_depends_on(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["combined_metric"]
+
+            [metrics.combined_metric]
+            depends_on = ["non_existing"]
+
+            [metrics.combined_metric.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+
+        with pytest.raises(DefinitionNotFound):
+            spec.resolve(experiments[0], config_collection)
+
+    def test_empty_metric_definition_not_allowed(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["empty_metric"]
+
+            [metrics.empty_metric]
+
+            [metrics.empty_metric.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+
+        with pytest.raises(DefinitionNotFound):
+            spec.resolve(experiments[0], config_collection)
+
+    def test_circular_depends_on(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["spam", "ham"]
+
+            [metrics.spam]
+            depends_on = ["ham"]
+
+            [metrics.spam.statistics.bootstrap_mean]
+
+            [metrics.ham]
+            depends_on = ["spam"]
+
+            [metrics.ham.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+
+        with pytest.raises(RecursionError):
+            spec.resolve(experiments[0], config_collection)
+
+    def test_multiple_nesting(self, experiments, config_collection):
+        config_str = dedent(
+            """
+            [metrics]
+            weekly = ["spam", "ham", "wham"]
+
+            [metrics.spam]
+            data_source = "main"
+            select_expression = "1"
+
+            [metrics.spam.statistics.bootstrap_mean]
+
+            [metrics.ham]
+            depends_on = ["spam"]
+
+            [metrics.ham.statistics.bootstrap_mean]
+
+            [metrics.wham]
+            depends_on = ["ham"]
+
+            [metrics.wham.statistics.bootstrap_mean]
+            """
+        )
+
+        spec = AnalysisSpec.from_dict(toml.loads(config_str))
+        cfg = spec.resolve(experiments[0], config_collection)
+
+        assert len(cfg.metrics[AnalysisPeriod.WEEK]) == 3
+
+        metric = [m for m in cfg.metrics[AnalysisPeriod.WEEK] if m.metric.name == "wham"][0].metric
+        assert metric.select_expression is None
+        assert metric.data_source is None
+        assert len(metric.depends_on) == 1
+        assert metric.depends_on[0].metric.name == "ham"
+        assert len(metric.depends_on[0].metric.depends_on) == 1
+        assert metric.depends_on[0].metric.depends_on[0].metric.name == "spam"
+        assert metric.depends_on[0].metric.depends_on[0].metric.select_expression == "1"
```

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/metric_config_parser/util.py` & `mozilla-metric-config-parser-2023.6.5/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.4/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.4/setup.py` & `mozilla-metric-config-parser-2023.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2023.6.4",
+    version="2023.6.5",
 )
```

