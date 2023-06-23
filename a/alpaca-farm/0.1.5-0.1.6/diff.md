# Comparing `tmp/alpaca_farm-0.1.5.tar.gz` & `tmp/alpaca_farm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.5.tar", last modified: Thu Jun 15 04:33:44 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.6.tar", last modified: Fri Jun 23 08:08:23 2023, max compression
```

## Comparing `alpaca_farm-0.1.5.tar` & `alpaca_farm-0.1.6.tar`

### file list

```diff
@@ -1,97 +1,93 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.005156 alpaca_farm-0.1.5/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.5/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.5/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-15 04:33:44.004931 alpaca_farm-0.1.5/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    16695 2023-06-12 23:53:35.000000 alpaca_farm-0.1.5/README.md
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-15 04:33:44.005191 alpaca_farm-0.1.5/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.5/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.987712 alpaca_farm-0.1.5/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.992692 alpaca_farm-0.1.5/src/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.994807 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 xuechenli   (501) staff       (20)      672 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/analysis.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.988075 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.999859 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.000369 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.000668 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/decoders.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4692 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    28861 2023-06-13 06:34:11.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/pairwise_annotators.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11404 2023-06-15 04:30:13.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/constants.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.001488 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.002061 alpaca_farm-0.1.5/src/alpaca_farm/inference/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/score.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/logging.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.002637 alpaca_farm-0.1.5/src/alpaca_farm/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11542 2023-06-11 22:43:54.000000 alpaca_farm-0.1.5/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.003999 alpaca_farm-0.1.5/src/alpaca_farm/rl/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.5/src/alpaca_farm/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.993331 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     4356 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.004732 alpaca_farm-0.1.5/tests/
--rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.609046 alpaca_farm-0.1.6/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.6/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.6/MANIFEST.in
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16786 2023-06-23 08:08:23.608833 alpaca_farm-0.1.6/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16132 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/README.md
+-rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-23 08:08:23.609084 alpaca_farm-0.1.6/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2599 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.591823 alpaca_farm-0.1.6/src/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.597614 alpaca_farm-0.1.6/src/alpaca_farm/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-23 08:07:51.000000 alpaca_farm-0.1.6/src/alpaca_farm/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.598757 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      640 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/__init__.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.592186 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604102 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7266 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604616 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      500 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604816 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      446 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7108 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/common.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/constants.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.605680 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.606251 alpaca_farm-0.1.6/src/alpaca_farm/inference/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/logging.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.606829 alpaca_farm-0.1.6/src/alpaca_farm/models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11576 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.607962 alpaca_farm-0.1.6/src/alpaca_farm/rl/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.6/src/alpaca_farm/types.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.598364 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16786 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4168 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      307 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.608603 alpaca_farm-0.1.6/tests/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.5/LICENSE` & `alpaca_farm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/PKG-INFO` & `alpaca_farm-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center" width="100%">
 <img src="assets/AlpacaFarm_big.png" alt="AlpacaFarm" style="width: 50%; min-width: 300px; display: block; margin: auto;">
 </p>
 
 # AlpacaFarm: A Simulation Framework for Methods that <br/>Learn from Human Feedback
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Research and development on learning from human feedback is difficult because methods
 like [RLHF](https://arxiv.org/abs/2203.02155) are complex and costly to run.
 AlpacaFarm is a simulator that enables research and development on learning from feedback at a fraction of the usual
 cost, promoting accessible research on instruction following and alignment.
 
@@ -84,24 +85,15 @@
 packages.
 
 ## Simulating pairwise preference
 
 **Notebook
 example:** [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tatsu-lab/alpaca_farm/blob/main/examples/auto_annotations.ipynb)
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the set of dependencies for simulating pairwise preference, run
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation and annotations we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators and additional noise to simulate the variance of human annotations.
 
 To get started, set the environment variable `OPENAI_API_KEY` to your OpenAI API key, and (optionally) `OPENAI_ORG` to
 the
 organization ID.
 You can do this by running
 
 ```bash
@@ -125,48 +117,39 @@
 #   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
 #   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]"}]
 
 annotator = PairwiseAutoAnnotator()
 annotated = annotator.annotate_pairs(outputs_pairs)
 
 print(annotated[-1:])
-# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.',
-#   'input': '',
-#   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
-#   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
-#   'annotator': 'davinci003_3',
-#   'preference': 1.0}]
+# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.', 
+# 'input': '', 
+# 'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]", 
+# 'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
+# 'annotator': 'chatgpt_2', 
+# 'preference': 2}]
 ```
 
 If instead of pairs you have a list of sampled outputs, you can use the following.
 
 ```python
 multisample_outputs = [dict(instruction="repeat the following", input="yes", output=["yes", "no", "maybe", "repeat"])]
 print(annotator.annotate_samples(multisample_outputs))
-# [{'sample_id': 0,
-#   'instruction': 'repeat the following',
-#   'input': 'yes',
-#   'output_1': 'yes',
-#   'output_2': 'no',
-#   'annotator': 'gpt4_2',
+# [{'sample_id': 0, 
+#   'instruction': 'repeat the following', 
+#   'input': 'yes', 
+#   'output_1': 'yes', 
+#   'output_2': 'maybe', 
+#   'annotator': 'chatgpt_2', 
 #   'preference': 1}]
 ```
 
 ## Running automatic evaluation
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the auto annotators with minimal additional packages use the following
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators. 
 
 To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
 organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
@@ -183,23 +166,23 @@
 ...  # use the data to get outputs for your model and save it
 path_to_outputs = "examples/data/eval_gpt-3.5-turbo-0301.json"
 # outputs should be a list of json as such:
 # [{'instruction': 'What are the names of some famous actors that started their careers on Broadway?', 'input': '', 'output': 'Some famous actors that started their careers on Broadway are Hugh Jackman, Meryl Streep, Denzel Washington, Audra McDonald, and Lin-Manuel Miranda.', 'generator': 'gpt-3.5-turbo-0301', 'dataset': 'helpful_base', 'datasplit': 'eval'},
 # ...]
 
 alpaca_leaderboard(path_or_all_outputs=path_to_outputs, name="My fancy model", is_print_metrics=True)
-#                                         n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
-# GPT4                                      17.00   805.00  639.00       149.00            1.38     80.43
-# ChatGPT                                    9.00   804.00  489.00       306.00            1.71     61.38
-# My fancy model                             9.00   804.00  483.00       312.00            1.71     60.63
-# RLHF PPO                                   9.00   803.00  370.00       424.00            1.75     46.64
-# SFT 52k (Alpaca 7B)                       16.00   804.00  320.00       468.00            1.72     40.80
-# SFT 10k                                   19.00   802.00  278.00       505.00            1.67     35.85
-# Davinci001                                 0.00   805.00  201.00       604.00            1.53     24.97
-# LLaMA 7B                                   0.00   786.00   94.00       692.00            1.16     11.96
+#                      n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
+# GPT4                   17.00   804.00  631.00       156.00            1.40     79.54
+# ChatGPT                 9.00   805.00  503.00       293.00            1.69     63.04
+# My fancy model          9.00   803.00  497.00       297.00            1.70     62.45
+# RLHF PPO                9.00   805.00  392.00       404.00            1.75     49.25
+# SFT 52k (Alpaca 7B)    16.00   805.00  312.00       477.00            1.71     39.75
+# SFT 10k                19.00   802.00  278.00       505.00            1.67     35.85
+# Davinci001              0.00   805.00  201.00       604.00            1.53     24.97
+# LLaMA 7B                0.00   775.00   98.00       677.00            1.19     12.65
 ```
 
 If you want to compare against our baseline model (Davinci003 with
 our [prompt](https://github.com/tatsu-lab/alpaca_farm/blob/main/examples/prompts/v0_inputs_noinputs.json)) on your own
 data, you can decode it using [main_oai_baselines](#openai-models).
 
 ## Running reference methods
@@ -260,17 +243,17 @@
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
 according
 to the previous step.
 Note the KL penalty coefficient for human reward PPO is much larger than for simulated PPO.
-Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.0002` for human PPO to recover our original results.
-Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 pass through the entire
-set of instructions), and starts to decay with more PPO steps.
+Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.02` for human PPO to recover our original results.
+Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 passes through the entire
+set of instructions) and starts to decay with more PPO steps.
 
 ### Best-of-n decoding
 
 To replicate our best-of-n inference-time decoding results for the AlpacaFarm evaluation suite, run
 
 ```bash
 python examples/best_of_n.py \
