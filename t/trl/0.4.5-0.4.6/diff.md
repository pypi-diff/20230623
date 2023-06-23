# Comparing `tmp/trl-0.4.5.tar.gz` & `tmp/trl-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.4.5.tar", last modified: Fri Jun 23 08:15:58 2023, max compression
+gzip compressed data, was "trl-0.4.6.tar", last modified: Fri Jun 23 09:18:14 2023, max compression
```

## Comparing `trl-0.4.5.tar` & `trl-0.4.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.533237 trl-0.4.5/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2445 2023-05-03 09:18:40.000000 trl-0.4.5/CONTRIBUTING.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.4.5/LICENSE
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.4.5/MANIFEST.in
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 08:15:58.533237 trl-0.4.5/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5413 2023-05-03 09:18:40.000000 trl-0.4.5/README.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      315 2023-06-23 08:15:58.533237 trl-0.4.5/setup.cfg
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3779 2023-06-23 08:13:13.000000 trl-0.4.5/setup.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.529236 trl-0.4.5/tests/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.4.5/tests/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.4.5/tests/test_best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.4.5/tests/test_core.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.4.5/tests/test_e2e.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.4.5/tests/test_modeling_value_head.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.4.5/tests/test_no_peft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.4.5/tests/test_peft_models.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    41226 2023-06-23 08:12:16.000000 trl-0.4.5/tests/test_ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-06-21 08:50:41.000000 trl-0.4.5/tests/test_reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18911 2023-06-23 08:12:16.000000 trl-0.4.5/tests/test_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.4.5/tests/testing_constants.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.4.5/tests/testing_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.529236 trl-0.4.5/trl/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      407 2023-06-23 08:13:20.000000 trl-0.4.5/trl/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7920 2023-05-03 09:18:40.000000 trl-0.4.5/trl/core.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.529236 trl-0.4.5/trl/extras/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.4.5/trl/extras/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.4.5/trl/extras/best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.4.5/trl/import_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.533237 trl-0.4.5/trl/models/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.4.5/trl/models/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23627 2023-06-23 08:12:16.000000 trl-0.4.5/trl/models/modeling_base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    17967 2023-05-17 09:28:26.000000 trl-0.4.5/trl/models/modeling_value_head.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.533237 trl-0.4.5/trl/trainer/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1035 2023-06-21 09:04:57.000000 trl-0.4.5/trl/trainer/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.4.5/trl/trainer/base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8308 2023-06-23 08:12:16.000000 trl-0.4.5/trl/trainer/ppo_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    52510 2023-06-23 08:12:16.000000 trl-0.4.5/trl/trainer/ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10115 2023-06-23 08:12:16.000000 trl-0.4.5/trl/trainer/reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14717 2023-06-23 08:12:16.000000 trl-0.4.5/trl/trainer/sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11523 2023-06-23 08:12:16.000000 trl-0.4.5/trl/trainer/utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 08:15:58.529236 trl-0.4.5/trl.egg-info/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 08:15:58.000000 trl-0.4.5/trl.egg-info/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      887 2023-06-23 08:15:58.000000 trl-0.4.5/trl.egg-info/SOURCES.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-06-23 08:15:58.000000 trl-0.4.5/trl.egg-info/dependency_links.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.4.5/trl.egg-info/not-zip-safe
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      225 2023-06-23 08:15:58.000000 trl-0.4.5/trl.egg-info/requires.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-06-23 08:15:58.000000 trl-0.4.5/trl.egg-info/top_level.txt
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.319674 trl-0.4.6/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2445 2023-05-03 09:18:40.000000 trl-0.4.6/CONTRIBUTING.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.4.6/LICENSE
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.4.6/MANIFEST.in
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 09:18:14.319674 trl-0.4.6/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5413 2023-05-03 09:18:40.000000 trl-0.4.6/README.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      315 2023-06-23 09:18:14.319674 trl-0.4.6/setup.cfg
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3779 2023-06-23 09:17:08.000000 trl-0.4.6/setup.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.311673 trl-0.4.6/tests/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.4.6/tests/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_core.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_e2e.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_modeling_value_head.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_no_peft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.4.6/tests/test_peft_models.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    41226 2023-06-23 08:12:16.000000 trl-0.4.6/tests/test_ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18911 2023-06-23 08:12:16.000000 trl-0.4.6/tests/test_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.4.6/tests/testing_constants.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.4.6/tests/testing_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      407 2023-06-23 09:17:04.000000 trl-0.4.6/trl/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7920 2023-05-03 09:18:40.000000 trl-0.4.6/trl/core.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/extras/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.4.6/trl/extras/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.4.6/trl/extras/best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.4.6/trl/import_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/models/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.4.6/trl/models/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23627 2023-06-23 08:12:16.000000 trl-0.4.6/trl/models/modeling_base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    17967 2023-05-17 09:28:26.000000 trl-0.4.6/trl/models/modeling_value_head.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.319674 trl-0.4.6/trl/trainer/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1035 2023-06-21 09:04:57.000000 trl-0.4.6/trl/trainer/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.4.6/trl/trainer/base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8312 2023-06-23 09:13:55.000000 trl-0.4.6/trl/trainer/ppo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    52510 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10115 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14717 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11523 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl.egg-info/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      887 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/SOURCES.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/dependency_links.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.4.6/trl.egg-info/not-zip-safe
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      225 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/requires.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/top_level.txt
```

### Comparing `trl-0.4.5/CONTRIBUTING.md` & `trl-0.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/LICENSE` & `trl-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/PKG-INFO` & `trl-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Pytorch implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `trl-0.4.5/README.md` & `trl-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/setup.py` & `trl-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 8. Change the version in __init__.py and setup.py to X.X.X+1.dev0 (e.g. VERSION=1.18.3 -> 1.18.4.dev0).
    Then push the change with a message 'set dev version'
 """
 
 from setuptools import setup, find_packages
 
-__version__ = "0.4.5"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+__version__ = "0.4.6"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.18.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
```

