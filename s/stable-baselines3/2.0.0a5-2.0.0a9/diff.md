# Comparing `tmp/stable_baselines3-2.0.0a5.tar.gz` & `tmp/stable_baselines3-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable_baselines3-2.0.0a5.tar", last modified: Fri Apr 14 11:50:42 2023, max compression
+gzip compressed data, was "stable_baselines3-2.0.0a9.tar", last modified: Sat May 20 08:31:33 2023, max compression
```

## Comparing `stable_baselines3-2.0.0a5.tar` & `stable_baselines3-2.0.0a9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a5/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a5/NOTICE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14112 2023-03-29 22:22:11.000000 stable_baselines3-2.0.0a5/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2893 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/pyproject.toml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5706 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3/a2c/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/a2c.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/atari_wrappers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    37082 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/base_class.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    33755 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26487 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    27242 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20619 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7539 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/env_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8099 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/bit_flipping_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/identity_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6449 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/multi_input_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    23428 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5545 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/noise.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26104 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12001 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    40165 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/results_plotter.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/running_mean_std.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20664 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/save_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5631 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/torch_layers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3117 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21221 2023-04-14 11:50:27.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15814 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/base_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7073 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/patch_gym.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8298 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/stacked_observations.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10631 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2986 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/util.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-12 13:21:02.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2062 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3807 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_transpose.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/ddpg.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12908 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10673 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/her/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/__init__.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/goal_selection_strategy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/her_replay_buffer.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14928 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a5/stable_baselines3/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20669 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15920 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.668670 stable_baselines3-2.0.0a5/stable_baselines3/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14471 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11193 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/td3.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-14 11:50:27.000000 stable_baselines3-2.0.0a5/stable_baselines3/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      744 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5687 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/tests/test_custom_policy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a5/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3739 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9887 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_gae.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_her.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14793 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3756 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_predict.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26907 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a5/tests/test_sde.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4338 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_spaces.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/tests/test_tensorboard.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22809 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1389 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20064 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2231 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_stacked_obs.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.067686 stable_baselines3-2.0.0a9/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a9/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a9/NOTICE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3287 2023-05-20 08:31:33.067686 stable_baselines3-2.0.0a9/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14165 2023-05-08 11:48:33.000000 stable_baselines3-2.0.0a9/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2224 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/pyproject.toml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-05-20 08:31:33.067686 stable_baselines3-2.0.0a9/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5722 2023-05-08 11:48:33.000000 stable_baselines3-2.0.0a9/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.039685 stable_baselines3-2.0.0a9/stable_baselines3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.043685 stable_baselines3-2.0.0a9/stable_baselines3/a2c/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/a2c/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/a2c/a2c.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a9/stable_baselines3/a2c/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.047685 stable_baselines3-2.0.0a9/stable_baselines3/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/atari_wrappers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    37082 2023-05-14 16:40:17.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/base_class.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    33605 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26487 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27242 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20766 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7630 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/env_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.051685 stable_baselines3-2.0.0a9/stable_baselines3/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8367 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/envs/bit_flipping_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-05-08 12:31:56.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/envs/identity_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6497 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/envs/multi_input_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    24012 2023-05-08 07:54:58.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5541 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/noise.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26104 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12001 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    40165 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/results_plotter.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/running_mean_std.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20664 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/save_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.051685 stable_baselines3-2.0.0a9/stable_baselines3/common/sb2_compat/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/sb2_compat/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5625 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/torch_layers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3117 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20791 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.055685 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    16645 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/base_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6831 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/dummy_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/patch_gym.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8298 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/stacked_observations.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10480 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/subproc_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3042 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/util.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1194 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2114 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_frame_stack.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3892 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-05-01 11:47:05.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_transpose.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_video_recorder.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.055685 stable_baselines3-2.0.0a9/stable_baselines3/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a9/stable_baselines3/ddpg/ddpg.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/ddpg/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.055685 stable_baselines3-2.0.0a9/stable_baselines3/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12838 2023-04-28 07:57:28.000000 stable_baselines3-2.0.0a9/stable_baselines3/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10673 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.059686 stable_baselines3-2.0.0a9/stable_baselines3/her/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/her/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a9/stable_baselines3/her/goal_selection_strategy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/her/her_replay_buffer.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.059686 stable_baselines3-2.0.0a9/stable_baselines3/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a9/stable_baselines3/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14928 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a9/stable_baselines3/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.059686 stable_baselines3-2.0.0a9/stable_baselines3/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20669 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15920 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.059686 stable_baselines3-2.0.0a9/stable_baselines3/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/stable_baselines3/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14471 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11193 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/stable_baselines3/td3/td3.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/stable_baselines3/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.039685 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3287 2023-05-20 08:31:32.000000 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-05-20 08:31:32.000000 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-05-20 08:31:32.000000 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      750 2023-05-20 08:31:32.000000 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-05-20 08:31:32.000000 stable_baselines3-2.0.0a9/stable_baselines3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:31:33.067686 stable_baselines3-2.0.0a9/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5740 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/tests/test_custom_policy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-05-14 15:40:24.000000 stable_baselines3-2.0.0a9/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3750 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10278 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_gae.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_her.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15808 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3767 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_predict.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27434 2023-04-28 07:57:28.000000 stable_baselines3-2.0.0a9/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a9/tests/test_sde.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4504 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_spaces.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a9/tests/test_tensorboard.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22783 2023-05-05 11:41:26.000000 stable_baselines3-2.0.0a9/tests/test_utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1398 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20486 2023-05-20 08:31:13.000000 stable_baselines3-2.0.0a9/tests/test_vec_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2231 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a9/tests/test_vec_stacked_obs.py
```

### Comparing `stable_baselines3-2.0.0a5/LICENSE` & `stable_baselines3-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/NOTICE` & `stable_baselines3-2.0.0a9/NOTICE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/PKG-INFO` & `stable_baselines3-2.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.0.0a5
+Version: 2.0.0a9
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
 Project-URL: SB3-Contrib, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: RL-Zoo, https://github.com/DLR-RM/rl-baselines3-zoo
-Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
+Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gymnasium gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `stable_baselines3-2.0.0a5/README.md` & `stable_baselines3-2.0.0a9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     # VecEnv resets automatically
     # if done:
     #   obs = env.reset()
 
 env.close()
 ```
 
