# Comparing `tmp/ml-rwkv-0.0.4.tar.gz` & `tmp/ml-rwkv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-rwkv-0.0.4.tar", last modified: Thu Jun 22 20:29:22 2023, max compression
+gzip compressed data, was "ml-rwkv-0.0.5.tar", last modified: Fri Jun 23 02:27:46 2023, max compression
```

## Comparing `ml-rwkv-0.0.4.tar` & `ml-rwkv-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/ml_rwkv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 20:29:22.000000 ml-rwkv-0.0.4/ml_rwkv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/rwkv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/rwkv/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/rwkv/triton/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/wkv/eps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/wkv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/triton/wkv/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/rwkv/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/wkv/eps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/wkv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/rwkv/wkv/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:29:22.652034 ml-rwkv-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/tests/test_eps_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/tests/test_log_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/tests/test_vanilla_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-22 20:29:09.000000 ml-rwkv-0.0.4/tests/test_wkv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/ml_rwkv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/triton/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_eps_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_log_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_vanilla_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_wkv.py
```

### Comparing `ml-rwkv-0.0.4/LICENSE` & `ml-rwkv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/PKG-INFO` & `ml-rwkv-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.4
+Version: 0.0.5
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.4/README.md` & `ml-rwkv-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/ml_rwkv.egg-info/PKG-INFO` & `ml-rwkv-0.0.5/ml_rwkv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.4
+Version: 0.0.5
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.4/ml_rwkv.egg-info/SOURCES.txt` & `ml-rwkv-0.0.5/ml_rwkv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/pyproject.toml` & `ml-rwkv-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/rwkv/model.py` & `ml-rwkv-0.0.5/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/rwkv/run.py` & `ml-rwkv-0.0.5/rwkv/run.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/rwkv/triton/utils.py` & `ml-rwkv-0.0.5/rwkv/triton/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,7 +19,22 @@
 
         assert triton is not None
         return True
     except (ImportError, ModuleNotFoundError):
         if torch.cuda.is_available():
             warnings.warn("Triton is not installed, but CUDA is available; install with `pip install triton`")
         return False
+
+
+def largest_div_power_of_2(n: int, init_k: int = 32) -> int:
+    k = init_k
+    while k * 2 <= n:
+        k *= 2
+    return k
+
+
+def get_block_size_c(chans: int) -> int:
+    if chans < 32:
+        return 32
+    if chans < 64:
+        return 64
+    return 128
```

### Comparing `ml-rwkv-0.0.4/rwkv/triton/wkv/eps.py` & `ml-rwkv-0.0.5/rwkv/triton/wkv/eps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # mypy: disable-error-code="import, no-untyped-def, override"
 # ruff: noqa: ANN001, ANN201, ANN202, N803, N806
 """Defines Triton kernels for numerically-stable RWKV forward and backward passes."""
 
-from typing import cast
+from typing import Any, cast
 
 import torch
 import triton
 import triton.language as tl
 from torch import Tensor
 from torch.autograd.function import Function, FunctionCtx, once_differentiable
 
+from rwkv.triton.utils import get_block_size_c
 
+AUTOTUNE_CONFIGS: list[triton.Config] = [
+    triton.Config({"BLOCK_SIZE_C": 32}, num_warps=2),
+    triton.Config({"BLOCK_SIZE_C": 128}, num_warps=4),
+    triton.Config({"BLOCK_SIZE_C": 1024}, num_warps=8),
+]
+
+
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
 def wkv_triton_with_eps_forward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
@@ -48,16 +57,17 @@
     # Params
     chans,
     tsz,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     alpha_ptr = state_ptr + b_idx * state_s_b
     beta_ptr = state_ptr + b_idx * state_s_b + state_s_abe
@@ -78,57 +88,60 @@
 
     for t in range(tsz):
         kt = tl.load(k_ptr + t * k_s_t + cs * k_s_c, mask=cmask).to(tl.float32)
         vt = tl.load(v_ptr + t * v_s_t + cs * v_s_c, mask=cmask).to(tl.float32)
 
         ukt = u + kt
         tau = tl.maximum(ukt, eps)
-        e1 = tl.exp(eps - tau)
-        e2 = tl.exp(ukt - tau)
-        wkv = (e1 * alpha + e2 * vt) / (e1 * beta + e2)
+        e1a = tl.exp(eps - tau)
+        e2a = tl.exp(ukt - tau)
+        wkv = (e1a * alpha + e2a * vt) / (e1a * beta + e2a)
         tl.store(wkv_ptr + t * wkv_s_t + cs * wkv_s_c, wkv, mask=cmask)
 
         w_eps = w + eps
         eps = tl.maximum(w_eps, kt)
