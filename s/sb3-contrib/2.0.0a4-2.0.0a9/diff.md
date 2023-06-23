# Comparing `tmp/sb3_contrib-2.0.0a4.tar.gz` & `tmp/sb3_contrib-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb3_contrib-2.0.0a4.tar", last modified: Thu Apr 13 14:51:19 2023, max compression
+gzip compressed data, was "sb3_contrib-2.0.0a9.tar", last modified: Sat May 20 08:57:56 2023, max compression
```

## Comparing `sb3_contrib-2.0.0a4.tar` & `sb3_contrib-2.0.0a9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1078 2020-09-20 20:10:25.000000 sb3_contrib-2.0.0a4/LICENSE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3584 2022-11-28 21:39:26.000000 sb3_contrib-2.0.0a4/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1789 2023-04-13 14:13:11.000000 sb3_contrib-2.0.0a4/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      525 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/ars/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      145 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    16834 2023-04-13 14:13:09.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/ars.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4299 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-11-13 12:40:30.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      262 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4261 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/invalid_actions_env.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8740 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5744 2023-02-13 13:32:37.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11653 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7006 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    19187 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1080 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17764 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26968 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      778 2023-04-03 13:50:28.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7022 2023-04-03 13:03:38.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       85 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8405 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/async_eval.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1139 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/action_masker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4085 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/time_feature.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      208 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      294 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    24110 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/ppo_mask.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      249 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      313 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21599 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/ppo_recurrent.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2020-09-25 09:51:52.000000 sb3_contrib-2.0.0a4/sb3_contrib/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      187 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11417 2023-04-13 13:57:06.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14168 2023-04-13 13:57:14.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/qrdqn.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/tqc/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      177 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    23495 2023-04-13 14:23:36.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15637 2023-04-13 14:22:39.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/tqc.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/trpo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      182 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      302 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20271 2023-04-13 14:25:24.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/trpo.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 13:50:37.000000 sb3_contrib-2.0.0a4/sb3_contrib/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1893 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       27 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       12 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/top_level.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4146 2023-04-13 14:50:50.000000 sb3_contrib-2.0.0a4/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7675 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2385 2023-02-13 13:36:17.000000 sb3_contrib-2.0.0a4/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9174 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11090 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a4/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1366 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9645 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_invalid_actions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6862 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_lstm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4994 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17613 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9974 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2165 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a4/tests/test_utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.346022 sb3_contrib-2.0.0a9/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1078 2020-09-20 20:10:25.000000 sb3_contrib-2.0.0a9/LICENSE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-05-20 08:57:56.346022 sb3_contrib-2.0.0a9/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3584 2023-05-08 11:50:09.000000 sb3_contrib-2.0.0a9/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1528 2023-05-14 15:59:15.000000 sb3_contrib-2.0.0a9/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.314022 sb3_contrib-2.0.0a9/sb3_contrib/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      525 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.314022 sb3_contrib-2.0.0a9/sb3_contrib/ars/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      145 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/ars/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    16834 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/ars/ars.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4299 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/ars/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.314022 sb3_contrib-2.0.0a9/sb3_contrib/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-11-13 12:40:30.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.318022 sb3_contrib-2.0.0a9/sb3_contrib/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      262 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4376 2023-05-14 15:53:59.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/envs/invalid_actions_env.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.322022 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8740 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5744 2023-02-13 13:32:37.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11653 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7006 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    19187 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1080 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.326022 sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17764 2023-04-27 10:09:44.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26968 2023-04-27 10:09:44.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      778 2023-04-27 10:09:44.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7022 2023-04-03 13:03:38.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.326022 sb3_contrib-2.0.0a9/sb3_contrib/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       85 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8436 2023-05-20 08:57:42.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/vec_env/async_eval.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.326022 sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1139 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/action_masker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4085 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/time_feature.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.330021 sb3_contrib-2.0.0a9/sb3_contrib/ppo_mask/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      208 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_mask/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      294 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_mask/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    24110 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_mask/ppo_mask.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.334022 sb3_contrib-2.0.0a9/sb3_contrib/ppo_recurrent/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      249 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_recurrent/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      313 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_recurrent/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21599 2023-04-27 10:09:44.000000 sb3_contrib-2.0.0a9/sb3_contrib/ppo_recurrent/ppo_recurrent.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2020-09-25 09:51:52.000000 sb3_contrib-2.0.0a9/sb3_contrib/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.334022 sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      187 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11417 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14168 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/qrdqn.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.334022 sb3_contrib-2.0.0a9/sb3_contrib/tqc/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      177 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/tqc/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    23495 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/tqc/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15637 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/tqc/tqc.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.338022 sb3_contrib-2.0.0a9/sb3_contrib/trpo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      182 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a9/sb3_contrib/trpo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      302 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a9/sb3_contrib/trpo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20271 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/sb3_contrib/trpo/trpo.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-05-20 08:57:42.000000 sb3_contrib-2.0.0a9/sb3_contrib/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.314022 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-05-20 08:57:56.000000 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1893 2023-05-20 08:57:56.000000 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-05-20 08:57:56.000000 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       27 2023-05-20 08:57:56.000000 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       12 2023-05-20 08:57:56.000000 sb3_contrib-2.0.0a9/sb3_contrib.egg-info/top_level.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-05-20 08:57:56.346022 sb3_contrib-2.0.0a9/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4146 2023-05-20 08:57:42.000000 sb3_contrib-2.0.0a9/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-05-20 08:57:56.342022 sb3_contrib-2.0.0a9/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7675 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2385 2023-02-13 13:36:17.000000 sb3_contrib-2.0.0a9/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9174 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11090 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a9/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1366 2023-05-20 08:57:42.000000 sb3_contrib-2.0.0a9/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9645 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_invalid_actions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6862 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_lstm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4994 2023-05-14 16:02:11.000000 sb3_contrib-2.0.0a9/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17613 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9974 2023-04-27 09:36:48.000000 sb3_contrib-2.0.0a9/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2165 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a9/tests/test_utils.py
```

### Comparing `sb3_contrib-2.0.0a4/LICENSE` & `sb3_contrib-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/PKG-INFO` & `sb3_contrib-2.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb3_contrib
-Version: 2.0.0a4
+Version: 2.0.0a9
 Summary: Contrib package of Stable Baselines3, experimental code.
 Home-page: https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: Documentation, https://sb3-contrib.readthedocs.io/