-Or just train a model with a one liner if [the environment is registered in Gym](https://github.com/openai/gym/wiki/Environments) and if [the policy is registered](https://stable-baselines3.readthedocs.io/en/master/guide/custom_policy.html):
+Or just train a model with a one liner if [the environment is registered in Gymnasium](https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/#registering-envs) and if [the policy is registered](https://stable-baselines3.readthedocs.io/en/master/guide/custom_policy.html):
 
 ```python
 from stable_baselines3 import PPO
 
 model = PPO("MlpPolicy", "CartPole-v1").learn(10_000)
 ```
```

### Comparing `stable_baselines3-2.0.0a5/setup.py` & `stable_baselines3-2.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 setup(
     name="stable_baselines3",
     packages=[package for package in find_packages() if package.startswith("stable_baselines3")],
     package_data={"stable_baselines3": ["py.typed", "version.txt"]},
     install_requires=[
         "gymnasium==0.28.1",
-        "numpy",
+        "numpy>=1.20",
         "torch>=1.11",
         'typing_extensions>=4.0,<5; python_version < "3.8.0"',
         # For saving models
         "cloudpickle",
         # For reading logs
         "pandas",
         # Plotting learning curves
@@ -145,15 +145,15 @@
         "extra_no_roms": extra_no_roms,
     },
     description="Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.",
     author="Antonin Raffin",
     url="https://github.com/DLR-RM/stable-baselines3",
     author_email="antonin.raffin@dlr.de",
     keywords="reinforcement-learning-algorithms reinforcement-learning machine-learning "
-    "gym openai stable baselines toolbox python data-science",
+    "gymnasium gym openai stable baselines toolbox python data-science",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=__version__,
     python_requires=">=3.7",
     # PyPI package information.
     project_urls={
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/__init__.py` & `stable_baselines3-2.0.0a9/stable_baselines3/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/a2c/a2c.py` & `stable_baselines3-2.0.0a9/stable_baselines3/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/atari_wrappers.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/base_class.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/base_class.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/buffers.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,14 +677,16 @@
     :param device: PyTorch device
     :param gae_lambda: Factor for trade-off of bias vs variance for Generalized Advantage Estimator
         Equivalent to Monte-Carlo advantage estimate when set to 1.
     :param gamma: Discount factor
     :param n_envs: Number of parallel environments
     """
 
+    observations: Dict[str, np.ndarray]
+
     def __init__(
         self,
         buffer_size: int,
         observation_space: spaces.Space,
         action_space: spaces.Space,
         device: Union[th.device, str] = "auto",
         gae_lambda: float = 1,
@@ -693,16 +695,15 @@
     ):
         super(RolloutBuffer, self).__init__(buffer_size, observation_space, action_space, device, n_envs=n_envs)
 
         assert isinstance(self.obs_shape, dict), "DictRolloutBuffer must be used with Dict obs space only"
 
         self.gae_lambda = gae_lambda
         self.gamma = gamma
-        self.observations, self.actions, self.rewards, self.advantages = None, None, None, None
-        self.returns, self.episode_starts, self.values, self.log_probs = None, None, None, None
+
         self.generator_ready = False
         self.reset()
 
     def reset(self) -> None:
         assert isinstance(self.obs_shape, dict), "DictRolloutBuffer must be used with Dict obs space only"
         self.observations = {}
         for key, obs_input_shape in self.obs_shape.items():
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/callbacks.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/distributions.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/env_checker.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/env_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,19 @@
     # ============= Check the spaces (observation and action) ================
     _check_spaces(env)
 
     # Define aliases for convenience
     observation_space = env.observation_space
     action_space = env.action_space
 
+    try:
+        env.reset(seed=0)
+    except TypeError as e:
+        raise TypeError("The reset() method must accept a `seed` parameter") from e
+
     # Warn the user if needed.
     # A warning means that the environment may run but not work properly with Stable Baselines algorithms
     if warn:
         _check_unsupported_spaces(env, observation_space, action_space)
 
         obs_spaces = observation_space.spaces if isinstance(observation_space, spaces.Dict) else {"": observation_space}
         for key, space in obs_spaces.items():
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/env_util.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/env_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from typing import Any, Callable, Dict, Optional, Type, Union
 
 import gymnasium as gym
 
 from stable_baselines3.common.atari_wrappers import AtariWrapper
 from stable_baselines3.common.monitor import Monitor
-from stable_baselines3.common.utils import compat_gym_seed
 from stable_baselines3.common.vec_env import DummyVecEnv, SubprocVecEnv, VecEnv
 from stable_baselines3.common.vec_env.patch_gym import _patch_env
 
 
 def unwrap_wrapper(env: gym.Env, wrapper_class: Type[gym.Wrapper]) -> Optional[gym.Wrapper]:
     """
     Retrieve a ``VecEnvWrapper`` object by recursively searching.
@@ -97,15 +96,16 @@
                     env = gym.make(env_id, **env_kwargs)
             else:
                 env = env_id(**env_kwargs)
                 # Patch to support gym 0.21/0.26 and gymnasium
                 env = _patch_env(env)
 
             if seed is not None:
-                compat_gym_seed(env, seed=seed + rank)
+                # Note: here we only seed the action space
+                # We will seed the env at the next reset
                 env.action_space.seed(seed + rank)
             # Wrap the env in a Monitor wrapper
             # to have additional training information
             monitor_path = os.path.join(monitor_dir, str(rank)) if monitor_dir is not None else None
             # Create the monitor folder if needed
             if monitor_path is not None and monitor_dir is not None:
                 os.makedirs(monitor_dir, exist_ok=True)
@@ -118,15 +118,18 @@
         return _init
 
     # No custom VecEnv is passed
     if vec_env_cls is None:
         # Default: use a DummyVecEnv
         vec_env_cls = DummyVecEnv
 
-    return vec_env_cls([make_env(i + start_index) for i in range(n_envs)], **vec_env_kwargs)
+    vec_env = vec_env_cls([make_env(i + start_index) for i in range(n_envs)], **vec_env_kwargs)
+    # Prepare the seeds for the first reset
+    vec_env.seed(seed)
+    return vec_env
 
 
 def make_atari_env(
     env_id: Union[str, Callable[..., gym.Env]],
     n_envs: int = 1,
     seed: Optional[int] = None,
     start_index: int = 0,
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/__init__.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/bit_flipping_env.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/envs/bit_flipping_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,28 @@
     :param discrete_obs_space: Whether to use the discrete observation
         version or not, by default, it uses the ``MultiBinary`` one
     :param image_obs_space: Use image as input instead of the ``MultiBinary`` one.
     :param channel_first: Whether to use channel-first or last image.
     """
 
     spec = EnvSpec("BitFlippingEnv-v0", "no-entry-point")
+    state: np.ndarray
 
     def __init__(
         self,
         n_bits: int = 10,
         continuous: bool = False,
         max_steps: Optional[int] = None,
         discrete_obs_space: bool = False,
         image_obs_space: bool = False,
         channel_first: bool = True,
+        render_mode: str = "human",
     ):
         super().__init__()
+        self.render_mode = render_mode
         # Shape of the observation when using image space
         self.image_shape = (1, 36, 36) if channel_first else (36, 36, 1)
         # The achieved goal is determined by the current state
         # here, it is a special where they are equal
         if discrete_obs_space:
             # In the discrete case, the agent act on the binary
             # representation of the observation
@@ -91,15 +94,14 @@
         if continuous:
             self.action_space = spaces.Box(-1, 1, shape=(n_bits,), dtype=np.float32)
         else:
             self.action_space = spaces.Discrete(n_bits)
         self.continuous = continuous
         self.discrete_obs_space = discrete_obs_space
         self.image_obs_space = image_obs_space
-        self.state = None
         self.desired_goal = np.ones((n_bits,), dtype=self.observation_space["desired_goal"].dtype)
         if max_steps is None:
             max_steps = n_bits
         self.max_steps = max_steps
         self.current_step = 0
 
     def seed(self, seed: int) -> None:
@@ -123,29 +125,28 @@
             return image.reshape(self.image_shape).astype(np.uint8)
         return state
 
     def convert_to_bit_vector(self, state: Union[int, np.ndarray], batch_size: int) -> np.ndarray:
         """
         Convert to bit vector if needed.
 
-        :param state:
-        :param batch_size:
-        :return:
+        :param state: The state to be converted, which can be either an integer or a numpy array.
+        :param batch_size: The batch size.
+        :return: The state converted into a bit vector.
         """
         # Convert back to bit vector
         if isinstance(state, int):
-            state = np.array(state).reshape(batch_size, -1)
+            bit_vector = np.array(state).reshape(batch_size, -1)
             # Convert to binary representation
-            state = ((state[:, :] & (1 << np.arange(len(self.state)))) > 0).astype(int)
+            bit_vector = ((bit_vector[:, :] & (1 << np.arange(len(self.state)))) > 0).astype(int)
         elif self.image_obs_space:
-            state = state.reshape(batch_size, -1)[:, : len(self.state)] / 255
+            bit_vector = state.reshape(batch_size, -1)[:, : len(self.state)] / 255
         else:
-            state = np.array(state).reshape(batch_size, -1)
-
-        return state
+            bit_vector = np.array(state).reshape(batch_size, -1)
+        return bit_vector
 
     def _get_obs(self) -> Dict[str, Union[int, np.ndarray]]:
         """
         Helper to create the observation.
 
         :return: The current observation.
         """
@@ -201,14 +202,15 @@
         achieved_goal = self.convert_to_bit_vector(achieved_goal, batch_size)
 
         # Deceptive reward: it is positive only when the goal is achieved
         # Here we are using a vectorized version
         distance = np.linalg.norm(achieved_goal - desired_goal, axis=-1)
         return -(distance > 0).astype(np.float32)
 
-    def render(self, mode: str = "human") -> Optional[np.ndarray]:
-        if mode == "rgb_array":
+    def render(self) -> Optional[np.ndarray]:  # type: ignore[override]
+        if self.render_mode == "rgb_array":
             return self.state.copy()
         print(self.state)
+        return None
 
     def close(self) -> None:
         pass
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/identity_env.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/envs/identity_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/multi_input_envs.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/envs/multi_input_envs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
 
 from stable_baselines3.common.type_aliases import GymStepReturn
 
@@ -69,15 +69,15 @@
         self.max_count = 100
         self.log = ""
         self.state = 0
         self.action2str = ["left", "down", "right", "up"]
         self.init_possible_transitions()
 
         self.num_col = num_col
-        self.state_mapping = []
+        self.state_mapping: List[Dict[str, np.ndarray]] = []
         self.init_state_mapping(num_col, num_row)
 
         self.max_state = len(self.state_mapping) - 1
 
     def init_state_mapping(self, num_col: int, num_row: int) -> None:
         """
         Initializes the state_mapping array which holds the observation values for each state
@@ -117,28 +117,26 @@
         in order to define the transitions of the environment
         """
         self.left_possible = [1, 2, 3, 13, 14, 15]
         self.down_possible = [0, 4, 8, 3, 7, 11]
         self.right_possible = [0, 1, 2, 12, 13, 14]
         self.up_possible = [4, 8, 12, 7, 11, 15]
 
-    def step(self, action: Union[float, np.ndarray]) -> GymStepReturn:
+    def step(self, action: Union[int, np.ndarray]) -> GymStepReturn:
         """
         Run one timestep of the environment's dynamics. When end of
         episode is reached, you are responsible for calling `reset()`
         to reset this environment's state.
-        Accepts an action and returns a tuple (observation, reward, done, info).
+        Accepts an action and returns a tuple (observation, reward, terminated, truncated, info).
 
         :param action:
-        :return: tuple (observation, reward, done, info).
+        :return: tuple (observation, reward, terminated, truncated, info).
         """
         if not self.discrete_actions:
-            action = np.argmax(action)
-        else:
-            action = int(action)
+            action = np.argmax(action)  # type: ignore[assignment]
 
         self.count += 1
 
         prev_state = self.state
 
         reward = -0.1
         # define state transition
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/evaluation.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/evaluation.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/logger.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import json
 import os
 import sys
 import tempfile
 import warnings
 from collections import defaultdict
+from io import TextIOBase
 from typing import Any, Dict, List, Mapping, Optional, Sequence, TextIO, Tuple, Union
 
 import numpy as np
 import pandas
 import torch as th
 from matplotlib import pyplot as plt
 
@@ -109,15 +110,15 @@
 
 
 class KVWriter:
     """
     Key Value writer
     """
 
-    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Union[str, Tuple[str, ...]]], step: int = 0) -> None:
+    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], step: int = 0) -> None:
         """
         Write a dictionary to file
 
         :param key_values:
         :param key_excluded:
         :param step:
         """
@@ -131,15 +132,15 @@
 
 
 class SeqWriter:
     """
     sequence writer
     """
 
-    def write_sequence(self, sequence: List) -> None:
+    def write_sequence(self, sequence: List[str]) -> None:
         """
         write_sequence an array to file
 
         :param sequence:
         """
         raise NotImplementedError
 
@@ -159,23 +160,24 @@
     """
 
     def __init__(self, filename_or_file: Union[str, TextIO], max_length: int = 36):
         self.max_length = max_length
         if isinstance(filename_or_file, str):
             self.file = open(filename_or_file, "w")
             self.own_file = True
-        else:
-            assert hasattr(filename_or_file, "write"), f"Expected file or str, got {filename_or_file}"
+        elif isinstance(filename_or_file, TextIOBase):
             self.file = filename_or_file
             self.own_file = False
+        else:
+            raise ValueError(f"Expected file or str, got {filename_or_file}")
 
-    def write(self, key_values: Dict, key_excluded: Dict, step: int = 0) -> None:
+    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], step: int = 0) -> None:
         # Create strings for printing
         key2str = {}
-        tag = None
+        tag = ""
         for (key, value), (_, excluded) in zip(sorted(key_values.items()), sorted(key_excluded.items())):
             if excluded is not None and ("stdout" in excluded or "log" in excluded):
                 continue
 
             elif isinstance(value, Video):
                 raise FormatUnsupportedError(["stdout", "log"], "video")
 
@@ -193,17 +195,17 @@
                 value_str = f"{value:<8.3g}"
             else:
                 value_str = str(value)
 
             if key.find("/") > 0:  # Find tag and add it to the dict
                 tag = key[: key.find("/") + 1]
                 key2str[(tag, self._truncate(tag))] = ""
-            # Remove tag from key
-            if tag is not None and tag in key:
-                key = str("   " + key[len(tag) :])
+            # Remove tag from key and indent the key
+            if len(tag) > 0 and tag in key:
+                key = f"{'':3}{key[len(tag) :]}"
 
             truncated_key = self._truncate(key)
             if (tag, truncated_key) in key2str:
                 raise ValueError(
                     f"Key '{key}' truncated to '{truncated_key}' that already exists. Consider increasing `max_length`."
                 )
             key2str[(tag, truncated_key)] = self._truncate(value_str)
@@ -236,16 +238,15 @@
         self.file.flush()
 
     def _truncate(self, string: str) -> str:
         if len(string) > self.max_length:
             string = string[: self.max_length - 3] + "..."
         return string
 
-    def write_sequence(self, sequence: List) -> None:
-        sequence = list(sequence)
+    def write_sequence(self, sequence: List[str]) -> None:
         for i, elem in enumerate(sequence):
             self.file.write(elem)
             if i < len(sequence) - 1:  # add space unless this is the last one
                 self.file.write(" ")
         self.file.write("\n")
         self.file.flush()
 
@@ -253,17 +254,15 @@
         """
         closes the file
         """
         if self.own_file:
             self.file.close()
 
 
-def filter_excluded_keys(
-    key_values: Dict[str, Any], key_excluded: Dict[str, Union[str, Tuple[str, ...]]], _format: str
-) -> Dict[str, Any]:
+def filter_excluded_keys(key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], _format: str) -> Dict[str, Any]:
     """
     Filters the keys specified by ``key_exclude`` for the specified format
 
     :param key_values: log dictionary to be filtered
     :param key_excluded: keys to be excluded per format
     :param _format: format for which this filter is run
     :return: dict without the excluded keys
@@ -281,15 +280,15 @@
 
     :param filename: the file to write the log to
     """
 
     def __init__(self, filename: str):
         self.file = open(filename, "w")
 
-    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Union[str, Tuple[str, ...]]], step: int = 0) -> None:
+    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], step: int = 0) -> None:
         def cast_to_json_serializable(value: Any):
             if isinstance(value, Video):
                 raise FormatUnsupportedError(["json"], "video")
             if isinstance(value, Figure):
                 raise FormatUnsupportedError(["json"], "figure")
             if isinstance(value, Image):
                 raise FormatUnsupportedError(["json"], "image")
