# Comparing `tmp/rlberry-0.4.1.tar.gz` & `tmp/rlberry-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlberry-0.4.1.tar", last modified: Mon Jun 19 08:56:17 2023, max compression
+gzip compressed data, was "rlberry-0.5.0.tar", last modified: Fri Jun 23 08:39:51 2023, max compression
```

## Comparing `rlberry-0.4.1.tar` & `rlberry-0.5.0.tar`

### file list

```diff
@@ -1,319 +1,332 @@
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1067 2022-05-09 08:37:51.000000 rlberry-0.4.1/LICENSE
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       55 2022-05-09 08:37:51.000000 rlberry-0.4.1/MANIFEST.in
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6752 2023-06-19 08:56:17.238106 rlberry-0.4.1/PKG-INFO
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5868 2023-06-19 08:30:31.000000 rlberry-0.4.1/README.md
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/assets/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5723 2023-06-19 08:30:31.000000 rlberry-0.4.1/assets/logo_square.svg
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5542 2023-06-19 08:30:31.000000 rlberry-0.4.1/assets/logo_wide.svg
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      335 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       23 2023-06-19 08:31:37.000000 rlberry-0.4.1/rlberry/_version.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      530 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/adaptiveql/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       40 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5479 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/adaptiveql.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6237 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/tree.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1691 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    18386 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/agent.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/bandits/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      479 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3361 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/bandit_base.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3300 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/index_agents.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    12014 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/indices.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4472 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/priors.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4068 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/randomized_agents.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/bandits/tools/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       35 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/tools/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8519 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/tools/tracker.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5109 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/bandits/ts_agents.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/dynprog/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       49 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/dynprog/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8882 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/dynprog/utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2540 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/dynprog/value_iteration.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1324 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/tests/test_sac.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/torch/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    13132 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/sac.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2278 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/features/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       36 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/features/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      580 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/features/feature_map.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/kernel_based/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       83 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      908 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/common.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1929 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/kernels.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    12466 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/kernel_based/rs_kernel_ucbvi.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11254 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/kernel_based/rs_ucbvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/linear/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       35 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/linear/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11184 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/linear/lsvi_ucb.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/mbqvi/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/mbqvi/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4943 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/mbqvi/mbqvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/optql/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/optql/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6595 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/optql/optql.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/psrl/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       28 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/psrl/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8344 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/psrl/psrl.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/rlsvi/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/rlsvi/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8502 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/rlsvi/rlsvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/stable_baselines/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       51 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/stable_baselines/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8702 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/stable_baselines/stable_baselines.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/tabular_rl/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       61 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3991 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/qlearning.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4042 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/sarsa.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      377 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_adaptiveql.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3509 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tests/test_bandits.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4902 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_dynprog.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1558 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_kernel_based.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6078 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_lsvi_ucb.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      808 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_mbqvi.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      304 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_optql.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      772 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_psrl.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5707 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_replay.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      507 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_rlsvi.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1058 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_stable_baselines.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1016 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tests/test_tabular_rl.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      779 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_ucbvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      191 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/a2c/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/a2c/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11487 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/a2c/a2c.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/dqn/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       63 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    16491 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/dqn.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4226 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/dqn_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17760 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/mdqn.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/ppo/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    24870 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/ppo.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5962 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/ppo_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/reinforce/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       38 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/reinforce/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7207 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/reinforce/reinforce.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3388 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_a2c.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1140 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_dqn.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      692 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_factory.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1134 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_mdqn.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5752 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_ppo.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1434 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_reinforce.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3850 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_atari.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1230 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_models.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1080 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_training.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/utils/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/utils/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17133 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/utils/models.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5201 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/utils/training.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/ucbvi/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/ucbvi/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10335 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/ucbvi/ucbvi.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1952 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/ucbvi/utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/utils/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/utils/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1525 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/utils/memories.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14236 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/utils/replay.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5290 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/utils/replay_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      357 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/check_packages.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/colab_utils/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/colab_utils/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1053 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/colab_utils/display_setup.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      263 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/bandits/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      181 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/bandits/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3392 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/bandits/bandit_base.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2614 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/bandits/corrupted_bandits.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1370 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/bandits/stochastic_bandits.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3817 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/basewrapper.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       49 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4995 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/ball2d.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14237 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/pball.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5440 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/twinrooms.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5294 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/apple_gold.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3816 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/four_room.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10490 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/nroom.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4229 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/six_room.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/classic_control/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    18518 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/classic_control/SpringCartPole.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      141 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/classic_control/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11984 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/acrobot.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5938 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/mountain_car.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3635 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/pendulum.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/finite/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       92 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3956 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/chain.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5594 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/finite/finite_mdp.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    16178 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/finite/gridworld.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2011 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/gridworld_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3776 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/gym_make.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/interface/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       25 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/interface/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4813 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/interface/model.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1227 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/pipeline.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1593 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_bandits.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2589 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/test_env_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2225 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/test_gym_env_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7440 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_instantiation.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2635 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_spring_env.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      845 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/experiment/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      142 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/experiment/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1815 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/experiment/generator.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3705 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/experiment/load_results.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6283 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/experiment/yaml_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3507 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/discrete_counter.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6179 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/exploration_tools/online_discretization_counter.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4326 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/exploration_tools/tests/test_discrete_counter.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/torch/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7356 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/rnd.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      711 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/test_rnd.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2341 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/typing.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1012 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/uncertainty_estimator.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/manager/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      180 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    48007 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/agent_manager.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    19901 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/evaluation.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2967 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/multiple_managers.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7863 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/remote_agent_manager.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/manager/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10244 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_agent_manager.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2648 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/tests/test_agent_manager_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5965 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_hyperparam_optim.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4544 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_plot.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1249 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/tests/test_shared_data.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      391 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1947 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/metadata_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/network/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1522 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/client.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2836 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/interface.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6408 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/network/server.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5062 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/server_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/network/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1393 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/conftest.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2792 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/test_server.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2631 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/rendering/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      138 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1001 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/common_shapes.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1265 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/core.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7709 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/opengl_render2d.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5931 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/pygame_render2d.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4427 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/render_interface.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/rendering/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3049 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/tests/test_rendering_interface.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1864 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/rendering/utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/seeding/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       99 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3973 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/seeding/seeder.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2105 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/seeding/seeding.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/seeding/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1728 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      874 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_threads.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1072 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_threads_torch.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/spaces/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      180 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3003 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/box.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      807 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/dict.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1553 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/discrete.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1429 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/from_gym.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1261 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/multi_binary.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1347 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/multi_discrete.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/spaces/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4724 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/test_from_gym.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3611 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/test_spaces.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      763 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tuple.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2397 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_agent_extra.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1878 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_agents_base.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      760 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_envs.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      283 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/types.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/utils/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      228 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1177 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/binsearch.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    23015 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/check_agent.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1728 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/check_bandit_agent.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1478 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/check_env.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10915 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/check_gym_env.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      199 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/factory.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      847 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/io.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      395 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/jit_setup.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3453 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/logging.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      326 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/math.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      699 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/metrics.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2200 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/space_discretizer.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/utils/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1061 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_binsearch.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2976 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_check.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      483 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_metrics.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1410 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/tests/test_writer.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2517 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/torch.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17154 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/writers.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/wrappers/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      195 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5812 2022-10-06 15:00:01.000000 rlberry-0.4.1/rlberry/wrappers/atari_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      890 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/autoreset.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      962 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/discrete2onehot.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3273 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/discretize_state.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1217 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/gym_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2064 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/rescale_reward.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      551 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/wrappers/scalarize.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/wrappers/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      776 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_basewrapper.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5701 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_common_wrappers.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2988 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_gym_space_conversion.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3981 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_wrapper_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1114 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_writer_utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3482 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/wrappers/uncertainty_estimator_wrapper.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14355 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/wrappers/vis2d.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1425 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/writer_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry.egg-info/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6752 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/PKG-INFO
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     9039 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/SOURCES.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/dependency_links.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2022-05-10 07:35:31.000000 rlberry-0.4.1/rlberry.egg-info/not-zip-safe
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      514 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/requires.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        8 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/top_level.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       74 2023-06-19 08:56:17.238106 rlberry-0.4.1/setup.cfg
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2332 2023-06-19 08:56:07.000000 rlberry-0.4.1/setup.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.460643 rlberry-0.5.0/
+-rw-r--r--   0 frost     (1000) frost     (1000)     1067 2023-01-18 09:58:26.000000 rlberry-0.5.0/LICENSE
+-rw-r--r--   0 frost     (1000) frost     (1000)       55 2023-01-18 09:58:26.000000 rlberry-0.5.0/MANIFEST.in
+-rw-r--r--   0 frost     (1000) frost     (1000)     6752 2023-06-23 08:39:51.460643 rlberry-0.5.0/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     5868 2023-06-23 07:58:17.000000 rlberry-0.5.0/README.md
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.433977 rlberry-0.5.0/assets/
+-rw-r--r--   0 frost     (1000) frost     (1000)     5723 2023-04-06 12:46:10.000000 rlberry-0.5.0/assets/logo_square.svg
+-rw-r--r--   0 frost     (1000) frost     (1000)     5542 2023-04-06 12:46:10.000000 rlberry-0.5.0/assets/logo_wide.svg
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.433977 rlberry-0.5.0/rlberry/
+-rw-r--r--   0 frost     (1000) frost     (1000)      335 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)       23 2023-06-23 08:38:30.000000 rlberry-0.5.0/rlberry/_version.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.433977 rlberry-0.5.0/rlberry/agents/
+-rw-r--r--   0 frost     (1000) frost     (1000)      560 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/adaptiveql/
+-rw-r--r--   0 frost     (1000) frost     (1000)       40 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/adaptiveql/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5626 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/adaptiveql/adaptiveql.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6243 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/adaptiveql/tree.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1691 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/adaptiveql/utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    25440 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/agent.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/bandits/
+-rw-r--r--   0 frost     (1000) frost     (1000)      479 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/bandits/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3364 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/bandits/bandit_base.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3303 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/bandits/index_agents.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    12014 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/bandits/indices.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4472 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/bandits/priors.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4071 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/bandits/randomized_agents.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/bandits/tools/
+-rw-r--r--   0 frost     (1000) frost     (1000)       35 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/bandits/tools/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     8519 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/bandits/tools/tracker.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5112 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/bandits/ts_agents.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/dynprog/
+-rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/dynprog/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     8882 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/dynprog/utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2540 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/dynprog/value_iteration.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/experimental/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/experimental/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/experimental/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/experimental/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1324 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/experimental/tests/test_sac.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/experimental/torch/
+-rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-05-04 08:55:47.000000 rlberry-0.5.0/rlberry/agents/experimental/torch/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.437310 rlberry-0.5.0/rlberry/agents/experimental/torch/sac/
+-rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/experimental/torch/sac/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    13420 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/experimental/torch/sac/sac.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2284 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/experimental/torch/sac/utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/features/
+-rw-r--r--   0 frost     (1000) frost     (1000)       36 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/features/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      580 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/features/feature_map.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/kernel_based/
+-rw-r--r--   0 frost     (1000) frost     (1000)       83 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/kernel_based/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      908 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/kernel_based/common.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1929 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/kernel_based/kernels.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    12613 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/kernel_based/rs_kernel_ucbvi.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    11401 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/kernel_based/rs_ucbvi.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/linear/
+-rw-r--r--   0 frost     (1000) frost     (1000)       35 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/linear/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    11335 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/linear/lsvi_ucb.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/mbqvi/
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/mbqvi/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4952 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/mbqvi/mbqvi.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/optql/
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/optql/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6748 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/optql/optql.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/psrl/
+-rw-r--r--   0 frost     (1000) frost     (1000)       28 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/psrl/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     8497 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/psrl/psrl.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/rlsvi/
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/rlsvi/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     8655 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/rlsvi/rlsvi.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/stable_baselines/
+-rw-r--r--   0 frost     (1000) frost     (1000)       51 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/stable_baselines/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     8702 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/stable_baselines/stable_baselines.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.440643 rlberry-0.5.0/rlberry/agents/tabular_rl/
+-rw-r--r--   0 frost     (1000) frost     (1000)       61 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tabular_rl/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4102 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tabular_rl/qlearning.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4153 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tabular_rl/sarsa.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      377 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_adaptiveql.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3509 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tests/test_bandits.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4902 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_dynprog.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1558 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_kernel_based.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6168 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tests/test_lsvi_ucb.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      808 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_mbqvi.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      304 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_optql.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      772 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_psrl.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5888 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tests/test_replay.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      507 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_rlsvi.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1058 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_stable_baselines.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1016 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/tests/test_tabular_rl.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      779 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/tests/test_ucbvi.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/
+-rw-r--r--   0 frost     (1000) frost     (1000)      191 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/a2c/
+-rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/a2c/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    11638 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/a2c/a2c.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/dqn/
+-rw-r--r--   0 frost     (1000) frost     (1000)       63 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/dqn/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    16651 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/dqn/dqn.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4226 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/dqn/dqn_utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    17919 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/dqn/mdqn.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/ppo/
+-rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/ppo/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    28973 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/ppo/ppo.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5999 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/ppo/ppo_utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/reinforce/
+-rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/reinforce/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7375 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/reinforce/reinforce.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3394 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_a2c.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4571 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_dqn.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      692 2023-05-04 08:55:47.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_factory.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1170 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_mdqn.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5758 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_ppo.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1434 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_reinforce.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    10855 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_torch_atari.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1230 2023-05-04 08:55:47.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_torch_models.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1080 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/tests/test_torch_training.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/torch/utils/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/torch/utils/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    17314 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/utils/models.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5207 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/torch/utils/training.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.443976 rlberry-0.5.0/rlberry/agents/ucbvi/
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/ucbvi/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    10488 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/ucbvi/ucbvi.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1952 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/ucbvi/utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/agents/utils/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/utils/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1525 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/utils/memories.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    14321 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/agents/utils/replay.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5290 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/agents/utils/replay_utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      358 2023-06-23 08:36:04.000000 rlberry-0.5.0/rlberry/check_packages.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/colab_utils/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/colab_utils/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1053 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/colab_utils/display_setup.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/
+-rw-r--r--   0 frost     (1000) frost     (1000)      263 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/bandits/
+-rw-r--r--   0 frost     (1000) frost     (1000)      181 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/bandits/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2633 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/bandits/bandit_base.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2614 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/bandits/corrupted_bandits.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1370 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/bandits/stochastic_bandits.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4496 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/basewrapper.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/benchmarks/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/benchmarks/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/
+-rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4995 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/ball2d.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    14349 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/pball.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/benchmarks/generalization/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/benchmarks/generalization/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5574 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/generalization/twinrooms.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5510 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/apple_gold.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3901 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/four_room.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    10611 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/nroom.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4314 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/six_room.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.447310 rlberry-0.5.0/rlberry/envs/classic_control/
+-rw-r--r--   0 frost     (1000) frost     (1000)    18563 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/classic_control/SpringCartPole.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      141 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/classic_control/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    12056 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/classic_control/acrobot.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6133 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/classic_control/mountain_car.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3671 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/classic_control/pendulum.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/envs/finite/
+-rw-r--r--   0 frost     (1000) frost     (1000)       92 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/finite/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4012 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/finite/chain.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5728 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/finite/finite_mdp.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    16234 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/finite/gridworld.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2011 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/finite/gridworld_utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5218 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/gym_make.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/envs/interface/
+-rw-r--r--   0 frost     (1000) frost     (1000)       25 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/interface/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4826 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/interface/model.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1227 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/pipeline.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/envs/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/envs/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1593 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_bandits.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2598 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_env_seeding.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2342 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_gym_env_seeding.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4784 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_gym_make.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7491 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_instantiation.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3001 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/tests/test_spring_env.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      849 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/envs/utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/experiment/
+-rw-r--r--   0 frost     (1000) frost     (1000)      142 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/experiment/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1815 2023-04-06 12:46:10.000000 rlberry-0.5.0/rlberry/experiment/generator.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3705 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/experiment/load_results.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6283 2023-04-06 12:46:10.000000 rlberry-0.5.0/rlberry/experiment/yaml_utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/exploration_tools/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3507 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/discrete_counter.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6185 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/exploration_tools/online_discretization_counter.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/exploration_tools/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4338 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/exploration_tools/tests/test_discrete_counter.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/exploration_tools/torch/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/torch/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7362 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/exploration_tools/torch/rnd.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.450643 rlberry-0.5.0/rlberry/exploration_tools/torch/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/torch/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      833 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/exploration_tools/torch/tests/test_rnd.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2341 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/typing.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1012 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/exploration_tools/uncertainty_estimator.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/manager/
+-rw-r--r--   0 frost     (1000) frost     (1000)      180 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    48202 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/agent_manager.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    19901 2023-04-06 12:46:10.000000 rlberry-0.5.0/rlberry/manager/evaluation.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2967 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/manager/multiple_managers.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7863 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/manager/remote_agent_manager.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/manager/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/manager/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    10244 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/tests/test_agent_manager.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2696 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/tests/test_agent_manager_seeding.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5965 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/tests/test_hyperparam_optim.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4544 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/manager/tests/test_plot.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1249 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/manager/tests/test_shared_data.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      391 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/manager/utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1947 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/metadata_utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/network/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1522 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/client.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2836 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/interface.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6408 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/server.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5062 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/server_utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/network/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/network/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1393 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/tests/conftest.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2792 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/network/tests/test_server.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2631 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/network/utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/rendering/
+-rw-r--r--   0 frost     (1000) frost     (1000)      138 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/rendering/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1001 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/rendering/common_shapes.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1265 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/rendering/core.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7709 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/rendering/opengl_render2d.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5931 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/rendering/pygame_render2d.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4427 2023-04-06 12:46:10.000000 rlberry-0.5.0/rlberry/rendering/render_interface.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/rendering/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/rendering/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3926 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/rendering/tests/test_rendering_interface.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1864 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/rendering/utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.453976 rlberry-0.5.0/rlberry/seeding/
+-rw-r--r--   0 frost     (1000) frost     (1000)       99 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3973 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/seeder.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2234 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/seeding/seeding.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.457310 rlberry-0.5.0/rlberry/seeding/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1728 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/tests/test_seeding.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      874 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/tests/test_threads.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1072 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/seeding/tests/test_threads_torch.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.457310 rlberry-0.5.0/rlberry/spaces/
+-rw-r--r--   0 frost     (1000) frost     (1000)      180 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/spaces/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3022 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/box.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      826 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/dict.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1572 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/discrete.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1471 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/from_gym.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1280 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/multi_binary.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1366 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/multi_discrete.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.457310 rlberry-0.5.0/rlberry/spaces/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/spaces/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4874 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/tests/test_from_gym.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3611 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/spaces/tests/test_spaces.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      782 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/spaces/tuple.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.457310 rlberry-0.5.0/rlberry/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2397 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/tests/test_agent_extra.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1878 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/tests/test_agents_base.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      760 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/tests/test_envs.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      296 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/types.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.457310 rlberry-0.5.0/rlberry/utils/
+-rw-r--r--   0 frost     (1000) frost     (1000)      228 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1177 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/binsearch.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    23533 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/check_agent.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1777 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/check_bandit_agent.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1478 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/check_env.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    11321 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/check_gym_env.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      199 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/factory.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      847 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/io.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      395 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/jit_setup.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3466 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/logging.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      326 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/math.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      699 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/metrics.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2206 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/space_discretizer.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.460643 rlberry-0.5.0/rlberry/utils/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/tests/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1061 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/tests/test_binsearch.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3129 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/tests/test_check.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      483 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/tests/test_metrics.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1410 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/tests/test_writer.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2517 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/utils/torch.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    17154 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/utils/writers.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.460643 rlberry-0.5.0/rlberry/wrappers/
+-rw-r--r--   0 frost     (1000) frost     (1000)      436 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1017 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/autoreset.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1059 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/discrete2onehot.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3455 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/discretize_state.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1956 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/gym_utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2154 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/rescale_reward.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.460643 rlberry-0.5.0/rlberry/wrappers/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)      243 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/__init__.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.460643 rlberry-0.5.0/rlberry/wrappers/tests/old_env/
+-rw-r--r--   0 frost     (1000) frost     (1000)      411 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    12196 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_acrobot.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5543 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_apple_gold.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6337 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_ball2d.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5806 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_finite_mdp.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4065 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_four_room.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    16428 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_gridworld.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     6150 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_mountain_car.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    10743 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_nroom.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    14893 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_pball.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3847 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_pendulum.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4478 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_six_room.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     5652 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_twinrooms.py
+-rw-r--r--   0 frost     (1000) frost     (1000)      789 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/test_basewrapper.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     7899 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/test_common_wrappers.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3001 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/test_gym_space_conversion.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     4003 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/tests/test_wrapper_seeding.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1114 2023-01-18 09:58:26.000000 rlberry-0.5.0/rlberry/wrappers/tests/test_writer_utils.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     3636 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/uncertainty_estimator_wrapper.py
+-rw-r--r--   0 frost     (1000) frost     (1000)    14445 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/vis2d.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     1459 2023-06-23 07:58:17.000000 rlberry-0.5.0/rlberry/wrappers/writer_utils.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-23 08:39:51.433977 rlberry-0.5.0/rlberry.egg-info/
+-rw-r--r--   0 frost     (1000) frost     (1000)     6752 2023-06-23 08:39:51.000000 rlberry-0.5.0/rlberry.egg-info/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     9622 2023-06-23 08:39:51.000000 rlberry-0.5.0/rlberry.egg-info/SOURCES.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-23 08:39:51.000000 rlberry-0.5.0/rlberry.egg-info/dependency_links.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-01-18 10:00:11.000000 rlberry-0.5.0/rlberry.egg-info/not-zip-safe
+-rw-r--r--   0 frost     (1000) frost     (1000)      523 2023-06-23 08:39:51.000000 rlberry-0.5.0/rlberry.egg-info/requires.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        8 2023-06-23 08:39:51.000000 rlberry-0.5.0/rlberry.egg-info/top_level.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       74 2023-06-23 08:39:51.460643 rlberry-0.5.0/setup.cfg
+-rw-r--r--   0 frost     (1000) frost     (1000)     2302 2023-06-23 07:58:17.000000 rlberry-0.5.0/setup.py
```

### Comparing `rlberry-0.4.1/LICENSE` & `rlberry-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/PKG-INFO` & `rlberry-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlberry
-Version: 0.4.1
+Version: 0.5.0
 Summary: An easy-to-use reinforcement learning library for research and education
 Home-page: https://github.com/rlberry-py
 Author: Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,17 +12,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: default
