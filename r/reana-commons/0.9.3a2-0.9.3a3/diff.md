# Comparing `tmp/reana-commons-0.9.3a2.tar.gz` & `tmp/reana-commons-0.9.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reana-commons-0.9.3a2.tar", last modified: Mon Mar 20 15:30:57 2023, max compression
+gzip compressed data, was "reana-commons-0.9.3a3.tar", last modified: Fri Jun 23 14:26:30 2023, max compression
```

## Comparing `reana-commons-0.9.3a2.tar` & `reana-commons-0.9.3a3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.891457 reana-commons-0.9.3a2/
--rw-r--r--   0 madonado   (501) staff       (20)      272 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/.flake8
--rw-r--r--   0 madonado   (501) staff       (20)     1161 2023-03-20 15:29:06.000000 reana-commons-0.9.3a2/AUTHORS.rst
--rw-r--r--   0 madonado   (501) staff       (20)     9963 2023-03-20 15:29:06.000000 reana-commons-0.9.3a2/CHANGES.rst
--rw-r--r--   0 madonado   (501) staff       (20)      676 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/CONTRIBUTING.rst
--rw-r--r--   0 madonado   (501) staff       (20)     1092 2023-02-24 09:26:28.000000 reana-commons-0.9.3a2/LICENSE
--rw-r--r--   0 madonado   (501) staff       (20)      601 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/MANIFEST.in
--rw-r--r--   0 madonado   (501) staff       (20)    13350 2023-03-20 15:30:57.891688 reana-commons-0.9.3a2/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)     2114 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/README.rst
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.873765 reana-commons-0.9.3a2/docs/
--rw-r--r--   0 madonado   (501) staff       (20)     6508 2023-02-24 09:26:28.000000 reana-commons-0.9.3a2/docs/conf.py
--rw-r--r--   0 madonado   (501) staff       (20)     1361 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/docs/index.rst
--rw-r--r--   0 madonado   (501) staff       (20)      240 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/docs/requirements.txt
--rw-r--r--   0 madonado   (501) staff       (20)      308 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/pytest.ini
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.878737 reana-commons-0.9.3a2/reana_commons/
--rw-r--r--   0 madonado   (501) staff       (20)      377 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)     8543 2022-12-12 10:24:13.000000 reana-commons-0.9.3a2/reana_commons/api_client.py
--rw-r--r--   0 madonado   (501) staff       (20)    16844 2023-01-13 10:27:42.000000 reana-commons-0.9.3a2/reana_commons/config.py
--rw-r--r--   0 madonado   (501) staff       (20)     2595 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/consumer.py
--rw-r--r--   0 madonado   (501) staff       (20)     1947 2022-09-22 12:50:04.000000 reana-commons-0.9.3a2/reana_commons/email.py
--rw-r--r--   0 madonado   (501) staff       (20)     2950 2022-11-21 09:18:07.000000 reana-commons-0.9.3a2/reana_commons/errors.py
--rw-r--r--   0 madonado   (501) staff       (20)     1859 2022-03-30 10:25:47.000000 reana-commons-0.9.3a2/reana_commons/job_utils.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.882219 reana-commons-0.9.3a2/reana_commons/k8s/
--rw-r--r--   0 madonado   (501) staff       (20)      265 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/k8s/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)     1925 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/k8s/api_client.py
--rw-r--r--   0 madonado   (501) staff       (20)     4330 2023-01-18 14:17:44.000000 reana-commons-0.9.3a2/reana_commons/k8s/kerberos.py
--rw-r--r--   0 madonado   (501) staff       (20)    11521 2022-03-30 10:25:47.000000 reana-commons-0.9.3a2/reana_commons/k8s/secrets.py
--rw-r--r--   0 madonado   (501) staff       (20)     3248 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/k8s/volumes.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.883339 reana-commons-0.9.3a2/reana_commons/openapi_specifications/
--rw-r--r--   0 madonado   (501) staff       (20)    12023 2022-09-19 08:59:20.000000 reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_job_controller.json
--rw-r--r--   0 madonado   (501) staff       (20)   137719 2023-03-20 15:29:06.000000 reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_server.json
--rw-r--r--   0 madonado   (501) staff       (20)    50816 2022-11-24 15:09:51.000000 reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_workflow_controller.json
--rw-r--r--   0 madonado   (501) staff       (20)     6332 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/publisher.py
--rw-r--r--   0 madonado   (501) staff       (20)     8302 2022-09-19 08:59:20.000000 reana-commons-0.9.3a2/reana_commons/serial.py
--rw-r--r--   0 madonado   (501) staff       (20)     7051 2022-04-28 15:01:43.000000 reana-commons-0.9.3a2/reana_commons/snakemake.py
--rw-r--r--   0 madonado   (501) staff       (20)     4101 2023-02-24 09:26:28.000000 reana-commons-0.9.3a2/reana_commons/specification.py
--rw-r--r--   0 madonado   (501) staff       (20)    17086 2023-02-13 09:19:24.000000 reana-commons-0.9.3a2/reana_commons/utils.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.885244 reana-commons-0.9.3a2/reana_commons/validation/
--rw-r--r--   0 madonado   (501) staff       (20)      268 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/validation/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)     6129 2022-03-29 07:52:46.000000 reana-commons-0.9.3a2/reana_commons/validation/compute_backends.py
--rw-r--r--   0 madonado   (501) staff       (20)     2093 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/validation/operational_options.py
--rw-r--r--   0 madonado   (501) staff       (20)    17863 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/validation/parameters.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.885560 reana-commons-0.9.3a2/reana_commons/validation/schemas/
--rw-r--r--   0 madonado   (501) staff       (20)     6139 2022-07-08 11:45:07.000000 reana-commons-0.9.3a2/reana_commons/validation/schemas/reana_analysis_schema.json
--rw-r--r--   0 madonado   (501) staff       (20)     2779 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/validation/utils.py
--rwxr-xr-x   0 madonado   (501) staff       (20)      458 2023-03-20 15:29:06.000000 reana-commons-0.9.3a2/reana_commons/version.py
--rw-r--r--   0 madonado   (501) staff       (20)     7404 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/reana_commons/workflow_engine.py
--rw-r--r--   0 madonado   (501) staff       (20)     7536 2023-02-02 15:27:51.000000 reana-commons-0.9.3a2/reana_commons/workspace.py
--rw-r--r--   0 madonado   (501) staff       (20)     2163 2022-03-30 10:25:47.000000 reana-commons-0.9.3a2/reana_commons/yadage.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.880508 reana-commons-0.9.3a2/reana_commons.egg-info/
--rw-r--r--   0 madonado   (501) staff       (20)    13350 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)     1702 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/SOURCES.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/dependency_links.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/not-zip-safe
--rw-r--r--   0 madonado   (501) staff       (20)      766 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/requires.txt
--rw-r--r--   0 madonado   (501) staff       (20)       14 2023-03-20 15:30:57.000000 reana-commons-0.9.3a2/reana_commons.egg-info/top_level.txt
--rwxr-xr-x   0 madonado   (501) staff       (20)     1172 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/run-tests.sh
--rw-r--r--   0 madonado   (501) staff       (20)      136 2023-03-20 15:30:57.892579 reana-commons-0.9.3a2/setup.cfg
--rwxr-xr-x   0 madonado   (501) staff       (20)     3331 2023-02-02 15:27:51.000000 reana-commons-0.9.3a2/setup.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-03-20 15:30:57.891007 reana-commons-0.9.3a2/tests/
--rw-r--r--   0 madonado   (501) staff       (20)     1317 2023-02-21 12:54:49.000000 reana-commons-0.9.3a2/tests/conftest.py
--rw-r--r--   0 madonado   (501) staff       (20)      718 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/tests/test_email.py
--rw-r--r--   0 madonado   (501) staff       (20)     3200 2022-03-30 10:25:47.000000 reana-commons-0.9.3a2/tests/test_job_utils.py
--rw-r--r--   0 madonado   (501) staff       (20)     2700 2022-03-30 10:25:47.000000 reana-commons-0.9.3a2/tests/test_mq.py
--rw-r--r--   0 madonado   (501) staff       (20)     1659 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/tests/test_operational_options.py
--rw-r--r--   0 madonado   (501) staff       (20)     3925 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/tests/test_secrets_store.py
--rw-r--r--   0 madonado   (501) staff       (20)     1383 2022-11-14 14:24:49.000000 reana-commons-0.9.3a2/tests/test_snakemake.py
--rw-r--r--   0 madonado   (501) staff       (20)     1674 2023-02-24 09:26:28.000000 reana-commons-0.9.3a2/tests/test_specification.py
--rw-r--r--   0 madonado   (501) staff       (20)     4726 2023-02-13 09:19:24.000000 reana-commons-0.9.3a2/tests/test_utils.py
--rw-r--r--   0 madonado   (501) staff       (20)     1004 2022-07-08 11:45:07.000000 reana-commons-0.9.3a2/tests/test_validation.py
--rw-r--r--   0 madonado   (501) staff       (20)      446 2022-03-25 14:09:43.000000 reana-commons-0.9.3a2/tests/test_version.py
--rw-r--r--   0 madonado   (501) staff       (20)    10248 2022-11-22 16:13:14.000000 reana-commons-0.9.3a2/tests/test_workspace.py
--rw-r--r--   0 madonado   (501) staff       (20)      333 2022-11-14 14:24:49.000000 reana-commons-0.9.3a2/tox.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      272 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/.flake8
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1161 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/AUTHORS.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    10156 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/CHANGES.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      676 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/CONTRIBUTING.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1092 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/LICENSE
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      601 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/MANIFEST.in
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    13543 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2114 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/README.rst
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.453793 reana-commons-0.9.3a3/docs/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6508 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/conf.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1361 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/index.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      240 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/requirements.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      308 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/pytest.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.455793 reana-commons-0.9.3a3/reana_commons/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      377 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     8543 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/api_client.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    16844 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/config.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2588 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/consumer.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2350 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/email.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2950 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/errors.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1859 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/job_utils.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.456793 reana-commons-0.9.3a3/reana_commons/k8s/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      265 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/api_client.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4330 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/kerberos.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    11521 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/secrets.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/volumes.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.456793 reana-commons-0.9.3a3/reana_commons/openapi_specifications/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    12023 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_job_controller.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)   137719 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_server.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    50816 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_workflow_controller.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6328 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/publisher.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     8302 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/serial.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7051 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/snakemake.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4101 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/specification.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    17086 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/utils.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.457793 reana-commons-0.9.3a3/reana_commons/validation/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      268 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6129 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/compute_backends.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2093 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/operational_options.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    17863 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/parameters.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.457793 reana-commons-0.9.3a3/reana_commons/validation/schemas/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6528 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/schemas/reana_analysis_schema.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2779 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/utils.py
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)      458 2023-06-23 14:25:16.000000 reana-commons-0.9.3a3/reana_commons/version.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7404 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/workflow_engine.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7536 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/workspace.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2163 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/yadage.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.455793 reana-commons-0.9.3a3/reana_commons.egg-info/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    13543 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1702 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/not-zip-safe
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      766 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/requires.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)       14 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/top_level.txt
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     1172 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/run-tests.sh
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      136 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/setup.cfg
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     3331 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/setup.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/tests/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1317 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/conftest.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      718 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_email.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3200 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_job_utils.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2700 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_mq.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1659 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_operational_options.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_secrets_store.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1383 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_snakemake.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1674 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_specification.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4726 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_utils.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1004 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_validation.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      446 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_version.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    10248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_workspace.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      333 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tox.ini
```

### Comparing `reana-commons-0.9.3a2/AUTHORS.rst` & `reana-commons-0.9.3a3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/CHANGES.rst` & `reana-commons-0.9.3a3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Changes
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
+- Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
```

### Comparing `reana-commons-0.9.3a2/CONTRIBUTING.rst` & `reana-commons-0.9.3a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/LICENSE` & `reana-commons-0.9.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/MANIFEST.in` & `reana-commons-0.9.3a3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/PKG-INFO` & `reana-commons-0.9.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-commons
-Version: 0.9.3a2
+Version: 0.9.3a3
 Summary: REANA-Commons.
 Home-page: https://github.com/reanahub/reana-commons
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -95,14 +95,16 @@
 Changes
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
+- Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
```

### Comparing `reana-commons-0.9.3a2/README.rst` & `reana-commons-0.9.3a3/README.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/docs/conf.py` & `reana-commons-0.9.3a3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,9 +203,9 @@
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
 
 # Intersphinx configuration
 intersphinx_mapping = {
-    "kombu": ("https://docs.celeryq.dev/projects/kombu/en/latest/", None),
+    "kombu": ("https://docs.celeryq.dev/projects/kombu/en/stable/", None),
 }