@@ -328,15 +327,15 @@
 
     def __init__(self, filename: str):
         self.file = open(filename, "w+t")
         self.keys: List[str] = []
         self.separator = ","
         self.quotechar = '"'
 
-    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Union[str, Tuple[str, ...]]], step: int = 0) -> None:
+    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], step: int = 0) -> None:
         # Add our current row to the history
         key_values = filter_excluded_keys(key_values, key_excluded, "csv")
         extra_keys = key_values.keys() - self.keys
         if extra_keys:
             self.keys.extend(extra_keys)
             self.file.seek(0)
             lines = self.file.readlines()
@@ -390,18 +389,20 @@
     """
     Dumps key/value pairs into TensorBoard's numeric format.
 
     :param folder: the folder to write the log to
     """
 
     def __init__(self, folder: str):
-        assert SummaryWriter is not None, "tensorboard is not installed, you can use " "pip install tensorboard to do so"
+        assert SummaryWriter is not None, "tensorboard is not installed, you can use `pip install tensorboard` to do so"
         self.writer = SummaryWriter(log_dir=folder)
+        self._is_closed = False
 
-    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Union[str, Tuple[str, ...]]], step: int = 0) -> None:
+    def write(self, key_values: Dict[str, Any], key_excluded: Dict[str, Tuple[str, ...]], step: int = 0) -> None:
+        assert not self._is_closed, "The SummaryWriter was closed, please re-create one."
         for (key, value), (_, excluded) in zip(sorted(key_values.items()), sorted(key_excluded.items())):
             if excluded is not None and "tensorboard" in excluded:
                 continue
 
             if isinstance(value, np.ScalarType):
                 if isinstance(value, str):
                     # str is considered a np.ScalarType
@@ -433,15 +434,15 @@
 
     def close(self) -> None:
         """
         closes the file
         """
         if self.writer:
             self.writer.close()
-            self.writer = None
+            self._is_closed = True
 
 
 def make_output_format(_format: str, log_dir: str, log_suffix: str = "") -> KVWriter:
     """
     return a logger for the requested format
 
     :param _format: the requested format to log to ('stdout', 'log', 'json' or 'csv' or 'tensorboard')
@@ -474,49 +475,59 @@
     The logger class.
 
     :param folder: the logging location
     :param output_formats: the list of output formats
     """
 
     def __init__(self, folder: Optional[str], output_formats: List[KVWriter]):
-        self.name_to_value = defaultdict(float)  # values this iteration
-        self.name_to_count = defaultdict(int)
-        self.name_to_excluded = defaultdict(str)
+        self.name_to_value: Dict[str, float] = defaultdict(float)  # values this iteration
+        self.name_to_count: Dict[str, int] = defaultdict(int)
+        self.name_to_excluded: Dict[str, Tuple[str, ...]] = {}
         self.level = INFO
         self.dir = folder
         self.output_formats = output_formats
 
+    @staticmethod
+    def to_tuple(string_or_tuple: Optional[Union[str, Tuple[str, ...]]]) -> Tuple[str, ...]:
+        """
+        Helper function to convert str to tuple of str.
+        """
+        if string_or_tuple is None:
+            return ("",)
+        if isinstance(string_or_tuple, tuple):
+            return string_or_tuple
+        return (string_or_tuple,)
+
     def record(self, key: str, value: Any, exclude: Optional[Union[str, Tuple[str, ...]]] = None) -> None:
         """
         Log a value of some diagnostic
         Call this once for each diagnostic quantity, each iteration
         If called many times, last value will be used.
 
         :param key: save to log this key
         :param value: save to log this value
         :param exclude: outputs to be excluded
         """
         self.name_to_value[key] = value
-        self.name_to_excluded[key] = exclude
+        self.name_to_excluded[key] = self.to_tuple(exclude)
 
-    def record_mean(self, key: str, value: Any, exclude: Optional[Union[str, Tuple[str, ...]]] = None) -> None:
+    def record_mean(self, key: str, value: Optional[float], exclude: Optional[Union[str, Tuple[str, ...]]] = None) -> None:
         """
         The same as record(), but if called many times, values averaged.
 
         :param key: save to log this key
         :param value: save to log this value
         :param exclude: outputs to be excluded
         """
         if value is None:
-            self.name_to_value[key] = None
             return
         old_val, count = self.name_to_value[key], self.name_to_count[key]
         self.name_to_value[key] = old_val * count / (count + 1) + value / (count + 1)
         self.name_to_count[key] = count + 1