-Provides-Extra: deploy
 Provides-Extra: jax_agents
 Provides-Extra: torch_agents
+Provides-Extra: deploy
 License-File: LICENSE
 
 <!-- Logo -->
 <p align="center">
    <img src="https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/logo_wide.svg" width="50%">
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: rlberry Version: 0.4.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: rlberry Version: 0.5.0 Summary: An easy-to-use
 reinforcement learning library for research and education Home-page: https://
 github.com/rlberry-py Author: Omar Darwiche Domingues, Yannis Flet-Berliac,
 Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Education Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
-Extra: default Provides-Extra: deploy Provides-Extra: jax_agents Provides-
-Extra: torch_agents License-File: LICENSE
+Extra: default Provides-Extra: jax_agents Provides-Extra: torch_agents
+Provides-Extra: deploy License-File: LICENSE
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
            [pytest] [Documentation_Status] [contributors] [codecov]
 
                     Try_it_on_Google_Colab!_[Open_In_Colab]
```

### Comparing `rlberry-0.4.1/README.md` & `rlberry-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/assets/logo_square.svg` & `rlberry-0.5.0/assets/logo_square.svg`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/assets/logo_wide.svg` & `rlberry-0.5.0/assets/logo_wide.svg`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/__init__.py` & `rlberry-0.5.0/rlberry/agents/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Interfaces
 from .agent import Agent
 from .agent import AgentWithSimplePolicy
+from .agent import AgentTorch
 
 # Basic agents (in alphabetical order)
 # basic = does not require torch, jax, etc...
 from .adaptiveql import AdaptiveQLAgent
 from .dynprog import ValueIterationAgent
 from .kernel_based import RSUCBVIAgent, RSKernelUCBVIAgent
 from .linear import LSVIUCBAgent
```

### Comparing `rlberry-0.4.1/rlberry/agents/adaptiveql/adaptiveql.py` & `rlberry-0.5.0/rlberry/agents/adaptiveql/adaptiveql.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 import numpy as np
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.adaptiveql.tree import MDPTreePartition
 
 import rlberry
 
 logger = rlberry.logger
