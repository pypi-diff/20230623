# Comparing `tmp/macq-0.3.4.tar.gz` & `tmp/macq-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macq-0.3.4.tar", last modified: Fri Jun 23 02:52:04 2023, max compression
+gzip compressed data, was "macq-0.3.5.tar", last modified: Fri Jun 23 04:04:24 2023, max compression
```

## Comparing `macq-0.3.4.tar` & `macq-0.3.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 02:51:43.000000 macq-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 02:52:04.061415 macq-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 02:51:43.000000 macq-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.053415 macq-0.3.4/macq/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 02:51:43.000000 macq-0.3.4/macq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/amdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/arms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/learned_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/learned_fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    34948 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/locm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/slaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/generate/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/fd_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/planning_domains_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/random_goal_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/trace_from_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/vanilla_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/observation/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/action_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/atomic_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/id_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/identity_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_partial_disordered_parallel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/observed_tracelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/partial_observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/trace/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/disordered_parallel_actions_observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/partial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/trace_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/macq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/common_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/complex_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/tokenization_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/trace_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/trace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.053415 macq-0.3.4/macq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 02:51:43.000000 macq-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 02:52:04.061415 macq-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-23 02:51:43.000000 macq-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-23 02:51:43.000000 macq-0.3.4/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.668473 macq-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 04:04:05.000000 macq-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 04:04:24.668473 macq-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 04:04:05.000000 macq-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.656473 macq-0.3.5/macq/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 04:04:06.000000 macq-0.3.5/macq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.660473 macq-0.3.5/macq/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/amdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/learned_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/learned_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34948 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/locm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-23 04:04:06.000000 macq-0.3.5/macq/extract/slaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.660473 macq-0.3.5/macq/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.660473 macq-0.3.5/macq/generate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/fd_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/planning_domains_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/random_goal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/trace_from_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/pddl/vanilla_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 04:04:06.000000 macq-0.3.5/macq/generate/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.664473 macq-0.3.5/macq/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/action_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/atomic_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/id_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/identity_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/noisy_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/noisy_partial_disordered_parallel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/noisy_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/observed_tracelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-23 04:04:06.000000 macq-0.3.5/macq/observation/partial_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.664473 macq-0.3.5/macq/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/disordered_parallel_actions_observation_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/partial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-23 04:04:06.000000 macq-0.3.5/macq/trace/trace_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.668473 macq-0.3.5/macq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/complex_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/tokenization_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/trace_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 04:04:06.000000 macq-0.3.5/macq/utils/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.656473 macq-0.3.5/macq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 04:04:24.000000 macq-0.3.5/macq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-23 04:04:24.000000 macq-0.3.5/macq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:04:24.000000 macq-0.3.5/macq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 04:04:24.000000 macq-0.3.5/macq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 04:04:24.000000 macq-0.3.5/macq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 04:04:06.000000 macq-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:04:24.668473 macq-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-23 04:04:06.000000 macq-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:04:24.668473 macq-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-23 04:04:06.000000 macq-0.3.5/tests/test_readme.py
```

### Comparing `macq-0.3.4/LICENSE` & `macq-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/PKG-INFO` & `macq-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.4
+Version: 0.3.5
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.4/README.md` & `macq-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/__init__.py` & `macq-0.3.5/macq/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/amdn.py` & `macq-0.3.5/macq/extract/amdn.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/arms.py` & `macq-0.3.5/macq/extract/arms.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/exceptions.py` & `macq-0.3.5/macq/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/extract.py` & `macq-0.3.5/macq/extract/extract.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/learned_action.py` & `macq-0.3.5/macq/extract/learned_action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/learned_fluent.py` & `macq-0.3.5/macq/extract/learned_fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/locm.py` & `macq-0.3.5/macq/extract/locm.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/model.py` & `macq-0.3.5/macq/extract/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 lang.predicate(f.name, *f.param_sorts)
 
         if self.actions:
             for a in self.actions:
                 vars = [lang.variable(f"x{i}", s) for i, s in enumerate(a.param_sorts)]
 
                 if len(a.precond) == 1:
-                    precond = lang.get(list(a.precond)[0].name)(*[vars[i] for i in a.precond[0].param_act_inds])  # type: ignore
+                    precond = lang.get(list(a.precond)[0].name)(*[vars[i] for i in list(a.precond)[0].param_act_inds])  # type: ignore
                 else:
                     precond = CompoundFormula(
                         Connective.And,
                         [
                             lang.get(f.name)(*[vars[i] for i in f.param_act_inds])  # type: ignore
                             for f in a.precond
                         ],
```

### Comparing `macq-0.3.4/macq/extract/observer.py` & `macq-0.3.5/macq/extract/observer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/extract/slaf.py` & `macq-0.3.5/macq/extract/slaf.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/csv.py` & `macq-0.3.5/macq/generate/csv.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/fd_random_walk.py` & `macq-0.3.5/macq/generate/pddl/fd_random_walk.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/generator.py` & `macq-0.3.5/macq/generate/pddl/generator.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/planning_domains_api.py` & `macq-0.3.5/macq/generate/pddl/planning_domains_api.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/random_goal_sampling.py` & `macq-0.3.5/macq/generate/pddl/random_goal_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/trace_from_goal.py` & `macq-0.3.5/macq/generate/pddl/trace_from_goal.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/pddl/vanilla_sampling.py` & `macq-0.3.5/macq/generate/pddl/vanilla_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/generate/plan.py` & `macq-0.3.5/macq/generate/plan.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/__init__.py` & `macq-0.3.5/macq/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/action_observation.py` & `macq-0.3.5/macq/observation/action_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/atomic_partial_observation.py` & `macq-0.3.5/macq/observation/atomic_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/identity_observation.py` & `macq-0.3.5/macq/observation/identity_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/noisy_observation.py` & `macq-0.3.5/macq/observation/noisy_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/noisy_partial_disordered_parallel_observation.py` & `macq-0.3.5/macq/observation/noisy_partial_disordered_parallel_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/noisy_partial_observation.py` & `macq-0.3.5/macq/observation/noisy_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/observation.py` & `macq-0.3.5/macq/observation/observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/observed_tracelist.py` & `macq-0.3.5/macq/observation/observed_tracelist.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/observation/partial_observation.py` & `macq-0.3.5/macq/observation/partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/__init__.py` & `macq-0.3.5/macq/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/action.py` & `macq-0.3.5/macq/trace/action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/disordered_parallel_actions_observation_lists.py` & `macq-0.3.5/macq/trace/disordered_parallel_actions_observation_lists.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/fluent.py` & `macq-0.3.5/macq/trace/fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/state.py` & `macq-0.3.5/macq/trace/state.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/step.py` & `macq-0.3.5/macq/trace/step.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/trace.py` & `macq-0.3.5/macq/trace/trace.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/trace/trace_list.py` & `macq-0.3.5/macq/trace/trace_list.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/__init__.py` & `macq-0.3.5/macq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/progress.py` & `macq-0.3.5/macq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/pysat.py` & `macq-0.3.5/macq/utils/pysat.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/timer.py` & `macq-0.3.5/macq/utils/timer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/trace_errors.py` & `macq-0.3.5/macq/utils/trace_errors.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq/utils/trace_utils.py` & `macq-0.3.5/macq/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/macq.egg-info/PKG-INFO` & `macq-0.3.5/macq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.4
+Version: 0.3.5
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.4/macq.egg-info/SOURCES.txt` & `macq-0.3.5/macq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macq-0.3.4/setup.py` & `macq-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 
 NAME = "macq"
 
 DESCRIPTION = "Action model acquisition from state trace data."
 
 DEPENDENCIES = [
     "tarski",
```

### Comparing `macq-0.3.4/tests/test_readme.py` & `macq-0.3.5/tests/test_readme.py`

 * *Files identical despite different names*