-        self.name_to_excluded[key] = exclude
+        self.name_to_excluded[key] = self.to_tuple(exclude)
 
     def dump(self, step: int = 0) -> None:
         """
         Write all of the diagnostics from the current iteration
         """
         if self.level == DISABLED:
             return
@@ -588,15 +599,15 @@
         """
         Set logging threshold on current logger.
 
         :param level: the logging level (can be DEBUG=10, INFO=20, WARN=30, ERROR=40, DISABLED=50)
         """
         self.level = level
 
-    def get_dir(self) -> str:
+    def get_dir(self) -> Optional[str]:
         """
         Get directory that log files are being written to.
         will be None if there is no output directory (i.e., if you didn't call start)
 
         :return: the logging directory
         """
         return self.dir
@@ -606,23 +617,23 @@
         closes the file
         """
         for _format in self.output_formats:
             _format.close()
 
     # Misc
     # ----------------------------------------
-    def _do_log(self, args) -> None:
+    def _do_log(self, args: Tuple[Any, ...]) -> None:
         """
         log to the requested format outputs
 
         :param args: the arguments to log
         """
         for _format in self.output_formats:
             if isinstance(_format, SeqWriter):
-                _format.write_sequence(map(str, args))
+                _format.write_sequence(list(map(str, args)))
 
 
 def configure(folder: Optional[str] = None, format_strings: Optional[List[str]] = None) -> Logger:
     """
     Configure the current logger.
 
     :param folder: the save location
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/monitor.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/noise.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         if indices is None:
             indices = range(len(self.noises))
 
         for index in indices:
             self.noises[index].reset()
 
     def __repr__(self) -> str:
-        return f"VecNoise(BaseNoise={repr(self.base_noise)}), n_envs={len(self.noises)})"
+        return f"VecNoise(BaseNoise={self.base_noise!r}), n_envs={len(self.noises)})"
 
     def __call__(self) -> np.ndarray:
         """
         Generate and stack the action noise from each noise object.
         """
         noise = np.stack([noise() for noise in self.noises])
         return noise
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/off_policy_algorithm.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/off_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/on_policy_algorithm.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/on_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/policies.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/preprocessing.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/results_plotter.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/results_plotter.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/running_mean_std.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/save_util.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/save_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def __setstate__(self, state: Dict[str, Any]) -> None:
         super().__setstate__(state)
         for group in self.param_groups:
             group.setdefault("momentum", 0)
             group.setdefault("centered", False)
 
     @torch.no_grad()
-    def step(self, closure: Optional[Callable[[], None]] = None) -> Optional[torch.Tensor]:
+    def step(self, closure: Optional[Callable[[], float]] = None) -> Optional[float]:
         """Performs a single optimization step.
 
         :param closure: A closure that reevaluates the model
             and returns the loss.
         :return: loss
         """
         loss = None
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/torch_layers.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/torch_layers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/type_aliases.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/type_aliases.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/utils.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import glob
 import os
 import platform
 import random
 import re
 from collections import deque
-from inspect import signature
 from itertools import zip_longest
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import cloudpickle
 import gymnasium as gym
 import numpy as np
 import torch as th
@@ -545,22 +544,7 @@
 
     env_info_str = ""
     for key, value in env_info.items():
         env_info_str += f"- {key}: {value}\n"
     if print_info:
         print(env_info_str)
     return env_info, env_info_str
-
-
-def compat_gym_seed(env: GymEnv, seed: int) -> None:
-    """
-    Compatibility helper to seed Gym envs.
-
-    :param env: The Gym environment.
-    :param seed: The seed for the pseudo random generator
-    """
-    if "seed" in signature(env.unwrapped.reset).parameters:
-        # gym >= 0.23.1
-        env.reset(seed=seed)
-    else:
-        # VecEnv and backward compatibility
-        env.seed(seed)
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/__init__.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/base_vec_env.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/base_vec_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 # it contains the observation for each env
 VecEnvObs = Union[np.ndarray, Dict[str, np.ndarray], Tuple[np.ndarray, ...]]
 # VecEnvStepReturn is what is returned by the step() method
 # it contains the observation, reward, done, info for each env
 VecEnvStepReturn = Tuple[VecEnvObs, np.ndarray, np.ndarray, List[Dict]]
 
 
-def tile_images(img_nhwc: Sequence[np.ndarray]) -> np.ndarray:  # pragma: no cover
+def tile_images(images_nhwc: Sequence[np.ndarray]) -> np.ndarray:  # pragma: no cover
     """
     Tile N images into one big PxQ image
     (P,Q) are chosen to be as close as possible, and if N
     is square, then P=Q.
 
-    :param img_nhwc: list or array of images, ndim=4 once turned into array. img nhwc
+    :param images_nhwc: list or array of images, ndim=4 once turned into array.
         n = batch index, h = height, w = width, c = channel
     :return: img_HWc, ndim=3
     """
-    img_nhwc = np.asarray(img_nhwc)
+    img_nhwc = np.asarray(images_nhwc)
     n_images, height, width, n_channels = img_nhwc.shape
     # new_height was named H before
     new_height = int(np.ceil(np.sqrt(n_images)))
     # new_width was named W before
     new_width = int(np.ceil(float(n_images) / new_height))
     img_nhwc = np.array(list(img_nhwc) + [img_nhwc[0] * 0 for _ in range(n_images, new_height * new_width)])
     # img_HWhwc
@@ -63,15 +63,24 @@
         action_space: spaces.Space,
         render_mode: Optional[str] = None,
     ):
         self.num_envs = num_envs
         self.observation_space = observation_space
         self.action_space = action_space
         self.render_mode = render_mode
-        self.reset_infos = [{} for _ in range(num_envs)]  # store info returned by the reset method
+        # store info returned by the reset method
+        self.reset_infos: List[Dict[str, Any]] = [{} for _ in range(num_envs)]
+        # seeds to be used in the next call to env.reset()
+        self._seeds: List[Optional[int]] = [None for _ in range(num_envs)]
+
+    def _reset_seeds(self) -> None:
+        """
+        Reset the seeds that are going to be used at the next reset.
+        """
+        self._seeds = [None for _ in range(self.num_envs)]
 
     @abstractmethod
     def reset(self) -> VecEnvObs:
         """
         Reset all the environments and return an array of
         observations, or a tuple of observation arrays.
 
@@ -188,42 +197,42 @@
             # we can still display that image using opencv
             if self.render_mode != "rgb_array":
                 warnings.warn(
                     f"You tried to render a VecEnv with mode='{mode}' "
                     "but the render mode defined when initializing the environment must be "
                     f"'human' or 'rgb_array', not '{self.render_mode}'."
                 )
-                return
+                return None
 
         elif mode and self.render_mode != mode:
             warnings.warn(
                 f"""Starting from gymnasium v0.26, render modes are determined during the initialization of the environment.
                 We allow to pass a mode argument to maintain a backwards compatible VecEnv API, but the mode ({mode})
                 has to be the same as the environment render mode ({self.render_mode}) which is not the case."""
             )
-            return
+            return None
 
         mode = mode or self.render_mode
 
         if mode is None:
             warnings.warn("You tried to call render() but no `render_mode` was passed to the env constructor.")
-            return
+            return None
 
         # mode == self.render_mode == "human"
         # In that case, we try to call `self.env.render()` but it might
         # crash for subprocesses
         if self.render_mode == "human":
             self.env_method("render")
-            return
+            return None
 
         if mode == "rgb_array" or mode == "human":
             # call the render method of the environments
             images = self.get_images()
             # Create a big image by tiling images from subprocesses
-            bigimg = tile_images(images)
+            bigimg = tile_images(images)  # type: ignore[arg-type]
 
             if mode == "human":
                 # Display it using OpenCV
                 import cv2  # pytype:disable=import-error
 
                 cv2.imshow("vecenv", bigimg[:, :, ::-1])
                 cv2.waitKey(1)
@@ -232,26 +241,34 @@
 
         else:
             # Other render modes:
             # In that case, we try to call `self.env.render()` but it might
             # crash for subprocesses
             # and we don't return the values
             self.env_method("render")
+        return None
 
-    @abstractmethod
-    def seed(self, seed: Optional[int] = None) -> List[Union[None, int]]:
+    def seed(self, seed: Optional[int] = None) -> Sequence[Union[None, int]]:
         """
         Sets the random seeds for all environments, based on a given seed.
         Each individual environment will still get its own seed, by incrementing the given seed.
