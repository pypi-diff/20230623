# Comparing `tmp/macq-0.3.3.tar.gz` & `tmp/macq-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macq-0.3.3.tar", last modified: Fri Jun 16 19:19:04 2023, max compression
+gzip compressed data, was "macq-0.3.4.tar", last modified: Fri Jun 23 02:52:04 2023, max compression
```

## Comparing `macq-0.3.3.tar` & `macq-0.3.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 19:18:40.000000 macq-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 19:19:04.689309 macq-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-16 19:18:40.000000 macq-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.681309 macq-0.3.3/macq/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 19:18:40.000000 macq-0.3.3/macq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/amdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/arms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/learned_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/learned_fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    31588 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/locm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/slaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/generate/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/fd_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/planning_domains_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/random_goal_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/trace_from_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/vanilla_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/observation/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/action_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/atomic_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/id_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/identity_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_partial_disordered_parallel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/observed_tracelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/partial_observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/macq/trace/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/disordered_parallel_actions_observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/partial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/trace_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/macq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/common_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/complex_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/tokenization_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/trace_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/trace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.681309 macq-0.3.3/macq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 19:18:40.000000 macq-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:19:04.689309 macq-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 19:18:40.000000 macq-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 19:18:40.000000 macq-0.3.3/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 02:51:43.000000 macq-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 02:52:04.061415 macq-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 02:51:43.000000 macq-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.053415 macq-0.3.4/macq/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 02:51:43.000000 macq-0.3.4/macq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/amdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/learned_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/learned_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34948 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/locm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-23 02:51:43.000000 macq-0.3.4/macq/extract/slaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/generate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/fd_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/planning_domains_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/random_goal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/trace_from_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/pddl/vanilla_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 02:51:43.000000 macq-0.3.4/macq/generate/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/action_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/atomic_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/id_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/identity_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_partial_disordered_parallel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/noisy_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/observed_tracelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-23 02:51:43.000000 macq-0.3.4/macq/observation/partial_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.057415 macq-0.3.4/macq/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/disordered_parallel_actions_observation_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/partial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-23 02:51:43.000000 macq-0.3.4/macq/trace/trace_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/macq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/complex_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/tokenization_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/trace_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 02:51:43.000000 macq-0.3.4/macq/utils/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.053415 macq-0.3.4/macq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 02:52:04.000000 macq-0.3.4/macq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 02:51:43.000000 macq-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 02:52:04.061415 macq-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-23 02:51:43.000000 macq-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:52:04.061415 macq-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-23 02:51:43.000000 macq-0.3.4/tests/test_readme.py
```

### Comparing `macq-0.3.3/LICENSE` & `macq-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/PKG-INFO` & `macq-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.3
+Version: 0.3.4
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.3/README.md` & `macq-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/__init__.py` & `macq-0.3.4/macq/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/amdn.py` & `macq-0.3.4/macq/extract/amdn.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/arms.py` & `macq-0.3.4/macq/extract/arms.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/exceptions.py` & `macq-0.3.4/macq/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/extract.py` & `macq-0.3.4/macq/extract/extract.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/learned_action.py` & `macq-0.3.4/macq/extract/learned_action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/learned_fluent.py` & `macq-0.3.4/macq/extract/learned_fluent.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return isinstance(other, LearnedLiftedFluent) and hash(self) == hash(other)
 
     def __hash__(self):
         # Order of objects is important!
         return hash(self.details())
 
     def __str__(self):
-        return self.details()
+        return self.details() + f" {self.param_act_inds}"
 
     def __repr__(self):
         return self.details()
 
     def details(self):
         return f"({self.name} {' '.join(self.param_sorts)})"
```

### Comparing `macq-0.3.3/macq/extract/locm.py` & `macq-0.3.4/macq/extract/locm.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """Action.Position (of object parameter). Position is 1-indexed."""
 
     action: Action
     pos: int  # NOTE: 1-indexed
     sort: int
 
     def __repr__(self) -> str:
-        return f"{self.action.name}.{self.pos}"
+        return f"{self.action.name}.{self.pos} [sort{self.sort}]"
 
     def __hash__(self):
         return hash(self.action.name + str(self.pos))
 
     def __eq__(self, other):
         return hash(self) == hash(other)
 