```

### Comparing `sb3_contrib-2.0.0a4/README.md` & `sb3_contrib-2.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/pyproject.toml` & `sb3_contrib-2.0.0a9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -31,33 +31,28 @@
 	| sb3_contrib/ars/ars.py$
 	| sb3_contrib/common/recurrent/policies.py$
 	| sb3_contrib/common/recurrent/buffers.py$
 	| sb3_contrib/common/maskable/distributions.py$
 	| sb3_contrib/common/maskable/callbacks.py$
 	| sb3_contrib/common/maskable/policies.py$
 	| sb3_contrib/common/maskable/buffers.py$
-	| sb3_contrib/common/envs/invalid_actions_env.py$
 	| sb3_contrib/common/vec_env/async_eval.py$
 	| sb3_contrib/ppo_mask/ppo_mask.py$
 	| tests/test_train_eval_mode.py$
   )"""
 
 [tool.pytest.ini_options]
 # Deterministic ordering for tests; useful for pytest-xdist.
 env = [
 	"PYTHONHASHSEED=0"
 ]
 
 filterwarnings = [
     # Tensorboard warnings
     "ignore::DeprecationWarning:tensorboard",
-    # Gym warnings
-    "ignore:Parameters to load are deprecated.:DeprecationWarning",
-    "ignore:the imp module is deprecated in favour of importlib:PendingDeprecationWarning",
-    "ignore::UserWarning:gym",
 ]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')"
 ]
 
 [tool.coverage.run]
 disable_warnings = ["couldnt-parse"]
```

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/__init__.py` & `sb3_contrib-2.0.0a9/sb3_contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/ars/ars.py` & `sb3_contrib-2.0.0a9/sb3_contrib/ars/ars.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/ars/policies.py` & `sb3_contrib-2.0.0a9/sb3_contrib/ars/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/envs/invalid_actions_env.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/envs/invalid_actions_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 import numpy as np
 from gymnasium import spaces
 from stable_baselines3.common.envs import IdentityEnv
 
 
-class InvalidActionEnvDiscrete(IdentityEnv):
+class InvalidActionEnvDiscrete(IdentityEnv[int]):
     """
     Identity env with a discrete action space. Supports action masking.
     """
 
     def __init__(
         self,
         dim: Optional[int] = None,
@@ -26,25 +26,27 @@
         self.invalid_actions: List[int] = []
         super().__init__(space=space, ep_length=ep_length)
 
     def _choose_next_state(self) -> None:
         self.state = self.action_space.sample()
         # Randomly choose invalid actions that are not the current state
         potential_invalid_actions = [i for i in self.possible_actions if i != self.state]
-        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False)
+        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False).tolist()
 
     def action_masks(self) -> List[bool]:
         return [action not in self.invalid_actions for action in self.possible_actions]
 
 
-class InvalidActionEnvMultiDiscrete(IdentityEnv):
+class InvalidActionEnvMultiDiscrete(IdentityEnv[np.ndarray]):
     """
     Identity env with a multidiscrete action space. Supports action masking.
     """
 
+    action_space: spaces.MultiDiscrete
+
     def __init__(
         self,
         dims: Optional[List[int]] = None,
         ep_length: int = 100,
         n_invalid_actions: int = 0,
     ):
         if dims is None:
@@ -66,21 +68,21 @@
         running_total = 0
         for i in range(len(self.action_space.nvec)):
             converted_state.append(running_total + self.state[i])
             running_total += self.action_space.nvec[i]
 
         # Randomly choose invalid actions that are not the current state
         potential_invalid_actions = [i for i in self.possible_actions if i not in converted_state]
-        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False)
+        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False).tolist()
 
     def action_masks(self) -> List[bool]:
         return [action not in self.invalid_actions for action in self.possible_actions]
 
 
-class InvalidActionEnvMultiBinary(IdentityEnv):
+class InvalidActionEnvMultiBinary(IdentityEnv[np.ndarray]):
     """
     Identity env with a multibinary action space. Supports action masking.
     """
 
     def __init__(
         self,
         dims: Optional[int] = None,
@@ -90,27 +92,28 @@
         if dims is None:
             dims = 1
 
         if n_invalid_actions > dims:
             raise ValueError(f"Cannot find a valid action for each dim. Set n_invalid_actions <= {dims}")
 
         space = spaces.MultiBinary(dims)
+        self.n_dims = dims
         self.n_invalid_actions = n_invalid_actions
         self.possible_actions = np.arange(2 * dims)
         self.invalid_actions: List[int] = []
         super().__init__(space=space, ep_length=ep_length)
 
     def _choose_next_state(self) -> None:
         self.state = self.action_space.sample()
 
         converted_state: List[int] = []
         running_total = 0
-        for i in range(self.action_space.n):
+        for i in range(self.n_dims):
             converted_state.append(running_total + self.state[i])
             running_total += 2
 
         # Randomly choose invalid actions that are not the current state
         potential_invalid_actions = [i for i in self.possible_actions if i not in converted_state]
-        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False)
+        self.invalid_actions = np.random.choice(potential_invalid_actions, self.n_invalid_actions, replace=False).tolist()
 
     def action_masks(self) -> List[bool]:
         return [action not in self.invalid_actions for action in self.possible_actions]
```

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/buffers.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/buffers.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/callbacks.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/callbacks.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/distributions.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/distributions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/evaluation.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/evaluation.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/policies.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/utils.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/maskable/utils.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/buffers.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/buffers.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/policies.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/type_aliases.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/recurrent/type_aliases.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/utils.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/utils.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/async_eval.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/vec_env/async_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import torch as th
 from stable_baselines3.common.evaluation import evaluate_policy
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.running_mean_std import RunningMeanStd
-from stable_baselines3.common.utils import compat_gym_seed
 from stable_baselines3.common.vec_env import VecEnv, unwrap_vec_normalize
 from stable_baselines3.common.vec_env.base_vec_env import CloudpickleWrapper
 
 
 def _worker(
     remote: mp.connection.Connection,
     parent_remote: mp.connection.Connection,
@@ -28,47 +27,48 @@
     :param remote: Pipe to communicate with the parent process.
     :param parent_remote:
     :param worker_env_wrapper: Callable used to create the environment inside the process.
     :param train_policy_wrapper: Callable used to create the policy inside the process.
     :param n_eval_episodes: Number of evaluation episodes per candidate.
     """
     parent_remote.close()
