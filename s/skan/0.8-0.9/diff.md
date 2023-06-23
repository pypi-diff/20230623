# Comparing `tmp/skan-0.8.tar.gz` & `tmp/skan-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skan-0.8.tar", last modified: Sun Jul  7 20:35:43 2019, max compression
+gzip compressed data, was "dist/skan-0.9.tar", last modified: Fri Feb 26 05:29:52 2021, max compression
```

## Comparing `skan-0.8.tar` & `skan-0.9.tar`

### file list

```diff
@@ -1,35 +1,81 @@
-drwxr-xr-x   0 jni       (1000) jni       (1000)        0 2019-07-07 20:35:43.000000 skan-0.8/
--rw-r--r--   0 jni       (1000) jni       (1000)      141 2019-07-07 20:35:43.000000 skan-0.8/setup.cfg
-drwxr-xr-x   0 jni       (1000) jni       (1000)        0 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/
--rw-r--r--   0 jni       (1000) jni       (1000)      571 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/SOURCES.txt
--rw-r--r--   0 jni       (1000) jni       (1000)       46 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/entry_points.txt
--rw-r--r--   0 jni       (1000) jni       (1000)        5 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/top_level.txt
--rw-r--r--   0 jni       (1000) jni       (1000)      953 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/PKG-INFO
--rw-r--r--   0 jni       (1000) jni       (1000)        1 2019-07-07 20:35:43.000000 skan-0.8/skan.egg-info/dependency_links.txt
--rw-r--r--   0 jni       (1000) jni       (1000)       49 2018-07-12 21:04:46.000000 skan-0.8/MANIFEST.in
--rw-r--r--   0 jni       (1000) jni       (1000)      953 2019-07-07 20:35:43.000000 skan-0.8/PKG-INFO
--rw-r--r--   0 jni       (1000) jni       (1000)      417 2018-07-12 21:04:46.000000 skan-0.8/README.md
--rw-r--r--   0 jni       (1000) jni       (1000)     1708 2019-07-07 20:34:09.000000 skan-0.8/setup.py
--rw-r--r--   0 jni       (1000) jni       (1000)     1519 2018-07-12 21:04:46.000000 skan-0.8/LICENSE
-drwxr-xr-x   0 jni       (1000) jni       (1000)        0 2019-07-07 20:35:43.000000 skan-0.8/skan/
--rw-r--r--   0 jni       (1000) jni       (1000)     3219 2018-07-27 10:14:57.000000 skan-0.8/skan/pre.py
--rw-r--r--   0 jni       (1000) jni       (1000)      729 2019-05-24 15:27:08.000000 skan-0.8/skan/io.py
--rw-r--r--   0 jni       (1000) jni       (1000)    36297 2019-06-27 05:01:03.000000 skan-0.8/skan/csr.py
-drwxr-xr-x   0 jni       (1000) jni       (1000)        0 2019-07-07 20:35:43.000000 skan-0.8/skan/test/
--rw-r--r--   0 jni       (1000) jni       (1000)     1428 2019-05-28 03:13:35.000000 skan-0.8/skan/test/test_io.py
--rw-r--r--   0 jni       (1000) jni       (1000)     1264 2018-07-12 21:04:47.000000 skan-0.8/skan/test/test_vendored_correlate.py
--rw-r--r--   0 jni       (1000) jni       (1000)     2848 2018-07-27 10:15:08.000000 skan-0.8/skan/test/test_pre.py
--rw-r--r--   0 jni       (1000) jni       (1000)     4749 2019-06-27 05:01:03.000000 skan-0.8/skan/test/test_csr.py
--rw-r--r--   0 jni       (1000) jni       (1000)     3488 2019-06-27 05:01:03.000000 skan-0.8/skan/test/test_skeleton_class.py
--rw-r--r--   0 jni       (1000) jni       (1000)      874 2018-07-12 21:04:47.000000 skan-0.8/skan/test/test_pipe.py
--rw-r--r--   0 jni       (1000) jni       (1000)     3586 2018-07-12 21:04:47.000000 skan-0.8/skan/test/test_draw.py
--rw-r--r--   0 jni       (1000) jni       (1000)     5664 2019-05-28 03:13:35.000000 skan-0.8/skan/pipe.py
--rw-r--r--   0 jni       (1000) jni       (1000)     6668 2018-07-12 21:04:47.000000 skan-0.8/skan/nputil.py
--rw-r--r--   0 jni       (1000) jni       (1000)    12181 2019-06-27 05:01:03.000000 skan-0.8/skan/draw.py
--rw-r--r--   0 jni       (1000) jni       (1000)      212 2019-07-07 20:34:09.000000 skan-0.8/skan/__init__.py
--rw-r--r--   0 jni       (1000) jni       (1000)     2693 2018-07-12 21:04:47.000000 skan-0.8/skan/image_stats.py
--rw-r--r--   0 jni       (1000) jni       (1000)    11875 2019-05-24 04:51:12.000000 skan-0.8/skan/gui.py
-drwxr-xr-x   0 jni       (1000) jni       (1000)        0 2019-07-07 20:35:43.000000 skan-0.8/skan/vendored/
--rw-r--r--   0 jni       (1000) jni       (1000)     7886 2019-06-27 05:01:03.000000 skan-0.8/skan/vendored/thresholding.py
--rw-r--r--   0 jni       (1000) jni       (1000)        0 2018-07-12 21:04:47.000000 skan-0.8/skan/vendored/__init__.py
--rw-r--r--   0 jni       (1000) jni       (1000)     2250 2018-07-27 10:13:49.000000 skan-0.8/skan/_testdata.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.157653 skan-0.9/
+-rw-r--r--   0 jni        (501) staff       (20)      369 2021-02-26 05:29:45.000000 skan-0.9/.bumpversion.cfg
+-rw-r--r--   0 jni        (501) staff       (20)      187 2020-08-03 11:47:28.000000 skan-0.9/.coveragerc
+-rw-r--r--   0 jni        (501) staff       (20)     1170 2020-10-31 08:48:15.000000 skan-0.9/.gitignore
+-rw-r--r--   0 jni        (501) staff       (20)     2844 2020-08-03 11:47:28.000000 skan-0.9/.travis.yml
+-rw-r--r--   0 jni        (501) staff       (20)     1519 2020-08-03 11:47:28.000000 skan-0.9/LICENSE
+-rw-r--r--   0 jni        (501) staff       (20)       49 2020-08-03 11:47:28.000000 skan-0.9/MANIFEST.in
+-rw-r--r--   0 jni        (501) staff       (20)      103 2020-08-03 11:47:28.000000 skan-0.9/Makefile
+-rw-r--r--   0 jni        (501) staff       (20)      953 2021-02-26 05:29:52.157854 skan-0.9/PKG-INFO
+-rw-r--r--   0 jni        (501) staff       (20)      417 2020-08-03 11:47:28.000000 skan-0.9/README.md
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.124904 skan-0.9/benchmarks/
+-rw-r--r--   0 jni        (501) staff       (20)       50 2020-08-03 11:47:28.000000 skan-0.9/benchmarks/.gitattributes
+-rw-r--r--   0 jni        (501) staff       (20)     1699 2020-08-03 11:47:28.000000 skan-0.9/benchmarks/bench_skan.py
+-rw-r--r--   0 jni        (501) staff       (20)      131 2020-08-03 11:47:28.000000 skan-0.9/benchmarks/infected3.npz
+-rw-r--r--   0 jni        (501) staff       (20)      399 2020-08-03 11:47:28.000000 skan-0.9/config.json
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.132124 skan-0.9/doc/
+-rw-r--r--   0 jni        (501) staff       (20)      604 2020-08-03 11:47:28.000000 skan-0.9/doc/Makefile
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.132359 skan-0.9/doc/_static/
+-rw-r--r--   0 jni        (501) staff       (20)   199431 2020-08-03 11:47:28.000000 skan-0.9/doc/_static/gui-screenshot.png
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.134064 skan-0.9/doc/api/
+-rw-r--r--   0 jni        (501) staff       (20)      132 2020-08-03 11:47:28.000000 skan-0.9/doc/api/api.rst
+-rw-r--r--   0 jni        (501) staff       (20)      135 2020-08-03 11:47:28.000000 skan-0.9/doc/api/skan.csr.rst
+-rw-r--r--   0 jni        (501) staff       (20)      108 2020-08-03 11:47:28.000000 skan-0.9/doc/api/skan.draw.rst
+-rw-r--r--   0 jni        (501) staff       (20)      146 2020-08-03 11:47:28.000000 skan-0.9/doc/api/skan.pipe.rst
+-rw-r--r--   0 jni        (501) staff       (20)       99 2020-08-03 11:47:28.000000 skan-0.9/doc/api/skan.pre.rst
+-rw-r--r--   0 jni        (501) staff       (20)      246 2020-08-03 11:47:28.000000 skan-0.9/doc/api/skan.vendored.thresholding.rst
+-rw-r--r--   0 jni        (501) staff       (20)   518374 2020-08-03 11:47:28.000000 skan-0.9/doc/complete_analysis.ipynb
+-rw-r--r--   0 jni        (501) staff       (20)     6950 2020-08-03 11:47:28.000000 skan-0.9/doc/complete_analysis.rst
+-rw-r--r--   0 jni        (501) staff       (20)     5856 2020-08-03 11:47:28.000000 skan-0.9/doc/conf.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.141888 skan-0.9/doc/example-data/
+-rw-r--r--   0 jni        (501) staff       (20)  1701667 2020-08-03 11:47:28.000000 skan-0.9/doc/example-data/inf1.tif
+-rw-r--r--   0 jni        (501) staff       (20)  1701661 2020-08-03 11:47:28.000000 skan-0.9/doc/example-data/inf2.tif
+-rw-r--r--   0 jni        (501) staff       (20)  1701666 2020-08-03 11:47:28.000000 skan-0.9/doc/example-data/rbc1.tif
+-rw-r--r--   0 jni        (501) staff       (20)  1701663 2020-08-03 11:47:28.000000 skan-0.9/doc/example-data/rbc2.tif
+-rw-r--r--   0 jni        (501) staff       (20)  2902444 2020-08-03 11:47:28.000000 skan-0.9/doc/getting_started.ipynb
+-rw-r--r--   0 jni        (501) staff       (20)    15095 2021-02-26 05:24:42.000000 skan-0.9/doc/getting_started.rst
+-rw-r--r--   0 jni        (501) staff       (20)     3586 2020-08-03 11:47:28.000000 skan-0.9/doc/gui.rst
+-rw-r--r--   0 jni        (501) staff       (20)      807 2020-08-03 11:47:28.000000 skan-0.9/doc/index.rst
+-rw-r--r--   0 jni        (501) staff       (20)     1125 2020-08-03 11:47:28.000000 skan-0.9/doc/install.rst
+-rw-r--r--   0 jni        (501) staff       (20)      802 2020-08-03 11:47:28.000000 skan-0.9/doc/make.bat
+-rw-r--r--   0 jni        (501) staff       (20)     4408 2020-08-03 11:47:28.000000 skan-0.9/github_deploy_key_jni_skan.enc
+-rw-r--r--   0 jni        (501) staff       (20)       63 2020-08-03 11:47:28.000000 skan-0.9/readthedocs.yml
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.144616 skan-0.9/requirements/
+-rw-r--r--   0 jni        (501) staff       (20)      168 2020-08-03 11:47:28.000000 skan-0.9/requirements/default.txt
+-rw-r--r--   0 jni        (501) staff       (20)      102 2020-08-03 11:47:28.000000 skan-0.9/requirements/doc.txt
+-rw-r--r--   0 jni        (501) staff       (20)       78 2020-08-03 11:47:28.000000 skan-0.9/requirements/test.txt
+-rw-r--r--   0 jni        (501) staff       (20)       53 2020-08-03 11:47:28.000000 skan-0.9/requirements.txt
+-rw-r--r--   0 jni        (501) staff       (20)      141 2021-02-26 05:29:52.158304 skan-0.9/setup.cfg
+-rw-r--r--   0 jni        (501) staff       (20)     1708 2021-02-26 05:29:45.000000 skan-0.9/setup.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.147143 skan-0.9/skan/
+-rw-r--r--   0 jni        (501) staff       (20)      212 2021-02-26 05:29:45.000000 skan-0.9/skan/__init__.py
+-rw-r--r--   0 jni        (501) staff       (20)     2250 2020-08-03 11:47:28.000000 skan-0.9/skan/_testdata.py
+-rw-r--r--   0 jni        (501) staff       (20)    36886 2021-02-26 05:22:46.000000 skan-0.9/skan/csr.py
+-rw-r--r--   0 jni        (501) staff       (20)    12181 2020-08-03 11:47:28.000000 skan-0.9/skan/draw.py
+-rw-r--r--   0 jni        (501) staff       (20)    11875 2020-08-03 11:47:28.000000 skan-0.9/skan/gui.py
+-rw-r--r--   0 jni        (501) staff       (20)     2693 2020-08-03 11:47:28.000000 skan-0.9/skan/image_stats.py
+-rw-r--r--   0 jni        (501) staff       (20)      729 2020-08-03 11:47:28.000000 skan-0.9/skan/io.py
+-rw-r--r--   0 jni        (501) staff       (20)     6668 2020-08-03 11:47:28.000000 skan-0.9/skan/nputil.py
+-rw-r--r--   0 jni        (501) staff       (20)     5905 2020-10-31 08:52:40.000000 skan-0.9/skan/pipe.py
+-rw-r--r--   0 jni        (501) staff       (20)     3219 2020-08-03 11:47:28.000000 skan-0.9/skan/pre.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.154024 skan-0.9/skan/test/
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.156697 skan-0.9/skan/test/data/
+-rw-r--r--   0 jni        (501) staff       (20)  1701693 2020-08-03 11:47:28.000000 skan-0.9/skan/test/data/retic.tif
+-rw-r--r--   0 jni        (501) staff       (20)    68208 2020-08-03 11:47:28.000000 skan-0.9/skan/test/data/skeleton.tif
+-rw-r--r--   0 jni        (501) staff       (20)     4749 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_csr.py
+-rw-r--r--   0 jni        (501) staff       (20)     3586 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_draw.py
+-rw-r--r--   0 jni        (501) staff       (20)     1428 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_io.py
+-rw-r--r--   0 jni        (501) staff       (20)      874 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_pipe.py
+-rw-r--r--   0 jni        (501) staff       (20)     2848 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_pre.py
+-rw-r--r--   0 jni        (501) staff       (20)     3488 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_skeleton_class.py
+-rw-r--r--   0 jni        (501) staff       (20)     1264 2020-08-03 11:47:28.000000 skan-0.9/skan/test/test_vendored_correlate.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.157284 skan-0.9/skan/vendored/
+-rw-r--r--   0 jni        (501) staff       (20)        0 2020-08-03 11:47:28.000000 skan-0.9/skan/vendored/__init__.py
+-rw-r--r--   0 jni        (501) staff       (20)     7886 2020-08-03 11:47:28.000000 skan-0.9/skan/vendored/thresholding.py
+drwxr-xr-x   0 jni        (501) staff       (20)        0 2021-02-26 05:29:52.152120 skan-0.9/skan.egg-info/
+-rw-r--r--   0 jni        (501) staff       (20)      953 2021-02-26 05:29:51.000000 skan-0.9/skan.egg-info/PKG-INFO
+-rw-r--r--   0 jni        (501) staff       (20)     1386 2021-02-26 05:29:52.000000 skan-0.9/skan.egg-info/SOURCES.txt
+-rw-r--r--   0 jni        (501) staff       (20)        1 2021-02-26 05:29:51.000000 skan-0.9/skan.egg-info/dependency_links.txt
+-rw-r--r--   0 jni        (501) staff       (20)       46 2021-02-26 05:29:51.000000 skan-0.9/skan.egg-info/entry_points.txt
+-rw-r--r--   0 jni        (501) staff       (20)        5 2021-02-26 05:29:51.000000 skan-0.9/skan.egg-info/top_level.txt
+-rw-r--r--   0 jni        (501) staff       (20)      440 2020-08-03 11:47:28.000000 skan-0.9/test-environment.yml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `skan-0.8/skan.egg-info/PKG-INFO` & `skan-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: skan
-Version: 0.8
+Version: 0.9
 Summary: Analysis of object skeletons
 Home-page: https://github.com/jni/skan
 Author: Juan Nunez-Iglesias
 Author-email: juan.n@unimelb.edu.au
 License: BSD 3-clause
 Description: skan: skeleton analysis in Python.
```

