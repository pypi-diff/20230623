# Comparing `tmp/torchlie-0.0.1.dev5.tar.gz` & `tmp/torchlie-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlie-0.0.1.dev5.tar", last modified: Fri Jun  2 21:06:38 2023, max compression
+gzip compressed data, was "torchlie-0.0.1rc1.tar", last modified: Fri Jun 23 04:49:21 2023, max compression
```

## Comparing `torchlie-0.0.1.dev5.tar` & `torchlie-0.0.1rc1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.101780 torchlie-0.0.1.dev5/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 21:06:38.100315 torchlie-0.0.1.dev5/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/README.md
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.048425 torchlie-0.0.1.dev5/lie/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      583 2023-06-02 20:20:32.000000 torchlie-0.0.1.dev5/lie/__init__.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.078567 torchlie-0.0.1.dev5/lie/functional/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-02 17:13:39.000000 torchlie-0.0.1.dev5/lie/functional/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/check_contexts.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-02 16:51:55.000000 torchlie-0.0.1.dev5/lie/functional/constants.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/lie_group.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32686 2023-06-02 19:50:24.000000 torchlie-0.0.1.dev5/lie/functional/se3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35973 2023-06-02 19:39:01.000000 torchlie-0.0.1.dev5/lie/functional/so3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/functional/utils.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/lie_tensor.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2166 2023-06-02 20:21:09.000000 torchlie-0.0.1.dev5/lie/options.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/lie/types.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-02 21:06:38.102854 torchlie-0.0.1.dev5/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-31 14:51:18.000000 torchlie-0.0.1.dev5/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-02 21:06:38.095300 torchlie-0.0.1.dev5/torchlie.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      402 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-06-02 21:06:37.000000 torchlie-0.0.1.dev5/torchlie.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.223213 torchlie-0.0.1rc1/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1088 2023-06-23 04:44:04.000000 torchlie-0.0.1rc1/LICENSE
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       43 2023-06-23 04:43:58.000000 torchlie-0.0.1rc1/MANIFEST.in
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-23 04:49:21.221901 torchlie-0.0.1rc1/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/README.md
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-23 04:49:21.224185 torchlie-0.0.1rc1/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1199 2023-06-23 03:50:52.000000 torchlie-0.0.1rc1/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.176507 torchlie-0.0.1rc1/torchlie/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      582 2023-06-23 04:07:46.000000 torchlie-0.0.1rc1/torchlie/__init__.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.217637 torchlie-0.0.1rc1/torchlie/functional/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/check_contexts.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/constants.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/lie_group.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32701 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/se3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35989 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/so3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/utils.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/lie_tensor.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2262 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/options.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/types.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.191102 torchlie-0.0.1rc1/torchlie.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      477 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        9 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/top_level.txt
```

### Comparing `torchlie-0.0.1.dev5/PKG-INFO` & `torchlie-0.0.1rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev5
+Version: 0.0.1rc1
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `torchlie-0.0.1.dev5/lie/__init__.py` & `torchlie-0.0.1rc1/torchlie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.0.1.dev5"
+__version__ = "0.0.1.rc1"
 
 from .types import ltype, SE3, SO3
 from .lie_tensor import (  # usort: skip
     LieTensor,
     adj,
     as_euclidean,
     as_lietensor,
```

### Comparing `torchlie-0.0.1.dev5/lie/functional/check_contexts.py` & `torchlie-0.0.1rc1/torchlie/functional/check_contexts.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev5/lie/functional/constants.py` & `torchlie-0.0.1rc1/torchlie/functional/constants.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev5/lie/functional/lie_group.py` & `torchlie-0.0.1rc1/torchlie/functional/lie_group.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev5/lie/functional/se3_impl.py` & `torchlie-0.0.1rc1/torchlie/functional/se3_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from typing import cast, List, Tuple, Optional
 
-from lie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
+from torchlie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
 from . import constants, lie_group, so3_impl as SO3
 from .check_contexts import checks_base
 from .utils import get_module, shape_err_msg
 
 
 NAME: str = "SE3"
 DIM: int = 6
@@ -410,29 +410,29 @@
     two_cosine_minus_two_nz: torch.Tensor,
     a: torch.Tensor,
     b: torch.Tensor,
 ):
     ret_lin = tangent_vector[..., :3]
     ret_ang = tangent_vector[..., 3:]
     size = get_tangent_vector_size(tangent_vector)
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    d_near_zero = theta < LIE_OPTS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
     jac = tangent_vector.new_zeros(*size, 6, 6)
     jac[..., :3, :3], (b_ret_ang,) = SO3._jlog_impl_helper(ret_ang, theta, sine, cosine)
     jac[..., 3:, 3:] = jac[..., :3, :3]
 
-    theta_nz = torch.where(near_zero, constants._NON_ZERO, theta)
+    theta_nz = torch.where(d_near_zero, constants._NON_ZERO, theta)
     theta4_nz = theta2_nz**2
     c = torch.where(
-        near_zero,
+        d_near_zero,
         -1 / 360.0 - theta2 / 7560.0,
         -(2 * two_cosine_minus_two_nz + theta * sine + theta2)
         / (theta4_nz * two_cosine_minus_two_nz),
     )
     d = torch.where(
-        near_zero,
+        d_near_zero,
         -1 / 6.0 - theta2 / 180.0,
         (theta - sine) / (theta_nz * two_cosine_minus_two_nz),
     )
 
     e = ret_ang.view(*size, 1, 3) @ ret_lin.view(*size, 3, 1)
     e = e.view(*size) if len(size) > 0 else e.squeeze()
```

### Comparing `torchlie-0.0.1.dev5/lie/functional/so3_impl.py` & `torchlie-0.0.1rc1/torchlie/functional/so3_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from typing import cast, List, Tuple, Optional
 
