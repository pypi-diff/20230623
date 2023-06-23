# Comparing `tmp/optimum-neuron-0.0.4.tar.gz` & `tmp/optimum-neuron-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.4.tar", last modified: Mon May  8 22:42:52 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.5.tar", last modified: Fri Jun 23 16:06:47 2023, max compression
```

## Comparing `optimum-neuron-0.0.4.tar` & `optimum-neuron-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,84 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.4/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.4/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     4906 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4648 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1141 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2971 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/optimum/commands/neuron/cache.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/register/register_export.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5035 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-26 13:29:33.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12081 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-26 13:29:33.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/model_configs.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.4/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-24 14:58:35.000000 optimum-neuron-0.0.4/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-05-08 22:41:10.000000 optimum-neuron-0.0.4/optimum/neuron/trainers.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5163 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    20411 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.4/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-05-08 22:41:25.000000 optimum-neuron-0.0.4/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1303 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      362 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-05-08 22:42:52.877747 optimum-neuron-0.0.4/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2776 2023-05-08 22:41:25.000000 optimum-neuron-0.0.4/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    25748 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27159 2023-05-02 15:09:11.000000 optimum-neuron-0.0.4/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.4/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.5/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.5/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4927 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/commands/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/commands/neuron/cache.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.5/optimum/commands/register/register_export.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.5/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5317 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11086 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12824 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4092 2023-05-30 08:48:22.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/model_configs.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2431 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/accelerate/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      732 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12887 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/accelerator.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2330 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/optimizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/scheduler.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15103 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/state.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      764 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6605 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/dataclasses.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/misc.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/distributed/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7136 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3797 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/encoder_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2172 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/parallelizers_manager.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2324 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.5/optimum/neuron/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18203 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/modeling_base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12800 2023-06-08 09:55:27.000000 optimum-neuron-0.0.5/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    15201 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8564 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/training_args.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5967 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    29996 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/constant.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/misc.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6684 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/patching.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-06-23 15:38:20.000000 optimum-neuron-0.0.5/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-06-23 15:59:16.000000 optimum-neuron-0.0.5/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    34743 2023-06-13 15:28:53.000000 optimum-neuron-0.0.5/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/tests/test_compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_generate.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    45311 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.5/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.4/LICENSE` & `optimum-neuron-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/MANIFEST.in` & `optimum-neuron-0.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/PKG-INFO` & `optimum-neuron-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -108,15 +108,15 @@
     tokenizer=tokenizer,
     data_collator=data_collator,
 )
 ```
 
 ### Documentation
 
-Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum/**neuron**/index) for more advanced usage.
+Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum-neuron/index) for more advanced usage.
 
 <!---
 
 ## Validated Models
 
 The following model architectures, tasks and device distributions have been validated for 🤗 Optimum Neuron:
```

### Comparing `optimum-neuron-0.0.4/README.md` & `optimum-neuron-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     tokenizer=tokenizer,
     data_collator=data_collator,
 )
 ```
 
 ### Documentation
 
-Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum/**neuron**/index) for more advanced usage.
+Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum-neuron/index) for more advanced usage.
 
 <!---
 
 ## Validated Models
 
 The following model architectures, tasks and device distributions have been validated for 🤗 Optimum Neuron:
```

### Comparing `optimum-neuron-0.0.4/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.5/optimum/commands/export/neuron.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,33 +73,40 @@
         help='The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"`, `"mixed"` or `"tf32"`.',
     )
     optional_group.add_argument(
         "--disable-fast-relayout",
         action="store_true",
         help="Whether to disable fast relayout optimization which improves performance by using the matrix multiplier for tensor transpose.",
     )
+    optional_group.add_argument(
+        "--disable-fallback",
+        action="store_true",
+        help="Whether to disable CPU partitioning to force operations to Neuron. Defaults to `False`, as without fallback, there could be some compilation failures or performance problems.",
+    )
+    optional_group.add_argument(
+        "--dynamic-batch-size",
+        action="store_true",
+        help="Enable dynamic batch size for neuron compiled model. If this option is enabled, the input batch size can be dynamic during the inference, but it comes with a potential tradeoff in terms of latency.",
+    )
 
     input_group = parser.add_argument_group("Input shapes")
     doc_input = "that the Neuron-cc compiler exported model will be able to take as input."
     input_group.add_argument(
         "--batch_size",
         type=int,
-        default=1,
         help=f"Batch size {doc_input}",
     )
     input_group.add_argument(
         "--sequence_length",
         type=int,
-        default=16,
         help=f"Sequence length {doc_input}",
     )
     input_group.add_argument(
         "--num_choices",
         type=int,
-        default=4,
         help=f"Only for the multiple-choice task. Num choices {doc_input}",
     )
 
 
 class NeuronExportCommand(BaseOptimumCLICommand):
     COMMAND = CommandInfo(name="neuron", help="Export PyTorch models to Neuron compiled TorchScript models.")
```

### Comparing `optimum-neuron-0.0.4/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.5/optimum/commands/export/neuronx.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,33 +68,35 @@
     optional_group.add_argument(
         "--auto_cast_type",
         type=str,
         default="bf16",
         choices=["bf16", "fp16", "tf32"],
         help='The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"` or `"tf32"`.',
     )
+    optional_group.add_argument(
+        "--dynamic-batch-size",
+        action="store_true",
+        help="Enable dynamic batch size for neuron compiled model. If this option is enabled, the input batch size can be a multiple of the batch size during the compilation, but it comes with a potential tradeoff in terms of latency.",
+    )
 
     input_group = parser.add_argument_group("Input shapes")
     doc_input = "that the Neuronx-cc compiler exported model will be able to take as input."
     input_group.add_argument(
         "--batch_size",
         type=int,
-        default=1,
         help=f"Batch size {doc_input}",
     )
     input_group.add_argument(
         "--sequence_length",
         type=int,
-        default=16,
         help=f"Sequence length {doc_input}",
     )
     input_group.add_argument(
         "--num_choices",
         type=int,
-        default=4,
         help=f"Only for the multiple-choice task. Num choices {doc_input}",
     )
 
 
 class NeuronxExportCommand(BaseOptimumCLICommand):
     COMMAND = CommandInfo(name="neuron", help="Export PyTorch models to Neuronx compiled TorchScript models.")
```

### Comparing `optimum-neuron-0.0.4/optimum/commands/neuron/base.py` & `optimum-neuron-0.0.5/optimum/commands/neuron/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Defines the root command line class for optimum-neuron."""
 
 from ...utils import logging
 from ..base import BaseOptimumCLICommand, CommandInfo
 from .cache import CustomCacheRepoCommand
```

### Comparing `optimum-neuron-0.0.4/optimum/commands/register/register_export.py` & `optimum-neuron-0.0.5/optimum/commands/register/register_export.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.5/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/__main__.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Entry point to the optimum.exporters.neuron command line."""
 
 import copy
 from argparse import ArgumentParser
 
-from ...neuron.utils import is_neuron_available, is_neuronx_available
+from ...neuron.utils import is_neuron_available, is_neuronx_available, store_compilation_config
 from ...utils import logging
 from ...utils.save_utils import maybe_save_preprocessors
 from ..error_utils import AtolError, OutputMatchError, ShapeError
 from ..tasks import TasksManager
 from .convert import export, validate_model_outputs
 from .model_configs import *  # noqa: F403
 
@@ -67,43 +67,44 @@
     model = TasksManager.get_model_from_task(
         task, args.model, framework="pt", cache_dir=args.cache_dir, trust_remote_code=args.trust_remote_code
     )
     ref_model = copy.deepcopy(model)
 
     neuron_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="neuron", task=task)
     # TODO: find a cleaner way to do this.
-    shapes = {name: getattr(args, name) for name in neuron_config_constructor.func.get_mandatory_axes_for_task(task)}
-    neuron_config = neuron_config_constructor(model.config, **shapes)
+    input_shapes = {
+        name: getattr(args, name) for name in neuron_config_constructor.func.get_mandatory_axes_for_task(task)
+    }
+    if is_neuron_available() and args.dynamic_batch_size is True and "batch_size" in input_shapes:
+        input_shapes["batch_size"] = 1
+    neuron_config = neuron_config_constructor(model.config, dynamic_batch_size=args.dynamic_batch_size, **input_shapes)
 
     if args.atol is None:
         args.atol = neuron_config.ATOL_FOR_VALIDATION
 
     # Get compilation arguments
     auto_cast = None if args.auto_cast == "none" else args.auto_cast
-    auto_cast_type = args.auto_cast_type
-    kwargs = {"auto_cast": auto_cast, "auto_cast_type": auto_cast_type}
+    auto_cast_type = None if auto_cast is None else args.auto_cast_type
+    compiler_kwargs = {"auto_cast": auto_cast, "auto_cast_type": auto_cast_type}
     if hasattr(args, "disable_fast_relayout"):
-        kwargs["disable_fast_relayout"] = getattr(args, "disable_fast_relayout")
+        compiler_kwargs["disable_fast_relayout"] = getattr(args, "disable_fast_relayout")
+    if hasattr(args, "disable_fallback"):
+        compiler_kwargs["disable_fallback"] = getattr(args, "disable_fallback")
 
     neuron_inputs, neuron_outputs = export(
         model=model,
         config=neuron_config,
         output=args.output,
-        **kwargs,
+        **compiler_kwargs,
     )
 
-    # Add input shapes during compilation to the config
-    for axe, shape in shapes.items():
-        axe = f"neuron_{axe}"
-        model.config.__setattr__(axe, shape)
-    # Add compilation args to the config
-    if auto_cast is None:
-        kwargs["auto_cast_type"] = None
-    for arg, value in kwargs.items():
-        model.config.__setattr__(arg, value)
+    # For torch_neuron, batch_size must be equal to 1 when dynamic batching is on.
+    store_compilation_config(
+        model.config, input_shapes, compiler_kwargs, neuron_inputs, neuron_outputs, args.dynamic_batch_size
+    )
 
     # Saving the model config and preprocessor as this is needed sometimes.
     model.config.save_pretrained(args.output.parent)
     maybe_save_preprocessors(args.model, args.output.parent)
 
     # Validate compiled model
     try:
```

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,28 @@
 """Neuron configuration base classes."""
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import torch
 
-from optimum.exporters.base import ExportConfig
+from ...exporters.base import ExportConfig
+from ...neuron.utils import is_neuron_available
+from ...utils import logging
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedModel
 
     from optimum.utils import DummyInputGenerator
 
 
+logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
+
+
 class MissingMandatoryAxisDimension(ValueError):
     pass
 
 
 class NeuronConfig(ExportConfig, ABC):
     """
     Base class for Neuron exportable model describing metadata on how to export the model through the TorchScript format.
@@ -56,14 +61,16 @@
         for the number of possible choices is needed when the task is multiple-choice.
 
     Args:
         config (`transformers.PretrainedConfig`):
             The model configuration.
         task (`str`, defaults to `"feature-extraction"`):
             The task the model should be exported for.
+        dynamic_batch_size (`bool`, defaults to `False`):
+            Whether the Neuron compiled model supports dynamic batch size.
 
         The rest of the arguments are used to specify the shape of the inputs the model can take.
         They are required or not depending on the model the `NeuronConfig` is designed for.
     """
 
     NORMALIZED_CONFIG_CLASS = None
     DUMMY_INPUT_GENERATOR_CLASSES = ()
@@ -88,29 +95,35 @@
         "audio-xvector": ["logits"],
     }
 
     def __init__(
         self,
         config: "PretrainedConfig",
         task: str,
-        batch_size: int = 1,
+        batch_size: Optional[int] = None,
+        dynamic_batch_size: bool = False,
         sequence_length: Optional[int] = None,
         num_choices: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         num_channels: Optional[int] = None,
         feature_size: Optional[int] = None,
         nb_max_frames: Optional[int] = None,
         audio_sequence_length: Optional[int] = None,
     ):
         self._config = config
         self._normalized_config = self.NORMALIZED_CONFIG_CLASS(self._config)
         self.mandatory_axes = ()
         self.task = task
         self._axes: Dict[str, int] = {}
+        self.dynamic_batch_size = dynamic_batch_size
+
+        if self.dynamic_batch_size is True and is_neuron_available():
+            logger.info("Overwriting batch size to 1 for neuron dynamic batch size support.")
+            batch_size = 1
 
         # To avoid using **kwargs.
         axes_values = {
             "batch_size": batch_size,
             "sequence_length": sequence_length,
             "num_choices": num_choices,
             "width": width,
```

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/config.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Neuron TorchScript model check and export functions."""
+"""Neuron compiled model check and export functions."""
 
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Tuple
 
 import numpy as np
 import torch
 
@@ -72,14 +72,16 @@
             atol = config.ATOL_FOR_VALIDATION[config.task]
         else:
             atol = config.ATOL_FOR_VALIDATION
 
     input_shapes = {}
     for axe in config.mandatory_axes:
         input_shapes[axe] = getattr(config, axe)
+    if config.dynamic_batch_size is True:
+        input_shapes["batch_size"] *= 2
     ref_inputs = config.generate_dummy_inputs(return_tuple=False, **input_shapes)
     with torch.no_grad():
         reference_model.eval()
         ref_outputs = reference_model(**ref_inputs)
 
     neuron_inputs = tuple(ref_inputs.values())
     neuron_model = torch.jit.load(neuron_model_path)
@@ -145,34 +147,36 @@
 def export(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
     auto_cast_type: str = "bf16",
     disable_fast_relayout: bool = False,
+    disable_fallback: bool = False,
 ) -> Tuple[List[str], List[str]]:
     if is_neuron_available():
-        return export_neuron(model, config, output, auto_cast, auto_cast_type, disable_fast_relayout)
+        return export_neuron(model, config, output, auto_cast, auto_cast_type, disable_fast_relayout, disable_fallback)
     elif is_neuronx_available():
         return export_neuronx(model, config, output, auto_cast, auto_cast_type)
     else:
         raise RuntimeError(
             "Cannot export the model because the neuron(x) compiler is not installed. See https://awsdocs-neuron.readthedocs-hosted.com/en/latest/frameworks/torch/torch-setup.html."
         )
 
 
 def export_neuronx(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
     auto_cast_type: str = "bf16",
+    dynamic_batch_size: bool = False,
 ) -> Tuple[List[str], List[str]]:
     """
-    Exports a PyTorch model to a Neuronx compiled TorchScript model.
+    Exports a PyTorch model to a serialized TorchScript module compiled by neuronx-cc compiler.
 
     Args:
         model ([`PreTrainedModel`]):
             The model to export.
         config ([`~exporter.NeuronConfig`]):
             The Neuron configuration associated with the exported model.
         output (`Path`):
@@ -215,43 +219,50 @@
 
         logger.info(f"Using Neuron: --auto-cast-type {auto_cast_type}")
         compiler_args.extend(["--auto-cast-type", auto_cast_type])
     else:
         compiler_args = ["--auto-cast", "none"]
 
     neuron_model = neuronx.trace(checked_model, dummy_inputs_tuple, compiler_args=compiler_args)
+
+    if config.dynamic_batch_size is True:
+        neuron_model = neuronx.dynamic_batch(neuron_model)
+
     torch.jit.save(neuron_model, output)
 
     return config.inputs, config.outputs
 
 
 def export_neuron(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
     auto_cast_type: str = "bf16",
     disable_fast_relayout: bool = False,
+    disable_fallback: bool = False,
 ) -> Tuple[List[str], List[str]]:
     """
-    Exports a PyTorch model to a Neuron compiled TorchScript model.
+    Exports a PyTorch model to a serialized TorchScript module compiled by neuron-cc compiler.
 
     Args:
         model ([`PreTrainedModel`]):
             The model to export.
         config ([`~exporter.NeuronConfig`]):
             The Neuron configuration associated with the exported model.
         output (`Path`):
             Directory to store the exported Neuron model.
         auto_cast (`Optional[str]`, defaults to `None`):
             Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `None`, `"matmul"` or `"all"`, you should use `None` to disable any auto-casting, use `"matmul"` to cast FP32 matrix multiplication operations, and use `"all"` to cast all FP32 operations.
         auto_cast_type (`str`, defaults to `"bf16"`):
             The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"`, ``"mixed" or `"tf32"`. `"mixed"` is only available when auto_cast is "matmul", it will cast operators that use Neuron Matmult engine to bf16 while using fp16 for matmult-based transpose.
         disable_fast_relayout (`bool`, defaults to `False`):
             Whether to disable fast relayout optimization which improves performance by using the matrix multiplier for tensor transpose.
+        disable_fallback (`bool`, defaults to `False`):
+            Whether to disable CPU partitioning to force operations to Neuron. Defaults to `False`, as without fallback, there could be some compilation failures or performance problems.
 
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named inputs from
         the Neuron configuration.
     """
     output.parent.mkdir(parents=True, exist_ok=True)
 
@@ -270,11 +281,18 @@
     for axe in config.mandatory_axes:
         input_shapes[axe] = getattr(config, axe)
 
     dummy_inputs = config.generate_dummy_inputs(**input_shapes)
     dummy_inputs_tuple = tuple(dummy_inputs.values())
     checked_model = config.check_model_inputs_order(model, dummy_inputs)
     compiler_args = convert_neuronx_compiler_args_to_neuron(auto_cast, auto_cast_type, disable_fast_relayout)
-    neuron_model = neuron.trace(checked_model, dummy_inputs_tuple, compiler_args=compiler_args)
-    neuron_model.save(output)
+
+    neuron_model = neuron.trace(
+        checked_model,
+        dummy_inputs_tuple,
+        dynamic_batch_size=config.dynamic_batch_size,
+        compiler_args=compiler_args,
+        fallback=not disable_fallback,
+    )
+    torch.jit.save(neuron_model, output)
 
     return config.inputs, config.outputs
```

### Comparing `optimum-neuron-0.0.4/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.5/optimum/exporters/neuron/model_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,47 +44,45 @@
 
 
 @register_in_tasks_manager("albert", *COMMON_TEXT_TASKS)
 class AlbertNeuronConfig(BertNeuronConfig):
     pass
 
 
-# Issue: https://github.com/aws-neuron/aws-neuron-sdk/issues/641
-# (will be fixed by the next neuron sdk release)
-# @register_in_tasks_manager("convbert", *COMMON_TEXT_TASKS)
-# class ConvBertNeuronConfig(BertNeuronConfig):
-#     pass
-
-
-@register_in_tasks_manager("electra", *COMMON_TEXT_TASKS)
-class ElectraNeuronConfig(BertNeuronConfig):
+@register_in_tasks_manager("convbert", *COMMON_TEXT_TASKS)
+class ConvBertNeuronConfig(BertNeuronConfig):
     @property
     def outputs(self) -> List[str]:
         if self.task == "feature-extraction":
             return ["last_hidden_state"]
         return self._TASK_TO_COMMON_OUTPUTS[self.task]
 
 
+@register_in_tasks_manager("electra", *COMMON_TEXT_TASKS)
+class ElectraNeuronConfig(ConvBertNeuronConfig):
+    pass
+
+
 @register_in_tasks_manager("flaubert", *COMMON_TEXT_TASKS)
-class FlaubertNeuronConfig(ElectraNeuronConfig):
+class FlaubertNeuronConfig(ConvBertNeuronConfig):
     pass
 
 
 @register_in_tasks_manager("mobilebert", *COMMON_TEXT_TASKS)
 class MobileBertNeuronConfig(BertNeuronConfig):
     pass
 
 
 @register_in_tasks_manager("roformer", *COMMON_TEXT_TASKS)
-class RoFormerNeuronConfig(ElectraNeuronConfig):
+class RoFormerNeuronConfig(ConvBertNeuronConfig):
     pass
 
 
 @register_in_tasks_manager("xlm", *COMMON_TEXT_TASKS)
-class XLMNeuronConfig(ElectraNeuronConfig):
+class XLMNeuronConfig(ConvBertNeuronConfig):
     pass
 
 
 @register_in_tasks_manager("distilbert", *COMMON_TEXT_TASKS)
 class DistilBertNeuronConfig(BertNeuronConfig):
     ATOL_FOR_VALIDATION = 1e-4
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.5/optimum/neuron/hf_argparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Customizes the HfArgumentParser to add checks for AWS Tranium instances."""
 
 from transformers import HfArgumentParser
 
 from .utils.argument_utils import validate_arg
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.5/optimum/neuron/trainer_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Defines custom Trainer callbacks specific to AWS Trainium instances."""
 
 import inspect
 import json
 import shutil
 import subprocess
 from collections import defaultdict
@@ -84,15 +85,17 @@
             self.tmp_neuron_cache = self.create_temporary_neuron_cache(self.neuron_cache_path)
         else:
             self.tmp_neuron_cache = tmp_neuron_cache
         self.tmp_neuron_cache_path = Path(self.tmp_neuron_cache.name) / NEURON_COMPILE_CACHE_NAME
         self.tmp_neuron_cache_state = list_files_in_neuron_cache(self.tmp_neuron_cache_path, only_relevant_files=True)
         self.fetch_files = set()
 
-        self.neuron_hashes: Dict[Tuple["PreTrainedModel", Tuple[Tuple[int], ...], torch.dtype], NeuronHash] = {}
+        self.neuron_hashes: Dict[
+            Tuple["PreTrainedModel", Tuple[Tuple[str, Tuple[int]], ...], torch.dtype], NeuronHash
+        ] = {}
         self.neuron_hash_to_files: Dict[NeuronHash, List[Path]] = defaultdict(list)
 
     def prepare_state(self, state: TrainerState):
         if isinstance(state, NeuronTrainerState):
             return state
         return NeuronTrainerState.from_trainer_state(state)
 
@@ -172,15 +175,17 @@
         self,
         args: "TrainingArguments",
         model: "PreTrainedModel",
         inputs: Dict[str, Any],
         try_to_fetch_cached_model: bool = False,
     ) -> NeuronHash:
         input_names = inspect.signature(model.forward).parameters.keys()
