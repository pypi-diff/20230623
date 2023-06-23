# Comparing `tmp/finetuning-scheduler-2.0.2.tar.gz` & `tmp/finetuning-scheduler-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuning-scheduler-2.0.2.tar", last modified: Thu Apr  6 21:15:19 2023, max compression
+gzip compressed data, was "finetuning-scheduler-2.0.4.tar", last modified: Fri Jun 23 00:14:14 2023, max compression
```

## Comparing `finetuning-scheduler-2.0.2.tar` & `finetuning-scheduler-2.0.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.472727 finetuning-scheduler-2.0.2/.actions/
--rw-r--r--   0 runner    (1001) docker     (122)     6935 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (122)    14615 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11482 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11035 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.472727 finetuning-scheduler-2.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/cli.txt
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/examples.txt
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/extra.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/ipynb.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/standalone_base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     6919 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.468727 finetuning-scheduler-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.472727 finetuning-scheduler-2.0.2/src/finetuning_scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    49224 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/fts.py
--rw-r--r--   0 runner    (1001) docker     (122)   101936 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/fts_supporters.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/setup_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    40034 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11482 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-06 21:15:19.000000 finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/legacy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6933 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/cli_experiment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.468727 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_explicit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_implicit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/nofts_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6848 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/fts_fsdp_superglue.py
--rw-r--r--   0 runner    (1001) docker     (122)    17790 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/fts_superglue.py
--rw-r--r--   0 runner    (1001) docker     (122)    18350 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/legacy/patched_adamw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.476727 finetuning-scheduler-2.0.2/src/fts_examples/stable/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7788 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/cli_experiment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.468727 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_explicit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_implicit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/config/nofts_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/extended_profiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    15557 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/src/fts_examples/stable/fts_superglue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:15:19.480727 finetuning-scheduler-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)   108541 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/tests/test_finetuning_scheduler_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)    40054 2023-04-06 21:15:10.000000 finetuning-scheduler-2.0.2/tests/test_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (122)     6935 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14847 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11482 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11035 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/cli.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/ipynb.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/standalone_base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6919 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.876730 finetuning-scheduler-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/src/finetuning_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49378 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/fts.py
+-rw-r--r--   0 runner    (1001) docker     (122)   102498 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/fts_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/setup_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14897 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40090 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11482 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-23 00:14:14.000000 finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.880730 finetuning-scheduler-2.0.4/src/fts_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/legacy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6933 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/cli_experiment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.876730 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_explicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_implicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/nofts_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     6848 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/fts_fsdp_superglue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17790 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/fts_superglue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18350 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/legacy/patched_adamw.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/stable/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7788 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/cli_experiment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.876730 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.884730 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_explicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_implicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/config/nofts_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/extended_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15557 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/src/fts_examples/stable/fts_superglue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 00:14:14.888730 finetuning-scheduler-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)   108644 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/tests/test_finetuning_scheduler_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41486 2023-06-23 00:14:06.000000 finetuning-scheduler-2.0.4/tests/test_fsdp.py
```

### Comparing `finetuning-scheduler-2.0.2/.actions/assistant.py` & `finetuning-scheduler-2.0.4/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/CHANGELOG.md` & `finetuning-scheduler-2.0.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
+## [2.0.4] - 2023-06-22
+- Support for PyTorch Lightning 2.0.3 and 2.0.4
+- adjusted default example log name
+- disabled fsdp 1.x mixed precision tests temporarily until https://github.com/Lightning-AI/lightning/pull/17807 is merged
+
 ## [2.0.2] - 2023-04-06
 
 ### Added
 
 - Beta support for [optimizer reinitialization](https://finetuning-scheduler.readthedocs.io/en/stable/advanced/optimizer_reinitialization.html). Resolves [#6](https://github.com/speediedan/finetuning-scheduler/issues/6)
 - Use structural typing for Fine-Tuning Scheduler supported optimizers with ``ParamGroupAddable``
 - Support for ``jsonargparse`` version ``4.20.1``
```

### Comparing `finetuning-scheduler-2.0.2/CITATION.cff` & `finetuning-scheduler-2.0.4/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 message: "If you want to cite this extension, feel free to use this 😊"
 title: "Fine-Tuning Scheduler"
 abstract: "A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules."
 date-released: 2022-02-04
 authors:
   - family-names: "Dale"
     given-names: "Dan"
-version: 2.0.2
+version: 2.0.4
 identifiers:
   - description: "Fine-Tuning Scheduler (all versions)"
     type: doi
     value: 10.5281/zenodo.6463952
   - description: "Fine-Tuning Scheduler (v0.1.1)"
     type: doi
     value: 10.5281/zenodo.6463992
@@ -70,14 +70,17 @@
     value: 10.5281/zenodo.7734581
   - description: "Fine-Tuning Scheduler (v2.0.0)"
     type: doi
     value: 10.5281/zenodo.7738722
   - description: "Fine-Tuning Scheduler (v2.0.1)"
     type: doi
     value: 10.5281/zenodo.7803180
+  - description: "Fine-Tuning Scheduler (v2.0.2)"
+    type: doi
+    value: 10.5281/zenodo.7806830
 license: "Apache-2.0"
 url: "https://finetuning-scheduler.readthedocs.io/"
 repository-code: "https://github.com/speediedan/finetuning-scheduler"
 keywords:
   - machine learning
   - deep learning
   - artificial intelligence
```

### Comparing `finetuning-scheduler-2.0.2/LICENSE` & `finetuning-scheduler-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/MANIFEST.in` & `finetuning-scheduler-2.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/PKG-INFO` & `finetuning-scheduler-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuning-scheduler
-Version: 2.0.2
+Version: 2.0.4
 Summary: A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.
 Home-page: https://github.com/speediedan/finetuning-scheduler
 Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale
 Author-email: danny.dale@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/issues
@@ -33,39 +33,39 @@
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/_static/images/logos/logo_fts.png" width="401px">
+<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/_static/images/logos/logo_fts.png" width="401px">
 
 **A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://finetuning-scheduler.readthedocs.io/en/stable/">Docs</a> •
   <a href="#Setup">Setup</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-scheduler)](https://pypi.org/project/finetuning-scheduler/)
 [![PyPI Status](https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/finetuning-scheduler)\
-[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.0.2/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
+[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.0.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
 [![ReadTheDocs](https://readthedocs.org/projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-scheduler.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/455666112.svg)](https://zenodo.org/badge/latestdoi/455666112)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 
 </div>
 
 ______________________________________________________________________
 
-<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
+<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
 
 [FinetuningScheduler](https://finetuning-scheduler.readthedocs.io/en/stable/api/finetuning_scheduler.fts.html#finetuning_scheduler.fts.FinetuningScheduler) is simple to use yet powerful, offering a number of features that facilitate model research and exploration:
 
 - easy specification of flexible fine-tuning schedules with explicit or regex-based parameter selection
   - implicit schedules for initial/naive model exploration
   - explicit schedules for performance tuning, fine-grained behavioral experimentation and computational efficiency
 - automatic restoration of best per-phase checkpoints driven by iterative application of early-stopping criteria to each fine-tuning phase
@@ -132,18 +132,18 @@
 To ensure maximum stability, the latest Lightning patch release fully tested with Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning patch version greater than that currently in Fine-Tuning Scheduler's requirements.txt, it will likely work but you should install Fine-Tuning Scheduler from source and update the requirements.txt as desired.
 
 <details>
   <summary>Current build statuses for Fine-Tuning Scheduler </summary>
 
 | System / (PyTorch/Python ver) |                                                                                                         1.11/3.8                                                                                                         |                                                                                                              2.0.0/3.8, 2.0.0/3.10                                                                                                               |
 | :---------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
-|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.2)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.0.2) |
-|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.4)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.0.4) |
+|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 
 - \*\* tests run on two RTX 2070s
 
 </details>
 
 ## Community
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuning-scheduler Version: 2.0.2 Summary: A
+Metadata-Version: 2.1 Name: finetuning-scheduler Version: 2.0.4 Summary: A
 PyTorch Lightning extension that enhances model experimentation with flexible
 fine-tuning schedules. Home-page: https://github.com/speediedan/finetuning-
 scheduler Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale Author-email: danny.dale@gmail.com License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/
 issues Project-URL: Documentation, https://finetuning-scheduler.readthedocs.io/
 en/latest/ Project-URL: Source Code, https://github.com/speediedan/finetuning-
@@ -16,24 +16,24 @@
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: examples Provides-
 Extra: extra Provides-Extra: test Provides-Extra: ipynb Provides-Extra: cli
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE
-  [https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/
+  [https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/
     _static/images/logos/logo_fts.png] **A PyTorch Lightning extension that
      enhances model experimentation with flexible fine-tuning schedules.**
     ______________________________________________________________________
                    Docs â¢ Setup â¢ Examples â¢ Community
  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-
   scheduler)](https://pypi.org/project/finetuning-scheduler/) [![PyPI Status]
 (https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/
 finetuning-scheduler)\ [![codecov](https://codecov.io/gh/speediedan/finetuning-
-   scheduler/release/2.0.2/graph/badge.svg?flag=gpu)](https://codecov.io/gh/
+   scheduler/release/2.0.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/
    speediedan/finetuning-scheduler) [![ReadTheDocs](https://readthedocs.org/
    projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-
     scheduler.readthedocs.io/en/stable/) [![DOI](https://zenodo.org/badge/
    455666112.svg)](https://zenodo.org/badge/latestdoi/455666112) [![license]
     (https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
         github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 ______________________________________________________________________
@@ -99,33 +99,33 @@
 -------------------------------------------------------------------------------
 -----------------------------------------------: | :---------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------: | | Linux \[GPUs\*\*\] |
 - | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/
 _apis/build/status/Multi-
-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.2)](https://
+GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.4)](https://
 dev.azure.com/speediedan/finetuning-scheduler/_build/
-latest?definitionId=2&branchName=refs%2Ftags%2F2.0.2) | | Linux (Ubuntu 20.04)
+latest?definitionId=2&branchName=refs%2Ftags%2F2.0.4) | | Linux (Ubuntu 20.04)
 | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/
-workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/
+workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/
 finetuning-scheduler/actions/workflows/ci_test-full.yml) | [![Test](https://
 github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/
-badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/
+badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/
 actions/workflows/ci_test-full.yml) | | OSX (11) | [![Test](https://github.com/
 speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/
-badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/
+badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/
 actions/workflows/ci_test-full.yml) | [![Test](https://github.com/speediedan/
-finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)]
+finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)]
 (https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-
 full.yml) | | Windows (2022) | [![Test](https://github.com/speediedan/
-finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)]
+finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)]
 (https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-
 full.yml) | [![Test](https://github.com/speediedan/finetuning-scheduler/
-actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/
+actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/
 speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) | - \*\*
 tests run on two RTX 2070s  ## Community Fine-Tuning Scheduler is developed and
 maintained by the community in close communication with the [Lightning team]
 (https://pytorch-lightning.readthedocs.io/en/stable/governance.html). Thanks to
 everyone in the community for their tireless effort building and improving the
 immensely useful core Lightning project. PR's welcome! Please see the
 [contributing guidelines](https://finetuning-scheduler.readthedocs.io/en/
```

### Comparing `finetuning-scheduler-2.0.2/README.md` & `finetuning-scheduler-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/pyproject.toml` & `finetuning-scheduler-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/setup.py` & `finetuning-scheduler-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/__about__.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/__about__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 
 _this_year = time.strftime("%Y")
-__version__ = "2.0.2"
+__version__ = "2.0.4"
 __author__ = "Dan Dale"
 __author_email__ = "danny.dale@gmail.com"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2021-{_this_year}, {__author__}"
 __homepage__ = "https://github.com/speediedan/finetuning-scheduler"
 __docs_url__ = "https://finetuning-scheduler.readthedocs.io/en/latest/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/__init__.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/fts.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/fts.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,21 +316,21 @@
         assert self.pl_module.trainer is not None
         pre_reinit_state = self._save_pre_reinit_lr_state(self.pl_module.trainer)
         if not self._fts_state._resume_fit_from_ckpt:
             if self.restore_best:
                 self.restore_best_ckpt()
                 self.step_pg(
                     depth=self.curr_depth,
-                    optimizer=self.pl_module.trainer.optimizers[0],
+                    optimizer=self.pl_module.trainer.optimizers[0],  # type: ignore[arg-type]
                     pre_reinit_state=pre_reinit_state,
                 )
             else:
                 self.step_pg(
                     depth=self.curr_depth,
-                    optimizer=self.pl_module.trainer.optimizers[0],
+                    optimizer=self.pl_module.trainer.optimizers[0],  # type: ignore[arg-type]
                     depth_sync=False,
                     pre_reinit_state=pre_reinit_state,
                 )
         else:
             self.thaw_to_depth()
         if self.depth_remaining == 0 and not self.epoch_transitions_only:
             assert self.pl_module.trainer.early_stopping_callback is not None
@@ -470,15 +470,15 @@
         # if restarting across multiple depths, need to ensure we're restoring optimizer state appropriately
         # by resetting optimizer groups and allowing state dict to be reset commensurate w/ ckpt state
         for opt_idx, optimizer in enumerate(self.pl_module.trainer.optimizers):
             optimizer.param_groups = BaseFinetuning._apply_mapping_to_param_groups(
                 self._fts_state._fts_ckpt_metadata["best_ckpt_pgs"][opt_idx], dict(self.pl_module.named_parameters())
             )
             if self.strategy_adapter.using_sharded_optimizer:
-                ScheduleImplMixin._repartition_sharded_optim(optimizer)
+                ScheduleImplMixin._repartition_sharded_optim(optimizer)  # type: ignore[arg-type]
         # we're restoring everything but callbacks and loops, otherwise, checkpoint_connector.restore() could be used
         assert self.pl_module.trainer.checkpoint_callback is not None
         checkpoint_path = self.pl_module.trainer.checkpoint_callback.best_model_path  # type: ignore[attr-defined]
         self.pl_module.trainer._checkpoint_connector.resume_start(checkpoint_path=checkpoint_path)
         self.pl_module.trainer._checkpoint_connector.restore_datamodule()
         self.pl_module.trainer._checkpoint_connector.restore_model()
         # we need to override checkpoint_connector.restore_training_state() to bypass loop restoration
@@ -526,15 +526,15 @@
             strategy (Strategy): The PL :external+pl:class:`~lightning.pytorch.strategies.Strategy` context to use.
             decision (bool): The local process decision.
 
         Returns:
             bool: The reduced decision across all world processes.
         """
         decision = torch.tensor(int(decision), device=strategy.root_device)
-        decision = bool(strategy.reduce(decision, reduce_op=ReduceOp.SUM))
+        decision = bool(strategy.reduce(decision, reduce_op=ReduceOp.SUM))  # type:ignore[arg-type]
         return decision
 
     def _sync_es_state(self, trainer: "pl.Trainer") -> None:
         """Synchronize the :class:`~finetuning_scheduler.fts_supporters.FTSEarlyStopping` callback transition state
         across distributed processes to avoid rare transition divergences when the user does not set ``sync_dist``
         to ``True`` in logging the monitored metric.
 
@@ -794,15 +794,18 @@
             num_saved_groups = (
                 len(self._internal_optimizer_metadata[opt_idx]) if opt_idx in self._internal_optimizer_metadata else 0
             )
             current_param_groups = optimizer.param_groups
             self._store(pl_module, opt_idx, num_saved_groups, current_param_groups)
 
     def on_before_zero_grad(
-        self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", optimizer: ParamGroupAddable
+        self,
+        trainer: "pl.Trainer",
+        pl_module: "pl.LightningModule",
+        optimizer: ParamGroupAddable,  # type: ignore[override]
     ) -> None:
         """Afer the latest optimizer step, update the
         :attr:`~finetuning_scheduler.fts.FinetuningScheduler._fts_state`, incrementing the
         global fine-tuning steps taken
 
         Args:
             trainer (:external+pl:class:`~lightning.pytorch.trainer.trainer.Trainer`): The
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/fts_supporters.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/fts_supporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -937,15 +937,15 @@
         Args:
             trainer (pl.Trainer): The :external+pl:class:`~lightning.pytorch.trainer.trainer.Trainer` object.
 
         Returns:
             Tuple[Dict, List]: The lr state to restore from the current lr scheduler and the most recent `lr`s for
                 parameter groups associated with the current phases's optimizer.
         """
-        curr_lr_state = {}
+        curr_lr_state: Dict = {}
         if trainer.lr_scheduler_configs:
             curr_lr_state = deepcopy(trainer.lr_scheduler_configs[0].scheduler.state_dict())
         prev_optimizer_lrs = copy([group["lr"] for group in trainer.strategy.optimizers[0].param_groups])
         return curr_lr_state, prev_optimizer_lrs
 
     def reinit_optimizer(self, new_optimizer: Dict, trainer: pl.Trainer, init_params: List) -> ParamGroupAddable:
         """Reinitialize the optimizer, using a validated optimizer reinitialization configuration.
@@ -958,26 +958,28 @@
         Returns:
             ParamGroupAddable: A handle for the newly reinitialized optimizer.
         """
         optimizer_init = new_optimizer["optimizer_init"]
         prev_optim_repr = repr(trainer.strategy.optimizers[0])
         optimizer_class = self._import_reinit_class(optimizer_init, reinit_target="optimizer")
         reinit_pgs = self._reinit_phase0_pgs(thawed_pl=init_params)
-        new_optimizer_handle = optimizer_class(reinit_pgs, **optimizer_init.get("init_args", {}))
+        new_optimizer_handle = optimizer_class(
+            reinit_pgs, **optimizer_init.get("init_args", {})  # type: ignore[operator, arg-type]
+        )
         # If the user or optimizer doesn't set `initial_lr` keys, add them based on the initial lr values.
         # The latest LR state will still be set in subsequent phases, but this allows subsequent lr scheduler
         # reinitializations to access an `initial_lr` for the existing optimizer if desired (important for consistency
         # with lr scheduler-only reinitializations).
-        for group in new_optimizer_handle.param_groups:
+        for group in new_optimizer_handle.param_groups:  # type: ignore[union-attr]
             group["initial_lr"] = group.get("initial_lr", group["lr"])
-        trainer.strategy.optimizers = [new_optimizer_handle]
+        trainer.strategy.optimizers = [new_optimizer_handle]  # type: ignore[list-item]
         if trainer.lr_scheduler_configs:
             trainer.lr_scheduler_configs[0].scheduler.optimizer = new_optimizer_handle
         self._maybe_trace_reinit("optimizer", prev_optim_repr, repr(trainer.strategy.optimizers[0]))
-        return new_optimizer_handle
+        return new_optimizer_handle  # type:ignore[return-value]
 
     def reinit_lr_scheduler(self, new_lr_scheduler: Dict, trainer: pl.Trainer, optimizer: ParamGroupAddable) -> None:
         """Reinitialize the learning rate scheduler, using a validated learning rate scheduler configuration and
         wrapping the existing optimizer.
 
         Args:
             new_lr_scheduler (Dict): A dictionary defining the new lr scheduler configuration to be initialized.
@@ -1003,19 +1005,22 @@
         initial_optimizer_lrs = new_lr_scheduler.get("init_pg_lrs", curr_optimizer_lrs)
         for _, data in enumerate(zip(optimizer.param_groups, initial_optimizer_lrs)):
             param_group, lr = data
             param_group["lr"] = lr
             if reset_init_pg_lrs:
                 param_group["initial_lr"] = lr
         if "pl_lrs_cfg" in new_lr_scheduler.keys():
-            new_lr_scheduler["pl_lrs_cfg"] = self._update_pl_lrs(new_lr_scheduler["pl_lrs_cfg"], lrs_class=lrs_class)
+            new_lr_scheduler["pl_lrs_cfg"] = self._update_pl_lrs(
+                new_lr_scheduler["pl_lrs_cfg"], lrs_class=lrs_class  # type:ignore[arg-type]
+            )
+        assert callable(lrs_class)
         new_lrs_config = LRSchedulerConfig(
             scheduler=lrs_class(
-                optimizer=optimizer, **lr_scheduler_init.get("init_args", {})
-            ),  # type: ignore[arg-type]
+                optimizer=optimizer, **lr_scheduler_init.get("init_args", {})  # type: ignore[arg-type]
+            ),
             **new_lr_scheduler.get("pl_lrs_cfg", {}),
         )
         trainer.strategy.lr_scheduler_configs = [new_lrs_config]
         self._maybe_trace_reinit("lr scheduler", prev_lrs_repr, repr(trainer.lr_scheduler_configs[0]))
 
     def _maybe_trace_reinit(self, target_type: str, prev_repr: str, new_repr: str) -> None:
         """Trace valid optimizer and lr scheduler transitions (including intermediate restorations).
@@ -1086,15 +1091,15 @@
         Args:
             optim_class (ParamGroupAddable): The optimizer class to be inspected for support.
 
         Raises:
             MisconfigurationException: If the provided optimizer class is known to be currently unsupported in the
                 context of optimizer reinitialization.
         """
-        if issubclass(optim_class, ZeroRedundancyOptimizer):
+        if issubclass(optim_class, ZeroRedundancyOptimizer):  # type: ignore[arg-type]
             error_msg = (
                 f"The provided optimizer ({optim_class}) is not currently supported by FinetuningScheduler in the"
                 " context of optimizer reinitialization. Please use a currently supported torch optimizer (or subclass"
                 " thereof) from those provided in `torch.optim`: https://pytorch.org/docs/stable/optim.html#algorithms."
             )
             rank_zero_warn(error_msg)
             raise MisconfigurationException(error_msg)
@@ -1111,14 +1116,15 @@
 
         Raises:
             MisconfigurationException: If the specified class cannot be imported successfully.
 
         Returns:
             Union[FTSLRSchedulerType, ParamGroupAddable]: The class to reinitialize.
         """
+        # TODO: refactor this function to enable type narrowing while continuing to share relevant code paths
         try:
             class_module, class_name = reinit_cfg["class_path"].rsplit(".", 1)
             module = __import__(class_module, fromlist=[class_name])
             reinit_class = getattr(module, class_name)
             if reinit_target == "lr_scheduler":
                 self._is_supported_lr(reinit_class)
         except (ImportError, AttributeError) as err:
@@ -1179,15 +1185,18 @@
             MisconfigurationException: If a valid and supported scheduler cannot be instantiated with the specified
                 init args.
         """
         optimizer_class = self._import_reinit_class(optimizer_init, reinit_target="optimizer")
         self._is_supported_reinit_optimizer(optimizer_class)
         test_optimizer_init = copy(optimizer_init.get("init_args", {}))
         try:
-            test_optimizer = optimizer_class(ScheduleParsingMixin.SANITY_CHK_ITERABLE, **test_optimizer_init)
+            assert callable(optimizer_class)
+            test_optimizer = optimizer_class(
+                ScheduleParsingMixin.SANITY_CHK_ITERABLE, **test_optimizer_init  # type: ignore[arg-type]
+            )
         except Exception as err:
             error_msg = (
                 "Could not configure the specified optimizer class using the `init_args` "
                 f"({optimizer_init['init_args']}). Recieved the following error while sanity checking schedule "
                 f"phases: {err}. Please validate specified `init_args` before resubmitting."
             )
             rank_zero_warn(error_msg)
@@ -1217,25 +1226,28 @@
             )
             rank_zero_warn(warn_msg)
             del lr_scheduler_init["init_args"]["optimizer"]
         min_lr_param = lr_scheduler_init["init_args"].get("min_lr")
         invalid_min_lr = (
             True if min_lr_param and (isinstance(min_lr_param, list) or isinstance(min_lr_param, tuple)) else False
         )
-        reinit_rlrop = is_implicit_mode and issubclass(lrs_class, torch.optim.lr_scheduler.ReduceLROnPlateau)
+        reinit_rlrop = is_implicit_mode and issubclass(
+            lrs_class, torch.optim.lr_scheduler.ReduceLROnPlateau  # type: ignore[arg-type]
+        )
         if reinit_rlrop and invalid_min_lr:
             raise MisconfigurationException(
                 "In the lr scheduler configuration passed via `reinit_lr_cfg` (i.e. implicit mode training)"
                 " `min_lr` cannot be a list or tuple since the same lr scheduler configuration is intended to be"
                 " reinitialized at every fine-tuning phase with implicit mode fine-tuning."
             )
         test_lr_init = copy(lr_scheduler_init.get("init_args", {}))
         if min_lr_param:
             del test_lr_init["min_lr"]  # our mock optimizer will not have any param groups
         try:
+            assert callable(lrs_class)
             testlr = lrs_class(optimizer=_MockOptimizer(), **test_lr_init)
         except Exception as err:
             error_msg = (
                 "Could not configure the specified LR scheduler class using the `init_args` "
                 f"({lr_scheduler_init['init_args']}). Recieved the following error while sanity checking schedule "
                 f"phases: {err}. Please validate specified `init_args` before resubmitting."
             )
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/setup_tools.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/setup_tools.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/__init__.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/base.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                 currently supported by FTS, this list will have only a single element in this verison.)
         """
         orig_num_pgs = []
         for optimizer in trainer.optimizers:
             orig_num_pgs.append(len(optimizer.param_groups))
             optimizer.param_groups = []
         for lrs_cfg in trainer.lr_scheduler_configs:
-            lrs_cfg.scheduler.last_epoch = -1
+            lrs_cfg.scheduler.last_epoch = -1  # type: ignore[union-attr]
             if not isinstance(lrs_cfg.scheduler, ReduceLROnPlateau):
                 lrs_cfg.scheduler.base_lrs = []
         return orig_num_pgs
 
     def _reconfigure_optimizer_for_phase0(self, trainer: Trainer) -> None:
         """Reconfigure optimizer state to comport with the scheduled phase 0.
 
@@ -211,15 +211,17 @@
         """
         # since we may have added parameter groups (e.g. implementing ``no_decay`` for user), we need to reinitialize
         # certain lr_scheduler variables (including type-dependent ones like ``min_lrs`` and ``lr_lambdas``)
         if trainer.lr_scheduler_configs:
             for lrs_cfg in trainer.lr_scheduler_configs:
                 if _TORCH_GREATER_EQUAL_1_13 and not isinstance(lrs_cfg.scheduler, ReduceLROnPlateau):
                     lrs_cfg.scheduler._initial_step()
-                lrs_cfg.scheduler._last_lr = [group["lr"] for group in lrs_cfg.scheduler.optimizer.param_groups]
+                lrs_cfg.scheduler._last_lr = [  # type: ignore[union-attr]
+                    group["lr"] for group in lrs_cfg.scheduler.optimizer.param_groups
+                ]
                 if isinstance(lrs_cfg.scheduler, ReduceLROnPlateau):
                     lrs_cfg.scheduler.min_lrs = lrs_cfg.scheduler.min_lrs[orig_num_pgs[0] :]
                 elif hasattr(lrs_cfg.scheduler, "lr_lambdas"):
                     lrs_cfg.scheduler.lr_lambdas = lrs_cfg.scheduler.lr_lambdas[orig_num_pgs[0] :]
 
     def phase0_optimizer_override(self) -> None:
         """Reconfigure the user-configured optimizer (configured via `configure_optimizers`) to optimize the
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/strategy_adapters/fsdp.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/strategy_adapters/fsdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,17 @@
         """
         with self._enable_name_based_overrides():
             for n, m in self.pl_module.named_children():
                 setattr(self.pl_module, n, wrap(m))
 
         # apply wrappers to enable activation checkpointing if requested
         if self.pls_handle._activation_checkpointing:
-            _setup_activation_checkpointing(module=self.pl_module, layers=self.pls_handle._activation_checkpointing)
+            _setup_activation_checkpointing(
+                module=self.pl_module, layers=self.pls_handle._activation_checkpointing  # type: ignore[arg-type]
+            )
 
     def _after_configure_sharded_model(self) -> None:
         """Generate the parameter-level bi-directional translations the FTS FSDP adapter requires and then execute
         the previously deferred first fine-tuning phase."""
         assert isinstance(self.fts_handle.ft_schedule, Dict)  # TODO: move/consolidate ft_schedule assertions
         self._init_fsdp_param_map()
         _, self.fts_handle._fts_state._curr_thawed_params = self.exec_ft_phase(
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler/types.py` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler/types.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/PKG-INFO` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuning-scheduler
-Version: 2.0.2
+Version: 2.0.4
 Summary: A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.
 Home-page: https://github.com/speediedan/finetuning-scheduler
 Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale
 Author-email: danny.dale@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/issues
@@ -33,39 +33,39 @@
 Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/_static/images/logos/logo_fts.png" width="401px">
+<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/_static/images/logos/logo_fts.png" width="401px">
 
 **A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://finetuning-scheduler.readthedocs.io/en/stable/">Docs</a> •
   <a href="#Setup">Setup</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-scheduler)](https://pypi.org/project/finetuning-scheduler/)
 [![PyPI Status](https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/finetuning-scheduler)\
-[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.0.2/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
+[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.0.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
 [![ReadTheDocs](https://readthedocs.org/projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-scheduler.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/455666112.svg)](https://zenodo.org/badge/latestdoi/455666112)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 
 </div>
 
 ______________________________________________________________________
 
-<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
+<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
 
 [FinetuningScheduler](https://finetuning-scheduler.readthedocs.io/en/stable/api/finetuning_scheduler.fts.html#finetuning_scheduler.fts.FinetuningScheduler) is simple to use yet powerful, offering a number of features that facilitate model research and exploration:
 
 - easy specification of flexible fine-tuning schedules with explicit or regex-based parameter selection
   - implicit schedules for initial/naive model exploration
   - explicit schedules for performance tuning, fine-grained behavioral experimentation and computational efficiency
 - automatic restoration of best per-phase checkpoints driven by iterative application of early-stopping criteria to each fine-tuning phase
@@ -132,18 +132,18 @@
 To ensure maximum stability, the latest Lightning patch release fully tested with Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning patch version greater than that currently in Fine-Tuning Scheduler's requirements.txt, it will likely work but you should install Fine-Tuning Scheduler from source and update the requirements.txt as desired.
 
 <details>
   <summary>Current build statuses for Fine-Tuning Scheduler </summary>
 
 | System / (PyTorch/Python ver) |                                                                                                         1.11/3.8                                                                                                         |                                                                                                              2.0.0/3.8, 2.0.0/3.10                                                                                                               |
 | :---------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
-|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.2)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.0.2) |
-|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.4)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.0.4) |
+|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 
 - \*\* tests run on two RTX 2070s
 
 </details>
 
 ## Community
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuning-scheduler Version: 2.0.2 Summary: A
+Metadata-Version: 2.1 Name: finetuning-scheduler Version: 2.0.4 Summary: A
 PyTorch Lightning extension that enhances model experimentation with flexible
 fine-tuning schedules. Home-page: https://github.com/speediedan/finetuning-
 scheduler Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale Author-email: danny.dale@gmail.com License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/
 issues Project-URL: Documentation, https://finetuning-scheduler.readthedocs.io/
 en/latest/ Project-URL: Source Code, https://github.com/speediedan/finetuning-
@@ -16,24 +16,24 @@
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: examples Provides-
 Extra: extra Provides-Extra: test Provides-Extra: ipynb Provides-Extra: cli
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE
-  [https://github.com/speediedan/finetuning-scheduler/raw/v2.0.2/docs/source/
+  [https://github.com/speediedan/finetuning-scheduler/raw/v2.0.4/docs/source/
     _static/images/logos/logo_fts.png] **A PyTorch Lightning extension that
      enhances model experimentation with flexible fine-tuning schedules.**
     ______________________________________________________________________
                    Docs â¢ Setup â¢ Examples â¢ Community
  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-
   scheduler)](https://pypi.org/project/finetuning-scheduler/) [![PyPI Status]
 (https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/
 finetuning-scheduler)\ [![codecov](https://codecov.io/gh/speediedan/finetuning-
-   scheduler/release/2.0.2/graph/badge.svg?flag=gpu)](https://codecov.io/gh/
+   scheduler/release/2.0.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/
    speediedan/finetuning-scheduler) [![ReadTheDocs](https://readthedocs.org/
    projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-
     scheduler.readthedocs.io/en/stable/) [![DOI](https://zenodo.org/badge/
    455666112.svg)](https://zenodo.org/badge/latestdoi/455666112) [![license]
     (https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
         github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 ______________________________________________________________________
@@ -99,33 +99,33 @@
 -------------------------------------------------------------------------------
 -----------------------------------------------: | :---------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------: | | Linux \[GPUs\*\*\] |
 - | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/
 _apis/build/status/Multi-
-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.2)](https://
+GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.0.4)](https://
 dev.azure.com/speediedan/finetuning-scheduler/_build/
-latest?definitionId=2&branchName=refs%2Ftags%2F2.0.2) | | Linux (Ubuntu 20.04)
+latest?definitionId=2&branchName=refs%2Ftags%2F2.0.4) | | Linux (Ubuntu 20.04)
 | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/
-workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/speediedan/
+workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/speediedan/
 finetuning-scheduler/actions/workflows/ci_test-full.yml) | [![Test](https://
 github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/
-badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/
+badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/
 actions/workflows/ci_test-full.yml) | | OSX (11) | [![Test](https://github.com/
 speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/
-badge.svg?tag=2.0.2)](https://github.com/speediedan/finetuning-scheduler/
+badge.svg?tag=2.0.4)](https://github.com/speediedan/finetuning-scheduler/
 actions/workflows/ci_test-full.yml) | [![Test](https://github.com/speediedan/
-finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)]
+finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)]
 (https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-
 full.yml) | | Windows (2022) | [![Test](https://github.com/speediedan/
-finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)]
+finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)]
 (https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-
 full.yml) | [![Test](https://github.com/speediedan/finetuning-scheduler/
-actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.2)](https://github.com/
+actions/workflows/ci_test-full.yml/badge.svg?tag=2.0.4)](https://github.com/
 speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) | - \*\*
 tests run on two RTX 2070s  ## Community Fine-Tuning Scheduler is developed and
 maintained by the community in close communication with the [Lightning team]
 (https://pytorch-lightning.readthedocs.io/en/stable/governance.html). Thanks to
 everyone in the community for their tireless effort building and improving the
 immensely useful core Lightning project. PR's welcome! Please see the
 [contributing guidelines](https://finetuning-scheduler.readthedocs.io/en/
```

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/SOURCES.txt` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/finetuning_scheduler.egg-info/requires.txt` & `finetuning-scheduler-2.0.4/src/finetuning_scheduler.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightning<2.0.2,>=2.0.0
+lightning<2.0.5,>=2.0.0
 torch>=1.11.0
 
 [all]
 rich!=10.15.0.a,>=10.14.0
 jsonargparse[signatures]!=4.18.0,!=4.19.0,!=4.20.0,>=4.15.2
 omegaconf>=2.1.0
 hydra-core>=1.1.0
```

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/cli_experiment_utils.py` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/cli_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/explicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_defaults.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_defaults.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_explicit.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_explicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/config/fts_implicit.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/config/fts_implicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/fts_fsdp_superglue.py` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/fts_fsdp_superglue.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/fts_superglue.py` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/fts_superglue.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/legacy/patched_adamw.py` & `finetuning-scheduler-2.0.4/src/fts_examples/legacy/patched_adamw.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/cli_experiment_utils.py` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/cli_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_defaults.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_defaults.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -32,7 +32,8 @@
   accelerator: gpu
   strategy: ddp_find_unused_parameters_false
   precision: 16-mixed
   logger:
     class_path: lightning.pytorch.loggers.TensorBoardLogger
     init_args:
       save_dir: lightning_logs
+      name: fts_default
```

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_explicit.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_explicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/config/fts_implicit.yaml` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/config/fts_implicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/extended_profiler.py` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/extended_profiler.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/src/fts_examples/stable/fts_superglue.py` & `finetuning-scheduler-2.0.4/src/fts_examples/stable/fts_superglue.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.0.2/tests/test_finetuning_scheduler_callback.py` & `finetuning-scheduler-2.0.4/tests/test_finetuning_scheduler_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1210,14 +1210,15 @@
     "does not have many workers",
     "GPU available but",
     "`max_epochs` was not",
     "that ended mid-epoch",
     "The dirpath has changed from",
     "Torchmetrics v0.9",  # temporarily allow until _ResultMetric updated
     "distutils Version classes are deprecated",  # temporarily allow until PL utilities/migration/utils.py updated
+    "Conversion of an array with ndim > 0 to",  # warning caused by deprecated behavior of tensorboard
 ]
 EXPECTED_TRAIN_CHK_WARNS = ["could not find the monitored key", "callbacks used to create"]
 EXPECTED_DIRPATH = "exists and is not empty"
 
 
 @pytest.mark.parametrize("diff_dirpath,", [True, False], ids=["diffdirpath", "samedirpath"])
 @pytest.mark.parametrize("train_chk_mode,", [None, True], ids=["defaultchk", "trainchk"])
```

### Comparing `finetuning-scheduler-2.0.2/tests/test_fsdp.py` & `finetuning-scheduler-2.0.4/tests/test_fsdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "The distutils package is deprecated",  # for tensorboard (but not tensorboardX) import as of PT 1.13.1
     "`tensorboardX` has been removed as a depend",  # in case tensorboard/tensorboardX are not available
     "is still running",  # subprocess is implicitly cleaned up
     "Please use torch.distributed.all_gather_into_tensor",  # can be removed once PyTorch stops using internally,
     "Please use torch.distributed.reduce_scatter_tensor",  # can be removed once PyTorch stops using internally,
     "when logging on epoch level in distributed",  # validating FTS handling in this scenario
     "Deallocating Tensor that still has live",  # TODO: investigate the occasional occurance of this warning
+    "Conversion of an array with ndim > 0 to",  # warning caused by deprecated behavior of tensorboard
 ]
 EXPECTED_WARNS.extend(additional_fsdp_warns)
 FSDP_BASE_WARNS = EXPECTED_WARNS
 FSDP_DYNAMO_EXPECTED_WARNS = [
     "Final phase max_transition_epoch",
     "Your compiler for AOTAutograd is returning",  # out of initial scope
 ]