### Comparing `trl-0.4.5/tests/test_best_of_n_sampler.py` & `trl-0.4.6/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_core.py` & `trl-0.4.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_modeling_value_head.py` & `trl-0.4.6/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_no_peft.py` & `trl-0.4.6/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_peft_models.py` & `trl-0.4.6/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_ppo_trainer.py` & `trl-0.4.6/tests/test_ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_reward_trainer.py` & `trl-0.4.6/tests/test_reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/test_sft_trainer.py` & `trl-0.4.6/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/testing_constants.py` & `trl-0.4.6/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/tests/testing_utils.py` & `trl-0.4.6/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/core.py` & `trl-0.4.6/trl/core.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/extras/__init__.py` & `trl-0.4.6/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/extras/best_of_n_sampler.py` & `trl-0.4.6/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/import_utils.py` & `trl-0.4.6/trl/import_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/models/__init__.py` & `trl-0.4.6/trl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/models/modeling_base.py` & `trl-0.4.6/trl/models/modeling_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/models/modeling_value_head.py` & `trl-0.4.6/trl/models/modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/__init__.py` & `trl-0.4.6/trl/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/base.py` & `trl-0.4.6/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/ppo_config.py` & `trl-0.4.6/trl/trainer/ppo_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                 existing_wandb_tag = os.environ.get("WANDB_TAGS", "")
                 wandb_tag = autotag()
                 if len(wandb_tag) > 0:
                     if len(existing_wandb_tag) > 0:
                         os.environ["WANDB_TAGS"] = ",".join([existing_wandb_tag, wandb_tag])
                     else:
                         os.environ["WANDB_TAGS"] = wandb_tag
-                logging.info(f"the following tags will be used for wandb logging: {os.environ['WANDB_TAGS']}")
+                    logging.info(f"the following tags will be used for wandb logging: {os.environ['WANDB_TAGS']}")
             except ImportError:
                 raise ImportError(
                     "Please install wandb to use wandb logging. You can do this by running `pip install wandb`."
                 )
 
         self.total_ppo_epochs = int(np.ceil(self.steps / self.batch_size))
```

### Comparing `trl-0.4.5/trl/trainer/ppo_trainer.py` & `trl-0.4.6/trl/trainer/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/reward_trainer.py` & `trl-0.4.6/trl/trainer/reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/sft_trainer.py` & `trl-0.4.6/trl/trainer/sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl/trainer/utils.py` & `trl-0.4.6/trl/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.5/trl.egg-info/PKG-INFO` & `trl-0.4.6/trl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Pytorch implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `trl-0.4.5/trl.egg-info/SOURCES.txt` & `trl-0.4.6/trl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

