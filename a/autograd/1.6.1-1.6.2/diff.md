# Comparing `tmp/autograd-1.6.1.tar.gz` & `tmp/autograd-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autograd-1.6.1.tar", last modified: Thu Jun 22 20:49:56 2023, max compression
+gzip compressed data, was "autograd-1.6.2.tar", last modified: Fri Jun 23 08:35:52 2023, max compression
```

## Comparing `autograd-1.6.1.tar` & `autograd-1.6.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.694909 autograd-1.6.1/
--rw-r--r--   0 jamietownsend   (501) staff       (20)       41 2020-03-21 18:01:53.000000 autograd-1.6.1/MANIFEST.in
--rw-r--r--   0 jamietownsend   (501) staff       (20)      642 2023-06-22 20:49:56.695189 autograd-1.6.1/PKG-INFO
--rw-r--r--   0 jamietownsend   (501) staff       (20)     4443 2020-03-21 18:01:53.000000 autograd-1.6.1/README.md
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.623638 autograd-1.6.1/autograd/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      504 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     6328 2023-06-22 12:39:21.000000 autograd-1.6.1/autograd/builtins.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    12235 2023-06-22 12:38:25.000000 autograd-1.6.1/autograd/core.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     8515 2022-06-15 10:01:07.000000 autograd-1.6.1/autograd/differential_operators.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      304 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/extend.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.630828 autograd-1.6.1/autograd/misc/
--rw-r--r--   0 jamietownsend   (501) staff       (20)       62 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/misc/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      771 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/misc/fixed_points.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1120 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/misc/flatten.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2757 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/misc/optimizers.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2200 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/misc/tracers.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.640457 autograd-1.6.1/autograd/numpy/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      232 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/numpy/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5250 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/numpy/fft.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    11352 2022-09-29 07:03:46.000000 autograd-1.6.1/autograd/numpy/linalg.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3465 2023-06-22 20:47:35.000000 autograd-1.6.1/autograd/numpy/numpy_boxes.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    10766 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/numpy/numpy_jvps.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    32566 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/numpy/numpy_vjps.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2815 2023-06-22 20:47:35.000000 autograd-1.6.1/autograd/numpy/numpy_vspaces.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5459 2021-03-03 09:26:31.000000 autograd-1.6.1/autograd/numpy/numpy_wrapper.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      149 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/numpy/random.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.651317 autograd-1.6.1/autograd/scipy/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      183 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2867 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/integrate.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2363 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/linalg.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      168 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/misc.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5924 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/signal.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5135 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/special.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.666031 autograd-1.6.1/autograd/scipy/stats/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      391 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1332 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/beta.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      809 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/chi2.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      772 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/dirichlet.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      987 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/gamma.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2509 2023-03-22 11:58:08.000000 autograd-1.6.1/autograd/scipy/stats/multivariate_normal.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2758 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/norm.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      715 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/poisson.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2670 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/scipy/stats/t.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2881 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/test_util.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3951 2023-06-22 12:38:25.000000 autograd-1.6.1/autograd/tracer.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1482 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/util.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1581 2020-03-21 18:01:53.000000 autograd-1.6.1/autograd/wrap_util.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.626585 autograd-1.6.1/autograd.egg-info/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      642 2023-06-22 20:49:56.000000 autograd-1.6.1/autograd.egg-info/PKG-INFO
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1710 2023-06-22 20:49:56.000000 autograd-1.6.1/autograd.egg-info/SOURCES.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)        1 2023-06-22 20:49:56.000000 autograd-1.6.1/autograd.egg-info/dependency_links.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)       27 2023-06-22 20:49:56.000000 autograd-1.6.1/autograd.egg-info/requires.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)        9 2023-06-22 20:49:56.000000 autograd-1.6.1/autograd.egg-info/top_level.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)       79 2023-06-22 20:49:56.696106 autograd-1.6.1/setup.cfg
--rw-r--r--   0 jamietownsend   (501) staff       (20)      952 2023-06-22 20:48:58.000000 autograd-1.6.1/setup.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 20:49:56.693672 autograd-1.6.1/tests/
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3217 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_binary_ops.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      644 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_builtins.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1151 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_complex.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1653 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_core.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3599 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_dict.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      860 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_direct.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     6104 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_fft.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     4963 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_graphs.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1444 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_jacobian.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    11222 2023-03-22 10:31:09.000000 autograd-1.6.1/tests/test_linalg.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1842 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_list.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1563 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_logic.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2970 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_misc.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    17858 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_numpy.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      144 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_performance.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     4514 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_scalar_ops.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    14435 2023-06-22 10:48:10.000000 autograd-1.6.1/tests/test_scipy.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    15326 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_systematic.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      785 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_tests.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      515 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_truediv.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1791 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_tuple.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5016 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_vspaces.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    10495 2020-03-21 18:01:53.000000 autograd-1.6.1/tests/test_wrappers.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.936080 autograd-1.6.2/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       41 2020-03-21 18:01:53.000000 autograd-1.6.2/MANIFEST.in
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      642 2023-06-23 08:35:52.936368 autograd-1.6.2/PKG-INFO
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4443 2020-03-21 18:01:53.000000 autograd-1.6.2/README.md
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.859987 autograd-1.6.2/autograd/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      504 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     6328 2023-06-22 12:39:21.000000 autograd-1.6.2/autograd/builtins.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    12235 2023-06-22 12:38:25.000000 autograd-1.6.2/autograd/core.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     8515 2022-06-15 10:01:07.000000 autograd-1.6.2/autograd/differential_operators.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      304 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/extend.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.874499 autograd-1.6.2/autograd/misc/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       62 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/misc/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      771 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/misc/fixed_points.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1120 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/misc/flatten.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2757 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/misc/optimizers.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2200 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/misc/tracers.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.887199 autograd-1.6.2/autograd/numpy/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      232 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/numpy/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5250 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/numpy/fft.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    11352 2022-09-29 07:03:46.000000 autograd-1.6.2/autograd/numpy/linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3496 2023-06-23 08:34:58.000000 autograd-1.6.2/autograd/numpy/numpy_boxes.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    10766 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/numpy/numpy_jvps.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    32566 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/numpy/numpy_vjps.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2846 2023-06-23 08:34:58.000000 autograd-1.6.2/autograd/numpy/numpy_vspaces.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5459 2021-03-03 09:26:31.000000 autograd-1.6.2/autograd/numpy/numpy_wrapper.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      149 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/numpy/random.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.893069 autograd-1.6.2/autograd/scipy/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      183 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2867 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/integrate.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2363 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      168 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/misc.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5924 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/signal.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5135 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/special.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.902501 autograd-1.6.2/autograd/scipy/stats/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      391 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1332 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/beta.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      809 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/chi2.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      772 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/dirichlet.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      987 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/gamma.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2509 2023-03-22 11:58:08.000000 autograd-1.6.2/autograd/scipy/stats/multivariate_normal.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2758 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/norm.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      715 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/poisson.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2670 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/scipy/stats/t.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2881 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/test_util.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3951 2023-06-22 12:38:25.000000 autograd-1.6.2/autograd/tracer.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1482 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/util.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1581 2020-03-21 18:01:53.000000 autograd-1.6.2/autograd/wrap_util.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.868943 autograd-1.6.2/autograd.egg-info/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      642 2023-06-23 08:35:52.000000 autograd-1.6.2/autograd.egg-info/PKG-INFO
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1710 2023-06-23 08:35:52.000000 autograd-1.6.2/autograd.egg-info/SOURCES.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)        1 2023-06-23 08:35:52.000000 autograd-1.6.2/autograd.egg-info/dependency_links.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       27 2023-06-23 08:35:52.000000 autograd-1.6.2/autograd.egg-info/requires.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)        9 2023-06-23 08:35:52.000000 autograd-1.6.2/autograd.egg-info/top_level.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       79 2023-06-23 08:35:52.937580 autograd-1.6.2/setup.cfg
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      952 2023-06-23 08:34:58.000000 autograd-1.6.2/setup.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-23 08:35:52.934804 autograd-1.6.2/tests/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3217 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_binary_ops.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      644 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_builtins.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1151 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_complex.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1653 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_core.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3599 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_dict.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      860 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_direct.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     6104 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_fft.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4963 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_graphs.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1444 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_jacobian.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    11222 2023-03-22 10:31:09.000000 autograd-1.6.2/tests/test_linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1842 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_list.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1563 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_logic.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2970 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_misc.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    17858 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_numpy.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      144 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_performance.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4514 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_scalar_ops.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    14435 2023-06-22 10:48:10.000000 autograd-1.6.2/tests/test_scipy.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    15326 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_systematic.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      785 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_tests.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      515 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_truediv.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1791 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_tuple.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5016 2020-03-21 18:01:53.000000 autograd-1.6.2/tests/test_vspaces.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    10645 2023-06-23 08:34:58.000000 autograd-1.6.2/tests/test_wrappers.py
```

### Comparing `autograd-1.6.1/PKG-INFO` & `autograd-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograd
-Version: 1.6.1
+Version: 1.6.2
 Summary: Efficiently computes derivatives of numpy code.
 Home-page: https://github.com/HIPS/autograd
 Author: Dougal Maclaurin and David Duvenaud and Matthew Johnson
 Author-email: maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu
 License: MIT
 Keywords: Automatic differentiation,backpropagation,gradients,machine learning,optimization,neural networks,Python,Numpy,Scipy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autograd-1.6.1/README.md` & `autograd-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/builtins.py` & `autograd-1.6.2/autograd/builtins.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/core.py` & `autograd-1.6.2/autograd/core.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/differential_operators.py` & `autograd-1.6.2/autograd/differential_operators.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/misc/fixed_points.py` & `autograd-1.6.2/autograd/misc/fixed_points.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/misc/flatten.py` & `autograd-1.6.2/autograd/misc/flatten.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/misc/optimizers.py` & `autograd-1.6.2/autograd/misc/optimizers.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/misc/tracers.py` & `autograd-1.6.2/autograd/misc/tracers.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/numpy/fft.py` & `autograd-1.6.2/autograd/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/numpy/linalg.py` & `autograd-1.6.2/autograd/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/numpy/numpy_boxes.py` & `autograd-1.6.2/autograd/numpy/numpy_boxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     def __ge__(self, other): return anp.greater_equal(self, other)
     def __lt__(self, other): return anp.less(self, other)
     def __le__(self, other): return anp.less_equal(self, other)
     def __abs__(self): return anp.abs(self)
     def __hash__(self): return id(self)
 
 ArrayBox.register(np.ndarray)
