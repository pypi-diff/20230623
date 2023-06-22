# Comparing `tmp/abmarl-0.2.5.tar.gz` & `tmp/abmarl-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rusu1/Abmarl/dist/.tmp-1n2_09t9/abmarl-0.2.5.tar", last modified: Fri Jan  6 01:45:28 2023, max compression
+gzip compressed data, was "abmarl-0.2.6.tar", last modified: Thu Jun 22 22:08:13 2023, max compression
```

## Comparing `abmarl-0.2.5.tar` & `abmarl-0.2.6.tar`

### file list

```diff
@@ -1,140 +1,144 @@
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/
--rw-r--r--   0 rusu1    (58596)    58596     2255 2022-08-02 17:16:47.000000 abmarl-0.2.5/LICENSE
--rw-r--r--   0 rusu1    (58596)    58596     1166 2022-08-02 17:16:47.000000 abmarl-0.2.5/NOTICE
--rw-r--r--   0 rusu1    (58596)    58596     4390 2023-01-06 01:45:28.000000 abmarl-0.2.5/PKG-INFO
--rw-r--r--   0 rusu1    (58596)    58596     3491 2022-08-18 15:34:16.000000 abmarl-0.2.5/README.md
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/__init__.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/algs/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/algs/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     2852 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/algs/monte_carlo.py
--rw-r--r--   0 rusu1    (58596)    58596      807 2022-10-15 14:07:02.000000 abmarl-0.2.5/abmarl/debug.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/examples/
--rw-r--r--   0 rusu1    (58596)    58596      335 2022-09-22 18:22:42.000000 abmarl-0.2.5/abmarl/examples/__init__.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/examples/sim/
--rw-r--r--   0 rusu1    (58596)    58596      399 2022-09-22 18:22:42.000000 abmarl-0.2.5/abmarl/examples/sim/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596    13354 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/examples/sim/comms_blocking.py
--rw-r--r--   0 rusu1    (58596)    58596     1969 2022-08-18 18:46:52.000000 abmarl-0.2.5/abmarl/examples/sim/maze_navigation.py
--rw-r--r--   0 rusu1    (58596)    58596     8336 2022-10-03 15:03:13.000000 abmarl-0.2.5/abmarl/examples/sim/multi_agent_sim.py
--rw-r--r--   0 rusu1    (58596)    58596     6875 2022-10-05 19:22:45.000000 abmarl-0.2.5/abmarl/examples/sim/multi_corridor.py
--rw-r--r--   0 rusu1    (58596)    58596     5882 2022-10-07 02:49:32.000000 abmarl-0.2.5/abmarl/examples/sim/reach_the_target.py
--rw-r--r--   0 rusu1    (58596)    58596     3299 2022-10-07 02:49:32.000000 abmarl-0.2.5/abmarl/examples/sim/team_battle_example.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/external/
--rw-r--r--   0 rusu1    (58596)    58596      152 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/external/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     2200 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/external/gym_env_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596    12105 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/external/open_spiel_env_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     1511 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/external/rllib_multiagentenv_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     4548 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/make_runnable.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/managers/
--rw-r--r--   0 rusu1    (58596)    58596      199 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/managers/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     2481 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/managers/all_step_manager.py
--rw-r--r--   0 rusu1    (58596)    58596     4066 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/managers/dynamic_order_manager.py
--rw-r--r--   0 rusu1    (58596)    58596     1677 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/managers/simulation_manager.py
--rw-r--r--   0 rusu1    (58596)    58596     4288 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/managers/turn_based_manager.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/policies/
--rw-r--r--   0 rusu1    (58596)    58596      114 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/policies/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596      170 2022-09-21 20:13:19.000000 abmarl-0.2.5/abmarl/policies/interactive_policy.py
--rw-r--r--   0 rusu1    (58596)    58596     2720 2022-08-19 18:06:43.000000 abmarl-0.2.5/abmarl/policies/policy.py
--rw-r--r--   0 rusu1    (58596)    58596     3810 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/policies/q_table_policy.py
--rw-r--r--   0 rusu1    (58596)    58596     1152 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/policies/rllib_policy.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/scripts/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596      785 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/analyze_script.py
--rw-r--r--   0 rusu1    (58596)    58596     1162 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/debug_script.py
--rw-r--r--   0 rusu1    (58596)    58596     1240 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/make_runnable_script.py
--rw-r--r--   0 rusu1    (58596)    58596     2088 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/scripts.py
--rw-r--r--   0 rusu1    (58596)    58596      473 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/train_script.py
--rw-r--r--   0 rusu1    (58596)    58596     1463 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/scripts/visualize_script.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/sim/
--rw-r--r--   0 rusu1    (58596)    58596      139 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     9551 2022-10-03 15:03:13.000000 abmarl-0.2.5/abmarl/sim/agent_based_simulation.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/sim/gridworld/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/gridworld/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596    24758 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/sim/gridworld/actor.py
--rw-r--r--   0 rusu1    (58596)    58596     8439 2022-09-22 18:22:42.000000 abmarl-0.2.5/abmarl/sim/gridworld/agent.py
--rw-r--r--   0 rusu1    (58596)    58596     6617 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/sim/gridworld/base.py
--rw-r--r--   0 rusu1    (58596)    58596     1841 2022-08-18 20:02:21.000000 abmarl-0.2.5/abmarl/sim/gridworld/done.py
--rw-r--r--   0 rusu1    (58596)    58596     4116 2022-10-07 22:08:54.000000 abmarl-0.2.5/abmarl/sim/gridworld/grid.py
--rw-r--r--   0 rusu1    (58596)    58596    10177 2022-10-12 18:42:22.000000 abmarl-0.2.5/abmarl/sim/gridworld/observer.py
--rw-r--r--   0 rusu1    (58596)    58596     3043 2022-09-26 17:36:18.000000 abmarl-0.2.5/abmarl/sim/gridworld/state.py
--rw-r--r--   0 rusu1    (58596)    58596     6689 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/gridworld/utils.py
--rw-r--r--   0 rusu1    (58596)    58596    10483 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/sim/gridworld/wrapper.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/sim/wrappers/
--rw-r--r--   0 rusu1    (58596)    58596      327 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/wrappers/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     4829 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/sim/wrappers/communication_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     8247 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/sim/wrappers/flatten_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     7441 2023-01-06 01:43:01.000000 abmarl-0.2.5/abmarl/sim/wrappers/ravel_discrete_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     2144 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/wrappers/sar_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596    13292 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/sim/wrappers/super_agent_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     1520 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/sim/wrappers/wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     5105 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/stage.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/tools/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/tools/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     1810 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/tools/gym_utils.py
--rw-r--r--   0 rusu1    (58596)    58596      666 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/tools/matplotlib_utils.py
--rw-r--r--   0 rusu1    (58596)    58596      766 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/tools/numpy_utils.py
--rw-r--r--   0 rusu1    (58596)    58596     2201 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/tools/utils.py
--rw-r--r--   0 rusu1    (58596)    58596      946 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/train.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl/trainers/
--rw-r--r--   0 rusu1    (58596)    58596       90 2022-08-02 17:16:47.000000 abmarl-0.2.5/abmarl/trainers/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     8535 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/trainers/base.py
--rw-r--r--   0 rusu1    (58596)    58596     3672 2022-10-21 00:59:36.000000 abmarl-0.2.5/abmarl/trainers/debug.py
--rw-r--r--   0 rusu1    (58596)    58596     1390 2022-08-18 15:34:16.000000 abmarl-0.2.5/abmarl/trainers/monte_carlo.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/
--rw-r--r--   0 rusu1    (58596)    58596     4390 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/PKG-INFO
--rw-r--r--   0 rusu1    (58596)    58596     3658 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/SOURCES.txt
--rw-r--r--   0 rusu1    (58596)    58596        1 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/dependency_links.txt
--rw-r--r--   0 rusu1    (58596)    58596       54 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/entry_points.txt
--rw-r--r--   0 rusu1    (58596)    58596       91 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/requires.txt
--rw-r--r--   0 rusu1    (58596)    58596       22 2023-01-06 01:45:28.000000 abmarl-0.2.5/abmarl.egg-info/top_level.txt
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/examples/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/examples/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     1205 2022-08-02 17:16:47.000000 abmarl-0.2.5/examples/analysis_prototype.py
--rw-r--r--   0 rusu1    (58596)    58596     2351 2022-08-02 17:16:47.000000 abmarl-0.2.5/examples/config_prototype.py
--rw-r--r--   0 rusu1    (58596)    58596      856 2022-10-15 14:07:02.000000 abmarl-0.2.5/examples/debug_example.py
--rw-r--r--   0 rusu1    (58596)    58596     2214 2022-10-07 22:20:01.000000 abmarl-0.2.5/examples/maze_navigation_example.py
--rw-r--r--   0 rusu1    (58596)    58596     1555 2023-01-06 01:43:01.000000 abmarl-0.2.5/examples/multi_corridor_example.py
--rw-r--r--   0 rusu1    (58596)    58596     2753 2022-10-06 21:02:41.000000 abmarl-0.2.5/examples/reach_the_target_example.py
--rw-r--r--   0 rusu1    (58596)    58596     2656 2022-08-18 15:34:16.000000 abmarl-0.2.5/examples/team_battle_example.py
--rw-r--r--   0 rusu1    (58596)    58596     2920 2022-08-18 15:34:16.000000 abmarl-0.2.5/examples/team_battle_super_agent.py
--rw-r--r--   0 rusu1    (58596)    58596       38 2023-01-06 01:45:28.000000 abmarl-0.2.5/setup.cfg
--rw-r--r--   0 rusu1    (58596)    58596     1432 2023-01-06 01:43:01.000000 abmarl-0.2.5/setup.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/__init__.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/policies/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/policies/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     5042 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/policies/test_q_table_policy.py
--rw-r--r--   0 rusu1    (58596)    58596     1016 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/policies/test_random_policy.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/sim/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/sim/__init__.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/sim/gridworld/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/sim/gridworld/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596    40226 2022-10-07 02:49:32.000000 abmarl-0.2.5/tests/sim/gridworld/test_actor.py
--rw-r--r--   0 rusu1    (58596)    58596     4572 2022-09-22 18:22:42.000000 abmarl-0.2.5/tests/sim/gridworld/test_agent.py
--rw-r--r--   0 rusu1    (58596)    58596     1336 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/sim/gridworld/test_done.py
--rw-r--r--   0 rusu1    (58596)    58596     3821 2022-10-07 22:08:54.000000 abmarl-0.2.5/tests/sim/gridworld/test_grid.py
--rw-r--r--   0 rusu1    (58596)    58596    30064 2022-10-12 18:42:22.000000 abmarl-0.2.5/tests/sim/gridworld/test_observer.py
--rw-r--r--   0 rusu1    (58596)    58596     1735 2022-09-26 17:32:33.000000 abmarl-0.2.5/tests/sim/gridworld/test_state.py
--rw-r--r--   0 rusu1    (58596)    58596     9745 2022-10-07 02:49:32.000000 abmarl-0.2.5/tests/sim/gridworld/test_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     6594 2022-10-03 15:03:13.000000 abmarl-0.2.5/tests/sim/test_agent_based_simulation.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/sim/wrappers/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/sim/wrappers/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596    11612 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/sim/wrappers/test_super_agent_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     8183 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_all_step_multi_corridor.py
--rw-r--r--   0 rusu1    (58596)    58596     8035 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_communication_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     2974 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_dynamic_order_manager.py
--rw-r--r--   0 rusu1    (58596)    58596    14211 2022-12-05 20:26:07.000000 abmarl-0.2.5/tests/test_flatten_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596      772 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/test_generate_episode.py
--rw-r--r--   0 rusu1    (58596)    58596      773 2022-09-30 18:08:40.000000 abmarl-0.2.5/tests/test_gym_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596    12532 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_multi_corridor.py
--rw-r--r--   0 rusu1    (58596)    58596     1039 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_off_policy_monte_carlo.py
--rw-r--r--   0 rusu1    (58596)    58596    10175 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_ravel_discrete_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     9610 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_sar_wrapper.py
--rw-r--r--   0 rusu1    (58596)    58596     1220 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_simulation_manager_corridor.py
--rw-r--r--   0 rusu1    (58596)    58596     8913 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/test_turn_based_multi_corridor.py
-drwxr-xr-x   0 rusu1    (58596)    58596        0 2023-01-06 01:45:28.000000 abmarl-0.2.5/tests/trainers/
--rw-r--r--   0 rusu1    (58596)    58596        0 2022-08-02 17:16:47.000000 abmarl-0.2.5/tests/trainers/__init__.py
--rw-r--r--   0 rusu1    (58596)    58596     4412 2022-10-07 17:35:12.000000 abmarl-0.2.5/tests/trainers/test_debug_trainer.py
--rw-r--r--   0 rusu1    (58596)    58596      938 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/trainers/test_monte_carlo.py
--rw-r--r--   0 rusu1    (58596)    58596     7323 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/trainers/test_multi_policy_trainer.py
--rw-r--r--   0 rusu1    (58596)    58596     4567 2022-08-18 15:34:16.000000 abmarl-0.2.5/tests/trainers/test_single_policy_trainer.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.909943 abmarl-0.2.6/
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2255 2022-10-11 17:26:44.000000 abmarl-0.2.6/LICENSE
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1166 2022-10-11 17:26:44.000000 abmarl-0.2.6/NOTICE
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4442 2023-06-22 22:08:13.908946 abmarl-0.2.6/PKG-INFO
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3441 2023-05-02 17:19:22.000000 abmarl-0.2.6/README.md
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.424900 abmarl-0.2.6/abmarl/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/__init__.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.452900 abmarl-0.2.6/abmarl/algs/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/algs/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2852 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/algs/monte_carlo.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      807 2023-05-02 17:19:22.000000 abmarl-0.2.6/abmarl/debug.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.456900 abmarl-0.2.6/abmarl/examples/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      402 2023-05-23 19:30:55.000000 abmarl-0.2.6/abmarl/examples/__init__.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.497901 abmarl-0.2.6/abmarl/examples/sim/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      536 2023-05-23 19:30:55.000000 abmarl-0.2.6/abmarl/examples/sim/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    13354 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/examples/sim/comms_blocking.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1970 2023-05-23 19:30:55.000000 abmarl-0.2.6/abmarl/examples/sim/maze_navigation.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      788 2023-05-08 22:54:58.000000 abmarl-0.2.6/abmarl/examples/sim/multi_agent_grid_sim.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8336 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/examples/sim/multi_agent_sim.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     7057 2023-06-06 20:58:33.000000 abmarl-0.2.6/abmarl/examples/sim/multi_corridor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2272 2023-06-22 19:03:53.000000 abmarl-0.2.6/abmarl/examples/sim/multi_maze_navigation.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     5882 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/examples/sim/reach_the_target.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3299 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/examples/sim/team_battle_example.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.516953 abmarl-0.2.6/abmarl/external/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      152 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/external/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2200 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/external/gym_env_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    12105 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/external/open_spiel_env_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1511 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/external/rllib_multiagentenv_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4548 2023-03-02 21:37:39.000000 abmarl-0.2.6/abmarl/make_runnable.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.538941 abmarl-0.2.6/abmarl/managers/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      199 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/managers/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3688 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/managers/all_step_manager.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4066 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/managers/dynamic_order_manager.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1687 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/managers/simulation_manager.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4288 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/managers/turn_based_manager.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.555899 abmarl-0.2.6/abmarl/policies/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      114 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/policies/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2720 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/policies/policy.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3810 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/policies/q_table_policy.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1152 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/policies/rllib_policy.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.585920 abmarl-0.2.6/abmarl/scripts/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/scripts/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      785 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/scripts/analyze_script.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1162 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/scripts/debug_script.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1240 2023-03-02 21:37:39.000000 abmarl-0.2.6/abmarl/scripts/make_runnable_script.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2088 2023-03-02 21:37:39.000000 abmarl-0.2.6/abmarl/scripts/scripts.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      473 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/scripts/train_script.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1669 2023-06-13 18:38:05.000000 abmarl-0.2.6/abmarl/scripts/visualize_script.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.599540 abmarl-0.2.6/abmarl/sim/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      139 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/sim/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     9551 2023-05-09 17:14:56.000000 abmarl-0.2.6/abmarl/sim/agent_based_simulation.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.636559 abmarl-0.2.6/abmarl/sim/gridworld/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/sim/gridworld/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    27414 2023-06-22 22:05:47.000000 abmarl-0.2.6/abmarl/sim/gridworld/actor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8439 2023-05-03 18:54:47.000000 abmarl-0.2.6/abmarl/sim/gridworld/agent.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    11297 2023-06-12 22:20:53.000000 abmarl-0.2.6/abmarl/sim/gridworld/base.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3396 2023-05-24 17:32:13.000000 abmarl-0.2.6/abmarl/sim/gridworld/done.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4818 2023-05-10 20:08:43.000000 abmarl-0.2.6/abmarl/sim/gridworld/grid.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    14622 2023-06-22 22:05:47.000000 abmarl-0.2.6/abmarl/sim/gridworld/observer.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    15682 2023-06-22 22:05:47.000000 abmarl-0.2.6/abmarl/sim/gridworld/state.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    10199 2023-05-23 19:30:55.000000 abmarl-0.2.6/abmarl/sim/gridworld/utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    10483 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/sim/gridworld/wrapper.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.667553 abmarl-0.2.6/abmarl/sim/wrappers/
+-rw-------   0 rusu1    (58596) rusu1    (58596)      327 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/sim/wrappers/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4829 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/sim/wrappers/communication_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8247 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/sim/wrappers/flatten_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     7444 2023-05-03 18:11:50.000000 abmarl-0.2.6/abmarl/sim/wrappers/ravel_discrete_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2144 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/sim/wrappers/sar_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    13304 2023-06-06 19:20:54.000000 abmarl-0.2.6/abmarl/sim/wrappers/super_agent_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1520 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/sim/wrappers/wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     5568 2023-06-13 18:38:05.000000 abmarl-0.2.6/abmarl/stage.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.685951 abmarl-0.2.6/abmarl/tools/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/tools/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1810 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/tools/gym_utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      666 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/tools/matplotlib_utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      766 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/tools/numpy_utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2201 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/tools/utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      946 2022-10-11 17:26:44.000000 abmarl-0.2.6/abmarl/train.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.703956 abmarl-0.2.6/abmarl/trainers/
+-rw-------   0 rusu1    (58596) rusu1    (58596)       90 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/trainers/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8535 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/trainers/base.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3672 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/trainers/debug.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1390 2023-05-02 17:19:23.000000 abmarl-0.2.6/abmarl/trainers/monte_carlo.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.450541 abmarl-0.2.6/abmarl.egg-info/
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4442 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/PKG-INFO
+-rw-------   0 rusu1    (58596) rusu1    (58596)     3816 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/SOURCES.txt
+-rw-------   0 rusu1    (58596) rusu1    (58596)        1 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/dependency_links.txt
+-rw-------   0 rusu1    (58596) rusu1    (58596)       54 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/entry_points.txt
+-rw-------   0 rusu1    (58596) rusu1    (58596)       93 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/requires.txt
+-rw-------   0 rusu1    (58596) rusu1    (58596)       22 2023-06-22 22:08:13.000000 abmarl-0.2.6/abmarl.egg-info/top_level.txt
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.756947 abmarl-0.2.6/examples/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/examples/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1205 2022-10-11 17:26:44.000000 abmarl-0.2.6/examples/analysis_prototype.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2351 2023-05-02 17:19:23.000000 abmarl-0.2.6/examples/config_prototype.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      856 2023-05-02 17:19:23.000000 abmarl-0.2.6/examples/debug_example.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2216 2023-05-23 19:30:55.000000 abmarl-0.2.6/examples/maze_navigation_example.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1555 2023-06-06 15:13:29.000000 abmarl-0.2.6/examples/multi_corridor_example.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2506 2023-06-22 19:14:02.000000 abmarl-0.2.6/examples/multi_maze_navigation_rllib.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2753 2023-05-10 20:08:43.000000 abmarl-0.2.6/examples/reach_the_target_example.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2691 2023-06-06 19:20:54.000000 abmarl-0.2.6/examples/team_battle_example.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2965 2023-06-06 19:20:54.000000 abmarl-0.2.6/examples/team_battle_super_agent.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)       38 2023-06-22 22:08:13.910951 abmarl-0.2.6/setup.cfg
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1534 2023-06-22 22:05:47.000000 abmarl-0.2.6/setup.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.809940 abmarl-0.2.6/tests/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/__init__.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.827951 abmarl-0.2.6/tests/policies/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/policies/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     5042 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/policies/test_q_table_policy.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1016 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/policies/test_random_policy.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.828940 abmarl-0.2.6/tests/sim/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/sim/__init__.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.874908 abmarl-0.2.6/tests/sim/gridworld/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/sim/gridworld/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    44627 2023-05-10 20:08:43.000000 abmarl-0.2.6/tests/sim/gridworld/test_actor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4572 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/sim/gridworld/test_agent.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    23319 2023-05-10 20:08:43.000000 abmarl-0.2.6/tests/sim/gridworld/test_base.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4691 2023-05-23 20:44:48.000000 abmarl-0.2.6/tests/sim/gridworld/test_done.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4073 2023-05-10 20:08:43.000000 abmarl-0.2.6/tests/sim/gridworld/test_grid.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    34358 2023-05-10 20:08:43.000000 abmarl-0.2.6/tests/sim/gridworld/test_observer.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    17737 2023-05-23 19:30:55.000000 abmarl-0.2.6/tests/sim/gridworld/test_state.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1034 2023-05-23 19:30:55.000000 abmarl-0.2.6/tests/sim/gridworld/test_utils.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     9745 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/sim/gridworld/test_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     6594 2023-05-03 18:11:50.000000 abmarl-0.2.6/tests/sim/test_agent_based_simulation.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.882900 abmarl-0.2.6/tests/sim/wrappers/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/sim/wrappers/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    11659 2023-06-06 19:20:54.000000 abmarl-0.2.6/tests/sim/wrappers/test_super_agent_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    10714 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_all_step_multi_corridor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8035 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_communication_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     2974 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_dynamic_order_manager.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    14211 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_flatten_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      772 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/test_generate_episode.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      773 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_gym_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    12532 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_multi_corridor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1039 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_off_policy_monte_carlo.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)    10175 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_ravel_discrete_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     9610 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_sar_wrapper.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     1220 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_simulation_manager_corridor.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     8913 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/test_turn_based_multi_corridor.py
+drwx--S---   0 rusu1    (58596) rusu1    (58596)        0 2023-06-22 22:08:13.904941 abmarl-0.2.6/tests/trainers/
+-rw-------   0 rusu1    (58596) rusu1    (58596)        0 2022-10-11 17:26:44.000000 abmarl-0.2.6/tests/trainers/__init__.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4412 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/trainers/test_debug_trainer.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)      938 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/trainers/test_monte_carlo.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     7323 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/trainers/test_multi_policy_trainer.py
+-rw-------   0 rusu1    (58596) rusu1    (58596)     4567 2023-05-02 17:19:23.000000 abmarl-0.2.6/tests/trainers/test_single_policy_trainer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `abmarl-0.2.5/LICENSE` & `abmarl-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/NOTICE` & `abmarl-0.2.6/NOTICE`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/PKG-INFO` & `abmarl-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: abmarl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Agent Based Simulation and MultiAgent Reinforcement Learning
 Home-page: https://github.com/llnl/abmarl
 Author: Edward Rusu
 Author-email: rusu1@llnl.gov
 License: BSD 3
 Project-URL: Featured Usage, https://abmarl.readthedocs.io/en/latest/featured_usage.html
 Project-URL: Documentation, https://abmarl.readthedocs.io/en/latest/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.9
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Abmarl
 
 Abmarl is a package for developing Agent-Based Simulations and training them with