+        WARNING: since gym 0.26, those seeds will only be passed to the environment
+        at the next reset.
 
         :param seed: The random seed. May be None for completely random seeding.
         :return: Returns a list containing the seeds for each individual env.
             Note that all list elements may be None, if the env does not return anything when being seeded.
         """
-        pass
+        if seed is None:
+            # To ensure that subprocesses have different seeds,
+            # we still populate the seed variable when no argument is passed
+            seed = np.random.randint(0, 2**32 - 1)
+
+        self._seeds = [seed + idx for idx in range(self.num_envs)]
+        return self._seeds
 
     @property
     def unwrapped(self) -> "VecEnv":
         if isinstance(self, VecEnvWrapper):
             return self.venv.unwrapped
         else:
             return self
@@ -315,15 +332,15 @@
     def reset(self) -> VecEnvObs:
         pass
 
     @abstractmethod
     def step_wait(self) -> VecEnvStepReturn:
         pass
 
-    def seed(self, seed: Optional[int] = None) -> List[Union[None, int]]:
+    def seed(self, seed: Optional[int] = None) -> Sequence[Union[None, int]]:
         return self.venv.seed(seed)
 
     def close(self) -> None:
         return self.venv.close()
 
     def render(self, mode: Optional[str] = None) -> Optional[np.ndarray]:
         return self.venv.render(mode=mode)
@@ -390,15 +407,15 @@
         """See base class.
 
         :return: name of module whose attribute is being shadowed, if any.
         """
         all_attributes = self._get_all_attributes()
         if name in all_attributes and already_found:
             # this venv's attribute is being hidden because of a higher venv.
-            shadowed_wrapper_class = f"{type(self).__module__}.{type(self).__name__}"
+            shadowed_wrapper_class: Optional[str] = f"{type(self).__module__}.{type(self).__name__}"
         elif name in all_attributes and not already_found:
             # we have found the first reference to the attribute. Now check for duplicates.
             shadowed_wrapper_class = self.venv.getattr_depth_check(name, True)
         else:
             # this wrapper does not have the attribute. Keep searching.
             shadowed_wrapper_class = self.venv.getattr_depth_check(name, already_found)
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/dummy_vec_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 from collections import OrderedDict
 from copy import deepcopy
-from typing import Any, Callable, List, Optional, Sequence, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Type
 
 import gymnasium as gym
 import numpy as np
 
 from stable_baselines3.common.vec_env.base_vec_env import VecEnv, VecEnvIndices, VecEnvObs, VecEnvStepReturn
 from stable_baselines3.common.vec_env.patch_gym import _patch_env
 from stable_baselines3.common.vec_env.util import copy_obs_dict, dict_to_obs, obs_space_info
@@ -20,14 +20,16 @@
     require a vectorized environment, but that you want a single environments to train with.
 
     :param env_fns: a list of functions
         that return environments to vectorize
     :raises ValueError: If the same environment instance is passed as the output of two or more different env_fn.
     """
 
+    actions: np.ndarray
+
     def __init__(self, env_fns: List[Callable[[], gym.Env]]):
         self.envs = [_patch_env(fn()) for fn in env_fns]
         if len(set([id(env.unwrapped) for env in self.envs])) != len(self.envs):
             raise ValueError(
                 "You tried to create multiple environments, but the function to create them returned the same instance "
                 "instead of creating different objects. "
                 "You are probably using `make_vec_env(lambda: env)` or `DummyVecEnv([lambda: env] * n_envs)`. "
@@ -40,16 +42,15 @@
         VecEnv.__init__(self, len(env_fns), env.observation_space, env.action_space, env.render_mode)
         obs_space = env.observation_space
         self.keys, shapes, dtypes = obs_space_info(obs_space)
 
         self.buf_obs = OrderedDict([(k, np.zeros((self.num_envs, *tuple(shapes[k])), dtype=dtypes[k])) for k in self.keys])
         self.buf_dones = np.zeros((self.num_envs,), dtype=bool)
         self.buf_rews = np.zeros((self.num_envs,), dtype=np.float32)
-        self.buf_infos = [{} for _ in range(self.num_envs)]
-        self.actions = None
+        self.buf_infos: List[Dict[str, Any]] = [{} for _ in range(self.num_envs)]
         self.metadata = env.metadata
 
     def step_async(self, actions: np.ndarray) -> None:
         self.actions = actions
 
     def step_wait(self) -> VecEnvStepReturn:
         # Avoid circular imports
@@ -66,42 +67,33 @@
             if self.buf_dones[env_idx]:
                 # save final observation where user can get it, then reset
                 self.buf_infos[env_idx]["terminal_observation"] = obs
                 obs, self.reset_infos[env_idx] = self.envs[env_idx].reset()
             self._save_obs(env_idx, obs)
         return (self._obs_from_buf(), np.copy(self.buf_rews), np.copy(self.buf_dones), deepcopy(self.buf_infos))
 
-    def seed(self, seed: Optional[int] = None) -> List[Union[None, int]]:
-        # Avoid circular import
-        from stable_baselines3.common.utils import compat_gym_seed
-
-        if seed is None:
-            seed = np.random.randint(0, 2**32 - 1)
-        seeds = []
-        for idx, env in enumerate(self.envs):
-            seeds.append(compat_gym_seed(env, seed=seed + idx))
-        return seeds
-
     def reset(self) -> VecEnvObs:
         for env_idx in range(self.num_envs):
-            obs, self.reset_infos[env_idx] = self.envs[env_idx].reset()
+            obs, self.reset_infos[env_idx] = self.envs[env_idx].reset(seed=self._seeds[env_idx])
             self._save_obs(env_idx, obs)
+        # Seeds are only used once
+        self._reset_seeds()
         return self._obs_from_buf()
 
     def close(self) -> None:
         for env in self.envs:
             env.close()
 
     def get_images(self) -> Sequence[Optional[np.ndarray]]:
         if self.render_mode != "rgb_array":
             warnings.warn(
                 f"The render mode is {self.render_mode}, but this method assumes it is `rgb_array` to obtain images."
             )
             return [None for _ in self.envs]
-        return [env.render() for env in self.envs]
+        return [env.render() for env in self.envs]  # type: ignore[misc]
 
     def render(self, mode: Optional[str] = None) -> Optional[np.ndarray]:
         """
         Gym environment rendering. If there are multiple environments then
         they are tiled together in one image via ``BaseVecEnv.render()``.
 
         :param mode: The rendering type.
@@ -109,15 +101,15 @@
         return super().render(mode=mode)
 
     def _save_obs(self, env_idx: int, obs: VecEnvObs) -> None:
         for key in self.keys:
             if key is None:
                 self.buf_obs[key][env_idx] = obs
             else:
-                self.buf_obs[key][env_idx] = obs[key]
+                self.buf_obs[key][env_idx] = obs[key]  # type: ignore[call-overload]
 
     def _obs_from_buf(self) -> VecEnvObs:
         return dict_to_obs(self.observation_space, copy_obs_dict(self.buf_obs))
 
     def get_attr(self, attr_name: str, indices: VecEnvIndices = None) -> List[Any]:
         """Return attribute from vectorized environment (see base class)."""
         target_envs = self._get_target_envs(indices)
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/patch_gym.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/patch_gym.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/stacked_observations.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/stacked_observations.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/subproc_vec_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import multiprocessing as mp
 import warnings
 from collections import OrderedDict
-from typing import Any, Callable, List, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
 
 from stable_baselines3.common.vec_env.base_vec_env import (
     CloudpickleWrapper,
@@ -20,36 +20,33 @@
 def _worker(
     remote: mp.connection.Connection,
     parent_remote: mp.connection.Connection,
     env_fn_wrapper: CloudpickleWrapper,
 ) -> None:
     # Import here to avoid a circular import
     from stable_baselines3.common.env_util import is_wrapped
-    from stable_baselines3.common.utils import compat_gym_seed
 
     parent_remote.close()
     env = _patch_env(env_fn_wrapper.var())
-    reset_info = {}
+    reset_info: Optional[Dict[str, Any]] = {}
     while True:
         try:
             cmd, data = remote.recv()
             if cmd == "step":
                 observation, reward, terminated, truncated, info = env.step(data)
                 # convert to SB3 VecEnv api
                 done = terminated or truncated
                 info["TimeLimit.truncated"] = truncated and not terminated
                 if done:
                     # save final observation where user can get it, then reset
                     info["terminal_observation"] = observation
                     observation, reset_info = env.reset()
                 remote.send((observation, reward, done, info, reset_info))
-            elif cmd == "seed":
-                remote.send(compat_gym_seed(env, seed=data))
             elif cmd == "reset":
-                observation, reset_info = env.reset()
+                observation, reset_info = env.reset(seed=data)
                 remote.send((observation, reset_info))
             elif cmd == "render":
                 remote.send(env.render())
             elif cmd == "close":
                 env.close()
                 remote.close()
                 break
@@ -57,15 +54,15 @@
                 remote.send((env.observation_space, env.action_space))
             elif cmd == "env_method":
                 method = getattr(env, data[0])
                 remote.send(method(*data[1], **data[2]))
             elif cmd == "get_attr":
                 remote.send(getattr(env, data))
             elif cmd == "set_attr":
-                remote.send(setattr(env, data[0], data[1]))
+                remote.send(setattr(env, data[0], data[1]))  # type: ignore[func-returns-value]
             elif cmd == "is_wrapped":
                 remote.send(is_wrapped(env, data))
             else:
                 raise NotImplementedError(f"`{cmd}` is not implemented in the worker")
         except EOFError:
             break
 
@@ -108,15 +105,17 @@
         ctx = mp.get_context(start_method)
 
         self.remotes, self.work_remotes = zip(*[ctx.Pipe() for _ in range(n_envs)])
         self.processes = []
         for work_remote, remote, env_fn in zip(self.work_remotes, self.remotes, env_fns):
             args = (work_remote, remote, CloudpickleWrapper(env_fn))
             # daemon=True: if the main process crashes, we should not cause things to hang
-            process = ctx.Process(target=_worker, args=args, daemon=True)  # pytype:disable=attribute-error
+            # pytype: disable=attribute-error
+            process = ctx.Process(target=_worker, args=args, daemon=True)  # type: ignore[attr-defined]
+            # pytype: enable=attribute-error
             process.start()
             self.processes.append(process)
             work_remote.close()
 
         self.remotes[0].send(("get_spaces", None))
         observation_space, action_space = self.remotes[0].recv()
 
@@ -131,26 +130,21 @@
 
     def step_wait(self) -> VecEnvStepReturn:
         results = [remote.recv() for remote in self.remotes]
         self.waiting = False
         obs, rews, dones, infos, self.reset_infos = zip(*results)
         return _flatten_obs(obs, self.observation_space), np.stack(rews), np.stack(dones), infos
 
-    def seed(self, seed: Optional[int] = None) -> List[Union[None, int]]:
-        if seed is None:
-            seed = np.random.randint(0, 2**32 - 1)
-        for idx, remote in enumerate(self.remotes):
-            remote.send(("seed", seed + idx))
-        return [remote.recv() for remote in self.remotes]
-
     def reset(self) -> VecEnvObs:
-        for remote in self.remotes:
-            remote.send(("reset", None))
+        for env_idx, remote in enumerate(self.remotes):
+            remote.send(("reset", self._seeds[env_idx]))
         results = [remote.recv() for remote in self.remotes]
         obs, self.reset_infos = zip(*results)
+        # Seeds are only used once
+        self._reset_seeds()
         return _flatten_obs(obs, self.observation_space)
 
     def close(self) -> None:
         if self.closed:
             return
         if self.waiting:
             for remote in self.remotes:
@@ -231,10 +225,10 @@
     if isinstance(space, spaces.Dict):
         assert isinstance(space.spaces, OrderedDict), "Dict space must have ordered subspaces"
         assert isinstance(obs[0], dict), "non-dict observation for environment with Dict observation space"
         return OrderedDict([(k, np.stack([o[k] for o in obs])) for k in space.spaces.keys()])
     elif isinstance(space, spaces.Tuple):
         assert isinstance(obs[0], tuple), "non-tuple observation for environment with Tuple observation space"
         obs_len = len(space.spaces)
-        return tuple(np.stack([o[i] for o in obs]) for i in range(obs_len))
+        return tuple(np.stack([o[i] for o in obs]) for i in range(obs_len))  # type: ignore[index]
     else:
-        return np.stack(obs)
+        return np.stack(obs)  # type: ignore[arg-type]
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/util.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         dtypes: a dict mapping keys to dtypes.
     """
     check_for_nested_spaces(obs_space)
     if isinstance(obs_space, spaces.Dict):
         assert isinstance(obs_space.spaces, OrderedDict), "Dict space must have ordered subspaces"
         subspaces = obs_space.spaces
     elif isinstance(obs_space, spaces.Tuple):
-        subspaces = {i: space for i, space in enumerate(obs_space.spaces)}
+        subspaces = {i: space for i, space in enumerate(obs_space.spaces)}  # type: ignore[assignment]
     else:
         assert not hasattr(obs_space, "spaces"), f"Unsupported structured space '{type(obs_space)}'"
-        subspaces = {None: obs_space}
+        subspaces = {None: obs_space}  # type: ignore[assignment]
     keys = []
     shapes = {}
     dtypes = {}
     for key, box in subspaces.items():
         keys.append(key)
         shapes[key] = box.shape
         dtypes[key] = box.dtype
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_check_nan.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_frame_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         observation_space = self.stacked_obs.stacked_observation_space
         super().__init__(venv, observation_space=observation_space)
 
     def step_wait(
         self,
     ) -> Tuple[Union[np.ndarray, Dict[str, np.ndarray]], np.ndarray, np.ndarray, List[Dict[str, Any]],]:
         observations, rewards, dones, infos = self.venv.step_wait()
-        observations, infos = self.stacked_obs.update(observations, dones, infos)
+        observations, infos = self.stacked_obs.update(observations, dones, infos)  # type: ignore[arg-type]
         return observations, rewards, dones, infos
 
     def reset(self) -> Union[np.ndarray, Dict[str, np.ndarray]]:
         """
         Reset all environments
         """
         observation = self.venv.reset()  # pytype:disable=annotation-type-mismatch
-        observation = self.stacked_obs.reset(observation)
+        observation = self.stacked_obs.reset(observation)  # type: ignore[arg-type]
         return observation
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_monitor.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,30 +45,30 @@
                 "The environment is already wrapped with a `Monitor` wrapper"
                 "but you are wrapping it with a `VecMonitor` wrapper, the `Monitor` statistics will be"
                 "overwritten by the `VecMonitor` ones.",
                 UserWarning,
             )
 
         VecEnvWrapper.__init__(self, venv)