@@ -130,23 +130,26 @@
             raise ValueError(
                 "Error: bonus type {} not implemented".format(self.bonus_type)
             )
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action, node = self._get_action_and_node(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action, node = self._get_action_and_node(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward
 
-            self._update(node, state, action, next_state, reward, hh)
+            self._update(node, observation, action, next_observation, reward, hh)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # update info
         self.episode += 1
 
         # writer
```

### Comparing `rlberry-0.4.1/rlberry/agents/adaptiveql/tree.py` & `rlberry-0.5.0/rlberry/agents/adaptiveql/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 import numpy as np
 import matplotlib.pyplot as plt
 from rlberry.agents.adaptiveql.utils import bounds_contains, split_bounds
 
 
 class TreeNode:
     """
```

### Comparing `rlberry-0.4.1/rlberry/agents/adaptiveql/utils.py` & `rlberry-0.5.0/rlberry/agents/adaptiveql/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/agent.py` & `rlberry-0.5.0/rlberry/agents/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -301,29 +301,32 @@
         """
         # remove writer if not pickleable
         if not dill.pickles(self.writer):
             self.set_writer(None)
         # save
         filename = Path(filename).with_suffix(".pickle")
         filename.parent.mkdir(parents=True, exist_ok=True)
+
+        dict_to_save = dict(self.__dict__)
+
         try:
             if not self.compress_pickle:
                 with filename.open("wb") as ff:
-                    pickle.dump(self.__dict__, ff)
+                    pickle.dump(dict_to_save, ff)
             else:
                 with bz2.BZ2File(filename, "wb") as ff:
-                    cPickle.dump(self.__dict__, ff)
-        except Exception:
+                    cPickle.dump(dict_to_save, ff)
+        except Exception as ex:
             try:
                 if not self.compress_pickle:
                     with filename.open("wb") as ff:
-                        dill.dump(self.__dict__, ff)
+                        dill.dump(dict_to_save, ff)
                 else:
                     with bz2.BZ2File(filename, "wb") as ff:
-                        dill.dump(self.__dict__, ff)
+                        dill.dump(dict_to_save, ff)
             except Exception as ex:
                 logger.warning("Agent instance cannot be pickled: " + str(ex))
                 return None
 
         return filename
 
     @classmethod
@@ -343,24 +346,25 @@
         try:
             if not obj.compress_pickle:
                 with filename.open("rb") as ff:
                     tmp_dict = pickle.load(ff)
             else:
                 with bz2.BZ2File(filename, "rb") as ff:
                     tmp_dict = cPickle.load(ff)
-        except Exception:
+        except Exception as ex:
             if not obj.compress_pickle:
                 with filename.open("rb") as ff:
                     tmp_dict = dill.load(ff)
             else:
                 with bz2.BZ2File(filename, "rb") as ff:
                     tmp_dict = dill.load(ff)
 
         obj.__dict__.clear()
         obj.__dict__.update(tmp_dict)
+
         return obj
 
     @classmethod
     def _get_param_names(cls):
         """Get parameter names for the Model"""
         # fetch the constructor or the original constructor before
         # deprecation wrapping if any
@@ -466,18 +470,18 @@
     >>> class RandomAgent(AgentWithSimplePolicy):
     >>>     name = "RandomAgent"
     >>>
     >>>     def __init__(self, env, **kwargs):
     >>>         AgentWithSimplePolicy.__init__(self, env, **kwargs)
     >>>
     >>>         def fit(self, budget=100, **kwargs):
-    >>>             observation = self.env.reset()
+    >>>             observation,info = self.env.reset()
     >>>             for ep in range(budget):
     >>>                 action = self.policy(observation)
-    >>>                 observation, reward, done, _ = self.env.step(action)
+    >>>                 observation, reward, terminated, truncated, info = self.env.step(action)
     >>>
     >>>         def policy(self, observation):
     >>>             return self.env.action_space.sample()  # choose an action at random
     """
 
     @abstractmethod
     def policy(self, observation):
@@ -505,17 +509,196 @@
         References
         ----------
         .. [1] http://incompleteideas.net/book/first/ebook/node50.html
         """
         del kwargs  # unused
         episode_rewards = np.zeros(n_simulations)
         for sim in range(n_simulations):
-            observation = self.eval_env.reset()
+            observation, info = self.eval_env.reset()
             tt = 0
             while tt < eval_horizon:
                 action = self.policy(observation)
-                observation, reward, done, _ = self.eval_env.step(action)
+                observation, reward, terminated, truncated, info = self.eval_env.step(
+                    action
+                )
+                done = terminated or truncated
                 episode_rewards[sim] += reward * np.power(gamma, tt)
                 tt += 1
                 if done:
                     break
         return episode_rewards.mean()
+
+
+class AgentTorch(Agent):
+    """Interface for torch agent agents to specify the save and load.
+
+    Parameters
+    ----------
+    env : gym.Env or tuple (constructor, kwargs)
+        Environment used to fit the agent.
+    eval_env : gym.Env or tuple (constructor, kwargs)
+        Environment on which to evaluate the agent. If None, copied from env.
+    copy_env : bool
+        If true, makes a deep copy of the environment.
+    compress_pickle : bool
+        If true, compress the save files using bz2.
+    seeder : :class:`~rlberry.seeding.seeder.Seeder`, int, or None
+        Seeder/seed for random number generation.
+    output_dir : str or Path
+        Directory that the agent can use to store data.
+    _execution_metadata : ExecutionMetadata, optional
+        Extra information about agent execution (e.g. about which is the process id where the agent is running).
+        Used by :class:`~rlberry.manager.AgentManager`.
+    _default_writer_kwargs : dict, optional
+        Parameters to initialize :class:`~rlberry.utils.writers.DefaultWriter` (attribute self.writer).
+        Used by :class:`~rlberry.manager.AgentManager`.
+    _thread_shared_data : dict, optional
+        Used by :class:`~rlberry.manager.AgentManager` to share data across Agent
+        instances created in different threads.
+    **kwargs : dict
+        Classes that implement this interface must send ``**kwargs``
+        to :code:`Agent.__init__()`.
+
+    Attributes
+    ----------
+    name : string
+        Agent identifier (not necessarily unique).
+    env : :class:`gym.Env` or tuple (constructor, kwargs)
+        Environment on which to train the agent.
+    eval_env : :class:`gym.Env` or tuple (constructor, kwargs)
+        Environment on which to evaluate the agent. If None, copied from env.
+    writer : object, default: None
+        Writer object (e.g. tensorboard SummaryWriter).
+    seeder : :class:`~rlberry.seeding.seeder.Seeder`, int, or None
+        Seeder/seed for random number generation.
+    rng : :class:`numpy.random._generator.Generator`
+        Random number generator. If you use random numbers in your agent, this
+        attribute must be used in order to ensure reproducibility. See `numpy's
+        documentation <https://numpy.org/doc/stable/reference/random/generator.html>`_.
+    output_dir : str or Path
+        Directory that the agent can use to store data.
+    unique_id : str
+        Unique identifier for the agent instance. Can be used, for example,
+        to create files/directories for the agent to log data safely.
+    thread_shared_data : dict
+        Data shared by agent instances among different threads.
+    """
+
+    def save(self, filename):
+        """
+        Overwrite the 'save' function to manage CPU vs GPU  save/load in torch agent
+
+        ----- documentation from original save -----
+
+        Save agent object. By default, the agent is pickled.
+
+        If overridden, the load() method must also be overriden.
+
+        Before saving, consider setting writer to None if it can't be pickled (tensorboard writers
+        keep references to files and cannot be pickled).
+
+        Note: dill[1]_ is used when pickle fails
+        (see https://stackoverflow.com/a/25353243, for instance).
+        Pickle is tried first, since it is faster.
+
+        Parameters
+        ----------
+        filename: Path or str
+            File in which to save the Agent.
+
+        Returns
+        -------
+        pathlib.Path
+            If save() is successful, a Path object corresponding to the filename is returned.
+            Otherwise, None is returned.
+        .. warning:: The returned filename might differ from the input filename: For instance,
+        the method can append the correct suffix to the name before saving.
+
+        References
+        ----------
+        .. [1] https://github.com/uqfoundation/dill
+        """
+
+        import torch
+
+        # remove writer if not pickleable
+        if not dill.pickles(self.writer):
+            self.set_writer(None)
+        # save
+        filename = Path(filename).with_suffix(".pickle")
+        filename.parent.mkdir(parents=True, exist_ok=True)
+
+        dict_to_save = dict(self.__dict__)
+
+        try:
+            if not self.compress_pickle:
+                with filename.open("wb") as ff:
+                    # pickle.dump(dict_to_save, ff)
+                    torch.save(dict_to_save, ff, pickle)
+            else:
+                with bz2.BZ2File(filename, "wb") as ff:
+                    # cPickle.dump(dict_to_save, ff)
+                    torch.save(dict_to_save, ff, cPickle)
+        except Exception as ex:
+            try:
+                if not self.compress_pickle:
+                    with filename.open("wb") as ff:
+                        # dill.dump(dict_to_save, ff)
+                        torch.save(dict_to_save, ff, dill)
+                else:
+                    with bz2.BZ2File(filename, "wb") as ff:
+                        # dill.dump(dict_to_save, ff)
+                        torch.save(dict_to_save, ff, dill)
+            except Exception as ex:
+                logger.warning("Agent instance cannot be pickled: " + str(ex))
+                return None
+
+        return filename
+
+    @classmethod
+    def load(cls, filename, **kwargs):
+        """
+        Overwrite the 'save' and 'load' functions to manage CPU vs GPU  save/load in torch agent.
+
+        ----- documentation from original load -----
+        Load agent object.
+        If overridden, save() method must also be overriden.
+
+        Parameters
+        ----------
+        **kwargs: dict
+            Arguments to required by the __init__ method of the Agent subclass.
+        """
+
+        from rlberry.utils.torch import choose_device
+        import torch
+
+        device_str = "cuda:best"
+        if "device" in kwargs.keys():
+            device_str = kwargs.pop("device", None)
+        device = choose_device(device_str)
+
+        filename = Path(filename).with_suffix(".pickle")
+        obj = cls(**kwargs)
+
+        try:
+            if not obj.compress_pickle:
+                with filename.open("rb") as ff:
+                    tmp_dict = torch.load(ff, map_location=device, pickle_module=pickle)
+            else:
+                with bz2.BZ2File(filename, "rb") as ff:
+                    tmp_dict = torch.load(
+                        ff, map_location=device, pickle_module=cPickle
+                    )
+        except Exception as ex:
+            if not obj.compress_pickle:
+                with filename.open("rb") as ff:
+                    tmp_dict = torch.load(ff, map_location=device, pickle_module=dill)
+            else:
+                with bz2.BZ2File(filename, "rb") as ff:
+                    tmp_dict = torch.load(ff, map_location=device, pickle_module=dill)
+
+        obj.__dict__.clear()
+        obj.__dict__.update(tmp_dict)
+
+        obj.device = device
+        return obj
```

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/bandit_base.py` & `rlberry-0.5.0/rlberry/agents/bandits/bandit_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         horizon = budget
         rewards = np.zeros(horizon)
 
         for ep in range(horizon):
             # choose the optimal action
             # for demo purpose, we will always choose action 0
             action = 0
-            _, reward, _, _ = self.env.step(action)
+            _, reward, _, _, _ = self.env.step(action)
             self.tracker.update(action, reward)
             rewards[ep] = reward
 
         self.optimal_action = 0
         info = {"episode_reward": np.sum(rewards)}
         return info
```

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/index_agents.py` & `rlberry-0.5.0/rlberry/agents/bandits/index_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             if ep < self.n_arms:
                 action = ep
             else:
                 # Compute index for each arm and play the highest one
                 indices = self.index_function(self.tracker)
                 action = np.argmax(indices)
 
-            _, reward, _, _ = self.env.step(action)
+            _, reward, _, _, _ = self.env.step(action)
 
             # Feed the played action and the resulting reward to the tracker
             self.tracker.update(action, reward)
 
             total_reward += reward
 
         # Best action in hinsight is the one with highest index
```

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/indices.py` & `rlberry-0.5.0/rlberry/agents/bandits/indices.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/priors.py` & `rlberry-0.5.0/rlberry/agents/bandits/priors.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/randomized_agents.py` & `rlberry-0.5.0/rlberry/agents/bandits/randomized_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 probs = [float(k == action) for k in self.arms]
             else:
                 # Compute sampling probability for each arm
                 # and play one at random
                 probs = self.prob_function(self.tracker)
                 action = self.rng.choice(self.arms, p=probs)
 
-            _, reward, _, _ = self.env.step(action)
+            _, reward, _, _, _ = self.env.step(action)
 
             # Feed the played action and the resulting reward and sampling
             # probability to the tracker.
             self.tracker.update(action, reward, {"p": probs[action]})
 
             total_reward += reward
```

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/tools/tracker.py` & `rlberry-0.5.0/rlberry/agents/bandits/tools/tracker.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/bandits/ts_agents.py` & `rlberry-0.5.0/rlberry/agents/bandits/ts_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                 action = ep
             else:
                 # Sample from mean parameters from prior distributions
                 sample_mu = self.prior_sampler(self.tracker)
                 # Play the best sampled mean
                 action = np.argmax(sample_mu)
 
-            _, reward, _, _ = self.env.step(action)
+            _, reward, _, _, _ = self.env.step(action)
 
             # Feed the played action and the resulting reward to the tracker
             self.tracker.update(action, reward)
 
             total_reward += reward
 
         # Best action in hinsight is the one with highest index
```

### Comparing `rlberry-0.4.1/rlberry/agents/dynprog/utils.py` & `rlberry-0.5.0/rlberry/agents/dynprog/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/dynprog/value_iteration.py` & `rlberry-0.5.0/rlberry/agents/dynprog/value_iteration.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/experimental/tests/test_sac.py` & `rlberry-0.5.0/rlberry/agents/experimental/tests/test_sac.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/experimental/torch/sac/sac.py` & `rlberry-0.5.0/rlberry/agents/experimental/torch/sac/sac.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from .utils import ReplayBuffer, get_qref, get_vref, alpha_sync
 
 import torch
 import torch.nn as nn
 from torch.nn.functional import one_hot
-
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.agents.torch.utils.models import default_value_net_fn
 from rlberry.agents.torch.utils.models import default_twinq_net_fn
 from rlberry.utils.torch import choose_device
@@ -245,36 +244,46 @@
         action_logprob = action_dist.log_prob(action)
 
         return action.item(), action_logprob.item()
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         done = False
 
         while not done:
             # running policy_old
-            action, action_logprob = self._select_action(state)
-            next_state, reward, done, info = self.env.step(action)
+            action, action_logprob = self._select_action(observation)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward
 
             # check whether to use bonus
             bonus = 0.0
             if self.use_bonus:
                 if info is not None and "exploration_bonus" in info:
                     bonus = info["exploration_bonus"]
 
             # save in batch
             self.replay_buffer.push(
-                (state, next_state, action, action_logprob, reward + bonus, done)
+                (
+                    observation,
+                    next_observation,
+                    action,
+                    action_logprob,
+                    reward + bonus,
+                    done,
+                )
             )
 
-            # update state
-            state = next_state
+            # update observation
+            observation = next_observation
 
         # update; TODO this condition "self.episode % self.batch_size == 0:" seems to be  completely random to me
         # implement self.episode -> self.steps
         self.episode += 1
         if self.episode % self.batch_size == 0:
             self._update()
```

### Comparing `rlberry-0.4.1/rlberry/agents/experimental/torch/sac/utils.py` & `rlberry-0.5.0/rlberry/agents/experimental/torch/sac/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch.nn.functional import one_hot
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 import numpy as np
 
 
 class ReplayBuffer:
     def __init__(self, capacity, rng):
         """
         Parameters
```

### Comparing `rlberry-0.4.1/rlberry/agents/features/feature_map.py` & `rlberry-0.5.0/rlberry/agents/features/feature_map.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/kernel_based/common.py` & `rlberry-0.5.0/rlberry/agents/kernel_based/common.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/kernel_based/kernels.py` & `rlberry-0.5.0/rlberry/agents/kernel_based/kernels.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/kernel_based/rs_kernel_ucbvi.py` & `rlberry-0.5.0/rlberry/agents/kernel_based/rs_kernel_ucbvi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from rlberry.utils.jit_setup import numba_jit
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.dynprog.utils import backward_induction
 from rlberry.agents.dynprog.utils import backward_induction_in_place
 from rlberry.utils.metrics import metric_lp
 from rlberry.agents.kernel_based.kernels import kernel_func
 from rlberry.agents.kernel_based.common import map_to_representative
 
@@ -351,20 +351,23 @@
         assert self.Q is not None
         repr_state = self._map_to_repr(state, False)
         return self.Q[hh, repr_state, :].argmax()
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
-            self._update(state, action, next_state, reward)
-            state = next_state
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
+            self._update(observation, action, next_observation, reward)
+            observation = next_observation
             episode_rewards += reward
 
             if done:
                 break
 
         # run backward induction
         backward_induction_in_place(
```

### Comparing `rlberry-0.4.1/rlberry/agents/kernel_based/rs_ucbvi.py` & `rlberry-0.5.0/rlberry/agents/kernel_based/rs_ucbvi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rlberry.agents.agent import AgentWithSimplePolicy
 import numpy as np
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents.dynprog.utils import backward_induction
 from rlberry.agents.dynprog.utils import backward_induction_in_place
 from rlberry.agents.kernel_based.common import map_to_representative
 
 import rlberry
 
 logger = rlberry.logger
@@ -289,26 +289,29 @@
         assert self.Q is not None
         repr_state = self._map_to_repr(state, False)
         return self.Q[hh, repr_state, :].argmax()
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward  # used for logging only
 
             if self.reward_free:
                 reward = 0.0  # set to zero before update if reward_free
 
-            self._update(state, action, next_state, reward)
+            self._update(observation, action, next_observation, reward)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # run backward induction
         backward_induction_in_place(
             self.Q[:, : self.M, :],
             self.V[:, : self.M],
```

### Comparing `rlberry-0.4.1/rlberry/agents/linear/lsvi_ucb.py` & `rlberry-0.5.0/rlberry/agents/linear/lsvi_ucb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from rlberry.agents import AgentWithSimplePolicy
-from gym.spaces import Discrete
+from gymnasium.spaces import Discrete
 from rlberry.utils.jit_setup import numba_jit
 
 import rlberry
 
 logger = rlberry.logger
 
 
@@ -253,54 +253,57 @@
 
     def _optimistic_policy(self, observation, hh):
         q_w = self.w_vec[hh, :]
         q_vec = self._compute_q_vec(q_w, observation, self.bonus_scale_factor)
         return q_vec.argmax()
 
     def run_episode(self):
-        state = self.env.reset()
+        observation, info = self.env.reset()
         episode_rewards = 0
         for hh in range(self.horizon):
             if self.bonus_scale_factor == 0.0:
                 action = self.env.action_space.sample()
             else:
-                action = self._optimistic_policy(state, hh)
+                action = self._optimistic_policy(observation, hh)
 
-            next_state, reward, is_terminal, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
 
-            feat = self.feature_map.map(state, action)
+            feat = self.feature_map.map(observation, action)
             outer_prod = np.outer(feat, feat)
             inv = self.lambda_mat_inv
 
             #
             self.lambda_mat += np.outer(feat, feat)
             # update inverse
             self.lambda_mat_inv -= (inv @ outer_prod @ inv) / (1 + feat @ inv.T @ feat)
 
             # update history
             self.reward_hist[self.total_time_steps] = reward
-            self.state_hist.append(state)
+            self.state_hist.append(observation)
             self.action_hist.append(action)
-            self.nstate_hist.append(next_state)
+            self.nstate_hist.append(next_observation)
 
             #
             tt = self.total_time_steps
-            self.feat_hist[tt, :] = self.feature_map.map(state, action)
+            self.feat_hist[tt, :] = self.feature_map.map(observation, action)
             for aa in range(self.env.action_space.n):
                 self.feat_ns_all_actions[tt, aa, :] = self.feature_map.map(
-                    next_state, aa
+                    next_observation, aa
                 )
 
             # increments
             self.total_time_steps += 1
             episode_rewards += reward
 
             #
-            state = next_state
-            if is_terminal:
+            observation = next_observation
+            if done:
                 break
 
         # store data
         self._rewards[self.episode] = episode_rewards
 
         # update ep
         self.episode += 1
```

### Comparing `rlberry-0.4.1/rlberry/agents/mbqvi/mbqvi.py` & `rlberry-0.5.0/rlberry/agents/mbqvi/mbqvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.dynprog.utils import backward_induction, value_iteration
-from gym.spaces import Discrete
+from gymnasium.spaces import Discrete
 
 import rlberry
 
 logger = rlberry.logger
 
 
 class MBQVIAgent(AgentWithSimplePolicy):
@@ -100,15 +100,15 @@
         logger.debug(
             f"[{self.name}] collecting {self.n_samples} samples per (s,a)"
             f", total = {total_samples} samples."
         )
         for ss in range(S):
             for aa in range(A):
                 for _ in range(self.n_samples):
-                    next_state, reward, _, _ = self.env.sample(ss, aa)
+                    next_state, reward, _, _, _ = self.env.sample(ss, aa)
                     self._update(ss, aa, next_state, reward)
 
                     count += 1
                     if count % 10000 == 0:
                         completed = 100 * count / total_samples
                         logger.debug(
                             "[{}] ... {}/{} ({:0.0f}%)".format(
```

### Comparing `rlberry-0.4.1/rlberry/agents/optql/optql.py` & `rlberry-0.5.0/rlberry/agents/optql/optql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 
 import rlberry
 
 logger = rlberry.logger
 
@@ -154,25 +154,28 @@
                 self.Q[hh, state, action] + bonus
             )  # bonus here
             self.V[hh, state] = min(self.v_max[hh], self.Q_bar[hh, state, :].max())
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward  # used for logging only
 
-            self.counter.update(state, action)
+            self.counter.update(observation, action)
 
-            self._update(state, action, next_state, reward, hh)
+            self._update(observation, action, next_observation, reward, hh)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # update info
         self.episode += 1
 
         # writer
```

### Comparing `rlberry-0.4.1/rlberry/agents/psrl/psrl.py` & `rlberry-0.5.0/rlberry/agents/psrl/psrl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 from rlberry.agents.dynprog.utils import (
     backward_induction_in_place,
     backward_induction_sd,
 )
 
@@ -184,28 +184,31 @@
                 self.P_sample,
                 self.horizon,
                 self.gamma,
                 self.v_max[0],
             )
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward  # used for logging only
 
-            self.counter.update(state, action)
+            self.counter.update(observation, action)
 
             if self.reward_free:
                 reward = 0.0  # set to zero before update if reward_free
 
-            self._update(state, action, next_state, reward, hh)
+            self._update(observation, action, next_observation, reward, hh)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # update info
         self.episode += 1
 
         # writer
```

### Comparing `rlberry-0.4.1/rlberry/agents/rlsvi/rlsvi.py` & `rlberry-0.5.0/rlberry/agents/rlsvi/rlsvi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 from rlberry.agents.dynprog.utils import (
     backward_induction_in_place,
     backward_induction_reward_sd,
     backward_induction_sd,
 )
@@ -204,28 +204,31 @@
                 self.V,
                 self.R_hat + noise_sa,
                 self.P_hat,
                 self.gamma,
                 self.v_max[0],
             )
 
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward  # used for logging only
 
-            self.counter.update(state, action)
+            self.counter.update(observation, action)
 
             if self.reward_free:
                 reward = 0.0  # set to zero before update if reward_free
 
-            self._update(state, action, next_state, reward, hh)
+            self._update(observation, action, next_observation, reward, hh)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # update info
         self.episode += 1
 
         # writer
```

### Comparing `rlberry-0.4.1/rlberry/agents/stable_baselines/stable_baselines.py` & `rlberry-0.5.0/rlberry/agents/stable_baselines/stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tabular_rl/qlearning.py` & `rlberry-0.5.0/rlberry/agents/tabular_rl/sarsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Literal
 import numpy as np
-from gym import spaces
+from gymnasium import spaces
 from scipy.special import softmax
 
 from rlberry import types
 from rlberry.agents import AgentWithSimplePolicy
 
 
-class QLAgent(AgentWithSimplePolicy):
-    """Q-Learning Agent.
+class SARSAAgent(AgentWithSimplePolicy):
+    """SARSA Agent.
 
     Parameters
     ----------
     env: :class:`~rlberry.types.Env`
         Environment with discrete states and actions.
     gamma: float, default = 0.99
         Discount factor.
@@ -25,28 +25,25 @@
     exploration_rate: float, default: None
         epsilon parameter for Epsilon-Greedy exploration or tau parameter for Boltzmann exploration.
 
     Attributes
     ----------
     Q : ndarray
         2D array that stores the estimation ofexpected rewards for state-action pairs.
-
     Examples
     --------
     >>> from rlberry.envs import GridWorld
     >>>
     >>> env = GridWorld(walls=(), nrows=5, ncols=5)
-    >>> agent = QLAgent()
+    >>> agent = SARSAAgent()
     >>> agent.fit(budget=1000)
     >>> agent.policy(env.observation_space.sample())
     >>> agent.reset()
     """
 
-    name = "QL"
-
     def __init__(
         self,
         env: types.Env,
         gamma: float = 0.99,
         alpha: float = 0.1,
         exploration_type: Optional[Literal["epsilon", "boltzmann"]] = None,
         exploration_rate: Optional[float] = None,
@@ -96,29 +93,33 @@
         Train the agent using the provided environment.
         Parameters
         ----------
         budget: int
             number of Q updates.
         """
         del kwargs
-        observation = self.env.reset()
+        observation, info = self.env.reset()
         episode_rewards = 0
         for i in range(budget):
             action = self.get_action(observation)
-            next_observation, reward, done, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward
             if self.writer is not None:
                 self.writer.add_scalar("episode_rewards", episode_rewards, i)
             if done:
                 self.Q[observation, action] = reward
             else:
+                next_action = self.get_action(next_observation)
                 self.Q[observation, action] = self.Q[
                     observation, action
                 ] + self.alpha * (
                     reward
-                    + self.gamma * np.amax(self.Q[next_observation])
+                    + self.gamma * self.Q[next_observation, next_action]
                     - self.Q[observation, action]
                 )
             observation = next_observation
             if done:
-                observation = self.env.reset()
+                observation, info = self.env.reset()
                 episode_rewards = 0
```

### Comparing `rlberry-0.4.1/rlberry/agents/tabular_rl/sarsa.py` & `rlberry-0.5.0/rlberry/agents/tabular_rl/qlearning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Literal
 import numpy as np
-from gym import spaces
+from gymnasium import spaces
 from scipy.special import softmax
 
 from rlberry import types
 from rlberry.agents import AgentWithSimplePolicy
 
 
-class SARSAAgent(AgentWithSimplePolicy):
-    """SARSA Agent.
+class QLAgent(AgentWithSimplePolicy):
+    """Q-Learning Agent.
 
     Parameters
     ----------
     env: :class:`~rlberry.types.Env`
         Environment with discrete states and actions.
     gamma: float, default = 0.99
         Discount factor.
@@ -25,25 +25,28 @@
     exploration_rate: float, default: None
         epsilon parameter for Epsilon-Greedy exploration or tau parameter for Boltzmann exploration.
 
     Attributes
     ----------
     Q : ndarray
         2D array that stores the estimation ofexpected rewards for state-action pairs.
+
     Examples
     --------
     >>> from rlberry.envs import GridWorld
     >>>
     >>> env = GridWorld(walls=(), nrows=5, ncols=5)
-    >>> agent = SARSAAgent()
+    >>> agent = QLAgent()
     >>> agent.fit(budget=1000)
     >>> agent.policy(env.observation_space.sample())
     >>> agent.reset()
     """
 
+    name = "QL"
+
     def __init__(
         self,
         env: types.Env,
         gamma: float = 0.99,
         alpha: float = 0.1,
         exploration_type: Optional[Literal["epsilon", "boltzmann"]] = None,
         exploration_rate: Optional[float] = None,
@@ -93,30 +96,32 @@
         Train the agent using the provided environment.
         Parameters
         ----------
         budget: int
             number of Q updates.
         """
         del kwargs
-        observation = self.env.reset()
+        observation, info = self.env.reset()
         episode_rewards = 0
         for i in range(budget):
             action = self.get_action(observation)
-            next_observation, reward, done, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward
             if self.writer is not None:
                 self.writer.add_scalar("episode_rewards", episode_rewards, i)
             if done:
                 self.Q[observation, action] = reward
             else:
-                next_action = self.get_action(next_observation)
                 self.Q[observation, action] = self.Q[
                     observation, action
                 ] + self.alpha * (
                     reward
-                    + self.gamma * self.Q[next_observation, next_action]
+                    + self.gamma * np.amax(self.Q[next_observation])
                     - self.Q[observation, action]
                 )
             observation = next_observation
             if done:
-                observation = self.env.reset()
+                observation, info = self.env.reset()
                 episode_rewards = 0
```

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_bandits.py` & `rlberry-0.5.0/rlberry/agents/tests/test_bandits.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_dynprog.py` & `rlberry-0.5.0/rlberry/agents/tests/test_dynprog.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_kernel_based.py` & `rlberry-0.5.0/rlberry/agents/tests/test_kernel_based.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_lsvi_ucb.py` & `rlberry-0.5.0/rlberry/agents/tests/test_lsvi_ucb.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,18 @@
         states and actions
         """
         N = agent.n_episodes * agent.horizon
         count = 0
         while count < N:
             state = agent.env.observation_space.sample()
             action = agent.env.action_space.sample()
-            next_state, reward, done, info = agent.env.sample(state, action)
+            next_state, reward, terminated, truncated, info = agent.env.sample(
+                state, action
+            )
+            done = terminated or truncated
             #
             #
             feat = agent.feature_map.map(state, action)
             outer_prod = np.outer(feat, feat)
             inv = agent.lambda_mat_inv
 
             #
```

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_mbqvi.py` & `rlberry-0.5.0/rlberry/agents/tests/test_mbqvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_psrl.py` & `rlberry-0.5.0/rlberry/agents/tests/test_psrl.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_replay.py` & `rlberry-0.5.0/rlberry/agents/tests/test_replay.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import numpy as np
 from rlberry.agents.utils import replay
 from rlberry.envs.finite import GridWorld
-from gym.wrappers import TimeLimit
+from gymnasium.wrappers import TimeLimit
 
 
 def _get_filled_replay(max_replay_size):
     """runs env for ~ 2 * max_replay_size timesteps."""
     env = GridWorld(terminal_states=None)
     env = TimeLimit(env, max_episode_steps=200)
     env.reseed(123)
@@ -25,28 +25,29 @@
 
     # Fill the replay buffer
     total_time = 0
     while True:
         if total_time > 2 * buffer._max_replay_size:
             break
         done = False
-        obs = env.reset()
+        observation, info = env.reset()
         while not done:
             total_time += 1
             action = env.action_space.sample()
-            next_obs, reward, done, _ = env.step(action)
+            next_observation, reward, terminated, truncated, info = env.step(action)
+            done = terminated or truncated
             buffer.append(
                 {
-                    "observations": obs,
+                    "observations": observation,
                     "actions": action,
                     "rewards": reward,
                     "dones": done,
                 }
             )
-            obs = next_obs
+            observation = next_observation
             if done:
                 buffer.end_episode()
     return buffer, env
 
 
 def test_replay_size():
     # get replay buffer
@@ -109,19 +110,20 @@
     # add more data, sample batches and check that sampled sub-trajetories
     # are not "crossing" the current position (buffer._position)
     total_time = 0
     while True:
         if total_time > 1000:
             break
         done = False
-        obs = env.reset()
+        obs, info = env.reset()
         while not done:
             total_time += 1
             action = env.action_space.sample()
-            next_obs, reward, done, _ = env.step(action)
+            next_obs, reward, terminated, truncated, _ = env.step(action)
+            done = terminated or truncated
             buffer.append(
                 {
                     "observations": obs,
                     "actions": action,
                     "rewards": reward,
                     "dones": done,
                 }
```

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_stable_baselines.py` & `rlberry-0.5.0/rlberry/agents/tests/test_stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_tabular_rl.py` & `rlberry-0.5.0/rlberry/agents/tests/test_tabular_rl.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/tests/test_ucbvi.py` & `rlberry-0.5.0/rlberry/agents/tests/test_ucbvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/a2c/a2c.py` & `rlberry-0.5.0/rlberry/agents/torch/a2c/a2c.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import torch
 import torch.nn as nn
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 import numpy as np
-from rlberry.agents import AgentWithSimplePolicy
+from rlberry.agents import AgentWithSimplePolicy, AgentTorch
 from rlberry.agents.utils.replay import ReplayBuffer
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.agents.torch.utils.models import default_value_net_fn
 from rlberry.utils.torch import choose_device
 from rlberry.utils.factory import load
 from typing import Optional
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class A2CAgent(AgentWithSimplePolicy):
+class A2CAgent(AgentTorch, AgentWithSimplePolicy):
     """
     Advantage Actor Critic Agent.
 
     A2C, or Advantage Actor Critic, is a synchronous version of the A3C policy
     gradient method. As an alternative to the asynchronous implementation of
     A3C, A2C is a synchronous, deterministic implementation that waits for each
     actor to finish its segment of experience before updating, averaging over
@@ -183,18 +183,21 @@
             Number of timesteps to train the agent for.
             One step = one transition in the environment.
         """
         del kwargs
         timesteps_counter = 0
         episode_rewards = 0.0
         episode_timesteps = 0
-        observation = self.env.reset()
+        observation, info = self.env.reset()
         while timesteps_counter < budget:
             action = self._select_action(observation)
-            next_obs, reward, done, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             # if self._policy.ctns_actions:
             #     action = torch.from_numpy(action).float().to(self.device)
             # store data
             episode_rewards += reward
             self.memory.append(
                 {
                     "states": observation,
@@ -204,15 +207,15 @@
                 }
             )
 
             # counters and next obs
             self.total_timesteps += 1
             timesteps_counter += 1
             episode_timesteps += 1
-            observation = next_obs
+            observation = next_observation
 
             # update
             if self.total_timesteps % self.batch_size == 0:
                 self._update()
 
             # eval
             total_timesteps = self.total_timesteps
@@ -239,15 +242,15 @@
                         "episode_rewards", episode_rewards, total_timesteps
                     )
                     self.writer.add_scalar(
                         "total_episodes", self.total_episodes, total_timesteps
                     )
                 episode_rewards = 0.0
                 episode_timesteps = 0
-                observation = self.env.reset()
+                observation, info = self.env.reset()
 
     def _select_action(self, state):
         state = torch.from_numpy(state).float().to(self.device)
         action_dist = self._policy_old(state)
         action = action_dist.sample()
         if self._policy.ctns_actions:
             action = action.numpy()
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/dqn/dqn.py` & `rlberry-0.5.0/rlberry/agents/torch/dqn/dqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 from typing import Callable, Optional, Union
 
-from gym import spaces
+from gymnasium import spaces
 import numpy as np
 import torch
 
 from rlberry import types
-from rlberry.agents import AgentWithSimplePolicy
+from rlberry.agents import AgentWithSimplePolicy, AgentTorch
 from rlberry.agents.torch.utils.training import (
     loss_function_factory,
     model_factory,
     optimizer_factory,
     size_model_config,
 )
 from rlberry.agents.torch.dqn.dqn_utils import polynomial_schedule, lambda_returns
@@ -34,15 +34,15 @@
         "layer_sizes": (64, 64),
         "reshape": False,
     }
     model_config = size_model_config(env, **model_config)
     return model_factory(**model_config)
 
 
-class DQNAgent(AgentWithSimplePolicy):
+class DQNAgent(AgentTorch, AgentWithSimplePolicy):
     """DQN Agent based on PyTorch.
 
     Notes
     -----
     Uses Q(lambda) for computing targets by default. To recover
     the standard DQN, set :code:`lambda_ = 0.0` and :code:`chunk_size = 1`.
 
@@ -156,14 +156,15 @@
         max_replay_size: int = 200_000,
         learning_starts: int = 5_000,
         eval_interval: Optional[int] = None,
         **kwargs,
     ):
         # For all parameters, define self.param = param
         _, _, _, values = inspect.getargvalues(inspect.currentframe())
+
         values.pop("self")
         for arg, val in values.items():
             setattr(self, arg, val)
 
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
         env = self.env
         assert isinstance(env.observation_space, spaces.Box)
@@ -365,40 +366,43 @@
             Number of timesteps to train the agent for.
             One step = one transition in the environment.
         """
         del kwargs
         timesteps_counter = 0
         episode_rewards = 0.0
         episode_timesteps = 0
-        observation = self.env.reset()
+        observation, info = self.env.reset()
         while timesteps_counter < budget:
             if self.total_timesteps < self._learning_starts:
                 action = self.env.action_space.sample()
             else:
                 self._timesteps_since_last_update += 1
                 action = self._policy(observation, evaluation=False)
-            next_obs, reward, done, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
 
             # store data
             episode_rewards += reward
             self._replay_buffer.append(
                 {
                     "observations": observation,
                     "actions": action,
                     "rewards": reward,
                     "dones": done,
-                    "next_observations": next_obs,
+                    "next_observations": next_observation,
                 }
             )
 
             # counters and next obs
             self._total_timesteps += 1
             timesteps_counter += 1
             episode_timesteps += 1
-            observation = next_obs
+            observation = next_observation
 
             # update
             run_update, n_gradient_steps = self._must_update(done)
             if run_update:
                 self._update(n_gradient_steps)
 
             # eval
@@ -426,15 +430,15 @@
                         "episode_rewards", episode_rewards, total_timesteps
                     )
                     self.writer.add_scalar(
                         "total_episodes", self._total_episodes, total_timesteps
                     )
                 episode_rewards = 0.0
                 episode_timesteps = 0
-                observation = self.env.reset()
+                observation, info = self.env.reset()
 
     def _policy(self, observation, evaluation=False):
         epsilon = self._epsilon_schedule(self.total_timesteps)
         if (not evaluation) and self.rng.uniform() < epsilon:
             if self.writer:
                 self.writer.add_scalar("epsilon", epsilon, self.total_timesteps)
             return self.env.action_space.sample()
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/dqn/dqn_utils.py` & `rlberry-0.5.0/rlberry/agents/torch/dqn/dqn_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/dqn/mdqn.py` & `rlberry-0.5.0/rlberry/agents/torch/dqn/mdqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 
 import numpy as np
 import torch
-from gym import spaces
+from gymnasium import spaces
 from rlberry import types
-from rlberry.agents import AgentWithSimplePolicy
+from rlberry.agents import AgentWithSimplePolicy, AgentTorch
 from rlberry.agents.torch.utils.training import (
     loss_function_factory,
     model_factory,
     optimizer_factory,
     size_model_config,
 )
 from rlberry.agents.torch.dqn.dqn_utils import (
@@ -38,15 +38,15 @@
         "layer_sizes": (64, 64),
         "reshape": False,
     }
     model_config = size_model_config(env, **model_config)
     return model_factory(**model_config)
 
 
-class MunchausenDQNAgent(AgentWithSimplePolicy):
+class MunchausenDQNAgent(AgentTorch, AgentWithSimplePolicy):
     """Munchausen DQN Agent based on PyTorch.
 
     Notes
     -----
     Uses Munchausen trick for DQN for computing targets by default.
     Compared to DQN, the scaled log-policy was added to the immediate
     reward. Slightly modifying DQN in that way provides an agent that
@@ -389,40 +389,43 @@
             Number of timesteps to train the agent for.
             One step = one transition in the environment.
         """
         del kwargs
         timesteps_counter = 0
         episode_rewards = 0.0
         episode_timesteps = 0
-        observation = self.env.reset()
+        observation, info = self.env.reset()
         while timesteps_counter < budget:
             if self.total_timesteps < self._learning_starts:
                 action = self.env.action_space.sample()
             else:
                 self._timesteps_since_last_update += 1
                 action = self._policy(observation, evaluation=False)
-            next_obs, reward, done, _ = self.env.step(action)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
 
             # store data
             episode_rewards += reward
             self._replay_buffer.append(
                 {
                     "observations": observation,
                     "actions": action,
                     "rewards": reward,
                     "dones": done,
-                    "next_observations": next_obs,
+                    "next_observations": next_observation,
                 }
             )
 
             # counters and next obs
             self._total_timesteps += 1
             timesteps_counter += 1
             episode_timesteps += 1
-            observation = next_obs
+            observation = next_observation
 
             # update
             run_update, n_gradient_steps = self._must_update(done)
             if run_update:
                 self._update(n_gradient_steps)
 
             # eval
@@ -450,15 +453,15 @@
                         "episode_rewards", episode_rewards, total_timesteps
                     )
                     self.writer.add_scalar(
                         "total_episodes", self._total_episodes, total_timesteps
                     )
                 episode_rewards = 0.0
                 episode_timesteps = 0