### Comparing `skan-0.8/PKG-INFO` & `skan-0.9/skan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: skan
-Version: 0.8
+Version: 0.9
 Summary: Analysis of object skeletons
 Home-page: https://github.com/jni/skan
 Author: Juan Nunez-Iglesias
 Author-email: juan.n@unimelb.edu.au
 License: BSD 3-clause
 Description: skan: skeleton analysis in Python.
```

### Comparing `skan-0.8/setup.py` & `skan-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 DESCRIPTION         = 'Analysis of object skeletons'
 LONG_DESCRIPTION    = descr
 MAINTAINER          = 'Juan Nunez-Iglesias'
 MAINTAINER_EMAIL    = 'juan.n@unimelb.edu.au'
 URL                 = 'https://github.com/jni/skan'
 LICENSE             = 'BSD 3-clause'
 DOWNLOAD_URL        = 'https://github.com/jni/skan'
-VERSION             = '0.8'
+VERSION             = '0.9'
 PYTHON_VERSION      = (3, 6)
 INST_DEPENDENCIES   = []
 
 
 if __name__ == '__main__':
 
     setup(name=DISTNAME,
```

### Comparing `skan-0.8/LICENSE` & `skan-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/pre.py` & `skan-0.9/skan/pre.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/io.py` & `skan-0.9/skan/io.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/csr.py` & `skan-0.9/skan/csr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ('indptr', numba.int32[:]),
     ('indices', numba.int32[:]),
     ('data', numba.float64[:]),
     ('shape', numba.int32[:]),
     ('node_properties', numba.float64[:])
 ]
 
