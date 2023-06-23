# Comparing `tmp/klongpy-0.3.69.tar.gz` & `tmp/klongpy-0.3.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.69.tar", last modified: Wed Apr  5 21:27:08 2023, max compression
+gzip compressed data, was "klongpy-0.3.71.tar", last modified: Fri Jun 23 00:44:26 2023, max compression
```

## Comparing `klongpy-0.3.69.tar` & `klongpy-0.3.71.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-04-05 21:27:08.325494 klongpy-0.3.69/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.69/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    11058 2023-04-05 21:27:08.325494 klongpy-0.3.69/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    10523 2023-03-13 00:39:32.000000 klongpy-0.3.69/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-04-05 21:27:08.325494 klongpy-0.3.69/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.69/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13224 2023-04-05 16:20:02.000000 klongpy-0.3.69/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2300 2023-04-05 16:20:02.000000 klongpy-0.3.69/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    23011 2023-04-05 16:24:45.000000 klongpy-0.3.69/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    31270 2023-04-05 16:20:02.000000 klongpy-0.3.69/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20402 2023-04-03 23:16:48.000000 klongpy-0.3.69/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-05 16:20:02.000000 klongpy-0.3.69/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.69/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.69/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.69/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-04-05 21:27:08.325494 klongpy-0.3.69/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11058 2023-04-05 21:27:08.000000 klongpy-0.3.69/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      591 2023-04-05 21:27:08.000000 klongpy-0.3.69/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-04-05 21:27:08.000000 klongpy-0.3.69/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-04-05 21:27:08.000000 klongpy-0.3.69/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-04-05 21:27:08.000000 klongpy-0.3.69/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-04-05 21:27:08.325494 klongpy-0.3.69/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.69/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-04-05 21:27:08.325494 klongpy-0.3.69/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-04-05 21:26:39.000000 klongpy-0.3.69/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-04-05 21:27:08.325494 klongpy-0.3.69/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     5703 2023-04-05 16:20:02.000000 klongpy-0.3.69/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.69/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20982 2023-03-12 00:53:23.000000 klongpy-0.3.69/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1952 2023-03-12 01:19:51.000000 klongpy-0.3.69/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.69/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.69/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.69/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.69/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.69/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.69/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.71/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 00:44:26.793443 klongpy-0.3.71/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.71/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.71/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    13005 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.71/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    23120 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30983 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20402 2023-04-03 23:16:48.000000 klongpy-0.3.71/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.71/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.71/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.71/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.71/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.71/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 00:44:26.793443 klongpy-0.3.71/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 00:44:02.000000 klongpy-0.3.71/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.71/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    21480 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1952 2023-03-12 01:19:51.000000 klongpy-0.3.71/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.71/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3808 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.71/tests/test_util.py
```

### Comparing `klongpy-0.3.69/LICENSE` & `klongpy-0.3.71/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/PKG-INFO` & `klongpy-0.3.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.69
+Version: 0.3.71
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -32,14 +32,15 @@
 
 
 Klong was created by Nils M Holm and he has also written a [Klong Book](https://t3x.org/klong/book.html).
 
 
 # Related
 
+ * [Klupyter - KlongPy in Jupyter Notebooks](https://github.com/briangu/klupyter)
  * [Advent Of Code '22](https://github.com/briangu/aoc/tree/main/22)
  * [Example Ticker Plant with streaming and dataframes](https://github.com/briangu/kdfs)
 
 
 # Overview
 
 KlongPy brings together the Klong terse array language notation with the performance of NumPy.  I wanted to use Klong but I also wanted it to be a fast as possible.  Bonus is the ability to mix Klong with Python libraries making it easy to pick and choose the tools as appropriate.
```

### Comparing `klongpy-0.3.69/README.md` & `klongpy-0.3.71/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 Klong was created by Nils M Holm and he has also written a [Klong Book](https://t3x.org/klong/book.html).
 
 
 # Related
 
+ * [Klupyter - KlongPy in Jupyter Notebooks](https://github.com/briangu/klupyter)
  * [Advent Of Code '22](https://github.com/briangu/aoc/tree/main/22)
  * [Example Ticker Plant with streaming and dataframes](https://github.com/briangu/kdfs)
 
 
 # Overview
 
 KlongPy brings together the Klong terse array language notation with the performance of NumPy.  I wanted to use Klong but I also wanted it to be a fast as possible.  Bonus is the ability to mix Klong with Python libraries making it easy to pick and choose the tools as appropriate.
```

### Comparing `klongpy-0.3.69/klongpy/adverbs.py` & `klongpy-0.3.71/klongpy/adverbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,24 +234,16 @@
             return np.multiply.reduce(a)
         elif safe_eq(wrapped.a, '%') and hasattr(np.divide,'reduce'):
             return np.divide.reduce(a)
         elif safe_eq(wrapped.a, '&') and len(a.shape) == 1:
             return np.min(a)
         elif safe_eq(wrapped.a, '|') and len(a.shape) == 1:
             return np.max(a)
-        elif safe_eq(wrapped.a, ','):
-            if isinstance(a,str):
-                return a
-            r = np.hstack(a)
-            if a.dtype == np.dtype('O') and len(r) > 0 and is_float(r[0]):
-                try:
-                    r = r.astype(type(r[0]))
-                except ValueError:
-                    pass
-            return r
+        elif safe_eq(wrapped.a, ',') and np.isarray(a) and a.dtype != 'O':
+            return a if a.ndim == 1 else np.concatenate(a, axis=0)
     return functools.reduce(f, a)
 
 
 def eval_adverb_over_neutral(f, a, b):
     """
 
         a f/b                                             [Over-Neutral]
@@ -358,18 +350,17 @@
         the square root of 2.
 
         Example: ,/\~["a" ["b"] "c"]  -->  [["a" ["b"] "c"]
                                             ["a" "b" "c"]
                                             "abc"]
 
     """
-    r = [a]
     x = a
     xx = f(a)
-    r.append(xx)
+    r = [a, xx]
     while not array_equal(x,xx):
         x = xx
         xx = f(x)
         r.append(xx)
     r.pop()
     try:
         return np.asarray(r)
```

### Comparing `klongpy-0.3.69/klongpy/backend.py` & `klongpy-0.3.71/klongpy/backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,103 @@
 import os
 import warnings
 
+# Attempt to import CuPy. If not available, set use_gpu to False.
 use_gpu = bool(os.environ.get('USE_GPU') == '1')
+if use_gpu:
+    try:
+        import cupy as np
+        use_gpu = True
+    except ImportError:
+        import numpy as np
+        use_gpu = False
+else:
+    import numpy as np
+
+
+def is_supported_type(x):
+    """
+    CuPy does not support strings or jagged arrays.
+    Note: add any other unsupported types here.
+    """
+    if isinstance(x, str) or is_jagged_array(x):
+        return False
+    return True
+
+
+def is_jagged_array(x):
+    """
+    Check if an array is jagged.
+    """
+    if isinstance(x, list):
+        # If the lengths of sublists vary, it's a jagged array.
+        return len(set(map(len, x))) > 1
+    return False
 
 if use_gpu:
-    import cupy as cp
-    import cupy as np
+    import cupy
     import numpy
 
     class CuPyReductionKernelWrapper:
         def __init__(self, fn, reduce_fn_1, reduce_fn_2):
             self.fn = fn
             self.reduce_fn_1 = reduce_fn_1
             self.reduce_fn_2 = reduce_fn_2
 
         def __call__(self, *args, **kwargs):
             return self.fn(*args, **kwargs)
 
         def reduce(self, x):
             return self.reduce_fn_1(x) if len(x.shape) == 1 else self.reduce_fn_2(x[0], x[1])
 
-    add_reduce_2 = cp.ElementwiseKernel(
+    add_reduce_2 = cupy.ElementwiseKernel(
             'T x, T y',
             'T z',
             'z = (x + y)',
             'add_reduce_2')
-    cp.add = CuPyReductionKernelWrapper(cp.add, cp.sum, add_reduce_2)
+    np.add = CuPyReductionKernelWrapper(cupy.add, cupy.sum, add_reduce_2)
 
     def subtract_reduce_1(x):
-        return 2*x[0] - cp.sum(x)
+        return 2*x[0] - cupy.sum(x)
 
-    subtract_reduce_2 = cp.ElementwiseKernel(
+    subtract_reduce_2 = cupy.ElementwiseKernel(
             'T x, T y',
             'T z',
             'z = (x - y)',
             'subtract_reduce_2')
-    np.subtract = CuPyReductionKernelWrapper(cp.subtract, subtract_reduce_1, subtract_reduce_2)
+    np.subtract = CuPyReductionKernelWrapper(cupy.subtract, subtract_reduce_1, subtract_reduce_2)
 
-    multiply_reduce_1 = cp.ReductionKernel(
+    multiply_reduce_1 = cupy.ReductionKernel(
                 'T x',
                 'T y',
                 'x',
                 'a * b',
                 'y = a',
                 '1',
                 'multiply_reduce_1'
              )
-    multiply_reduce_2 = cp.ElementwiseKernel(
+    multiply_reduce_2 = cupy.ElementwiseKernel(
             'T x, T y',
             'T z',
             'z = (x * y)',
             'multiply_reduce_2')
-    np.multiply = CuPyReductionKernelWrapper(cp.multiply, multiply_reduce_1, multiply_reduce_2)
+    np.multiply = CuPyReductionKernelWrapper(cupy.multiply, multiply_reduce_1, multiply_reduce_2)
 
-    divide_reduce_1 = cp.ReductionKernel(
-                'T x',
-                'T y',
-                'x',
-                'a / b',
-                'y = a',
-                '1',
-                'divide_reduce_1'
-             )
-    divide_reduce_2 = cp.ElementwiseKernel(
+    def divide_reduce_1(x):
+        raise NotImplementedError()
+
+    divide_reduce_2 = cupy.ElementwiseKernel(
             'T x, T y',
             'T z',
             'z = (x / y)',
             'divide_reduce_2')
-    np.divide = CuPyReductionKernelWrapper(cp.divide, divide_reduce_1, divide_reduce_2)
+    np.divide = CuPyReductionKernelWrapper(cupy.divide, divide_reduce_1, divide_reduce_2)
+
+    np.isarray = lambda x: isinstance(x, (numpy.ndarray, cupy.ndarray))
 
-    np.isarray = lambda x: isinstance(x, (numpy.ndarray, cp.ndarray))
+#    np.hstack = lambda x: cupy.hstack(x) if use_gpu and is_supported_type(x) else numpy.hstack(x)
 else:
-    import numpy as np
     np.seterr(divide='ignore')
     warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
     np.isarray = lambda x: isinstance(x, np.ndarray)
 
 np
```

### Comparing `klongpy-0.3.69/klongpy/core.py` & `klongpy-0.3.71/klongpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import inspect
 import weakref
 from enum import Enum
 import sys
 
 from .backend import np
 
+# python3.11 support
+if not hasattr(inspect, 'getargspec'):
+    inspect.getargspec = inspect.getfullargspec
+
 
 class KGSym(str):
     def __repr__(self):
         return f":{super().__str__()}"
     def __eq__(self, o):
         return isinstance(o,KGSym) and self.__str__() == o.__str__()
     def __hash__(self):
```

### Comparing `klongpy-0.3.69/klongpy/dyads.py` & `klongpy-0.3.71/klongpy/dyads.py`

 * *Files 3% similar despite different names*

```diff
@@ -445,14 +445,25 @@
     """
     def _e(x,y):
         a = np.trunc(np.divide(x, y))
         return np.asarray(a,dtype=int) if np.isarray(a) else int(a)
     return vec_fn2(a, b, _e)
 
 
+def dyad_join_to_list(a):
+    if np.isarray(a):
+        if a.ndim == 1:
+            return a
+        elif a.shape[0] == 1:
+            return [a.flatten()]
+        elif a.shape[0] > 1:
+            return a
+    return [a]
+
+
 def eval_dyad_join(a, b):
     """
 
         a,b                                                       [Join]
 
         The "," operator joins objects of any type, forming lists or
         strings.
@@ -496,28 +507,23 @@
     if isinstance(a,dict):
         a[b[0]] = b[1]
         return a
     if isinstance(b,dict) and is_list(a) and len(a) == 2:
         b[a[0]] = a[1]
         return b
 
-    # TODO: this code in general needs a lot more optimization
     if np.isarray(a) and np.isarray(b):
         if len(a) == 0:
             return b
-        elif len(a) == 1 and len(b) == 1:
-            return np.asarray([a[0], b[0]])
         if len(a.shape) == len(b.shape) and a.shape[-1] == b.shape[-1]:
             return np.concatenate((a,b))
-    # elif is_number(a) and isinstance(b,np.ndarray):
-        # return np.asarray([a,b], dtype=object)
-
-    aa = a if isinstance(a, list) else ([a[0]] if len(a.shape) > 1 and a.shape[0] == 1 else a.tolist() if len(a.shape) == 1 else [a]) if np.isarray(a) else [a]
-    bb = b if isinstance(b, list) else ([b[0]] if len(b.shape) > 1 and b.shape[0] == 1 else b.tolist() if len(b.shape) == 1 else [b]) if np.isarray(b) else [b]
 
+    aa = dyad_join_to_list(a)
+    bb = dyad_join_to_list(b)
+ 
     r = [*aa,*bb]
     nr = np.asarray(r)
     t = nr.dtype.type
     return nr if issubclass(t, np.integer) or issubclass(t, np.floating) else np.asarray(r,dtype=object)
 
 
 def eval_dyad_less(a, b):
@@ -583,14 +589,15 @@
     if is_list(a):
         if is_list(b):
             return kg_truth(rec_flatten(vec_fn2(a, b, _e)).all() if len(a) == len(b) else 0)
     elif not is_list(b):
         return kg_truth(_e(a,b))
     return False
 
+
 def eval_dyad_maximum(a, b):
     """
 
         a|b                                                     [Max/Or]
 
         Return the larger one of two numbers.
```

### Comparing `klongpy-0.3.69/klongpy/interpreter.py` & `klongpy-0.3.71/klongpy/interpreter.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/klongpy/monads.py` & `klongpy-0.3.71/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/klongpy/sys_fn.py` & `klongpy-0.3.71/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/klongpy/sys_var.py` & `klongpy-0.3.71/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/klongpy/utils.py` & `klongpy-0.3.71/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.71/klongpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.69
+Version: 0.3.71
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -32,14 +32,15 @@
 
 
 Klong was created by Nils M Holm and he has also written a [Klong Book](https://t3x.org/klong/book.html).
 
 
 # Related
 
+ * [Klupyter - KlongPy in Jupyter Notebooks](https://github.com/briangu/klupyter)
  * [Advent Of Code '22](https://github.com/briangu/aoc/tree/main/22)
  * [Example Ticker Plant with streaming and dataframes](https://github.com/briangu/kdfs)
 
 
 # Overview
 
 KlongPy brings together the Klong terse array language notation with the performance of NumPy.  I wanted to use Klong but I also wanted it to be a fast as possible.  Bonus is the ability to mix Klong with Python libraries making it easy to pick and choose the tools as appropriate.
```

### Comparing `klongpy-0.3.69/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.71/klongpy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 klongpy.egg-info/top_level.txt
 scripts/kgpy
 tests/test_accel.py
 tests/test_examples.py
 tests/test_extra_suite.py
 tests/test_fn.py
 tests/test_interop.py
+tests/test_join_over.py
 tests/test_prog.py
 tests/test_suite.py
 tests/test_suite_file.py
 tests/test_sys_fn.py
 tests/test_util.py
```

### Comparing `klongpy-0.3.69/scripts/kgpy` & `klongpy-0.3.71/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/setup.py` & `klongpy-0.3.71/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.69',
+    version='0.3.71',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.3.69/tests/test_accel.py` & `klongpy-0.3.71/tests/test_accel.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     return np.random.rand(100)
 
 
 def get_reduce_data(data):
     return data if isinstance(data, numpy.ndarray) else data.get()
 
 
+# This approach isn't great because any usage of the thunked method will pass
+# We need a way to intercept the real call
 class TestAccelerate(unittest.TestCase):
     """
     Verify that we are actually running the adverb_over accelerated paths for cases that we can.
     """
 
     # TODO: this is not parallel test safe
     #       add ability to intercept calls in interpeter
@@ -124,15 +126,30 @@
         finally:
             np.multiply = e.fn
         self.assertTrue(numpy.isclose(r, numpy.multiply.reduce(get_reduce_data(data))))
         self.assertTrue(e.executed)
 
     ####### Divide
 
+    def test_over_divide_nested_array(self):
+        klong = KlongInterpreter()
+        e = ExecutedReduce(np.divide)
+        data = get_rnd_nested_array()
+        try:
+            np.divide = e
+            klong['data'] = data
+            r = klong('%/data')
+        finally:
+            np.divide = e.fn
+        self.assertTrue(array_equal(r, numpy.divide.reduce(get_reduce_data(data))))
+        self.assertTrue(e.executed)
+
     def test_over_divide(self):
+        if np != numpy:
+            return
         if not hasattr(np.divide, "reduce"):
             return
         klong = KlongInterpreter()
         e = ExecutedReduce(np.divide)
         data = get_rnd_array()
         try:
             np.divide = e
@@ -189,21 +206,22 @@
         finally:
             np.max = e.fn
         self.assertEqual(r, 4)
         self.assertTrue(e.executed)
 
     ####### Join
 
+    @unittest.skip
     def test_over_join(self):
         if np != numpy:
             return
         klong = KlongInterpreter()
-        e = Executed(np.hstack)
+        e = Executed(np.concatenate)
         try:
-            np.hstack = e
-            r = klong(',/:~[[1] [[2]] [3]]')
+            np.concatenate = e
+            r = klong(',/:~[[1] [2] [3]]')
         finally:
-            np.hstack = e.fn
+            np.concatenate = e.fn
         self.assertTrue(array_equal(r, [1,2,3]))
         self.assertTrue(e.executed)
```

### Comparing `klongpy-0.3.69/tests/test_examples.py` & `klongpy-0.3.71/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_extra_suite.py` & `klongpy-0.3.71/tests/test_extra_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 import unittest
 from klongpy import KlongInterpreter
-from klongpy.core import rec_flatten, rec_fn2, KGChar, KGSym, is_integer, is_float
+from klongpy.core import rec_flatten, rec_fn2, KGChar, KGSym, is_integer, is_float, is_list
 from utils import *
 import time
+import random
+import string
+
 
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
+    def test_dyad_join_mixed_types(self):
+        klong = KlongInterpreter()
+        r = klong(',/["a" [1]]')
+        self.assertTrue(array_equal(r, np.array(['a', 1], dtype='object')))
+
+    def test_dyad_join_nested_array(self):
+        klong = KlongInterpreter()
+        r = klong('[1],[[2 3]]')
+        self.assertTrue(array_equal(r, np.array([1,[2,3]])))
+        r = klong(',/[0 [[1] [2]]]')
+        self.assertTrue(array_equal(r, np.array([0,[1],[2]])))
+
     @unittest.skip
     def test_dict_inner_create_syntax(self):
         klong = KlongInterpreter()
         with self.assertRaises(RuntimeError):
             # should fail to parse
             r = klong(":{[1 :{[2 3]}}")
```

### Comparing `klongpy-0.3.69/tests/test_fn.py` & `klongpy-0.3.71/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_interop.py` & `klongpy-0.3.71/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_prog.py` & `klongpy-0.3.71/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_suite.py` & `klongpy-0.3.71/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_suite_file.py` & `klongpy-0.3.71/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_sys_fn.py` & `klongpy-0.3.71/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.69/tests/test_util.py` & `klongpy-0.3.71/tests/test_util.py`

 * *Files identical despite different names*