-                observation = self.env.reset()
+                observation, info = self.env.reset()
 
     def _policy(self, observation, evaluation=False):
         epsilon = self._epsilon_schedule(self.total_timesteps)
         if (not evaluation) and self.rng.uniform() < epsilon:
             if self.writer:
                 self.writer.add_scalar("epsilon", epsilon, self.total_timesteps)
             return self.env.action_space.sample()
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/ppo/ppo.py` & `rlberry-0.5.0/rlberry/agents/torch/ppo/ppo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-import gym.spaces as spaces
 import numpy as np
 import torch
 import torch.nn as nn
 
+import gymnasium.spaces as spaces
 import rlberry
 from rlberry.agents import AgentWithSimplePolicy
+from rlberry.agents import AgentTorch
 from rlberry.envs.utils import process_env
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.agents.torch.utils.models import default_value_net_fn
 from rlberry.utils.torch import choose_device
 from rlberry.utils.factory import load
 from rlberry.agents.torch.ppo.ppo_utils import (
     process_ppo_env,
     lambda_returns,
     RolloutBuffer,
 )
 
+import dill
+import pickle
+import bz2
+import _pickle as cPickle
+from pathlib import Path
+
+
 logger = rlberry.logger
 
 
 # Notes about VecEnvs:
 # - reset() returns a numpy array of shape (n_envs, state_dim)
 # - step() returns a tuple of arrays (states, rewards, dones, infos)
 #   - states: np.array (n_envs, state_dim) dtype varies
 #   - rewards: np.array (n_envs,) np.float64
 #   - dones: np.array (n_envs,) bool
 #   - infos: list (n_envs,) dict
 # - close() closes all environments
 
 
-class PPOAgent(AgentWithSimplePolicy):
+class PPOAgent(AgentTorch, AgentWithSimplePolicy):
     """
     Proximal Policy Optimization Agent.
 
     Policy gradient methods for reinforcement learning, which alternate between
     sampling data through interaction with the environment, and optimizing a
     “surrogate” objective function using stochastic gradient ascent.
 
@@ -122,14 +130,15 @@
     name = "PPO"
     __value_losses__ = ["clipped", "mse", "avec"]
     __lr_schedule___ = ["constant", "linear"]
 
     def __init__(
         self,
         env,
+        copy_env=True,
         n_envs=1,
         n_steps=512,
         batch_size=64,
         gamma=0.99,
         k_epochs=10,
         clip_eps=0.2,
         target_kl=0.05,
@@ -155,18 +164,19 @@
     ):
         kwargs.pop("eval_env", None)
         AgentWithSimplePolicy.__init__(
             self, None, **kwargs
         )  # PPO handles the env internally
 
         # create environment
+        self.copy_env = copy_env
         self.n_envs = n_envs
-        self.env = process_ppo_env(env, self.seeder, n_envs)
+        self.env = process_ppo_env(env, self.seeder, num_envs=n_envs, copy_env=copy_env)
         eval_env = eval_env or env
-        self.eval_env = process_env(eval_env, self.seeder, copy_env=True)
+        self.eval_env = process_env(eval_env, self.seeder, copy_env=copy_env)
 
         # hyperparameters
         value_loss, lr_schedule = value_loss.lower(), lr_schedule.lower()
         assert value_loss in self.__value_losses__, "value_loss must be in {}".format(
             self.__value_losses__
         )
         assert lr_schedule in self.__lr_schedule___, "lr_schedule must be in {}".format(
@@ -293,55 +303,55 @@
             timesteps_counter = 0
         else:  # it's not the first "fit" on this agent, so there is a previous buffer to continue
             timesteps_counter = len(self.memory) * self.n_envs
 
         episode_returns = np.zeros(self.n_envs, dtype=np.float32)
         episode_lengths = np.zeros(self.n_envs, dtype=np.int32)
 
-        next_obs = torch.Tensor(self.env.reset()).to(
+        next_obs, infos = self.env.reset()
+        next_obs = torch.Tensor(next_obs).to(
             self.device
         )  # should always be a torch tensor
         next_done = np.zeros(self.n_envs, dtype=bool)  # initialize done to False
         while timesteps_counter < budget:
             obs = next_obs
             done = next_done
 
             # select action and take step
             with torch.no_grad():
                 action, logprobs = self._select_action(obs)
-            next_obs, reward, next_done, info = self.env.step(action)
+            next_obs, reward, next_terminated, next_truncated, info = self.env.step(
+                action
+            )
+            next_done = np.logical_or(next_terminated, next_truncated)
             next_obs = torch.Tensor(next_obs).to(self.device)
 
             # end of episode logging
             for i in range(self.n_envs):
                 if next_done[i]:
                     self.total_episodes += 1
-                    if self.writer and "episode" in info[i]:
-                        if "episode" in info[i]:
-                            r, l = info[i]["episode"]["r"], info[i]["episode"]["l"]
+                    if self.writer and "episode" in info["final_info"][i]:
+                        if "episode" in info["final_info"][i]:
+                            r, l = (
+                                info["final_info"][i]["episode"]["r"],
+                                info["final_info"][i]["episode"]["l"],
+                            )
                         else:
                             r, l = episode_returns[i], episode_lengths[i]
                         self.writer.add_scalar(
                             "episode_returns", r, self.total_timesteps
                         )
                         self.writer.add_scalar(
                             "episode_lengths", l, self.total_timesteps
                         )
                         self.writer.add_scalar(
                             "total_episodes", self.total_episodes, self.total_timesteps
                         )
                     episode_returns[i], episode_lengths[i] = 0.0, 0
 
-            # only accept done if not truncated
-            # TODO: not needed with gymnasium
-            for i in range(self.n_envs):
-                if next_done[i]:
-                    if "TimeLimit.truncated" in info[i]:
-                        next_done[i] = False
-
             # append data to memory and update variables
             self.memory.append(
                 {
                     "observations": obs.cpu().numpy(),
                     "actions": action,
                     "rewards": reward,
                     "dones": done,
@@ -649,7 +659,118 @@
             "batch_size": batch_size,
             "gamma": gamma,
             "learning_rate": learning_rate,
             "entr_coef": entr_coef,
             "clip_eps": clip_eps,
             "k_epochs": k_epochs,
         }
+
+    ##### Overwrite some inherited functions
+
+    def save(self, filename):
+        """
+        Overwrite the 'save' and 'load' functions to not store the env if it's a "vectorized env" (can't be managed with pickle)
+
+        ----- documentation from original save -----
+
+        Save agent object. By default, the agent is pickled.
+
+        If overridden, the load() method must also be overriden.
+
+        Before saving, consider setting writer to None if it can't be pickled (tensorboard writers
+        keep references to files and cannot be pickled).
+
+        Note: dill[1]_ is used when pickle fails
+        (see https://stackoverflow.com/a/25353243, for instance).
+        Pickle is tried first, since it is faster.
+
+        Parameters
+        ----------
+        filename: Path or str
+            File in which to save the Agent.
+
+        Returns
+        -------
+        pathlib.Path
+            If save() is successful, a Path object corresponding to the filename is returned.
+            Otherwise, None is returned.
+        .. warning:: The returned filename might differ from the input filename: For instance,
+        the method can append the correct suffix to the name before saving.
+
+        References
+        ----------
+        .. [1] https://github.com/uqfoundation/dill
+        """
+        # remove writer if not pickleable
+        if not dill.pickles(self.writer):
+            self.set_writer(None)
+        # save
+        filename = Path(filename).with_suffix(".pickle")
+        filename.parent.mkdir(parents=True, exist_ok=True)
+
+        dict_to_save = dict(self.__dict__)
+        del dict_to_save["env"]
+        del dict_to_save["eval_env"]
+
+        try:
+            if not self.compress_pickle:
+                with filename.open("wb") as ff:
+                    pickle.dump(dict_to_save, ff)
+            else:
+                with bz2.BZ2File(filename, "wb") as ff:
+                    cPickle.dump(dict_to_save, ff)
+        except Exception:
+            try:
+                if not self.compress_pickle:
+                    with filename.open("wb") as ff:
+                        dill.dump(dict_to_save, ff)
+                else:
+                    with bz2.BZ2File(filename, "wb") as ff:
+                        dill.dump(dict_to_save, ff)
+            except Exception as ex:
+                logger.warning("Agent instance cannot be pickled: " + str(ex))
+                return None
+
+        return filename
+
+    @classmethod
+    def load(cls, filename, **kwargs):
+        """
+        Overwrite the 'save' and 'load' functions to not store the env if it's a "vectorized env" (can't be managed with pickle)
+
+        ----- documentation from original load -----
+        Load agent object.
+        If overridden, save() method must also be overriden.
+
+        Parameters
+        ----------
+        **kwargs: dict
+            Arguments to required by the __init__ method of the Agent subclass.
+        """
+        filename = Path(filename).with_suffix(".pickle")
+        obj = cls(**kwargs)
+
+        try:
+            if not obj.compress_pickle:
+                with filename.open("rb") as ff:
+                    tmp_dict = pickle.load(ff)
+            else:
+                with bz2.BZ2File(filename, "rb") as ff:
+                    tmp_dict = cPickle.load(ff)
+        except Exception:
+            if not obj.compress_pickle:
+                with filename.open("rb") as ff:
+                    tmp_dict = dill.load(ff)
+            else:
+                with bz2.BZ2File(filename, "rb") as ff:
+                    tmp_dict = dill.load(ff)
+
+        temp_env = obj.__dict__["env"]
+        temp_eval_env = obj.__dict__["eval_env"]
+
+        obj.__dict__.clear()
+        obj.__dict__.update(tmp_dict)
+
+        obj.__dict__["env"] = temp_env
+        obj.__dict__["eval_env"] = temp_eval_env
+
+        return obj
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/ppo/ppo_utils.py` & `rlberry-0.5.0/rlberry/agents/torch/ppo/ppo_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import copy
 import logging
 
-import gym
+import gymnasium as gym
 import numpy as np
 
 from rlberry.envs.utils import process_env
 from rlberry.utils.jit_setup import numba_jit
 
 
 logger = logging.getLogger(__name__)
 
 
-def process_ppo_env(env, seeder, num_envs=1, asynchronous=False):
+def process_ppo_env(env, seeder, num_envs=1, asynchronous=False, copy_env=True):
     """
-    Process environment for PPO. It is the only agent that supports vectorized
+    Process environment for PPO. It's the only agent that supports vectorized
     environments.
 
     Parameters
     ----------
     env : gym.Env
         Environment to be processed.
     seeder : rlberry.Seeder
@@ -25,22 +25,22 @@
     num_envs : int
         Number of environments to be used.
     asynchronous : bool
         If True, the environments are run asynchronously.
 
     Returns
     -------
-    vec_env : gym.vector.VectorEnv
+    vec_env : gymnasium.vector.VectorEnv
         Vectorized environment.
     """
     vec_env_cls = (
         gym.vector.AsyncVectorEnv if asynchronous else gym.vector.SyncVectorEnv
     )
     return vec_env_cls(
-        [lambda: process_env(env, seeder, copy_env=True) for _ in range(num_envs)]
+        [lambda: process_env(env, seeder, copy_env=copy_env) for _ in range(num_envs)]
     )
 
 
 @numba_jit
 def lambda_returns(r_t, terminal_tp1, v_tp1, gamma, lambda_):
     """
     Compute lambda returns.
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/reinforce/reinforce.py` & `rlberry-0.5.0/rlberry/agents/torch/reinforce/reinforce.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import torch
 import inspect
 import numpy as np
 
-import gym.spaces as spaces
-from rlberry.agents import AgentWithSimplePolicy
+import gymnasium.spaces as spaces
+from rlberry.agents import AgentWithSimplePolicy, AgentTorch
 from rlberry.agents.utils.memories import Memory
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.utils.torch import choose_device
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class REINFORCEAgent(AgentWithSimplePolicy):
+class REINFORCEAgent(AgentTorch, AgentWithSimplePolicy):
     """
     REINFORCE with entropy regularization.
 
     Parameters
     ----------
     env : Model
         Online model with continuous (Box) state space and discrete actions
@@ -139,38 +139,41 @@
         while count < n_episodes_to_run:
             self._run_episode()
             count += 1
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for _ in range(self.horizon):
             # running policy
-            action = self.policy(state)
-            next_state, reward, done, info = self.env.step(action)
+            action = self.policy(observation)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
 
             # check whether to use bonus
             bonus = 0.0
             if self.use_bonus_if_available:
                 if info is not None and "exploration_bonus" in info:
                     bonus = info["exploration_bonus"]
 
             # save in batch
-            self.memory.states.append(state)
+            self.memory.states.append(observation)
             self.memory.actions.append(action)
             self.memory.rewards.append(reward + bonus)  # add bonus here
             self.memory.is_terminals.append(done)
             episode_rewards += reward
 
             if done:
                 break
 
-            # update state
-            state = next_state
+            # update observation
+            observation = next_observation
 
         # update
         self.episode += 1
 
         #
         if self.writer is not None:
             self.writer.add_scalar("episode_rewards", episode_rewards, self.episode)
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_a2c.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_a2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rlberry.envs import Wrapper
 from rlberry.agents.torch import A2CAgent
 from rlberry.manager import AgentManager, evaluate_agents
 from rlberry.envs.benchmarks.ball_exploration import PBall2D
-from gym import make
+from gymnasium import make
 
 
 def test_a2c():
     env = "CartPole-v1"
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_dqn.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_mdqn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import pytest
 from rlberry.envs import gym_make
-from rlberry.agents.torch.dqn import DQNAgent
+from rlberry.agents.torch.dqn import MunchausenDQNAgent
 from rlberry.agents.torch.utils.training import model_factory
 
 
-@pytest.mark.parametrize(
-    "use_double_dqn, use_prioritized_replay", [(False, False), (True, True)]
-)
-def test_dqn_agent(use_double_dqn, use_prioritized_replay):
+@pytest.mark.parametrize("use_prioritized_replay", [(False), (True)])
+def test_mdqn_agent(use_prioritized_replay):
     env = gym_make("CartPole-v1")
-    agent = DQNAgent(
+    agent = MunchausenDQNAgent(
         env,
         learning_starts=5,
-        eval_interval=75,
+        batch_size=5,
+        eval_interval=2,
         train_interval=2,
         gradient_steps=-1,
-        use_double_dqn=use_double_dqn,
         use_prioritized_replay=use_prioritized_replay,
     )
-    agent.fit(budget=500)
+    agent.fit(budget=50)
 
     model_configs = {
         "type": "MultiLayerPerceptron",
         "layer_sizes": (5, 5),
         "reshape": False,
     }
 
@@ -30,11 +28,13 @@
         """
         Returns a default Q value network.
         """
         kwargs["in_size"] = env.observation_space.shape[0]
         kwargs["out_size"] = env.action_space.n
         return model_factory(**kwargs)
 
-    new_agent = DQNAgent(
+    new_agent = MunchausenDQNAgent(
         env, q_net_constructor=mlp, q_net_kwargs=model_configs, learning_starts=100
     )
-    new_agent.fit(budget=2000)
+    new_agent.fit(budget=200)
+    observation, info = env.reset()
+    new_agent.policy(observation)
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_factory.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_ppo.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_ppo.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # ppo.fit(4096)
 
 import pytest
 from rlberry.envs import Wrapper
 from rlberry.agents.torch import PPOAgent
 from rlberry.manager import AgentManager, evaluate_agents
 from rlberry.envs.benchmarks.ball_exploration import PBall2D
-from gym import make
+from gymnasium import make
 from rlberry.agents.torch.utils.training import model_factory_from_env
 import sys
 
 
 @pytest.mark.timeout(300)
 @pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 def test_ppo():
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_reinforce.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_reinforce.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_atari.py` & `rlberry-0.5.0/rlberry/envs/tests/test_gym_make.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,122 @@
-from rlberry.manager.agent_manager import AgentManager
-from rlberry.agents.torch.dqn.dqn import DQNAgent
 from rlberry.envs.gym_make import atari_make
 
 
-def test_forward_dqn():
-    mlp_configs = {
-        "type": "MultiLayerPerceptron",  # A network architecture
-        "layer_sizes": [512],  # Network dimensions
-        "reshape": False,
-        "is_policy": False,  # The network should output a distribution
-        # over actions
-    }
-
-    cnn_configs = {
-        "type": "ConvolutionalNetwork",  # A network architecture
-        "activation": "RELU",
-        "in_channels": 4,
-        "in_height": 84,
-        "in_width": 84,
-        "head_mlp_kwargs": mlp_configs,
-        "transpose_obs": False,
-        "is_policy": False,  # The network should output a distribution
-    }
-
-    tuned_agent = AgentManager(
-        DQNAgent,  # The Agent class.
-        (
-            atari_make,
-            # uncomment when rlberry will manage vectorized env
-            # dict(id="ALE/Breakout-v5", n_envs=3),
-            dict(id="ALE/Breakout-v5", n_envs=1),
-        ),  # The Environment to solve.
-        init_kwargs=dict(  # Where to put the agent's hyperparameters
-            q_net_constructor="rlberry.agents.torch.utils.training.model_factory_from_env",
-            q_net_kwargs=cnn_configs,
-            max_replay_size=100,
-            batch_size=32,
-            learning_starts=100,
-            gradient_steps=1,
-            epsilon_final=0.01,
-            learning_rate=1e-4,  # Size of the policy gradient descent steps.
-            chunk_size=5,
-        ),
-        fit_budget=200,  # The number of interactions between the agent and the environment during training.
-        eval_kwargs=dict(
-            eval_horizon=10
-        ),  # The number of interactions between the agent and the environment during evaluations.
-        n_fit=1,  # The number of agents to train. Usually, it is good to do more than 1 because the training is stochastic.
-        agent_name="DQN_test",  # The agent's name.
+def test_atari_make():
+    wrappers_dict = dict(terminal_on_life_loss=True, frame_skip=8)
+    env = atari_make(
+        "ALE/Freeway-v5", render_mode="rgb_array", atari_SB3_wrappers_dict=wrappers_dict
     )
-
-    tuned_agent.fit()
-
-
-def test_forward_empty_input_dim():
-    mlp_configs = {
-        "type": "MultiLayerPerceptron",  # A network architecture
-        "layer_sizes": [512],  # Network dimensions
-        "reshape": False,
-        "is_policy": False,  # The network should output a distribution
-        # over actions
-    }
-
-    cnn_configs = {
-        "type": "ConvolutionalNetwork",  # A network architecture
-        "activation": "RELU",
-        "head_mlp_kwargs": mlp_configs,
-        "transpose_obs": False,
-        "is_policy": False,  # The network should output a distribution
-    }
-
-    tuned_agent = AgentManager(
-        DQNAgent,  # The Agent class.
-        (
-            atari_make,
-            # uncomment when rlberry will manage vectorized env
-            # dict(id="ALE/Breakout-v5", n_envs=3),
-            dict(id="ALE/Breakout-v5", n_envs=1),
-        ),  # The Environment to solve.
-        init_kwargs=dict(  # Where to put the agent's hyperparameters
-            q_net_constructor="rlberry.agents.torch.utils.training.model_factory_from_env",
-            q_net_kwargs=cnn_configs,
-            max_replay_size=100,
-            batch_size=32,
-            learning_starts=100,
-            gradient_steps=1,
-            epsilon_final=0.01,
-            learning_rate=1e-4,  # Size of the policy gradient descent steps.
-            chunk_size=5,
-        ),
-        fit_budget=10,  # The number of interactions between the agent and the environment during training.
-        eval_kwargs=dict(
-            eval_horizon=10
-        ),  # The number of interactions between the agent and the environment during evaluations.
-        n_fit=1,  # The number of agents to train. Usually, it is good to do more than 1 because the training is stochastic.
-        agent_name="DQN_test",  # The agent's name.
+    assert "EpisodicLifeEnv" in str(env)
+    assert "MaxAndSkipEnv" in str(env)
+    assert "ClipRewardEnv" in str(env)
+    assert env.render_mode == "rgb_array"
+
+    wrappers_dict2 = dict(terminal_on_life_loss=False, frame_skip=0)
+    env2 = atari_make(
+        "ALE/Breakout-v5", render_mode="human", atari_SB3_wrappers_dict=wrappers_dict2
     )
+    assert "EpisodicLifeEnv" not in str(env2)
+    assert "MaxAndSkipEnv" not in str(env2)
+    assert "ClipRewardEnv" in str(env2)
+    assert env2.render_mode == "human"
+
+
+def test_rendering_with_atari_make():
+    from rlberry.manager.agent_manager import AgentManager
+    from rlberry.agents.torch import PPOAgent
+    from gymnasium.wrappers.record_video import RecordVideo
+    import os
+    from rlberry.envs.gym_make import atari_make
+    from rlberry.agents.torch.utils.training import model_factory_from_env
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        policy_mlp_configs = {
+            "type": "MultiLayerPerceptron",  # A network architecture
+            "layer_sizes": [16],  # Network dimensions
+            "reshape": False,
+            "is_policy": True,  # The network should output a distribution
+            # over actions
+        }
+
+        critic_mlp_configs = {
+            "type": "MultiLayerPerceptron",
+            "layer_sizes": [16],
+            "reshape": False,
+            "out_size": 1,  # The critic network is an approximator of
+            # a value function V: States -> |R
+        }
+
+        policy_configs = {
+            "type": "ConvolutionalNetwork",  # A network architecture
+            "activation": "RELU",
+            "in_channels": 4,
+            "in_height": 84,
+            "in_width": 84,
+            "head_mlp_kwargs": policy_mlp_configs,
+            "transpose_obs": False,
+            "is_policy": True,  # The network should output a distribution
+        }
+
+        critic_configs = {
+            "type": "ConvolutionalNetwork",
+            "layer_sizes": "RELU",
+            "in_channels": 4,
+            "in_height": 84,
+            "in_width": 84,
+            "head_mlp_kwargs": critic_mlp_configs,
+            "transpose_obs": False,
+            "out_size": 1,
+        }
+
+        tuned_agent = AgentManager(
+            PPOAgent,  # The Agent class.
+            (
+                atari_make,
+                dict(id="ALE/Breakout-v5"),
+            ),  # The Environment to solve.
+            init_kwargs=dict(  # Where to put the agent's hyperparameters
+                batch_size=16,
+                optimizer_type="ADAM",  # What optimizer to use for policy gradient descent steps.
+                learning_rate=2.5e-4,  # Size of the policy gradient descent steps.
+                policy_net_fn=model_factory_from_env,  # A policy network constructor
+                policy_net_kwargs=policy_configs,  # Policy network's architecure
+                value_net_fn=model_factory_from_env,  # A Critic network constructor
+                value_net_kwargs=critic_configs,  # Critic network's architecure.
+                n_envs=8,
+                gamma=0.99,
+                gae_lambda=0.95,
+                clip_eps=0.1,
+                k_epochs=4,
+                n_steps=32,
+            ),
+            fit_budget=1000,  # The number of interactions between the agent and the environment during training.
+            eval_kwargs=dict(
+                eval_horizon=500
+            ),  # The number of interactions between the agent and the environment during evaluations.
+            n_fit=1,  # The number of agents to train. Usually, it is good to do more than 1 because the training is stochastic.
+            agent_name="PPO_tuned",  # The agent's name.
+            output_dir=str(tmpdirname) + "/PPO_for_breakout",
+        )
+
+        tuned_agent.fit()
+
+        env = atari_make("ALE/Breakout-v5", render_mode="rgb_array")
+        env = RecordVideo(env, str(tmpdirname) + "/_video/temp")
+
+        if "render_modes" in env.metadata:
+            env.metadata["render.modes"] = env.metadata[
+                "render_modes"
+            ]  # bug with some 'gym' version
+
+        observation, info = env.reset()
+        for tt in range(3000):
+            action = tuned_agent.get_agent_instances()[0].policy(observation)
+            observation, reward, terminated, truncated, info = env.step(action)
+            done = terminated or truncated
+            if done:
+                break
+
+        env.close()
 
-    tuned_agent.fit()
+        assert os.path.exists(str(tmpdirname) + "/_video/temp/rl-video-episode-0.mp4")
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_models.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_torch_models.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_training.py` & `rlberry-0.5.0/rlberry/agents/torch/tests/test_torch_training.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/torch/utils/models.py` & `rlberry-0.5.0/rlberry/agents/torch/utils/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #
 # Simple MLP and CNN models
 #
 from functools import partial
 
-from gym import spaces
-from gym.vector.sync_vector_env import SyncVectorEnv
+
+from gymnasium import spaces
+from gymnasium.vector.sync_vector_env import SyncVectorEnv
+from gymnasium.vector.async_vector_env import AsyncVectorEnv
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions import Categorical, Normal
 
 from rlberry.agents.torch.utils.training import model_factory, activation_factory
@@ -48,15 +50,17 @@
     return (q1, q2)
 
 
 def default_policy_net_fn(env):
     """
     Returns a default policy network.
     """
-    if type(env) is SyncVectorEnv:
+
+    # remove potential wrappers
+    while type(env) in [SyncVectorEnv, AsyncVectorEnv]:
         env = env.envs[0]
 
     if isinstance(env.observation_space, spaces.Box):
         obs_shape = env.observation_space.shape
     elif isinstance(env.observation_space, spaces.Tuple):
         obs_shape = env.observation_space.spaces[0].shape
     else:
@@ -119,15 +123,16 @@
 
 
 def default_value_net_fn(env):
     """
     Returns a default value network.
     """
 
-    if type(env) is SyncVectorEnv:
+    # remove potential wrappers
+    while type(env) in [SyncVectorEnv, AsyncVectorEnv]:
         env = env.envs[0]
 
     if isinstance(env.observation_space, spaces.Box):
         obs_shape = env.observation_space.shape
     elif isinstance(env.observation_space, spaces.Tuple):
         obs_shape = env.observation_space.spaces[0].shape
     else:
```

### Comparing `rlberry-0.4.1/rlberry/agents/torch/utils/training.py` & `rlberry-0.5.0/rlberry/agents/torch/utils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import torch
-from gym import spaces
+from gymnasium import spaces
 from torch import nn as nn
 from torch.nn import functional as F
 
 
 def loss_function_factory(loss_function, **kwargs):
     if loss_function == "l2":
         return torch.nn.MSELoss(**kwargs)
```

### Comparing `rlberry-0.4.1/rlberry/agents/ucbvi/ucbvi.py` & `rlberry-0.5.0/rlberry/agents/ucbvi/ucbvi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.ucbvi.utils import (
     update_value_and_get_action,
     update_value_and_get_action_sd,
 )
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 from rlberry.agents.dynprog.utils import (
@@ -233,28 +233,31 @@
             self.P_hat[state, action, next_state] += 1.0 / nn
 
             self.B_sa[hh, state, action] = self._compute_bonus(nn, hh)
 
     def _run_episode(self):
         # interact for H steps
         episode_rewards = 0
-        state = self.env.reset()
+        observation, info = self.env.reset()
         for hh in range(self.horizon):
-            action = self._get_action(state, hh)
-            next_state, reward, done, _ = self.env.step(action)
+            action = self._get_action(observation, hh)
+            next_observation, reward, terminated, truncated, info = self.env.step(
+                action
+            )
+            done = terminated or truncated
             episode_rewards += reward  # used for logging only
 
-            self.counter.update(state, action)
+            self.counter.update(observation, action)
 
             if self.reward_free:
                 reward = 0.0  # set to zero before update if reward_free
 
-            self._update(state, action, next_state, reward, hh)
+            self._update(observation, action, next_observation, reward, hh)
 
-            state = next_state
+            observation = next_observation
             if done:
                 break
 
         # run backward induction
         if not self.real_time_dp:
             if self.stage_dependent:
                 backward_induction_sd(
```

### Comparing `rlberry-0.4.1/rlberry/agents/ucbvi/utils.py` & `rlberry-0.5.0/rlberry/agents/ucbvi/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/utils/memories.py` & `rlberry-0.5.0/rlberry/agents/utils/memories.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/agents/utils/replay.py` & `rlberry-0.5.0/rlberry/agents/utils/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,26 +57,27 @@
     >>> buffer.setup_entry("actions", np.uint32)
     >>> buffer.setup_entry("rewards", np.float32)
     >>>
     >>> # Store data in the replay
     >>> env = gym_make("CartPole-v1")
     >>> for _ in range(500):
     >>>     done = False
-    >>>     obs = env.reset()
+    >>>     obs,info = env.reset()
     >>>     while not done:
     >>>         action = env.action_space.sample()
-    >>>         next_obs, reward, done, info = env.step(action)
+    >>>         next_observation, reward, terminated, truncated, info = env.step(action)
+    >>>         done = terminated or truncated
     >>>         buffer.append(
     >>>             {
     >>>                 "observations": obs,
     >>>                 "actions": action,
     >>>                 "rewards": reward
     >>>             }
     >>>         )
-    >>>         obs = next_obs
+    >>>         obs = next_observation
     >>>         if done:
     >>>             buffer.end_episode()
     >>> # Sample a batch of 32 sub-trajectories of length 100.
     >>> # Note: a sub-trajectory may include transitions from more than one episode!
     >>> batch = buffer.sample(batch_size=32, chunk_size=100)
     >>> for tag in buffer.tags:
     >>>     print(tag, batch.data[tag].shape)
```

### Comparing `rlberry-0.4.1/rlberry/agents/utils/replay_utils.py` & `rlberry-0.5.0/rlberry/agents/utils/replay_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/colab_utils/display_setup.py` & `rlberry-0.5.0/rlberry/colab_utils/display_setup.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/bandits/bandit_base.py` & `rlberry-0.5.0/rlberry/envs/bandits/bandit_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import deque
 
+
 from rlberry.envs.interface import Model
 import rlberry.spaces as spaces
-from rlberry.seeding import Seeder
 
 import rlberry
 
 logger = rlberry.logger
 
 
 class Bandit(Model):
@@ -42,49 +42,25 @@
     def step(self, action):
         """
         Sample the reward associated to the action.
         """
         # test that the action exists
         assert action < self.n_arms
 
-        # If the queue of reward for the action is empty, sample 2*size of old reward queue. Otherwise, pop from queue
-        if self.rewards[action]:
-            reward = self.rewards[action].pop()
-        else:
-            self.n_rewards[action] = 2 * self.n_rewards[action]
-            self.rewards[action] = deque(
-                self.laws[action].rvs(
-                    size=self.n_rewards[action], random_state=self.rng
-                )
-            )
-            reward = self.rewards[action].pop()
-
-        done = True
-
-        return 0, reward, done, {}
-
-    def reseed(self, seed_seq=None):
-        if seed_seq is None:
-            self.seeder = self.seeder.spawn()
-        else:
-            self.seeder = Seeder(seed_seq)
-        # spaces
-        self.action_space.reseed(self.seeder.seed_seq)
+        reward = self.laws[action].rvs(random_state=self.rng, size=1)[0]
+        terminated = True
+        truncated = False
 
-        self.rewards = [
-            deque(self.laws[action].rvs(size=10, random_state=self.rng))
-            for action in range(self.n_arms)
-        ]
-        self.n_rewards = [10] * self.n_arms
+        return 0, reward, terminated, truncated, {}
 
-    def reset(self):
+    def reset(self, seed=None, option=None):
         """
         Reset the environment to a default state.
         """
-        return 0
+        return 0, {}
 
 
 class AdversarialBandit(Model):
     """
     Base class for a adversarial multi-armed bandit with oblivious
     opponent, i.e all rewards are fixed in advance at the start of the run.
 