```

### Comparing `alpaca_farm-0.1.5/README.md` & `alpaca_farm-0.1.6/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+Metadata-Version: 2.1
+Name: alpaca-farm
+Version: 0.1.6
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: dev
+License-File: LICENSE
+
 <p align="center" width="100%">
 <img src="assets/AlpacaFarm_big.png" alt="AlpacaFarm" style="width: 50%; min-width: 300px; display: block; margin: auto;">
 </p>
 
 # AlpacaFarm: A Simulation Framework for Methods that <br/>Learn from Human Feedback
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Research and development on learning from human feedback is difficult because methods
 like [RLHF](https://arxiv.org/abs/2203.02155) are complex and costly to run.
 AlpacaFarm is a simulator that enables research and development on learning from feedback at a fraction of the usual
 cost, promoting accessible research on instruction following and alignment.
 
@@ -67,24 +85,15 @@
 packages.
 
 ## Simulating pairwise preference
 
 **Notebook
 example:** [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tatsu-lab/alpaca_farm/blob/main/examples/auto_annotations.ipynb)
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the set of dependencies for simulating pairwise preference, run
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation and annotations we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators and additional noise to simulate the variance of human annotations.
 
 To get started, set the environment variable `OPENAI_API_KEY` to your OpenAI API key, and (optionally) `OPENAI_ORG` to
 the
 organization ID.
 You can do this by running
 
 ```bash
@@ -108,48 +117,39 @@
 #   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
 #   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]"}]
 
 annotator = PairwiseAutoAnnotator()
 annotated = annotator.annotate_pairs(outputs_pairs)
 
 print(annotated[-1:])
-# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.',
-#   'input': '',
-#   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
-#   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
-#   'annotator': 'davinci003_3',
-#   'preference': 1.0}]
+# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.', 
+# 'input': '', 
+# 'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]", 
+# 'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
+# 'annotator': 'chatgpt_2', 
+# 'preference': 2}]
 ```
 
 If instead of pairs you have a list of sampled outputs, you can use the following.
 
 ```python
 multisample_outputs = [dict(instruction="repeat the following", input="yes", output=["yes", "no", "maybe", "repeat"])]
 print(annotator.annotate_samples(multisample_outputs))
-# [{'sample_id': 0,
-#   'instruction': 'repeat the following',
-#   'input': 'yes',
-#   'output_1': 'yes',
-#   'output_2': 'no',
-#   'annotator': 'gpt4_2',
+# [{'sample_id': 0, 
+#   'instruction': 'repeat the following', 
+#   'input': 'yes', 
+#   'output_1': 'yes', 
+#   'output_2': 'maybe', 
+#   'annotator': 'chatgpt_2', 
 #   'preference': 1}]
 ```
 
 ## Running automatic evaluation
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the auto annotators with minimal additional packages use the following
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators. 
 
 To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
 organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
@@ -166,23 +166,23 @@
 ...  # use the data to get outputs for your model and save it
 path_to_outputs = "examples/data/eval_gpt-3.5-turbo-0301.json"
 # outputs should be a list of json as such:
 # [{'instruction': 'What are the names of some famous actors that started their careers on Broadway?', 'input': '', 'output': 'Some famous actors that started their careers on Broadway are Hugh Jackman, Meryl Streep, Denzel Washington, Audra McDonald, and Lin-Manuel Miranda.', 'generator': 'gpt-3.5-turbo-0301', 'dataset': 'helpful_base', 'datasplit': 'eval'},
 # ...]
 
 alpaca_leaderboard(path_or_all_outputs=path_to_outputs, name="My fancy model", is_print_metrics=True)
-#                                         n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
-# GPT4                                      17.00   805.00  639.00       149.00            1.38     80.43
-# ChatGPT                                    9.00   804.00  489.00       306.00            1.71     61.38
-# My fancy model                             9.00   804.00  483.00       312.00            1.71     60.63
-# RLHF PPO                                   9.00   803.00  370.00       424.00            1.75     46.64
-# SFT 52k (Alpaca 7B)                       16.00   804.00  320.00       468.00            1.72     40.80
-# SFT 10k                                   19.00   802.00  278.00       505.00            1.67     35.85
-# Davinci001                                 0.00   805.00  201.00       604.00            1.53     24.97
-# LLaMA 7B                                   0.00   786.00   94.00       692.00            1.16     11.96
+#                      n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
+# GPT4                   17.00   804.00  631.00       156.00            1.40     79.54
+# ChatGPT                 9.00   805.00  503.00       293.00            1.69     63.04
+# My fancy model          9.00   803.00  497.00       297.00            1.70     62.45
+# RLHF PPO                9.00   805.00  392.00       404.00            1.75     49.25
+# SFT 52k (Alpaca 7B)    16.00   805.00  312.00       477.00            1.71     39.75
+# SFT 10k                19.00   802.00  278.00       505.00            1.67     35.85
+# Davinci001              0.00   805.00  201.00       604.00            1.53     24.97
+# LLaMA 7B                0.00   775.00   98.00       677.00            1.19     12.65
 ```
 
 If you want to compare against our baseline model (Davinci003 with
 our [prompt](https://github.com/tatsu-lab/alpaca_farm/blob/main/examples/prompts/v0_inputs_noinputs.json)) on your own
 data, you can decode it using [main_oai_baselines](#openai-models).
 
 ## Running reference methods
@@ -243,17 +243,17 @@
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
 according
 to the previous step.
 Note the KL penalty coefficient for human reward PPO is much larger than for simulated PPO.
-Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.0002` for human PPO to recover our original results.
-Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 pass through the entire
-set of instructions), and starts to decay with more PPO steps.
+Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.02` for human PPO to recover our original results.
+Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 passes through the entire
+set of instructions) and starts to decay with more PPO steps.
 
 ### Best-of-n decoding
 
 To replicate our best-of-n inference-time decoding results for the AlpacaFarm evaluation suite, run
 
 ```bash
 python examples/best_of_n.py \