-        self.episode_returns = None
-        self.episode_lengths = None
         self.episode_count = 0
         self.t_start = time.time()
 
         env_id = None
         if hasattr(venv, "spec") and venv.spec is not None:
             env_id = venv.spec.id
 
+        self.results_writer: Optional[ResultsWriter] = None
         if filename:
             self.results_writer = ResultsWriter(
-                filename, header={"t_start": self.t_start, "env_id": env_id}, extra_keys=info_keywords
+                filename, header={"t_start": self.t_start, "env_id": str(env_id)}, extra_keys=info_keywords
             )
-        else:
-            self.results_writer = None
+
         self.info_keywords = info_keywords
+        self.episode_returns = np.zeros(self.num_envs, dtype=np.float32)
+        self.episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
 
     def reset(self) -> VecEnvObs:
         obs = self.venv.reset()
         self.episode_returns = np.zeros(self.num_envs, dtype=np.float32)
         self.episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
         return obs
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_normalize.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_transpose.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_transpose.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py` & `stable_baselines3-2.0.0a9/stable_baselines3/common/vec_env/vec_video_recorder.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/ddpg/ddpg.py` & `stable_baselines3-2.0.0a9/stable_baselines3/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/dqn/dqn.py` & `stable_baselines3-2.0.0a9/stable_baselines3/dqn/dqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,38 +147,37 @@
         self.batch_norm_stats = get_parameters_by_name(self.q_net, ["running_"])
         self.batch_norm_stats_target = get_parameters_by_name(self.q_net_target, ["running_"])
         self.exploration_schedule = get_linear_fn(
             self.exploration_initial_eps,
             self.exploration_final_eps,
             self.exploration_fraction,
         )
-        # Account for multiple environments
-        # each call to step() corresponds to n_envs transitions
+
         if self.n_envs > 1:
             if self.n_envs > self.target_update_interval:
                 warnings.warn(
                     "The number of environments used is greater than the target network "
                     f"update interval ({self.n_envs} > {self.target_update_interval}), "
                     "therefore the target network will be updated after each call to env.step() "
                     f"which corresponds to {self.n_envs} steps."
                 )
 