-        input_shapes = tuple(tuple(value.shape) for (input_name, value) in inputs.items() if input_name in input_names)
+        input_shapes = tuple(
+            (input_name, tuple(input_.shape)) for input_name, input_ in inputs.items() if input_name in input_names
+        )
 
         if args.fp16:
             data_type = torch.float16
         elif args.bf16:
             data_type = torch.bfloat16
         else:
             data_type = torch.float32
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.5/optimum/neuron/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .argument_utils import convert_neuronx_compiler_args_to_neuron
-from .import_utils import is_neuron_available, is_neuronx_available
+from .argument_utils import convert_neuronx_compiler_args_to_neuron, store_compilation_config
+from .constant import NEURON_FILE_NAME
+from .import_utils import (
+    is_accelerate_available,
+    is_neuron_available,
+    is_neuronx_available,
+    is_neuronx_distributed_available,
+    is_torch_xla_available,
+)
+from .patching import DynamicPatch, ModelPatcher, Patcher, patch_everywhere, patch_within_function
 from .training_utils import (
     FirstAndLastDataset,
-    Patcher,
     is_model_officially_supported,
     is_precompilation,
-    patch_forward,
-    patch_model,
     patch_transformers_for_neuron_sdk,
     patched_finfo,
     prepare_environment_for_neuron,
 )
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.5/optimum/neuron/utils/argument_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Utilities related to CLI arguments."""
 
 import os
-from typing import Any, Callable, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 from ...utils import logging
 
 
+if TYPE_CHECKING:
+    from transformers import PretrainedConfig
+
 logger = logging.get_logger()
 
 DISABLE_ARGUMENT_PATCH = os.environ.get("OPTIMUM_DISABLE_ARGUMENT_PATCH", "0")
 DISABLE_STRICT_MODE = os.environ.get("OPTIMUM_DISABLE_STRICT_MODE", "0")
 
 
 def validate_arg(
@@ -125,7 +129,31 @@
             f"The auto_cast value {auto_cast} is not valid. Please use one of the following: None, all or matmul."
         )
 
     if disable_fast_relayout is True:
         compiler_args.append("no-fast-relayout")
 
     return compiler_args
+
+
+def store_compilation_config(
+    config: "PretrainedConfig",
+    input_shapes: Dict[str, int],
+    compiler_kwargs: Dict[str, Any],
+    input_names: List[str],
+    output_names: List[str],
+    dynamic_batch_size: bool,
+    **kwargs,
+):
+    # Add input shapes during compilation to the config
+    for axe, shape in input_shapes.items():
+        axe = f"neuron_{axe}"
+        config.__setattr__(axe, shape)
+
+    config.__setattr__("dynamic_batch_size", dynamic_batch_size)
+
+    # Add compilation args to the config
+    for arg, value in compiler_kwargs.items():
+        config.__setattr__(arg, value)
+
+    config.input_names = input_names
+    config.output_names = output_names
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.5/optimum/neuron/utils/cache_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Utilities for caching."""
 
 import hashlib
 import io
 import json
 import os
 import re
@@ -24,18 +25,27 @@
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import huggingface_hub
 import numpy as np
 import torch
-from huggingface_hub import HfApi, HfFolder, RepoUrl, create_repo
-from huggingface_hub.utils import HfHubHTTPError, RepositoryNotFoundError
+from huggingface_hub import (
+    CommitOperationAdd,
+    CommitOperationDelete,
+    HfApi,
+    HfFolder,
+    RepoUrl,
+    create_repo,
+    hf_hub_download,
+)
+from huggingface_hub.utils import EntryNotFoundError, HfHubHTTPError, RepositoryNotFoundError
 
 from ...utils import logging
+from ...utils.logging import warn_once
 from .version_utils import get_neuronxcc_version
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedModel
 
 
@@ -53,84 +63,139 @@
 
 CACHE_REPO_NAME = "optimum-neuron-cache"
 if os.environ.get("HUGGINGFACE_CO_STAGING") == "1":
     HF_HUB_CACHE_REPOS = []
 else:
     HF_HUB_CACHE_REPOS = [f"aws-neuron/{CACHE_REPO_NAME}"]
 
-HASH_FILE_NAME = "pytorch_model.bin"
+HASH_FILENAME = "pytorch_model.bin"
+REGISTRY_FILENAME = "registry.json"
 NEURON_COMPILE_CACHE_NAME = "neuron-compile-cache"
 
 _IP_PATTERN = re.compile(r"ip-([0-9]{1,3}-){4}")
+_HF_HUB_HTTP_ERROR_REQUEST_ID_PATTERN = re.compile(r"\(Request ID: Root=[\w-]+\)")
+
+_WRITING_ACCESS_CACHE: Dict[Tuple[str, str], bool] = {}
+_REGISTRY_FILE_EXISTS: Dict[str, bool] = {}
+_ADDED_IN_REGISTRY: Dict[Tuple[str, "NeuronHash"], bool] = {}
 
 
 def load_custom_cache_repo_name_from_hf_home(
     hf_home_cache_repo_file: Union[str, Path] = HF_HOME_CACHE_REPO_FILE
 ) -> Optional[str]:
     if Path(hf_home_cache_repo_file).exists():
         with open(hf_home_cache_repo_file, "r") as fp:
             return fp.read()
     return None
 
 
-def set_custom_cache_repo_name_in_hf_home(repo_id: str, hf_home: str = HF_HOME):
+def set_custom_cache_repo_name_in_hf_home(repo_id: str, hf_home: str = HF_HOME, check_repo: bool = True):
     hf_home_cache_repo_file = f"{hf_home}/{CACHE_REPO_FILENAME}"
-    try:
-        HfApi().repo_info(repo_id, repo_type="model")
-    except Exception as e:
-        raise ValueError(
-            f"Could not save the custom Trainium cache repo to be {repo_id} because it does not exist or is private to "
-            f"you. Complete exception message: {e}."
-        )
+    if check_repo:
+        try:
+            HfApi().repo_info(repo_id, repo_type="model")
+        except Exception as e:
+            raise ValueError(
+                f"Could not save the custom Trainium cache repo to be {repo_id} because it does not exist or is "
+                f"private to you. Complete exception message: {e}."
+            )
 
     existing_custom_cache_repo = load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file)
     if existing_custom_cache_repo is not None:
         logger.warning(
             f"A custom cache repo was already registered: {existing_custom_cache_repo}. It will be overwritten to "
             f"{repo_id}."
         )
 
     with open(hf_home_cache_repo_file, "w") as fp:
         fp.write(repo_id)
 
 
+def delete_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file: str = HF_HOME_CACHE_REPO_FILE):
+    Path(hf_home_cache_repo_file).unlink(missing_ok=True)
+
+
 def create_custom_cache_repo(repo_id: str = CACHE_REPO_NAME, private: bool = True) -> RepoUrl:
     repo_url = create_repo(repo_id, private=private, repo_type="model")
+    create_registry_file_if_does_not_exist(repo_id)
     set_custom_cache_repo_name_in_hf_home(repo_url.repo_id)
     return repo_url
 
 
 def is_private_repo(repo_id: str) -> bool:
     HfApi().list_repo_files(repo_id=repo_id, token=HfFolder.get_token())
     private = False
     try:
         HfApi().list_repo_files(repo_id=repo_id, token=False)
     except RepositoryNotFoundError:
         private = True
     return private
 
 
+def has_write_access_to_repo(repo_id: str) -> bool:
+    token = HfFolder.get_token()
+    if (token, repo_id) in _WRITING_ACCESS_CACHE:
+        return _WRITING_ACCESS_CACHE[(token, repo_id)]
+
+    has_access = False
+    with tempfile.NamedTemporaryFile() as fp:
+        tmpfilename = Path(fp.name)
+        try:
+            add_file = CommitOperationAdd(tmpfilename.name, tmpfilename.as_posix())
+            HfApi().create_commit(repo_id, operations=[add_file], commit_message="Check write access")
+        except (HfHubHTTPError, RepositoryNotFoundError):
+            pass
+        else:
+            delete_file = CommitOperationDelete(tmpfilename.name)
+            HfApi().create_commit(repo_id, operations=[delete_file], commit_message="Check write access [DONE]")
+            has_access = True
+
+    _WRITING_ACCESS_CACHE[(token, repo_id)] = has_access
+    return has_access
+
+
 def get_hf_hub_cache_repos():
     hf_hub_repos = HF_HUB_CACHE_REPOS
 
     saved_custom_cache_repo = load_custom_cache_repo_name_from_hf_home()
     if saved_custom_cache_repo is None:
-        logger.warning(
+        warn_once(
+            logger,
             "No Trainium cache name is saved locally. This means that only the official Trainium cache, and "
             "potentially a cache defined in $CUSTOM_CACHE_REPO will be used. You can create a Trainium cache repo by "
             "running the following command: `optimum-cli neuron cache create`. If the Trainium cache already exists "
-            "you can set it by running the following command: `optimum-cli neuron cache set -n [name]`."
+            "you can set it by running the following command: `optimum-cli neuron cache set -n [name]`.",
         )
     else:
         hf_hub_repos = [saved_custom_cache_repo] + hf_hub_repos
 
     custom_cache_repo = os.environ.get("CUSTOM_CACHE_REPO", None)
     if custom_cache_repo is not None:
         hf_hub_repos = [custom_cache_repo] + hf_hub_repos
 
+    # TODO: this is a quick fix.
+    # Cache utils should not be aware of the multiprocessing side of things.
+    # The issue here is that `has_write_access_to_repo` actually pushes stuff to the HF Hub.
+    # Pushing stuff to the HF Hub should be limited to the `push_to_cache_on_hub` function,
+    # making it easier for higher-level abstractions using the cache utils to reason on which
+    # parts should only run on the master process and which parts should run on everyone.
+    from . import is_torch_xla_available
+
+    process_index = 0
+    if is_torch_xla_available():
+        import torch_xla.core.xla_model as xm
+
+        process_index = xm.get_ordinal()
+
+    if process_index == 0 and hf_hub_repos and not has_write_access_to_repo(hf_hub_repos[0]):
+        warn_once(
+            logger,
+            f"You do not have write access to {hf_hub_repos[0]} so you will not be able to push any cached compilation "
+            "files. Please log in and/or use a custom Trainium cache.",
+        )
     return hf_hub_repos
 
 
 def get_neuron_cache_path() -> Optional[Path]:
     # NEURON_CC_FLAGS is the environment variable read by the neuron compiler.
     # Among other things, this is where the cache directory is specified.
     neuron_cc_flags = os.environ.get("NEURON_CC_FLAGS", "")
@@ -200,14 +265,190 @@
     return Path("").joinpath(*path.parts[index:])
 
 
 def remove_ip_adress_from_path(path: Path) -> Path:
     return Path().joinpath(*(re.sub(_IP_PATTERN, "", part) for part in path.parts))
 
 
+def _get_model_name_or_path(config: "PretrainedConfig") -> Optional[str]:
+    attribute_names_to_try = ["_model_name_or_path", "_name_or_path"]
+    model_name_or_path = None
+    for name in attribute_names_to_try:
+        attribute = getattr(config, name, None)
+        if attribute is not None:
+            model_name_or_path = attribute
+            break
+    if model_name_or_path == "":
+        model_name_or_path = None
+    return model_name_or_path
+
+
+def create_registry_file_if_does_not_exist(repo_id: str):
+    was_created = _REGISTRY_FILE_EXISTS.get(repo_id, False)
+    if was_created:
+        return
+    file_exists = True
+    try:
+        hf_hub_download(repo_id, REGISTRY_FILENAME, force_download=True)
+    except EntryNotFoundError:
+        file_exists = False
+    if file_exists:
+        return
+    with tempfile.NamedTemporaryFile() as tmpfile:
+        with open(tmpfile.name, "w") as fp:
+            json.dump({}, fp)
+        tmpfilename = Path(tmpfile.name)
+        add_registry_file = CommitOperationAdd(REGISTRY_FILENAME, tmpfilename.as_posix())
+        HfApi().create_commit(repo_id, operations=[add_registry_file], commit_message="Create cache registry file")
+
+    _REGISTRY_FILE_EXISTS[repo_id] = True
+
+
+def add_in_registry(repo_id: str, neuron_hash: "NeuronHash"):
+    was_added = _ADDED_IN_REGISTRY.get((repo_id, neuron_hash), False)
+    if was_added:
+        return
+    model_name_or_path = _get_model_name_or_path(neuron_hash.model.config)
+    if model_name_or_path is None:
+        model_name_or_path = "null"
+
+    model_hash, overall_hash = neuron_hash.compute_hash()
+
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        keep_going = True
+        while keep_going:
+            tmpdirpath = Path(tmpdirname)
+            head = HfApi().model_info(repo_id).sha
+            hf_hub_download(
+                repo_id,
+                REGISTRY_FILENAME,
+                revision=head,
+                local_dir=tmpdirpath,
+                local_dir_use_symlinks=False,
+            )
+            registry_path = tmpdirpath / REGISTRY_FILENAME
+            with open(registry_path, "r") as fp:
+                registry = json.load(fp)
+
+            orig_registry = registry
+            if neuron_hash.neuron_compiler_version not in registry:
+                registry[neuron_hash.neuron_compiler_version] = {}
+            registry = registry[neuron_hash.neuron_compiler_version]
+
+            key = model_name_or_path if model_name_or_path != "null" else model_hash
+            if model_name_or_path not in registry:
+                registry[key] = {"model_name_or_path": model_name_or_path, "model_hash": model_hash}
+            registry = registry[key]
+
+            if "features" not in registry:
+                registry["features"] = []
+
+            exists_already = False
+            for feature in registry["features"]:
+                if feature["neuron_hash"] == overall_hash:
+                    exists_already = True
+
+            if not exists_already:
+                data = {
+                    "input_shapes": neuron_hash.input_shapes,
+                    "precision": str(neuron_hash.data_type),
+                    "num_neuron_cores": neuron_hash.num_neuron_cores,
+                    "neuron_hash": overall_hash,
+                }
+                registry["features"].append(data)
+
+            with open(registry_path, "w") as fp:
+                json.dump(orig_registry, fp)
+
+            add_model_in_registry = CommitOperationAdd(REGISTRY_FILENAME, registry_path.as_posix())
+            try:
+                HfApi().create_commit(
+                    repo_id,
+                    operations=[add_model_in_registry],
+                    commit_message=f"Add {model_name_or_path} in registry for NeuronHash {overall_hash}",
+                    parent_commit=head,
+                )
+            except ValueError as e:
+                if "A commit has happened since" in str(e):
+                    logger.info(
+                        "A commit has happened in cache repository since we tried to update the registry, starting again..."
+                    )
+                else:
+                    raise e
+            else:
+                keep_going = False
+
+        _ADDED_IN_REGISTRY[(repo_id, neuron_hash)] = True
+
+
+def _list_in_registry_dict(
+    registry: Dict[str, Any],
+    model_name_or_path_or_hash: Optional[str] = None,
+    neuron_compiler_version: Optional[str] = None,
+) -> List[str]:
+    entries = []
+    if neuron_compiler_version is not None:
+        registry = registry.get(neuron_compiler_version, {})
+    else:
+        for version in registry:
+            entries += _list_in_registry_dict(
+                registry, model_name_or_path_or_hash=model_name_or_path_or_hash, neuron_compiler_version=version
+            )
+        return entries
+
+    def validate_features_input_shapes(input_shapes: Tuple[Tuple[str, Tuple[int, ...]], ...]) -> bool:
+        return len(input_shapes) > 0 and all(len(entry) == 2 for entry in input_shapes)
+
+    # model_key is either a model name or path or a model hash.
+    for model_key in registry:
+        data = registry[model_key]
+        if model_name_or_path_or_hash is not None and not (
+            data["model_name_or_path"].startswith(model_name_or_path_or_hash)
+            or data["model_hash"].startswith(model_name_or_path_or_hash)
+        ):
+            continue
+
+        for features in data["features"]:
+            if not validate_features_input_shapes(features["input_shapes"]):
+                continue
+            if len(features["input_shapes"]) > 1:
+                inputs = "\n\t- ".join(f"{x[0]} => {x[1]}" for x in features["input_shapes"])
+                inputs = f"\t- {inputs}"
+            else:
+                x = features["input_shapes"][0]
+                inputs = f"\t- {x[0]} => {x[1]}"
+            information = [
+                f"Model name:\t{data['model_name_or_path']}",
+                f"Model hash:\t{data['model_hash']}",
+                f"Global hash:\t{features['neuron_hash']}",
+                f"Precision:\t{features['precision']}",
+                f"Neuron X Compiler version:\t{neuron_compiler_version}",
+                f"Num of neuron cores:\t{features['num_neuron_cores']}",
+                f"Input shapes:\n{inputs}",
+            ]
+            entries.append("\n".join(information))
+    return entries
+
+
+def list_in_registry(
+    repo_id: str, model_name_or_path_or_hash: Optional[str] = None, neuron_compiler_version: Optional[str] = None
+):
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        hf_hub_download(repo_id, REGISTRY_FILENAME, local_dir=tmpdirname, local_dir_use_symlinks=False)
+        registry_filename = Path(tmpdirname) / REGISTRY_FILENAME
+        with open(registry_filename, "r") as fp:
+            registry = json.load(fp)
+
+    return _list_in_registry_dict(
+        registry,
+        model_name_or_path_or_hash=model_name_or_path_or_hash,
+        neuron_compiler_version=neuron_compiler_version,
+    )
+
+
 class StaticTemporaryDirectory:
     def __init__(self, dirname: Union[str, Path]):
         if isinstance(dirname, str):
             dirname = Path(dirname)
         if dirname.exists():
             raise FileExistsError(
                 f"{dirname} already exists, cannot create a static temporary directory with this name."
@@ -234,15 +475,15 @@
     def __hash__(self):
         return hash(f"{self.model_hash}_{self.overall_hash}")
 
 
 @dataclass(frozen=True)
 class NeuronHash:
     model: "PreTrainedModel"
-    input_shapes: Tuple[Tuple[int], ...]
+    input_shapes: Tuple[Tuple[str, Tuple[int, ...]], ...]
     data_type: torch.dtype
     num_neuron_cores: int = field(default_factory=get_num_neuron_cores_used)
     neuron_compiler_version: str = field(default_factory=get_neuronxcc_version)
     _hash: _MutableHashAttribute = field(default_factory=_MutableHashAttribute)
 
     def __post_init__(self):
         self.compute_hash()
@@ -301,28 +542,18 @@
     def cache_path(self) -> Path:
         return Path().joinpath(*self.folders)
 
     @property
     def neuron_compiler_version_dir_name(self):
         return f"USER_neuroncc-{self.neuron_compiler_version}"
 
-    def _try_to_retrive_model_name_or_path(self, config: "PretrainedConfig") -> Optional[str]:
-        attribute_names_to_try = ["_model_name_or_path", "_name_or_path"]
-        model_name_or_path = None
-        for name in attribute_names_to_try:
-            attribute = getattr(config, name, None)
-            if attribute is not None:
-                model_name_or_path = attribute
-                break
-        return model_name_or_path
-
     @property
     def is_private(self):
         private = None
-        model_name_or_path = self._try_to_retrive_model_name_or_path(self.model.config)
+        model_name_or_path = _get_model_name_or_path(self.model.config)
         if model_name_or_path is None:
             private = True
         elif Path(model_name_or_path).exists():
             private = True
         else:
             private = is_private_repo(model_name_or_path)
         return private
@@ -441,14 +672,20 @@
     cache_repo_id: Optional[str] = None,
     overwrite_existing: bool = False,
     local_path_to_path_in_repo: Optional[Callable[[Path], Path]] = None,
 ) -> CachedModelOnTheHub:
     if cache_repo_id is None:
         cache_repo_id = get_hf_hub_cache_repos()[0]
 
+    try:
+        create_registry_file_if_does_not_exist(cache_repo_id)
+        _REGISTRY_FILE_EXISTS[cache_repo_id] = True
+    except HfHubHTTPError:
+        pass
+
     is_cache_repo_private = is_private_repo(cache_repo_id)
     if neuron_hash.is_private and not is_cache_repo_private:
         raise ValueError(
             f"Cannot push the cached model to {cache_repo_id} because this repo is not private but the original model is "
             "coming from private repo."
         )
 
@@ -478,15 +715,15 @@
             logger.warning(
                 "Overwriting the already existing cached model on the Hub by the one located at "
                 f"{local_cache_dir_or_file}"
             )
 
     could_not_push_message = (
         "Could not push the cached model to the repo {cache_repo_id}, most likely due to not having the write permission "
-        "for this repo. Exact error: {error}."
+        "for this repo. Exact error:\n{error}."
     )
     if local_cache_dir_or_file.is_dir():
         try:
             with tempfile.TemporaryDirectory() as tmpdirname:
                 local_anynonymous_cache_dir = remove_ip_adress_from_path(
                     Path(tmpdirname) / local_cache_dir_or_file.name
                 )
@@ -505,16 +742,17 @@
                 HfApi().upload_folder(
                     folder_path=local_anynonymous_cache_dir.as_posix(),
                     path_in_repo=path_in_repo.as_posix(),
                     repo_id=cache_repo_id,
                     repo_type="model",
                 )
         except HfHubHTTPError as e:
-            # TODO: create PR when no writing rights?
-            logger.warning(could_not_push_message.format(cache_repo_id=cache_repo_id, error=e))
+            msg = could_not_push_message.format(cache_repo_id=cache_repo_id, error=e)
+            msg = re.sub(_HF_HUB_HTTP_ERROR_REQUEST_ID_PATTERN, "", msg)
+            warn_once(logger, msg)
     else:
         try:
             with tempfile.TemporaryDirectory() as tmpdirname:
                 local_anynonymous_cache_file = remove_ip_adress_from_path(local_cache_dir_or_file)
                 if local_cache_dir_or_file != local_anynonymous_cache_file:
                     local_anynonymous_cache_file = Path(tmpdirname) / path_after_folder(
                         local_anynonymous_cache_file, NEURON_COMPILE_CACHE_NAME
@@ -525,10 +763,18 @@
                 HfApi().upload_file(
                     path_or_fileobj=local_anynonymous_cache_file.as_posix(),
                     path_in_repo=path_in_repo.as_posix(),
                     repo_id=cache_repo_id,
                     repo_type="model",
                 )
         except HfHubHTTPError as e:
-            # TODO: create PR when no writing rights?
-            logger.warning(could_not_push_message.format(cache_repo_id=cache_repo_id, error=e))
+            msg = could_not_push_message.format(cache_repo_id=cache_repo_id, error=e)
+            msg = re.sub(_HF_HUB_HTTP_ERROR_REQUEST_ID_PATTERN, "", msg)
+            warn_once(logger, msg)
+
+    # Adding the model to the registry.
+    try:
+        add_in_registry(cache_repo_id, neuron_hash)
+    except HfHubHTTPError:
+        pass
+
     return CachedModelOnTheHub(cache_repo_id, path_in_repo)
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.5/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.5/optimum/neuron/utils/version_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Version utilities."""
 
 
 def get_neuronxcc_version() -> str:
     try:
         import neuronxcc
     except ImportError:
```

### Comparing `optimum-neuron-0.0.4/optimum/neuron/version.py` & `optimum-neuron-0.0.5/optimum/neuron/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

### Comparing `optimum-neuron-0.0.4/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.5/optimum_neuron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -108,15 +108,15 @@
     tokenizer=tokenizer,
     data_collator=data_collator,
 )
 ```
 
 ### Documentation
 
-Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum/**neuron**/index) for more advanced usage.
+Check out [the documentation of Optimum Neuron](https://huggingface.co/docs/optimum-neuron/index) for more advanced usage.
 
 <!---
 
 ## Validated Models
 
 The following model architectures, tasks and device distributions have been validated for 🤗 Optimum Neuron:
```

### Comparing `optimum-neuron-0.0.4/pyproject.toml` & `optimum-neuron-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.4/setup.py` & `optimum-neuron-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 import re
 
 from setuptools import find_namespace_packages, setup
 
 
 # Ensure we match the version set in optimum/neuron/version.py
+filepath = "optimum/neuron/version.py"
 try:
-    filepath = "optimum/neuron/version.py"
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
     "transformers >= 4.28.0",
+    "accelerate >= 0.20.1",
     "optimum",
     "huggingface_hub >= 0.14.0",
-    "numpy>1.19, <=1.21.6",
+    "numpy>=1.18.5, <=1.21.6",
     "protobuf<4",
 ]
 
-TESTS_REQUIRE = [
-    "pytest",
-    "psutil",
-    "parameterized",
-    "GitPython",
-    "sentencepiece",
-    "datasets",
-]
+TESTS_REQUIRE = ["pytest", "psutil", "parameterized", "GitPython", "sentencepiece", "datasets", "sacremoses"]
 
 QUALITY_REQUIRES = [
     "black",
     "ruff",
     "isort",
-    "hf_doc_builder",
+    # "hf_doc_builder @ git+https://github.com/huggingface/doc-builder.git",
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
     "neuron": [
         "wheel",
         "torch-neuron==1.13.1.*",
-        "neuron-cc[tensorflow]",
+        "torch==1.13.1.*",
+        "neuron-cc[tensorflow]==1.15.*",
         "protobuf",
         "torchvision",
     ],
     "neuronx": [
         "wheel",
-        "neuronx-cc==2.*",
+        "neuronx-cc==2.6.*",
         "torch-neuronx",
         "torch==1.13.1.*",
         "torchvision==0.14.*",
     ],
 }
 
 setup(
```

### Comparing `optimum-neuron-0.0.4/tests/test_cache_utils.py` & `optimum-neuron-0.0.5/tests/test_cache_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,105 +7,76 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Tests for the cache utilities."""
 
+import json
 import logging
 import os
 import random
 from dataclasses import FrozenInstanceError
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import List
 from unittest import TestCase
 
 import torch
-from huggingface_hub import HfApi, HfFolder, create_repo, delete_repo
+from huggingface_hub import HfApi, HfFolder, create_repo, delete_repo, hf_hub_download
 from transformers import BertConfig, BertModel, set_seed
 from transformers.testing_utils import TOKEN as TRANSFORMERS_TOKEN
 from transformers.testing_utils import USER as TRANSFORMERS_USER
 from transformers.testing_utils import is_staging_test
 
 from optimum.neuron.utils.cache_utils import (
     CACHE_REPO_FILENAME,
     NEURON_COMPILE_CACHE_NAME,
+    REGISTRY_FILENAME,
     NeuronHash,
+    _list_in_registry_dict,
+    add_in_registry,
+    create_registry_file_if_does_not_exist,
     download_cached_model_from_hub,
     get_cached_model_on_the_hub,
     get_neuron_cache_path,
     get_num_neuron_cores_used,
+    has_write_access_to_repo,
     list_files_in_neuron_cache,
+    list_in_registry,
     load_custom_cache_repo_name_from_hf_home,
     path_after_folder,
     push_to_cache_on_hub,
     remove_ip_adress_from_path,
     set_custom_cache_repo_name_in_hf_home,
     set_neuron_cache_path,
 )
 from optimum.neuron.utils.testing_utils import is_trainium_test
+from optimum.utils.testing_utils import TOKEN, USER
 
-# Use that once optimum==1.7.4 is released.
-# from optimum.utils.testing_utils import USER
-from .utils import TOKEN, MyTinyModel, StagingTestMixin, get_random_string
+from .utils import MyTinyModel, StagingTestMixin, get_random_string
 
 
-USER = "__DUMMY_OPTIMUM_USER__"
-
 DUMMY_COMPILER_VERSION = "1.2.3"
 
 
 class NeuronUtilsTestCase(TestCase):
     def test_load_custom_cache_repo_name_from_hf_home(self):
         with TemporaryDirectory() as tmpdirname:
             hf_home_cache_repo_file = f"{tmpdirname}/{CACHE_REPO_FILENAME}"
             with open(hf_home_cache_repo_file, "w") as fp:
                 fp.write("blablabla")
             self.assertEqual(load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file), "blablabla")
 
             bad_hf_home_cache_repo_file = f"{tmpdirname}/does_not_exist"
             self.assertIsNone(load_custom_cache_repo_name_from_hf_home(bad_hf_home_cache_repo_file))
 
-    @is_staging_test
-    def test_set_custom_cache_repo_name_in_hf_home(self):
-        orig_token = HfFolder.get_token()
-        HfFolder.save_token(TOKEN)
-
-        repo_name = "blablabla"
-        repo_id = f"{USER}/{repo_name}"
-        create_repo(repo_name, repo_type="model")
-
-        def remove_repo():
-            delete_repo(repo_name, repo_type="model")
-
-        with TemporaryDirectory() as tmpdirname:
-            try:
-                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
-            except ValueError as e:
-                remove_repo()
-                if orig_token:
-                    HfFolder.save_token(orig_token)
-                self.fail(str(e))
-
-            with open(f"{tmpdirname}/{CACHE_REPO_FILENAME}", "r") as fp:
-                content = fp.read()
-
-            self.assertEqual(content, repo_id, "The stored repo id must match the one specified.")
-
-            with self.assertLogs("optimum", level=logging.WARNING) as cm:
-                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
-                self.assertIn("A custom cache repo was already", cm.output[0])
-
-            remove_repo()
-            if orig_token:
-                HfFolder.save_token(orig_token)
-
     def test_get_neuron_cache_path(self):
         os.environ["NEURON_CC_FLAGS"] = "--some --parameters --here --no-cache --other --paremeters --here"
         assert get_neuron_cache_path() is None
 
         custom_cache_dir_name = Path("_this/is_/my1/2custom/cache/dir")
         os.environ[
             "NEURON_CC_FLAGS"
@@ -180,27 +151,216 @@
 
         with TemporaryDirectory() as tmpdirname:
             filenames = self._create_random_neuron_cache(Path(tmpdirname), return_only_relevant_files=True)
             self.assertSetEqual(
                 set(filenames), set(list_files_in_neuron_cache(Path(tmpdirname), only_relevant_files=True))
             )
 
+    def test_list_in_registry_dict(self):
+        registry = {
+            "2.1.0": {
+                "model_1": {
+                    "model_name_or_path": "model_1",
+                    "model_hash": "my model hash",
+                    "features": [
+                        {
+                            "input_shapes": [["x", [1, 2]], ["y", [2, 3]]],
+                            "precision": "torch.float32",
+                            "num_neuron_cores": 16,
+                            "neuron_hash": "neuron hash 1",
+                        },
+                        {
+                            "input_shapes": [["x", [3, 2]], ["y", [7, 3]]],
+                            "precision": "torch.float32",
+                            "num_neuron_cores": 8,
+                            "neuron_hash": "neuron hash 2",
+                        },
+                    ],
+                },
+                "model_2": {
+                    "model_name_or_path": "null",
+                    "model_hash": "my model hash 2",
+                    "features": [
+                        {
+                            "input_shapes": [["x", [1, 2]], ["y", [2, 3]]],
+                            "precision": "torch.float16",
+                            "num_neuron_cores": 16,
+                            "neuron_hash": "neuron hash 3",
+                        },
+                        {
+                            "input_shapes": [["x", [3, 2]], ["y", [7, 3]]],
+                            "precision": "torch.float32",
+                            "num_neuron_cores": 8,
+                            "neuron_hash": "neuron hash 4",
+                        },
+                    ],
+                },
+            },
+            "2.5.0": {
+                "model_1": {
+                    "model_name_or_path": "model_1",
+                    "model_hash": "my model hash",
+                    "features": [
+                        {
+                            "input_shapes": [["x", [1, 2]], ["y", [2, 3]]],
+                            "precision": "torch.float32",
+                            "num_neuron_cores": 16,
+                            "neuron_hash": "neuron hash 5",
+                        },
+                        {
+                            "input_shapes": [["x", [3, 2]], ["y", [7, 3]]],
+                            "precision": "torch.float32",
+                            "num_neuron_cores": 8,
+                            "neuron_hash": "neuron hash 6",
+                        },
+                    ],
+                },
+            },
+        }
+
+        result = _list_in_registry_dict(registry)
+        self.assertEqual(len(result), 6)
+        self.assertTrue(result[-1].startswith("Model name:\tmodel_1"))
+
+        result = _list_in_registry_dict(registry, model_name_or_path_or_hash="model_1")
+        self.assertEqual(len(result), 4)
+        self.assertTrue(result[0].startswith("Model name:\tmodel_1"))
+
+        result = _list_in_registry_dict(registry, model_name_or_path_or_hash="my model hash 2")
+        self.assertEqual(len(result), 2)
+        self.assertTrue(result[0].startswith("Model name:\tnull"))
+
+        result = _list_in_registry_dict(registry, neuron_compiler_version="2.5.0")
+        self.assertEqual(len(result), 2)
+        self.assertTrue(result[0].startswith("Model name:\tmodel_1"))
+
+        result = _list_in_registry_dict(registry, model_name_or_path_or_hash="random bad string")
+        self.assertEqual(len(result), 0)
+
+        result = _list_in_registry_dict(registry, neuron_compiler_version="-1.2")
+        self.assertEqual(len(result), 0)
+
+
+@is_staging_test
+class StagingNeuronUtilsTestCase(StagingTestMixin, TestCase):
+    def test_set_custom_cache_repo_name_in_hf_home(self):
+        orig_token = HfFolder.get_token()
+        HfFolder.save_token(TOKEN)
+
+        repo_name = f"blablabla-{self.seed}"
+        repo_id = f"{USER}/{repo_name}"
+        create_repo(repo_name, repo_type="model")
+
+        def remove_repo():
+            delete_repo(repo_name, repo_type="model")
+
+        with TemporaryDirectory() as tmpdirname:
+            try:
+                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
+            except ValueError as e:
+                remove_repo()
+                if orig_token:
+                    HfFolder.save_token(orig_token)
+                self.fail(str(e))
+
+            with open(f"{tmpdirname}/{CACHE_REPO_FILENAME}", "r") as fp:
+                content = fp.read()
+
+            self.assertEqual(content, repo_id, "The stored repo id must match the one specified.")
+
+            with self.assertLogs("optimum", level=logging.WARNING) as cm:
+                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
+                self.assertIn("A custom cache repo was already", cm.output[0])
+
+            remove_repo()
+            if orig_token:
+                HfFolder.save_token(orig_token)
+
+    @is_staging_test
+    def test_has_write_access_to_repo(self):
+        orig_token = HfFolder.get_token()
+        wrong_token = "random_string"
+        HfFolder.save_token(wrong_token)
+
+        self.assertFalse(has_write_access_to_repo(self.CUSTOM_CACHE_REPO))
+        self.assertFalse(has_write_access_to_repo(self.CUSTOM_PRIVATE_CACHE_REPO))
+
+        HfFolder.save_token(orig_token)
+
+        self.assertTrue(has_write_access_to_repo(self.CUSTOM_CACHE_REPO))
+        self.assertTrue(has_write_access_to_repo(self.CUSTOM_PRIVATE_CACHE_REPO))
+
+    @is_staging_test
+    def test_list_in_registry(self):
+        def _test_list_in_registry(use_private_cache_repo: bool):
+            if use_private_cache_repo:
+                cache_repo = self.CUSTOM_PRIVATE_CACHE_REPO
+            else:
+                cache_repo = self.CUSTOM_CACHE_REPO
+            create_registry_file_if_does_not_exist(cache_repo)
+            entries = list_in_registry(cache_repo)
+            self.assertEqual(len(entries), 0)
+
+            bert_model = BertModel(BertConfig())
+            neuron_hash = NeuronHash(
+                bert_model,
+                (("x", (4, 12)), ("y", (4, 12))),
+                torch.float32,
+                2,
+                neuron_compiler_version=DUMMY_COMPILER_VERSION,
+            )
+            add_in_registry(cache_repo, neuron_hash)
+            entries = list_in_registry(cache_repo)
+            self.assertEqual(len(entries), 1)
+
+            bert_model = BertModel(BertConfig())
+            neuron_hash = NeuronHash(
+                bert_model,
+                (("x", (4, 8)), ("y", (4, 12))),
+                torch.float32,
+                2,
+                neuron_compiler_version=DUMMY_COMPILER_VERSION,
+            )
+            add_in_registry(cache_repo, neuron_hash)
+            entries = list_in_registry(cache_repo)
+            self.assertEqual(len(entries), 2)
+
+            model_hash = neuron_hash.compute_hash()[0]
+            entries = list_in_registry(cache_repo, model_name_or_path_or_hash=model_hash)
+            self.assertEqual(len(entries), 1)
+
+            entries = list_in_registry(cache_repo, model_name_or_path_or_hash="dummy hash")
+            self.assertEqual(len(entries), 0)
+
+            entries = list_in_registry(cache_repo, neuron_compiler_version=DUMMY_COMPILER_VERSION)
+            self.assertEqual(len(entries), 2)
+
+            entries = list_in_registry(cache_repo, neuron_compiler_version="Bad version")
+            self.assertEqual(len(entries), 0)
+
+        _test_list_in_registry(False)
+        _test_list_in_registry(True)
+
 
 class NeuronHashTestCase(TestCase):
     def test_neuron_hash_is_not_mutable(self):
         bert_model = BertModel(BertConfig())
         neuron_hash = NeuronHash(
-            bert_model, ((4, 12), (4, 12)), torch.float32, 2, neuron_compiler_version=DUMMY_COMPILER_VERSION
+            bert_model,
+            (("x", (4, 12)), ("y", (4, 12))),
+            torch.float32,
+            2,
+            neuron_compiler_version=DUMMY_COMPILER_VERSION,
         )
 
         with self.assertRaises(FrozenInstanceError):
             neuron_hash.model = bert_model
 
         with self.assertRaises(FrozenInstanceError):
-            neuron_hash.input_shapes = ((2, 32), (2, 32))
+            neuron_hash.input_shapes = (("x", (2, 32)), ("y", (2, 32)))
 
         with self.assertRaises(FrozenInstanceError):
             neuron_hash.num_neuron_cores = 32
 
     def _test_neuron_hash(
         self,
         model_a,
@@ -274,15 +434,15 @@
         params_a = [p[0] for p in parameters]
         for i in range(len(parameters)):
             params_b = [p[int(i == j)] for j, p in enumerate(parameters)]
             self._test_neuron_hash(bert_model, *params_a, bert_model, *params_b, False)
 
     def test_neuron_hash_folders(self):
         bert_model = BertModel(BertConfig())
-        input_shapes = ((1, 2), (2, 3))
+        input_shapes = (("x", (1, 2)), ("y", (2, 3)))
         data_type = torch.float32
         num_neuron_cores = 32
 
         neuron_hash = NeuronHash(
             bert_model,
             input_shapes,
             data_type,
@@ -290,15 +450,15 @@
             neuron_compiler_version=DUMMY_COMPILER_VERSION,
         )
         hashes = neuron_hash.compute_hash()
         expected_folders = [DUMMY_COMPILER_VERSION, "bert"] + list(hashes)
         self.assertListEqual(neuron_hash.folders, expected_folders)
 
     def test_neuron_hash_is_private(self):
-        input_shapes = ((1, 2), (2, 3))
+        input_shapes = (("x", (1, 2)), ("y", (2, 3)))
         data_type = torch.float32
 
         bert_model = BertModel(BertConfig())
         neuron_hash = NeuronHash(bert_model, input_shapes, data_type, neuron_compiler_version=DUMMY_COMPILER_VERSION)
         self.assertTrue(neuron_hash.is_private)
 
         bert_model = BertModel.from_pretrained("hf-internal-testing/tiny-random-bert")
@@ -318,15 +478,15 @@
 @is_trainium_test
 @is_staging_test
 class CachedModelOnTheHubTestCase(StagingTestMixin, TestCase):
     def test_push_to_hub_fails_with_private_model_and_public_repo(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
 
-            input_shapes = (1,)
+            input_shapes = (("x", (1,)),)
             data_type = torch.float32
             tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
             neuron_hash = NeuronHash(tiny_model, input_shapes, data_type)
 
             cached_files = list_files_in_neuron_cache(Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME)
 
             # The model being loaded locally is assumed to be private, push to hub should prevent from pushing to a
@@ -340,29 +500,29 @@
             )
             self.assertIsNotNone(cached_model_on_the_hub)
 
     def test_push_to_hub_without_specifying_a_cache_repo_id(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
 
-            input_shapes = (1,)
+            input_shapes = (("x", (1,)),)
             data_type = torch.float32
             tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
             neuron_hash = NeuronHash(tiny_model, input_shapes, data_type)
 
             cached_files = list_files_in_neuron_cache(Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME)
 
-            os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
+            set_custom_cache_repo_name_in_hf_home(self.CUSTOM_PRIVATE_CACHE_REPO)
             push_to_cache_on_hub(neuron_hash, cached_files[0])
 
     def test_push_to_hub_overwrite_existing(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
 
-            input_shapes = (1,)
+            input_shapes = (("x", (1,)),)
             data_type = torch.float32
             tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
             neuron_hash = NeuronHash(tiny_model, input_shapes, data_type)
 
             cache_dir = Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME
             cached_files = list_files_in_neuron_cache(cache_dir)
 
@@ -392,15 +552,15 @@
                     "Overwriting the already existing cached model on the Hub by the one located at", cm.output[0]
                 )
 
     def test_push_to_hub_local_path_in_repo(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
 
-            input_shapes = (1,)
+            input_shapes = (("x", (1,)),)
             data_type = torch.float32
             tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
             neuron_hash = NeuronHash(tiny_model, input_shapes, data_type)
 
             cache_dir = Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME
             cached_files = list_files_in_neuron_cache(cache_dir)
 
@@ -441,62 +601,108 @@
                     )
                     self.assertIn(path_in_repo, files_in_repo)
 
     def test_push_to_hub_without_writing_rights(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
 
-            input_shapes = ((1,),)
+            input_shapes = (("x", (1,)),)
             data_type = torch.float32
             tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
-            tiny_model.push_to_hub("tiny-public-model")
-            public_tiny_model = MyTinyModel.from_pretrained(f"{USER}/tiny-public-model")
+            tiny_model.push_to_hub(f"tiny-public-model-{self.seed}")
+            public_tiny_model = MyTinyModel.from_pretrained(f"{USER}/tiny-public-model-{self.seed}")
             neuron_hash = NeuronHash(public_tiny_model, input_shapes, data_type)
 
             public_tiny_model = public_tiny_model.to("xla")
             input_ = torch.rand((32, 1)).to("xla")
             print(public_tiny_model(input_))
 
             # This should work because we do have writing access to this repo.
-            os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_CACHE_REPO
+            set_custom_cache_repo_name_in_hf_home(self.CUSTOM_CACHE_REPO)
             push_to_cache_on_hub(neuron_hash, get_neuron_cache_path())
 
             # Creating a repo under the Transformers user.
             orig_token = self.set_hf_hub_token(TRANSFORMERS_TOKEN)
-            repo_name = "optimum-neuron-cache"
+            repo_name = f"optimum-neuron-cache-{self.seed}"
             create_repo(repo_name, repo_type="model", exist_ok=True)
             self.set_hf_hub_token(orig_token)
 
-            os.environ["CUSTOM_CACHE_REPO"] = f"{TRANSFORMERS_USER}/{repo_name}"
+            set_custom_cache_repo_name_in_hf_home(f"{TRANSFORMERS_USER}/{repo_name}")
             with self.assertLogs("optimum", "WARNING") as cm:
                 push_to_cache_on_hub(neuron_hash, get_neuron_cache_path())
                 self.assertTrue(any("Could not push the cached model to the repo" in output for output in cm.output))
 
             self.set_hf_hub_token(TRANSFORMERS_TOKEN)
             delete_repo(repo_name, repo_type="model")
             self.set_hf_hub_token(orig_token)
 
+    def _test_push_to_hub_create_and_add_registry(self, with_model_name_or_path: bool):
+        with TemporaryDirectory() as tmpdirname:
+            set_neuron_cache_path(tmpdirname)
+
+            input_shapes = (("x", (1,)),)
+            data_type = torch.float32
+            data_type = torch.float32
+            tiny_model = self.create_and_run_tiny_pretrained_model(random_num_linears=True)
+            model_name = f"dummy_model-{self.seed}"
+            if with_model_name_or_path:
+                tiny_model.push_to_hub(model_name)
+                model_name = f"{USER}/{model_name}"
+                tiny_model.config._model_name_or_path = model_name
+            neuron_hash = NeuronHash(tiny_model, input_shapes, data_type)
+
+            set_custom_cache_repo_name_in_hf_home(self.CUSTOM_PRIVATE_CACHE_REPO)
+            files_in_repo = HfApi().list_repo_files(repo_id=self.CUSTOM_PRIVATE_CACHE_REPO)
+            files_in_repo = [filename for filename in files_in_repo if not filename.startswith(".")]
+            self.assertListEqual(files_in_repo, [], "Repo should be empty")
+
+            cached_files = list_files_in_neuron_cache(Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME)
+            push_to_cache_on_hub(neuron_hash, cached_files[0])
+            files_in_repo = HfApi().list_repo_files(repo_id=self.CUSTOM_PRIVATE_CACHE_REPO)
+
+            self.assertIn(REGISTRY_FILENAME, files_in_repo)
+            hf_hub_download(
+                self.CUSTOM_PRIVATE_CACHE_REPO,
+                REGISTRY_FILENAME,
+                force_download=True,
+                local_dir=tmpdirname,
+                local_dir_use_symlinks=False,
+            )
+            with open(Path(tmpdirname) / REGISTRY_FILENAME, "r") as fp:
+                registry = json.load(fp)
+
+            neuron_compiler_version = list(registry.keys())[0]
+            model_key = list(registry[neuron_compiler_version].keys())[0]
+            expected_value = model_name if with_model_name_or_path else neuron_hash.compute_hash()[0]
+            self.assertEqual(model_key, expected_value)
+
+    def test_push_to_hub_create_and_add_registry_without_model_name_or_path(self):
+        return self._test_push_to_hub_create_and_add_registry(False)
+
+    def test_push_to_hub_create_and_add_registry_with_model_name_or_path(self):
+        return self._test_push_to_hub_create_and_add_registry(True)
+
     def test_download_cached_model_from_hub(self):
-        os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
-        neuron_hash = self.push_tiny_pretrained_model_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
+        set_custom_cache_repo_name_in_hf_home(self.CUSTOM_PRIVATE_CACHE_REPO)
+        neuron_hash = self.push_tiny_pretrained_model_cache_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
 
         neuron_cc_flags = os.environ["NEURON_CC_FLAGS"]
 
         with self.assertRaisesRegex(
             ValueError, "A target directory must be specified when no caching directory is used"
         ):
             os.environ["NEURON_CC_FLAGS"] = "--no-cache"
             self.assertTrue(download_cached_model_from_hub(neuron_hash))
 
         os.environ["NEURON_CC_FLAGS"] = neuron_cc_flags
         self.assertTrue(download_cached_model_from_hub(neuron_hash))
 
     def test_download_cached_model_from_hub_with_target_directory(self):
-        os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
-        neuron_hash = self.push_tiny_pretrained_model_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
+        set_custom_cache_repo_name_in_hf_home(self.CUSTOM_PRIVATE_CACHE_REPO)
+        neuron_hash = self.push_tiny_pretrained_model_cache_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
 
         cached_model_on_the_hub = get_cached_model_on_the_hub(neuron_hash)
         if cached_model_on_the_hub is None:
             self.fail("Could not find the model on the Hub, but it should be there.")
 
         repo_files = set(cached_model_on_the_hub.files_on_the_hub)
 
@@ -518,16 +724,16 @@
             success = download_cached_model_from_hub(neuron_hash, target_directory=tmpdir)
             self.assertTrue(success)
 
             target_directory_files = {str(path_after_folder(f, tmpdir)) for f in tmpdir.glob("**/*") if f.is_file()}
             self.assertSetEqual(target_directory_files, repo_files)
 
     def test_download_cached_model_from_hub_with_path_in_repo_to_path_in_target_directory(self):
-        os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
-        neuron_hash = self.push_tiny_pretrained_model_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
+        set_custom_cache_repo_name_in_hf_home(self.CUSTOM_PRIVATE_CACHE_REPO)
+        neuron_hash = self.push_tiny_pretrained_model_cache_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO)
 
         cached_model_on_the_hub = get_cached_model_on_the_hub(neuron_hash)
         if cached_model_on_the_hub is None:
             self.fail("Could not find the model on the Hub, but it should be there.")
 
         def path_in_repo_to_path_in_target_directory(path):
             return Path("custom_folder") / path.name
@@ -557,15 +763,15 @@
             # self.assertListEqual([f.name for f in tmpdir.iterdir()], ["custom_folder"])
 
     # TODO: not passing yet, to fix ASAP.
     # def test_download_cached_model_from_hub_needs_to_download(self):
     #     os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
 
     #     with TemporaryDirectory() as tmpdirname:
-    #         neuron_hash = self._push_tiny_pretrained_model_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO, cache_dir=tmpdirname)
+    #         neuron_hash = self._push_tiny_pretrained_model_cache_to_hub(self.CUSTOM_PRIVATE_CACHE_REPO, cache_dir=tmpdirname)
 
     #         with patch("huggingface_hub.snapshot_download") as mock_snapshot_download:
     #             # All the files are already there, should not download anything.
     #             download_cached_model_from_hub(neuron_hash, target_directory=tmpdirname)
     #             self.assertFalse(mock_snapshot_download.called, "No downloading should be peformed since all the files are already in the cache.")
     #             mock_snapshot_download.reset_mock()
     #
```

### Comparing `optimum-neuron-0.0.4/tests/test_examples.py` & `optimum-neuron-0.0.5/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,29 +37,34 @@
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
 
-from optimum.neuron.utils.cache_utils import set_neuron_cache_path
+from optimum.neuron.utils.cache_utils import (
+    load_custom_cache_repo_name_from_hf_home,
+    set_custom_cache_repo_name_in_hf_home,
+    set_neuron_cache_path,
+)
 from optimum.neuron.utils.testing_utils import is_trainium_test
 
 
 # Doing it this way to be able to use this file in tools.
 path_tests = Path(__file__).parent
 sys.path.insert(0, str(path_tests))
 from utils import MODELS_TO_TEST_MAPPING  # noqa: E402
 
 
 TOKEN = HfFolder.get_token()
 if os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI", None) is not None:
-    print("TESSSST", os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI"))
     TOKEN = os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI")
 
+CACHE_REPO_NAME = "optimum-internal-testing/optimum-neuron-cache-for-testing"
+
 
 def _get_supported_models_for_script(
     models_to_test: Dict[str, str], task_mapping: Dict[str, str], to_exclude: Optional[Set[str]] = None
 ) -> List[str]:
     """
     Filters models that can perform the task from models_to_test.
     """
@@ -250,29 +255,36 @@
     LEARNING_RATE = 1e-4
     TRAIN_BATCH_SIZE = 16
     EVAL_BATCH_SIZE = 16
     GRADIENT_ACCUMULATION_STEPS = 16
     NPROC_PER_NODE = 2
     EXTRA_COMMAND_LINE_ARGUMENTS = None
     LOGGING_STEPS = 1
-    SAVE_STEPS = -1
+    SAVE_STEPS = 200
     ONLY_PRECOMPILATION = False
-    DO_PRECOMPILATION = True
+    DO_PRECOMPILATION = False
     NEURON_CACHE = None
     MULTI_PROC = os.environ.get("MULTI_PROC", "false")
     BF16 = True
 
     @classmethod
     def setUpClass(cls):
         cls._create_venv()
+        cls._orig_token = HfFolder.get_token()
+        cls._orig_cache_repo = load_custom_cache_repo_name_from_hf_home()
         HfFolder.save_token(TOKEN)
+        set_custom_cache_repo_name_in_hf_home(CACHE_REPO_NAME)
 
     @classmethod
     def tearDownClass(cls):
         cls._remove_venv()
+        if cls._orig_token is not None:
+            HfFolder.save_token(cls._orig_token)
+        if cls._orig_cache_repo is not None:
+            set_custom_cache_repo_name_in_hf_home(cls._orig_cache_repo)
 
     def setUp(self):
         set_neuron_cache_path("/var/tmp/neuron-compile-cache")
 
     def tearDown(self):
         set_neuron_cache_path("/var/tmp/neuron-compile-cache")
 
@@ -319,17 +331,19 @@
         logging_steps = ExampleTestMeta.process_class_attribute(self.LOGGING_STEPS, model_type)
         save_steps = ExampleTestMeta.process_class_attribute(self.SAVE_STEPS, model_type)
 
         bf16 = ExampleTestMeta.process_class_attribute(self.BF16, model_type)
         multi_proc = ExampleTestMeta.process_class_attribute(self.MULTI_PROC, model_type)
 
         # Extra
-        extra_command_line_arguments = [
-            ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
-        ]
+        extra_command_line_arguments = []
+        if self.EXTRA_COMMAND_LINE_ARGUMENTS is not None:
+            extra_command_line_arguments = [
+                ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
+            ]
 
         do_eval = eval_is_supported and not is_precompilation
 
         do_eval_option = "--do_eval" if do_eval else " "
         task_option = f"--{dataset_parameter_name} {task}" if task else " "
 
         if multi_proc == "false":
@@ -487,48 +501,54 @@
             p = subprocess.Popen(cmd_line, env=env_with_updated_path)
             self.assertEqual(return_code, 0)
 
 
 class CausalLMExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_clm"):
     TASK_NAME = "wikitext"
     DATASET_CONFIG_NAME = "wikitext-2-raw-v1"
-    NUM_EPOCHS = 3
-    TRAIN_BATCH_SIZE = 4
+    NUM_EPOCHS = 1
+    TRAIN_BATCH_SIZE = {"default": 2, "gpt2": 1}
+    EVAL_BATCH_SIZE = 2
     SCORE_NAME = "random_test"
     EVAL_SCORE_THRESHOLD = 35
     EVAL_SCORE_GREATER_IS_BETTER = False
 
 
 class TextClassificationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_glue"):
     TASK_NAME = "sst2"
     DATASET_PARAMETER_NAME = "task_name"
+    NUM_EPOCHS = 1
 
 
 class TokenClassificationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_ner"):
     TASK_NAME = "conll2003"
     TRAIN_BATCH_SIZE = {"default": 4, "distilbert": 6}
     EVAL_BATCH_SIZE = {"default": 4, "distilbert": 6}
+    NUM_EPOCHS = 1
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--max_seq_length 384",
     ]
 
 
 class MultipleChoiceExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_swag"):
     EVAL_SCORE_THRESHOLD = {"default": 0.75, "camembert": 0.5, "distilbert": 0.645}
     TRAIN_BATCH_SIZE = {"default": 2, "distilbert": 3}
     EVAL_BATCH_SIZE = {"default": 2, "distilbert": 3}
-    NUM_EPOCHS = 3
+    MAX_STEPS = 100
+    NUM_EPOCHS = 1
     EXTRA_COMMAND_LINE_ARGUMENTS = [
+        "--max_eval_samples 840",
         "--max_seq_length 512",
     ]
 
 
 class QuestionAnsweringExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_qa"):
     TASK_NAME = "squad"
     SCORE_NAME = "eval_f1"
+    NUM_EPOCHS = 1
 
 
 class SummarizationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_summarization"):
     TASK_NAME = "cnn_dailymail"
     DATASET_CONFIG_NAME = "3.0.0"
     TRAIN_BATCH_SIZE = 1
     EVAL_BATCH_SIZE = 1
@@ -581,58 +601,44 @@
         "--pad_to_max_length",
         {"default": "--max_source_length 512", "m2m_100": "--max_source_length 128"},
         {"default": "--max_target_length 512", "m2m_100": "--max_target_length 128"},
         # "--max_source_length 512",
         # "--max_target_length 512",
         "--prediction_loss_only",
     ]
-    # TODO: for now it does not work for T5, enable this ASAP.
-    DO_PRECOMPILATION = {"t5": False, "default": True}
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
+        model_type: str,
         output_dir: str,
         is_precompilation: bool = False,
-        task: Optional[str] = None,
-        dataset_config_name: Optional[str] = None,
-        do_eval: bool = True,
-        lr: float = 1e-4,
-        train_batch_size: int = 1,
-        eval_batch_size: int = 1,
-        num_epochs: int = 2,
-        gradient_accumulation_steps: int = 64,
-        extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
+        extra_command_line_arguments = [
+            ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
+        ]
         if extra_command_line_arguments is None:
             extra_command_line_arguments = []
         if "t5" in model_name:
             extra_command_line_arguments.append("--source_prefix 'translate English to Romanian: '")
         return super()._create_command_line(
             script,
             model_name,
+            model_type,
             output_dir,
             is_precompilation=is_precompilation,
-            task=task,
-            dataset_config_name=dataset_config_name,
-            do_eval=do_eval,
-            lr=lr,
-            train_batch_size=train_batch_size,
-            eval_batch_size=eval_batch_size,
-            num_epochs=num_epochs,
-            gradient_accumulation_steps=gradient_accumulation_steps,
-            extra_command_line_arguments=extra_command_line_arguments,
         )
 
 
 class ImageClassificationExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_image_classification"
 ):
     TASK_NAME = "cifar10"
+    NUM_EPOCHS = 2
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--remove_unused_columns false",
         "--dataloader_drop_last true",
         "--ignore_mismatched_sizes",
     ]
```

### Comparing `optimum-neuron-0.0.4/tests/test_trainer_callback.py` & `optimum-neuron-0.0.5/tests/test_trainer_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from unittest import TestCase
 
 import torch
@@ -48,15 +49,15 @@
 
         callback = NeuronCacheCallaback()
 
         # We first check that no hashes is in the hash cache already.
         self.assertFalse(callback.neuron_hashes)
 
         callback.neuron_hash_for_model(args, model, inputs)
-        neuron_hash = callback.neuron_hashes[(model, (tuple(inputs["x"].shape),), torch.float32)]
+        neuron_hash = callback.neuron_hashes[(model, (("x", tuple(inputs["x"].shape)),), torch.float32)]
 
         same_neuron_hash = callback.neuron_hash_for_model(args, model, inputs)
 
         self.assertEqual(neuron_hash, same_neuron_hash, "Neuron hashes should be equal")
         self.assertEqual(len(callback.neuron_hashes.keys()), 1, "There should be only one entry in neuron_hashes.")
 
     def test_try_to_fetch_cached_model(self):
@@ -64,15 +65,15 @@
         model = self.create_tiny_pretrained_model(random_num_linears=True).to("xla")
 
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
             args = TrainingArguments(tmpdirname)
             inputs = {"x": torch.rand((8, 1)).to("xla")}
             print(model(**inputs))
-            neuron_hash = NeuronHash(model, ((8, 1),), torch.float32)
+            neuron_hash = NeuronHash(model, (("x", (8, 1)),), torch.float32)
             push_to_cache_on_hub(neuron_hash, Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME)
 
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
             callback = NeuronCacheCallaback()
             args = TrainingArguments(tmpdirname)
             inputs = {"x": torch.rand((24, 1))}
```

### Comparing `optimum-neuron-0.0.4/tests/test_trainers.py` & `optimum-neuron-0.0.5/tests/test_trainers.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 
 import copy
+import json
 import os
 import random
 import subprocess
 import time
 import unittest
 from pathlib import Path
 from tempfile import TemporaryDirectory
@@ -31,28 +33,28 @@
 from optimum.neuron.utils.cache_utils import (
     get_neuron_cache_path,
     list_files_in_neuron_cache,
     remove_ip_adress_from_path,
     set_neuron_cache_path,
 )
 from optimum.neuron.utils.testing_utils import is_trainium_test
+from optimum.utils.testing_utils import USER
 
 from .utils import (
-    USER,
     StagingTestMixin,
     create_dummy_dataset,
     create_dummy_text_classification_dataset,
     create_tiny_pretrained_model,
     get_random_string,
 )
 
 
 @is_trainium_test
 @is_staging_test
-class TrainiumTrainerTestCase(StagingTestMixin, TestCase):
+class StagingTrainiumTrainerTestCase(StagingTestMixin, TestCase):
     def test_train_and_eval(self):
         os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
 
         # We take a batch size that does not divide the total number of samples.
         num_train_samples = 1000
         per_device_train_batch_size = 32
         dummy_train_dataset = create_dummy_dataset({"x": (1,), "labels": (1,)}, num_train_samples)
@@ -302,7 +304,122 @@
 
             self.assertTrue(
                 second_training_duration < first_training_duration,
                 "Second training should be faster because cached graphs can be used.",
             )
 
         self.remove_model_and_dataset_on_staging_hub(dataset_name, model_name)
+
+
+@is_trainium_test
+class TrainiumTrainerTestCase(TestCase):
+    def _test_training_with_fsdp_mode(self, fsdp_mode: str):
+        model_name = "prajjwal1/bert-tiny"
+        task_name = "sst2"
+
+        with TemporaryDirectory() as tmpdirname:
+            set_neuron_cache_path(tmpdirname)
+            output_1 = Path(tmpdirname) / "out_1"
+            fsdp_cmd = [
+                "torchrun",
+                "--nproc_per_node=2",
+                "examples/text-classification/run_glue.py",
+                f"--model_name_or_path={model_name}",
+                f"--task_name={task_name}",
+                "--per_device_train_batch_size=16",
+                "--per_device_eval_batch_size=16",
+                f"--output_dir={output_1}",
+                "--save_strategy=steps",
+                "--save_steps=10",
+                "--max_steps=100",
+                "--do_train",
+                # "--do_eval",
+                "--bf16",
+                f"--fsdp={fsdp_mode}",
+            ]
+
+            proc = subprocess.Popen(fsdp_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            stdout, stderr = proc.communicate()
+
+            checkpoint = output_1 / "checkpoint-50"
+            output_2 = Path(tmpdirname) / "out_2"
+
+            resume_fsdp_cmd = [
+                "torchrun",
+                "--nproc_per_node=2",
+                "examples/text-classification/run_glue.py",
+                f"--model_name_or_path={model_name}",
+                f"--task_name={task_name}",
+                "--per_device_train_batch_size=16",
+                "--per_device_eval_batch_size=16",
+                f"--output_dir={output_2}",
+                "--save_strategy=steps",
+                "--save_steps=10",
+                "--max_steps=100",
+                "--do_train",
+                # "--do_eval",
+                "--bf16",
+                f"--resume_from_checkpoint={checkpoint}",
+                f"--fsdp={fsdp_mode}",
+            ]
+
+            proc = subprocess.Popen(resume_fsdp_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            stdout, stderr = proc.communicate()
+
+            training_fsdp_metrics = {}
+            with open(output_1 / "all_results.json") as fp:
+                training_fsdp_metrics = json.load(fp)
+
+            resume_training_fsdp_metrics = {}
+            with open(output_2 / "all_results.json") as fp:
+                resume_training_fsdp_metrics = json.load(fp)
+
+            print(training_fsdp_metrics)
+            print(resume_training_fsdp_metrics)
+            # self.assertEqual(training_fsdp_metrics["eval_loss"], resume_training_fsdp_metrics["eval_loss"])
+            # self.assertEqual(training_fsdp_metrics["eval_accuracy"], resume_training_fsdp_metrics["eval_accuracy"])
+
+            output_3 = Path(tmpdirname) / "out_3"
+
+            cmd = [
+                "torchrun",
+                "--nproc_per_node=2",
+                "examples/text-classification/run_glue.py",
+                f"--model_name_or_path={model_name}",
+                f"--task_name={task_name}",
+                "--per_device_train_batch_size=16",
+                "--per_device_eval_batch_size=16",
+                f"--output_dir={output_3}",
+                "--save_strategy=steps",
+                "--save_steps=10",
+                "--max_steps=100",
+                "--do_train",
+                # "--do_eval",
+                "--bf16",
+                f"--fsdp={fsdp_mode}",
+            ]
+
+            proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            stdout, stderr = proc.communicate()
+
+            regular_training_metrics = {}
+            with open(output_3 / "all_results.json") as fp:
+                regular_training_metrics = json.load(fp)
+
+            self.assertEqual(training_fsdp_metrics["train_loss"], regular_training_metrics["train_loss"])
+            # self.assertEqual(training_fsdp_metrics["eval_loss"], regular_training_metrics["eval_loss"])
+            # self.assertEqual(training_fsdp_metrics["eval_accuracy"], regular_training_metrics["eval_accuracy"])
+
+    def test_training_with_fsdp_full_shard(self):
+        return self._test_training_with_fsdp_mode("full_shard")
+
+    # def test_training_with_fsdp_shard_grad_op(self):
+    #     return self._test_training_with_fsdp_mode("shard_grad_op")
+
+    def test_training_with_fsdp_no_shard(self):
+        return self._test_training_with_fsdp_mode("no_shard")
+
+    # def test_training_with_fsdp_offload(self):
+    #     return self._test_training_with_fsdp_mode("offload")
+
+    # def test_training_with_fsdp_auto_wrap(self):
+    #     return self._test_training_with_fsdp_mode("auto_wrap")
```

### Comparing `optimum-neuron-0.0.4/tests/test_utils.py` & `optimum-neuron-0.0.5/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
+# limitations under the License.
 """Tests for utility functions and classes."""
 
 from typing import Dict, Literal, Union
 from unittest import TestCase
 
 import torch
 from torch.utils.data import DataLoader, Dataset, IterableDataset
 from transformers import BertConfig, BertForSequenceClassification, PreTrainedModel, Wav2Vec2Config, Wav2Vec2Model
 
-from optimum.neuron.utils.training_utils import FirstAndLastDataset, is_model_officially_supported, patch_model
+from optimum.neuron.trainers import MODEL_PATCHING_SPECS
+from optimum.neuron.utils import ModelPatcher
+from optimum.neuron.utils.testing_utils import is_trainium_test
+from optimum.neuron.utils.training_utils import FirstAndLastDataset, is_model_officially_supported
 
 
+@is_trainium_test
 def test_is_model_officially_supported():
     class DummyModelClass(PreTrainedModel):
         pass
 
     unsupported_model = DummyModelClass(BertConfig())
     assert is_model_officially_supported(unsupported_model) is False
 
@@ -157,24 +162,30 @@
             world_size=world_size,
         )
         self.assertEqual(len(first_and_last) / (gradient_accumulation_steps * world_size), num_repeat)
 
 
 def test_patch_model():
     bert_model = BertForSequenceClassification(BertConfig())
-    patch_model(bert_model)
-    assert getattr(bert_model.config, "layerdrop", None) is None
-
-    # Checking that the context manager exists.
-    with bert_model.no_sync():
-        pass
+    patching_specs = []
+    for spec in MODEL_PATCHING_SPECS:
+        patching_specs.append((bert_model,) + spec)
+
+    with ModelPatcher(patching_specs, ignore_missing_attributes=True):
+        assert getattr(bert_model.config, "layerdrop", None) == 0
+        # Checking that the context manager exists.
+        with bert_model.no_sync():
+            pass
 
     wav2vec2_model = Wav2Vec2Model(Wav2Vec2Config())
     assert (
         wav2vec2_model.config.layerdrop > 0
     ), "Default Wav2vec2Config layerdrop value is already 0 so the test will not check anything."
-    patch_model(wav2vec2_model)
-    assert wav2vec2_model.config.layerdrop == 0, "layerdrop was not patched properly."
-
-    # Checking that the context manager exists.
-    with wav2vec2_model.no_sync():
-        pass
+    patching_specs = []
+    for spec in MODEL_PATCHING_SPECS:
+        patching_specs.append((wav2vec2_model,) + spec)
+    with ModelPatcher(patching_specs, ignore_missing_attributes=True):
+        assert wav2vec2_model.config.layerdrop == 0, "layerdrop was not patched properly."
+
+        # Checking that the context manager exists.
+        with wav2vec2_model.no_sync():
+            pass
```

