# Comparing `tmp/jaxdf-0.2.4.tar.gz` & `tmp/jaxdf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "jaxdf-0.2.5.tar", max compression
```

## Comparing `jaxdf-0.2.4.tar` & `jaxdf-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/__about__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/__init__.py
--rwxr-xr-x   0        0        0     5318 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/conv.py
--rw-r--r--   0        0        0    11860 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/core.py
--rw-r--r--   0        0        0    13161 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/discretization.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/exceptions.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/geometry.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/util.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/__init__.py
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/differential.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/dummy.py
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/functions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/linear_algebra.py
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 jaxdf-0.2.4/jaxdf/operators/magic.py
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 jaxdf-0.2.4/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 jaxdf-0.2.4/LICENSE
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 jaxdf-0.2.4/README.md
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 jaxdf-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    16289 2020-02-02 00:00:00.000000 jaxdf-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-23 12:29:53.472909 jaxdf-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5669 2023-06-23 12:29:53.472909 jaxdf-0.2.5/README.md
+-rwxr-xr-x   0        0        0       19 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/__about__.py
+-rw-r--r--   0        0        0      316 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/__init__.py
+-rwxr-xr-x   0        0        0     5318 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/conv.py
+-rw-r--r--   0        0        0    11860 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/core.py
+-rw-r--r--   0        0        0    13240 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/discretization.py
+-rw-r--r--   0        0        0      953 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/exceptions.py
+-rw-r--r--   0        0        0     5283 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/geometry.py
+-rw-r--r--   0        0        0      155 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/__init__.py
+-rw-r--r--   0        0        0    12765 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/differential.py
+-rw-r--r--   0        0        0     1060 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/dummy.py
+-rw-r--r--   0        0        0     6275 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/functions.py
+-rw-r--r--   0        0        0      327 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/linear_algebra.py
+-rw-r--r--   0        0        0     7493 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/operators/magic.py
+-rw-r--r--   0        0        0     1329 2023-06-23 12:29:53.496909 jaxdf-0.2.5/jaxdf/util.py
+-rw-r--r--   0        0        0     3021 2023-06-23 12:29:53.496909 jaxdf-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7513 1970-01-01 00:00:00.000000 jaxdf-0.2.5/PKG-INFO
```

### Comparing `jaxdf-0.2.4/jaxdf/conv.py` & `jaxdf-0.2.5/jaxdf/conv.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/core.py` & `jaxdf-0.2.5/jaxdf/core.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/discretization.py` & `jaxdf-0.2.5/jaxdf/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,33 @@
           get_fun (Callable): A function that takes a parameter vector and a point in
           the domain and returns the field at that point. The signature of this
           function is `get_field(params, x)`.
 
         Returns:
           Continuous: A continuous discretization.
         """
-        aux = {"get_field": get_fun}
-        x = domain.origin
-        dims = eval_shape(get_fun, params, x).shape
-        super().__init__(params, domain, dims, aux)
+        self.params = params
+        self.domain = domain
+        self.aux = {"get_field": get_fun}
+
+    @property
+    def dims(self):
+        get_fun = self.aux["get_field"]
+        x = self.domain.origin
+        return eval_shape(get_fun, self.params, x).shape
 
     def tree_flatten(self):
         children = (self.params,)
-        aux_data = (self.dims, self.domain, self.aux["get_field"])
+        aux_data = (self.domain, self.aux["get_field"])
         return (children, aux_data)
 
     @classmethod
     def tree_unflatten(cls, aux_data, children):
         params = children[0]
-        dims, domain, get_fun = aux_data
+        domain, get_fun = aux_data
         a = cls(params, domain=domain, get_fun=get_fun)
         return a
 
     def replace_params(self, new_params):
         r"""Replaces the parameters of the discretization with new ones. The domain
         and `get_field` function are not changed.
```

### Comparing `jaxdf-0.2.4/jaxdf/exceptions.py` & `jaxdf-0.2.5/jaxdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/geometry.py` & `jaxdf-0.2.5/jaxdf/geometry.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/util.py` & `jaxdf-0.2.5/jaxdf/util.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/operators/differential.py` & `jaxdf-0.2.5/jaxdf/operators/differential.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     Returns:
       The gradient of the field
     """
     get_x = x.aux["get_field"]
 
     def grad_fun(p, coords):
         f_jac = jax.jacfwd(get_x, argnums=(1,))
-        v = f_jac(p, coords)[0]
+        v = f_jac(p, coords)[0][0]
         return v
 
     return x.update_fun_and_params(x.params, grad_fun)
 
 
 @operator(init_params=fd_diag_jacobian_init)  # type: ignore
 def gradient(x: FiniteDifferences, *, stagger=[0], params=None) -> FiniteDifferences:
```

### Comparing `jaxdf-0.2.4/jaxdf/operators/dummy.py` & `jaxdf-0.2.5/jaxdf/operators/dummy.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/operators/functions.py` & `jaxdf-0.2.5/jaxdf/operators/functions.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/jaxdf/operators/magic.py` & `jaxdf-0.2.5/jaxdf/operators/magic.py`

 * *Files identical despite different names*

### Comparing `jaxdf-0.2.4/LICENSE` & `jaxdf-0.2.5/LICENSE`

 * *Files identical despite different names*