```

### Comparing `alpaca_farm-0.1.5/setup.py` & `alpaca_farm-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         "scikit-learn",
         "sentencepiece",
         "pandas",
         "wandb",
         "torch>=1.13.1",
         "fire",
         "openai",
+        "alpaca_eval",
     ],
     extras_require={
         "full": [
             # Training efficiency.
             "flash-attn",
             "apex",
             "deepspeed",
@@ -64,21 +65,22 @@
         ],
         "dev": {
             "pre-commit>=3.2.0",
             "black>=23.1.0",
             "isort",
         },
     },
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.6/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .eval import alpaca_leaderboard
-from .pairwise_annotators import PairwiseAutoAnnotator
+from .eval import PairwiseAutoAnnotator, alpaca_leaderboard
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,194 +1,207 @@
 # paths are relative to auto_annotations
 
 gpt4_1 : # gpt-4-0314_pairwise_v1_b4_chatml-chat_CoT_JSON_temp=1.0 in old code
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-4-0314"
     max_tokens: 600
     temperature: 1.0
-  outputs_to_match:
-    1: ': true'
-    2: ': false'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: ': true'
+      2: ': false'
   batch_size: 4
 
 gpt4_2 : # gpt-4-0314_pairwise_diverse-diana_v0_b5_chatml-prompt_short_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b5_diana_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b5_diana_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-4-0314"
     max_tokens: 250
     temperature: 1.0
