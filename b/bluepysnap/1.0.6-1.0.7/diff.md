# Comparing `tmp/bluepysnap-1.0.6.tar.gz` & `tmp/bluepysnap-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepysnap-1.0.6.tar", last modified: Mon Jun 12 09:38:23 2023, max compression
+gzip compressed data, was "bluepysnap-1.0.7.tar", last modified: Fri Jun 23 12:13:01 2023, max compression
```

## Comparing `bluepysnap-1.0.6.tar` & `bluepysnap-1.0.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/_doctools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/bbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/edges/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24870 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/edge_population.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/frame_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/morph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/neuron_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/node_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28955 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/node_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/circuit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/datatypes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/edge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/node.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/edge/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical_virtual.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/electrical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/endfoot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/glialglial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/neuromodulatory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/synapse_astrocyte.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/node/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/astrocyte.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/biophysical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/vasculature.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/virtual.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/sonata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/spike_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-12 09:38:23.000000 bluepysnap-1.0.6/bluepysnap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.085936 bluepysnap-1.0.7/bluepysnap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/_doctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 12:13:00.000000 bluepysnap-1.0.7/bluepysnap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/bbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/circuit_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/circuit_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24911 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/edges/edge_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/edges/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/frame_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/neuron_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/node_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/nodes/node_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/nodes/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/circuit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/schemas/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/definitions/datatypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/definitions/edge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/definitions/node.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/schemas/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/chemical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/chemical_virtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/electrical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/endfoot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/glialglial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/neuromodulatory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/edge/synapse_astrocyte.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap/schemas/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/node/astrocyte.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/node/biophysical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/node/vasculature.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/node/virtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/sonata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/spike_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/bluepysnap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/bluepysnap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 12:13:01.000000 bluepysnap-1.0.7/bluepysnap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:13:01.089937 bluepysnap-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-23 12:12:56.000000 bluepysnap-1.0.7/setup.py
```

### Comparing `bluepysnap-1.0.6/COPYING` & `bluepysnap-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/COPYING.LESSER` & `bluepysnap-1.0.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/PKG-INFO` & `bluepysnap-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepysnap
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simulation and Neural network Analysis Productivity layer
 Home-page: https://github.com/BlueBrain/snap
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Keywords: SONATA,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Provides-Extra: spatial-index
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS.txt
 
 |banner|
 
-|build_status| |license| |coverage| |docs|
+|build_status| |license| |coverage| |docs| |DOI|
 
 Blue Brain SNAP
 ===============
 
 Blue Brain Simulation and Neural network Analysis Productivity layer (Blue Brain SNAP).
 
 Blue Brain SNAP is a Python library for accessing BlueBrain circuit models represented in
@@ -127,26 +127,30 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-.. |build_status| image:: https://travis-ci.com/BlueBrain/snap.svg?branch=master
-   :target: https://travis-ci.com/BlueBrain/snap
+.. |build_status| image:: https://github.com/BlueBrain/snap/actions/workflows/run-tox.yml/badge.svg
    :alt: Build Status
 
 .. |license| image:: https://img.shields.io/pypi/l/bluepysnap
-                :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :alt: License
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/snap/coverage.svg?branch=master
    :target: https://codecov.io/github/BlueBrain/snap?branch=master
    :alt: codecov.io
 
 .. |docs| image:: https://readthedocs.org/projects/bluebrainsnap/badge/?version=latest
-             :target: https://bluebrainsnap.readthedocs.io/
-             :alt: documentation status
+   :target: https://bluebrainsnap.readthedocs.io/
+   :alt: documentation status
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8026852.svg
+   :target: https://doi.org/10.5281/zenodo.8026852
+   :alt: DOI
 
 .. substitutions
 .. |banner| image:: doc/source/_images/BlueBrainSNAP.jpg
 .. |circuit| replace:: **Circuit**
 .. |simulation| replace:: **Simulation**
```

### Comparing `bluepysnap-1.0.6/README.rst` & `bluepysnap-1.0.7/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 |banner|
 
-|build_status| |license| |coverage| |docs|
+|build_status| |license| |coverage| |docs| |DOI|
 
 Blue Brain SNAP
 ===============
 
 Blue Brain Simulation and Neural network Analysis Productivity layer (Blue Brain SNAP).
 
 Blue Brain SNAP is a Python library for accessing BlueBrain circuit models represented in
@@ -101,26 +101,30 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-.. |build_status| image:: https://travis-ci.com/BlueBrain/snap.svg?branch=master
-   :target: https://travis-ci.com/BlueBrain/snap
+.. |build_status| image:: https://github.com/BlueBrain/snap/actions/workflows/run-tox.yml/badge.svg
    :alt: Build Status
 
 .. |license| image:: https://img.shields.io/pypi/l/bluepysnap
-                :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :alt: License
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/snap/coverage.svg?branch=master
    :target: https://codecov.io/github/BlueBrain/snap?branch=master
    :alt: codecov.io
 
 .. |docs| image:: https://readthedocs.org/projects/bluebrainsnap/badge/?version=latest
