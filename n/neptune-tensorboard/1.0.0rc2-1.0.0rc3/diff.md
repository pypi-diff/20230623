# Comparing `tmp/neptune_tensorboard-1.0.0rc2.tar.gz` & `tmp/neptune_tensorboard-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_tensorboard-1.0.0rc2.tar", max compression
+gzip compressed data, was "neptune_tensorboard-1.0.0rc3.tar", max compression
```

## Comparing `neptune_tensorboard-1.0.0rc2.tar` & `neptune_tensorboard-1.0.0rc3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      767 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/README.md
--rw-r--r--   0        0        0     2792 2023-06-14 08:02:10.005843 neptune_tensorboard-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      820 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/__init__.py
--rw-r--r--   0        0        0     4872 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/__init__.py
--rw-r--r--   0        0        0     5605 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/pytorch_integration.py
--rw-r--r--   0        0        0     5662 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorboardx_integration.py
--rw-r--r--   0        0        0     3563 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorflow_integration.py
--rw-r--r--   0        0        0      292 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/utils.py
--rw-r--r--   0        0        0      742 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/version.py
--rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      948 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/README.md
+-rw-r--r--   0        0        0     2928 2023-06-23 07:20:54.616009 neptune_tensorboard-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      820 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/__init__.py
+-rw-r--r--   0        0        0     4964 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/__init__.py
+-rw-r--r--   0        0        0     5671 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/pytorch_integration.py
+-rw-r--r--   0        0        0     5728 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/tensorboardx_integration.py
+-rw-r--r--   0        0        0     3606 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/tensorflow_integration.py
+-rw-r--r--   0        0        0      292 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/utils.py
+-rw-r--r--   0        0        0      760 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/version.py
+-rw-r--r--   0        0        0       80 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/sync/__init__.py
+-rw-r--r--   0        0        0     3705 2023-06-23 07:20:38.059774 neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/sync/sync_impl.py
+-rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc3/PKG-INFO
```

### Comparing `neptune_tensorboard-1.0.0rc2/CHANGELOG.md` & `neptune_tensorboard-1.0.0rc3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-tensorboard 1.0.0.pre3
+
+### Changes
+- Add support to export existing Tensorboard logs via CLI plugin ([#59](https://github.com/neptune-ai/neptune-tensorboard/pull/59/))
+
 ## neptune-tensorboard 1.0.0.pre2
 
 ### Changes
 - Update integration to work with tensorboardX's SummaryWriter ([#56](https://github.com/neptune-ai/neptune-tensorboard/pull/56))
 
 ## neptune-tensorboard 1.0.0.pre1
```

### Comparing `neptune_tensorboard-1.0.0rc2/LICENSE` & `neptune_tensorboard-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc2/pyproject.toml` & `neptune_tensorboard-1.0.0rc3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 python = "^3.7"
 
 # Python lack of functionalities from future versions
 importlib-metadata = { version = "*", python = "<3.8" }
 tensorflow = { version = ">=2.0.0", optional = true }
 torch = { version = ">=1.9.0", optional = true }
 tensorboardX = { version = ">=2.2.0", optional = true }
+tbparse = { version = "*", optional = true }
 
 # dev
 pre-commit = { version = "*", optional = true }
 pytest = { version = ">=5.0", optional = true }
 pytest-cov = { version = "2.10.1", optional = true }
 pytest-xdist = { version = "*", optional = true }
 pydot = { version = "*", optional = true }
@@ -41,15 +42,15 @@
 repository = "https://github.com/neptune-ai/neptune-tensorboard"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorboard"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-tensorboard"
 readme = "README.md"
-version = "1.0.0-pre.2"
+version = "1.0.0-pre.3"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
@@ -95,7 +96,10 @@
 profile = "black"
 line_length = 120
 force_grid_wrap = 2
 
 [tool.flake8]
 max-line-length = 120
 extend-ignore = "E203"
+
+[tool.poetry.plugins."neptune.plugins"]
+"tensorboard" = "neptune_tensorboard_plugin:sync"
```

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/__init__.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/__init__.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,18 @@
         try:
             # noinspection PyUnresolvedReferences
             version = parse_version(tf.version.VERSION)
 
             if version >= parse_version(MIN_TF_VERSION):
                 return
         except AttributeError:
+            # user facing
             message = (
-                f"Unrecognized tensorflow version: {version}. Please make sure "
-                "that the tensorflow version is >={MIN_TF_VERSION}"
+                f"Unrecognized TensorFlow version: {version}. Please make sure "
+                "that the TensorFlow version is >={MIN_TF_VERSION}"
             )
             raise Exception(message)
 
 
 if IS_PYT_AVAILABLE:
     MIN_PT_VERSION = "1.9.0"
     import torch
@@ -76,14 +77,15 @@
         try:
             # noinspection PyUnresolvedReferences
             version = parse_version(torch.__version__)
 
             if version >= parse_version(MIN_PT_VERSION):
                 return
         except AttributeError:
+            # user facing
             message = (
                 f"Unrecognized PyTorch version: {version}. Please make sure "
                 "that the PyTorch version is >={MIN_PT_VERSION}"
             )
             raise Exception(message)
 
 
@@ -101,23 +103,25 @@
         try:
             # noinspection PyUnresolvedReferences
             version = parse_version(tensorboardX.__version__)
 
             if version >= parse_version(MIN_TBX_VERSION):
                 return
         except AttributeError:
+            # user facing
             message = (
                 f"Unrecognized tensorboardX version: {version}. Please make sure "
                 "that the tensorboardX version is >={MIN_TBX_VERSION}"
             )
             raise Exception(message)
 
 
+# user facing
 FRAMEWORK_NOT_FOUND_WARNING_MSG = (
-    "neptune-tensorboard: Tensorflow or PyTorch or tensorboardX was not found, ",
+    "neptune-tensorboard: TensorFlow or PyTorch or tensorboardX was not found, ",
     "please ensure that it is available.",
 )
 
 
 def enable_tensorboard_logging(run, *, base_namespace="tensorboard"):
     if IS_TF_AVAILABLE:
         check_tf_version()
```

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/pytorch_integration.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/pytorch_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     # dataformats : CHW, HWC, HW, WH
     if dataformats == "NCHW":
         # convert to HWC
         img_tensor = img_tensor.movedim(1, 3)
     elif dataformats == "NHWC":
         pass
     else:
+        # user facing
         warnings.warn("neptune-tensorboard: Skipping logging images as  {dataformats} is not supported.")
 
     for idx in range(img_tensor.shape[0]):
         run[base_namespace]["images"][tag].append(File.as_image(img_tensor[idx]))
 
 
 def track_figure(
@@ -89,18 +90,20 @@
     run[base_namespace]["text"][tag].append(text_string)
 
 
 def track_graph(
     summary_writer, model, input_to_model=None, verbose=False, use_strict_trace=True, run=None, base_namespace=None
 ):
     if not IS_TORCHVIZ_AVAILABLE:
+        # user facing
         msg = "neptune-tensorboard: Skipping model visualization because no torchviz installation was found."
         warnings.warn(msg)
         return
     if input_to_model is None:
+        # user facing
         msg = "neptune-tensorboard: Skipping model visualization because input_to_model was None."
         warnings.warn(msg)
         return
     output = model(input_to_model)
     graph = torchviz.make_dot(output, params=dict(model.named_parameters()))
     png_bytes = graph.pipe(format="png")
     run[base_namespace]["graph"].upload(File.from_content(png_bytes, extension="png"))
```

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorboardx_integration.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/tensorboardx_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     # dataformats : CHW, HWC, HW, WH
     if dataformats == "NCHW":
         # convert to HWC
         img_tensor = img_tensor.movedim(1, 3)
     elif dataformats == "NHWC":
         pass
     else:
+        # user facing
         warnings.warn("neptune-tensorboard: Skipping logging images as  {dataformats} is not supported.")
 
     for idx in range(img_tensor.shape[0]):
         run[base_namespace]["images"][tag].append(File.as_image(img_tensor[idx]))
 
 
 def track_figure(
@@ -89,18 +90,20 @@
     run[base_namespace]["text"][tag].append(text_string)
 
 
 def track_graph(
     summary_writer, model, input_to_model=None, verbose=False, use_strict_trace=True, run=None, base_namespace=None
 ):
     if not IS_TORCHVIZ_AVAILABLE:
+        # user facing
         msg = "neptune-tensorboard: Skipping model visualization because no torchviz installation was found."
         warnings.warn(msg)
         return
     if input_to_model is None:
+        # user facing
         msg = "neptune-tensorboard: Skipping model visualization because input_to_model was None."
         warnings.warn(msg)
         return
     output = model(input_to_model)
     graph = torchviz.make_dot(output, params=dict(model.named_parameters()))
     png_bytes = graph.pipe(format="png")
     run[base_namespace]["graph"].upload(File.from_content(png_bytes, extension="png"))
```

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorflow_integration.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/tensorflow_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 def track_graph(graph_data, run=None, base_namespace=None):
     if IS_GRAPHLIB_AVAILABLE:
         graph = tfg.board(graph_data)
         png_bytes = graph.pipe(format="png")
         # There is only one graph
         run[base_namespace]["graph"].upload(File.from_content(png_bytes, extension="png"))
     else:
-        warnings.warn("Skipping model visualization because no tfgraphviz installation was found.")
+        # user facing
+        warnings.warn("neptune-tensorboard: Skipping model visualization because no tfgraphviz installation was found.")
 
 
 class NeptuneTensorflowTracker(contextlib.AbstractContextManager):
     def __init__(self, run, base_namespace):
         self.org_scalar = tf.summary.scalar
         self.org_image = tf.summary.image
         self.org_text = tf.summary.text
```

### Comparing `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/version.py` & `neptune_tensorboard-1.0.0rc3/src/neptune_tensorboard/integration/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 else:
     from importlib_metadata import (
         PackageNotFoundError,
         version,
     )
 
 if not (find_spec("neptune") or find_spec("neptune-client")):
+    # user facing
     msg = """
             The Neptune client library was not found.
 
             Install the neptune package with
                 `pip install neptune`
 
             Need help? -> https://docs.neptune.ai/setup/installation/"""
```