@@ -276,30 +277,33 @@
     def _assert_layer_fsdp_instance(self) -> None:
         if self.outer_is_wrapped:
             assert isinstance(self.layer, FullyShardedDataParallel)
         else:
             assert isinstance(self.layer, torch.nn.Sequential)
         if self.precision_key == "auto_16":
             assert isinstance(self.trainer.strategy.precision_plugin, FSDPMixedPrecisionPlugin)
-            precision = torch.float16 if self.trainer.precision == "16-mixed" else torch.bfloat16
+            # TODO: hack, fully test new mp semantics once https://github.com/Lightning-AI/lightning/pull/17807 merged
+            reduce_dtype = buffer_dtype = param_dtype = torch.float16
+            if self.trainer.precision == "16-mixed":
+                param_dtype = torch.float32
         # ensure our ignored module is not wrapped
         for i in self.fsdp_mask["unwrapped_mods"]:
             assert not isinstance(self.layer[i], FullyShardedDataParallel)
         # but that all other modules are wrapped
         for i in self.fsdp_mask["wrapped_mods"]:
             assert isinstance(self.layer[i], FullyShardedDataParallel)
             if self.precision_key:
                 if isinstance(self.layer[i].module, torch.nn.modules.batchnorm._BatchNorm):
                     assert self.layer[i].mixed_precision.param_dtype is None
                     assert self.layer[i].mixed_precision.reduce_dtype is None
                     assert self.layer[i].mixed_precision.buffer_dtype is None
                 else:
-                    assert self.layer[i].mixed_precision.param_dtype == precision
-                    assert self.layer[i].mixed_precision.reduce_dtype == precision
-                    assert self.layer[i].mixed_precision.buffer_dtype == precision
+                    assert self.layer[i].mixed_precision.param_dtype == param_dtype
+                    assert self.layer[i].mixed_precision.reduce_dtype == reduce_dtype
+                    assert self.layer[i].mixed_precision.buffer_dtype == buffer_dtype
 
 
 class NonDynamicLossAdamFSDPModel(FTSBaseFSDPModel):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def val_loss(self, batch, prediction):
@@ -595,14 +599,15 @@
 path_optimlr_reinit = {0: (2, 4, "SGD", 0, 0.1), 1: (6, 12, "Adam", 32, 0.00021), 2: (7, 14, "SGD", 64, 0.002)}
 lrs_path_default = {0: (0.1,), 1: (0.07, 1e-06), 2: (0.049, 7e-07, 1e-05)}
 lrs_path_optimlr_reinit = {0: (0.1,), 1: (0.00021, 1e-06), 2: (0.002, 1e-06, 3e-06)}
 
 
 EXPECTED_FSDP_FTS_RESULTS = {
     "cust_awp_noprec": (path_default, *nones(3)),
+    "cust_awp_noprec_pt1x": (path_default, *nones(3)),
     "cust_awp_noprec_use_orig": (path_default_orig, *nones(3)),
     "cust_awp_noprec_dynamo_use_orig": (path_default_orig_eo_dyn, *nones(3)),
     "cust_awp_mwp_reinitlr_optim": (path_optimlr_reinit, ("Incompatible check",), None, lrs_path_optimlr_reinit),
     "cust_awp_mwp_parity": (path_default, *nones(3)),
     "override_csm_noprec": (path_default, *nones(3)),
     # TODO: once PyTorch deprecates ``ignored_modules``, check for that deprecation warning in this test
     "cust_awp_nop_ignore_m_no_ofld": (path_8_14, *nones(3)),
@@ -612,15 +617,15 @@
     "non_disjoint_phase_mods": ({}, None, "not have disjoint", None),
     "non_disjoint_excluded_ft_params": ({}, None, "parameters not included in", None),
     "already_fsdp_wrapped": ({}, None, "already wrapped by FSDP", None),
     "no_fsdp_params_p0": ({}, None, "one or more FSDP", None),
     "warn_unsupp_nodecay": ({}, "will now be unset", *nones(2)),
     "unmatched_awp_overrides": ({}, None, "did not match any named modules", None),
     "cust_awp_prec": (path_default, *nones(3)),
-    "cust_awp_prec_pt1x": (path_default, *nones(3)),
+    # "cust_awp_prec_pt1x": (path_default, *nones(3)),
     "enforceP0_cust_awp_prec": (path_default, *nones(3)),
     # "batch_norm_auto_prec": (path_8_16, "Both mixed precision", None),  # _dynamo/allowed_functions.py suppresses
     "batch_norm_auto_prec": (path_8_16, *nones(3)),
     "shared_params_auto_prec": (path_5_10, ("Pruning explicitly specified",), *nones(2)),
     "override_csm_adam_noprec": (path_ext_7_14, *nones(3)),
     "cust_awp_overrides_prec": (path_default, *nones(3)),
     "cust_awp_overrides_prec_ext": (path_ext_8_16, *nones(3)),
@@ -632,14 +637,17 @@
 @RunIf(min_cuda_gpus=2, skip_windows=True, standalone=True, min_torch="1.13")
 @pytest.mark.parametrize(
     "model_cfg_key, model_cls, auto_wrap_policy, use_precision, ft_sched_idx, model_cfg, strategy_adapter_cfg, fts_cfg,\
           trainer_cfg, strategy_cfg",
     [
         ("cust_awp_noprec", base_model, cust_awp, False, 0, unwrap_7, *nones(3), act_ckpt_cfg),
         pytest.param(
+            "cust_awp_noprec_pt1x", base_model, cust_awp, False, 0, unwrap_7, *nones(4), marks=RunIf(max_torch="2.0.0")
+        ),
+        pytest.param(
             "cust_awp_noprec_use_orig",
             base_model,
             cust_awp,
             False,
             0,
             unwrap_7,
             *nones(3),
@@ -706,31 +714,84 @@
             0,
             unwrap_7,
             *nones(4),
             marks=RunIf(min_torch="2.0.0"),
         ),
         ("no_fsdp_params_p0", cust_model, None, False, 0, unwrap_5_7, *nones(4)),
         ("warn_unsupp_nodecay", nodecay_model, cust_awp, False, 0, unwrap_7, *nones(4)),
-        ("unmatched_awp_overrides", base_model, warn_cust_awp, True, 0, wrap_5_7, awp_5_9, *nones(3)),
-        ("cust_awp_prec", base_model, cust_awp, True, 0, unwrap_7_mp, *nones(4)),
         pytest.param(
-            "cust_awp_prec_pt1x", base_model, cust_awp, True, 0, unwrap_7_mp, *nones(4), marks=RunIf(max_torch="2.0.0")
+            "unmatched_awp_overrides",
+            base_model,
+            warn_cust_awp,
+            True,
+            0,
+            wrap_5_7,
+            awp_5_9,
+            *nones(3),
+            marks=RunIf(min_torch="2.0.0"),
+        ),
+        pytest.param(
+            "cust_awp_prec", base_model, cust_awp, True, 0, unwrap_7_mp, *nones(4), marks=RunIf(min_torch="2.0.0")
+        ),
+        # pytest.param(
+        #     "cust_awp_prec_pt1x", base_model, cust_awp, True, 0, unwrap_7_mp, *nones(4),
+        #     marks=RunIf(max_torch="2.0.0")
+        # ),
+        pytest.param(
+            "enforceP0_cust_awp_prec",
+            enforceP0_model,
+            cust_awp,
+            True,
+            0,
+            unwrap_7_mp,
+            *nones(4),
+            marks=RunIf(min_torch="2.0.0"),
         ),
-        ("enforceP0_cust_awp_prec", enforceP0_model, cust_awp, True, 0, unwrap_7_mp, *nones(4)),
         pytest.param(
             "batch_norm_auto_prec", BN_model, cust_awp, True, 2, unwrap_8_mp, *nones(4), marks=RunIf(min_torch="2.0.0")
         ),
-        ("shared_params_auto_prec", shared_model, cust_awp, True, 3, unwrap_7_mp, awp_1, *nones(3)),
+        pytest.param(
+            "shared_params_auto_prec",
+            shared_model,
+            cust_awp,
+            True,
+            3,
+            unwrap_7_mp,
+            awp_1,
+            *nones(3),
+            marks=RunIf(min_torch="2.0.0"),
+        ),
         ("override_csm_adam_noprec", csm_adam_model, None, False, 4, unwrap_7_diverge, *nones(2), max_epoch_5, None),
-        ("cust_awp_overrides_prec", base_model, cust_awp, True, 0, wrap_all_mp, awp_7, *nones(3)),
-        ("cust_awp_overrides_prec_ext", ext_model, cust_ext_awp, True, 6, wrap_ext_mp, awp_7_8, *nones(3)),
+        pytest.param(
+            "cust_awp_overrides_prec",
+            base_model,
+            cust_awp,
+            True,
+            0,
+            wrap_all_mp,
+            awp_7,
+            *nones(3),
+            marks=RunIf(min_torch="2.0.0"),
+        ),
+        pytest.param(
+            "cust_awp_overrides_prec_ext",
+            ext_model,
+            cust_ext_awp,
+            True,
+            6,
+            wrap_ext_mp,
+            awp_7_8,
+            *nones(3),
+            marks=RunIf(min_torch="2.0.0"),
+        ),
         ("warn_ignore_awp_override", cust_model, None, False, 0, unwrap_7, awp_7, *nones(3)),
     ],
     ids=[
         "cust_awp_noprec",
+        "cust_awp_noprec_pt1x",
         "cust_awp_noprec_use_orig",
         "cust_awp_noprec_dynamo_use_orig",
         "cust_awp_mwp_reinitlr_optim",
         "cust_awp_mwp_parity",
         "override_csm_noprec",
         "cust_awp_nop_ignore_m_no_ofld",
         "cust_awp_nop_ignore_p_no_ofld_uo",
@@ -739,15 +800,15 @@
         "non_disjoint_phase_mods",
         "non_disjoint_excluded_ft_params",
         "already_fsdp_wrapped",
         "no_fsdp_params_p0",
         "warn_unsupp_nodecay",
         "unmatched_awp_overrides",
         "cust_awp_prec",
-        "cust_awp_prec_pt1x",
+        # "cust_awp_prec_pt1x",
         "enforceP0_cust_awp_prec",
         "batch_norm_auto_prec",
         "shared_params_auto_prec",
         "override_csm_adam_noprec",
         "cust_awp_overrides_prec",
         "cust_awp_overrides_prec_ext",
         "warn_ignore_awp_override",
```