-             :target: https://bluebrainsnap.readthedocs.io/
-             :alt: documentation status
+   :target: https://bluebrainsnap.readthedocs.io/
+   :alt: documentation status
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8026852.svg
+   :target: https://doi.org/10.5281/zenodo.8026852
+   :alt: DOI
 
 .. substitutions
 .. |banner| image:: doc/source/_images/BlueBrainSNAP.jpg
 .. |circuit| replace:: **Circuit**
 .. |simulation| replace:: **Simulation**
```

### Comparing `bluepysnap-1.0.6/bluepysnap/__init__.py` & `bluepysnap-1.0.7/bluepysnap/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/_doctools.py` & `bluepysnap-1.0.7/bluepysnap/_doctools.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/_plotting.py` & `bluepysnap-1.0.7/bluepysnap/_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,28 +244,30 @@
     Args:
         x_axis (str): Node enum that will determine the animation x_axis
         y_axis (str): Node enum that will determine the animation y_axis
         dt (int) : the time bin size of each frame in the video in ms
         ax(matplotlib.Axis): matplotlib Axis to draw on (if not specified, pyplot.gca()
             and plt.figure() are used).
 
-    Returns :
+    Returns:
         (matplotlib.animation.FuncAnimation, matplotlib.Axis): the matplotlib animation object and
-            the corresponding axis.
+        the corresponding axis.
 
-    Notes:
+    Examples:
         From scripts:
+
         >>> import matplotlib.pyplot as plt
         >>> from bluepysnap import Simulation
         >>> report = Simulation("config.json").spikes["my_population"]
         >>> anim, ax = report.firing_animation()
         >>> plt.show()
         >>> # to save the animation : do not plt.show() and just anim.save('my_movie.mp4')
 
         From notebooks:
+
         >>> from IPython.display import HTML
         >>> from bluepysnap import Simulation
         >>> report = Simulation("config.json").spikes["my_population"]
         >>> anim, ax = report.firing_animation()
         >>> HTML(anim.to_html5_video())
     """
     plt = _get_pyplot()
```

### Comparing `bluepysnap-1.0.6/bluepysnap/bbp.py` & `bluepysnap-1.0.7/bluepysnap/bbp.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/circuit.py` & `bluepysnap-1.0.7/bluepysnap/circuit.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/circuit_ids.py` & `bluepysnap-1.0.7/bluepysnap/circuit_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             this function takes randomly ``sample_size`` values of a circuit node ids.
 
         Args:
             sample_size (int): the size of the sample. If the size of the sample is greater than
                 the size of the CircuitIds then all ids are taken and shuffled.
             inplace (bool): if set to True. Do the transformation inplace.
         """
-        sampling = np.random.choice(len(self), size=min(sample_size, len(self)))
+        sampling = np.random.choice(len(self), size=min(sample_size, len(self)), replace=False)
         return self._apply(lambda x: x[sampling], inplace)
 
     def limit(self, limit_size, inplace=False):
         """Limit the size of a CircuitIds.
 
         Notes:
             this function takes the first ``limit_size`` values of a circuit node ids.
@@ -249,14 +249,26 @@
         """Returns only unique CircuitIds.
 
         Notes:
             this function does not sort the ids
         """
         return self._apply(lambda x: x.unique(), inplace)
 
+    def intersection(self, circuit_ids, inplace=False):
+        """Take the intersection of this CircuitIds and the input.
+
+        The index of the resulting object is sorted if ``inplace=False``.
+        Otherwise, the orginal order of the index is kept.
+
+        Args:
+            circuit_ids (CircuitIds): The CircuitIds to intersect with.
+            inplace (bool): if set to True, do the transformation inplace.
+        """
+        return self._apply(lambda x: x.intersection(circuit_ids.index), inplace)
+
     def to_csv(self, filepath):
         """Save CircuitIds to csv format."""
         self.index.to_frame(index=False).to_csv(filepath, index=False)
 
     @classmethod
     def from_csv(cls, filepath):
         """Load CircuitIds from csv."""
```

### Comparing `bluepysnap-1.0.6/bluepysnap/circuit_validation.py` & `bluepysnap-1.0.7/bluepysnap/circuit_validation.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/cli.py` & `bluepysnap-1.0.7/bluepysnap/cli.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/config.py` & `bluepysnap-1.0.7/bluepysnap/config.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/edges/edge_population.py` & `bluepysnap-1.0.7/bluepysnap/edges/edge_population.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,16 @@
     def _topology_property_names(self):
         return {Edge.SOURCE_NODE_ID, Edge.TARGET_NODE_ID}
 
     @property
     def config(self):
         """Access the configuration for the population.
 
-        This configuration is extended with
+        This configuration is extended with:
+
         * 'components' of the circuit config
         * 'edges_file': the path the h5 file containing the population.
         """
         return self._circuit.get_edge_population_config(self.name)
 
     @property
     def property_names(self):
@@ -150,15 +151,15 @@
         """Lists the ConstContainer properties shared with the EdgePopulation.
 
         Args:
             container (ConstContainer): a container class for edge properties.
 
         Returns:
             list: A list of strings corresponding to the properties that you can use from the