@@ -46,15 +48,14 @@
 
 
 ## Quickstart
 
 To use Abmarl, install via pip: `pip install abmarl`
 
 To develop Abmarl, clone the repository and install via pip's development mode.
-Note: Abmarl requires `python3.7` or `python3.8`.
 
 ```
 git clone git@github.com:LLNL/Abmarl.git
 cd abmarl
 pip install -r requirements.txt
 pip install -e . --no-deps
 ```
```

### Comparing `abmarl-0.2.5/README.md` & `abmarl-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 ## Quickstart
 
 To use Abmarl, install via pip: `pip install abmarl`
 
 To develop Abmarl, clone the repository and install via pip's development mode.
-Note: Abmarl requires `python3.7` or `python3.8`.
 
 ```
 git clone git@github.com:LLNL/Abmarl.git
 cd abmarl
 pip install -r requirements.txt
 pip install -e . --no-deps
 ```
```

### Comparing `abmarl-0.2.5/abmarl/algs/monte_carlo.py` & `abmarl-0.2.6/abmarl/algs/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/debug.py` & `abmarl-0.2.6/abmarl/debug.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/examples/sim/comms_blocking.py` & `abmarl-0.2.6/abmarl/examples/sim/comms_blocking.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/examples/sim/maze_navigation.py` & `abmarl-0.2.6/abmarl/examples/sim/maze_navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class MazeNavigationAgent(GridObservingAgent, MovingAgent):
     def __init__(self, **kwargs):
         super().__init__(move_range=1, **kwargs)
 
 