-  outputs_to_match:
-    1: '(?:^|\n)Output \(a\)'
-    2: '(?:^|\n)Output \(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '(?:^|\n) ?Output \(a\)'
+      2: '(?:^|\n) ?Output \(b\)'
   batch_size: 5
 
 gpt4_3 : # gpt-4-0314_pairwise_vH_b5_chatml-prompt_short_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b5_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b5_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b5_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b5_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-4-0314"
     max_tokens: 250
     temperature: 1.0
-  outputs_to_match:
-    1: '(?:^|\n)Output \(a\)'
-    2: '(?:^|\n)Output \(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '(?:^|\n) ?Output \(a\)'
+      2: '(?:^|\n) ?Output \(b\)'
   batch_size: 5
 
 gpt4_4 : # gpt-4-0314_pairwise_v2_b1_chatml-chat_reasoning_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b1_chat_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b1_chat_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-4-0314"
     max_tokens: 20
     temperature: 1.0
     # messing with tokens is not necessary for GPT4 but we use the same prompt for chatGPT
-    tokens_to_avoid: ['Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry']
-    tokens_to_favor: ["Output (a)", "Output (b)"]
-  outputs_to_match:
-    1: '(?:^|\n)Output \(a\)'
-    2: '(?:^|\n)Output \(b\)'
+    tokens_to_avoid: [ 'Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry' ]
+    tokens_to_favor: [ "Output (a)", "Output (b)" ]
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '(?:^|\n) ?Output \(a\)'
+      2: '(?:^|\n) ?Output \(b\)'
   batch_size: 1
 
 gpt4_5 : # gpt-4-0314_pairwise_diverse-joeX_v0_b5_chatml-prompt_short_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b5_joe_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b5_joe_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-4-0314"
     max_tokens: 250
     temperature: 1.0