@@ -111,16 +87,16 @@
         Sample the reward associated to the action.
         """
         # test that the action exists
         assert action < self.n_arms
 
         rewards = self.rewards.popleft()
         reward = rewards[action]
-        done = True
-
-        return 0, reward, done, {}
+        terminated = True
+        truncated = False
+        return 0, reward, terminated, truncated, {}
 
-    def reset(self):
+    def reset(self, seed=None, option=None):
         """
         Reset the environment to a default state.
         """
-        return 0
+        return 0, {}
```

### Comparing `rlberry-0.4.1/rlberry/envs/bandits/corrupted_bandits.py` & `rlberry-0.5.0/rlberry/envs/bandits/corrupted_bandits.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/bandits/stochastic_bandits.py` & `rlberry-0.5.0/rlberry/envs/bandits/stochastic_bandits.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/basewrapper.py` & `rlberry-0.5.0/rlberry/envs/basewrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gymnasium as gym
 from rlberry.seeding import Seeder, safe_reseed
 import numpy as np
 from rlberry.envs.interface import Model
 from rlberry.spaces.from_gym import convert_space_from_gym
 
 
 class Wrapper(Model):
@@ -16,27 +17,38 @@
     Parameters
     ----------
     env: gym.Env
         Environment to be wrapped.
     wrap_spaces: bool, default = False
         If True, gym.spaces are converted to rlberry.spaces, which defined a reseed() method.
 
+    Attributes
+    ----------
+    env : gym.Env
+        The wrapped environment
+    metadata : dict
+        InitiallThe meatadata of the wrapped environment
+    render_mode : str
+        The render_mode of the wrapped environment
+
+
     See also:
     https://stackoverflow.com/questions/1443129/completely-wrap-an-object-in-python
 
     [1] https://github.com/openai/gym/blob/master/gym/core.py
     """
 
     def __init__(self, env, wrap_spaces=False):
         # Init base class
         Model.__init__(self)
 
         # Save reference to env
         self.env = env
         self.metadata = self.env.metadata
+        self.render_mode = self.env.render_mode
 
         if wrap_spaces:
             self.observation_space = convert_space_from_gym(self.env.observation_space)
             self.action_space = convert_space_from_gym(self.env.action_space)
         else:
             self.observation_space = self.env.observation_space
             self.action_space = self.env.action_space
@@ -71,41 +83,52 @@
 
     def reseed(self, seed_seq=None):
         # self.seeder
         if seed_seq is None:
             self.seeder = self.seeder.spawn()
         else:
             self.seeder = Seeder(seed_seq)
-        # seed gym.Env that is not a rlberry Model
-        if not isinstance(self.env, Model):
-            # get a seed for gym environment; spaces are reseeded below.
-            safe_reseed(self.env, self.seeder, reseed_spaces=False)
-        # seed rlberry Model
-        else:
+
+        # get a seed for gym environment; spaces are reseeded below.
+        if isinstance(self.env, Model):
+            # seed rlberry Model
             self.env.reseed(self.seeder)
+        elif isinstance(self.env, gym.Env):
+            # seed gym.Env that is not a rlberry Model
+            seed_val = self.seeder.rng.integers(2**32).item()
+            self.env.reset(seed=seed_val)
+        else:
+            # other
+            safe_reseed(self.env, self.seeder, reseed_spaces=False)
+
         safe_reseed(self.observation_space, self.seeder)
         safe_reseed(self.action_space, self.seeder)
 
-    def reset(self):
-        return self.env.reset()
+    def reset(self, seed=None, options=None):
+        if self.env.render_mode == "human":
+            self.render()
+        return self.env.reset(seed=seed, options=options)
 
     def step(self, action):
+        if self.render_mode == "human":
+            self.render()
         return self.env.step(action)
 
     def sample(self, state, action):
         return self.env.sample(state, action)
 
-    def render(self, mode="human", **kwargs):
-        return self.env.render(mode=mode, **kwargs)
+    def render(self, **kwargs):
+        return self.env.render(**kwargs)
 
     def close(self):
         return self.env.close()
 
     def seed(self, seed=None):
-        return self.env.seed(seed)
+        # return self.env.seed(seed)
+        return self.env.reset(seed=seed)
 
     def compute_reward(self, achieved_goal, desired_goal, info):
         return self.env.compute_reward(achieved_goal, desired_goal, info)
 
     def is_online(self):
         try:
             self.env.reset()
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/ball2d.py` & `rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/ball2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/pball.py` & `rlberry-0.5.0/rlberry/envs/benchmarks/ball_exploration/pball.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,24 +163,24 @@
 
         #
         self.name = "Lp-Ball"
 
         # Initalize state
         self.reset()
 
-    def reset(self, state=None):
+    def reset(self, state=None, seed=None, options=None):
         if state is not None:
             self.state = state
         else:
             self.state = self.mu_init + self.sigma_init * self.seeder.rng.normal(
                 size=self.d
             )
             # projection to unit ball
         self.state = projection_to_pball(self.state, self.p)
-        return self.state.copy()
+        return self.state.copy(), {}
 
     def sample(self, state, action):
         assert self.action_space.contains(action)
         assert self.observation_space.contains(state)
 
         # next state
         action_vec = self.action_list[action]
@@ -188,23 +188,24 @@
             self.A.dot(state)
             + self.B.dot(action_vec)
             + self.sigma * self.rng.normal(size=self.d)
         )
         next_s = projection_to_pball(next_s, self.p)
 
         # done and reward
-        done = False
+        terminated = False
+        truncated = False
         reward = self.compute_reward_at(state)
 
-        return next_s, reward, done, {}
+        return next_s, reward, terminated, truncated, {}
 
     def step(self, action):
-        next_s, reward, done, info = self.sample(self.state, action)
+        next_s, reward, terminated, truncated, info = self.sample(self.state, action)
         self.state = next_s.copy()
-        return next_s, reward, done, info
+        return next_s, reward, terminated, truncated, info
 
     def compute_reward_at(self, x):
         reward = 0.0
         for ii, b_ii in enumerate(self.reward_amplitudes):
             c_ii = self.reward_smoothness[ii]
             x_ii = self.reward_centers[ii]
             dist = np.linalg.norm(x - x_ii, ord=self.p)
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/generalization/twinrooms.py` & `rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_twinrooms.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from rlberry.rendering.common_shapes import circle_shape
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class TwinRooms(RenderInterface2D, Model):
+class Old_TwinRooms(RenderInterface2D, Model):
     """
+    'Old' because it's a pre-gymnasium version (like gym=0.21)
+        - step with 'done' instead of 'terminated' and 'truncated'
+        - reset with 'observation' only, instead of 'observation' and 'info'
+
     Two continuous grid worlds, side by side, separated by a wall.
     Both are identical (or almost identical), and the agent has equal probability to
     start in any of the two rooms.
 
     It can be used to test the generalization capability of agents:
     a policy learned in one of the rooms can be used to learn faster
     a policy in the other room.
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/apple_gold.py` & `rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/apple_gold.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,37 +102,42 @@
         xx = xx + 0.5
         yy = yy + 0.5
         # map to [0, 1]
         xx = xx / self.ncols
         yy = yy / self.nrows
         return np.array([xx, yy])
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         self.state = self.coord2index[self.start_coord]
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
-        return state_to_return
+        if self.render_mode == "human":
+            self.render()
+        return state_to_return, {}
 
     def step(self, action):
         assert self.action_space.contains(action), "Invalid action!"
 
         # save state for rendering
         if self.is_render_enabled():
             self.append_state_for_rendering(self.state)
 
         # take step
-        next_state, reward, done, info = self.sample(self.state, action)
+        next_state, reward, terminated, truncated, info = self.sample(
+            self.state, action
+        )
         self.state = next_state
 
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
-
-        return state_to_return, reward, done, info
+        if self.render_mode == "human":
+            self.render()
+        return state_to_return, reward, terminated, truncated, info
 
     def get_background(self):
         """
         Returne a scene (list of shapes) representing the background
         """
         bg = Scene()
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/four_room.py` & `rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_four_room.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import numpy as np
 import rlberry.spaces as spaces
-from rlberry.envs.finite import GridWorld
+from rlberry.wrappers.tests.old_env.old_gridworld import Old_GridWorld
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class FourRoom(GridWorld):
+class Old_FourRoom(Old_GridWorld):
     """
+    'Old' because it's a pre-gymnasium version (like gym=0.21)
+        - step with 'done' instead of 'terminated' and 'truncated'
+        - reset with 'observation' only, instead of 'observation' and 'info'
+
     GridWorld with four rooms.
 
     Parameters
     ----------
     reward_free : bool, default=False
         If true, no rewards are given to the agent.
     difficulty: int, {0, 1 or 2}
@@ -72,15 +76,15 @@
             elif difficulty in [1, 2]:
                 reward_at = {
                     (8, 0): 1.0,
                     (3, 3): 0.1,
                 }
 
         # Init base class
