# Comparing `tmp/tensor_parallel-1.2.7.tar.gz` & `tmp/tensor_parallel-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.7.tar", last modified: Tue Jun 20 16:48:59 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.8.tar", last modified: Fri Jun 23 13:23:29 2023, max compression
```

## Comparing `tensor_parallel-1.2.7.tar` & `tensor_parallel-1.2.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:48:59.689957 tensor_parallel-1.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-20 16:48:59.000000 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 16:48:59.000000 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:48:59.000000 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 16:48:59.000000 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 16:48:59.000000 tensor_parallel-1.2.7/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:48:59.693957 tensor_parallel-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-20 16:48:44.000000 tensor_parallel-1.2.7/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.771500 tensor_parallel-1.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.779501 tensor_parallel-1.2.8/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.779501 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.7/LICENCE` & `tensor_parallel-1.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/PKG-INFO` & `tensor_parallel-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.7
+Version: 1.2.8
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.7 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.8 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.7/README.md` & `tensor_parallel-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/setup.cfg` & `tensor_parallel-1.2.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.7
+version = 1.2.8
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.8/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.8/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.8/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.8/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/config.py` & `tensor_parallel-1.2.8/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.8/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.8/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.8/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.8/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.8/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.8/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.8/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.8/src/tensor_parallel/slicing_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,16 @@
                 world_size=world_size, dim=1, chunk_size=q_per_kv * head_dim
             ),
             # MLP
             r".*mlp\.dense_h_to_4h\.weight$": Split(world_size=world_size, dim=0),
             r".*mlp\.dense_4h_to_h\.weight$": Split(world_size=world_size, dim=1),
             # RWModel
             r".*word_embeddings\.weight$": Split(world_size=world_size, dim=1),
+            # RWForCausalLM
+            r".*lm_head\.weight$": Split(world_size=world_size, dim=1),
         },
         input_rules={
             r".*self_attention$": {"layer_past": select_kv_for_rank},
             r".*lm_head$": {0: "split -1"},  # note: we need to split lm_head inputs because
             # ... lm_head's weights (tied embeddings) are already split across input dimension
         },
         output_rules={
```

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.8/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.8/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.8/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.8/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.8/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.7
+Version: 1.2.8
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.7 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.8 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.7/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.8/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/tests/test_basic.py` & `tensor_parallel-1.2.8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/tests/test_factory.py` & `tensor_parallel-1.2.8/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/tests/test_integration.py` & `tensor_parallel-1.2.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/tests/test_saving.py` & `tensor_parallel-1.2.8/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.7/tests/test_transformers.py` & `tensor_parallel-1.2.8/tests/test_transformers.py`

 * *Files identical despite different names*