-class MazeNaviationSim(GridWorldSimulation):
+class MazeNavigationSim(GridWorldSimulation):
     def __init__(self, **kwargs):
         self.agents = kwargs['agents']
         self.navigator = kwargs['agents']['navigator']
         self.target = kwargs['agents']['target']
 
         # State Components
         self.position_state = PositionState(**kwargs)
```

### Comparing `abmarl-0.2.5/abmarl/examples/sim/multi_agent_sim.py` & `abmarl-0.2.6/abmarl/examples/sim/multi_agent_sim.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/examples/sim/multi_corridor.py` & `abmarl-0.2.6/abmarl/examples/sim/multi_corridor.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,25 @@
         for i, agent in enumerate(self.agents.values()):
             agent.position = location_sample[i]
             self.corridor[location_sample[i]] = agent
 
         # Track the agents' rewards over multiple steps.
         self.reward = {agent_id: 0 for agent_id in self.agents}
 
+        # Track the last actions that were given to the simulation.
+        self._last_action = {agent_id: None for agent_id in self.agents}
+
     def step(self, action_dict, **kwargs):
         """
         The agents can choose to move left, move right, or stay where they are. If
         an agent bumps into another agent, then both agents receive a penalty.
         The offending agent receives a larger penalty than the offended agent.
         The agent is done when it reaches the end of the corridor.
         """
+        self._last_action = action_dict
         for agent_id, action in action_dict.items():
             agent = self.agents[agent_id]
             if action == self.Actions.LEFT:
                 if agent.position != 0 and self.corridor[agent.position-1] is None:
                     # Good move, no extra penalty
                     self.corridor[agent.position] = None
                     agent.position -= 1
```

### Comparing `abmarl-0.2.5/abmarl/examples/sim/reach_the_target.py` & `abmarl-0.2.6/abmarl/examples/sim/reach_the_target.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/examples/sim/team_battle_example.py` & `abmarl-0.2.6/abmarl/examples/sim/team_battle_example.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/external/gym_env_wrapper.py` & `abmarl-0.2.6/abmarl/external/gym_env_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/external/open_spiel_env_wrapper.py` & `abmarl-0.2.6/abmarl/external/open_spiel_env_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/external/rllib_multiagentenv_wrapper.py` & `abmarl-0.2.6/abmarl/external/rllib_multiagentenv_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/make_runnable.py` & `abmarl-0.2.6/abmarl/make_runnable.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/managers/dynamic_order_manager.py` & `abmarl-0.2.6/abmarl/managers/dynamic_order_manager.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/managers/simulation_manager.py` & `abmarl-0.2.6/abmarl/managers/simulation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     flow.
 
     Attributes:
         sim: The AgentBasedSimulation.
         agents: The agents that are in the AgentBasedSimulation.
         done_agents: Set of agents that are done.
     """
-    def __init__(self, sim):
+    def __init__(self, sim, **kwargs):
         assert isinstance(sim, AgentBasedSimulation), \
             "SimulationManager can only interface with AgentBasedSimulation."
         self.sim = sim
         self.agents = sim.agents
         self.done_agents = set()
 
     @abstractmethod
```

### Comparing `abmarl-0.2.5/abmarl/managers/turn_based_manager.py` & `abmarl-0.2.6/abmarl/managers/turn_based_manager.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/policies/policy.py` & `abmarl-0.2.6/abmarl/policies/policy.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/policies/q_table_policy.py` & `abmarl-0.2.6/abmarl/policies/q_table_policy.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/policies/rllib_policy.py` & `abmarl-0.2.6/abmarl/policies/rllib_policy.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/scripts/analyze_script.py` & `abmarl-0.2.6/abmarl/scripts/analyze_script.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/scripts/debug_script.py` & `abmarl-0.2.6/abmarl/scripts/debug_script.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/scripts/make_runnable_script.py` & `abmarl-0.2.6/abmarl/scripts/make_runnable_script.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/scripts/scripts.py` & `abmarl-0.2.6/abmarl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/scripts/visualize_script.py` & `abmarl-0.2.6/abmarl/scripts/visualize_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     )
     visualize_parser.add_argument(
         '-s', '--steps-per-episode', type=int, default=200,
         help='The maximum number of steps to take per epsiode. Default 200.'
     )
     visualize_parser.add_argument(
         '--record', action='store_true',
-        help='Record a video of the agent(s) interacting in the simulation.'
+        help='Record a video of the agent(s) interacting in the simulation and display it live.'
+    )
+    visualize_parser.add_argument(
+        '--record-only', action='store_true',
+        help='Only record a video of the agent(s) interacting in the simulation. No live display.'
     )
     visualize_parser.add_argument(
         '--frame-delay', type=int,
         help='The number of milliseconds to delay between each frame in the animation.',
         default=200
     )
     visualize_parser.add_argument(
```

### Comparing `abmarl-0.2.5/abmarl/sim/agent_based_simulation.py` & `abmarl-0.2.6/abmarl/sim/agent_based_simulation.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/gridworld/actor.py` & `abmarl-0.2.6/abmarl/sim/gridworld/actor.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,14 +109,94 @@
                     return True
                 else:
                     return False
             else:
                 return False
 
 
+class CrossMoveActor(ActorBaseComponent):
+    """
+    Agents can move up, down, left, right, or stay in place.
+    """
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        for agent in self.agents.values():
+            if isinstance(agent, self.supported_agent_type):
+                agent.action_space[self.key] = Discrete(5)
+                agent.null_action[self.key] = 0
+
+    @property
+    def key(self):
+        """
+        This Actors key is "move".
+        """
+        return "move"
+
+    @property
+    def supported_agent_type(self):
+        """
+        This Actor works with MovingAgent, but the move_range parameter is ignored.
+        """
+        return MovingAgent
+
+    def grid_action(self, cross_action):
+        """
+        Grid action converts the cross action to an action in the grid.
+
+        0: Stay
+        1: Move up
+        2: Move right
+        3; Move down
+        4: Move left
+        """
+        assert cross_action in [0, 1, 2, 3, 4], "Cross action must be 0, 1, 2, 3, or 4."
+        return {
+            0: np.array((0, 0)), # Stay
+            1: np.array([0, -1]), # Up
+            2: np.array([1, 0]), # Right
+            3: np.array([0, 1]), # Down
+            4: np.array([-1, 0]), # Left
+        }[cross_action]
+
+    def process_action(self, agent, action_dict, **kwargs):
+        """
+        The agent can move up, down, left, right, or stay in place.
+
+        The agent's new position must be within the grid and the cell-occupation rules
+        must be met.
+
+        Args:
+            agent: Move the agent if it is a MovingAgent.
+            action_dict: The action dictionary for this agent in this step. If
+                the agent is a MovingAgent, then the action dictionary will contain
+                the "move" entry.
+
+        Returns:
+            True if the move is successful, False otherwise.
+        """
+        if isinstance(agent, self.supported_agent_type):
+            cross_action = action_dict[self.key]
+            action = self.grid_action(cross_action)
+            new_position = agent.position + action
+            if 0 <= new_position[0] < self.rows and \
+                    0 <= new_position[1] < self.cols:
+                from_ndx = tuple(agent.position)
+                to_ndx = tuple(new_position)
+                if to_ndx == from_ndx:
+                    return True
+                elif self.grid.query(agent, to_ndx):
+                    self.grid.remove(agent, from_ndx)
+                    self.grid.place(agent, to_ndx)
+                    return True
+                else:
+                    return False
+            else:
+                return False
+
+
 class AttackActorBaseComponent(ActorBaseComponent, ABC):
     """
     Abstract class that provides the properties and structure for attack actors.
 
     The agent chooses to attack other agents within its surrounding grid. The derived
     attack actor interprets and implements the specific attack. Attacked agents
     have their health reduced by the attacking agent's strength and possibly become