-        e1 = tl.exp(w_eps - eps)
-        e2 = tl.exp(kt - eps)
-        alpha = e1 * alpha + e2 * vt
-        beta = e1 * beta + e2
+        e1b = tl.exp(w_eps - eps)
+        e2b = tl.exp(kt - eps)
+        alpha = e1b * alpha + e2b * vt
+        beta = e1b * beta + e2b
         tl.store(alpha_out_ptr + t * state_out_s_t + cs * state_out_s_c, alpha, mask=cmask)
         tl.store(beta_out_ptr + t * state_out_s_t + cs * state_out_s_c, beta, mask=cmask)
         tl.store(eps_out_ptr + t * state_out_s_t + cs * state_out_s_c, eps, mask=cmask)
 
 
 def wkv_triton_with_eps_forward(
     w: Tensor,
     u: Tensor,
     k: Tensor,
     v: Tensor,
     state: Tensor,
 ) -> tuple[Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 3, 1, chans), f"{state.shape} != {(bsz, 3, 1, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     wkvs = k.new_empty(bsz, tsz, chans)
     state_out = k.new_empty(bsz, 3, tsz, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
 
-    wkv_triton_with_eps_forward_kernel[(bsz,)](
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
+
+    wkv_triton_with_eps_forward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
@@ -164,16 +177,17 @@
     )
 
     state_out = torch.cat((state, state_out), dim=2)
 
     return wkvs, state_out
 
 
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
-def wkv_with_eps_triton_backward_kernel(
+def wkv_triton_with_eps_backward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
     u_s_c,
     # K
@@ -226,16 +240,17 @@
     # Params
     tsz,
     chans,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     alpha_ptr = state_ptr + b_idx * state_s_b
     beta_ptr = state_ptr + b_idx * state_s_b + state_s_abe
@@ -352,39 +367,42 @@
     u: Tensor,
     k: Tensor,
     v: Tensor,
     state: Tensor,
     grad_wkv: Tensor,
     grad_state: Tensor,
 ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 3, tsz + 1, chans), f"{state.shape} != {(bsz, 3, tsz + 1, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
     assert grad_wkv.shape == (bsz, tsz, chans)
     assert grad_state.shape == (bsz, 3, 1, chans)
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u, grad_wkv, grad_state):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     gw = torch.zeros_like(w)
     gu = torch.zeros_like(u)
     gk = torch.empty_like(k)
     gv = torch.empty_like(v)
     gstate = k.new_empty(bsz, 3, 1, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
+
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
 
-    wkv_with_eps_triton_backward_kernel[(bsz,)](
+    wkv_triton_with_eps_backward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
```

### Comparing `ml-rwkv-0.0.4/rwkv/triton/wkv/log.py` & `ml-rwkv-0.0.5/rwkv/triton/wkv/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # mypy: disable-error-code="import, no-untyped-def, override"
 # ruff: noqa: ANN001, ANN201, ANN202, N803, N806
 """Defines Triton kernels for the log-space RWKV forward and backward passes."""
 
 import math
-from typing import cast
+from typing import Any, cast
 
 import torch
 import triton
 import triton.language as tl
 from torch import Tensor
 from torch.autograd.function import Function, FunctionCtx, once_differentiable
 
+from rwkv.triton.utils import get_block_size_c
 from rwkv.wkv.log import EPS
 
+AUTOTUNE_CONFIGS: list[triton.Config] = [
+    triton.Config({"BLOCK_SIZE_C": 32}, num_warps=2),
+    triton.Config({"BLOCK_SIZE_C": 128}, num_warps=4),
+    triton.Config({"BLOCK_SIZE_C": 1024}, num_warps=8),
+]
+
 
 @triton.jit
 def logaddexp(a, b):
     max_ab = tl.maximum(a, b)
     return max_ab + tl.log(tl.exp(a - max_ab) + tl.exp(b - max_ab))
 
 
 @triton.jit
 def logsubexp(a, b, log_eps: tl.constexpr):
     max_ab = tl.maximum(tl.maximum(a, b), log_eps)
     return max_ab + tl.log(tl.exp(a - max_ab) - tl.exp(b - max_ab))
 
 
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
 def wkv_triton_log_space_forward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
@@ -66,16 +74,17 @@
     eps: tl.constexpr,
     log_eps: tl.constexpr,
     normalize: tl.constexpr,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     ln_alpha_p_ptr = state_ptr + b_idx * state_s_b
     ln_alpha_m_ptr = state_ptr + b_idx * state_s_b + state_s_abe
@@ -126,34 +135,37 @@
     u: Tensor,
     k: Tensor,
     v: Tensor,
     state: Tensor,
     eps: float = EPS,
     normalize: bool = False,
 ) -> tuple[Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 3, 1, chans), f"{state.shape} != {(bsz, 3, 1, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     wkvs = k.new_empty(bsz, tsz, chans)
     state_out = k.new_empty(bsz, 3, tsz, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
+
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
 
-    wkv_triton_log_space_forward_kernel[(bsz,)](
+    wkv_triton_log_space_forward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
@@ -192,16 +204,17 @@
     )
 
     state_out = torch.cat((state, state_out), dim=2)
 
     return wkvs, state_out
 
 
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
-def wkv_log_space_triton_backward_kernel(
+def wkv_triton_log_space_backward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
     u_s_c,
     # K
@@ -255,16 +268,17 @@
     tsz,
     chans,
     eps: tl.constexpr,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     alpha_p_ptr = state_ptr + b_idx * state_s_b
     alpha_m_ptr = state_ptr + b_idx * state_s_b + state_s_abe
@@ -379,39 +393,42 @@
     k: Tensor,
     v: Tensor,
     state: Tensor,
     grad_wkv: Tensor,
     grad_state: Tensor,
     eps: float = EPS,
 ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 3, tsz, chans), f"{state.shape} != {(bsz, 3, tsz, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
     assert grad_wkv.shape == (bsz, tsz, chans)
     assert grad_state.shape == (bsz, 3, 1, chans)
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u, grad_wkv, grad_state):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     gw = torch.zeros_like(w)
     gu = torch.zeros_like(u)
     gk = torch.empty_like(k)
     gv = torch.empty_like(v)
     gstate = k.new_empty(bsz, 3, 1, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
 
-    wkv_log_space_triton_backward_kernel[(bsz,)](
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
+
+    wkv_triton_log_space_backward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
@@ -509,7 +526,15 @@
     k: Tensor,
     v: Tensor,
     state: Tensor,
     eps: float = EPS,
     normalize: bool = False,
 ) -> tuple[Tensor, Tensor]:
     return WKVTritonFunction.apply(w, u, k, v, state, eps, normalize)
+
+
+def run_benchmark() -> None:
+    pass
+
+
+if __name__ == "__main__":
+    run_benchmark()
```

### Comparing `ml-rwkv-0.0.4/rwkv/triton/wkv/vanilla.py` & `ml-rwkv-0.0.5/rwkv/triton/wkv/vanilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,32 @@
 """Defines Triton kernels for the vanilla RWKV forward and backward passes.
 
 This kernel is used to make the WKV computation in the attention layer run
 faster while using less memory. It requires that ``triton`` is installed, which
 in turn requires a ``triton``-compatible GPU and CUDA version.
 """
 
-from typing import cast
+from typing import Any, cast
 
 import torch
 import triton
 import triton.language as tl
 from torch import Tensor
 from torch.autograd.function import Function, FunctionCtx, once_differentiable
 
+from rwkv.triton.utils import get_block_size_c
 
+AUTOTUNE_CONFIGS: list[triton.Config] = [
+    triton.Config({"BLOCK_SIZE_C": 32}, num_warps=2),
+    triton.Config({"BLOCK_SIZE_C": 128}, num_warps=4),
+    triton.Config({"BLOCK_SIZE_C": 1024}, num_warps=8),
+]
+
+
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
 def wkv_triton_vanilla_forward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
@@ -53,16 +62,17 @@
     # Params
     chans,
     tsz,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     alpha_ptr = state_ptr + b_idx * state_s_b
     beta_ptr = state_ptr + b_idx * state_s_b + state_s_ab
@@ -81,53 +91,54 @@
     ew = tl.exp(w)
 
     for t in range(tsz):
         kt = tl.load(k_ptr + t * k_s_t + cs * k_s_c, mask=cmask).to(tl.float32)
         vt = tl.load(v_ptr + t * v_s_t + cs * v_s_c, mask=cmask).to(tl.float32)
 
         euk = tl.exp(u + kt)
-
         wkv = (alpha + euk * vt) / (beta + euk)
         tl.store(wkv_ptr + t * wkv_s_t + cs * wkv_s_c, wkv, mask=cmask)
 
         ek = tl.exp(kt)
         alpha = ew * alpha + ek * vt
         beta = ew * beta + ek
-
         tl.store(alpha_out_ptr + t * state_out_s_t + cs * state_out_s_c, alpha, mask=cmask)
         tl.store(beta_out_ptr + t * state_out_s_t + cs * state_out_s_c, beta, mask=cmask)
 
 
 def wkv_triton_vanilla_forward(
     w: Tensor,
     u: Tensor,
     k: Tensor,
     v: Tensor,
     state: Tensor,
 ) -> tuple[Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 2, 1, chans), f"{state.shape} != {(bsz, 2, 1, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     wkvs = k.new_empty(bsz, tsz, chans)
     state_out = k.new_empty(bsz, 2, tsz, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
+
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
 
-    wkv_triton_vanilla_forward_kernel[(bsz,)](
+    wkv_triton_vanilla_forward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
@@ -163,16 +174,17 @@
     )
 
     state_out = torch.cat((state, state_out), dim=2)
 
     return wkvs, state_out
 
 
+# @triton.autotune(configs=AUTOTUNE_CONFIGS, key=["chans"])
 @triton.jit
-def wkv_vanilla_triton_backward_kernel(
+def wkv_triton_vanilla_backward_kernel(
     # W
     w_ptr,
     w_s_c,
     # U
     u_ptr,
     u_s_c,
     # K
@@ -225,16 +237,17 @@
     # Params
     tsz,
     chans,
     BLOCK_SIZE_C: tl.constexpr,
 ):
     # Parallelize over the batch dimension.
     b_idx = tl.program_id(0)
+    c_idx = tl.program_id(1)
 
-    cs = tl.arange(0, BLOCK_SIZE_C)
+    cs = (c_idx * BLOCK_SIZE_C) + tl.arange(0, BLOCK_SIZE_C)
     cmask = cs < chans
 
     # Pointers to the batch (and possibly channel) for the input tensors.
     k_ptr = k_ptr + b_idx * k_s_b
     v_ptr = v_ptr + b_idx * v_s_b
     alpha_ptr = state_ptr + b_idx * state_s_b
     beta_ptr = state_ptr + b_idx * state_s_b + state_s_ab
@@ -319,39 +332,42 @@
     u: Tensor,
     k: Tensor,
     v: Tensor,
     state: Tensor,
     grad_wkv: Tensor,
     grad_state: Tensor,
 ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
-    (bsz, tsz, chans), device, dtype = k.shape, k.device, k.dtype
+    (bsz, tsz, chans), device = k.shape, k.device
 
     # Checks tensor shapes.
     assert v.shape == (bsz, tsz, chans), f"{v.shape} != {(bsz, tsz, chans)}"
     assert state.shape == (bsz, 2, tsz, chans), f"{state.shape} != {(bsz, 2, tsz, chans)}"
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
     assert grad_wkv.shape == (bsz, tsz, chans)
     assert grad_state.shape == (bsz, 2, 1, chans)
 
-    # Checks tensor dtypes and devices.
+    # Checks tensor devices.
     for t in (v, state, w, u, grad_wkv, grad_state):
-        assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
+        assert t.device == device, f"{t.device} != {device}"
 
     # New tensors to output.
     gw = torch.zeros_like(w)
     gu = torch.zeros_like(u)
     gk = torch.empty_like(k)
     gv = torch.empty_like(v)
     gstate = k.new_empty(bsz, 2, 1, chans)
 
     # Constants.
-    block_size_c = max(triton.next_power_of_2(chans), 32)
+    block_size_c = get_block_size_c(chans)
+
+    def grid(meta: dict[str, Any]) -> tuple[int, ...]:
+        return (bsz, triton.cdiv(chans, meta["BLOCK_SIZE_C"]))
 
-    wkv_vanilla_triton_backward_kernel[(bsz,)](
+    wkv_triton_vanilla_backward_kernel[grid](
         # W
         w,
         w.stride(0),
         # U
         u,
         u.stride(0),
         # K
```

### Comparing `ml-rwkv-0.0.4/rwkv/wkv/__init__.py` & `ml-rwkv-0.0.5/rwkv/wkv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def get_default_impl() -> WkvImpl:
     if "WKV_IMPL" in os.environ:
         assert (wkv_impl := os.environ["WKV_IMPL"]) in get_args(WkvImpl)
         return cast(WkvImpl, wkv_impl)
 
     warnings.warn("WKV_IMPL environment variable not set; using default")
-    return "log"
+    return "eps"
 
 
 def get_wkv_fn(emb_dim: int, impl: WkvImpl | None = None, use_triton: bool = True) -> tuple[WkvFn, WkvInitState]:
     """Returns the WKV function to use and the hidden state.
 
     The function takes the
```

### Comparing `ml-rwkv-0.0.4/rwkv/wkv/eps.py` & `ml-rwkv-0.0.5/rwkv/wkv/eps.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/rwkv/wkv/log.py` & `ml-rwkv-0.0.5/rwkv/wkv/log.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/rwkv/wkv/vanilla.py` & `ml-rwkv-0.0.5/rwkv/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/setup.py` & `ml-rwkv-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/tests/test_eps_wkv.py` & `ml-rwkv-0.0.5/tests/test_eps_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/tests/test_log_wkv.py` & `ml-rwkv-0.0.5/tests/test_log_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/tests/test_vanilla_wkv.py` & `ml-rwkv-0.0.5/tests/test_vanilla_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.4/tests/test_wkv.py` & `ml-rwkv-0.0.5/tests/test_wkv.py`

 * *Files identical despite different names*