-    env = worker_env_wrapper.var()
+    vec_env: VecEnv = worker_env_wrapper.var()
     train_policy = train_policy_wrapper.var
-    vec_normalize = unwrap_vec_normalize(env)
+    vec_normalize = unwrap_vec_normalize(vec_env)
     if vec_normalize is not None:
         obs_rms = vec_normalize.obs_rms
     else:
         obs_rms = None
     while True:
         try:
             cmd, data = remote.recv()
             if cmd == "eval":
                 results = []
                 # Evaluate each candidate and save results
                 for weights_idx, candidate_weights in data:
                     train_policy.load_from_vector(candidate_weights.cpu())
                     episode_rewards, episode_lengths = evaluate_policy(
                         train_policy,
-                        env,
+                        vec_env,
                         n_eval_episodes=n_eval_episodes,
                         return_episode_rewards=True,
                         warn=False,
                     )
                     results.append((weights_idx, (episode_rewards, episode_lengths)))
                 remote.send(results)
             elif cmd == "seed":
-                remote.send(compat_gym_seed(env, seed=data))
+                # Note: the seed will only be effective at the next reset
+                remote.send(vec_env.seed(seed=data))
             elif cmd == "get_obs_rms":
                 remote.send(obs_rms)
             elif cmd == "sync_obs_rms":
                 vec_normalize.obs_rms = data
                 obs_rms = data
             elif cmd == "close":