-  outputs_to_match:
-    1: '(?:^|\n)Output \(a\)'
-    2: '(?:^|\n)Output \(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '(?:^|\n)Output \(a\)'
+      2: '(?:^|\n)Output \(b\)'
   batch_size: 5
 
 chatgpt_1 : # gpt-3.5-turbo_pairwise_vH_b1_chatml-prompt_short_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b1_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b1_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b1_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b1_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-3.5-turbo-0301"
     max_tokens: 50
     temperature: 1.0
-    tokens_to_avoid: ['Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context','It', 'both','Sorry']
+    tokens_to_avoid: [ 'Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context','It', 'both','Sorry' ]
     tokens_to_favor: [ "Output (a)", "Output (b)" ]
-  outputs_to_match:
-    1: 'Output \(a\)'
-    2: 'Output \(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '(?:^|\n) ?Output \(a\)'
+      2: '(?:^|\n) ?Output \(b\)'
   batch_size: 1
 
 chatgpt_2 : # gpt-3.5-turbo-0301_pairwise_v1_b1_chatml-chat_CoT_JSON_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-3.5-turbo-0301"
     max_tokens: 150
     temperature: 1.0
-    tokens_to_avoid: ['Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context','It', 'both','Sorry']
-  outputs_to_match: # to test
-    1: ': true'
-    2: ': false'
+    tokens_to_avoid: [ 'Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context','It', 'both','Sorry' ]
+  completion_parser_kwargs:
+    outputs_to_match: # to test
+      1: ': true'
+      2: ': false'
   batch_size: 1
 
 chatgpt_3 : # gpt-3.5-turbo_pairwise_v2_b1_chatml-chat_reasoning_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b1_chat_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b1_chat_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-3.5-turbo-0301"
     max_tokens: 20
     temperature: 1.0
-    tokens_to_avoid: ['Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry']
-    tokens_to_favor: ["Output (a)", "Output (b)"]
-  outputs_to_match:
-    1: 'Output \(a\)'
-    2: 'Output \(b\)'
+    tokens_to_avoid: [ 'Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry' ]
+    tokens_to_favor: [ "Output (a)", "Output (b)" ]
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: 'Output \(a\)'
+      2: 'Output \(b\)'
   batch_size: 1
 
 chatgpt_4 : # gpt-3.5-turbo_pairwise_v0_b1_chatml-chat_reasoning_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "gpt-3.5-turbo-0301"
     max_tokens: 20
     temperature: 1.0