```

### Comparing `reana-commons-0.9.3a2/docs/index.rst` & `reana-commons-0.9.3a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/api_client.py` & `reana-commons-0.9.3a3/reana_commons/api_client.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/config.py` & `reana-commons-0.9.3a3/reana_commons/config.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/consumer.py` & `reana-commons-0.9.3a3/reana_commons/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,49 +20,49 @@
 
 class BaseConsumer(ConsumerMixin):
     """Base RabbitMQ consumer."""
 
     def __init__(self, queue=None, connection=None, message_default_format=None):
         """Construct a BaseConsumer.
 
-        :param connection: A :class:`kombu.Connection`, if not provided a
-            :class:`kombu.Connection` with the default configuration will
+        :param connection: A class:`kombu.Connection`, if not provided a
+            class:`kombu.Connection` with the default configuration will
             be instantiated.
-        :param queue: Name or :class:`kombu.Queue` where the messages will
+        :param queue: Name or class:`kombu.Queue` where the messages will
             be consumed from.
         :param message_default_format: Defines the format the consuemer is
             configured to deserialize the messages to.
         """
         self.exchange = self._build_default_exchange()
         if not isinstance(queue, Queue):
             queue = Queue(queue, **MQ_DEFAULT_QUEUES[queue])
         self.queue = queue
         self.connection = connection or Connection(MQ_CONNECTION_STRING)
         self.message_default_format = message_default_format or MQ_DEFAULT_FORMAT
 
     def _build_default_exchange(self):