-                container class
+            container class
 
         Examples:
             >>> from bluepysnap.sonata_constants import Edge
             >>> print(my_edge_population.container_property_names(Edge))
             >>> ["AXONAL_DELAY", "SYN_WEIGHT"] # values you can use with my_edge_population
         """
         if not inspect.isclass(container) or not issubclass(container, ConstContainer):
@@ -240,14 +241,15 @@
 
     def ids(self, group=None, limit=None, sample=None, raise_missing_property=True):
         """Edge IDs corresponding to edges ``edge_ids``.
 
         Args:
             group (None/int/CircuitEdgeId/CircuitEdgeIds/sequence): Which IDs will be
                 returned depends on the type of the ``group`` argument:
+
                 - ``None``: return all IDs.
                 - ``int``, ``CircuitEdgeId``: return a single edge ID.
                 - ``CircuitEdgeIds`` return IDs of edges the edge population in an array.
                 - ``sequence``: return IDs of edges in an array.
 
             sample (int): If specified, randomly choose ``sample`` number of
                 IDs from the match result. If the size of the sample is greater than
@@ -295,16 +297,16 @@
 
         Args:
             edge_ids (array-like): array-like of edge IDs
             properties (str/list): an edge property name or a list of edge property names
 
         Returns:
             pandas.Series/pandas.DataFrame:
-                A pandas Series indexed by edge IDs if ``properties`` is scalar.
-                A pandas DataFrame indexed by edge IDs if ``properties`` is list.
+                - A pandas Series indexed by edge IDs if ``properties`` is scalar.
+                - A pandas DataFrame indexed by edge IDs if ``properties`` is list.
 
         Notes:
             The EdgePopulation.property_names function will give you all the usable properties
             for the `properties` argument.
         """
         edge_ids = self.ids(edge_ids)
         selection = libsonata.Selection(edge_ids)
@@ -390,17 +392,17 @@
 
         Args:
             source (CircuitNodeIds/int/sequence/str/mapping/None): source node group
             target (CircuitNodeIds/int/sequence/str/mapping/None): target node group
             properties: None / edge property name / list of edge property names
 
         Returns:
-            List of edge IDs, if ``properties`` is None;
-            Pandas Series indexed by edge IDs if ``properties`` is string;
-            Pandas DataFrame indexed by edge IDs if ``properties`` is list.
+            - List of edge IDs, if ``properties`` is None;
+            - Pandas Series indexed by edge IDs if ``properties`` is string;
+            - Pandas DataFrame indexed by edge IDs if ``properties`` is list.
         """
         if source is None and target is None:
             raise BluepySnapError("Either `source` or `target` should be specified")
 
         source_node_ids = self._resolve_node_ids(self.source, source)
         target_edge_ids = self._resolve_node_ids(self.target, target)
 
@@ -420,46 +422,46 @@
 
         Args:
             node_id (CircuitNodeIds/int/sequence/str/mapping/None) : Target node ID.
             properties: An edge property name, a list of edge property names, or None.
 
         Returns:
             pandas.Series/pandas.DataFrame/list:
-                A pandas Series indexed by edge ID if ``properties`` is a string.
-                A pandas DataFrame indexed by edge ID if ``properties`` is a list.
-                A list of edge IDs, if ``properties`` is None.
+                - A pandas Series indexed by edge ID if ``properties`` is a string.
+                - A pandas DataFrame indexed by edge ID if ``properties`` is a list.
+                - A list of edge IDs, if ``properties`` is None.
         """
         return self.pathway_edges(source=None, target=node_id, properties=properties)
 
     def efferent_edges(self, node_id, properties=None):
         """Get efferent edges for given ``node_id``.
 
         Args:
             node_id (CircuitNodeIds/int/sequence/str/mapping/None): source node ID
             properties: None / edge property name / list of edge property names
 
         Returns:
-            List of edge IDs, if ``properties`` is None;
-            Pandas Series indexed by edge IDs if ``properties`` is string;
-            Pandas DataFrame indexed by edge IDs if ``properties`` is list.
+            - List of edge IDs, if ``properties`` is None;
+            - Pandas Series indexed by edge IDs if ``properties`` is string;
+            - Pandas DataFrame indexed by edge IDs if ``properties`` is list.
         """
         return self.pathway_edges(source=node_id, target=None, properties=properties)
 
     def pair_edges(self, source_node_id, target_node_id, properties=None):
         """Get edges corresponding to ``source_node_id`` -> ``target_node_id`` connection.
 
         Args:
             source_node_id (CircuitNodeIds/int/sequence/str/mapping/None): source node ID
             target_node_id (CircuitNodeIds/int/sequence/str/mapping/None): target node ID
             properties: None / edge property name / list of edge property names
 
         Returns:
-            List of edge IDs, if ``properties`` is None;
-            Pandas Series indexed by edge IDs if ``properties`` is string;
-            Pandas DataFrame indexed by edge IDs if ``properties`` is list.
+            - List of edge IDs, if ``properties`` is None;
+            - Pandas Series indexed by edge IDs if ``properties`` is string;
+            - Pandas DataFrame indexed by edge IDs if ``properties`` is list.
         """
         return self.pathway_edges(
             source=source_node_id, target=target_node_id, properties=properties
         )
 
     def _iter_connections(self, source_node_ids, target_node_ids, unique_node_ids, shuffle):
         """Iterate through `source_node_ids` -> `target_node_ids` connections."""
@@ -550,17 +552,17 @@
             shuffle: if True, result order would be (somewhat) randomized
             return_edge_count: if True, edge count is added to yield result
             return_edge_ids: if True, edge ID list is added to yield result
 
         ``return_edge_count`` and ``return_edge_ids`` are mutually exclusive.
 
         Yields:
-            (source_node_id, target_node_id, edge_ids) if return_edge_ids == True;
-            (source_node_id, target_node_id, edge_count) if return_edge_count == True;
-            (source_node_id, target_node_id) otherwise.
+            - (source_node_id, target_node_id, edge_ids) if ``return_edge_ids`` is True;
+            - (source_node_id, target_node_id, edge_count) if ``return_edge_count`` is True;
+            - (source_node_id, target_node_id) otherwise.
         """
         if return_edge_ids and return_edge_count:
             raise BluepySnapError(
                 "`return_edge_count` and `return_edge_ids` are mutually exclusive"
             )
 
         source_node_ids = self._resolve_node_ids(self.source, source)
```

### Comparing `bluepysnap-1.0.6/bluepysnap/edges/edges.py` & `bluepysnap-1.0.7/bluepysnap/edges/edges.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,33 +47,34 @@
         return sorted(self._circuit.to_libsonata.edge_populations)
 
     def ids(self, group=None, sample=None, limit=None):
         """Edge CircuitEdgeIds corresponding to edges ``edge_ids``.
 
         Args:
             group (None/int/CircuitEdgeId/CircuitEdgeIds/sequence): Which IDs will be
-            returned depends on the type of the ``group`` argument:
+                returned depends on the type of the ``group`` argument:
+
                 - ``None``: return all CircuitEdgeIds.
                 - ``CircuitEdgeId``: return the ID in a CircuitEdgeIds object.
                 - ``CircuitEdgeIds``: return the IDs in a CircuitNodeIds object.
                 - ``int``: returns a CircuitEdgeIds object containing the corresponding edge ID
-                    for all populations.
+                  for all populations.
                 - ``sequence``: returns a CircuitEdgeIds object containing the corresponding edge
-                    IDs for all populations.
+                  IDs for all populations.
             sample (int): If specified, randomly choose ``sample`` number of
                 IDs from the match result. If the size of the sample is greater than
                 the size of all the EdgePopulations then all ids are taken and shuffled.
             limit (int): If specified, return the first ``limit`` number of
                 IDs from the match result. If limit is greater than the size of all the populations
                 all node IDs are returned.
 
         Returns:
             CircuitEdgeIds: returns a CircuitEdgeIds containing all the edge IDs and the
-                corresponding populations. For performance reasons we do not test if the edge ids
-                are present or not in the circuit.
+            corresponding populations. For performance reasons we do not test if the edge ids
+            are present or not in the circuit.
 
         Notes:
             This envision also the maybe future selection of edges on queries.
         """
         if isinstance(group, CircuitEdgeIds):
             diff = np.setdiff1d(group.get_populations(unique=True), self.population_names)
             if diff.size != 0:
@@ -87,16 +88,16 @@
         Args:
             edge_ids (int/CircuitEdgeId/CircuitEdgeIds/sequence): same as Edges.ids().
             properties (None/str/list): an edge property name or a list of edge property names.
                 If set to None ids are returned.
 
         Returns:
             pandas.Series/pandas.DataFrame:
-                A pandas Series indexed by edge IDs if ``properties`` is scalar.
-                A pandas DataFrame indexed by edge IDs if ``properties`` is list.
+                - A pandas Series indexed by edge IDs if ``properties`` is scalar.
+                - A pandas DataFrame indexed by edge IDs if ``properties`` is list.
 
         Notes:
             The Edges.property_names function will give you all the usable properties
             for the `properties` argument.
         """
         if edge_ids is None:
             raise BluepySnapError("You need to set edge_ids in get.")
@@ -167,17 +168,17 @@
 
         Args:
             source: source node group
             target: target node group
             properties: None / edge property name / list of edge property names
 
         Returns:
-            CircuitEdgeIDs, if ``properties`` is None;
-            Pandas Series indexed by CircuitEdgeIDs if ``properties`` is string;
-            Pandas DataFrame indexed by CircuitEdgeIDs if ``properties`` is list.
+            - CircuitEdgeIDs, if ``properties`` is None;
+            - Pandas Series indexed by CircuitEdgeIDs if ``properties`` is string;
+            - Pandas DataFrame indexed by CircuitEdgeIDs if ``properties`` is list.
         """
         if source is None and target is None:
             raise BluepySnapError("Either `source` or `target` should be specified")
 
         source_ids = self._circuit.nodes.ids(source)
         target_ids = self._circuit.nodes.ids(target)
 
@@ -194,46 +195,46 @@
 
         Args:
             node_id (int): Target node ID.
             properties: An edge property name, a list of edge property names, or None.
 
         Returns:
             pandas.Series/pandas.DataFrame/list:
-                A pandas Series indexed by edge ID if ``properties`` is a string.
-                A pandas DataFrame indexed by edge ID if ``properties`` is a list.
-                A list of edge IDs, if ``properties`` is None.
+                - A pandas Series indexed by edge ID if ``properties`` is a string.
+                - A pandas DataFrame indexed by edge ID if ``properties`` is a list.
+                - A list of edge IDs, if ``properties`` is None.
         """
         return self.pathway_edges(source=None, target=node_id, properties=properties)
 
     def efferent_edges(self, node_id, properties=None):
         """Get efferent edges for given ``node_id``.
 
         Args:
             node_id: source node ID
             properties: None / edge property name / list of edge property names
 
         Returns:
-            List of edge IDs, if ``properties`` is None;
-            Pandas Series indexed by edge IDs if ``properties`` is string;
-            Pandas DataFrame indexed by edge IDs if ``properties`` is list.
+            - List of edge IDs, if ``properties`` is None;
+            - Pandas Series indexed by edge IDs if ``properties`` is string;
+            - Pandas DataFrame indexed by edge IDs if ``properties`` is list.
         """
         return self.pathway_edges(source=node_id, target=None, properties=properties)
 
     def pair_edges(self, source_node_id, target_node_id, properties=None):
         """Get edges corresponding to ``source_node_id`` -> ``target_node_id`` connection.
 
         Args:
             source_node_id: source node ID
             target_node_id: target node ID
             properties: None / edge property name / list of edge property names
 
         Returns:
-            List of edge IDs, if ``properties`` is None;
-            Pandas Series indexed by edge IDs if ``properties`` is string;
-            Pandas DataFrame indexed by edge IDs if ``properties`` is list.
+            - List of edge IDs, if ``properties`` is None;
+            - Pandas Series indexed by edge IDs if ``properties`` is string;
+            - Pandas DataFrame indexed by edge IDs if ``properties`` is list.
         """
         return self.pathway_edges(
             source=source_node_id, target=target_node_id, properties=properties
         )
 
     @staticmethod
     def _add_circuit_ids(its, source, target):
@@ -278,17 +279,17 @@
             target (CircuitNodeIds/int/sequence/str/mapping/None): target node group
             return_edge_count: if True, edge count is added to yield result
             return_edge_ids: if True, edge ID list is added to yield result
 
         ``return_edge_count`` and ``return_edge_ids`` are mutually exclusive.
 
         Yields:
-            (source_node_id, target_node_id, edge_ids) if return_edge_ids == True;
-            (source_node_id, target_node_id, edge_count) if return_edge_count == True;
-            (source_node_id, target_node_id) otherwise.
+            - (source_node_id, target_node_id, edge_ids) if ``return_edge_ids`` is True;
+            - (source_node_id, target_node_id, edge_count) if ``return_edge_count`` is True;
+            - (source_node_id, target_node_id) otherwise.
         """
         if return_edge_ids and return_edge_count:
             raise BluepySnapError(
                 "`return_edge_count` and `return_edge_ids` are mutually exclusive"
             )
         for name, pop in self.items():
             it = pop.iter_connections(
```

### Comparing `bluepysnap-1.0.6/bluepysnap/exceptions.py` & `bluepysnap-1.0.7/bluepysnap/exceptions.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/frame_report.py` & `bluepysnap-1.0.7/bluepysnap/frame_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import numpy as np
 import pandas as pd
 from cached_property import cached_property
 from libsonata import ElementReportReader, SonataError
 
 import bluepysnap._plotting
 from bluepysnap.exceptions import BluepySnapError
-from bluepysnap.utils import ensure_ids, ensure_list
+from bluepysnap.utils import ensure_ids
 
 L = logging.getLogger(__name__)
 
 
 def _collect_population_reports(frame_report, cls):
     return {
         population: cls(frame_report, population) for population in frame_report.population_names
@@ -100,17 +100,14 @@
         try:
             view = self._frame_population.get(
                 node_ids=ids, tstart=t_start, tstop=t_stop, tstride=t_stride
             )
         except SonataError as e:
             raise BluepySnapError(e) from e
 
-        if len(view.ids) == 0:
-            return pd.DataFrame()
-
         # cell ids and section ids in the columns are enforced to be int64
         # to avoid issues with numpy automatic conversions and to ensure that
         # the results are the same regardless of the libsonata version [NSETM-1766]
         res = pd.DataFrame(
             data=view.data,
             columns=pd.MultiIndex.from_arrays(ensure_ids(view.ids).T),
             index=view.times,
@@ -155,33 +152,31 @@
 
     @cached_property
     def report(self):
         """Access to the report data.
 
         Returns:
             pandas.DataFrame: A DataFrame containing the data from the report. Row's indices are the
-                different timestamps and the column's MultiIndex are :
-                - (population_name, node_id, compartment id) for the CompartmentReport
-                - (population_name, node_id) for the SomaReport
+            different timestamps and the column's MultiIndex are:
+
+            - (population_name, node_id, compartment id) for the CompartmentReport
+            - (population_name, node_id) for the SomaReport
         """
-        res = pd.DataFrame()
+        dataframes = {}
         for population in self.frame_report.population_names:
             frames = self.frame_report[population]
-            try:
-                ids = frames.nodes.ids(group=self.group)
-            except BluepySnapError:
-                continue
-            data = frames.get(group=ids, t_start=self.t_start, t_stop=self.t_stop)
-            if data.empty:
-                continue
-            new_index = tuple(tuple([population] + ensure_list(x)) for x in data.columns)
-            data.columns = pd.MultiIndex.from_tuples(new_index)
-            # need to do this in order to preserve MultiIndex for columns
-            res = data if res.empty else data.join(res, how="outer")
-        return res.sort_index().sort_index(axis=1)
+            ids = frames.nodes.ids(group=self.group, raise_missing_property=False)
+            df = frames.get(group=ids, t_start=self.t_start, t_stop=self.t_stop)
+            dataframes[population] = df
+        # optimize when there is at most one non-empty df: use copy=False, and no need to sort
+        if sum(not df.empty for df in dataframes.values()) <= 1:
+            return pd.concat(dataframes, axis=1, copy=False)
+        # when concatenating multiple df, don't use copy=False because 2x slower (Pandas 2.0.2)
+        result = pd.concat(dataframes, axis=1)
+        return result.sort_index(axis=0).sort_index(axis=1)
 
     # pylint: disable=protected-access
     trace = bluepysnap._plotting.frame_trace
 
 
 class FrameReport:
     """Access to FrameReport data."""
```

### Comparing `bluepysnap-1.0.6/bluepysnap/morph.py` & `bluepysnap-1.0.7/bluepysnap/morph.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/network.py` & `bluepysnap-1.0.7/bluepysnap/network.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/neuron_models.py` & `bluepysnap-1.0.7/bluepysnap/neuron_models.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/node_sets.py` & `bluepysnap-1.0.7/bluepysnap/node_sets.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/nodes/node_population.py` & `bluepysnap-1.0.7/bluepysnap/nodes/node_population.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,16 @@
             edge.name for edge in self._circuit.edges.values() if self.name == edge.target.name
         )
 
     @property
     def config(self):
         """Access the configuration for the population.
 
-        This configuration is extended with
+        This configuration is extended with:
+
         * 'components' of the circuit config
         * 'nodes_file': the path the h5 file containing the population.
         """
         return self._circuit.get_node_population_config(self.name)
 
     @property
     def property_names(self):
@@ -269,15 +270,15 @@
         """Lists the ConstContainer properties shared with the NodePopulation.
 
         Args:
             container (ConstContainer): a container class for node properties.
 
         Returns:
             list: A list of strings corresponding to the properties that you can use from the
-                container class
+            container class
 
         Examples:
             >>> from bluepysnap.sonata_constants import Node
             >>> print(my_node_population.container_property_names(Node))
             >>> ["X", "Y", "Z"] # values from Node that you can use with my_node_population
             >>> my_node_population.property_values(Node.X)
             >>> my_node_population.property_values(Node.get("X"))
```

### Comparing `bluepysnap-1.0.6/bluepysnap/nodes/nodes.py` & `bluepysnap-1.0.7/bluepysnap/nodes/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,40 +55,41 @@
         )
 
     def ids(self, group=None, sample=None, limit=None):
         """Returns the CircuitNodeIds corresponding to the nodes from ``group``.
 
         Args:
             group (CircuitNodeId/CircuitNodeIds/int/sequence/str/mapping/None): Which IDs will be
-            returned depends on the type of the ``group`` argument:
+                returned depends on the type of the ``group`` argument:
+
                 - ``CircuitNodeId``: return the ID in a CircuitNodeIds object if it belongs to
-                    the circuit.
+                  the circuit.
                 - ``CircuitNodeIds``: return the IDs in a CircuitNodeIds object if they belong to
-                    the circuit.
+                  the circuit.
                 - ``int``: if the node ID is present in all populations, returns a CircuitNodeIds
-                    object containing the corresponding node ID for all populations.
+                  object containing the corresponding node ID for all populations.
                 - ``sequence``: if all the values contained in the sequence are present in all
-                    populations, returns a CircuitNodeIds object containing the corresponding node
-                    IDs for all populations.
+                  populations, returns a CircuitNodeIds object containing the corresponding node
+                  IDs for all populations.
                 - ``str``: use a node set name as input. Returns a CircuitNodeIds object containing
-                    nodes selected by the node set.
+                  nodes selected by the node set.
                 - ``mapping``: Returns a CircuitNodeIds object containing nodes matching a
-                    properties filter.
+                  properties filter.
                 - ``None``: return all node IDs of the circuit in a CircuitNodeIds object.
             sample (int): If specified, randomly choose ``sample`` number of
                 IDs from the match result. If the size of the sample is greater than
                 the size of all the NodePopulations then all ids are taken and shuffled.
             limit (int): If specified, return the first ``limit`` number of
                 IDs from the match result. If limit is greater than the size of all the populations,
                 all node IDs are returned.
 
         Returns:
             CircuitNodeIds: returns a CircuitNodeIds containing all the node IDs and the
-                corresponding populations. All the explicitly requested IDs must be present inside
-                the circuit.
+            corresponding populations. All the explicitly requested IDs must be present inside
+            the circuit.
 
         Raises:
             BluepySnapError: when a population from a CircuitNodeIds is not present in the circuit.
             BluepySnapError: when an id query via a int, sequence, or CircuitNodeIds is not present
                 in the circuit.
 
         Examples:
```

### Comparing `bluepysnap-1.0.6/bluepysnap/query.py` & `bluepysnap-1.0.7/bluepysnap/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Module to process search queries of nodes/edges."""
+import operator
 from collections.abc import Mapping
 from copy import deepcopy
+from functools import reduce
 
 import numpy as np
 
 from bluepysnap import utils
 from bluepysnap.exceptions import BluepySnapError
 
 # this constant is not part of the sonata standard
@@ -15,20 +17,65 @@
 AND_KEY = "$and"
 REGEX_KEY = "$regex"
 NODE_SET_KEY = "$node_set"
 VALUE_KEYS = {REGEX_KEY}
 ALL_KEYS = {NODE_ID_KEY, EDGE_ID_KEY, POPULATION_KEY, OR_KEY, AND_KEY, NODE_SET_KEY} | VALUE_KEYS
 
 
-# TODO: move to `libsonata` library
+def _logical_and(masks):
+    """Calculate and return the "logical and" of the given masks.
+
+    Args:
+        masks: list of array-like, or booleans.
+
+    Returns:
+        the resulting mask as a numpy array, or a bool.
+        Return True if the masks list is empty, similarly to all([]).
+    """
+    filtered_masks = []
+    for mask in masks:
+        if mask is False:
+            return False
+        if mask is True:
+            continue
+        filtered_masks.append(mask)
+    if not filtered_masks:
+        return True
+    # reduce(operator.and_, masks) is faster than np.logical_and.reduce() or np.all()
+    return reduce(operator.and_, (np.asarray(m, dtype=bool) for m in filtered_masks))
+
+
+def _logical_or(masks):
+    """Calculate and return the "logical or" of the given masks.
+
+    Args:
+        masks: list of array-like, or booleans.
+
+    Returns:
+        the resulting mask as a numpy array, or a bool.
+        Return False if the masks list is empty, similarly to any([]).
+    """
+    filtered_masks = []
+    for mask in masks:
+        if mask is True:
+            return True
+        if mask is False:
+            continue
+        filtered_masks.append(mask)
+    if not filtered_masks:
+        return False
+    # reduce(operator.or_, masks) is faster than np.logical_or.reduce() or np.any()
+    return reduce(operator.or_, (np.asarray(m, dtype=bool) for m in filtered_masks))
+
+
 def _complex_query(prop, query):
-    result = np.full(len(prop), True)
+    result = True
     for key, value in query.items():
         if key == REGEX_KEY:
-            result = np.logical_and(result, prop.str.match(value + "\\Z"))
+            result = _logical_and([result, prop.str.match(value + r"\Z")])
         else:
             raise BluepySnapError(f"Unknown query modifier: '{key}'")
     return result
 
 
 def _positional_mask(data, ids):
     """Positional mask for the node IDs.
@@ -37,15 +84,15 @@
         ids (None/numpy.ndarray): the ids array. If None all ids are selected.
 
     Examples:
         if the data set contains 5 nodes:
         _positional_mask(data, [0,2]) --> [True, False, True, False, False]
     """
     if ids is None:
-        return np.full(len(data), fill_value=True)
+        return True
     if isinstance(ids, int):
         ids = [ids]
     mask = np.full(len(data), fill_value=False)
     indices = data.index.get_indexer(ids)
     mask[indices[indices > -1]] = True
     return mask
 
@@ -60,31 +107,33 @@
     return queries, _positional_mask(data, ids)
 
 
 def _properties_mask(data, population_name, queries):
     """Return mask of IDs matching `props` dict."""
     unknown_props = set(queries) - set(data.columns) - ALL_KEYS
     if unknown_props:
-        return np.full(len(data), fill_value=False)
+        return False
 
     queries, mask = _circuit_mask(data, population_name, queries)
-    if not mask.any():
+    if mask is False or isinstance(mask, np.ndarray) and not mask.any():
         # Avoid fail and/or processing time if wrong population or no nodes
-        return mask
+        return False
 
     for prop, values in queries.items():
         prop = data[prop]
         if np.issubdtype(prop.dtype.type, np.floating):
             v1, v2 = values
             prop_mask = np.logical_and(prop >= v1, prop <= v2)
         elif isinstance(values, Mapping):
             prop_mask = _complex_query(prop, values)
+        elif isinstance(values, list):
+            prop_mask = prop.isin(values)
         else:
-            prop_mask = np.in1d(prop, values)
-        mask = np.logical_and(mask, prop_mask)
+            prop_mask = prop == values
+        mask = _logical_and([mask, prop_mask])
     return mask
 
 
 def traverse_queries_bottom_up(queries, traverse_fn):
     """Traverse queries tree from leaves to root, left to right.
 
     Args:
@@ -132,29 +181,28 @@
         queries (dict): queries
 
     Returns:
         np.array: index mask
     """
 
     def _merge_queries_masks(queries):
-        if len(queries) == 0:
-            return np.full(len(data), True)
-        return np.logical_and.reduce(list(queries.values()))
+        return _logical_and(queries.values())
 
     def _collect(queries, queries_key):
         # each queries value is replaced with a bit mask of corresponding ids
         if queries_key == OR_KEY:
             # children are already resolved masks due to traverse order
             children_mask = [_merge_queries_masks(query) for query in queries[queries_key]]
-            queries[queries_key] = np.logical_or.reduce(children_mask)
+            queries[queries_key] = _logical_or(children_mask)
         elif queries_key == AND_KEY:
             # children are already resolved masks due to traverse order
             children_mask = [_merge_queries_masks(query) for query in queries[queries_key]]
-            queries[queries_key] = np.logical_and.reduce(children_mask)
+            queries[queries_key] = _logical_and(children_mask)
         else:
             queries[queries_key] = _properties_mask(
                 data, population_name, {queries_key: queries[queries_key]}
             )
 
     queries = deepcopy(queries)
     traverse_queries_bottom_up(queries, _collect)
-    return _merge_queries_masks(queries)
+    result = _merge_queries_masks(queries)
+    return np.full(len(data), fill_value=result) if isinstance(result, bool) else result
```

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/circuit.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/circuit.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/definitions/datatypes.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/definitions/datatypes.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/definitions/edge.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/definitions/edge.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/definitions/node.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/definitions/node.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/chemical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical_virtual.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/chemical_virtual.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/electrical.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/electrical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/endfoot.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/endfoot.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/glialglial.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/glialglial.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/edge/synapse_astrocyte.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/edge/synapse_astrocyte.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/node/biophysical.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/node/biophysical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/node/vasculature.yaml` & `bluepysnap-1.0.7/bluepysnap/schemas/node/vasculature.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/schemas/schemas.py` & `bluepysnap-1.0.7/bluepysnap/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/settings.py` & `bluepysnap-1.0.7/bluepysnap/settings.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/simulation.py` & `bluepysnap-1.0.7/bluepysnap/simulation.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/sonata_constants.py` & `bluepysnap-1.0.7/bluepysnap/sonata_constants.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap/spike_report.py` & `bluepysnap-1.0.7/bluepysnap/spike_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     @cached_property
     def report(self):
         """Access to the report data.
 
         Returns:
             pandas.DataFrame: A DataFrame containing the data from the report. Row's indices are the
-                different timestamps and the columns are ids and population names.
+            different timestamps and the columns are ids and population names.
         """
         res = pd.DataFrame()
         for population in self.spike_report.population_names:
             spikes = self.spike_report[population]
             try:
                 ids = spikes.nodes.ids(group=self.group)
             except BluepySnapError:
```

### Comparing `bluepysnap-1.0.6/bluepysnap/utils.py` & `bluepysnap-1.0.7/bluepysnap/utils.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/bluepysnap.egg-info/PKG-INFO` & `bluepysnap-1.0.7/bluepysnap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepysnap
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simulation and Neural network Analysis Productivity layer
 Home-page: https://github.com/BlueBrain/snap
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Keywords: SONATA,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Provides-Extra: spatial-index
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS.txt
 
 |banner|
 
-|build_status| |license| |coverage| |docs|
+|build_status| |license| |coverage| |docs| |DOI|
 
 Blue Brain SNAP
 ===============
 
 Blue Brain Simulation and Neural network Analysis Productivity layer (Blue Brain SNAP).
 
 Blue Brain SNAP is a Python library for accessing BlueBrain circuit models represented in
@@ -127,26 +127,30 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-.. |build_status| image:: https://travis-ci.com/BlueBrain/snap.svg?branch=master
-   :target: https://travis-ci.com/BlueBrain/snap
+.. |build_status| image:: https://github.com/BlueBrain/snap/actions/workflows/run-tox.yml/badge.svg
    :alt: Build Status
 
 .. |license| image:: https://img.shields.io/pypi/l/bluepysnap
-                :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :target: https://github.com/BlueBrain/snap/blob/master/COPYING.LESSER
+   :alt: License
 
 .. |coverage| image:: https://codecov.io/github/BlueBrain/snap/coverage.svg?branch=master
    :target: https://codecov.io/github/BlueBrain/snap?branch=master
    :alt: codecov.io
 
 .. |docs| image:: https://readthedocs.org/projects/bluebrainsnap/badge/?version=latest
-             :target: https://bluebrainsnap.readthedocs.io/
-             :alt: documentation status
+   :target: https://bluebrainsnap.readthedocs.io/
+   :alt: documentation status
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8026852.svg
+   :target: https://doi.org/10.5281/zenodo.8026852
+   :alt: DOI
 
 .. substitutions
 .. |banner| image:: doc/source/_images/BlueBrainSNAP.jpg
 .. |circuit| replace:: **Circuit**
 .. |simulation| replace:: **Simulation**
```

### Comparing `bluepysnap-1.0.6/bluepysnap.egg-info/SOURCES.txt` & `bluepysnap-1.0.7/bluepysnap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/pyproject.toml` & `bluepysnap-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.6/setup.py` & `bluepysnap-1.0.7/setup.py`

 * *Files identical despite different names*