```

### Comparing `abmarl-0.2.5/abmarl/sim/gridworld/agent.py` & `abmarl-0.2.6/abmarl/sim/gridworld/agent.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/gridworld/observer.py` & `abmarl-0.2.6/abmarl/sim/gridworld/observer.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,112 @@
 
         Returns:
             This agent's observation.
         """
         pass
 
 
+class AbsoluteGridObserver(ObserverBaseComponent):
+    """
+    Observe the agents in the grid according to their actual positions.
+
+    This Observer represents agents by their encoding on cells according to their
+    actual positions in the grid.
+    If there are multiple agents on a single cell with different encodings, only
+    a single randomly chosen encoding will be observed. To be consistent with other
+    built-in observers, masked cells are indicated as -2. Typially, -1 is reserved
+    for out of bounds encoding, but because this Observer only reports cells in the
+    grid, we don't need an out of bounds distinction. Instead, in order for the observing
+    agent to identify itself distinctly from other agents of the same encoding,
+    it is reported as a -1.
+    """
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        max_encoding = max([agent.encoding for agent in self.agents.values()])
+        for agent in self.agents.values():
+            if isinstance(agent, self.supported_agent_type):
+                agent.observation_space[self.key] = Box(
+                    -2, max_encoding, (self.rows, self.cols), int
+                )
+                agent.null_observation[self.key] = -2 * np.ones(
+                    (self.rows, self.cols), dtype=int
+                )
+
+    @property
+    def key(self):
+        """
+        This Observer's key is "absolute_grid".
+        """
+        return 'absolute_grid'
+
+    @property
+    def supported_agent_type(self):
+        """
+        This Observer work with GridObservingAgents
+        """
+        return GridObservingAgent
+
+    def get_obs(self, agent, **kwargs):
+        """
+        The agent observes the grid.
+
+        The observation may include the agent itself indicated by a -1, other
+        agents indicated by their encodings, empty space indicated with a 0, and
+        masked cells indicated as -2, which are masked either because they are
+        too far away or because they are blocked from view by view-blocking agents.
+        """
+        if not isinstance(agent, self.supported_agent_type):
+            return {}
+
+        # To generate the observation, we first create a local grid and mask using
+        # the agent's view_range. Then we convolve local grid and mask together.
+        # Finally, we subsitute a portion of the full grid with the local grid.
+
+        # Generate a local grid and an observation mask
+        local_grid, mask = gu.create_grid_and_mask(
+            agent, self.grid, agent.view_range, self.agents
+        )
+
+        # Convolve the local grid observation with the mask.
+        convolved_grid = np.zeros((2 * agent.view_range + 1, 2 * agent.view_range + 1), dtype=int)
+        for r in range(2 * agent.view_range + 1):
+            for c in range(2 * agent.view_range + 1):
+                if mask[r, c]: # We can see this cell
+                    candidate_agents = local_grid[r, c]
+                    if candidate_agents is None: # This cell is out of bounds
+                        continue # Skip this since these cells will be cropped out
+                    elif not candidate_agents: # In bounds empty cell
+                        convolved_grid[r, c] = 0
+                    else: # Observe one of the agents at this cell
+                        # Prioritize observing yourself
+                        if agent.id in candidate_agents:
+                            convolved_grid[r, c] = -1
+                        else:
+                            convolved_grid[r, c] = np.random.choice([
+                                other.encoding
+                                for other in candidate_agents.values()
+                            ])
+                else: # Cell blocked by agent. Indicate invisible with -2
+                    convolved_grid[r, c] = -2
+
+        # Substitute the local grid in place in the full grid
+        obs = -2 * np.ones((self.rows, self.cols), dtype=int)
+        (r, c) = agent.position
+        r_lower = max([0, r - agent.view_range])
+        r_upper = min([self.grid.rows - 1, r + agent.view_range]) + 1
+        c_lower = max([0, c - agent.view_range])
+        c_upper = min([self.grid.cols - 1, c + agent.view_range]) + 1
+        obs[r_lower:r_upper, c_lower:c_upper] = convolved_grid[
+            (r_lower+agent.view_range-r):(r_upper+agent.view_range-r),
+            (c_lower+agent.view_range-c):(c_upper+agent.view_range-c)
+        ]
+
+        return {self.key: obs}
+
+
 class SingleGridObserver(ObserverBaseComponent):
     """
     Observe a subset of the grid centered on the agent's position.
 
     The observation is centered around the observing agent's position. Each agent
     in the "observation window" is recorded in the relative cell using its encoding.
     If there are multiple agents on a single cell with different encodings, the
@@ -241,15 +339,15 @@
     Agents observe their absolute position.
     """
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         for agent in self.agents.values():
             if isinstance(agent, self.supported_agent_type):
                 agent.observation_space[self.key] = Box(
-                    np.array([0, 0], dtype=np.int),
+                    np.array([0, 0], dtype=int),
                     np.array([self.grid.rows - 1, self.grid.cols - 1], dtype=int),
                     dtype=int
                 )
                 agent.null_observation[self.key] = np.zeros((2,), dtype=int)
 
     @property
     def key(self):
```

### Comparing `abmarl-0.2.5/abmarl/sim/gridworld/wrapper.py` & `abmarl-0.2.6/abmarl/sim/gridworld/wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/communication_wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/communication_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/flatten_wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/flatten_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/ravel_discrete_wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/ravel_discrete_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools
 
 import numpy as np
 from gym.spaces import Discrete, MultiDiscrete, MultiBinary, Box, Dict, Tuple
+from gym.spaces.box import get_inf
 
 from abmarl.sim import Agent
 
 from .sar_wrapper import SARWrapper
 
 
 def _ravel_helper(space, point):
@@ -115,18 +116,18 @@
 def _isbounded(space):
     """
     Gym Box converts np.inf to min and max values for integer types. As a result,
     Box.is_bounded doesn't work because it checks for inf, not for min/max values
     of that dtype. This function checks for min/max values of the dtype.
     """
     return space.is_bounded() and \
-        not (space.low == np.iinfo(space.dtype).min).any() and \
-        not (space.low == np.iinfo(space.dtype).max).any() and \
-        not (space.high == np.iinfo(space.dtype).min).any() and \
-        not (space.high == np.iinfo(space.dtype).max).any()
+        not (space.low == get_inf(int, '-')).any() and \
+        not (space.low == get_inf(int, '+')).any() and \
+        not (space.high == get_inf(int, '-')).any() and \
+        not (space.high == get_inf(int, '+')).any()
 
 
 def check_space(space):
     """
     Ensure that the space is of type that can be ravelled to discrete value.
     """
     if isinstance(space, Discrete) or isinstance(space, MultiDiscrete) or \
```

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/sar_wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/sar_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/super_agent_wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/super_agent_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import warnings
 
-from gym.spaces import Dict, Discrete
+from gym.spaces import Dict, MultiBinary
 
 from abmarl.sim.agent_based_simulation import Agent
 from abmarl.sim.wrappers import Wrapper
 from abmarl.tools import gym_utils as gu
 
 
 class SuperAgentWrapper(Wrapper):
@@ -149,22 +149,22 @@
         # the observation space
         if agent_id in self.super_agent_mapping:
             obs = {'mask': {}}
             for covered_agent in self.super_agent_mapping[agent_id]:
                 if self.sim.get_done(covered_agent, **kwargs):
                     if self._last_obs_reported[covered_agent]:
                         obs[covered_agent] = self._get_null_obs(covered_agent, **kwargs)
-                        obs['mask'][covered_agent] = False
+                        obs['mask'][covered_agent] = [False]
                     else:
                         obs[covered_agent] = self.sim.get_obs(covered_agent, **kwargs)
-                        obs['mask'][covered_agent] = False
+                        obs['mask'][covered_agent] = [False]
                         self._last_obs_reported[covered_agent] = True
                 else:
                     obs[covered_agent] = self.sim.get_obs(covered_agent, **kwargs)
-                    obs['mask'][covered_agent] = True
+                    obs['mask'][covered_agent] = [True]
             return obs
         else:
             return self.sim.get_obs(agent_id, **kwargs)
 
     def get_reward(self, agent_id, **kwargs):
         """
         Report the agent's reward.
@@ -249,15 +249,15 @@
         # Construct the agent dict with super agents
         for super_agent_id, covered_agent_list in self.super_agent_mapping.items():
             # Construct a mapping from the super agents to the covered agents' observation
             # and action spaces
             obs_mapping = {'mask': {}}
             for covered_agent_id in covered_agent_list:
                 obs_mapping[covered_agent_id] = self.sim.agents[covered_agent_id].observation_space