-    tokens_to_avoid: ['Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry']
-    tokens_to_favor: ["Output (a)", "Output (b)"]
-  outputs_to_match:
-    1: 'Output \(a\)'
-    2: 'Output \(b\)'
+    tokens_to_avoid: [ 'Both', 'Neither', 'None', ' Both', ' Neither', 'Either', 'depends', 'context', 'It', 'both', 'Sorry' ]
+    tokens_to_favor: [ "Output (a)", "Output (b)" ]
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: 'Output \(a\)'
+      2: 'Output \(b\)'
   batch_size: 1
 
 davinci003_1 : # text-davinci-003_v1Reasoning_b4-pairwise_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/text_b4_reasoning_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/text_b4_reasoning_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "text-davinci-003"
     max_tokens: 200
     temperature: 1.0
-    tokens_to_favor: ["(a)", "(b)"]
-  outputs_to_match:
-    1: '\(a\)'
-    2: '\(b\)'
+    tokens_to_favor: [ "(a)", "(b)" ]
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '\(a\)'
+      2: '\(b\)'
   batch_size: 4
 
 davinci003_2 : # text-davinci-003_v1_pairwise_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/text_b1_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/text_b1_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/text_b1_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/text_b1_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "text-davinci-003"
     max_tokens: 200
     temperature: 1.0
-  outputs_to_match:
-    1: '\n\(a\)'
-    2: '\n\(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '\n\(a\)'
+      2: '\n\(b\)'
   batch_size: 1
 
 davinci003_3 : # text-davinci-003_v1_b5-pairwise_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/text_b5_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/text_b5_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/text_b5_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/text_b5_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "text-davinci-003"
     max_tokens: 200
     temperature: 1.0
-  outputs_to_match:
-    1: '\n\(a\)'
-    2: '\n\(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: '\n\(a\)'
+      2: '\n\(b\)'
   batch_size: 5
 
 davinci003_4 : # text-davinci-003_v0_pairwise_temp=1.0
-  prompt_templates:
-    with_inputs: "annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt"
-    without_inputs: "annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt"
-  fn_decoder: "openai_completions"
-  decoder_kwargs:
+  prompt_template:
+    with_inputs: "annotator_pool_v0/text_b1_v0_with_inputs.txt"
+    without_inputs: "annotator_pool_v0/text_b1_v0_without_inputs.txt"
+  fn_completions: "openai_completions"
+  completions_kwargs:
     model_name: "text-davinci-003"
     max_tokens: 200
     temperature: 1.0