-        """Build :class:`kombu.Exchange` with default values."""
+        """Build class:`kombu.Exchange` with default values."""
         return Exchange(MQ_DEFAULT_EXCHANGE, type="direct")
 
     def get_consumers(self, Consumer, channel):
         """Map consumers to specific queues.
 
-        :param Consumer: A :class:`kombu.Consumer` to use for instantiating
+        :param Consumer: A class:`kombu.Consumer` to use for instantiating
             consumers.
-        :param channel: A :class:`kombu.transport.virtual.AbstractChannel`.
+        :param channel: A class:`kombu.transport.virtual.AbstractChannel`.
         """
         # return [Consumer(queues=self.queues,
         #                  callbacks=[self.on_message],
         #                  accept=[MQ_DEFAULT_FORMAT]))]
         raise NotImplementedError(
             "Implement this method to map which"
             "callbacks are connected with which queues"
         )
 
     def on_message(self, body, message):
         """Implement this method to manipulate the data received.
 
         :param body: The received message already decoded in the specified
             format.
-        :param message: A :class:`kombu.transport.virtual.Message`.
+        :param message: A class:`kombu.transport.virtual.Message`.
         """
         raise NotImplementedError("Implement this method to react to events.")
```

### Comparing `reana-commons-0.9.3a2/reana_commons/email.py` & `reana-commons-0.9.3a3/reana_commons/email.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of REANA.
-# Copyright (C) 2020, 2022 CERN.
+# Copyright (C) 2020, 2022, 2023 CERN.
 #
 # REANA is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 """REANA-Commons email util."""
 