-            self.target_update_interval = max(self.target_update_interval // self.n_envs, 1)
-
     def _create_aliases(self) -> None:
         self.q_net = self.policy.q_net
         self.q_net_target = self.policy.q_net_target
 
     def _on_step(self) -> None:
         """
         Update the exploration rate and target network if needed.
         This method is called in ``collect_rollouts()`` after each step in the environment.
         """
         self._n_calls += 1
-        if self._n_calls % self.target_update_interval == 0:
+        # Account for multiple environments
+        # each call to step() corresponds to n_envs transitions
+        if self._n_calls % max(self.target_update_interval // self.n_envs, 1) == 0:
             polyak_update(self.q_net.parameters(), self.q_net_target.parameters(), self.tau)
             # Copy running stats, see GH issue #996
             polyak_update(self.batch_norm_stats, self.batch_norm_stats_target, 1.0)
 
         self.exploration_rate = self.exploration_schedule(self._current_progress_remaining)
         self.logger.record("rollout/exploration_rate", self.exploration_rate)
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/dqn/policies.py` & `stable_baselines3-2.0.0a9/stable_baselines3/dqn/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/her/goal_selection_strategy.py` & `stable_baselines3-2.0.0a9/stable_baselines3/her/goal_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/her/her_replay_buffer.py` & `stable_baselines3-2.0.0a9/stable_baselines3/her/her_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/ppo/ppo.py` & `stable_baselines3-2.0.0a9/stable_baselines3/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/sac/policies.py` & `stable_baselines3-2.0.0a9/stable_baselines3/sac/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/sac/sac.py` & `stable_baselines3-2.0.0a9/stable_baselines3/sac/sac.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/td3/policies.py` & `stable_baselines3-2.0.0a9/stable_baselines3/td3/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3/td3/td3.py` & `stable_baselines3-2.0.0a9/stable_baselines3/td3/td3.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/PKG-INFO` & `stable_baselines3-2.0.0a9/stable_baselines3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: stable-baselines3
-Version: 2.0.0a5
+Version: 2.0.0a9
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
 Project-URL: SB3-Contrib, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: RL-Zoo, https://github.com/DLR-RM/rl-baselines3-zoo
-Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
+Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gymnasium gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/SOURCES.txt` & `stable_baselines3-2.0.0a9/stable_baselines3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/requires.txt` & `stable_baselines3-2.0.0a9/stable_baselines3.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 gymnasium==0.28.1
-numpy
+numpy>=1.20
 torch>=1.11
 cloudpickle
 pandas
 matplotlib
 
 [:python_version < "3.8.0"]
 typing_extensions<5,>=4.0
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_buffers.py` & `stable_baselines3-2.0.0a9/tests/test_buffers.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.action_space = spaces.Box(1, 5, (1,))
         self.observation_space = spaces.Box(1, 5, (1,))
         self._observations = np.array([[1.0], [2.0], [3.0], [4.0], [5.0]], dtype=np.float32)
         self._rewards = [1, 2, 3, 4, 5]
         self._t = 0
         self._ep_length = 100
 
-    def reset(self):
+    def reset(self, *, seed=None, options=None):
         self._t = 0
         obs = self._observations[0]
         return obs, {}
 
     def step(self, action):
         self._t += 1
         index = self._t % len(self._observations)
@@ -51,15 +51,15 @@
         space = spaces.Box(1, 5, (1,))
         self.observation_space = spaces.Dict({"observation": space, "achieved_goal": space, "desired_goal": space})
         self._observations = np.array([[1.0], [2.0], [3.0], [4.0], [5.0]], dtype=np.float32)
         self._rewards = [1, 2, 3, 4, 5]
         self._t = 0
         self._ep_length = 100
 
-    def reset(self):
+    def reset(self, seed=None, options=None):
         self._t = 0
         obs = {key: self._observations[0] for key in self.observation_space.spaces.keys()}
         return obs, {}
 
     def step(self, action):
         self._t += 1
         index = self._t % len(self._observations)
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_callbacks.py` & `stable_baselines3-2.0.0a9/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_cnn.py` & `stable_baselines3-2.0.0a9/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_custom_policy.py` & `stable_baselines3-2.0.0a9/tests/test_custom_policy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_deterministic.py` & `stable_baselines3-2.0.0a9/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_dict_env.py` & `stable_baselines3-2.0.0a9/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_distributions.py` & `stable_baselines3-2.0.0a9/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_env_checker.py` & `stable_baselines3-2.0.0a9/tests/test_env_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         observation = np.array([1.0, 1.5, 0.5], dtype=self.observation_space.dtype)
         reward = 1
         terminated = True
         truncated = False
         info = {}
         return observation, reward, terminated, truncated, info
 
-    def reset(self):
+    def reset(self, seed=None):
         return np.array([1.0, 1.5, 0.5], dtype=self.observation_space.dtype), {}
 
     def render(self):
         pass
 
 
 def test_check_env_dict_action():
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_envs.py` & `stable_baselines3-2.0.0a9/tests/test_envs.py`

 * *Files 15% similar despite different names*

```diff
@@ -126,16 +126,20 @@
         # Non zero start index inside a Dict
         spaces.Dict({"obs": spaces.Discrete(3, start=1)}),
     ],
 )
 def test_non_default_spaces(new_obs_space):
     env = FakeImageEnv()
     env.observation_space = new_obs_space
+
     # Patch methods to avoid errors
-    env.reset = lambda: (new_obs_space.sample(), {})
+    def patched_reset(seed=None):
+        return new_obs_space.sample(), {}
+
+    env.reset = patched_reset
 
     def patched_step(_action):
         return new_obs_space.sample(), 0.0, False, False, {}
 
     env.step = patched_step
     with pytest.warns(UserWarning):
         check_env(env)
@@ -200,15 +204,15 @@
 def check_reset_assert_error(env, new_reset_return):
     """
     Helper to check that the error is caught.
     :param env: (gym.Env)
     :param new_reset_return: (Any)
     """
 
-    def wrong_reset():
+    def wrong_reset(seed=None):
         return new_reset_return, {}
 
     # Patch the reset method with a wrong one
     env.reset = wrong_reset
     with pytest.raises(AssertionError):
         check_env(env)
 
@@ -220,33 +224,44 @@
     env = IdentityEnvBox()
     # Return an observation that does not match the observation_space
     check_reset_assert_error(env, np.ones((3,)))
     # The observation is not a numpy array
     check_reset_assert_error(env, 1)
 
     # Return only obs (gym < 0.26)
-    env.reset = env.observation_space.sample
+    def wrong_reset(self, seed=None):
+        return env.observation_space.sample()
+
+    env.reset = types.MethodType(wrong_reset, env)
     with pytest.raises(AssertionError):
         check_env(env)
 
+    # No seed parameter (gym < 0.26)
+    def wrong_reset(self):
+        return env.observation_space.sample(), {}
+
+    env.reset = types.MethodType(wrong_reset, env)
+    with pytest.raises(TypeError):
+        check_env(env)
+
     # Return not only the observation
     check_reset_assert_error(env, (env.observation_space.sample(), False))
 
     env = SimpleMultiObsEnv()
 
     # Observation keys and observation space keys must match
     wrong_obs = env.observation_space.sample()
     wrong_obs.pop("img")
     check_reset_assert_error(env, wrong_obs)
     wrong_obs = {**env.observation_space.sample(), "extra_key": None}
     check_reset_assert_error(env, wrong_obs)
 
     obs, _ = env.reset()
 
-    def wrong_reset(self):
+    def wrong_reset(self, seed=None):
         return {"img": obs["img"], "vec": obs["img"]}, {}
 
     env.reset = types.MethodType(wrong_reset, env)
     with pytest.raises(AssertionError) as excinfo:
         check_env(env)
 
     # Check that the key is explicitly mentioned
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_gae.py` & `stable_baselines3-2.0.0a9/tests/test_gae.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_her.py` & `stable_baselines3-2.0.0a9/tests/test_her.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_identity.py` & `stable_baselines3-2.0.0a9/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_logger.py` & `stable_baselines3-2.0.0a9/tests/test_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib.util
 import os
 import sys
 import time
+from io import TextIOBase
 from typing import Sequence
 from unittest import mock
 
 import gymnasium as gym
 import numpy as np
 import pytest
 import torch as th
@@ -91,15 +92,15 @@
 
             acc = EventAccumulator(str(tmp_path))
             acc.Reload()
 
             tb_values_logged = []
             for reservoir in [acc.scalars, acc.tensors, acc.images, acc.histograms, acc.compressed_histograms]:
                 for k in reservoir.Keys():
-                    tb_values_logged.append(f"{k}: {str(reservoir.Items(k))}")
+                    tb_values_logged.append(f"{k}: {reservoir.Items(k)!s}")
 
             content = LogContent(_format, tb_values_logged)
             return content
 
     return read_fn
 
 
@@ -348,15 +349,15 @@
 
     def __init__(self, delay: float = 0.01):
         super().__init__()
         self.delay = delay
         self.observation_space = spaces.Box(low=-20.0, high=20.0, shape=(4,), dtype=np.float32)
         self.action_space = spaces.Discrete(2)
 
-    def reset(self):
+    def reset(self, seed=None):
         return self.observation_space.sample(), {}
 
     def step(self, action):
         time.sleep(self.delay)
         obs = self.observation_space.sample()
         return obs, 0.0, True, False, {}
 
@@ -430,7 +431,45 @@
 def test_ep_buffers_stats_window_size(algo, stats_window_size):
     """Set stats_window_size for logging to non-default value and check if
     ep_info_buffer and ep_success_buffer are initialized to the correct length"""
     model = algo("MlpPolicy", "CartPole-v1", stats_window_size=stats_window_size)
     model.learn(total_timesteps=10)
     assert model.ep_info_buffer.maxlen == stats_window_size
     assert model.ep_success_buffer.maxlen == stats_window_size
+
+
+def test_human_output_format_custom_test_io():
+    class DummyTextIO(TextIOBase):
+        def __init__(self) -> None:
+            super().__init__()
+            self.lines = [[]]
+
+        def write(self, t: str) -> int:
+            self.lines[-1].append(t)
+
+        def flush(self) -> None:
+            self.lines.append([])
+
+        def close(self) -> None:
+            pass
+
+        def get_printed(self) -> str:
+            return "\n".join(["".join(line) for line in self.lines])
+
+    dummy_text_io = DummyTextIO()
+    output = HumanOutputFormat(dummy_text_io)
+    output.write({"key1": "value1", "key2": 42}, {"key1": None, "key2": None})
+    output.write({"key1": "value2", "key2": 43}, {"key1": None, "key2": None})
+    printed = dummy_text_io.get_printed()
+    desired_printed = """-----------------
+| key1 | value1 |
+| key2 | 42     |
+-----------------
+
+-----------------
+| key1 | value2 |
+| key2 | 43     |
+-----------------
+
+"""
+
+    assert printed == desired_printed
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_monitor.py` & `stable_baselines3-2.0.0a9/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_predict.py` & `stable_baselines3-2.0.0a9/tests/test_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class CustomSubClassedSpaceEnv(gym.Env):
     def __init__(self):
         super().__init__()
         self.observation_space = SubClassedBox(-1, 1, shape=(2,), dtype=np.float32)
         self.action_space = SubClassedBox(-1, 1, shape=(2,), dtype=np.float32)
 