-  outputs_to_match:
-    1: ' \(a\)'
-    2: ' \(b\)'
+  completion_parser_kwargs:
+    outputs_to_match:
+      1: ' \(a\)'
+      2: ' \(b\)'
   batch_size: 1
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/common.py` & `alpaca_farm-0.1.6/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.6/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.6/src/alpaca_farm/data_postprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.6/src/alpaca_farm/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.6/src/alpaca_farm/inference/decode.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.6/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.6/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.6/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.6/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/openai_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def _openai_completion_helper(
     prompt_batch: Sequence[StrOrOpenAIObject],
     is_chat: bool,
     sleep_time: int,
     openai_organization_ids: Optional[Sequence[str]] = None,
-    openai_api_key: Optional[str] = None,
+    openai_api_key: Optional[str] = os.environ.get("OPENAI_API_KEY", None),
     **shared_kwargs,
 ):
     if openai_api_key is not None:
         openai.api_key = openai_api_key
 
     # randomly select orgs
     if openai_organization_ids is not None:
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.6/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_trainer.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.6/src/alpaca_farm/rl/rl_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.6/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/types.py` & `alpaca_farm-0.1.6/src/alpaca_farm/types.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.6/src/alpaca_farm/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: alpaca-farm
-Version: 0.1.5
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: full
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center" width="100%">
 <img src="assets/AlpacaFarm_big.png" alt="AlpacaFarm" style="width: 50%; min-width: 300px; display: block; margin: auto;">
 </p>
 
 # AlpacaFarm: A Simulation Framework for Methods that <br/>Learn from Human Feedback
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Research and development on learning from human feedback is difficult because methods
 like [RLHF](https://arxiv.org/abs/2203.02155) are complex and costly to run.
 AlpacaFarm is a simulator that enables research and development on learning from feedback at a fraction of the usual
 cost, promoting accessible research on instruction following and alignment.
 
@@ -84,24 +67,15 @@
 packages.
 
 ## Simulating pairwise preference
 
 **Notebook
 example:** [![Using](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tatsu-lab/alpaca_farm/blob/main/examples/auto_annotations.ipynb)
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the set of dependencies for simulating pairwise preference, run
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation and annotations we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators and additional noise to simulate the variance of human annotations.
 
 To get started, set the environment variable `OPENAI_API_KEY` to your OpenAI API key, and (optionally) `OPENAI_ORG` to
 the
 organization ID.
 You can do this by running
 
 ```bash
@@ -125,48 +99,39 @@
 #   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
 #   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]"}]
 
 annotator = PairwiseAutoAnnotator()
 annotated = annotator.annotate_pairs(outputs_pairs)
 
 print(annotated[-1:])
-# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.',
-#   'input': '',
-#   'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]",
-#   'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
-#   'annotator': 'davinci003_3',
-#   'preference': 1.0}]
+# [{'instruction': 'If you could help me write an email to my friends inviting them to dinner on Friday, it would be greatly appreciated.', 
+# 'input': '', 
+# 'output_1': "Dear Friends, \r\n\r\nI hope this message finds you well. I'm excited to invite you to dinner on Friday. We'll meet at 7:00 PM at [location]. I look forward to seeing you there. \r\n\r\nBest,\r\n[Name]", 
+# 'output_2': "Hey everyone! \n\nI'm hosting a dinner party this Friday night and I'd love for all of you to come over. We'll have a delicious spread of food and some great conversations. \n\nLet me know if you can make it - I'd love to see you all there!\n\nCheers,\n[Your Name]",
+# 'annotator': 'chatgpt_2', 
+# 'preference': 2}]
 ```
 
 If instead of pairs you have a list of sampled outputs, you can use the following.
 
 ```python
 multisample_outputs = [dict(instruction="repeat the following", input="yes", output=["yes", "no", "maybe", "repeat"])]
 print(annotator.annotate_samples(multisample_outputs))
-# [{'sample_id': 0,
-#   'instruction': 'repeat the following',
-#   'input': 'yes',
-#   'output_1': 'yes',
-#   'output_2': 'no',
-#   'annotator': 'gpt4_2',
+# [{'sample_id': 0, 
+#   'instruction': 'repeat the following', 
+#   'input': 'yes', 
+#   'output_1': 'yes', 
+#   'output_2': 'maybe', 
+#   'annotator': 'chatgpt_2', 
 #   'preference': 1}]
 ```
 
 ## Running automatic evaluation
 
-<details>
-  <summary><b>Installing auto annotators with minimal dependencies</b></summary>
-    To install only the auto annotators with minimal additional packages use the following
-
-```bash
-pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
-pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
-```
-
-</details>
+For all the evaluation we use [**AlpacaEval**](https://github.com/tatsu-lab/alpaca_eval/tree/main#making-a-new-evaluator) with our pool of automatic annotators. 
 
 To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
 organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
@@ -183,23 +148,23 @@
 ...  # use the data to get outputs for your model and save it
 path_to_outputs = "examples/data/eval_gpt-3.5-turbo-0301.json"
 # outputs should be a list of json as such:
 # [{'instruction': 'What are the names of some famous actors that started their careers on Broadway?', 'input': '', 'output': 'Some famous actors that started their careers on Broadway are Hugh Jackman, Meryl Streep, Denzel Washington, Audra McDonald, and Lin-Manuel Miranda.', 'generator': 'gpt-3.5-turbo-0301', 'dataset': 'helpful_base', 'datasplit': 'eval'},
 # ...]
 
 alpaca_leaderboard(path_or_all_outputs=path_to_outputs, name="My fancy model", is_print_metrics=True)
-#                                         n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
-# GPT4                                      17.00   805.00  639.00       149.00            1.38     80.43
-# ChatGPT                                    9.00   804.00  489.00       306.00            1.71     61.38
-# My fancy model                             9.00   804.00  483.00       312.00            1.71     60.63
-# RLHF PPO                                   9.00   803.00  370.00       424.00            1.75     46.64
-# SFT 52k (Alpaca 7B)                       16.00   804.00  320.00       468.00            1.72     40.80
-# SFT 10k                                   19.00   802.00  278.00       505.00            1.67     35.85
-# Davinci001                                 0.00   805.00  201.00       604.00            1.53     24.97
-# LLaMA 7B                                   0.00   786.00   94.00       692.00            1.16     11.96
+#                      n_draws  n_total  n_wins  n_wins_base  standard_error  win_rate
+# GPT4                   17.00   804.00  631.00       156.00            1.40     79.54
+# ChatGPT                 9.00   805.00  503.00       293.00            1.69     63.04
+# My fancy model          9.00   803.00  497.00       297.00            1.70     62.45
+# RLHF PPO                9.00   805.00  392.00       404.00            1.75     49.25
+# SFT 52k (Alpaca 7B)    16.00   805.00  312.00       477.00            1.71     39.75
+# SFT 10k                19.00   802.00  278.00       505.00            1.67     35.85
+# Davinci001              0.00   805.00  201.00       604.00            1.53     24.97
+# LLaMA 7B                0.00   775.00   98.00       677.00            1.19     12.65
 ```
 
 If you want to compare against our baseline model (Davinci003 with
 our [prompt](https://github.com/tatsu-lab/alpaca_farm/blob/main/examples/prompts/v0_inputs_noinputs.json)) on your own
 data, you can decode it using [main_oai_baselines](#openai-models).
 
 ## Running reference methods
@@ -260,17 +225,17 @@
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
 according
 to the previous step.
 Note the KL penalty coefficient for human reward PPO is much larger than for simulated PPO.
-Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.0002` for human PPO to recover our original results.
-Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 pass through the entire
-set of instructions), and starts to decay with more PPO steps.
+Set `<kl_coef>` to `0.0067` for simulated PPO, and `0.02` for human PPO to recover our original results.
+Performance of the PPO model is typically much better than SFT at 20-80 PPO steps (less than 4 passes through the entire
+set of instructions) and starts to decay with more PPO steps.
 
 ### Best-of-n decoding
 
 To replicate our best-of-n inference-time decoding results for the AlpacaFarm evaluation suite, run
 
 ```bash
 python examples/best_of_n.py \
```

### Comparing `alpaca_farm-0.1.5/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.6/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 src/alpaca_farm/utils.py
 src/alpaca_farm.egg-info/PKG-INFO
 src/alpaca_farm.egg-info/SOURCES.txt
 src/alpaca_farm.egg-info/dependency_links.txt
 src/alpaca_farm.egg-info/requires.txt
 src/alpaca_farm.egg-info/top_level.txt
 src/alpaca_farm/auto_annotations/__init__.py
-src/alpaca_farm/auto_annotations/analysis.py
-src/alpaca_farm/auto_annotations/decoders.py
 src/alpaca_farm/auto_annotations/eval.py
-src/alpaca_farm/auto_annotations/pairwise_annotators.py
-src/alpaca_farm/auto_annotations/utils.py
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
 src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
```

### Comparing `alpaca_farm-0.1.5/tests/test_flash_llama.py` & `alpaca_farm-0.1.6/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/tests/test_flash_opt.py` & `alpaca_farm-0.1.6/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/tests/test_torch_ops.py` & `alpaca_farm-0.1.6/tests/test_torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.5/tests/test_utils.py` & `alpaca_farm-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