-@numba.jitclass(csr_spec)
+@numba.experimental.jitclass(csr_spec)
 class NBGraph:
     def __init__(self, indptr, indices, data, shape, node_props):
         self.indptr = indptr
         self.indices = indices
         self.data = data
         self.shape = shape
         self.node_properties = node_props
@@ -275,14 +275,18 @@
     source_image : array of float, same shape as `skeleton_image`
         The image that `skeleton_image` represents / summarizes / was generated
         from. This is used to produce visualizations as well as statistical
         properties of paths.
     keep_images : bool
         Whether or not to keep the original input images. These can be useful
         for visualization, but they may take up a lot of memory.
+    unique_junctions : bool, optional
+        If True, adjacent junction nodes get collapsed into a single
+        conceptual node, with position at the centroid of all the connected
+        initial nodes.
 
     Attributes
     ----------
     graph : scipy.sparse.csr_matrix, shape (N + 1, N + 1)
         The skeleton pixel graph, where each node is a non-zero pixel in the
         input image, and each edge connects adjacent pixels. The graph is
         represented as an adjacency matrix in SciPy sparse matrix format. For
@@ -298,26 +302,29 @@
     paths : scipy.sparse.csr_matrix, shape (P, N + 1)
         A csr_matrix where element [i, j] is on if node j is in path i. This
         includes path endpoints. The number of nonzero elements is N - J + Sd.
     n_paths : int
         The number of paths, P. This is redundant information given `n_paths`,
         but it is used often enough that it is worth keeping around.
     distances : array of float, shape (P,)