-from lie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
+from torchlie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
 from . import constants, lie_group
 from .check_contexts import checks_base
 from .utils import (
     get_module,
     shape_err_msg,
     permute_op_dim,
     unpermute_op_dim,
@@ -378,15 +378,15 @@
         1 + sine**2 / 6,
         theta / sine_nz,
     )
     ret = sine_axis * scale.view(*size, 1)
 
     # # theta ~ pi
     ddiag = torch.diagonal(group, dim1=-1, dim2=-2)
-    # Find the index of major coloumns and diagonals
+    # Find the index of major columns and diagonals
     major = torch.logical_and(
         ddiag[..., 1] > ddiag[..., 0], ddiag[..., 1] > ddiag[..., 2]
     ) + 2 * torch.logical_and(
         ddiag[..., 2] > ddiag[..., 0], ddiag[..., 2] > ddiag[..., 1]
     )
     major = major.view(-1)
     aux = torch.ones(size, dtype=torch.bool)
@@ -415,26 +415,26 @@
 def _jlog_impl_helper(
     tangent_vector: torch.Tensor,
     theta: torch.Tensor,
     sine: torch.Tensor,
     cosine: torch.Tensor,
 ):
     size = get_tangent_vector_size(tangent_vector)
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    d_near_zero = theta < LIE_OPTS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
-        near_zero, constants._NON_ZERO, two_cosine_minus_two
+        d_near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
-    theta2_nz = torch.where(near_zero, constants._NON_ZERO, theta2)
+    theta2_nz = torch.where(d_near_zero, constants._NON_ZERO, theta2)
 
-    a = torch.where(near_zero, 1 - theta2 / 12, -sine_theta / two_cosine_minus_two_nz)
+    a = torch.where(d_near_zero, 1 - theta2 / 12, -sine_theta / two_cosine_minus_two_nz)
     b = torch.where(
-        near_zero,
+        d_near_zero,
         1.0 / 12 + theta2 / 720,
         (sine_theta + two_cosine_minus_two) / (theta2_nz * two_cosine_minus_two_nz),
     )
 
     b_tangent_vector = b.view(*size, 1) * tangent_vector
     jac = b_tangent_vector.view(*size, 3, 1) * tangent_vector.view(*size, 1, 3)
```

### Comparing `torchlie-0.0.1.dev5/lie/functional/utils.py` & `torchlie-0.0.1rc1/torchlie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev5/lie/lie_tensor.py` & `torchlie-0.0.1rc1/torchlie/lie_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 
 
 class _LieAsEuclideanContext:
     contexts = threading.local()
 
     @classmethod
     def get_context(cls):
-        if not hasattr(cls.contexts, "as_eucledian"):
-            cls.contexts.as_eucledian = False
-        return cls.contexts.as_eucledian
+        if not hasattr(cls.contexts, "as_euclidean"):
+            cls.contexts.as_euclidean = False
+        return cls.contexts.as_euclidean
 
     @classmethod
-    def set_context(cls, as_eucledian: bool):
-        cls.contexts.as_eucledian = as_eucledian
+    def set_context(cls, as_euclidean: bool):
+        cls.contexts.as_euclidean = as_euclidean
 
 
 class as_euclidean:
     def __init__(self) -> None:
         self.prev = _LieAsEuclideanContext.get_context()
         _LieAsEuclideanContext.set_context(True)
```

### Comparing `torchlie-0.0.1.dev5/lie/options.py` & `torchlie-0.0.1rc1/torchlie/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,20 +38,22 @@
         _CHECK_DTYPE_SUPPORTED(dtype)
         attr_name = f"{ltype}_{attr}_eps_{str(dtype)[6:]}"
         return getattr(self, attr_name)
 
     def reset(self) -> None:
         self.so3_near_pi_eps_float32 = 1e-2
         self.so3_near_zero_eps_float32 = 1e-2
+        self.so3_d_near_zero_eps_float32 = 2e-1
         self.so3_matrix_eps_float32 = 4e-4
         self.so3_quat_eps_float32 = 2e-4
         self.so3_hat_eps_float32 = 5e-6
         self.se3_hat_eps_float32 = 5e-6
         self.so3_near_pi_eps_float64 = 1e-7
         self.so3_near_zero_eps_float64 = 5e-3
+        self.so3_d_near_zero_eps_float64 = 1e-2
         self.so3_matrix_eps_float64 = 1e-6
         self.so3_quat_eps_float64 = 5e-7
         self.so3_hat_eps_float64 = 5e-7
         self.se3_hat_eps_float64 = 5e-7
 
 
 _TORCHLIE_GLOBAL_OPTIONS = _TorchLieOptions()
```

### Comparing `torchlie-0.0.1.dev5/lie/types.py` & `torchlie-0.0.1rc1/torchlie/types.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev5/setup.py` & `torchlie-0.0.1rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 import setuptools
 from pathlib import Path
 
-lie_path = Path("lie")
+lie_path = Path("torchlie")
 with open(lie_path / "__init__.py", "r") as f:
     for line in f:
         if "__version__" in line:
             version = line.split("__version__ = ")[1].rstrip().strip('"')
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -21,15 +21,15 @@
     version=version,
     author="Meta Research",
     description="Torch extension for differentiable Lie groups.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/theseus/lie",
     keywords="lie groups, differentiable optimization",
-    packages=["lie", "lie.functional"],
+    packages=["torchlie", "torchlie.functional"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     python_requires=">=3.8",
```

### Comparing `torchlie-0.0.1.dev5/torchlie.egg-info/PKG-INFO` & `torchlie-0.0.1rc1/torchlie.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev5
+Version: 0.0.1rc1
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

