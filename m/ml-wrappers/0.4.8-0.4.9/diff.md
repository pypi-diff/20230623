# Comparing `tmp/ml_wrappers-0.4.8.tar.gz` & `tmp/ml_wrappers-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml_wrappers-0.4.8.tar", last modified: Mon Apr 24 21:47:52 2023, max compression
+gzip compressed data, was "dist/ml_wrappers-0.4.9.tar", last modified: Fri May 26 18:25:01 2023, max compression
```

## Comparing `ml_wrappers-0.4.8.tar` & `ml_wrappers-0.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/gpu_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/warnings_suppressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/timestamp_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/model/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/base_wrapped_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/endpoint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/fastai_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    29204 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/image_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/predictions_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/pytorch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/tensorflow_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/text_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_without_proba_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/common/gpu_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/common/warnings_suppressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/dataset/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/dataset/timestamp_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/base_wrapped_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/endpoint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/fastai_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30214 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/image_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/predictions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/pytorch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/tensorflow_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/text_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/wrapped_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/wrapped_classification_without_proba_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/model/wrapped_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/ml_wrappers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/ml_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 18:25:01.000000 ml_wrappers-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-26 18:22:02.000000 ml_wrappers-0.4.9/setup.py
```

### Comparing `ml_wrappers-0.4.8/LICENSE.txt` & `ml_wrappers-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/PKG-INFO` & `ml_wrappers-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_wrappers
-Version: 0.4.8
+Version: 0.4.9
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.8/README.md` & `ml_wrappers-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/__init__.py` & `ml_wrappers-0.4.9/ml_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/common/constants.py` & `ml_wrappers-0.4.9/ml_wrappers/common/constants.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/common/gpu_kmeans.py` & `ml_wrappers-0.4.9/ml_wrappers/common/gpu_kmeans.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/common/warnings_suppressor.py` & `ml_wrappers-0.4.9/ml_wrappers/common/warnings_suppressor.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_utils.py` & `ml_wrappers-0.4.9/ml_wrappers/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/dataset/timestamp_featurizer.py` & `ml_wrappers-0.4.9/ml_wrappers/dataset/timestamp_featurizer.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/__init__.py` & `ml_wrappers-0.4.9/ml_wrappers/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/base_wrapped_model.py` & `ml_wrappers-0.4.9/ml_wrappers/model/base_wrapped_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/endpoint_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/endpoint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/evaluator.py` & `ml_wrappers-0.4.9/ml_wrappers/model/evaluator.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/fastai_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/fastai_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/function_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/image_model_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/image_model_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import Any, Dict, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from ml_wrappers.common.constants import ModelTask
 from ml_wrappers.dataset.dataset_wrapper import DatasetWrapper
 from ml_wrappers.model.evaluator import _eval_model
+from ml_wrappers.model.model_utils import (_is_callable_pipeline,
+                                           _is_transformers_pipeline)
 from ml_wrappers.model.pytorch_wrapper import WrappedPytorchModel
 from ml_wrappers.model.wrapped_classification_model import \
     WrappedClassificationModel
 
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
@@ -216,15 +218,16 @@
         expanded_scores[i, int(label.item())] = score
 
     return expanded_scores
 
 
 def _wrap_image_model(model, examples, model_task, is_function,
                       number_of_classes: int = None,
-                      classes: Union[list, np.array] = None):
+                      classes: Union[list, np.array] = None,
+                      device='cpu'):
     """If needed, wraps the model or function in a common API.
 
     Wraps the model based on model task and prediction function contract.
 
     :param model: The model or function to evaluate on the examples.
     :type model: function or model to wrap
     :param examples: The model evaluation examples.
@@ -237,14 +240,17 @@
     :type model_task: str
     :param classes: optional parameter specifying a list of class names
     the dataset
     :type classes: list or np.ndarray
     :param number_of_classes: optional parameter specifying the
     number of classes in the dataset
     :type number_of_classes: int
+    :param device: optional parameter specifying the device to move the model
+        to. If not specified, then cpu is the default
+    :type device: str, for instance: 'cpu', 'cuda'
     :return: The function chosen from given model and chosen domain, or
     model wrapping the function and chosen domain.
     :rtype: (function, str) or (model, str)
     """
     _wrapped_model = model
     if model_task == ModelTask.IMAGE_CLASSIFICATION:
         try:
@@ -268,15 +274,15 @@
         elif hasattr(model, '_model_impl'):
             if str(type(model._model_impl.python_model)).endswith(
                 ("azureml.automl.dnn.vision.common.mlflow." +
                     "mlflow_model_wrapper.MLFlowImagesModelWrapper'>")
             ):
                 _wrapped_model = WrappedMlflowAutomlImagesClassificationModel(
                     model)
-        else:
+        elif _is_transformers_pipeline(model) or _is_callable_pipeline(model):
             _wrapped_model = WrappedTransformerImageClassificationModel(model)
     elif model_task == ModelTask.MULTILABEL_IMAGE_CLASSIFICATION:
         if _is_fastai_model(model):
             _wrapped_model = WrappedFastAIImageClassificationModel(
                 model, multilabel=True
             )
     elif model_task == ModelTask.OBJECT_DETECTION:
@@ -285,15 +291,15 @@
                 ("azureml.automl.dnn.vision.common.mlflow." +
                     "mlflow_model_wrapper.MLFlowImagesModelWrapper'>")
             ):
                 _wrapped_model = WrappedMlflowAutomlObjectDetectionModel(
                     model, classes)
         else:
             _wrapped_model = WrappedObjectDetectionModel(
-                model, number_of_classes)
+                model, number_of_classes, device)
     return _wrapped_model, model_task
 
 
 class WrappedTransformerImageClassificationModel(object):
     """A class for wrapping a Transformers model in the scikit-learn style."""
 
     def __init__(self, model):
@@ -433,25 +439,30 @@
         return np.stack(predictions.probs.values)
 
 
 class WrappedObjectDetectionModel:
     """A class for wrapping a object detection model in the scikit-learn
         style."""
 
-    def __init__(self, model: Any, number_of_classes: int) -> None:
+    def __init__(self, model: Any, number_of_classes: int, device='cpu') -> None:
         """Initialize the WrappedObjectDetectionModel with the model
             and evaluation function.
 
         :param model: mlflow model
         :type model: Any
+        :param number_of_classes: number of distinct labels
+        :type number_of_classes: int
+        :param device: optional parameter specifying the device to move the
+            model to. If not specified, then cpu is the default
+        :type device: str, for instance: 'cpu', 'cuda'
         """
-        self._device = torch.device("cuda" if torch.cuda.is_available()
-                                    else "cpu")
+        self._device = device
         model.eval()
         model.to(self._device)
+
         self._model = model
         self._number_of_classes = number_of_classes
 
     def predict(self, x, iou_thresh: float = 0.5, score_thresh: float = 0.5):
         """Create a list of detection records from the image predictions.
 
         :param x: Tensor of the image
@@ -526,15 +537,20 @@
         :type model: mlflow.pyfunc.PyFuncModel
         :param classes: list of class names
         :type classes: list or np.array
         """
 
         self._model = model
         self._classes = classes
-        self._label_dict = {label: (i+1) for i, label in enumerate(classes)}
+        try:
+            if type(classes[0] == str):
+                self._label_dict = {label: (i+1)
+                                    for i, label in enumerate(classes)}
+        except KeyError:
+            raise KeyError("classes parameter not a list of class labels")
 
     def _mlflow_predict(self, dataset: pd.DataFrame) -> pd.DataFrame:
         """Perform the inference using the wrapped MLflow model.
 
         :param dataset: The dataset to predict on.
         :type dataset: pandas.DataFrame
         :return: The predicted data.
@@ -633,25 +649,29 @@
     To be compatible with the D-RISE explainability method,
     all models must be wrapped to have the same output and input class and a
     predict function for object detection. This wrapper is customized for the
     FasterRCNN model from Pytorch, and can also be used with the RetinaNet or
     any other models with the same output class.
     """
 
