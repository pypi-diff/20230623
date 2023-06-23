# Comparing `tmp/seqpro-0.1.0.tar.gz` & `tmp/seqpro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqpro-0.1.0.tar", max compression
+gzip compressed data, was "seqpro-0.1.1.tar", max compression
```

## Comparing `seqpro-0.1.0.tar` & `seqpro-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      520 2023-06-23 17:13:31.000000 seqpro-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      977 2023-06-23 16:04:56.000000 seqpro-0.1.0/seqpro/__init__.py
--rw-r--r--   0        0        0     5455 2023-06-11 21:58:41.000000 seqpro-0.1.0/seqpro/_analyzers.py
--rw-r--r--   0        0        0     1276 2023-06-01 00:42:03.000000 seqpro-0.1.0/seqpro/_cleaners.py
--rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.0/seqpro/_comparisons.py
--rw-r--r--   0        0        0     5098 2023-06-23 16:45:31.000000 seqpro-0.1.0/seqpro/_encoders.py
--rw-r--r--   0        0        0     6782 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/_modifiers.py
--rw-r--r--   0        0        0     3535 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/_numba.py
--rw-r--r--   0        0        0     3810 2023-06-23 16:04:56.000000 seqpro-0.1.0/seqpro/_utils.py
--rw-r--r--   0        0        0     1458 2023-06-11 21:58:41.000000 seqpro-0.1.0/seqpro/alphabets/__init__.py
--rw-r--r--   0        0        0     8278 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/alphabets/_alphabets.py
--rw-r--r--   0        0        0     2504 2023-06-23 17:05:29.000000 seqpro-0.1.0/seqpro/deprecated/_analyzers.py
--rw-r--r--   0        0        0     1358 2023-06-23 17:05:27.000000 seqpro-0.1.0/seqpro/deprecated/_cleaners.py
--rw-r--r--   0        0        0     4364 2023-06-23 17:05:11.000000 seqpro-0.1.0/seqpro/deprecated/_encoders.py
--rw-r--r--   0        0        0     9481 2023-06-23 16:48:35.000000 seqpro-0.1.0/seqpro/deprecated/_helpers.py
--rw-r--r--   0        0        0     6113 2023-06-23 17:05:21.000000 seqpro-0.1.0/seqpro/deprecated/_modifiers.py
--rw-r--r--   0        0        0     1419 2023-06-23 17:05:25.000000 seqpro-0.1.0/seqpro/deprecated/_utils.py
--rw-r--r--   0        0        0     2162 2023-06-23 17:05:59.000000 seqpro-0.1.0/seqpro/experimental/_experimental.py
--rw-r--r--   0        0        0      773 2023-06-23 17:05:39.000000 seqpro-0.1.0/seqpro/experimental/_visualizers.py
--rw-r--r--   0        0        0     6198 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/xr/__init__.py
--rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 seqpro-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      543 2023-06-23 19:52:39.000000 seqpro-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      977 2023-06-23 19:48:20.000000 seqpro-0.1.1/seqpro/__init__.py
+-rw-r--r--   0        0        0     5455 2023-06-11 21:58:41.000000 seqpro-0.1.1/seqpro/_analyzers.py
+-rw-r--r--   0        0        0     1276 2023-06-01 00:42:03.000000 seqpro-0.1.1/seqpro/_cleaners.py
+-rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.1/seqpro/_comparisons.py
+-rw-r--r--   0        0        0     5098 2023-06-23 16:45:31.000000 seqpro-0.1.1/seqpro/_encoders.py
+-rw-r--r--   0        0        0     6926 2023-06-23 19:49:15.000000 seqpro-0.1.1/seqpro/_modifiers.py
+-rw-r--r--   0        0        0     3535 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/_numba.py
+-rw-r--r--   0        0        0     3810 2023-06-23 16:04:56.000000 seqpro-0.1.1/seqpro/_utils.py
+-rw-r--r--   0        0        0     1458 2023-06-11 21:58:41.000000 seqpro-0.1.1/seqpro/alphabets/__init__.py
+-rw-r--r--   0        0        0     8278 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/alphabets/_alphabets.py
+-rw-r--r--   0        0        0     2504 2023-06-23 17:05:29.000000 seqpro-0.1.1/seqpro/deprecated/_analyzers.py
+-rw-r--r--   0        0        0     1358 2023-06-23 17:05:27.000000 seqpro-0.1.1/seqpro/deprecated/_cleaners.py
+-rw-r--r--   0        0        0     4364 2023-06-23 17:05:11.000000 seqpro-0.1.1/seqpro/deprecated/_encoders.py
+-rw-r--r--   0        0        0     9481 2023-06-23 16:48:35.000000 seqpro-0.1.1/seqpro/deprecated/_helpers.py
+-rw-r--r--   0        0        0     6113 2023-06-23 17:05:21.000000 seqpro-0.1.1/seqpro/deprecated/_modifiers.py
+-rw-r--r--   0        0        0     1419 2023-06-23 17:05:25.000000 seqpro-0.1.1/seqpro/deprecated/_utils.py
+-rw-r--r--   0        0        0     2162 2023-06-23 17:05:59.000000 seqpro-0.1.1/seqpro/experimental/_experimental.py
+-rw-r--r--   0        0        0      773 2023-06-23 17:05:39.000000 seqpro-0.1.1/seqpro/experimental/_visualizers.py
+-rw-r--r--   0        0        0     6198 2023-06-21 17:46:41.000000 seqpro-0.1.1/seqpro/xr/__init__.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 seqpro-0.1.1/PKG-INFO
```

### Comparing `seqpro-0.1.0/seqpro/__init__.py` & `seqpro-0.1.1/seqpro/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/_analyzers.py` & `seqpro-0.1.1/seqpro/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/_cleaners.py` & `seqpro-0.1.1/seqpro/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/_encoders.py` & `seqpro-0.1.1/seqpro/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/_modifiers.py` & `seqpro-0.1.1/seqpro/_modifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Tuple, Union, cast
 
 import numpy as np