-        The distance of each path.
+        The distance of each path. Note: not initialized until `path_lengths()`
+        is called on the skeleton; use path_lengths() instead
     skeleton_image : array or None
         The input skeleton image. Only present if `keep_images` is True. Set to
         False to preserve memory.
     source_image : array or None
         The image from which the skeleton was derived. Only present if
         `keep_images` is True. This is useful for visualization.
     """
     def __init__(self, skeleton_image, *, spacing=1, source_image=None,
-                 _buffer_size_offset=None, keep_images=True):
+                 _buffer_size_offset=None, keep_images=True, 
+                 unique_junctions=True):
         graph, coords, degrees = skeleton_to_csgraph(skeleton_image,
-                                                     spacing=spacing)
+                                                     spacing=spacing,
+                                                     unique_junctions=unique_junctions)
         if np.issubdtype(skeleton_image.dtype, np.float_):
             pixel_values = ndi.map_coordinates(skeleton_image, coords.T,
                                                order=3)
         else:
             pixel_values = None
         self.graph = graph
         self.nbgraph = csr_to_nbgraph(graph, pixel_values)
@@ -581,15 +588,17 @@
         A graph of shape (Nnz + 1, Nnz + 1), where Nnz is the number of
         nonzero pixels in `skel`. The value graph[i, j] is the distance
         between adjacent pixels i and j. In a 2D image, that would be
         1 for immediately adjacent pixels and sqrt(2) for diagonally
         adjacent ones.
     pixel_coordinates : array of float
         An array of shape (Nnz + 1, skel.ndim), mapping indices in `graph`
-        to pixel coordinates in `degree_image` or `skel`.
+        to pixel coordinates in `degree_image` or `skel`. Array entry
+        (0,:) contains currently always zeros to index the pixels, which
+        start at 1, directly to the coordinates.
     degree_image : array of int, same shape as skel
         An image where each pixel value contains the degree of its
         corresponding node in `graph`. This is useful to classify nodes.
     """
     height = pad(skel, 0.) if value_is_height else None
     # ensure we have a bool image, since we later use it for bool indexing
     skel = skel.astype(bool)