-    def reset(self):
+    def reset(self, seed=None):
         return self.observation_space.sample(), {}
 
     def step(self, action):
         return self.observation_space.sample(), 0.0, np.random.rand() > 0.5, False, {}
 
 
 @pytest.mark.parametrize("env_cls", [CustomSubClassedSpaceEnv])
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_preprocessing.py` & `stable_baselines3-2.0.0a9/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_run.py` & `stable_baselines3-2.0.0a9/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_save_load.py` & `stable_baselines3-2.0.0a9/tests/test_save_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import gymnasium as gym
 import numpy as np
 import pytest
 import torch as th
 
 from stable_baselines3 import A2C, DDPG, DQN, PPO, SAC, TD3
 from stable_baselines3.common.base_class import BaseAlgorithm
+from stable_baselines3.common.env_util import make_vec_env
 from stable_baselines3.common.envs import FakeImageEnv, IdentityEnv, IdentityEnvBox
 from stable_baselines3.common.save_util import load_from_pkl, open_path, save_to_pkl
 from stable_baselines3.common.utils import get_device
 from stable_baselines3.common.vec_env import DummyVecEnv
 
 MODEL_LIST = [PPO, A2C, TD3, SAC, DQN, DDPG]
 
@@ -726,7 +727,18 @@
     os.system(f"cd {tmp_path}; zip ppo_pendulum.zip data")
     with pytest.warns(UserWarning, match=r"custom_objects"):
         PPO.load(path)
     # Load with custom object, no warnings
     with warnings.catch_warnings(record=True) as record:
         PPO.load(path, custom_objects=dict(learning_rate=lambda _: 1.0))
     assert len(record) == 0
+
+
+def test_dqn_target_update_interval(tmp_path):
+    # `target_update_interval` should not change when reloading the model. See GH Issue #1373.
+    env = make_vec_env(env_id="CartPole-v1", n_envs=2)
+    model = DQN("MlpPolicy", env, verbose=1, target_update_interval=100)
+    model.save(tmp_path / "dqn_cartpole")
+    del model
+    model = DQN.load(tmp_path / "dqn_cartpole")
+    os.remove(tmp_path / "dqn_cartpole.zip")
+    assert model.target_update_interval == 100
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_sde.py` & `stable_baselines3-2.0.0a9/tests/test_sde.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_spaces.py` & `stable_baselines3-2.0.0a9/tests/test_spaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,26 @@
 
 class DummyMultidimensionalAction(gym.Env):
     def __init__(self):
         super().__init__()
         self.observation_space = spaces.Box(low=-1, high=1, shape=(2,), dtype=np.float32)
         self.action_space = spaces.Box(low=-1, high=1, shape=(2, 2), dtype=np.float32)
 
-    def reset(self):
+    def reset(self, *, seed: Optional[int] = None, options: Optional[Dict] = None):
+        if seed is not None:
+            super().reset(seed=seed)
         return self.observation_space.sample(), {}
 
     def step(self, action):
         return self.observation_space.sample(), 0.0, False, False, {}
 
 
-@pytest.mark.parametrize("env", [DummyMultiDiscreteSpace([4, 3]), DummyMultiBinary(8), DummyMultiBinary((3, 2))])
+@pytest.mark.parametrize(
+    "env", [DummyMultiDiscreteSpace([4, 3]), DummyMultiBinary(8), DummyMultiBinary((3, 2)), DummyMultidimensionalAction()]
+)
 def test_env(env):
     # Check the env used for testing
     check_env(env, skip_render_check=True)
 
 
 @pytest.mark.parametrize("model_class", [SAC, TD3, DQN])
 @pytest.mark.parametrize("env", [DummyMultiDiscreteSpace([4, 3]), DummyMultiBinary(8), DummyMultiBinary((3, 2))])
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_tensorboard.py` & `stable_baselines3-2.0.0a9/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_train_eval_mode.py` & `stable_baselines3-2.0.0a9/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_utils.py` & `stable_baselines3-2.0.0a9/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import stable_baselines3 as sb3
 from stable_baselines3 import A2C
 from stable_baselines3.common.atari_wrappers import MaxAndSkipEnv
 from stable_baselines3.common.env_util import is_wrapped, make_atari_env, make_vec_env, unwrap_wrapper
 from stable_baselines3.common.evaluation import evaluate_policy
 from stable_baselines3.common.monitor import Monitor
-from stable_baselines3.common.noise import ActionNoise, OrnsteinUhlenbeckActionNoise, VectorizedActionNoise
+from stable_baselines3.common.noise import OrnsteinUhlenbeckActionNoise, VectorizedActionNoise
 from stable_baselines3.common.utils import (
     check_shape_equal,
     get_parameters_by_name,
     get_system_info,
     is_vectorized_observation,
     polyak_update,
     zip_strict,
@@ -345,15 +345,15 @@
 
 
 def test_vec_noise():
     num_envs = 4
     num_actions = 10
     mu = np.zeros(num_actions)
     sigma = np.ones(num_actions) * 0.4
-    base: ActionNoise = OrnsteinUhlenbeckActionNoise(mu, sigma)
+    base = OrnsteinUhlenbeckActionNoise(mu, sigma)
     with pytest.raises(ValueError):
         vec = VectorizedActionNoise(base, -1)
     with pytest.raises(ValueError):
         vec = VectorizedActionNoise(base, None)
     with pytest.raises(ValueError):
         vec = VectorizedActionNoise(base, "whatever")
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_check_nan.py` & `stable_baselines3-2.0.0a9/tests/test_vec_check_nan.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from stable_baselines3.common.vec_env import DummyVecEnv, VecCheckNan
 
 
 class NanAndInfEnv(gym.Env):
     """Custom Environment that raised NaNs and Infs"""
 
-    metadata = {"render.modes": ["human"]}
+    metadata = {"render_modes": ["human"]}
 
     def __init__(self):
         super().__init__()
         self.action_space = spaces.Box(low=-np.inf, high=np.inf, shape=(1,), dtype=np.float64)
         self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(1,), dtype=np.float64)
 
     @staticmethod
@@ -23,15 +23,15 @@
         elif np.all(np.array(action) < 0):
             obs = float("inf")
         else:
             obs = 0
         return [obs], 0.0, False, False, {}
 
     @staticmethod
-    def reset():
+    def reset(seed=None):
         return [0.0], {}
 
     def render(self):
         pass
 
 
 def test_check_nan():
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_envs.py` & `stable_baselines3-2.0.0a9/tests/test_vec_envs.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """Gym environment for testing that terminal observation is inserted
         correctly."""
         self.action_space = spaces.Discrete(2)
         self.observation_space = spaces.Box(np.array([0]), np.array([999]), dtype="int")
         self.max_steps = max_steps
         self.current_step = 0
 
-    def reset(self):
+    def reset(self, *, seed: Optional[int] = None, options: Optional[Dict] = None):
         self.current_step = 0
         return np.array([self.current_step], dtype="int"), {}
 
     def step(self, action):
         prev_step = self.current_step
         self.current_step += 1
         terminated = False
@@ -472,28 +472,34 @@
     assert vec_env.env_is_wrapped(Monitor) == [False, True]
 
     vec_env = VecFrameStack(vec_env, n_stack=2)
     assert vec_env.env_is_wrapped(Monitor) == [False, True]
 
 
 @pytest.mark.parametrize("vec_env_class", VEC_ENV_CLASSES)
-def test_backward_compat_seed(vec_env_class):
+def test_vec_deterministic(vec_env_class):
     def make_env():
         env = CustomGymEnv(gym.spaces.Box(low=np.zeros(2), high=np.ones(2)))
-        # Patch reset function to remove seed param
-        env.reset = lambda: (env.observation_space.sample(), {})
-        env.seed = env.observation_space.seed
         return env
 
     vec_env = vec_env_class([make_env for _ in range(N_ENVS)])
     vec_env.seed(3)
     obs = vec_env.reset()
     vec_env.seed(3)
     new_obs = vec_env.reset()
     assert np.allclose(new_obs, obs)
+    vec_env.close()
+    # Similar test but with make_vec_env
+    vec_env_1 = make_vec_env("Pendulum-v1", n_envs=N_ENVS, vec_env_cls=vec_env_class, seed=0)
+    vec_env_2 = make_vec_env("Pendulum-v1", n_envs=N_ENVS, vec_env_cls=vec_env_class, seed=0)
+    assert np.allclose(vec_env_1.reset(), vec_env_2.reset())
+    random_actions = [vec_env_1.action_space.sample() for _ in range(N_ENVS)]
+    assert np.allclose(vec_env_1.step(random_actions)[0], vec_env_2.step(random_actions)[0])
+    vec_env_1.close()
+    vec_env_2.close()
 
 
 @pytest.mark.parametrize("vec_env_class", VEC_ENV_CLASSES)
 def test_vec_seeding(vec_env_class):
     def make_env():
         return CustomGymEnv(spaces.Box(low=np.zeros(2), high=np.ones(2)))
```

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_extract_dict_obs.py` & `stable_baselines3-2.0.0a9/tests/test_vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_monitor.py` & `stable_baselines3-2.0.0a9/tests/test_vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_normalize.py` & `stable_baselines3-2.0.0a9/tests/test_vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a5/tests/test_vec_stacked_obs.py` & `stable_baselines3-2.0.0a9/tests/test_vec_stacked_obs.py`

 * *Files identical despite different names*