@@ -102,14 +102,15 @@
 
     "In general, there is a state S between two consecutive transitions B.k and
     C.l within the FSM associated with sort G, that is where B moves an object O
     of sort G into S, and C moves O out of S. When both actions B and C contain
     another argument of the same sort G′ in position k′ and l′ respectively, we
     hypothesise that there may be a relation between sorts G and G′."
     """
+
     S: int
     B: AP
     k: int
     k_: int
     C: AP
     l: int
     l_: int
@@ -127,18 +128,34 @@
                 self.l,
                 self.l_,
                 self.G_,
             )
         )
 
     def __repr__(self) -> str:
-        out = "<\n"
-        for k, v in asdict(self).items():
-            out += f"  {k}={v}\n"
-        return out.strip() + "\n>"
+        out = f"\n [->B->S->C->] = ({str(self.B)}) -> {str(self.S)} -> ({str(self.C)})"
+        out += "\n\tG\tG'\tS\tk\tk'\tl\tl'"
+        out += (
+            "\n\t"
+            + str(self.G)
+            + "\t"
+            + str(self.G_)
+            + "\t"
+            + str(self.S)
+            + "\t"
+            + str(self.k)
+            + "\t"
+            + str(self.k_)
+            + "\t"
+            + str(self.l)
+            + "\t"
+            + str(self.l_)
+            + "\n"
+        )
+        return out
 
     @staticmethod
     def from_dict(
         hs: Dict[HSIndex, Set[HSItem]]
     ) -> Dict[int, Dict[int, Set["Hypothesis"]]]:
         """Converts a dict of HSIndex -> HSItem to a dict of G -> S -> Hypothesis"""
         HS: Dict[int, Dict[int, Set["Hypothesis"]]] = defaultdict(
@@ -212,34 +229,35 @@
 
         obs_trace = obs_tracelist[0]
         fluents, actions = None, None
 
         sorts = LOCM._get_sorts(obs_trace, debug=debug["get_sorts"])
 
         if debug["sorts"]:
-            print(f"Sorts:\n{sorts}", end="\n\n")
+            sortid2objs = {v: [] for v in set(sorts.values())}
+            for k, v in sorts.items():
+                sortid2objs[v].append(k)
+            print("\nSorts:\n")
+            pprint(sortid2objs)
+            print("\n")
 
         TS, ap_state_pointers, OS = LOCM._step1(obs_trace, sorts, debug["step1"])
         HS = LOCM._step3(TS, ap_state_pointers, OS, sorts, debug["step3"])
         bindings = LOCM._step4(HS, debug["step4"])
         bindings = LOCM._step5(HS, bindings, debug["step5"])
         fluents, actions = LOCM._step7(
             OS,
             ap_state_pointers,
             sorts,
             bindings,
             statics if statics is not None else {},
             debug["step7"],
+            viz,
         )
 
-        if viz:
-            state_machines = LOCM.get_state_machines(ap_state_pointers, OS, bindings)
-            for sm in state_machines:
-                sm.render(view=view)
-
         return Model(fluents, actions)
 
     @staticmethod
     def _get_sorts(obs_trace: List[Observation], debug=False) -> Sorts:
         sorts = []  # initialize list of sorts for this trace
         # track actions seen in the trace, and the sort each actions params belong to
         ap_sort_pointers: Dict[str, List[int]] = {}
@@ -418,17 +436,20 @@
         # initialize the state set OS and transition set TS
         OS: OSType = defaultdict(list)
         TS: TSType = defaultdict(dict)
         # track pointers mapping A.P to its start and end states
         ap_state_pointers = defaultdict(dict)
         # iterate over each object and its action sequence
         for obj, seq in obj_traces.items():
-            state_n = 1  # count current (new) state id
             sort = sorts[obj.name] if obj != zero_obj else 0
             TS[sort][obj] = seq  # add the sequence to the transition set
+            # max of the states already in OS[sort], plus 1
+            state_n = (
+                max([max(s) for s in OS[sort]] + [0]) + 1
+            )  # count current (new) state id
             prev_states: StatePointers = None  # type: ignore
             # iterate over each transition A.P in the sequence
             for ap in seq:
                 # if the transition has not been seen before for the current sort
                 if ap not in ap_state_pointers[sort]:
                     ap_state_pointers[sort][ap] = StatePointers(state_n, state_n + 1)
 
@@ -449,14 +470,15 @@
 
                     # if not the same state set, merge the two
                     if start_state != prev_end_state:
                         OS[sort][start_state] = OS[sort][start_state].union(
                             OS[sort][prev_end_state]
                         )
                         OS[sort].pop(prev_end_state)
+                    assert len(set.union(*OS[sort])) == sum([len(s) for s in OS[sort]])
 
                 prev_states = ap_states
 
         # remove the zero-object sort if it only has one state
         if len(OS[0]) == 1:
             ap_state_pointers[0] = {}
             OS[0] = []
@@ -544,29 +566,26 @@
                             ):
                                 H.supported = True
                             else:  # otherwise remove the hypothesis
                                 HS[BkCl].remove(H)
 
         # Remove any unsupported hypotheses (but yet undisputed)
         for hind, hs in HS.copy().items():
-            for h in hs:
+            for h in hs.copy():
                 if not h.supported:
                     hs.remove(h)
             if len(hs) == 0:
                 del HS[hind]
 
         # Converts HS {HSIndex: HSItem} to a mapping of hypothesis for states of a sort {sort: {state: Hypothesis}}
         return Hypothesis.from_dict(HS)
 
     @staticmethod
-    def _step4(
-        HS: Dict[int, Dict[int, Set[Hypothesis]]], debug: bool = False
-    ) -> Bindings:
+    def _step4(HS: Hypotheses, debug: bool = False) -> Bindings:
         """Step 4: Creation and merging of state parameters"""
-
         # bindings = {sort: {state: [(hypothesis, state param)]}}
         bindings: Bindings = defaultdict(dict)
         for sort, hs_sort in HS.items():
             for state, hs_sort_state in hs_sort.items():
                 # state_bindings = {hypothesis (h): state param (v)}
                 state_bindings: Dict[Hypothesis, int] = {}
 
@@ -588,15 +607,15 @@
 
                 # for each (unordered) pair of hypotheses h1, h2
                 for i, h1 in enumerate(hs_sort_state):
                     for h2 in hs_sort_state[i + 1 :]:
                         # check if hypothesis parameters (v1 & v2) need to be unified
                         if (
                             (h1.B == h2.B and h1.k == h2.k and h1.k_ == h2.k_)
-                            or
+                                    and   # See https://github.com/AI-Planning/macq/discussions/200
                             (h1.C == h2.C and h1.l == h2.l and h1.l_ == h2.l_)  # fmt: skip
                         ):
                             v1 = state_bindings[h1]
                             v2 = state_bindings[h2]
 
                             # get the parameter sets P1, P2 that v1, v2 belong to
                             P1, P2 = LOCM._pointer_to_set(state_params, v1, v2)
@@ -605,219 +624,252 @@
                                 # merge P1 and P2
                                 state_params[P1] = state_params[P1].union(
                                     state_params[P2]
                                 )
                                 state_params.pop(P2)
                                 state_param_pointers[v2] = P1
 
+                                # fix state_param_pointers after v2
+                                for ind in range(v2 + 1, len(state_param_pointers)):
+                                    state_param_pointers[ind] -= 1
+
                 # add state bindings for the sort to the output bindings
                 # replacing hypothesis params with actual state params
                 bindings[sort][state] = [
                     Binding(h, LOCM._pointer_to_set(state_params, v)[0])
                     for h, v in state_bindings.items()
                 ]
 
         return dict(bindings)
 
     @staticmethod
     def _step5(
-        HS: Dict[int, Dict[int, Set[Hypothesis]]],
+        HS: Hypotheses,
         bindings: Bindings,
         debug: bool = False,
     ) -> Bindings:
         """Step 5: Removing parameter flaws"""
 
         # check each bindings[G][S] -> (h, P)
         for sort, hs_sort in HS.items():
-            for state in hs_sort:
+            for state_id in hs_sort:
                 # track all the h.Bs that occur in bindings[G][S]
                 all_hB = set()
                 # track the set of h.B that set parameter P
                 sets_P = defaultdict(set)
-                for h, P in bindings[sort][state]:
+                for h, P in bindings[sort][state_id]:
                     sets_P[P].add(h.B)
                     all_hB.add(h.B)
 
                 # for each P, check if there is a transition h.B that never sets parameter P
                 # i.e. if sets_P[P] != all_hB
                 for P, setby in sets_P.items():
                     if not setby == all_hB:  # P is a flawed parameter
                         # remove all bindings referencing P
-                        for h, P_ in bindings[sort][state].copy():
+                        for h, P_ in bindings[sort][state_id].copy():
                             if P_ == P:
-                                bindings[sort][state].remove(Binding(h, P_))
-                        if len(bindings[sort][state]) == 0:
-                            del bindings[sort][state]
+                                bindings[sort][state_id].remove(Binding(h, P_))
+                        if len(bindings[sort][state_id]) == 0:
+                            del bindings[sort][state_id]
+
+                # do the same for checking h.C reading parameter P
+                # See https://github.com/AI-Planning/macq/discussions/200
+                all_hC = set()
+                reads_P = defaultdict(set)
+                if state_id in bindings[sort]:
+                    for h, P in bindings[sort][state_id]:
+                        reads_P[P].add(h.C)
+                        all_hC.add(h.C)
+                    for P, readby in reads_P.items():
+                        if not readby == all_hC:
+                            for h, P_ in bindings[sort][state_id].copy():
+                                if P_ == P:
+                                    bindings[sort][state_id].remove(Binding(h, P_))
+                            if len(bindings[sort][state_id]) == 0:
+                                del bindings[sort][state_id]
 
         for k, v in bindings.copy().items():
             if not v:
                 del bindings[k]
 
         return bindings
 
     @staticmethod
-    def get_state_machines(
-        ap_state_pointers: APStatePointers,
-        OS: OSType,
-        bindings: Optional[Bindings] = None,
-    ):
-        from graphviz import Digraph
+    def _debug_state_machines(OS, ap_state_pointers, state_params):
+        import os
 
-        state_machines = []
-        for (sort, trans), states in zip(ap_state_pointers.items(), OS.values()):
-            graph = Digraph(f"LOCM-step1-sort{sort}")
-            for state in range(len(states)):
-                label = f"state{state}"
+        import networkx as nx
+
+        for sort in OS:
+            G = nx.DiGraph()
+            for n in range(len(OS[sort])):
+                lbl = f"state{n}"
                 if (
-                    bindings is not None
-                    and sort in bindings
-                    and state in bindings[sort]
+                    state_params is not None
+                    and sort in state_params
+                    and n in state_params[sort]
                 ):
-                    label += f"\n["
-                    params = []
-                    for binding in bindings[sort][state]:
-                        params.append(f"{binding.hypothesis.G_}")
-                    label += f",".join(params)
-                    label += f"]"
-                graph.node(str(state), label=label, shape="oval")
-            for ap, apstate in trans.items():
+                    lbl += str(
+                        [
+                            state_params[sort][n][v]
+                            for v in sorted(state_params[sort][n].keys())
+                        ]
+                    )
+                G.add_node(n, label=lbl, shape="oval")
+            for ap, apstate in ap_state_pointers[sort].items():
                 start_idx, end_idx = LOCM._pointer_to_set(
-                    states, apstate.start, apstate.end
+                    OS[sort], apstate.start, apstate.end
                 )
-                graph.edge(
-                    str(start_idx), str(end_idx), label=f"{ap.action.name}.{ap.pos}"
-                )
-
-            state_machines.append(graph)
-
-        return state_machines
+                # check if edge is already in graph
+                if G.has_edge(start_idx, end_idx):
+                    # append to the edge label
+                    G.edges[start_idx, end_idx][
+                        "label"
+                    ] += f"\n{ap.action.name}.{ap.pos}"
+                else:
+                    G.add_edge(start_idx, end_idx, label=f"{ap.action.name}.{ap.pos}")
+            # write to dot file
+            nx.drawing.nx_pydot.write_dot(G, f"LOCM-step7-sort{sort}.dot")
+            os.system(
+                f"dot -Tpng LOCM-step7-sort{sort}.dot -o LOCM-step7-sort{sort}.png"
+            )
+            os.system(f"rm LOCM-step7-sort{sort}.dot")
 
     @staticmethod
     def _step7(
         OS: OSType,
         ap_state_pointers: APStatePointers,
         sorts: Sorts,
         bindings: Bindings,
         statics: Statics,
         debug: bool = False,
+        viz: bool = False,
     ) -> Tuple[Set[LearnedLiftedFluent], Set[LearnedLiftedAction]]:
         """Step 7: Formation of PDDL action schema
         Implicitly includes Step 6 (statics) by including statics as an argument
         and adding to the relevant actions while being constructed.
         """
 
         # delete zero-object if it's state machine was discarded
         if not OS[0]:
             del OS[0]
             del ap_state_pointers[0]
 
-        if debug:
-            print("ap state pointers")
-            pprint(ap_state_pointers)
-            print()
-
-            print("OS:")
-            pprint(OS)
-            print()
-
-            print("bindings:")
-            pprint(bindings)
-            print()
-
-        bound_param_sorts = {
-            sort: {
-                state: [
-                    binding.hypothesis.G_
-                    for binding in bindings.get(sort, {}).get(state, [])
-                ]
-                for state in range(len(states))
-            }
-            for sort, states in OS.items()
-        }
-
-        actions = {}
-        fluents = defaultdict(dict)
-
+        # all_aps = {action_name: [AP]}
         all_aps: Dict[str, List[AP]] = defaultdict(list)
         for aps in ap_state_pointers.values():
             for ap in aps:
                 all_aps[ap.action.name].append(ap)
 
-        for action, aps in all_aps.items():
-            actions[action] = LearnedLiftedAction(
-                action, [f"sort{ap.sort}" for ap in aps]
-            )
+        state_params = defaultdict(dict)
+        state_params_to_hyps = defaultdict(dict)
+        for sort in bindings:
+            state_params[sort] = defaultdict(dict)
+            state_params_to_hyps[sort] = defaultdict(dict)
+            for state in bindings[sort]:
+                keys = {b.param for b in bindings[sort][state]}
+                typ = None
+                for key in keys:
+                    hyps = [
+                        b.hypothesis for b in bindings[sort][state] if b.param == key
+                    ]
+                    # assert that all are the same G_
+                    assert len(set([h.G_ for h in hyps])) == 1
+                    state_params[sort][state][key] = hyps[0].G_
+                    state_params_to_hyps[sort][state][key] = hyps
 
-        @dataclass
-        class TemplateFluent:
-            name: str
-            param_sorts: List[str]
-
-            def __hash__(self) -> int:
-                return hash(self.name + "".join(self.param_sorts))
-
-        for sort, state_bindings in bound_param_sorts.items():
-            for state, bound_sorts in state_bindings.items():
-                fluents[sort][state] = TemplateFluent(
-                    f"sort{sort}_state{state}",
-                    [f"sort{sort}"] + [f"sort{s}" for s in bound_sorts],
-                )
+        if viz:
+            LOCM._debug_state_machines(OS, ap_state_pointers, state_params)
+
+        fluents = defaultdict(dict)
+        actions = {}
+        for sort in ap_state_pointers:
+            sort_str = f"sort{sort}"
+            for ap in ap_state_pointers[sort]:
+                if ap.action.name not in actions:
+                    actions[ap.action.name] = LearnedLiftedAction(
+                        ap.action.name,
+                        [None for _ in range(len(all_aps[ap.action.name]))],  # type: ignore
+                    )
+                a = actions[ap.action.name]
+                a.param_sorts[ap.pos - 1] = sort_str
 
-        for (sort, aps), states in zip(ap_state_pointers.items(), OS.values()):
-            for ap, pointers in aps.items():
+                start_pointer, end_pointer = ap_state_pointers[sort][ap]
                 start_state, end_state = LOCM._pointer_to_set(
-                    states, pointers.start, pointers.end
+                    OS[sort], start_pointer, end_pointer
                 )
 
-                # preconditions += fluent for origin state
-                start_fluent_temp = fluents[sort][start_state]
+                start_fluent_name = f"sort{sort}_state{start_state}"
+                if start_fluent_name not in fluents[ap.action.name]:
+                    start_fluent = LearnedLiftedFluent(
+                        start_fluent_name,
+                        param_sorts=[sort_str],
+                        param_act_inds=[ap.pos - 1],
+                    )
+                    fluents[ap.action.name][start_fluent_name] = start_fluent
 
-                bound_param_inds = []
+                start_fluent = fluents[ap.action.name][start_fluent_name]
 
-                # for each bindings on the start state (if there are any)
-                # then add each binding.hypothesis.l_
-                if sort in bindings and start_state in bindings[sort]:
-                    bound_param_inds = [
-                        b.hypothesis.l_ - 1 for b in bindings[sort][start_state]
-                    ]
+                if (
+                    sort in state_params_to_hyps
+                    and start_state in state_params_to_hyps[sort]
+                ):
+                    for param in state_params_to_hyps[sort][start_state]:
+                        psort = None
+                        pind = None
+                        for hyp in state_params_to_hyps[sort][start_state][param]:
+                            if hyp.C == ap:
+                                assert psort is None or psort == hyp.G_
+                                assert pind is None or pind == hyp.l_
+                                psort = hyp.G_
+                                pind = hyp.l_
+                        assert psort is not None
+                        assert pind is not None
+                        start_fluent.param_sorts.append(f"sort{psort}")
+                        start_fluent.param_act_inds.append(pind - 1)
+
+                a.update_precond(start_fluent)
+
+                if end_state != start_state:
+                    end_fluent_name = f"sort{sort}_state{end_state}"
+                    if end_fluent_name not in fluents[ap.action.name]:
+                        end_fluent = LearnedLiftedFluent(
+                            end_fluent_name,
+                            param_sorts=[sort_str],
+                            param_act_inds=[ap.pos - 1],
+                        )
+                        fluents[ap.action.name][end_fluent_name] = end_fluent
 
-                start_fluent = LearnedLiftedFluent(
-                    start_fluent_temp.name,
-                    start_fluent_temp.param_sorts,
-                    [ap.pos - 1] + bound_param_inds,
-                )
-                fluents[sort][start_state] = start_fluent
-                actions[ap.action.name].update_precond(start_fluent)
+                    end_fluent = fluents[ap.action.name][end_fluent_name]
 
-                if start_state != end_state:
-                    # del += fluent for origin state
-                    actions[ap.action.name].update_delete(start_fluent)
-
-                    # add += fluent for destination state
-                    end_fluent_temp = fluents[sort][end_state]
-                    bound_param_inds = []
-                    if sort in bindings and end_state in bindings[sort]:
-                        bound_param_inds = [
-                            b.hypothesis.l_ - 1 for b in bindings[sort][end_state]
-                        ]
-                    end_fluent = LearnedLiftedFluent(
-                        end_fluent_temp.name,
-                        end_fluent_temp.param_sorts,
-                        [ap.pos - 1] + bound_param_inds,
-                    )
-                    fluents[sort][end_state] = end_fluent
-                    actions[ap.action.name].update_add(end_fluent)
+                    if (
+                        sort in state_params_to_hyps
+                        and end_state in state_params_to_hyps[sort]
+                    ):
+                        for param in state_params_to_hyps[sort][end_state]:
+                            psort = None
+                            pind = None
+                            for hyp in state_params_to_hyps[sort][end_state][param]:
+                                if hyp.B == ap:
+                                    assert psort is None or psort == hyp.G_
+                                    assert pind is None or pind == hyp.k_
+                                    psort = hyp.G_
+                                    pind = hyp.k_
+                            assert psort is not None
+                            assert pind is not None
+                            end_fluent.param_sorts.append(f"sort{psort}")
+                            end_fluent.param_act_inds.append(pind - 1)
 
-        fluents = set(fluent for sort in fluents.values() for fluent in sort.values())
-        actions = set(actions.values())
+                    a.update_delete(start_fluent)
+                    a.update_add(end_fluent)
 
         # Step 6: Extraction of static preconditions
-        for action in actions:
+        for action in actions.values():
             if action.name in statics:
                 for static in statics[action.name]:
                     action.update_precond(static)
 
-        if debug:
-            pprint(fluents)
-            pprint(actions)
-
-        return fluents, actions
+        return set(
+            fluent
+            for action_fluents in fluents.values()
+            for fluent in action_fluents.values()
+        ), set(actions.values())
```

### Comparing `macq-0.3.3/macq/extract/model.py` & `macq-0.3.4/macq/extract/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,15 @@
         if not problem_name:
             problem_name = domain_name + "_problem"
         if not domain_filename:
             domain_filename = domain_name + ".pddl"
         if not problem_filename:
             problem_filename = problem_name + ".pddl"
 
-        if (
-            isinstance(list(self.fluents)[0], LearnedLiftedFluent) and 
-            isinstance(list(self.actions)[0], LearnedLiftedAction)  # fmt: skip
-        ):
+        if isinstance(list(self.actions)[0], LearnedLiftedAction):
             self.to_pddl_lifted(
                 domain_name, problem_name, domain_filename, problem_filename
             )
         elif isinstance(list(self.actions)[0], LearnedAction):
             self.to_pddl_grounded(
                 domain_name, problem_name, domain_filename, problem_filename
             )
```

### Comparing `macq-0.3.3/macq/extract/observer.py` & `macq-0.3.4/macq/extract/observer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/extract/slaf.py` & `macq-0.3.4/macq/extract/slaf.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/csv.py` & `macq-0.3.4/macq/generate/csv.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/fd_random_walk.py` & `macq-0.3.4/macq/generate/pddl/fd_random_walk.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/generator.py` & `macq-0.3.4/macq/generate/pddl/generator.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/planning_domains_api.py` & `macq-0.3.4/macq/generate/pddl/planning_domains_api.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/random_goal_sampling.py` & `macq-0.3.4/macq/generate/pddl/random_goal_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/trace_from_goal.py` & `macq-0.3.4/macq/generate/pddl/trace_from_goal.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/pddl/vanilla_sampling.py` & `macq-0.3.4/macq/generate/pddl/vanilla_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/generate/plan.py` & `macq-0.3.4/macq/generate/plan.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/__init__.py` & `macq-0.3.4/macq/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/action_observation.py` & `macq-0.3.4/macq/observation/action_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/atomic_partial_observation.py` & `macq-0.3.4/macq/observation/atomic_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/identity_observation.py` & `macq-0.3.4/macq/observation/identity_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/noisy_observation.py` & `macq-0.3.4/macq/observation/noisy_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/noisy_partial_disordered_parallel_observation.py` & `macq-0.3.4/macq/observation/noisy_partial_disordered_parallel_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/noisy_partial_observation.py` & `macq-0.3.4/macq/observation/noisy_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/observation.py` & `macq-0.3.4/macq/observation/observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/observed_tracelist.py` & `macq-0.3.4/macq/observation/observed_tracelist.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/observation/partial_observation.py` & `macq-0.3.4/macq/observation/partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/__init__.py` & `macq-0.3.4/macq/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/action.py` & `macq-0.3.4/macq/trace/action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/disordered_parallel_actions_observation_lists.py` & `macq-0.3.4/macq/trace/disordered_parallel_actions_observation_lists.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/fluent.py` & `macq-0.3.4/macq/trace/fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/state.py` & `macq-0.3.4/macq/trace/state.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/step.py` & `macq-0.3.4/macq/trace/step.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/trace.py` & `macq-0.3.4/macq/trace/trace.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/trace/trace_list.py` & `macq-0.3.4/macq/trace/trace_list.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/__init__.py` & `macq-0.3.4/macq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/progress.py` & `macq-0.3.4/macq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/pysat.py` & `macq-0.3.4/macq/utils/pysat.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/timer.py` & `macq-0.3.4/macq/utils/timer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/trace_errors.py` & `macq-0.3.4/macq/utils/trace_errors.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq/utils/trace_utils.py` & `macq-0.3.4/macq/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/macq.egg-info/PKG-INFO` & `macq-0.3.4/macq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.3
+Version: 0.3.4
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.3/macq.egg-info/SOURCES.txt` & `macq-0.3.4/macq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macq-0.3.3/setup.py` & `macq-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.3"
+VERSION = "0.3.4"
 
 NAME = "macq"
 
 DESCRIPTION = "Action model acquisition from state trace data."
 
 DEPENDENCIES = [
     "tarski",
@@ -12,14 +12,16 @@
     "rich",
     "nnf",
     "python-sat",
     "bauhaus",
     "numpy",
     "clingo",
     "graphviz",
+    "networkx",
+    "pydot",
 ]
 
 DEV_DEPENDENCIES = [
     "pytest",
     "pytest-cov",
     "flake8",
     "black",
```

### Comparing `macq-0.3.3/tests/test_readme.py` & `macq-0.3.4/tests/test_readme.py`

 * *Files identical despite different names*