-for type_ in [float, np.float64, np.float32, np.float16,
-              complex, np.complex64, np.complex128]:
+for type_ in [float, np.longdouble, np.float64, np.float32, np.float16,
+              complex, np.clongdouble, np.complex64, np.complex128]:
     ArrayBox.register(type_)
 
 # These numpy.ndarray methods are just refs to an equivalent numpy function
 nondiff_methods = ['all', 'any', 'argmax', 'argmin', 'argpartition',
                    'argsort', 'nonzero', 'searchsorted', 'round']
 diff_methods = ['clip', 'compress', 'cumprod', 'cumsum', 'diagonal',
                 'max', 'mean', 'min', 'prod', 'ptp', 'ravel', 'repeat',
```

### Comparing `autograd-1.6.1/autograd/numpy/numpy_jvps.py` & `autograd-1.6.2/autograd/numpy/numpy_jvps.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/numpy/numpy_vjps.py` & `autograd-1.6.2/autograd/numpy/numpy_vjps.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/numpy/numpy_vspaces.py` & `autograd-1.6.2/autograd/numpy/numpy_vspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,18 @@
         return np.conj(x)
 
 VSpace.register(np.ndarray,
                 lambda x: ComplexArrayVSpace(x)
                 if np.iscomplexobj(x)
                 else ArrayVSpace(x))
 
-for type_ in [float, np.float64, np.float32, np.float16]:
+for type_ in [float, np.longdouble, np.float64, np.float32, np.float16]:
     ArrayVSpace.register(type_)
 
-for type_ in [complex, np.complex64, np.complex128]:
+for type_ in [complex, np.clongdouble, np.complex64, np.complex128]:
     ComplexArrayVSpace.register(type_)
 
 
 if np.__version__ >= '1.25':
     class EigResultVSpace(NamedTupleVSpace):     seq_type = np.linalg.linalg.EigResult
     class EighResultVSpace(NamedTupleVSpace):    seq_type = np.linalg.linalg.EighResult
     class QRResultVSpace(NamedTupleVSpace):      seq_type = np.linalg.linalg.QRResult
```

### Comparing `autograd-1.6.1/autograd/numpy/numpy_wrapper.py` & `autograd-1.6.2/autograd/numpy/numpy_wrapper.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/integrate.py` & `autograd-1.6.2/autograd/scipy/integrate.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/linalg.py` & `autograd-1.6.2/autograd/scipy/linalg.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/signal.py` & `autograd-1.6.2/autograd/scipy/signal.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/special.py` & `autograd-1.6.2/autograd/scipy/special.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/beta.py` & `autograd-1.6.2/autograd/scipy/stats/beta.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/chi2.py` & `autograd-1.6.2/autograd/scipy/stats/chi2.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/dirichlet.py` & `autograd-1.6.2/autograd/scipy/stats/dirichlet.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/gamma.py` & `autograd-1.6.2/autograd/scipy/stats/gamma.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/multivariate_normal.py` & `autograd-1.6.2/autograd/scipy/stats/multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/norm.py` & `autograd-1.6.2/autograd/scipy/stats/norm.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/poisson.py` & `autograd-1.6.2/autograd/scipy/stats/poisson.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/scipy/stats/t.py` & `autograd-1.6.2/autograd/scipy/stats/t.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/test_util.py` & `autograd-1.6.2/autograd/test_util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/tracer.py` & `autograd-1.6.2/autograd/tracer.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/util.py` & `autograd-1.6.2/autograd/util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd/wrap_util.py` & `autograd-1.6.2/autograd/wrap_util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/autograd.egg-info/PKG-INFO` & `autograd-1.6.2/autograd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograd
-Version: 1.6.1
+Version: 1.6.2
 Summary: Efficiently computes derivatives of numpy code.
 Home-page: https://github.com/HIPS/autograd
 Author: Dougal Maclaurin and David Duvenaud and Matthew Johnson
 Author-email: maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu
 License: MIT
 Keywords: Automatic differentiation,backpropagation,gradients,machine learning,optimization,neural networks,Python,Numpy,Scipy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autograd-1.6.1/autograd.egg-info/SOURCES.txt` & `autograd-1.6.2/autograd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/setup.py` & `autograd-1.6.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='autograd',
-    version='1.6.1',
+    version='1.6.2',
     description='Efficiently computes derivatives of numpy code.',
     author='Dougal Maclaurin and David Duvenaud and Matthew Johnson',
     author_email="maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu",
     packages=['autograd', 'autograd.numpy', 'autograd.scipy', 'autograd.scipy.stats', 'autograd.misc'],
     install_requires=['numpy>=1.12', 'future>=0.15.2'],
     keywords=['Automatic differentiation', 'backpropagation', 'gradients',
               'machine learning', 'optimization', 'neural networks',
```

### Comparing `autograd-1.6.1/tests/test_binary_ops.py` & `autograd-1.6.2/tests/test_binary_ops.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_builtins.py` & `autograd-1.6.2/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_complex.py` & `autograd-1.6.2/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_core.py` & `autograd-1.6.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_dict.py` & `autograd-1.6.2/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_direct.py` & `autograd-1.6.2/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_fft.py` & `autograd-1.6.2/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_graphs.py` & `autograd-1.6.2/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_jacobian.py` & `autograd-1.6.2/tests/test_jacobian.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_linalg.py` & `autograd-1.6.2/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_list.py` & `autograd-1.6.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_logic.py` & `autograd-1.6.2/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_misc.py` & `autograd-1.6.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_numpy.py` & `autograd-1.6.2/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_scalar_ops.py` & `autograd-1.6.2/tests/test_scalar_ops.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_scipy.py` & `autograd-1.6.2/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_systematic.py` & `autograd-1.6.2/tests/test_systematic.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_tests.py` & `autograd-1.6.2/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_truediv.py` & `autograd-1.6.2/tests/test_truediv.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_tuple.py` & `autograd-1.6.2/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_vspaces.py` & `autograd-1.6.2/tests/test_vspaces.py`

 * *Files identical despite different names*

### Comparing `autograd-1.6.1/tests/test_wrappers.py` & `autograd-1.6.2/tests/test_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,23 +222,29 @@
 def test_partial():
     def f(x, y):
         return x
     grad(partial(f, y=1))
 
 def test_dtypes():
     def f(x):
-        return np.sum(x**2)
+        return np.real(np.sum(x**2))
 
     # Array y with dtype np.float32
     y = np.random.randn(10, 10).astype(np.float32)
     assert grad(f)(y).dtype.type is np.float32
 
     y = np.random.randn(10, 10).astype(np.float16)
     assert grad(f)(y).dtype.type is np.float16
 
+    y = np.random.randn(10, 10).astype(np.longdouble)
+    grad(f)(y)
+
+    y = np.random.randn(10, 10).astype(np.clongdouble)
+    grad(f)(y)
+
 def test_checkpoint_correctness():
     bar = lambda x, y: 2*x + y + 5
     checkpointed_bar = checkpoint(bar)
     foo = lambda x: bar(x, x/3.) + bar(x, x**2)
     foo2 = lambda x: checkpointed_bar(x, x/3.) + checkpointed_bar(x, x**2)
     assert np.allclose(foo(3.), foo2(3.))
     assert np.allclose(grad(foo)(3.), grad(foo2)(3.))
```