```

### Comparing `skan-0.8/skan/test/test_io.py` & `skan-0.9/skan/test/test_io.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_vendored_correlate.py` & `skan-0.9/skan/test/test_vendored_correlate.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_pre.py` & `skan-0.9/skan/test/test_pre.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_csr.py` & `skan-0.9/skan/test/test_csr.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_skeleton_class.py` & `skan-0.9/skan/test/test_skeleton_class.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_pipe.py` & `skan-0.9/skan/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/test/test_draw.py` & `skan-0.9/skan/test/test_draw.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/pipe.py` & `skan-0.9/skan/pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,28 @@
 from skimage.feature import shape_index
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import multiprocessing as mp
 
 
 CPU_COUNT = int(os.environ.get('CPU_COUNT', mp.cpu_count()))
 
-
 def _get_scale(image, md_path_or_scale):
-    """Get a valid scale from an image and a metadata path or scale."""
+    """Get a valid scale from an image and a metadata path or scale.
+
+    Parameters
+    ----------
+    image : np.ndarray
+        The input image.
+    md_path_or_scale : float or image filename
+        The path to the file containing the metadata, or the scale.
+
+    Returns
+    -------
+    scale : float
+    """
     scale = None
     try:
         scale = float(md_path_or_scale)
     except ValueError:
         pass
     if md_path_or_scale is not None and scale is None:
         md_path = md_path_or_scale.split(sep='/')
```

### Comparing `skan-0.8/skan/nputil.py` & `skan-0.9/skan/nputil.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/draw.py` & `skan-0.9/skan/draw.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/image_stats.py` & `skan-0.9/skan/image_stats.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/gui.py` & `skan-0.9/skan/gui.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/vendored/thresholding.py` & `skan-0.9/skan/vendored/thresholding.py`

 * *Files identical despite different names*

### Comparing `skan-0.8/skan/_testdata.py` & `skan-0.9/skan/_testdata.py`

 * *Files identical despite different names*