-        GridWorld.__init__(
+        Old_GridWorld.__init__(
             self,
             nrows=nrows,
             ncols=ncols,
             start_coord=start_coord,
             terminal_states=terminal_states,
             success_probability=success_probability,
             reward_at=reward_at,
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/nroom.py` & `rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/nroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,37 +227,39 @@
         xx = xx + 0.5
         yy = yy + 0.5
         # map to [0, 1]
         xx = xx / self.ncols
         yy = yy / self.nrows
         return np.array([xx, yy])
 
-    def reset(self):
-        self.state = GridWorld.reset(self)
+    def reset(self, seed=None, options=None):
+        self.state, info = GridWorld.reset(self, seed=seed, options=options)
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
-        return state_to_return
+        return state_to_return, info
 
     def step(self, action):
         assert self.action_space.contains(action), "Invalid action!"
 
         # save state for rendering
         if self.is_render_enabled():
             self.append_state_for_rendering(self.state)
 
         # take step
-        next_state, reward, done, info = self.sample(self.state, action)
+        next_state, reward, terminated, truncated, info = self.sample(
+            self.state, action
+        )
         self.state = next_state
 
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
 
-        return state_to_return, reward, done, info
+        return state_to_return, reward, terminated, truncated, info
 
     def get_background(self):
         """
         Returne a scene (list of shapes) representing the background
         """
         bg = Scene()
```

### Comparing `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/six_room.py` & `rlberry-0.5.0/rlberry/envs/benchmarks/grid_exploration/six_room.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,37 +85,39 @@
         xx = xx + 0.5
         yy = yy + 0.5
         # map to [0, 1]
         xx = xx / self.ncols
         yy = yy / self.nrows
         return np.array([xx, yy])
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         self.state = self.coord2index[self.start_coord]
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
-        return state_to_return
+        return state_to_return, {}
 
     def step(self, action):
         assert self.action_space.contains(action), "Invalid action!"
 
         # save state for rendering
         if self.is_render_enabled():
             self.append_state_for_rendering(self.state)
 
         # take step
-        next_state, reward, done, info = self.sample(self.state, action)
+        next_state, reward, terminated, truncated, info = self.sample(
+            self.state, action
+        )
         self.state = next_state
 
         state_to_return = self.state
         if self.array_observation:
             state_to_return = self._convert_index_to_float_coord(self.state)
 
-        return state_to_return, reward, done, info
+        return state_to_return, reward, terminated, truncated, info
 
     def get_background(self):
         """
         Returne a scene (list of shapes) representing the background
         """
         bg = Scene()
```

### Comparing `rlberry-0.4.1/rlberry/envs/classic_control/SpringCartPole.py` & `rlberry-0.5.0/rlberry/envs/classic_control/SpringCartPole.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             rand_state[2] += np.pi
             rand_state[6] += np.pi
         if self.obs_trans:
             self.state = self.transform_states(rand_state)
         else:
             self.state = rand_state
         self.state_ = rand_state
-        return self.state
+        return self.state, {}
 
     def _reward(self):
         state = self.state
         if state.shape[-1] == 10:
             (
                 _,
                 _,
@@ -283,17 +283,18 @@
 
         ns = self.bound_states(ns)
         self.state_ = ns
         if self.obs_trans:
             self.state = self.transform_states(ns)
         else:
             self.state = ns
-        terminal = self._terminal()
+        terminated = self._terminal()
+        truncated = False
         reward = self._reward()[0]
-        return self.state, reward, terminal, {}
+        return self.state, reward, terminated, truncated, {}
 
     def _terminal(self):
         s = self.state_
         x1 = s[0]
         x2 = s[4]
         bad_condition = False
         bad_condition += np.abs(x1) > self.L
```

### Comparing `rlberry-0.4.1/rlberry/envs/classic_control/acrobot.py` & `rlberry-0.5.0/rlberry/envs/classic_control/acrobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,17 @@
         self.observation_space = spaces.Box(low=low, high=high)
         self.action_space = spaces.Discrete(3)
 
         # initialize
         self.state = None
         self.reset()
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         self.state = self.rng.uniform(low=-0.1, high=0.1, size=(4,))
-        return self._get_ob()
+        return self._get_ob(), {}
 
     def step(self, action):
         assert self.action_space.contains(action), "%r (%s) invalid" % (
             action,
             type(action),
         )
 
@@ -160,17 +160,18 @@
         # at the ''final timestep'', self.dt
 
         ns[0] = wrap(ns[0], -np.pi, np.pi)
         ns[1] = wrap(ns[1], -np.pi, np.pi)
         ns[2] = bound(ns[2], -self.MAX_VEL_1, self.MAX_VEL_1)
         ns[3] = bound(ns[3], -self.MAX_VEL_2, self.MAX_VEL_2)
         self.state = ns
-        terminal = self._terminal()
-        reward = -1.0 if not terminal else 0.0
-        return self._get_ob(), reward, terminal, {}
+        terminated = self._terminal()
+        truncated = False
+        reward = -1.0 if not terminated else 0.0
+        return self._get_ob(), reward, terminated, truncated, {}
 
     def _get_ob(self):
         s = self.state
         return np.array(
             [np.cos(s[0]), np.sin(s[0]), np.cos(s[1]), np.sin(s[1]), s[2], s[3]]
         )
```

### Comparing `rlberry-0.4.1/rlberry/envs/classic_control/mountain_car.py` & `rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_mountain_car.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 import numpy as np
 
 import rlberry.spaces as spaces
 from rlberry.envs.interface import Model
 from rlberry.rendering import Scene, GeometricPrimitive, RenderInterface2D
 
 
-class MountainCar(RenderInterface2D, Model):
+class Old_MountainCar(RenderInterface2D, Model):
     """
+    'Old' because it's a pre-gymnasium version (like gym=0.21)
+        - step with 'done' instead of 'terminated' and 'truncated'
+        - reset with 'observation' only, instead of 'observation' and 'info'
+
     The agent (a car) is started at the bottom of a valley. For any given
     state the agent may choose to accelerate to the left, right or cease
     any acceleration.
 
     Notes
     -----
     Source:
```

### Comparing `rlberry-0.4.1/rlberry/envs/classic_control/pendulum.py` & `rlberry-0.5.0/rlberry/envs/classic_control/pendulum.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,20 @@
             low=-self.max_torque, high=self.max_torque, shape=(1,)
         )
         self.observation_space = spaces.Box(low=low, high=high)
 
         # initialize
         self.reset()
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         high = np.array([np.pi, 1])
         low = -high
         self.state = self.rng.uniform(low=low, high=high)
         self.last_action = None
-        return self._get_ob()
+        return self._get_ob(), {}
 
     def step(self, action):
         assert self.action_space.contains(action), "%r (%s) invalid" % (
             action,
             type(action),
         )
 
@@ -91,15 +91,15 @@
             )
             * dt
         )
         newtheta = theta + newthetadot * dt
         newthetadot = np.clip(newthetadot, -self.max_speed, self.max_speed)
 
         self.state = np.array([newtheta, newthetadot])
-        return self._get_ob(), -costs, False, {}
+        return self._get_ob(), -costs, False, False, {}
 
     def _get_ob(self):
         theta, thetadot = self.state
         return np.array([np.cos(theta), np.sin(theta), thetadot])
 
     #
     # Below code for rendering
```

### Comparing `rlberry-0.4.1/rlberry/envs/finite/chain.py` & `rlberry-0.5.0/rlberry/envs/finite/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,20 @@
         assert action in self._actions, "Invalid action!"
 
         # save state for rendering
         if self.is_render_enabled():
             self.append_state_for_rendering(self.state)
 
         # take step
-        next_state, reward, done, info = self.sample(self.state, action)
+        next_state, reward, terminated, truncated, info = self.sample(
+            self.state, action
+        )
 
         self.state = next_state
-        return next_state, reward, done, info
+        return next_state, reward, terminated, truncated, info
 
     #
     # Code for rendering
     #
 
     def get_background(self):
         """
```

### Comparing `rlberry-0.4.1/rlberry/envs/finite/finite_mdp.py` & `rlberry-0.5.0/rlberry/wrappers/tests/old_env/old_finite_mdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from rlberry.envs.interface import Model
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class FiniteMDP(Model):
+class Old_FiniteMDP(Model):
     """
+    'Old' because it's a pre-gymnasium version (like gym=0.21)
+        - step with 'done' instead of 'terminated' and 'truncated'
+        - reset with 'observation' only, instead of 'observation' and 'info'
+
     Base class for a finite MDP.
 
     Terminal states are set to be absorbing, and
     are determined by the is_terminal() method,
     which can be overriden (and returns false by default).
 
     Parameters
```

### Comparing `rlberry-0.4.1/rlberry/envs/finite/gridworld.py` & `rlberry-0.5.0/rlberry/envs/finite/gridworld.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,17 +346,19 @@
         assert self.action_space.contains(action), "Invalid action!"
 
         # save state for rendering
         if self.is_render_enabled():
             self.append_state_for_rendering(self.state)
 
         # take step
-        next_state, reward, done, info = self.sample(self.state, action)
+        next_state, reward, terminated, truncated, info = self.sample(
+            self.state, action
+        )
         self.state = next_state
-        return next_state, reward, done, info
+        return next_state, reward, terminated, truncated, info
 
     #
     # Code for rendering
     #
     def get_layout_array(self, state_data=None, fill_walls_with=np.nan):
         """
         Returns an array 'layout' of shape (nrows, ncols) such that:
```

### Comparing `rlberry-0.4.1/rlberry/envs/finite/gridworld_utils.py` & `rlberry-0.5.0/rlberry/envs/finite/gridworld_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/interface/model.py` & `rlberry-0.5.0/rlberry/envs/interface/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import numpy as np
 
 import inspect
 from rlberry.seeding import Seeder
 
 import rlberry
```

### Comparing `rlberry-0.4.1/rlberry/envs/pipeline.py` & `rlberry-0.5.0/rlberry/envs/pipeline.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/tests/test_bandits.py` & `rlberry-0.5.0/rlberry/envs/tests/test_bandits.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/envs/tests/test_env_seeding.py` & `rlberry-0.5.0/rlberry/envs/tests/test_env_seeding.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     SixRoom,
     AppleGold,
 ]
 
 
 def get_env_trajectory(env, horizon):
     states = []
-    ss = env.reset()
+    ss, info = env.reset()
     for ii in range(horizon):
         states.append(ss)
-        ss, _, _, _ = env.step(env.action_space.sample())
+        ss, _, _, _, _ = env.step(env.action_space.sample())
     return states
 
 
 def compare_trajectories(traj1, traj2):
     """
     returns true if trajectories are equal
     """
```

### Comparing `rlberry-0.4.1/rlberry/envs/tests/test_gym_env_seeding.py` & `rlberry-0.5.0/rlberry/envs/tests/test_gym_env_seeding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from rlberry.seeding.seeding import safe_reseed
-import gym
+import gymnasium as gym
 import numpy as np
 import pytest
 from rlberry.seeding import Seeder
 from rlberry.envs import gym_make
 
 from copy import deepcopy
 
@@ -12,20 +12,21 @@
     "CartPole-v1",
     "MountainCar-v0",
 ]
 
 
 def get_env_trajectory(env, horizon):
     states = []
-    ss = env.reset()
+    observation, info = env.reset()
     for ii in range(horizon):
-        states.append(ss)
-        ss, _, done, _ = env.step(env.action_space.sample())
+        states.append(observation)
+        observation, _, terminated, truncated, _ = env.step(env.action_space.sample())
+        done = terminated or truncated
         if done:
-            ss = env.reset()
+            observation, info = env.reset()
     return states
 
 
 def compare_trajectories(traj1, traj2):
     for ss1, ss2 in zip(traj1, traj2):
         if not np.array_equal(ss1, ss2):
             return False
```

### Comparing `rlberry-0.4.1/rlberry/envs/tests/test_instantiation.py` & `rlberry-0.5.0/rlberry/envs/tests/test_instantiation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 
 @pytest.mark.parametrize("ModelClass", classes)
 def test_instantiation(ModelClass):
     env = ModelClass()
 
     if env.is_online():
         for _ in range(2):
-            state = env.reset()
+            state, info = env.reset()
             for _ in range(50):
                 assert env.observation_space.contains(state)
                 action = env.action_space.sample()
-                next_s, _, _, _ = env.step(action)
+                next_s, _, _, _, _ = env.step(action)
                 state = next_s
 
     if env.is_generative():
         for _ in range(100):
             state = env.observation_space.sample()
             action = env.action_space.sample()
-            next_s, _, _, _ = env.sample(state, action)
+            next_s, _, _, _, _ = env.sample(state, action)
             assert env.observation_space.contains(next_s)
 
 
 @pytest.mark.parametrize("ModelClass", classes)
 def test_rendering_calls(ModelClass):
     env = ModelClass()
     if isinstance(env, RenderInterface2D):
@@ -117,16 +117,16 @@
 def test_four_room(reward_free, difficulty, array_observation):
     env = FourRoom(
         reward_free=reward_free,
         difficulty=difficulty,
         array_observation=array_observation,
     )
 
-    initial_state = env.reset()
-    next_state, reward, _, _ = env.step(1)
+    initial_state, info = env.reset()
+    next_state, reward, _, _, _ = env.step(1)
 
     assert env.observation_space.contains(initial_state)
     assert env.observation_space.contains(next_state)
 
     if reward_free:
         assert env.reward_at == {}
 
@@ -146,16 +146,16 @@
         (True, False),
         (True, True),
     ],
 )
 def test_six_room(reward_free, array_observation):
     env = SixRoom(reward_free=reward_free, array_observation=array_observation)
 
-    initial_state = env.reset()
-    next_state, reward, _, _ = env.step(1)
+    initial_state, info = env.reset()
+    next_state, reward, _, _, _ = env.step(1)
 
     assert env.observation_space.contains(initial_state)
     assert env.observation_space.contains(next_state)
 
     if reward_free:
         assert env.reward_at == {}
 
@@ -172,16 +172,16 @@
         (True, False),
         (True, True),
     ],
 )
 def test_apple_gold(reward_free, array_observation):
     env = AppleGold(reward_free=reward_free, array_observation=array_observation)
 
-    initial_state = env.reset()
-    next_state, reward, _, _ = env.step(1)
+    initial_state, info = env.reset()
+    next_state, reward, _, _, _ = env.step(1)
     assert env.observation_space.contains(initial_state)
     assert env.observation_space.contains(next_state)
 
     if reward_free:
         assert env.reward_at == {}
 
     if array_observation:
@@ -202,16 +202,16 @@
 def test_n_room(reward_free, array_observation, initial_state_distribution):
     env = NRoom(
         reward_free=reward_free,
         array_observation=array_observation,
         initial_state_distribution=initial_state_distribution,
     )
 
-    initial_state = env.reset()
-    next_state, reward, _, _ = env.step(1)
+    initial_state, info = env.reset()
+    next_state, reward, _, _, _ = env.step(1)
 
     if initial_state_distribution == "uniform":
         assert env.initial_state_distribution[0] == 1.0 / env.observation_space.n
 
     assert env.observation_space.contains(initial_state)
     assert env.observation_space.contains(next_state)
 
@@ -229,15 +229,15 @@
 
     env_ctor, env_kwargs = PipelineEnv, {
         "env_ctor": gym_make,
         "env_kwargs": {"id": "Acrobot-v1"},
         "wrappers": [(RescaleRewardWrapper, {"reward_range": (0, 1)})],
     }
     env = env_ctor(**env_kwargs)
