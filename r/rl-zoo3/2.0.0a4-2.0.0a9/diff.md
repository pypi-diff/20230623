# Comparing `tmp/rl_zoo3-2.0.0a4.tar.gz` & `tmp/rl_zoo3-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_zoo3-2.0.0a4.tar", last modified: Thu Apr 13 14:54:20 2023, max compression
+gzip compressed data, was "rl_zoo3-2.0.0a9.tar", last modified: Sat May 20 11:22:12 2023, max compression
```

## Comparing `rl_zoo3-2.0.0a4.tar` & `rl_zoo3-2.0.0a9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1071 2019-10-14 19:05:46.000000 rl_zoo3-2.0.0a4/LICENSE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15989 2023-04-12 16:11:03.000000 rl_zoo3-2.0.0a4/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1477 2023-04-12 16:21:41.000000 rl_zoo3-2.0.0a4/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.784656 rl_zoo3-2.0.0a4/rl_zoo3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      672 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7346 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/benchmark.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8726 2023-04-13 14:26:15.000000 rl_zoo3-2.0.0a4/rl_zoo3/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      668 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/cli.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10854 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/enjoy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    36245 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/exp_manager.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3516 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/gym_patches.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3594 2022-09-26 13:08:47.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/a2c.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4549 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ars.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3039 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ddpg.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1902 2022-12-11 16:01:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/dqn.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3685 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/her.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12265 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11593 2023-03-12 18:55:26.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo_lstm.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1809 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/qrdqn.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5879 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/sac.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3248 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/td3.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5772 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/tqc.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3850 2023-01-05 13:20:22.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/trpo.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20864 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams_opt.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1657 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/import_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4606 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/load_from_hub.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/rl_zoo3/plots/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      222 2023-01-25 22:48:07.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10790 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/all_plots.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18815 2023-02-13 13:49:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_from_file.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3485 2022-12-18 18:36:38.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2777 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/score_normalization.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15321 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/push_to_hub.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/py.typed
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7030 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/rl_zoo3/record_training.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6562 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/record_video.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11132 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17652 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 14:14:10.000000 rl_zoo3-2.0.0a4/rl_zoo3/version.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12272 2023-04-13 13:47:23.000000 rl_zoo3-2.0.0a4/rl_zoo3/wrappers.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.784656 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1296 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       45 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/entry_points.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      150 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.780656 rl_zoo3-2.0.0a4/scripts/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       90 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/all_plots.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      105 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/plot_from_file.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       93 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/plot_train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2174 2023-04-13 14:52:51.000000 rl_zoo3-2.0.0a4/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      490 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4499 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_enjoy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4817 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_hyperparams_opt.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4407 2023-04-12 16:18:57.000000 rl_zoo3-2.0.0a4/tests/test_train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1697 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_wrappers.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1071 2019-10-14 19:05:46.000000 rl_zoo3-2.0.0a9/LICENSE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15989 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1477 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.047400 rl_zoo3-2.0.0a9/rl_zoo3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      672 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7346 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a9/rl_zoo3/benchmark.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8726 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      668 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/rl_zoo3/cli.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10854 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/enjoy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    36242 2023-05-20 11:22:05.000000 rl_zoo3-2.0.0a9/rl_zoo3/exp_manager.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3516 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/gym_patches.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3594 2022-09-26 13:08:47.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/a2c.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4549 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ars.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3039 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ddpg.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1902 2022-12-11 16:01:58.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/dqn.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3685 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/her.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12277 2023-04-27 10:12:59.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ppo.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11605 2023-04-27 10:19:00.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ppo_lstm.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1809 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/qrdqn.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5885 2023-04-27 10:12:59.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/sac.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3248 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/td3.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5772 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/tqc.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3850 2023-01-05 13:20:22.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/trpo.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20864 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a9/rl_zoo3/hyperparams_opt.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1657 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/import_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4606 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/rl_zoo3/load_from_hub.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/rl_zoo3/plots/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      222 2023-01-25 22:48:07.000000 rl_zoo3-2.0.0a9/rl_zoo3/plots/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10790 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a9/rl_zoo3/plots/all_plots.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18815 2023-02-13 13:49:57.000000 rl_zoo3-2.0.0a9/rl_zoo3/plots/plot_from_file.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3485 2022-12-18 18:36:38.000000 rl_zoo3-2.0.0a9/rl_zoo3/plots/plot_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2777 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/rl_zoo3/plots/score_normalization.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15321 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a9/rl_zoo3/push_to_hub.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/rl_zoo3/py.typed
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7030 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a9/rl_zoo3/record_training.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6302 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/record_video.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11132 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17652 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-05-20 11:22:05.000000 rl_zoo3-2.0.0a9/rl_zoo3/version.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12272 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/rl_zoo3/wrappers.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.047400 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-05-20 11:22:11.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1296 2023-05-20 11:22:12.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-05-20 11:22:11.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       45 2023-05-20 11:22:11.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/entry_points.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      150 2023-05-20 11:22:11.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-05-20 11:22:11.000000 rl_zoo3-2.0.0a9/rl_zoo3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.043400 rl_zoo3-2.0.0a9/scripts/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       90 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/scripts/all_plots.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      105 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/scripts/plot_from_file.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       93 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a9/scripts/plot_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2174 2023-05-20 11:22:05.000000 rl_zoo3-2.0.0a9/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 11:22:12.051400 rl_zoo3-2.0.0a9/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      490 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a9/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4499 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/tests/test_enjoy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4817 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/tests/test_hyperparams_opt.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4407 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/tests/test_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1697 2023-04-14 12:07:02.000000 rl_zoo3-2.0.0a9/tests/test_wrappers.py
```

### Comparing `rl_zoo3-2.0.0a4/LICENSE` & `rl_zoo3-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/PKG-INFO` & `rl_zoo3-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl_zoo3
-Version: 2.0.0a4
+Version: 2.0.0a9
 Summary: A Training Framework for Stable Baselines3 Reinforcement Learning Agents
 Home-page: https://github.com/DLR-RM/rl-baselines3-zoo
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym gymnasium openai stable baselines sb3 toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rl_zoo3-2.0.0a4/README.md` & `rl_zoo3-2.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/pyproject.toml` & `rl_zoo3-2.0.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/__init__.py` & `rl_zoo3-2.0.0a9/rl_zoo3/__init__.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/benchmark.py` & `rl_zoo3-2.0.0a9/rl_zoo3/benchmark.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/callbacks.py` & `rl_zoo3-2.0.0a9/rl_zoo3/callbacks.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/cli.py` & `rl_zoo3-2.0.0a9/rl_zoo3/cli.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/enjoy.py` & `rl_zoo3-2.0.0a9/rl_zoo3/enjoy.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/exp_manager.py` & `rl_zoo3-2.0.0a9/rl_zoo3/exp_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
 
         optuna_eval_freq = int(self.n_timesteps / self.n_evaluations)
         # Account for parallel envs
         optuna_eval_freq = max(optuna_eval_freq // self.n_envs, 1)
         # Use non-deterministic eval for Atari
         path = None
         if self.optimization_log_path is not None:
-            path = os.path.join(self.optimization_log_path, f"trial_{str(trial.number)}")
+            path = os.path.join(self.optimization_log_path, f"trial_{trial.number!s}")
         callbacks = get_callback_list({"callback": self.specified_callbacks})
         eval_callback = TrialEvalCallback(
             eval_env,
             trial,
             best_model_save_path=path,
             log_path=path,
             n_eval_episodes=self.n_eval_episodes,
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/gym_patches.py` & `rl_zoo3-2.0.0a9/rl_zoo3/gym_patches.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/a2c.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/a2c.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ars.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ars.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ddpg.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ddpg.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/dqn.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/dqn.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/her.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/her.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ppo.yml`

 * *Files 0% similar despite different names*

```diff
@@ -343,21 +343,21 @@
   <<: *minigrid-defaults
 
 MiniGrid-ObstructedMaze-2Dlh-v0:
   <<: *minigrid-defaults
   n_timesteps: !!float 1e7 # Unsolved
 
 
-CarRacing-v1:
+CarRacing-v2:
   env_wrapper:
     - rl_zoo3.wrappers.FrameSkip:
         skip: 2
-    - gym.wrappers.resize_observation.ResizeObservation:
+    - gymnasium.wrappers.resize_observation.ResizeObservation:
         shape: 64
-    - gym.wrappers.gray_scale_observation.GrayScaleObservation:
+    - gymnasium.wrappers.gray_scale_observation.GrayScaleObservation:
         keep_dim: true
   frame_stack: 2
   normalize: "{'norm_obs': False, 'norm_reward': True}"
   n_envs: 8
   n_timesteps: !!float 4e6
   policy: 'CnnPolicy'
   batch_size: 128
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo_lstm.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/ppo_lstm.yml`

 * *Files 1% similar despite different names*

```diff
@@ -279,21 +279,21 @@
   gamma: 0.99
   n_epochs: 10
   ent_coef: 0.0
   learning_rate: 2.5e-4
   clip_range: 0.2
 
 
-CarRacing-v0:
+CarRacing-v2:
   env_wrapper:
     # - rl_zoo3.wrappers.FrameSkip:
     #     skip: 2
-    - gym.wrappers.resize_observation.ResizeObservation:
+    - gymnasium.wrappers.resize_observation.ResizeObservation:
         shape: 64
-    - gym.wrappers.gray_scale_observation.GrayScaleObservation:
+    - gymnasium.wrappers.gray_scale_observation.GrayScaleObservation:
         keep_dim: true
   frame_stack: 2
   normalize: "{'norm_obs': False, 'norm_reward': True}"
   n_envs: 8
   n_timesteps: !!float 4e6
   policy: 'CnnLstmPolicy'
   batch_size: 128
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/qrdqn.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/qrdqn.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/sac.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/sac.yml`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
   batch_size: 256
   ent_coef: 'auto'
   train_freq: 1
   gradient_steps: 1
   learning_starts: 10000
 
 # To be tuned
-CarRacing-v1:
+CarRacing-v2:
   env_wrapper:
     - rl_zoo3.wrappers.FrameSkip:
         skip: 2
     # wrapper from https://github.com/araffin/aae-train-donkeycar
     - ae.wrapper.AutoencoderWrapper:
         ae_path: "logs/car_racing_rgb_160.pkl"
     - rl_zoo3.wrappers.HistoryWrapper:
@@ -231,15 +231,15 @@
   policy_kwargs: "dict(net_arch=[64, 64])"
 
 
 # ==== Custom Envs ===
 
 donkey-generated-track-v0:
   env_wrapper:
-    - gym.wrappers.time_limit.TimeLimit:
+    - gymnasium.wrappers.time_limit.TimeLimit:
         max_episode_steps: 500
     - rl_zoo3.wrappers.HistoryWrapper:
         horizon: 5
   n_timesteps: !!float 1e6
   policy: 'MlpPolicy'
   learning_rate: !!float 7.3e-4
   buffer_size: 300000
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/td3.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/td3.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/tqc.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/tqc.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/trpo.yml` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams/trpo.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams_opt.py` & `rl_zoo3-2.0.0a9/rl_zoo3/hyperparams_opt.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/import_envs.py` & `rl_zoo3-2.0.0a9/rl_zoo3/import_envs.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/load_from_hub.py` & `rl_zoo3-2.0.0a9/rl_zoo3/load_from_hub.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/plots/all_plots.py` & `rl_zoo3-2.0.0a9/rl_zoo3/plots/all_plots.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_from_file.py` & `rl_zoo3-2.0.0a9/rl_zoo3/plots/plot_from_file.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_train.py` & `rl_zoo3-2.0.0a9/rl_zoo3/plots/plot_train.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/plots/score_normalization.py` & `rl_zoo3-2.0.0a9/rl_zoo3/plots/score_normalization.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/push_to_hub.py` & `rl_zoo3-2.0.0a9/rl_zoo3/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/record_training.py` & `rl_zoo3-2.0.0a9/rl_zoo3/record_training.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/record_video.py` & `rl_zoo3-2.0.0a9/rl_zoo3/record_video.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,20 +133,14 @@
     # Deterministic by default except for atari games
     stochastic = args.stochastic or (is_atari or is_minigrid) and not args.deterministic
     deterministic = not stochastic
 
     if video_folder is None:
         video_folder = os.path.join(log_path, "videos")
 
-    if is_atari:
-        # Patch Atari for rendering
-        # see https://github.com/mgbellemare/Arcade-Learning-Environment/issues/473
-        env.unwrapped.render_mode = env_kwargs.get("render_mode")
-        env.render_mode = env_kwargs.get("render_mode")
-
     # Note: apparently it renders by default
     env = VecVideoRecorder(
         env,
         video_folder,
         record_video_trigger=lambda x: x == 0,
         video_length=video_length,
         name_prefix=name_prefix,
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/train.py` & `rl_zoo3-2.0.0a9/rl_zoo3/train.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/utils.py` & `rl_zoo3-2.0.0a9/rl_zoo3/utils.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3/wrappers.py` & `rl_zoo3-2.0.0a9/rl_zoo3/wrappers.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3.egg-info/PKG-INFO` & `rl_zoo3-2.0.0a9/rl_zoo3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl-zoo3
-Version: 2.0.0a4
+Version: 2.0.0a9
 Summary: A Training Framework for Stable Baselines3 Reinforcement Learning Agents
 Home-page: https://github.com/DLR-RM/rl-baselines3-zoo
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym gymnasium openai stable baselines sb3 toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rl_zoo3-2.0.0a4/rl_zoo3.egg-info/SOURCES.txt` & `rl_zoo3-2.0.0a9/rl_zoo3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/setup.py` & `rl_zoo3-2.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "py.typed",
             "version.txt",
             "hyperparams/*.yml",
         ]
     },
     entry_points={"console_scripts": ["rl_zoo3=rl_zoo3.cli:main"]},
     install_requires=[
-        "sb3_contrib>=2.0.0a4",
+        "sb3_contrib>=2.0.0a9",
         "gym==0.26.2",
         "huggingface_sb3>=2.2.1",
         "tqdm",
         "rich",
         "optuna",
         "pyyaml>=5.1",
         "pytablewriter~=0.64",
```

### Comparing `rl_zoo3-2.0.0a4/tests/test_enjoy.py` & `rl_zoo3-2.0.0a9/tests/test_enjoy.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/tests/test_hyperparams_opt.py` & `rl_zoo3-2.0.0a9/tests/test_hyperparams_opt.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/tests/test_train.py` & `rl_zoo3-2.0.0a9/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-2.0.0a4/tests/test_wrappers.py` & `rl_zoo3-2.0.0a9/tests/test_wrappers.py`

 * *Files identical despite different names*