-    def __init__(self, model, number_of_classes: int):
+    def __init__(self, model, number_of_classes: int, device='cpu'):
         """Initialize the PytorchDRiseWrapper.
 
         :param model: Object detection model
         :type model: PytorchFasterRCNN model
         :param number_of_classes: Number of classes the model is predicting
         :type number_of_classes: int
+        :param device: optional parameter specifying the device to move the
+            model to. If not specified, then cpu is the default
+        :type device: str, for instance: 'cpu', 'cuda'
         """
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-        model.to(device)
+        self._device = device
+        model.to(self._device)
         model.eval()
+
         self._model = model
         self._number_of_classes = number_of_classes
 
     def predict(self, x: Tensor):
         """Create a list of detection records from the image predictions.
 
         :param x: Tensor of the image
```

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/model_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/model_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     import torch.nn as nn
 except ImportError:
     module_logger.debug(
         'Could not import torch, required if using a PyTorch model')
 
 
 def wrap_model(model, examples, model_task: str = ModelTask.UNKNOWN,
-               num_classes: int = None, classes: Union[list, np.array] = None):
+               num_classes: int = None, classes: Union[list, np.array] = None,
+               device='cpu'):
     """If needed, wraps the model in a common API based on model task and
         prediction function contract.
 
     :param model: The model to evaluate on the examples.
     :type model: model with a predict or predict_proba function.
     :param examples: The model evaluation examples.
         Note the examples will be wrapped in a DatasetWrapper, if not
@@ -66,26 +67,30 @@
     :param classes: optional parameter specifying a list of class names
         the dataset
     :type classes: list or np.ndarray
     :param num_classes: optional parameter specifying the number of classes in
         the dataset
     :type num_classes: int
     :type model_task: str
+    :param device: optional parameter specifying the device to move the model
+        to. If not specified, then cpu is the default
+    :type device: str, for instance: 'cpu', 'cuda'
     :return: The wrapper model.
     :rtype: model
     """
     if model_task == ModelTask.UNKNOWN and _is_transformers_pipeline(model):
         # TODO: can we also dynamically figure out the task if it was
         # originally unknown for text scenarios?
         raise ValueError("ModelTask must be specified for text-based models")
     if model_task in text_model_tasks:
         return _wrap_text_model(model, examples, model_task, False)[0]
     if model_task in image_model_tasks:
         return _wrap_image_model(model, examples, model_task,
-                                 False,  num_classes, classes)[0]
+                                 False,  num_classes, classes,
+                                 device)[0]
     return _wrap_model(model, examples, model_task, False)[0]
 
 
 def _wrap_model(model, examples, model_task, is_function):
     """If needed, wraps the model or function in a common API based on model
         task and prediction function contract.
```

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/predictions_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/predictions_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,20 @@
         super(PredictionsModelWrapperClassification, self).__init__(
             test_data, y_pred)
         self._num_classes = None
         if y_pred_proba is not None:
             if not isinstance(y_pred_proba, np.ndarray):
                 raise DataValidationException(
                     "Expecting a numpy array for y_pred_proba")
+
+            if len(test_data) != len(y_pred_proba):
+                raise DataValidationException(
+                    "The number of instances in test data "
+                    "do not match with number of prediction probabilities")
+
             for i in range(0, len(y_pred_proba[0])):
                 self._combined_data[
                     TARGET + '_' + str(i)] = y_pred_proba[:, i]
             self._num_classes = len(y_pred_proba[0])
 
     def predict_proba(self, query_test_data: pd.DataFrame) -> np.ndarray:
         """Return the prediction probabilities based on the query data.
```

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/pytorch_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/tensorflow_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/tensorflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/text_model_wrapper.py` & `ml_wrappers-0.4.9/ml_wrappers/model/text_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_model.py` & `ml_wrappers-0.4.9/ml_wrappers/model/wrapped_classification_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_without_proba_model.py` & `ml_wrappers-0.4.9/ml_wrappers/model/wrapped_classification_without_proba_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_regression_model.py` & `ml_wrappers-0.4.9/ml_wrappers/model/wrapped_regression_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/ml_wrappers.egg-info/PKG-INFO` & `ml_wrappers-0.4.9/ml_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-wrappers
-Version: 0.4.8
+Version: 0.4.9
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.8/ml_wrappers.egg-info/SOURCES.txt` & `ml_wrappers-0.4.9/ml_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.8/setup.py` & `ml_wrappers-0.4.9/setup.py`

 * *Files identical despite different names*