-    _, reward, _, _ = env.step(0)
+    _, reward, _, _, _ = env.step(0)
     assert (reward <= 1) and (reward >= 0)
 
     env_ctor, env_kwargs = PipelineEnv, {
         "env_ctor": gym_make,
         "env_kwargs": {"id": "Acrobot-v1"},
         "wrappers": [
             (RescaleRewardWrapper, {"reward_range": (0, 1)}),
```

### Comparing `rlberry-0.4.1/rlberry/envs/utils.py` & `rlberry-0.5.0/rlberry/envs/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     else:
         if env is None:
             return None
         if copy_env:
             try:
                 processed_env = deepcopy(env)
             except Exception as ex:
-                logger.warning("[Agent] Not possible to deepcopy env: " + str(ex))
+                raise RuntimeError("[Agent] Not possible to deepcopy env: " + str(ex))
         else:
             processed_env = env
     reseeded = safe_reseed(processed_env, seeder)
     if not reseeded:
         logger.warning("[Agent] Not possible to reseed environment.")
     return processed_env
```

### Comparing `rlberry-0.4.1/rlberry/experiment/generator.py` & `rlberry-0.5.0/rlberry/experiment/generator.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/experiment/load_results.py` & `rlberry-0.5.0/rlberry/experiment/load_results.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/experiment/yaml_utils.py` & `rlberry-0.5.0/rlberry/experiment/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/discrete_counter.py` & `rlberry-0.5.0/rlberry/exploration_tools/discrete_counter.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/online_discretization_counter.py` & `rlberry-0.5.0/rlberry/exploration_tools/online_discretization_counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from rlberry.utils.jit_setup import numba_jit
 from rlberry.exploration_tools.uncertainty_estimator import UncertaintyEstimator
 from rlberry.exploration_tools.typing import preprocess_args
-from gym.spaces import Box, Discrete
+from gymnasium.spaces import Box, Discrete
 from rlberry.utils.metrics import metric_lp
 
 import rlberry
 
 logger = rlberry.logger
```

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/tests/test_discrete_counter.py` & `rlberry-0.5.0/rlberry/exploration_tools/tests/test_discrete_counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     for N in range(10, 20):
         assert counter.get_n_visited_states() == 0
         assert counter.get_entropy() == 0.0
 
         for ss in range(env.observation_space.n):
             for aa in range(env.action_space.n):
                 for _ in range(N):
-                    ns, rr, _, _ = env.sample(ss, aa)
+                    ns, rr, _, _, _ = env.sample(ss, aa)
                     counter.update(ss, aa, ns, rr)
                 assert counter.N_sa[ss, aa] == N
                 assert counter.count(ss, aa) == N
                 if rate_power == pytest.approx(1):
                     assert np.allclose(counter.measure(ss, aa), 1.0 / N)
                 elif rate_power == pytest.approx(0.5):
                     assert np.allclose(counter.measure(ss, aa), np.sqrt(1.0 / N))
@@ -46,15 +46,15 @@
     )
 
     for N in [10, 20]:
         for _ in range(10):
             ss = env.observation_space.sample()
             aa = env.action_space.sample()
             for _ in range(N):
-                ns, rr, _, _ = env.sample(ss, aa)
+                ns, rr, _, _, _ = env.sample(ss, aa)
                 counter.update(ss, aa, ns, rr)
 
             dss = counter.state_discretizer.discretize(ss)
             assert counter.N_sa[dss, aa] == N
             assert counter.count(ss, aa) == N
             if rate_power == pytest.approx(1):
                 assert np.allclose(counter.measure(ss, aa), 1.0 / N)
@@ -71,15 +71,15 @@
     )
 
     for N in [10, 20]:
         for _ in range(10):
             ss = env.observation_space.sample()
             aa = env.action_space.sample()
             for nn in range(N):
-                ns, rr, _, _ = env.sample(ss, aa)
+                ns, rr, _, _, _ = env.sample(ss, aa)
                 counter.update(ss, aa, ns, rr)
             assert counter.count(ss, aa) == N
             if rate_power == pytest.approx(1):
                 assert np.allclose(counter.measure(ss, aa), 1.0 / N)
             elif rate_power == pytest.approx(0.5):
                 assert np.allclose(counter.measure(ss, aa), np.sqrt(1.0 / N))
             counter.reset()
@@ -94,15 +94,15 @@
     for N in range(10, 20, 3):
         assert counter.get_n_visited_states() == 0
         assert counter.get_entropy() == 0.0
 
         for ss in range(env.discrete_observation_space.n):
             for aa in range(env.action_space.n):
                 for _ in range(N):
-                    ns, rr, _, _ = env.sample(ss, aa)
+                    ns, rr, _, _, _ = env.sample(ss, aa)
                     continuous_ss = env._convert_index_to_float_coord(ss)
                     counter.update(continuous_ss, aa, None, rr)
                 assert counter.N_sa[ss, aa] == N
                 assert counter.count(continuous_ss, aa) == N
                 assert np.allclose(counter.measure(continuous_ss, aa), np.sqrt(1.0 / N))
 
         assert counter.get_n_visited_states() == env.discrete_observation_space.n
```

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/torch/rnd.py` & `rlberry-0.5.0/rlberry/exploration_tools/torch/rnd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import partial
 
 import torch
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 from torch.nn import functional as F
 
 from rlberry.agents.utils.memories import ReplayMemory
 from rlberry.exploration_tools.uncertainty_estimator import UncertaintyEstimator
 from rlberry.exploration_tools.typing import preprocess_args
 from rlberry.agents.torch.utils.models import ConvolutionalNetwork
 from rlberry.agents.torch.utils.models import MultiLayerPerceptron
```

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/torch/tests/test_rnd.py` & `rlberry-0.5.0/rlberry/exploration_tools/torch/tests/test_rnd.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         env.action_space,
         learning_rate=0.1,
         update_period=100,
         embedding_dim=2,
     )
 
     # Test
-    state = env.reset()
+    observation, info = env.reset()
     for ii in range(1000):
         action = env.action_space.sample()
-        next_s, reward, _, _ = env.step(action)
-        rnd.update(state, action, next_s, reward)
-        state = next_s
+        next_observation, reward, terminated, truncated, info = env.step(action)
+        done = terminated or truncated
+        rnd.update(observation, action, next_observation, reward)
+        observation = next_observation
         # measure uncertainty
-        _ = rnd.measure(state, action)
+        _ = rnd.measure(observation, action)
```

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/typing.py` & `rlberry-0.5.0/rlberry/exploration_tools/typing.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/exploration_tools/uncertainty_estimator.py` & `rlberry-0.5.0/rlberry/exploration_tools/uncertainty_estimator.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/agent_manager.py` & `rlberry-0.5.0/rlberry/manager/agent_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,26 +837,31 @@
         Returns
         -------
         :class:`rlberry.manager.AgentManager`
             Loaded instance of AgentManager.
         """
         filename = Path(filename).with_suffix(".pickle")
 
+        if filename.name != "manager_obj.pickle":
+            raise ValueError(
+                "The agent_manager objects should be save in file named 'manager_obj.pickle'"
+            )
+
         obj = cls(None, None, None)
 
         compress_pickle = is_bz_file(filename)
 
         try:
             if not compress_pickle:
                 with filename.open("rb") as ff:
                     tmp_dict = pickle.load(ff)
             else:
                 with bz2.BZ2File(filename, "rb") as ff:
                     tmp_dict = cPickle.load(ff)
-        except Exception:
+        except Exception as ex:
             if not compress_pickle:
                 with filename.open("rb") as ff:
                     tmp_dict = dill.load(ff)
             else:
                 with bz2.BZ2File(filename, "rb") as ff:
                     tmp_dict = dill.load(ff)
```

### Comparing `rlberry-0.4.1/rlberry/manager/evaluation.py` & `rlberry-0.5.0/rlberry/manager/evaluation.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/multiple_managers.py` & `rlberry-0.5.0/rlberry/manager/multiple_managers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/remote_agent_manager.py` & `rlberry-0.5.0/rlberry/manager/remote_agent_manager.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/tests/test_agent_manager.py` & `rlberry-0.5.0/rlberry/manager/tests/test_agent_manager.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/tests/test_agent_manager_seeding.py` & `rlberry-0.5.0/rlberry/manager/tests/test_agent_manager_seeding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from rlberry.envs.tests.test_env_seeding import get_env_trajectory, compare_trajectories
 from rlberry.envs import gym_make
 from rlberry.envs.classic_control import MountainCar
 from rlberry.manager import AgentManager, MultipleManagers
 from rlberry.agents.torch import A2CAgent
-import gym
+import gymnasium as gym
 import pytest
 
 
 @pytest.mark.parametrize(
     "env, agent_class",
     [
         ((MountainCar, {}), A2CAgent),
         ((gym_make, {"id": "MountainCar-v0"}), A2CAgent),
-        ((gym.make, {"id": "MountainCar-v0"}), A2CAgent),
+        (
+            (gym.make, {"id": "MountainCar-v0"}),
+            A2CAgent,
+        ),
     ],
 )
 def test_agent_manager_and_multiple_managers_seeding(env, agent_class):
     agent_manager = AgentManager(
         agent_class, env, fit_budget=2, init_kwargs={}, n_fit=6, seed=3456
     )
     agent_manager_test = AgentManager(
```

### Comparing `rlberry-0.4.1/rlberry/manager/tests/test_hyperparam_optim.py` & `rlberry-0.5.0/rlberry/manager/tests/test_hyperparam_optim.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/tests/test_plot.py` & `rlberry-0.5.0/rlberry/manager/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/manager/tests/test_shared_data.py` & `rlberry-0.5.0/rlberry/manager/tests/test_shared_data.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/metadata_utils.py` & `rlberry-0.5.0/rlberry/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/client.py` & `rlberry-0.5.0/rlberry/network/client.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/interface.py` & `rlberry-0.5.0/rlberry/network/interface.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/server.py` & `rlberry-0.5.0/rlberry/network/server.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/server_utils.py` & `rlberry-0.5.0/rlberry/network/server_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/tests/conftest.py` & `rlberry-0.5.0/rlberry/network/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/tests/test_server.py` & `rlberry-0.5.0/rlberry/network/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/network/utils.py` & `rlberry-0.5.0/rlberry/network/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/common_shapes.py` & `rlberry-0.5.0/rlberry/rendering/common_shapes.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/core.py` & `rlberry-0.5.0/rlberry/rendering/core.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/opengl_render2d.py` & `rlberry-0.5.0/rlberry/rendering/opengl_render2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/pygame_render2d.py` & `rlberry-0.5.0/rlberry/rendering/pygame_render2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/render_interface.py` & `rlberry-0.5.0/rlberry/rendering/render_interface.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/rendering/utils.py` & `rlberry-0.5.0/rlberry/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/seeding/seeder.py` & `rlberry-0.5.0/rlberry/seeding/seeder.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/seeding/seeding.py` & `rlberry-0.5.0/rlberry/seeding/seeding.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,19 @@
         reseeded = True
     except AttributeError:
         seed_val = seeder.rng.integers(2**32).item()
         try:
             obj.seed(seed_val)
             reseeded = True
         except AttributeError:
-            reseeded = False
+            try:
+                obj.reset(seed=seed_val)
+                reseeded = True
+            except AttributeError:
+                reseeded = False
 
     # check if the object has observation and action spaces to be reseeded.
     if reseed_spaces:
         try:
             safe_reseed(obj.observation_space, seeder)
             safe_reseed(obj.action_space, seeder)
         except AttributeError:
```

### Comparing `rlberry-0.4.1/rlberry/seeding/tests/test_seeding.py` & `rlberry-0.5.0/rlberry/seeding/tests/test_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/seeding/tests/test_threads.py` & `rlberry-0.5.0/rlberry/seeding/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/seeding/tests/test_threads_torch.py` & `rlberry-0.5.0/rlberry/seeding/tests/test_threads_torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/spaces/box.py` & `rlberry-0.5.0/rlberry/spaces/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import gym
+import gymnasium as gym
 import numpy as np
 from rlberry.seeding import Seeder
 
 
 class Box(gym.spaces.Box):
     """
     Class that represents a space that is a cartesian product in R^n:
 
     [a_1, b_1] x [a_2, b_2] x ... x [a_n, b_n]
 
 
-    Inherited from gym.spaces.Box for compatibility with gym.
+    Inherited from gymnasium.spaces.Box for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
```

### Comparing `rlberry-0.4.1/rlberry/spaces/dict.py` & `rlberry-0.5.0/rlberry/spaces/tuple.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import gym
+import gymnasium as gym
 from rlberry.seeding import Seeder
 
 
-class Dict(gym.spaces.Dict):
+class Tuple(gym.spaces.Tuple):
     """
 
-    Inherited from gym.spaces.Dict for compatibility with gym.
+    Inherited from gymnasium.spaces.Tuple for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
@@ -17,17 +17,17 @@
 
     Methods
     -------
     reseed()
         get new random number generator
     """
 
-    def __init__(self, spaces=None, **spaces_kwargs):
-        gym.spaces.Dict.__init__(self, spaces, **spaces_kwargs)
+    def __init__(self, spaces):
+        gym.spaces.Tuple.__init__(self, spaces)
         self.seeder = Seeder()
 
     @property
     def rng(self):
         return self.seeder.rng
 
     def reseed(self, seed_seq=None):
-        _ = [space.reseed(seed_seq) for space in self.spaces.values()]
+        _ = [space.reseed(seed_seq) for space in self.spaces]
```

### Comparing `rlberry-0.4.1/rlberry/spaces/discrete.py` & `rlberry-0.5.0/rlberry/spaces/discrete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import gym
+import gymnasium as gym
 from rlberry.seeding import Seeder
 
 
 class Discrete(gym.spaces.Discrete):
     """
     Class that represents discrete spaces.
 
 
-    Inherited from gym.spaces.Discrete for compatibility with gym.
+    Inherited from gymnasium.spaces.Discrete for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
```

### Comparing `rlberry-0.4.1/rlberry/spaces/from_gym.py` & `rlberry-0.5.0/rlberry/spaces/from_gym.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import rlberry.spaces
-import gym.spaces
+import gymnasium.spaces
 
 
 def convert_space_from_gym(space):
-    if isinstance(space, gym.spaces.Box) and (
+    if isinstance(space, gymnasium.spaces.Box) and (
         not isinstance(space, rlberry.spaces.Box)
     ):
         return rlberry.spaces.Box(
             space.low, space.high, shape=space.shape, dtype=space.dtype
         )
-    if isinstance(space, gym.spaces.Discrete) and (
+    if isinstance(space, gymnasium.spaces.Discrete) and (
         not isinstance(space, rlberry.spaces.Discrete)
     ):
         return rlberry.spaces.Discrete(n=space.n)
-    if isinstance(space, gym.spaces.MultiBinary) and (
+    if isinstance(space, gymnasium.spaces.MultiBinary) and (
         not isinstance(space, rlberry.spaces.MultiBinary)
     ):
         return rlberry.spaces.MultiBinary(n=space.n)
-    if isinstance(space, gym.spaces.MultiDiscrete) and (
+    if isinstance(space, gymnasium.spaces.MultiDiscrete) and (
         not isinstance(space, rlberry.spaces.MultiDiscrete)
     ):
         return rlberry.spaces.MultiDiscrete(
             nvec=space.nvec,
             dtype=space.dtype,
         )
-    if isinstance(space, gym.spaces.Tuple) and (
+    if isinstance(space, gymnasium.spaces.Tuple) and (
         not isinstance(space, rlberry.spaces.Tuple)
     ):
         return rlberry.spaces.Tuple(
             spaces=[convert_space_from_gym(sp) for sp in space.spaces]
         )
-    if isinstance(space, gym.spaces.Dict) and (
+    if isinstance(space, gymnasium.spaces.Dict) and (
         not isinstance(space, rlberry.spaces.Dict)
     ):
         converted_spaces = dict()
         for key in space.spaces:
             converted_spaces[key] = convert_space_from_gym(space.spaces[key])
         return rlberry.spaces.Dict(spaces=converted_spaces)
```

### Comparing `rlberry-0.4.1/rlberry/spaces/multi_binary.py` & `rlberry-0.5.0/rlberry/spaces/multi_binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import gym
+import gymnasium as gym
 from rlberry.seeding import Seeder
 
 
 class MultiBinary(gym.spaces.MultiBinary):
     """
 
-    Inherited from gym.spaces.MultiBinary for compatibility with gym.
+    Inherited from gymnasium.spaces.MultiBinary for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
```

### Comparing `rlberry-0.4.1/rlberry/spaces/multi_discrete.py` & `rlberry-0.5.0/rlberry/spaces/multi_discrete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import gym
+import gymnasium as gym
 import numpy as np
 from rlberry.seeding import Seeder
 
 
 class MultiDiscrete(gym.spaces.MultiDiscrete):
     """
 
-    Inherited from gym.spaces.MultiDiscrete for compatibility with gym.
+    Inherited from gymnasium.spaces.MultiDiscrete for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
```

### Comparing `rlberry-0.4.1/rlberry/spaces/tests/test_from_gym.py` & `rlberry-0.5.0/rlberry/spaces/tests/test_from_gym.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pytest
-import gym.spaces
+import gymnasium.spaces
 import rlberry.spaces
 from rlberry.spaces.from_gym import convert_space_from_gym
 
 
 @pytest.mark.parametrize("n", list(range(1, 10)))
 def test_discrete_space(n):
-    gym_sp = gym.spaces.Discrete(n)
+    gym_sp = gymnasium.spaces.Discrete(n)
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.Discrete)
     sp.reseed(123)
     for ii in range(n):
         assert sp.contains(ii)
 
     for ii in range(2 * n):
@@ -36,15 +36,15 @@
         (-np.inf, np.inf, 1),
         (-np.inf, np.inf, 2),
         (-np.inf, np.inf, 4),
     ],
 )
 def test_box_space_case_1(low, high, dim):
     shape = (dim, 1)
-    gym_sp = gym.spaces.Box(low, high, shape=shape)
+    gym_sp = gymnasium.spaces.Box(low, high, shape=shape)
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.Box)
     sp.reseed(123)
     for _ in range(2**dim):
         assert sp.contains(sp.sample())
 
 
@@ -55,95 +55,95 @@
         (np.array([-10.0, -10.0, -10.0]), np.array([10.0, 10.0, 10.0])),
         (np.array([-10.0, -10.0, -10.0]), np.array([10.0, 10.0, np.inf])),
         (np.array([-np.inf, -10.0, -10.0]), np.array([10.0, 10.0, np.inf])),
         (np.array([-np.inf, -10.0, -10.0]), np.array([np.inf, 10.0, np.inf])),
     ],
 )
 def test_box_space_case_2(low, high):
-    gym_sp = gym.spaces.Box(low, high, dtype=np.float64)
+    gym_sp = gymnasium.spaces.Box(low, high, dtype=np.float64)
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.Box)
     sp.reseed(123)
     if (-np.inf in low) or (np.inf in high):
         assert not sp.is_bounded()
     else:
         assert sp.is_bounded()
     for ii in range(2 ** sp.shape[0]):
         assert sp.contains(sp.sample())
 
 
 def test_tuple():
-    sp1 = gym.spaces.Box(0.0, 1.0, shape=(3, 2))
-    sp2 = gym.spaces.Discrete(2)
-    gym_sp = gym.spaces.Tuple([sp1, sp2])
+    sp1 = gymnasium.spaces.Box(0.0, 1.0, shape=(3, 2))
+    sp2 = gymnasium.spaces.Discrete(2)
+    gym_sp = gymnasium.spaces.Tuple([sp1, sp2])
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.Tuple)
     assert isinstance(sp.spaces[0], rlberry.spaces.Box)
     assert isinstance(sp.spaces[1], rlberry.spaces.Discrete)
     sp.reseed(123)
     for _ in range(10):
         assert sp.contains(sp.sample())
 
 
 def test_multidiscrete():
-    gym_sp = gym.spaces.MultiDiscrete([5, 2, 2])
+    gym_sp = gymnasium.spaces.MultiDiscrete([5, 2, 2])
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.MultiDiscrete)
     sp.reseed(123)
     for _ in range(10):
         assert sp.contains(sp.sample())
 
 
 def test_multibinary():
     for n in [1, 5, [3, 4]]:
-        gym_sp = gym.spaces.MultiBinary(n)
+        gym_sp = gymnasium.spaces.MultiBinary(n)
         sp = convert_space_from_gym(gym_sp)
         assert isinstance(sp, rlberry.spaces.MultiBinary)
         for _ in range(10):
             assert sp.contains(sp.sample())
         sp.reseed(123)
 
 
 def test_dict():
-    nested_observation_space = gym.spaces.Dict(
+    nested_observation_space = gymnasium.spaces.Dict(
         {
-            "sensors": gym.spaces.Dict(
+            "sensors": gymnasium.spaces.Dict(
                 {
-                    "position": gym.spaces.Box(low=-100, high=100, shape=(3,)),
-                    "velocity": gym.spaces.Box(low=-1, high=1, shape=(3,)),
-                    "front_cam": gym.spaces.Tuple(
+                    "position": gymnasium.spaces.Box(low=-100, high=100, shape=(3,)),
+                    "velocity": gymnasium.spaces.Box(low=-1, high=1, shape=(3,)),
+                    "front_cam": gymnasium.spaces.Tuple(
                         (
-                            gym.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
-                            gym.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
+                            gymnasium.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
+                            gymnasium.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
                         )
                     ),
-                    "rear_cam": gym.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
+                    "rear_cam": gymnasium.spaces.Box(low=0, high=1, shape=(10, 10, 3)),
                 }
             ),
-            "ext_controller": gym.spaces.MultiDiscrete((5, 2, 2)),
-            "inner_state": gym.spaces.Dict(
+            "ext_controller": gymnasium.spaces.MultiDiscrete((5, 2, 2)),
+            "inner_state": gymnasium.spaces.Dict(
                 {
-                    "charge": gym.spaces.Discrete(100),
-                    "system_checks": gym.spaces.MultiBinary(10),
-                    "job_status": gym.spaces.Dict(
+                    "charge": gymnasium.spaces.Discrete(100),
+                    "system_checks": gymnasium.spaces.MultiBinary(10),
+                    "job_status": gymnasium.spaces.Dict(
                         {
-                            "task": gym.spaces.Discrete(5),
-                            "progress": gym.spaces.Box(low=0, high=100, shape=()),
+                            "task": gymnasium.spaces.Discrete(5),
+                            "progress": gymnasium.spaces.Box(low=0, high=100, shape=()),
                         }
                     ),
                 }
             ),
         }
     )
     gym_sp = nested_observation_space
     sp = convert_space_from_gym(gym_sp)
     assert isinstance(sp, rlberry.spaces.Dict)
     for _ in range(10):
         assert sp.contains(sp.sample())
     sp.reseed(123)
 
-    gym_sp2 = gym.spaces.Dict(sp.spaces)
+    gym_sp2 = gymnasium.spaces.Dict(sp.spaces)
     sp2 = convert_space_from_gym(gym_sp2)
     assert isinstance(sp2, rlberry.spaces.Dict)
     for _ in range(10):
         assert sp.contains(sp2.sample())
     sp2.reseed(123)
```

### Comparing `rlberry-0.4.1/rlberry/spaces/tests/test_spaces.py` & `rlberry-0.5.0/rlberry/spaces/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/spaces/tuple.py` & `rlberry-0.5.0/rlberry/spaces/dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import gym
+import gymnasium as gym
 from rlberry.seeding import Seeder
 
 
-class Tuple(gym.spaces.Tuple):
+class Dict(gym.spaces.Dict):
     """
 
-    Inherited from gym.spaces.Tuple for compatibility with gym.
+    Inherited from gymnasium.spaces.Dict for compatibility with gym.
 
     rlberry wraps gym.spaces to make sure the seeding
     mechanism is unified in the library (rlberry.seeding)
 
     Attributes
     ----------
     rng : numpy.random._generator.Generator
@@ -17,17 +17,17 @@
 
     Methods
     -------
     reseed()
         get new random number generator
     """
 
-    def __init__(self, spaces):
-        gym.spaces.Tuple.__init__(self, spaces)
+    def __init__(self, spaces=None, **spaces_kwargs):
+        gym.spaces.Dict.__init__(self, spaces, **spaces_kwargs)
         self.seeder = Seeder()
 
     @property
     def rng(self):
         return self.seeder.rng
 
     def reseed(self, seed_seq=None):
-        _ = [space.reseed(seed_seq) for space in self.spaces]
+        _ = [space.reseed(seed_seq) for space in self.spaces.values()]
```

### Comparing `rlberry-0.4.1/rlberry/tests/test_agent_extra.py` & `rlberry-0.5.0/rlberry/tests/test_agent_extra.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/tests/test_agents_base.py` & `rlberry-0.5.0/rlberry/tests/test_agents_base.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/tests/test_envs.py` & `rlberry-0.5.0/rlberry/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/binsearch.py` & `rlberry-0.5.0/rlberry/utils/binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/check_agent.py` & `rlberry-0.5.0/rlberry/utils/check_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     n_checks : int, default=5
         number of checks to do.
     """
     result = True
     set_external_seed(SEED)
     results1 = []
     if compare_using == "policy":
-        state = agent1.env.reset()
+        state, info = agent1.env.reset()
     for f in range(n_checks):
         # do several tests if there is some randomness.
         if compare_using == "policy":
             results1.append(agent1.policy(state))
         else:
             method_to_call = getattr(agent1, compare_using)
             results1.append(method_to_call())
@@ -254,33 +254,46 @@
 
         # test individual agents save and load
         assert (
             os.path.getsize(str(manager.output_dir_) + "/agent_handlers/idx_0.pickle")
             > 1
         ), "The saved file is empty."
         try:
-            manager.load(str(manager.output_dir_) + "/agent_handlers/idx_0.pickle")
-        except Exception:
+            params_for_loader = dict(env=test_env)
+
+            if agent.__module__ == "rlberry.agents.stable_baselines.stable_baselines":
+                # StableBaselinesAgent need to add some params to load
+                params_for_loader["algo_cls"] = init_kwargs["algo_cls"]
+
+            agent.load(
+                str(manager.output_dir_) + "/agent_handlers/idx_0.pickle",
+                **params_for_loader
+            )
+        except Exception as ex:
             raise RuntimeError("Failed to load the agent file.")
 
         # test agentManager save and load
         manager.save()
         assert os.path.exists(tmpdirname)
 
-        path_to_load = next(pathlib.Path(tmpdirname).glob("**/*.pickle"))
+        path_to_load = next(pathlib.Path(tmpdirname).glob("**/manager_obj.pickle"))
         loaded_agent_manager = AgentManager.load(path_to_load)
         assert loaded_agent_manager
 
         # test with first agent of the manager
-        observation = test_env.reset()
+        observation, info = test_env.reset()
+
         for tt in range(50):
             action = loaded_agent_manager.get_agent_instances()[0].policy(observation)
-            next_observation, reward, done, info = test_env.step(action)
+            next_observation, reward, terminated, truncated, info = test_env.step(
+                action
+            )
+            done = terminated or truncated
             if done:
-                next_observation = test_env.reset()
+                next_observation, info = test_env.reset()
             observation = next_observation
 
 
 def _check_save_load_without_manager(agent, env="continuous_state", init_kwargs=None):
     """
     Check that the agent save a non-empty file and can load.
 
@@ -309,35 +322,31 @@
 
         # test agentManager save and load
         my_agent.save(saving_path)
         assert os.path.exists(tmpdirname)
 
         params_for_loader = dict(env=train_env)
 
-        # extract the class name to check if we need to add some param to load
-        try:
-            from rlberry.agents.stable_baselines.stable_baselines import (
-                StableBaselinesAgent,
-            )
-
-            if issubclass(agent, StableBaselinesAgent):
-                params_for_loader["algo_cls"] = init_kwargs["algo_cls"]
-        except ModuleNotFoundError:
-            pass
+        if agent.__module__ == "rlberry.agents.stable_baselines.stable_baselines":
+            # StableBaselinesAgent need to add some params to load
+            params_for_loader["algo_cls"] = init_kwargs["algo_cls"]
 
         loaded_agent = agent.load(saving_path, **params_for_loader)
         assert loaded_agent
 
         # test the agent
-        observation = test_env.reset()
+        observation, info = test_env.reset()
         for tt in range(50):
             action = loaded_agent.policy(observation)
-            next_observation, reward, done, info = test_env.step(action)
+            next_observation, reward, terminated, truncated, info = test_env.step(
+                action
+            )
+            done = terminated or truncated
             if done:
-                next_observation = test_env.reset()
+                next_observation, info = test_env.reset()
             observation = next_observation
 
 
 def check_seeding_agent(agent, env=None, continuous_state=False, init_kwargs=None):
     """
     Check that the agent is reproducible.
 
@@ -393,18 +402,20 @@
     except:
         pass
 
     agent1.fit(13)
     agent1.fit(13)
 
     # test
-    state = test_load_env.reset()
+    state, info = test_load_env.reset()
     for tt in range(50):
         action = agent1.policy(state)
-        next_s, _, done, test = test_load_env.step(action)
+        next_s, _, terminated, truncated, test = test_load_env.step(action)
+        done = terminated or truncated
+
         if done:
             break
         state = next_s
 
 
 def check_vectorized_env_agent(
     agent, env="vectorized_env_continuous", agent_init_kwargs=None
@@ -440,18 +451,20 @@
     test_env = env_d[0](**env_d[1])
 
     agent1 = agent(train_env, **agent_init_kwargs)
     agent1.fit(13)
     agent1.fit(13)
 
     # test the agent
-    state = test_env.reset()
+    state, info = test_env.reset()
     for tt in range(50):
         action = agent1.policy(state)
-        next_s, _, done, test = test_env.step(action)
+        next_s, _, terminated, truncated, test = test_env.step(action)
+        done = terminated or truncated
+
         if done:
             break
         state = next_s
 
 
 def check_rl_agent(agent, env="continuous_state", init_kwargs=None):
     """
```

### Comparing `rlberry-0.4.1/rlberry/utils/check_bandit_agent.py` & `rlberry-0.5.0/rlberry/utils/check_bandit_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     )
     agent2 = AgentManager(
         Agent, (env_ctor, env_kwargs), fit_budget=10, n_fit=1, seed=seed
     )
 
     agent1.fit()
     agent2.fit()
-    state = 0
+    env = env_ctor(**env_kwargs)
+    state, info = env.reset()
     result = True
     for _ in range(5):
         # test reproducibility on 5 actions
         action1 = agent1.agent_handlers[0].policy(state)
         action2 = agent2.agent_handlers[0].policy(state)
         if action1 != action2:
             result = False
```

### Comparing `rlberry-0.4.1/rlberry/utils/check_env.py` & `rlberry-0.5.0/rlberry/utils/check_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/check_gym_env.py` & `rlberry-0.5.0/rlberry/utils/check_gym_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Based on https://github.com/openai/gym and then modified for our purpose.
 """
 
 from typing import Union, Optional
 import inspect
 
-import gym
+import gymnasium as gym
 import numpy as np
-from gym import logger
-from gym import spaces
+from gymnasium import logger
+from gymnasium import spaces
 
 
 def _is_numpy_array_space(space: spaces.Space) -> bool:
     """
     Returns False if provided space is not representable as a single numpy array
     (e.g. Dict and Tuple spaces return False)
     """
@@ -34,15 +34,15 @@
         )
 
 
 def _check_nan(env: gym.Env, check_inf: bool = True) -> None:
     """Check for NaN and Inf."""
     for _ in range(10):
         action = env.action_space.sample()
-        observation, reward, _, _ = env.step(action)
+        observation, reward, _, _, _ = env.step(action)
 
         if np.any(np.isnan(observation)):
             logger.warn("Encountered NaN value in observations.")
         if np.any(np.isnan(reward)):
             logger.warn("Encountered NaN value in rewards.")
         if check_inf and np.any(np.isinf(observation)):
             logger.warn("Encountered inf value in observations.")
@@ -125,57 +125,64 @@
 
 def _check_returned_values(
     env: gym.Env, observation_space: spaces.Space, action_space: spaces.Space
 ) -> None:
     """
     Check the returned values by the env when calling `.reset()` or `.step()` methods.
     """
-    # because env inherits from gym.Env, we assume that `reset()` and `step()` methods exists
-    obs = env.reset()
+    # because env inherits from gymnasium.Env, we assume that `reset()` and `step()` methods exists
+    observation, info = env.reset()
 
     if isinstance(observation_space, spaces.Dict):
         assert isinstance(
-            obs, dict
+            observation, dict
         ), "The observation returned by `reset()` must be a dictionary"
         for key in observation_space.spaces.keys():
             try:
-                _check_obs(obs[key], observation_space.spaces[key], "reset")
+                _check_obs(observation[key], observation_space.spaces[key], "reset")
             except AssertionError as e:
                 raise AssertionError(f"Error while checking key={key}: " + str(e))
     else:
-        _check_obs(obs, observation_space, "reset")
+        _check_obs(observation, observation_space, "reset")
 
     # Sample a random action
     action = action_space.sample()
     data = env.step(action)
 
     assert (
-        len(data) == 4
-    ), "The `step()` method must return four values: obs, reward, done, info"
+        len(data) == 5
+    ), "The `step()` method must return four values: observation, reward, terminated, truncated, info "
 
     # Unpack
-    obs, reward, done, info = data
+    observation, reward, terminated, truncated, info = data
 
     if isinstance(observation_space, spaces.Dict):
         assert isinstance(
-            obs, dict
+            observation, dict
         ), "The observation returned by `step()` must be a dictionary"
         for key in observation_space.spaces.keys():
             try:
-                _check_obs(obs[key], observation_space.spaces[key], "step")
+                _check_obs(observation[key], observation_space.spaces[key], "step")
             except AssertionError as e:
                 raise AssertionError(f"Error while checking key={key}: " + str(e))
 
     else:
-        _check_obs(obs, observation_space, "step")
+        _check_obs(observation, observation_space, "step")
 
     # We also allow int because the reward will be cast to float
     assert isinstance(
         reward, (float, int, np.float32)
     ), "The reward returned by `step()` must be a float"
+    assert isinstance(
+        terminated, bool
+    ), "The `terminated` returned by `step()` must be a boolean"
+    assert isinstance(
+        truncated, bool
+    ), "The `truncated` returned by `step()` must be a boolean"
+    done = terminated or truncated
     assert isinstance(done, bool), "The `done` signal must be a boolean"
     assert isinstance(
         info, dict
     ), "The `info` returned by `step()` must be a python dictionary"
 
 
 # Check render cannot be covered by CI
```

### Comparing `rlberry-0.4.1/rlberry/utils/io.py` & `rlberry-0.5.0/rlberry/utils/io.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/logging.py` & `rlberry-0.5.0/rlberry/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import logging.config
 from pathlib import Path
-import gym
+import gymnasium as gym
 import rlberry
 
 
 def set_level(level="INFO"):
     """
     Set rlberry's logger level.
```

### Comparing `rlberry-0.4.1/rlberry/utils/metrics.py` & `rlberry-0.5.0/rlberry/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/space_discretizer.py` & `rlberry-0.5.0/rlberry/utils/space_discretizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from gym.spaces import Box, Discrete
+from gymnasium.spaces import Box, Discrete
 from rlberry.utils.binsearch import binary_search_nd
 from rlberry.utils.binsearch import unravel_index_uniform_bin
 
 
 class Discretizer:
     def __init__(self, space, n_bins):
         assert isinstance(
```

### Comparing `rlberry-0.4.1/rlberry/utils/tests/test_binsearch.py` & `rlberry-0.5.0/rlberry/utils/tests/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/tests/test_check.py` & `rlberry-0.5.0/rlberry/utils/tests/test_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from rlberry.utils.check_env import check_env
 from rlberry.utils.check_agent import (
     check_rl_agent,
     _fit_agent_manager,
     check_agents_almost_equal,
 )
 from rlberry.spaces import Box, Dict, Discrete
-import gym
+import gymnasium as gym
 from rlberry.agents import ValueIterationAgent, UCBVIAgent
 
 
 class ActionDictTestEnv(gym.Env):
     action_space = Dict({"position": Discrete(1), "velocity": Discrete(1)})
     observation_space = Box(low=-1.0, high=2.0, shape=(3,), dtype=np.float32)
 
     def step(self, action):
         observation = np.array([1.0, 1.5, 0.5])
         reward = 1
         done = True
         return observation, reward, done
 
-    def reset(self):
-        return np.array([1.0, 1.5, 0.5])
+    def reset(self, seed=None, options=None):
+        return np.array([1.0, 1.5, 0.5]), {}
 
 
 class DummyAgent:
     def __init__(self, **kwargs):
         pass
 
 
@@ -38,19 +38,22 @@
     def eval(self, eval_horizon=5, n_simulations=2, gamma=1.0, **kwargs):
         """
         rewrite the eval function to have a smaller eval_horizon
         """
         del kwargs  # unused
         episode_rewards = np.zeros(n_simulations)
         for sim in range(n_simulations):
-            observation = self.eval_env.reset()
+            observation, info = self.eval_env.reset()
             tt = 0
             while tt < eval_horizon:
                 action = self.policy(observation)
-                observation, reward, done, _ = self.eval_env.step(action)
+                observation, reward, terminated, truncated, info = self.eval_env.step(
+                    action
+                )
+                done = terminated or truncated
                 episode_rewards[sim] += reward * np.power(gamma, tt)
                 tt += 1
 
         return episode_rewards.mean()
 
 
 def test_check_env_dict_action():
```

### Comparing `rlberry-0.4.1/rlberry/utils/tests/test_writer.py` & `rlberry-0.5.0/rlberry/utils/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/torch.py` & `rlberry-0.5.0/rlberry/utils/torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/utils/writers.py` & `rlberry-0.5.0/rlberry/utils/writers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/wrappers/discrete2onehot.py` & `rlberry-0.5.0/rlberry/wrappers/discrete2onehot.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         )
 
     def process_obs(self, obs):
         one_hot_obs = np.zeros(self.env.observation_space.n, dtype=np.uint32)
         one_hot_obs[obs] = 1.0
         return one_hot_obs
 
-    def reset(self):
-        obs = self.env.reset()
-        return self.process_obs(obs)
+    def reset(self, seed=None, options=None):
+        obs, info = self.env.reset(seed=seed, options=options)
+        return self.process_obs(obs), info
 
     def step(self, action):
-        observation, reward, done, info = self.env.step(action)
+        observation, reward, terminated, truncated, info = self.env.step(action)
         observation = self.process_obs(observation)
-        return observation, reward, done, info
+        return observation, reward, terminated, truncated, info
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/discretize_state.py` & `rlberry-0.5.0/rlberry/wrappers/discretize_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,32 +40,35 @@
         self.observation_space = spaces.Discrete(n_states)
 
         # List of discretized states
         self.discretized_states = np.zeros((self.dim, n_states))
         for ii in range(n_states):
             self.discretized_states[:, ii] = self.get_continuous_state(ii, False)
 
-    def reset(self):
-        return self.get_discrete_state(self.env.reset())
+    def reset(self, seed=None, options=None):
+        obs, info = self.env.reset(seed, options)
+        return self.get_discrete_state(obs), info
 
     def step(self, action):
-        next_state, reward, done, info = self.env.step(action)
-        next_state = binary_search_nd(next_state, self._bins)
-        return next_state, reward, done, info
+        next_observation, reward, terminated, truncated, info = self.env.step(action)
+        next_observation = binary_search_nd(next_observation, self._bins)
+        return next_observation, reward, terminated, truncated, info
 
     def sample(self, discrete_state, action):
         # map disctete state to continuous one
         assert self.observation_space.contains(discrete_state)
         continuous_state = self.get_continuous_state(discrete_state, randomize=True)
         # sample in the true environment
-        next_state, reward, done, info = self.env.sample(continuous_state, action)
+        next_state, reward, terminated, truncated, info = self.env.sample(
+            continuous_state, action
+        )
         # discretize next state
         next_state = binary_search_nd(next_state, self._bins)
 
-        return next_state, reward, done, info
+        return next_state, reward, terminated, truncated, info
 
     def get_discrete_state(self, continuous_state):
         return binary_search_nd(continuous_state, self._bins)
 
     def get_continuous_state(self, discrete_state, randomize=False):
         assert (
             discrete_state >= 0 and discrete_state < self.observation_space.n
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/rescale_reward.py` & `rlberry-0.5.0/rlberry/wrappers/rescale_reward.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             return self._linear_rescaling(x, 0.0, 1.0, u0, u1)
             # unbounded
         else:
             x = 1.0 / (1.0 + np.exp(-reward))  # [0, 1]
             return self._linear_rescaling(x, 0.0, 1.0, u0, u1)
 
     def step(self, action):
-        observation, reward, done, info = self.env.step(action)
+        observation, reward, terminated, truncated, info = self.env.step(action)
         rescaled_reward = self._rescale(reward)
-        return observation, rescaled_reward, done, info
+        return observation, rescaled_reward, terminated, truncated, info
 
     def sample(self, state, action):
-        observation, reward, done, info = self.env.sample(state, action)
+        observation, reward, terminated, truncated, info = self.env.sample(
+            state, action
+        )
         rescaled_reward = self._rescale(reward)
-        return observation, rescaled_reward, done, info
+        return observation, rescaled_reward, terminated, truncated, info
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/tests/test_basewrapper.py` & `rlberry-0.5.0/rlberry/wrappers/tests/test_basewrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rlberry.envs.interface import Model
 from rlberry.envs import Wrapper
 from rlberry.envs import GridWorld
-import gym
+import gymnasium as gym
 
 
 def test_wrapper():
     env = GridWorld()
     wrapped = Wrapper(env)
     assert isinstance(wrapped, Model)
     assert wrapped.is_online()
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/tests/test_gym_space_conversion.py` & `rlberry-0.5.0/rlberry/wrappers/tests/test_gym_space_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pytest
-import gym
+import gymnasium as gym
 import rlberry
 from rlberry.wrappers.gym_utils import convert_space_from_gym
 
 
 def convert_and_compare(sp, rlberry_space):
     sp_conv = convert_space_from_gym(sp)
     assert isinstance(sp_conv, rlberry_space)
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/tests/test_wrapper_seeding.py` & `rlberry-0.5.0/rlberry/wrappers/tests/test_wrapper_seeding.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from rlberry.envs.finite import GridWorld
 from rlberry.envs.benchmarks.ball_exploration import PBall2D, SimplePBallND
 from rlberry.envs import Wrapper
 from rlberry.wrappers import RescaleRewardWrapper
 
 _GYM_INSTALLED = True
 try:
-    import gym
+    import gymnasium as gym
 except Exception:
     _GYM_INSTALLED = False
 
 classes = [MountainCar, GridWorld, Chain, PBall2D, SimplePBallND, Acrobot]
 
 
 def get_env_trajectory(env, horizon):
     states = []
-    ss = env.reset()
+    ss, info = env.reset()
     for _ in range(horizon):
         states.append(ss)
-        ss, _, _, _ = env.step(env.action_space.sample())
+        ss, _, _, _, _ = env.step(env.action_space.sample())
     return states
 
 
 def compare_trajectories(traj1, traj2):
     for ss1, ss2 in zip(traj1, traj2):
         if not np.array_equal(ss1, ss2):
             return False
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/tests/test_writer_utils.py` & `rlberry-0.5.0/rlberry/wrappers/tests/test_writer_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.1/rlberry/wrappers/uncertainty_estimator_wrapper.py` & `rlberry-0.5.0/rlberry/wrappers/uncertainty_estimator_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Adds exploration bonuses to the info output of env.step(), according to an
     instance of UncertaintyEstimator.
 
     Example
     -------
 
     ```
-    observation, reward, done, info = env.step(action)
+    observation, reward, terminated, truncated, info  = env.step(action)
     bonus = info['exploration_bonus']
     ```
 
     Parameters
     ----------
     uncertainty_estimator_fn : function(observation_space,
                                         action_space, **kwargs)
@@ -55,27 +55,28 @@
             else uncertainty_estimator_fn
         )
         self.uncertainty_estimator = uncertainty_estimator_fn(
             env.observation_space, env.action_space, **uncertainty_estimator_kwargs
         )
         self.previous_obs = None
 
-    def reset(self):
-        self.previous_obs = self.env.reset()
-        return self.previous_obs
+    def reset(self, seed=None, options=None):
+        self.previous_obs, info = self.env.reset(seed=seed, options=options)
+        return self.previous_obs, info
 
     def _update_and_get_bonus(self, state, action, next_state, reward):
         if self.previous_obs is None:
             return 0.0
         #
         self.uncertainty_estimator.update(state, action, next_state, reward)
         return self.bonus(state, action)
 
     def step(self, action):
-        observation, reward, done, info = self.env.step(action)
+        observation, reward, terminated, truncated, info = self.env.step(action)
+        done = terminated or truncated
 
         # update uncertainty and compute bonus
         bonus = self._update_and_get_bonus(
             self.previous_obs, action, observation, reward
         )
         #
         self.previous_obs = observation
@@ -88,15 +89,15 @@
                 logger.error(
                     "UncertaintyEstimatorWrapper Error: info has"
                     + "  already a key named exploration_bonus!"
                 )
 
         info["exploration_bonus"] = bonus
 
-        return observation, reward, done, info
+        return observation, reward, terminated, truncated, info
 
     def sample(self, state, action):
         logger.warning(
             "[UncertaintyEstimatorWrapper]: sample()"
             + " method does not consider nor update bonuses."
         )
         return self.env.sample(state, action)
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/vis2d.py` & `rlberry-0.5.0/rlberry/wrappers/vis2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rlberry.envs import Wrapper
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from rlberry.rendering.utils import video_write
-import gym.spaces as spaces
+import gymnasium.spaces as spaces
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 import rlberry
 
 logger = rlberry.logger
@@ -106,21 +106,21 @@
         )
         self.episode_visit_counter = DiscreteCounter(
             self.env.observation_space, self.env.action_space, n_bins_obs=n_bins_obs
         )
         self.current_state = None
         self.curret_step = 0
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         self.current_step = 0
-        self.current_state = self.env.reset()
-        return self.current_state
+        self.current_state, info = self.env.reset(seed, options)
+        return self.current_state, info
 
     def step(self, action):
-        observation, reward, done, info = self.env.step(action)
+        observation, reward, terminated, truncated, info = self.env.step(action)
         # initialize new trajectory
         if self.current_step == 0:
             self.memory.end_trajectory()
             self.episode_visit_counter.reset()
         self.current_step += 1
         # update counters
         ss, aa = self.current_state, action
@@ -135,15 +135,15 @@
             reward,
             self.total_visit_counter.count(ss, aa),
             self.episode_visit_counter.count(ss, aa),
         )
         self.memory.append(transition)
         # update current state
         self.current_state = observation
-        return observation, reward, done, info
+        return observation, reward, terminated, truncated, info
 
     def plot_trajectories(
         self,
         fignum=None,
         figsize=(6, 6),
         hide_axis=True,
         show=True,
```

### Comparing `rlberry-0.4.1/rlberry/wrappers/writer_utils.py` & `rlberry-0.5.0/rlberry/wrappers/writer_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     def __init__(self, env, writer, write_scalar="reward"):
         Wrapper.__init__(self, env)
         self.writer = writer
         self.write_scalar = write_scalar
         self.iteration_ = 0
 
     def step(self, action):
-        observation, reward, done, info = self.env.step(action)
+        observation, reward, terminated, truncated, info = self.env.step(action)
 
         self.iteration_ += 1
         if self.write_scalar == "reward":
             self.writer.add_scalar("reward", reward, self.iteration_)
         elif self.write_scalar == "action":
             self.writer.add_scalar("action", action, self.iteration_)
         elif self.write_scalar == "action_and_reward":
             self.writer.add_scalar("reward", reward, self.iteration_)
             self.writer.add_scalar("action", action, self.iteration_)
         else:
             raise ValueError("write_scalar %s is not known" % (self.write_scalar))
 
-        return observation, reward, done, info
+        return observation, reward, terminated, truncated, info
```

### Comparing `rlberry-0.4.1/rlberry.egg-info/PKG-INFO` & `rlberry-0.5.0/rlberry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlberry
-Version: 0.4.1
+Version: 0.5.0
 Summary: An easy-to-use reinforcement learning library for research and education
 Home-page: https://github.com/rlberry-py
 Author: Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,17 +12,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: default
-Provides-Extra: deploy
 Provides-Extra: jax_agents
 Provides-Extra: torch_agents
+Provides-Extra: deploy
 License-File: LICENSE
 
 <!-- Logo -->
 <p align="center">
    <img src="https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/logo_wide.svg" width="50%">
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: rlberry Version: 0.4.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: rlberry Version: 0.5.0 Summary: An easy-to-use
 reinforcement learning library for research and education Home-page: https://
 github.com/rlberry-py Author: Omar Darwiche Domingues, Yannis Flet-Berliac,
 Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Education Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
-Extra: default Provides-Extra: deploy Provides-Extra: jax_agents Provides-
-Extra: torch_agents License-File: LICENSE
+Extra: default Provides-Extra: jax_agents Provides-Extra: torch_agents
+Provides-Extra: deploy License-File: LICENSE
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
            [pytest] [Documentation_Status] [contributors] [codecov]
 
                     Try_it_on_Google_Colab!_[Open_In_Colab]
```

### Comparing `rlberry-0.4.1/rlberry.egg-info/SOURCES.txt` & `rlberry-0.5.0/rlberry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 rlberry/envs/finite/gridworld_utils.py
 rlberry/envs/interface/__init__.py
 rlberry/envs/interface/model.py
 rlberry/envs/tests/__init__.py
 rlberry/envs/tests/test_bandits.py
 rlberry/envs/tests/test_env_seeding.py
 rlberry/envs/tests/test_gym_env_seeding.py
+rlberry/envs/tests/test_gym_make.py
 rlberry/envs/tests/test_instantiation.py
 rlberry/envs/tests/test_spring_env.py
 rlberry/experiment/__init__.py
 rlberry/experiment/generator.py
 rlberry/experiment/load_results.py
 rlberry/experiment/yaml_utils.py
 rlberry/exploration_tools/__init__.py
@@ -233,23 +234,34 @@
 rlberry/utils/writers.py
 rlberry/utils/tests/__init__.py
 rlberry/utils/tests/test_binsearch.py
 rlberry/utils/tests/test_check.py
 rlberry/utils/tests/test_metrics.py
 rlberry/utils/tests/test_writer.py
 rlberry/wrappers/__init__.py
-rlberry/wrappers/atari_utils.py
 rlberry/wrappers/autoreset.py
 rlberry/wrappers/discrete2onehot.py
 rlberry/wrappers/discretize_state.py
 rlberry/wrappers/gym_utils.py
 rlberry/wrappers/rescale_reward.py
-rlberry/wrappers/scalarize.py
 rlberry/wrappers/uncertainty_estimator_wrapper.py
 rlberry/wrappers/vis2d.py
 rlberry/wrappers/writer_utils.py
 rlberry/wrappers/tests/__init__.py
 rlberry/wrappers/tests/test_basewrapper.py
 rlberry/wrappers/tests/test_common_wrappers.py
 rlberry/wrappers/tests/test_gym_space_conversion.py
 rlberry/wrappers/tests/test_wrapper_seeding.py
-rlberry/wrappers/tests/test_writer_utils.py
+rlberry/wrappers/tests/test_writer_utils.py
+rlberry/wrappers/tests/old_env/__init__.py
+rlberry/wrappers/tests/old_env/old_acrobot.py
+rlberry/wrappers/tests/old_env/old_apple_gold.py
+rlberry/wrappers/tests/old_env/old_ball2d.py
+rlberry/wrappers/tests/old_env/old_finite_mdp.py
+rlberry/wrappers/tests/old_env/old_four_room.py
+rlberry/wrappers/tests/old_env/old_gridworld.py
+rlberry/wrappers/tests/old_env/old_mountain_car.py
+rlberry/wrappers/tests/old_env/old_nroom.py
+rlberry/wrappers/tests/old_env/old_pball.py
+rlberry/wrappers/tests/old_env/old_pendulum.py
+rlberry/wrappers/tests/old_env/old_six_room.py
+rlberry/wrappers/tests/old_env/old_twinrooms.py
```

### Comparing `rlberry-0.4.1/setup.py` & `rlberry-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,41 +14,43 @@
 install_requires = [
     "numpy>=1.17",
     "scipy>=1.6",
     "pygame-ce",
     "matplotlib",
     "seaborn",
     "pandas",
-    #"gym[accept-rom-license] @ git+https://github.com/rlberry-py/gym_fix_021",
-    "gym[accept-rom-license]==0.21",
+    "gymnasium",
     "dill",
     "docopt",
     "pyyaml",
+    "tqdm",
 ]
 
 #
 # Extras
 #
 
 # default installation
 default_requires = [
     "numba",
     "optuna",
     "ffmpeg-python",
     "PyOpenGL",
-    "PyOpenGL_accelerate",
     "pyvirtualdisplay",
+    "gymnasium",
 ]
 
 # tensorboard must be installed manually, due to conflicts with
 # dm-reverb-nightly[tensorflow] in jax_agents_requires
 torch_agents_requires = default_requires + [
     "torch>=1.6.0",
     "opencv-python",
-    "ale-py==0.7.4",
+    "gymnasium[atari,accept-rom-license]",
+    "ale-py>=0.8.0",
+    "stable-baselines3",
     # 'tensorboard'
 ]
 
 jax_agents_requires = default_requires + [
     "jax[cpu]",
     "chex",
     "dm-haiku",
```