-                env.close()
+                vec_env.close()
                 remote.close()
                 break
             else:
                 raise NotImplementedError(f"`{cmd}` is not implemented in the worker")
         except EOFError:
             break
```

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/action_masker.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/action_masker.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/time_feature.py` & `sb3_contrib-2.0.0a9/sb3_contrib/common/wrappers/time_feature.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/ppo_mask.py` & `sb3_contrib-2.0.0a9/sb3_contrib/ppo_mask/ppo_mask.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/ppo_recurrent.py` & `sb3_contrib-2.0.0a9/sb3_contrib/ppo_recurrent/ppo_recurrent.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/policies.py` & `sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/qrdqn.py` & `sb3_contrib-2.0.0a9/sb3_contrib/qrdqn/qrdqn.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/tqc/policies.py` & `sb3_contrib-2.0.0a9/sb3_contrib/tqc/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/tqc/tqc.py` & `sb3_contrib-2.0.0a9/sb3_contrib/tqc/tqc.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib/trpo/trpo.py` & `sb3_contrib-2.0.0a9/sb3_contrib/trpo/trpo.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib.egg-info/PKG-INFO` & `sb3_contrib-2.0.0a9/sb3_contrib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb3-contrib
-Version: 2.0.0a4
+Version: 2.0.0a9
 Summary: Contrib package of Stable Baselines3, experimental code.
 Home-page: https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: Documentation, https://sb3-contrib.readthedocs.io/
```

### Comparing `sb3_contrib-2.0.0a4/sb3_contrib.egg-info/SOURCES.txt` & `sb3_contrib-2.0.0a9/sb3_contrib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/setup.py` & `sb3_contrib-2.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 setup(
     name="sb3_contrib",
     packages=[package for package in find_packages() if package.startswith("sb3_contrib")],
     package_data={"sb3_contrib": ["py.typed", "version.txt"]},
     install_requires=[
-        "stable_baselines3>=2.0.0a4",
+        "stable_baselines3>=2.0.0a9",
     ],
     description="Contrib package of Stable Baselines3, experimental code.",
     author="Antonin Raffin",
     url="https://github.com/Stable-Baselines-Team/stable-baselines3-contrib",
     author_email="antonin.raffin@dlr.de",
     keywords="reinforcement-learning-algorithms reinforcement-learning machine-learning "
     "gym openai stable baselines toolbox python data-science",
```

### Comparing `sb3_contrib-2.0.0a4/tests/test_cnn.py` & `sb3_contrib-2.0.0a9/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_deterministic.py` & `sb3_contrib-2.0.0a9/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_dict_env.py` & `sb3_contrib-2.0.0a9/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_distributions.py` & `sb3_contrib-2.0.0a9/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_identity.py` & `sb3_contrib-2.0.0a9/tests/test_identity.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,13 +26,13 @@
         n_steps = 1500
         # DQN only support discrete actions
         if isinstance(env, (IdentityEnvMultiDiscrete, IdentityEnvMultiBinary)):
             return
     elif n_steps == TRPO:
         kwargs = dict(n_steps=256, cg_max_steps=5)
 
-    model = model_class("MlpPolicy", vec_env, learning_rate=1e-3, gamma=0.4, seed=1, **kwargs).learn(n_steps)
+    model = model_class("MlpPolicy", vec_env, learning_rate=1e-3, gamma=0.4, seed=0, **kwargs).learn(n_steps)
 
     evaluate_policy(model, vec_env, n_eval_episodes=20, reward_threshold=90, warn=False)
     obs = vec_env.reset()
 
     assert np.shape(model.predict(obs)[0]) == np.shape(obs)
```

### Comparing `sb3_contrib-2.0.0a4/tests/test_invalid_actions.py` & `sb3_contrib-2.0.0a9/tests/test_invalid_actions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_lstm.py` & `sb3_contrib-2.0.0a9/tests/test_lstm.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_run.py` & `sb3_contrib-2.0.0a9/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_save_load.py` & `sb3_contrib-2.0.0a9/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_train_eval_mode.py` & `sb3_contrib-2.0.0a9/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a4/tests/test_utils.py` & `sb3_contrib-2.0.0a9/tests/test_utils.py`

 * *Files identical despite different names*