-                obs_mapping['mask'][covered_agent_id] = Discrete(2)
+                obs_mapping['mask'][covered_agent_id] = MultiBinary(1)
             action_mapping = {
                 covered_agent_id: self.sim.agents[covered_agent_id].action_space
                 for covered_agent_id in covered_agent_list
             }
             agents[super_agent_id] = Agent(
                 id=super_agent_id,
                 observation_space=gu.make_dict(obs_mapping),
```

### Comparing `abmarl-0.2.5/abmarl/sim/wrappers/wrapper.py` & `abmarl-0.2.6/abmarl/sim/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/stage.py` & `abmarl-0.2.6/abmarl/stage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+import matplotlib
+
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 import ray
 import ray.rllib
 from ray.rllib.env import MultiAgentEnv
 from ray.tune.registry import get_trainable_cls
 
@@ -67,14 +69,22 @@
     analysis_mod.run(sim, trainer)
 
     _finish()
 
 
 def run_visualize(full_trained_directory, parameters):
     """Visualize MARL policies from a saved policy"""
+    if parameters.record_only:
+        matplotlib.use("Agg")
+    else:
+        try:
+            matplotlib.use("macosx")
+        except ImportError:
+            matplotlib.use('TkAgg')
+
     sim, trainer = _start(full_trained_directory, parameters.checkpoint, seed=parameters.seed)
 
     # Determine if we are single- or multi-agent case.
     def _multi_get_action(obs, done=None, sim=None, policy_agent_mapping=None, **kwargs):
         joint_action = {}
         if done is None:
             done = {agent: False for agent in obs}
@@ -118,30 +128,35 @@
             while not all_done:
                 i += 1
                 yield i
 
         def animate(i):
             nonlocal obs, done
             sim.render(fig=fig)
-            plt.pause(1e-16)
+            if not parameters.record_only:
+                plt.pause(1e-16)
             action = _get_action(
                 obs, done=done, sim=sim, trainer=trainer, policy_agent_mapping=policy_agent_mapping
             )
             obs, _, done, _ = sim.step(action)
             if _get_done(done) or i >= parameters.steps_per_episode:
                 nonlocal all_done
                 all_done = True
                 sim.render(fig=fig)
-                plt.pause(1e-16)
+                if not parameters.record_only:
+                    plt.pause(1e-16)
 
         anim = FuncAnimation(
             fig, animate, frames=gen_frame_until_done, repeat=False,
-            interval=parameters.frame_delay
+            interval=parameters.frame_delay, cache_frame_data=False
         )
         if parameters.record:
-            anim.save(os.path.join(full_trained_directory, 'Episode_{}.mp4'.format(episode)))
-        plt.show(block=False)
+            anim.save(os.path.join(full_trained_directory, 'Episode_{}.gif'.format(episode)))
+            plt.show(block=False)
+        elif parameters.record_only:
+            anim.save(os.path.join(full_trained_directory, 'Episode_{}.gif'.format(episode)))
+
         while not all_done:
             plt.pause(1)
         plt.close(fig)
 
     _finish()
```

### Comparing `abmarl-0.2.5/abmarl/tools/gym_utils.py` & `abmarl-0.2.6/abmarl/tools/gym_utils.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/tools/matplotlib_utils.py` & `abmarl-0.2.6/abmarl/tools/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/tools/numpy_utils.py` & `abmarl-0.2.6/abmarl/tools/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/tools/utils.py` & `abmarl-0.2.6/abmarl/tools/utils.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/train.py` & `abmarl-0.2.6/abmarl/train.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/trainers/base.py` & `abmarl-0.2.6/abmarl/trainers/base.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/trainers/debug.py` & `abmarl-0.2.6/abmarl/trainers/debug.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl/trainers/monte_carlo.py` & `abmarl-0.2.6/abmarl/trainers/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/abmarl.egg-info/PKG-INFO` & `abmarl-0.2.6/abmarl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: abmarl
-Version: 0.2.5
+Version: 0.2.6
 Summary: Agent Based Simulation and MultiAgent Reinforcement Learning
 Home-page: https://github.com/llnl/abmarl
 Author: Edward Rusu
 Author-email: rusu1@llnl.gov
 License: BSD 3
 Project-URL: Featured Usage, https://abmarl.readthedocs.io/en/latest/featured_usage.html
 Project-URL: Documentation, https://abmarl.readthedocs.io/en/latest/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.9
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Abmarl
 
 Abmarl is a package for developing Agent-Based Simulations and training them with
@@ -46,15 +48,14 @@
 
 
 ## Quickstart
 
 To use Abmarl, install via pip: `pip install abmarl`
 
 To develop Abmarl, clone the repository and install via pip's development mode.
-Note: Abmarl requires `python3.7` or `python3.8`.
 
 ```
 git clone git@github.com:LLNL/Abmarl.git
 cd abmarl
 pip install -r requirements.txt
 pip install -e . --no-deps
 ```
```

### Comparing `abmarl-0.2.5/abmarl.egg-info/SOURCES.txt` & `abmarl-0.2.6/abmarl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 abmarl.egg-info/top_level.txt
 abmarl/algs/__init__.py
 abmarl/algs/monte_carlo.py
 abmarl/examples/__init__.py
 abmarl/examples/sim/__init__.py
 abmarl/examples/sim/comms_blocking.py
 abmarl/examples/sim/maze_navigation.py
+abmarl/examples/sim/multi_agent_grid_sim.py
 abmarl/examples/sim/multi_agent_sim.py
 abmarl/examples/sim/multi_corridor.py
+abmarl/examples/sim/multi_maze_navigation.py
 abmarl/examples/sim/reach_the_target.py
 abmarl/examples/sim/team_battle_example.py
 abmarl/external/__init__.py
 abmarl/external/gym_env_wrapper.py
 abmarl/external/open_spiel_env_wrapper.py
 abmarl/external/rllib_multiagentenv_wrapper.py
 abmarl/managers/__init__.py
 abmarl/managers/all_step_manager.py
 abmarl/managers/dynamic_order_manager.py
 abmarl/managers/simulation_manager.py
 abmarl/managers/turn_based_manager.py
 abmarl/policies/__init__.py
-abmarl/policies/interactive_policy.py
 abmarl/policies/policy.py
 abmarl/policies/q_table_policy.py
 abmarl/policies/rllib_policy.py
 abmarl/scripts/__init__.py
 abmarl/scripts/analyze_script.py
 abmarl/scripts/debug_script.py
 abmarl/scripts/make_runnable_script.py
@@ -74,14 +75,15 @@
 abmarl/trainers/monte_carlo.py
 examples/__init__.py
 examples/analysis_prototype.py
 examples/config_prototype.py
 examples/debug_example.py
 examples/maze_navigation_example.py
 examples/multi_corridor_example.py
+examples/multi_maze_navigation_rllib.py
 examples/reach_the_target_example.py
 examples/team_battle_example.py
 examples/team_battle_super_agent.py
 tests/__init__.py
 tests/test_all_step_multi_corridor.py
 tests/test_communication_wrapper.py
 tests/test_dynamic_order_manager.py
@@ -98,18 +100,20 @@
 tests/policies/test_q_table_policy.py
 tests/policies/test_random_policy.py
 tests/sim/__init__.py
 tests/sim/test_agent_based_simulation.py
 tests/sim/gridworld/__init__.py
 tests/sim/gridworld/test_actor.py
 tests/sim/gridworld/test_agent.py
+tests/sim/gridworld/test_base.py
 tests/sim/gridworld/test_done.py
 tests/sim/gridworld/test_grid.py
 tests/sim/gridworld/test_observer.py
 tests/sim/gridworld/test_state.py
+tests/sim/gridworld/test_utils.py
 tests/sim/gridworld/test_wrapper.py
 tests/sim/wrappers/__init__.py
 tests/sim/wrappers/test_super_agent_wrapper.py
 tests/trainers/__init__.py
 tests/trainers/test_debug_trainer.py
 tests/trainers/test_monte_carlo.py
 tests/trainers/test_multi_policy_trainer.py
```

### Comparing `abmarl-0.2.5/examples/analysis_prototype.py` & `abmarl-0.2.6/examples/analysis_prototype.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/examples/config_prototype.py` & `abmarl-0.2.6/examples/config_prototype.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/examples/debug_example.py` & `abmarl-0.2.6/examples/debug_example.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/examples/maze_navigation_example.py` & `abmarl-0.2.6/examples/maze_navigation_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from abmarl.examples import MazeNavigationAgent, MazeNaviationSim
+from abmarl.examples import MazeNavigationAgent, MazeNavigationSim
 from abmarl.sim.gridworld.agent import GridWorldAgent
 from abmarl.managers import AllStepManager
 from abmarl.external import MultiAgentWrapper
 
 object_registry = {
     'N': lambda n: MazeNavigationAgent(
         id='navigator',
@@ -23,18 +23,18 @@
         render_shape='s'
     )
 }
 
 file_name = 'maze.txt'
 sim = MultiAgentWrapper(
     AllStepManager(
-        MazeNaviationSim.build_sim_from_file(
+        MazeNavigationSim.build_sim_from_file(
             file_name,
             object_registry,
-            overlapping={1: [3], 3: [1]}
+            overlapping={1: {3}, 3: {1}}
         )
     )
 )
 
 
 sim_name = "MazeNavigation"
 from ray.tune.registry import register_env
```

### Comparing `abmarl-0.2.5/examples/multi_corridor_example.py` & `abmarl-0.2.6/examples/multi_corridor_example.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/examples/reach_the_target_example.py` & `abmarl-0.2.6/examples/reach_the_target_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         attack_range=1,
         attack_strength=1,
         attack_accuracy=1,
         initial_position=np.array([int(grid_size / 2), int(grid_size / 2)], dtype=int)
     )
 }
 overlapping = {
-    2: [3],
-    3: [1, 2, 3]
+    2: {3},
+    3: {1, 2, 3}
 }
 attack_mapping = {
     2: [3]
 }
 
 sim = MultiAgentWrapper(
     AllStepManager(
```

### Comparing `abmarl-0.2.5/examples/team_battle_example.py` & `abmarl-0.2.6/examples/team_battle_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         id=f'agent{i}',
         encoding=i % 4 + 1,
         render_color=colors[i % 4],
         initial_position=positions[i % 4]
     ) for i in range(24)
 }
 overlap_map = {
-    1: [1],
-    2: [2],
-    3: [3],
-    4: [4]
+    1: {1},
+    2: {2},
+    3: {3},
+    4: {4}
 }
 attack_map = {
     1: [2, 3, 4],
     2: [1, 3, 4],
     3: [1, 2, 4],
     4: [1, 2, 3]
 }
@@ -74,14 +74,15 @@
         'run_or_experiment': 'A2C',
         'checkpoint_freq': 50,
         'checkpoint_at_end': True,
         'stop': {
             'episodes_total': 2000,
         },
         'verbose': 2,
+        'local_dir': 'output_dir',
         'config': {
             # --- Simulation ---
             'disable_env_checking': False,
             'env': sim_name,
             'horizon': 200,
             'env_config': {},
             # --- Multiagent ---
```

### Comparing `abmarl-0.2.5/examples/team_battle_super_agent.py` & `abmarl-0.2.6/examples/team_battle_super_agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         id=f'agent{i}',
         encoding=i % 4 + 1,
         render_color=colors[i % 4],
         initial_position=positions[i % 4],
     ) for i in range(24)
 }
 overlap_map = {
-    1: [1],
-    2: [2],
-    3: [3],
-    4: [4]
+    1: {1},
+    2: {2},
+    3: {3},
+    4: {4}
 }
 attack_map = {
     1: [2, 3, 4],
     2: [1, 3, 4],
     3: [1, 2, 4],
     4: [1, 2, 3]
 }
@@ -47,15 +47,15 @@
         ),
         super_agent_mapping=super_agent_mapping,
     )
 )
 sim = MultiAgentWrapper(sim_)
 
 
-sim_name = "TeamBattle"
+sim_name = "TeamBattleSuperAgent"
 from ray.tune.registry import register_env
 register_env(sim_name, lambda sim_config: sim)
 
 
 policies = {
     'red': (None, sim_.agents['red'].observation_space, sim_.agents['red'].action_space, {}),
     'blue': (None, sim_.agents['blue'].observation_space, sim_.agents['blue'].action_space, {}),
@@ -78,14 +78,15 @@
         'run_or_experiment': 'A2C',
         'checkpoint_freq': 50,
         'checkpoint_at_end': True,
         'stop': {
             'episodes_total': 2000,
         },
         'verbose': 2,
+        'local_dir': 'output_dir',
         'config': {
             # --- Simulation ---
             'disable_env_checking': False,
             'env': sim_name,
             'horizon': 200,
             'env_config': {},
             # --- Multiagent ---
```

### Comparing `abmarl-0.2.5/setup.py` & `abmarl-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='abmarl',
-    version='0.2.5',
+    version='0.2.6',
     description='Agent Based Simulation and MultiAgent Reinforcement Learning',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/llnl/abmarl',
     author='Edward Rusu',
     author_email='rusu1@llnl.gov',
     license='BSD 3',
@@ -17,30 +17,32 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     project_urls={
         'Featured Usage': 'https://abmarl.readthedocs.io/en/latest/featured_usage.html',
         'Documentation': 'https://abmarl.readthedocs.io/en/latest/index.html',
     },
     packages=setuptools.find_packages(),
     install_requires=[
         'importlib-metadata<5.0',
+        'numpy<1.24',
         'tensorflow',
-        'gym<0.22',
         'ray[rllib]==2.0.0',
         'open-spiel',
         'matplotlib',
         'seaborn',
     ],
-    python_requires='>=3.7, <3.9',
+    python_requires='>=3.7, <3.11',
     entry_points={
         'console_scripts': [
             'abmarl=abmarl.scripts.scripts:cli'
         ]
     },
 )
```

### Comparing `abmarl-0.2.5/tests/policies/test_q_table_policy.py` & `abmarl-0.2.6/tests/policies/test_q_table_policy.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/policies/test_random_policy.py` & `abmarl-0.2.6/tests/policies/test_random_policy.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/sim/gridworld/test_actor.py` & `abmarl-0.2.6/tests/sim/gridworld/test_actor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from gym.spaces import Box, Discrete, MultiDiscrete, Dict
 import numpy as np
 import pytest
 
-from abmarl.sim.gridworld.actor import MoveActor, BinaryAttackActor, SelectiveAttackActor, \
-    EncodingBasedAttackActor, RestrictedSelectiveAttackActor, ActorBaseComponent
+from abmarl.sim.gridworld.actor import MoveActor, CrossMoveActor, BinaryAttackActor, \
+    SelectiveAttackActor, EncodingBasedAttackActor, RestrictedSelectiveAttackActor, \
+    ActorBaseComponent
 from abmarl.sim.gridworld.state import PositionState, HealthState
 from abmarl.sim.gridworld.agent import MovingAgent, AttackingAgent, HealthAgent
 from abmarl.sim.gridworld.grid import Grid
 
 grid = Grid(5,6)
 
 
@@ -69,17 +70,17 @@
     np.testing.assert_array_equal(agents['agent1'].position, np.array([1, 2]))
     np.testing.assert_array_equal(agents['agent2'].position, np.array([0, 2]))
     np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 2]))
 
 
 def test_move_actor_with_overlap():
     overlapping = {
-        1: [1],
-        2: [3],
-        3: [2]
+        1: {1},
+        2: {3},
+        3: {2}
     }
     grid = Grid(5, 6, overlapping=overlapping)
     agents = {
         'agent0': MovingAgent(
             id='agent0', initial_position=np.array([4, 4]), encoding=1, move_range=1
         ),
         'agent1': MovingAgent(
@@ -120,14 +121,126 @@
         move_actor.process_action(agents[agent_id], action)
     np.testing.assert_array_equal(agents['agent0'].position, np.array([2, 4]))
     np.testing.assert_array_equal(agents['agent1'].position, np.array([2, 2]))
     np.testing.assert_array_equal(agents['agent2'].position, np.array([3, 3]))
     np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 2]))
 
 