-import ushuffle
+
 from numpy.typing import NDArray
 
 from ._numba import gufunc_jitter_helper
 from ._utils import SeqType, _check_axes, cast_seqs
 from .alphabets._alphabets import NucleotideAlphabet
 
 
@@ -56,15 +56,19 @@
         Needed for OHE input. Axis that corresponds to the one hot encoding, should be
         the same size as the length of the alphabet.
     seed : Optional[int], optional
         Seed for shuffling.
     alphabet : Optional[NucleotideAlphabet], optional
         Alphabet, needed for OHE sequence input.
     """
-
+    try:
+        import ushuffle
+    except ImportError:
+        raise ImportError("Please install ushuffle to use this function (pip install ushuffle))")
+    
     _check_axes(seqs, length_axis, ohe_axis)
 
     seqs = cast_seqs(seqs)
 
     # only get here if seqs was str or list[str]
     if length_axis is None:
         length_axis = -1
```

### Comparing `seqpro-0.1.0/seqpro/_numba.py` & `seqpro-0.1.1/seqpro/_numba.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/_utils.py` & `seqpro-0.1.1/seqpro/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/alphabets/__init__.py` & `seqpro-0.1.1/seqpro/alphabets/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/alphabets/_alphabets.py` & `seqpro-0.1.1/seqpro/alphabets/_alphabets.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_analyzers.py` & `seqpro-0.1.1/seqpro/deprecated/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_cleaners.py` & `seqpro-0.1.1/seqpro/deprecated/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_encoders.py` & `seqpro-0.1.1/seqpro/deprecated/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_helpers.py` & `seqpro-0.1.1/seqpro/deprecated/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_modifiers.py` & `seqpro-0.1.1/seqpro/deprecated/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/deprecated/_utils.py` & `seqpro-0.1.1/seqpro/deprecated/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/experimental/_experimental.py` & `seqpro-0.1.1/seqpro/experimental/_experimental.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/experimental/_visualizers.py` & `seqpro-0.1.1/seqpro/experimental/_visualizers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/seqpro/xr/__init__.py` & `seqpro-0.1.1/seqpro/xr/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.0/PKG-INFO` & `seqpro-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: seqpro
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sequence processing toolkit
 Author: Adam Klie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
 Requires-Dist: cython (>=0.29.35,<0.30.0)
-Requires-Dist: matplotlib[dev] (>=3.6.2,<4.0.0)
+Requires-Dist: matplotlib[dev] (>=3.6.2,<4.0.0) ; extra == "dev"
 Requires-Dist: numba (>=0.57.0,<0.58.0)
-Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: ushuffle (>=1.1.2,<2.0.0)
+Requires-Dist: numpy (>=1.23.5,<1.24.0)
```