+from distutils.util import strtobool
 from email.message import EmailMessage
 import logging
 import os
 import smtplib
 import ssl
 
 from reana_commons.errors import REANAEmailNotificationError
 
 # Email configuration
 REANA_EMAIL_SMTP_SERVER = os.getenv("REANA_EMAIL_SMTP_SERVER")
 REANA_EMAIL_SMTP_PORT = os.getenv("REANA_EMAIL_SMTP_PORT")
 REANA_EMAIL_LOGIN = os.getenv("REANA_EMAIL_LOGIN")
 REANA_EMAIL_SENDER = os.getenv("REANA_EMAIL_SENDER")
 REANA_EMAIL_PASSWORD = os.getenv("REANA_EMAIL_PASSWORD")
+REANA_EMAIL_SMTP_SSL = bool(strtobool(os.getenv("REANA_EMAIL_SMTP_SSL", "False")))
+REANA_EMAIL_SMTP_STARTTLS = bool(
+    strtobool(os.getenv("REANA_EMAIL_SMTP_STARTTLS", "True"))
+)
 
 
 def send_email(
     receiver_email,
     subject,
     body,
     login_email=REANA_EMAIL_LOGIN,
@@ -33,25 +38,34 @@
     """Send emails from REANA platform."""
     message = EmailMessage()
     message["From"] = f"REANA platform <{sender_email}>"
     message["To"] = receiver_email
     message["Subject"] = subject
     message.set_content(body)
 
-    context = ssl.create_default_context()
     if not (REANA_EMAIL_SMTP_SERVER and REANA_EMAIL_SMTP_PORT):
         raise REANAEmailNotificationError(
             "Cannot send email, missing server and port configuration. "
             "Please provide the following environment variables:\n"
             "REANA_EMAIL_SMTP_SERVER\nREANA_EMAIL_SMTP_PORT"
         )
-    with smtplib.SMTP(REANA_EMAIL_SMTP_SERVER, REANA_EMAIL_SMTP_PORT) as server:
-        if os.getenv("FLASK_ENV") != "development":
-            server.starttls(context=context)
-            server.login(login_email, REANA_EMAIL_PASSWORD)
-        server.send_message(message)
-        logging.info(
-            "Email sent, login: {}, sender: {}, receiver: {}".format(
-                login_email, sender_email, receiver_email
-            )
+
+    context = ssl.create_default_context()
+    if REANA_EMAIL_SMTP_SSL:
+        smtp_server = smtplib.SMTP_SSL(
+            REANA_EMAIL_SMTP_SERVER, REANA_EMAIL_SMTP_PORT, context=context
         )
-        logging.info("Body:\n{}".format(message))
+    else:
+        smtp_server = smtplib.SMTP(REANA_EMAIL_SMTP_SERVER, REANA_EMAIL_SMTP_PORT)
+
+    with smtp_server:
+        if REANA_EMAIL_SMTP_STARTTLS:
+            smtp_server.starttls(context=context)
+        if login_email or REANA_EMAIL_PASSWORD:
+            smtp_server.login(login_email, REANA_EMAIL_PASSWORD)
+        smtp_server.send_message(message)
+
+    logging.info(
+        f"Email sent, login: {login_email}, "
+        f"sender: {sender_email}, receiver: {receiver_email}\n"
+        f"Body:\n{message}"
+    )
```

### Comparing `reana-commons-0.9.3a2/reana_commons/errors.py` & `reana-commons-0.9.3a3/reana_commons/errors.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/job_utils.py` & `reana-commons-0.9.3a3/reana_commons/job_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/k8s/api_client.py` & `reana-commons-0.9.3a3/reana_commons/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/k8s/kerberos.py` & `reana-commons-0.9.3a3/reana_commons/k8s/kerberos.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/k8s/secrets.py` & `reana-commons-0.9.3a3/reana_commons/k8s/secrets.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/k8s/volumes.py` & `reana-commons-0.9.3a3/reana_commons/k8s/volumes.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_job_controller.json` & `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_job_controller.json`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_server.json` & `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_server.json`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/openapi_specifications/reana_workflow_controller.json` & `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_workflow_controller.json`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/publisher.py` & `reana-commons-0.9.3a3/reana_commons/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         connection=None,
         exchange=None,
         durable=False,
         max_priority=None,
     ):
         """Initialise the BasePublisher class.
 
-        :param connection: A :class:`kombu.Connection`, if not provided a
-            :class:`kombu.Connection` with the default configuration will
+        :param connection: A class:`kombu.Connection`, if not provided a
+            class:`kombu.Connection` with the default configuration will
             be instantiated.
         :param queue: String which represents the queue the messages will
             be sent to.
         :param routing_key: String which represents the routing key which
             will be used to send the messages, if not provided default
             routing key will be used.
-        :param exchange: A :class:`kombu.Exchange` where the messages will
+        :param exchange: A class:`kombu.Exchange` where the messages will
             be delivered to, if not provided, it will be instantiated with
             the default configuration.
         """
         self._routing_key = routing_key
         self._exchange = (
             exchange
             if isinstance(exchange, Exchange)
@@ -65,15 +65,15 @@
                 max_priority=max_priority,
             )
         )
         self._connection = connection or Connection(MQ_CONNECTION_STRING)
         self.producer = self._build_producer()
 
     def _build_producer(self):
-        """Instantiate a :class:`kombu.Producer`."""
+        """Instantiate a class:`kombu.Producer`."""
         return self._connection.Producer(serializer=MQ_DEFAULT_FORMAT)
 
     @staticmethod
     def __error_callback(exception: Exception, interval: int) -> None:
         """Execute when there is an error while sending a message.
 
         :param exception: Exception which has been thrown while trying to send
```

### Comparing `reana-commons-0.9.3a2/reana_commons/serial.py` & `reana-commons-0.9.3a3/reana_commons/serial.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/snakemake.py` & `reana-commons-0.9.3a3/reana_commons/snakemake.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/specification.py` & `reana-commons-0.9.3a3/reana_commons/specification.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/utils.py` & `reana-commons-0.9.3a3/reana_commons/utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/validation/compute_backends.py` & `reana-commons-0.9.3a3/reana_commons/validation/compute_backends.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/validation/operational_options.py` & `reana-commons-0.9.3a3/reana_commons/validation/operational_options.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/validation/parameters.py` & `reana-commons-0.9.3a3/reana_commons/validation/parameters.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/validation/schemas/reana_analysis_schema.json` & `reana-commons-0.9.3a3/reana_commons/validation/schemas/reana_analysis_schema.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9906712245324442%*

 * *Differences: {"'properties'": "{'inputs': {'properties': {'files': {delete: ['optional']}, 'directories': "*

 * *                 "{delete: ['optional']}, 'parameters': {delete: ['optional']}}}, 'workflow': "*

 * *                 "{'properties': {'resources': {'properties': {'cvmfs': {'items': {delete: "*

 * *                 "['optional']}}}}}}, 'outputs': {'properties': {'files': {delete: ['optional']}, "*

 * *                 "'directories': {delete: ['optional']}}}, 'tests': OrderedDict([('id', "*

 * *                 "'/properties/tests') […]*

```diff
@@ -13,40 +13,37 @@
                     "description": "List of directories provided as input for a given analysis.",
                     "id": "/properties/inputs/properties/directories",
                     "items": {
                         "id": "/properties/inputs/properties/directories/items",
                         "title": "Relative path to the directory.",
                         "type": "string"
                     },
-                    "optional": true,
                     "title": "Analysis input directories.",
                     "type": "array"
                 },
                 "files": {
                     "description": "List of files provided as input for a given analysis.",
                     "id": "/properties/inputs/properties/files",
                     "items": {
                         "id": "/properties/inputs/properties/files/items",
                         "title": "Relative path to the file.",
                         "type": "string"
                     },
-                    "optional": true,
                     "title": "Analysis input files.",
                     "type": "array"
                 },
                 "options": {
                     "description": "Extra operational options accepted by workflow engines.",
                     "id": "/properties/workflow/properties/options",
                     "title": "Workflow operational options.",
                     "type": "object"
                 },
                 "parameters": {
                     "description": "Key value data structure which represents the analysis parameters.",
                     "id": "/properties/inputs/properties/parameters",
-                    "optional": true,
                     "title": "Analysis parameters.",
                     "type": "object"
                 }
             },
             "title": "Analysis inputs.",
             "type": "object"
         },
@@ -58,34 +55,51 @@
                     "description": "Expected output from analysis represented by a set of directories.",
                     "id": "/properties/outputs/properties/directories",
                     "items": {
                         "id": "/properties/outputs/properties/directories/items",
                         "title": "Relative path to the directory.",
                         "type": "string"
                     },
-                    "optional": true,
                     "title": "Analysis result directories.",
                     "type": "array"
                 },
                 "files": {
                     "description": "Expected output from analysis represented by a set of files.",
                     "id": "/properties/outputs/properties/files",
                     "items": {
                         "id": "/properties/outputs/properties/files/items",
                         "title": "Relative path to the file.",
                         "type": "string"
                     },
-                    "optional": true,
                     "title": "Analysis result files.",
                     "type": "array"
                 }
             },
             "title": "Analysis outputs.",
             "type": "object"
         },
+        "tests": {
+            "additionalProperties": false,
+            "id": "/properties/tests",
+            "properties": {
+                "files": {
+                    "description": "Gherkin test feature files.",
+                    "id": "/properties/tests/properties/files",
+                    "items": {
+                        "id": "/properties/tests/properties/files/items",
+                        "title": "Relative path to the file.",
+                        "type": "string"
+                    },
+                    "title": "Analysis test files.",
+                    "type": "array"
+                }
+            },
+            "title": "Analysis tests.",
+            "type": "object"
+        },
         "version": {
             "description": "REANA platform version to which the analysis was written for.",
             "id": "/properties/version",
             "title": "REANA version.",
             "type": "string"
         },
         "workflow": {
@@ -114,15 +128,14 @@
                 },
                 "resources": {
                     "id": "/properties/workflow/properties/resources",
                     "properties": {
                         "cvmfs": {
                             "id": "/properties/workflow/properties/resources/properties/cvmfs",
                             "items": {
-                                "optional": false,
                                 "title": "CVMFS repos",
                                 "type": "string"
                             },
                             "type": "array"
                         },
                         "kerberos": {
                             "id": "/properties/workflow/properties/resources/properties/kerberos",
```

### Comparing `reana-commons-0.9.3a2/reana_commons/validation/utils.py` & `reana-commons-0.9.3a3/reana_commons/validation/utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/workflow_engine.py` & `reana-commons-0.9.3a3/reana_commons/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/workspace.py` & `reana-commons-0.9.3a3/reana_commons/workspace.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons/yadage.py` & `reana-commons-0.9.3a3/reana_commons/yadage.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons.egg-info/PKG-INFO` & `reana-commons-0.9.3a3/reana_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-commons
-Version: 0.9.3a2
+Version: 0.9.3a3
 Summary: REANA-Commons.
 Home-page: https://github.com/reanahub/reana-commons
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -95,14 +95,16 @@
 Changes
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
+- Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
```

### Comparing `reana-commons-0.9.3a2/reana_commons.egg-info/SOURCES.txt` & `reana-commons-0.9.3a3/reana_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/reana_commons.egg-info/requires.txt` & `reana-commons-0.9.3a3/reana_commons.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/run-tests.sh` & `reana-commons-0.9.3a3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/setup.py` & `reana-commons-0.9.3a3/setup.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/conftest.py` & `reana-commons-0.9.3a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_email.py` & `reana-commons-0.9.3a3/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_job_utils.py` & `reana-commons-0.9.3a3/tests/test_job_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_mq.py` & `reana-commons-0.9.3a3/tests/test_mq.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_operational_options.py` & `reana-commons-0.9.3a3/tests/test_operational_options.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_secrets_store.py` & `reana-commons-0.9.3a3/tests/test_secrets_store.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_snakemake.py` & `reana-commons-0.9.3a3/tests/test_snakemake.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_specification.py` & `reana-commons-0.9.3a3/tests/test_specification.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_utils.py` & `reana-commons-0.9.3a3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_validation.py` & `reana-commons-0.9.3a3/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a2/tests/test_workspace.py` & `reana-commons-0.9.3a3/tests/test_workspace.py`

 * *Files identical despite different names*