+def test_cross_move_actor():
+    agents = {
+        'agent0': MovingAgent(
+            id='agent0', initial_position=np.array([3, 5]), encoding=1, move_range=1
+        ),
+        'agent1': MovingAgent(
+            id='agent1', initial_position=np.array([2, 2]), encoding=2, move_range=2
+        ),
+        'agent2': MovingAgent(
+            id='agent2', initial_position=np.array([0, 1]), encoding=1, move_range=1
+        ),
+        'agent3': MovingAgent(
+            id='agent3', initial_position=np.array([2, 3]), encoding=3, move_range=3
+        ),
+    }
+
+    position_state = PositionState(grid=grid, agents=agents)
+    move_actor = CrossMoveActor(grid=grid, agents=agents)
+    assert isinstance(move_actor, ActorBaseComponent)
+    assert move_actor.key == 'move'
+    assert move_actor.supported_agent_type == MovingAgent
+    assert agents['agent0'].action_space['move'] == Discrete(5)
+    assert agents['agent1'].action_space['move'] == Discrete(5)
+    assert agents['agent2'].action_space['move'] == Discrete(5)
+    assert agents['agent3'].action_space['move'] == Discrete(5)
+
+    for agent in agents.values():
+        agent.finalize()
+        assert agent.null_action.keys() == set(('move',))
+        assert agent.null_action['move'] == 0
+
+    position_state.reset()
+    action = {
+        'agent0': {'move': 2},
+        'agent1': {'move': 4},
+        'agent2': {'move': 3},
+        'agent3': {'move': 1},
+    }
+    for agent_id, action in action.items():
+        move_actor.process_action(agents[agent_id], action)
+    np.testing.assert_array_equal(agents['agent0'].position, np.array([4, 5]))
+    np.testing.assert_array_equal(agents['agent1'].position, np.array([1, 2]))
+    np.testing.assert_array_equal(agents['agent2'].position, np.array([0, 2]))
+    np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 2]))
+
+    action = {
+        'agent0': {'move': 3},
+        'agent1': {'move': 0},
+        'agent2': {'move': 4},
+        'agent3': {'move': 4},
+    }
+    for agent_id, action in action.items():
+        move_actor.process_action(agents[agent_id], action)
+    np.testing.assert_array_equal(agents['agent0'].position, np.array([4, 5]))
+    np.testing.assert_array_equal(agents['agent1'].position, np.array([1, 2]))
+    np.testing.assert_array_equal(agents['agent2'].position, np.array([0, 2]))
+    np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 2]))
+
+
+def test_cross_move_actor_with_overlap():
+    overlapping = {
+        1: {1},
+        2: {3},
+        3: {2}
+    }
+    grid = Grid(5, 6, overlapping=overlapping)
+    agents = {
+        'agent0': MovingAgent(
+            id='agent0', initial_position=np.array([4, 4]), encoding=1, move_range=1
+        ),
+        'agent1': MovingAgent(
+            id='agent1', initial_position=np.array([2, 2]), encoding=2, move_range=2
+        ),
+        'agent2': MovingAgent(
+            id='agent2', initial_position=np.array([2, 4]), encoding=1, move_range=1
+        ),
+        'agent3': MovingAgent(
+            id='agent3', initial_position=np.array([3, 2]), encoding=3, move_range=3
+        ),
+    }
+
+    position_state = PositionState(grid=grid, agents=agents)
+    move_actor = CrossMoveActor(grid=grid, agents=agents)
+
+    position_state.reset()
+    action = {
+        'agent0': {'move': 4},
+        'agent1': {'move': 3},
+        'agent2': {'move': 2},
+        'agent3': {'move': 4},
+    }
+    for agent_id, action in action.items():
+        move_actor.process_action(agents[agent_id], action)
+    np.testing.assert_array_equal(agents['agent0'].position, np.array([3, 4]))
+    np.testing.assert_array_equal(agents['agent1'].position, np.array([2, 3]))
+    np.testing.assert_array_equal(agents['agent2'].position, np.array([3, 4]))
+    np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 2]))
+
+    action = {
+        'agent0': {'move': 4},
+        'agent1': {'move': 0},
+        'agent2': {'move': 1},
+        'agent3': {'move': 3},
+    }
+    for agent_id, action in action.items():
+        move_actor.process_action(agents[agent_id], action)
+    np.testing.assert_array_equal(agents['agent0'].position, np.array([2, 4]))
+    np.testing.assert_array_equal(agents['agent1'].position, np.array([2, 3]))
+    np.testing.assert_array_equal(agents['agent2'].position, np.array([3, 3]))
+    np.testing.assert_array_equal(agents['agent3'].position, np.array([2, 3]))
+
+
 def test_binary_attack_actor():
     agents = {
         'agent0': HealthAgent(id='agent0', initial_position=np.array([4, 4]), encoding=1),
         'agent1': AttackingAgent(
             id='agent1',
             initial_position=np.array([2, 2]),
             encoding=1,
@@ -497,15 +610,15 @@
     assert grid[4, 4]
     assert grid[3, 2]
     assert grid[2, 2]
     assert grid[2, 3]
 
 
 def test_selective_attack_actor_attack_count():
-    grid = Grid(2, 2, overlapping={1: [1, 2, 3], 2: [1, 2, 3], 3: [1, 2, 3]})
+    grid = Grid(2, 2, overlapping={1: {1, 2, 3}, 2: {1, 2, 3}, 3: {1, 2, 3}})
     agents = {
         'agent0': AttackingAgent(
             id='agent0',
             initial_position=np.array([1, 1]),
             encoding=3,
             attack_range=1,
             attack_strength=0,
@@ -598,15 +711,15 @@
     assert not agents['agent2'].active
     assert not agents['agent3'].active
     assert not agents['agent4'].active
 
 
 def test_selective_attack_actor_stacked_attack():
     np.random.seed(24)
-    grid = Grid(2, 2, overlapping={1: [1, 2, 3], 2: [1, 2, 3], 3: [1, 2, 3]})
+    grid = Grid(2, 2, overlapping={1: {1, 2, 3}, 2: {1, 2, 3}, 3: {1, 2, 3}})
     agents = {
         'agent0': AttackingAgent(
             id='agent0',
             initial_position=np.array([1, 1]),
             encoding=3,
             attack_range=1,
             attack_strength=1,
@@ -684,15 +797,15 @@
     assert attacked_agents[0] == agents['agent1']
     assert attacked_agents[1] == agents['agent1']
     assert attacked_agents[2] == agents['agent1']
     assert not agents['agent1'].active
 
 
 def test_encoding_based_attack_actor():
-    grid = Grid(2, 2, overlapping={1: [3], 3: [1]})
+    grid = Grid(2, 2, overlapping={1: {3}, 3: {1}})
     agents = {
         'agent0': HealthAgent(id='agent0', initial_position=np.array([0, 0]), encoding=1),
         'agent1': HealthAgent(id='agent1', initial_position=np.array([0, 1]), encoding=2),
         'agent2': HealthAgent(id='agent2', initial_position=np.array([1, 0]), encoding=2),
         'agent3': AttackingAgent(
             id='agent3',
             initial_position=np.array([1, 1]),
@@ -759,15 +872,15 @@
         attack_actor.process_action(agents['agent3'], {'attack': {1: 1, 2: 1}})
     assert attack_status
     assert type(attacked_agents) is list
     assert len(attacked_agents) == 0
 
 
 def test_encoding_based_attack_actor_attack_count():
-    grid = Grid(2, 2, overlapping={1: [3], 3: [1]})
+    grid = Grid(2, 2, overlapping={1: {3}, 3: {1}})
     agents = {
         'agent0': HealthAgent(id='agent0', initial_position=np.array([0, 0]), encoding=1),
         'agent1': HealthAgent(id='agent1', initial_position=np.array([0, 1]), encoding=2),
         'agent2': HealthAgent(id='agent2', initial_position=np.array([1, 0]), encoding=2),
         'agent3': AttackingAgent(
             id='agent3',
             initial_position=np.array([1, 1]),
@@ -874,15 +987,15 @@
         attack_actor.process_action(agents['agent3'], {'attack': {1: 1, 2: 1}})
     assert attack_status
     assert type(attacked_agents) is list
     assert len(attacked_agents) == 0
 
 
 def test_encoding_based_attack_actor_stacked_attack():
-    grid = Grid(2, 2, overlapping={1: [3], 3: [1]})
+    grid = Grid(2, 2, overlapping={1: {3}, 3: {1}})
     agents = {
         'agent0': HealthAgent(id='agent0', initial_position=np.array([0, 0]), encoding=1),
         'agent1': HealthAgent(id='agent1', initial_position=np.array([0, 1]), encoding=2),
         'agent2': HealthAgent(id='agent2', initial_position=np.array([1, 0]), encoding=2),
         'agent3': AttackingAgent(
             id='agent3',
             initial_position=np.array([1, 1]),
@@ -940,15 +1053,15 @@
     assert len(attacked_agents) == 2
     assert attacked_agents[0] == attacked_agents[1]
     assert attacked_agents[0].encoding == 2
     assert not attacked_agents[0].active
 
 
 def test_restricted_selective_attack_actor():
-    grid = Grid(2, 2, overlapping={1: [1]})
+    grid = Grid(2, 2, overlapping={1: {1}})
     agents = {
         'agent0': HealthAgent(id='agent0', initial_position=np.array([0, 0]), encoding=1),
         'agent1': HealthAgent(id='agent1', initial_position=np.array([0, 1]), encoding=2),
         'agent2': HealthAgent(id='agent2', initial_position=np.array([1, 0]), encoding=2),
         'agent3': AttackingAgent(
             id='agent3',
             initial_position=np.array([1, 1]),
@@ -1011,15 +1124,15 @@
     assert attacked_agents[0].active
     assert attacked_agents[0].encoding == 1
     assert attacked_agents[1].active
     assert attacked_agents[1].encoding == 2
 
 
 def test_restricted_selective_attack_actor_stacked_attacks():
-    grid = Grid(2, 2, overlapping={1: [1]})
+    grid = Grid(2, 2, overlapping={1: {1}})
     agents = {
         'agent0': HealthAgent(
             id='agent0', initial_position=np.array([0, 0]), encoding=1, initial_health=1
         ),
         'agent1': HealthAgent(
             id='agent1', initial_position=np.array([0, 1]), encoding=2, initial_health=1
         ),
```

### Comparing `abmarl-0.2.5/tests/sim/gridworld/test_agent.py` & `abmarl-0.2.6/tests/sim/gridworld/test_agent.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/sim/gridworld/test_grid.py` & `abmarl-0.2.6/tests/sim/gridworld/test_grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,28 +24,32 @@
 
 def test_grid_internal():
     grid = Grid(2, 6)
     np.testing.assert_equal(grid._internal, np.empty((2, 6), dtype=object))
 
 
 def test_grid_overlapping():
-    grid = Grid(3, 3, overlapping={1: [2], 2: [1], 3: [1, 2]})
-    assert grid._overlapping == {1: [2], 2: [1], 3: [1, 2]}
+    grid = Grid(3, 3, overlapping={1: {1, 2}, 3: {1, 2}})
+    assert grid.overlapping == {1: {1, 2, 3}, 2: {1, 3}, 3: {1, 2}}
 
     with pytest.raises(AssertionError):
+        # This fails because overlapping must be a dictionary
         Grid(2, 2, overlapping=[1, 2, 3])
 
     with pytest.raises(AssertionError):
-        Grid(2, 2, overlapping={'1': [3], 2.0: [6]})
+        # This fails because the keys must be integers
+        Grid(2, 2, overlapping={'1': {3}, 2.0: {6}})
 
     with pytest.raises(AssertionError):
-        Grid(2, 2, overlapping={1: 3, 2: [6]})
+        # This fails because all the values must be sets
+        Grid(2, 2, overlapping={1: 3, 2: {6}})
 
     with pytest.raises(AssertionError):
-        Grid(2, 2, overlapping={1: ['2', 3], 2: [2, 3]})
+        # This fails because all the elements in the sets must be integers
+        Grid(2, 2, overlapping={1: {'2', 3}, 2: {2, 3}})
 
 
 def test_grid_reset():
     grid = Grid(3, 3)
     grid.reset()
     for i in range(grid.rows):
         for j in range(grid.cols):
@@ -70,15 +74,15 @@
     agent2 = GridWorldAgent(id='agent2', encoding=1)
     assert grid.place(agent1, (1, 0))
     assert not grid.query(agent2, (1, 0))
     assert grid.query(agent2, (0, 1))
 
 
 def test_grid_query_with_overlap():
-    grid = Grid(3, 3, overlapping={1: [1]})
+    grid = Grid(3, 3, overlapping={1: {1}})
     grid.reset()
     agent1 = GridWorldAgent(id='agent1', encoding=1)
     agent2 = GridWorldAgent(id='agent2', encoding=1)
     assert grid.place(agent1, (1, 0))
     assert grid.query(agent2, (1, 0))
     assert grid.query(agent1, (1, 0))
 
@@ -101,25 +105,25 @@
     agent1 = GridWorldAgent(id='agent1', encoding=1)
     agent2 = GridWorldAgent(id='agent2', encoding=2)
     assert grid.place(agent1, (1, 0))
     assert not grid.place(agent2, (1, 0))
 
 
 def test_grid_place_with_overlap():
-    grid = Grid(3, 3, overlapping={1: [2], 2: [1]})
+    grid = Grid(3, 3, overlapping={1: {2}, 2: {1}})
     grid.reset()
     agent1 = GridWorldAgent(id='agent1', encoding=1)
     agent2 = GridWorldAgent(id='agent2', encoding=2)
     assert grid.place(agent1, (1, 0))
     assert grid.place(agent2, (1, 0))
     assert grid[1, 0] == {'agent1': agent1, 'agent2': agent2}
 
 
 def test_grid_remove():
-    grid = Grid(3, 3, overlapping={1: [2], 2: [1]})
+    grid = Grid(3, 3, overlapping={1: {2}, 2: {1}})
     grid.reset()
     agent1 = GridWorldAgent(id='agent1', encoding=1)
     agent2 = GridWorldAgent(id='agent2', encoding=2)
     agent3 = GridWorldAgent(id='agent3', encoding=2)
     assert grid.place(agent1, (1, 0))
     assert grid.place(agent2, (1, 0))
     assert grid.place(agent3, (0, 1))
```

### Comparing `abmarl-0.2.5/tests/sim/gridworld/test_observer.py` & `abmarl-0.2.6/tests/sim/gridworld/test_observer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,147 @@
 
 from gym.spaces import Box
 import numpy as np
 
 from abmarl.sim.agent_based_simulation import ObservingAgent
-from abmarl.sim.gridworld.observer import ObserverBaseComponent, SingleGridObserver, \
-    MultiGridObserver, AbsolutePositionObserver
+from abmarl.sim.gridworld.observer import ObserverBaseComponent, AbsoluteGridObserver, \
+    SingleGridObserver, MultiGridObserver, AbsolutePositionObserver
 from abmarl.sim.gridworld.agent import GridObservingAgent, GridWorldAgent, MovingAgent
 from abmarl.sim.gridworld.state import PositionState
 from abmarl.sim.gridworld.grid import Grid
 
 
+def test_absolute_grid_observer():
+    np.random.seed(24)
+    grid = Grid(5, 5, overlapping={1: {6}, 6: {1}})
+    agents = {
+        'agent0': GridObservingAgent(
+            id='agent0', encoding=1, view_range=2, initial_position=np.array([2, 2])
+        ),
+        'agent1': GridObservingAgent(
+            id='agent1', encoding=2, view_range=1, initial_position=np.array([0, 0])
+        ),
+        'agent2': GridObservingAgent(
+            id='agent2', encoding=3, view_range=4, initial_position=np.array([4, 4])
+        ),
+        'agent3': GridWorldAgent(
+            id='agent3', encoding=5, initial_position=np.array([3, 3])
+        ),
+        'agent4': GridWorldAgent(
+            id='agent4', encoding=4, initial_position=np.array([1, 1])
+        ),
+        'agent5': GridWorldAgent(
+            id='agent5', encoding=6, initial_position=np.array([2, 1])
+        ),
+        'agent6': GridWorldAgent(
+            id='agent6', encoding=6, initial_position=np.array([2, 2])
+        ),
+    }
+
+    position_state = PositionState(grid=grid, agents=agents)
+    observer = AbsoluteGridObserver(agents=agents, grid=grid)
+    assert isinstance(observer, ObserverBaseComponent)
+    position_state.reset()
+
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent0'])['absolute_grid'],
+        np.array([
+            [ 2,  0,  0,  0,  0],
+            [ 0,  4,  0,  0,  0],
+            [ 0,  6, -1,  0,  0],
+            [ 0,  0,  0,  5,  0],
+            [ 0,  0,  0,  0,  3]
+        ])
+    )
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent1'])['absolute_grid'],
+        np.array([
+            [-1,  0, -2, -2, -2],
+            [ 0,  4, -2, -2, -2],
+            [-2, -2, -2, -2, -2],
+            [-2, -2, -2, -2, -2],
+            [-2, -2, -2, -2, -2]
+        ])
+    )
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent2'])['absolute_grid'],
+        np.array([
+            [ 2,  0,  0,  0,  0],
+            [ 0,  4,  0,  0,  0],
+            [ 0,  6,  1,  0,  0],
+            [ 0,  0,  0,  5,  0],
+            [ 0,  0,  0,  0, -1]
+        ])
+    )
+
+
+def test_absolute_grid_observer_blocking():
+    np.random.seed(24)
+    grid = Grid(5, 5, overlapping={1: {6}, 6: {1}})
+    agents = {
+        'agent0': GridObservingAgent(
+            id='agent0', encoding=1, view_range=2, initial_position=np.array([2, 2])
+        ),
+        'agent1': GridObservingAgent(
+            id='agent1', encoding=2, view_range=1, initial_position=np.array([0, 0])
+        ),
+        'agent2': GridObservingAgent(
+            id='agent2', encoding=3, view_range=4, initial_position=np.array([4, 4])
+        ),
+        'agent3': GridWorldAgent(
+            id='agent3', encoding=5, initial_position=np.array([3, 3]), blocking=True
+        ),
+        'agent4': GridWorldAgent(
+            id='agent4', encoding=4, initial_position=np.array([1, 1]), blocking=True
+        ),
+        'agent5': GridWorldAgent(
+            id='agent5', encoding=6, initial_position=np.array([2, 1]), blocking=True
+        ),
+        'agent6': GridWorldAgent(
+            id='agent6', encoding=6, initial_position=np.array([2, 2])
+        ),
+    }
+
+    position_state = PositionState(grid=grid, agents=agents)
+    observer = AbsoluteGridObserver(agents=agents, grid=grid)
+    assert isinstance(observer, ObserverBaseComponent)
+    position_state.reset()
+
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent0'])['absolute_grid'],
+        np.array([
+            [-2, -2,  0,  0,  0],
+            [-2,  4,  0,  0,  0],
+            [-2,  6, -1,  0,  0],
+            [-2,  0,  0,  5, -2],
+            [ 0,  0,  0, -2, -2]
+        ])
+    )
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent1'])['absolute_grid'],
+        np.array([
+            [-1,  0, -2, -2, -2],
+            [ 0,  4, -2, -2, -2],
+            [-2, -2, -2, -2, -2],
+            [-2, -2, -2, -2, -2],
+            [-2, -2, -2, -2, -2]
+        ])
+    )
+    np.testing.assert_array_equal(
+        observer.get_obs(agents['agent2'])['absolute_grid'],
+        np.array([
+            [-2, -2, -2,  0,  0],
+            [-2, -2, -2,  0,  0],
+            [-2, -2, -2, -2,  0],
+            [ 0,  0, -2,  5,  0],
+            [ 0,  0,  0,  0, -1]
+        ])
+    )
+
+
 def test_single_grid_observer():
     grid = Grid(5, 5)
     agents = {
         'agent0': GridObservingAgent(
             id='agent0', encoding=1, view_range=2, initial_position=np.array([2, 2])
         ),
         'agent1': GridObservingAgent(
@@ -183,15 +311,15 @@
         'agent4': GridWorldAgent(
             id='agent4', encoding=4, initial_position=np.array([1, 1])
         ),
         'agent5': GridWorldAgent(
             id='agent5', encoding=6, initial_position=np.array([2, 1])
         ),
     }
-    grid = Grid(5, 5, overlapping={2: [3], 3: [2], 5: [5]})
+    grid = Grid(5, 5, overlapping={2: {3}, 3: {2}, 5: {5}})
 
     position_state = PositionState(grid=grid, agents=agents)
     observer = MultiGridObserver(agents=agents, grid=grid)
     assert observer.key == 'grid'
     assert observer.supported_agent_type == GridObservingAgent
     assert isinstance(observer, ObserverBaseComponent)
     assert observer.number_of_encodings == 6
@@ -447,15 +575,15 @@
         'agent4': GridWorldAgent(
             id='agent4', encoding=4, initial_position=np.array([1, 1]), blocking=True
         ),
         'agent5': GridWorldAgent(
             id='agent5', encoding=6, initial_position=np.array([2, 1]), blocking=True
         ),
     }
-    grid = Grid(5, 5, overlapping={2: [3], 3: [2], 5: [5]})
+    grid = Grid(5, 5, overlapping={2: {3}, 3: {2}, 5: {5}})
 
     position_state = PositionState(grid=grid, agents=agents)
     observer = MultiGridObserver(agents=agents, grid=grid)
     assert isinstance(observer, ObserverBaseComponent)
     position_state.reset()
 
     np.testing.assert_array_equal(
@@ -665,15 +793,15 @@
         'agent1': GridObservingAgent(
             id='agent1', encoding=2, view_range=1, initial_position=np.array([0, 0])
         ),
         'agent2': HackAgent(
             id='agent2', encoding=2, view_range=1, initial_position=np.array([2, 2]), move_range=1
         ),
     }
-    grid = Grid(5, 5, overlapping={1: [2], 2: [1]})
+    grid = Grid(5, 5, overlapping={1: {2}, 2: {1}})
 
     position_state = PositionState(grid=grid, agents=agents)
     position_state.reset()
     self_observer = SingleGridObserver(agents=agents, grid=grid)
     no_self_observer = SingleGridObserver(agents=agents, grid=grid, observe_self=False)
 
     np.testing.assert_array_equal(
@@ -712,15 +840,15 @@
             [-1,  0,  0]
         ])
     )
 
 
 def test_absolute_position_observer():
     class PositionObservingAgent(ObservingAgent, GridWorldAgent): pass
-    grid = Grid(6, 7, overlapping={1: [5], 4: [6], 5: [1], 6: [4]})
+    grid = Grid(6, 7, overlapping={1: {5}, 4: {6}, 5: {1}, 6: {4}})
     agents = {
         'agent0': PositionObservingAgent(
             id='agent0',
             encoding=1,
             initial_position=np.array([0, 0])
         ),
         'agent1': PositionObservingAgent(
@@ -791,15 +919,15 @@
     np.testing.assert_array_equal(
         observer.get_obs(agents['agent5'])['position'],
         np.array([5, 6], dtype=int)
     )
 
 
 def test_grid_and_absolute_position_observer_combined():
-    grid = Grid(6, 7, overlapping={1: [5], 4: [6], 5: [1], 6: [4]})
+    grid = Grid(6, 7, overlapping={1: {5}, 4: {6}, 5: {1}, 6: {4}})
     agents = {
         'agent0': GridObservingAgent(
             id='agent0',
             encoding=1,
             initial_position=np.array([2, 2]),
             view_range=2
         ),
```

### Comparing `abmarl-0.2.5/tests/sim/gridworld/test_wrapper.py` & `abmarl-0.2.6/tests/sim/gridworld/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/sim/test_agent_based_simulation.py` & `abmarl-0.2.6/tests/sim/test_agent_based_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     from gym.spaces import Discrete
     agent = ActingAgent(id='agent', seed=17, action_space={
         1: Discrete(12),
         2: Discrete(3),
     })
     agent.finalize()
     assert agent.configured
-    assert agent.action_space.sample() == {1: 5, 2: 1}
+    assert agent.action_space.sample() == {1: 2, 2: 0}
 
 
 def test_observing_agent_observation_space():
     with pytest.raises(AssertionError):
         ObservingAgent(id='agent', observation_space=13)
 
     with pytest.raises(AssertionError):
@@ -124,15 +124,15 @@
         id='agent', seed=7, observation_space={'obs': Discrete(2)},
         action_space={'act': Discrete(5)}
     )
     assert not agent.configured
     agent.finalize()
     assert agent.configured
 
-    assert agent.action_space.sample() == {'act': 2}
+    assert agent.action_space.sample() == {'act': 1}
     assert agent.observation_space.sample() == {'obs': 0}
 
 
 def test_agent_instance():
     class TestAgent(ObservingAgent, ActingAgent): pass
     agent_1 = TestAgent(id='agent1')
     agent_2 = Agent(id='agent2')
```

### Comparing `abmarl-0.2.5/tests/sim/wrappers/test_super_agent_wrapper.py` & `abmarl-0.2.6/tests/sim/wrappers/test_super_agent_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import warnings
 
-from gym.spaces import Discrete, Dict
+from gym.spaces import MultiBinary, Dict
 import pytest
 
 from abmarl.sim.wrappers import SuperAgentWrapper
 from abmarl.examples import MultiAgentGymSpacesSim
 
 
 sim = SuperAgentWrapper(
@@ -79,15 +79,15 @@
     assert agents['super0'].action_space == Dict({
         'agent0': original_agents['agent0'].action_space,
         'agent3': original_agents['agent3'].action_space,
     })
     assert agents['super0'].observation_space == Dict({
         'agent0': original_agents['agent0'].observation_space,
         'agent3': original_agents['agent3'].observation_space,
-        'mask': Dict({'agent0': Discrete(2), 'agent3': Discrete(2)})
+        'mask': Dict({'agent0': MultiBinary(1), 'agent3': MultiBinary(1)})
     })
     assert agents['agent1'] == original_agents['agent1']
     assert agents['agent2'] == original_agents['agent2']
     assert agents['agent4'] == original_agents['agent4']
 
 
 def test_sim_step():
@@ -151,15 +151,15 @@
 def test_sim_obs():
     sim.unwrapped.step_count = 4
     obs = sim.get_obs('super0')
     assert obs in agents['super0'].observation_space
     assert obs == {
         'agent0': [0, 0, 0, 1],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': False, 'agent3': True}
+        'mask': {'agent0': [False], 'agent3': [True]}
     }
 
     obs = sim.get_obs('agent1')
     assert obs in agents['agent1'].observation_space
     assert obs == [0]
 
     obs = sim.get_obs('agent2')
@@ -230,15 +230,15 @@
     assert sim2.agents['double0'].action_space == Dict({
         'super0': sim2.sim.agents['super0'].action_space,
         'agent1': sim2.sim.agents['agent1'].action_space
     })
     assert sim2.agents['double0'].observation_space == Dict({
         'super0': sim2.sim.agents['super0'].observation_space,
         'agent1': sim2.sim.agents['agent1'].observation_space,
-        'mask': Dict({'super0': Discrete(2), 'agent1': Discrete(2)})
+        'mask': Dict({'super0': MultiBinary(1), 'agent1': MultiBinary(1)})
     })
     assert sim2.agents['agent2'] == original_agents['agent2']
     assert sim2.agents['agent4'] == original_agents['agent4']
 
     sim2.reset()
     assert sim2.unwrapped.action == {
         'agent0': None,
@@ -266,18 +266,18 @@
 
     obs = sim2.get_obs('double0')
     assert obs in sim2.agents['double0'].observation_space
     assert obs == {
         'super0': {
             'agent0': [0, 0, 0, 1],
             'agent3': {'first': 1, 'second': [3, 1]},
-            'mask': {'agent0': True, 'agent3': True}
+            'mask': {'agent0': [True], 'agent3': [True]}
         },
         'agent1': [0],
-        'mask': {'agent1': True, 'super0': True}
+        'mask': {'agent1': [True], 'super0': [True]}
     }
     obs = sim2.get_obs('agent2')
     assert obs in sim2.agents['agent2'].observation_space
     assert obs == [1, 0]
 
     assert sim2.get_reward('double0') == 12
     assert sim2.get_reward('agent2') == 5
@@ -299,15 +299,15 @@
     sim.reset()
     sim.unwrapped.step_count = 2
     obs = sim.get_obs('super0')
     assert obs in agents['super0'].observation_space
     assert obs == {
         'agent0': [0, 0, 0, 1],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': True, 'agent3': True}
+        'mask': {'agent0': [True], 'agent3': [True]}
     }
 
 
     sim.step({'agent1': [2, 2, 0]})
     assert sim.unwrapped.step_count == 3
     assert sim.unwrapped.get_done('agent0')
     assert not sim.unwrapped.get_done('agent3')
@@ -316,20 +316,20 @@
     assert sim.unwrapped.step_count == 4
     assert sim.unwrapped.get_done('agent0')
     assert not sim.unwrapped.get_done('agent3')
 
     assert sim.get_obs('super0') == {
         'agent0': [0, 0, 0, 1],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': False, 'agent3': True}
+        'mask': {'agent0': [False], 'agent3': [True]}
     }
     assert sim.get_obs('super0') == {
         'agent0': [0, 0, 0, 0],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': False, 'agent3': True}
+        'mask': {'agent0': [False], 'agent3': [True]}
     }
     assert sim.unwrapped.get_obs('agent0') == [0, 0, 0, 1]
 
     assert sim.get_reward('super0') == 9
     assert sim.get_reward('super0') == 7
     assert sim.unwrapped.get_reward('agent0') == 2
 
@@ -338,20 +338,20 @@
     sim.unwrapped.step_count = 35
     assert sim.unwrapped.get_done('agent0')
     assert sim.unwrapped.get_done('agent3')
 
     assert sim.get_obs('super0') == {
         'agent0': [0, 0, 0, 0],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': False, 'agent3': False}
+        'mask': {'agent0': [False], 'agent3': [False]}
     }
     assert sim.get_obs('super0') == {
         'agent0': [0, 0, 0, 0],
         'agent3': {'first': 1, 'second': [3, 1]},
-        'mask': {'agent0': False, 'agent3': False}
+        'mask': {'agent0': [False], 'agent3': [False]}
     }
     assert sim.get_reward('super0') == 7
     assert sim.get_reward('super0') == 0
     assert sim.unwrapped.get_reward('agent3') == 7
 
 
 def test_null_obs_warning():
```

### Comparing `abmarl-0.2.5/tests/test_all_step_multi_corridor.py` & `abmarl-0.2.6/tests/test_all_step_multi_corridor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import random
+
 import numpy as np
 import pytest
 
 from abmarl.examples import MultiCorridor
 from abmarl.managers import AllStepManager
 
 
@@ -227,7 +229,79 @@
     obs, reward, done, _ = sim.step({
         'agent3': MultiCorridor.Actions.RIGHT,
     })
 
     assert obs == {'agent3': {'left': [False], 'position': [9], 'right': [False]}}
     assert reward == {'agent3': 100}
     assert done == {'agent3': True, '__all__': True}
+
+
+def test_randomized_order():
+    random.seed(24)
+    np.random.seed(24)
+
+    with pytest.raises(AssertionError):
+        AllStepManager(MultiCorridor(), randomize_action_input=0)
+
+    sim = AllStepManager(MultiCorridor())
+    assert not sim.randomize_action_input
+    sim.reset()
+    sim.step({
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent4': MultiCorridor.Actions.LEFT,
+    })
+    assert sim.sim._last_action == {
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent4': MultiCorridor.Actions.LEFT,
+    }
+
+    sim = AllStepManager(MultiCorridor(), randomize_action_input=True)
+    assert sim.randomize_action_input
+    sim.reset()
+    sim.step({
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent4': MultiCorridor.Actions.LEFT,
+    })
+    assert sim.sim._last_action == {
+        'agent4': MultiCorridor.Actions.LEFT,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent3': MultiCorridor.Actions.STAY,
+    }
+    sim.step({
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent4': MultiCorridor.Actions.LEFT,
+    })
+    assert sim.sim._last_action == {
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent4': MultiCorridor.Actions.LEFT,
+        'agent1': MultiCorridor.Actions.STAY,
+    }
+    sim.step({
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent1': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent4': MultiCorridor.Actions.LEFT,
+    })
+    assert sim.sim._last_action == {
+        'agent4': MultiCorridor.Actions.LEFT,
+        'agent0': MultiCorridor.Actions.RIGHT,
+        'agent3': MultiCorridor.Actions.STAY,
+        'agent2': MultiCorridor.Actions.LEFT,
+        'agent1': MultiCorridor.Actions.STAY,
+    }
```

### Comparing `abmarl-0.2.5/tests/test_communication_wrapper.py` & `abmarl-0.2.6/tests/test_communication_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_dynamic_order_manager.py` & `abmarl-0.2.6/tests/test_dynamic_order_manager.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_flatten_wrapper.py` & `abmarl-0.2.6/tests/test_flatten_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_generate_episode.py` & `abmarl-0.2.6/tests/test_generate_episode.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_gym_wrapper.py` & `abmarl-0.2.6/tests/test_gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_multi_corridor.py` & `abmarl-0.2.6/tests/test_multi_corridor.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_off_policy_monte_carlo.py` & `abmarl-0.2.6/tests/test_off_policy_monte_carlo.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_ravel_discrete_wrapper.py` & `abmarl-0.2.6/tests/test_ravel_discrete_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_sar_wrapper.py` & `abmarl-0.2.6/tests/test_sar_wrapper.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_simulation_manager_corridor.py` & `abmarl-0.2.6/tests/test_simulation_manager_corridor.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/test_turn_based_multi_corridor.py` & `abmarl-0.2.6/tests/test_turn_based_multi_corridor.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/trainers/test_debug_trainer.py` & `abmarl-0.2.6/tests/trainers/test_debug_trainer.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/trainers/test_monte_carlo.py` & `abmarl-0.2.6/tests/trainers/test_monte_carlo.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/trainers/test_multi_policy_trainer.py` & `abmarl-0.2.6/tests/trainers/test_multi_policy_trainer.py`

 * *Files identical despite different names*

### Comparing `abmarl-0.2.5/tests/trainers/test_single_policy_trainer.py` & `abmarl-0.2.6/tests/trainers/test_single_policy_trainer.py`

 * *Files identical despite different names*

