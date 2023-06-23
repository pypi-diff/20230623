# Comparing `tmp/ml-rwkv-0.0.5.tar.gz` & `tmp/ml-rwkv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-rwkv-0.0.5.tar", last modified: Fri Jun 23 02:27:46 2023, max compression
+gzip compressed data, was "ml-rwkv-0.0.6.tar", last modified: Fri Jun 23 02:50:47 2023, max compression
```

## Comparing `ml-rwkv-0.0.5.tar` & `ml-rwkv-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/ml_rwkv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 02:27:46.000000 ml-rwkv-0.0.5/ml_rwkv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/triton/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/eps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/triton/wkv/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/rwkv/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/eps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/rwkv/wkv/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:27:46.186287 ml-rwkv-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_eps_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_log_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_vanilla_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-23 02:27:34.000000 ml-rwkv-0.0.5/tests/test_wkv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.746095 ml-rwkv-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:50:47.746095 ml-rwkv-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.742095 ml-rwkv-0.0.6/ml_rwkv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 02:50:47.000000 ml-rwkv-0.0.6/ml_rwkv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.742095 ml-rwkv-0.0.6/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.742095 ml-rwkv-0.0.6/rwkv/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.742095 ml-rwkv-0.0.6/rwkv/triton/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/triton/wkv/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.746095 ml-rwkv-0.0.6/rwkv/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/rwkv/wkv/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 02:50:47.746095 ml-rwkv-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:47.746095 ml-rwkv-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/tests/test_eps_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/tests/test_log_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/tests/test_vanilla_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-23 02:50:36.000000 ml-rwkv-0.0.6/tests/test_wkv.py
```

### Comparing `ml-rwkv-0.0.5/LICENSE` & `ml-rwkv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/PKG-INFO` & `ml-rwkv-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.5
+Version: 0.0.6
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.5/README.md` & `ml-rwkv-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/ml_rwkv.egg-info/PKG-INFO` & `ml-rwkv-0.0.6/ml_rwkv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.5
+Version: 0.0.6
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.5/ml_rwkv.egg-info/SOURCES.txt` & `ml-rwkv-0.0.6/ml_rwkv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/pyproject.toml` & `ml-rwkv-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/model.py` & `ml-rwkv-0.0.6/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/run.py` & `ml-rwkv-0.0.6/rwkv/run.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/triton/utils.py` & `ml-rwkv-0.0.6/rwkv/triton/utils.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/triton/wkv/eps.py` & `ml-rwkv-0.0.6/rwkv/triton/wkv/eps.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
         w: Tensor,
         u: Tensor,
         k: Tensor,
         v: Tensor,
         state: Tensor,
     ) -> tuple[Tensor, Tensor]:
         wkv, state_out = wkv_triton_with_eps_forward(w, u, k, v, state)
-        ctx.save_for_backward(w, u, k, v, state_out[:, :, :-1])
+        ctx.save_for_backward(w, u, k, v, state_out)
         return wkv, state_out[:, :, -1:]
 
     @staticmethod
     @once_differentiable
     def backward(ctx: FunctionCtx, gwkv: Tensor, gstate: Tensor) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
         w, u, k, v, state = cast(tuple[Tensor, ...], ctx.saved_tensors)
         gw, gu, gk, gv, gstate = wkv_triton_with_eps_backward(w, u, k, v, state, gwkv, gstate)
```

### Comparing `ml-rwkv-0.0.5/rwkv/triton/wkv/log.py` & `ml-rwkv-0.0.6/rwkv/triton/wkv/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,20 +508,20 @@
 
     @staticmethod
     @once_differentiable
     def backward(
         ctx: FunctionCtx,
         gwkv: Tensor,
         gstate: Tensor,
-    ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor, None]:
+    ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor, None, None]:
         if ctx.normalize:
             raise NotImplementedError("Backward pass for normalized operation is incorrect")
         w, u, k, v, state = cast(tuple[Tensor, ...], ctx.saved_tensors)
         gw, gu, gk, gv, gstate = wkv_triton_log_space_backward(w, u, k, v, state, gwkv, gstate, ctx.eps)
-        return gw, gu, gk, gv, gstate, None
+        return gw, gu, gk, gv, gstate, None, None
 
 
 def wkv_triton_log_space(
     w: Tensor,
     u: Tensor,
     k: Tensor,
     v: Tensor,
```

### Comparing `ml-rwkv-0.0.5/rwkv/triton/wkv/vanilla.py` & `ml-rwkv-0.0.6/rwkv/triton/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/wkv/__init__.py` & `ml-rwkv-0.0.6/rwkv/wkv/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/wkv/eps.py` & `ml-rwkv-0.0.6/rwkv/wkv/eps.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/wkv/log.py` & `ml-rwkv-0.0.6/rwkv/wkv/log.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/rwkv/wkv/vanilla.py` & `ml-rwkv-0.0.6/rwkv/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/setup.py` & `ml-rwkv-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/tests/test_eps_wkv.py` & `ml-rwkv-0.0.6/tests/test_eps_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/tests/test_log_wkv.py` & `ml-rwkv-0.0.6/tests/test_log_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/tests/test_vanilla_wkv.py` & `ml-rwkv-0.0.6/tests/test_vanilla_wkv.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.5/tests/test_wkv.py` & `ml-rwkv-0.0.6/tests/test_wkv.py`

 * *Files identical despite different names*

