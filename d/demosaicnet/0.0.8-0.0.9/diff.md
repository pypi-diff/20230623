# Comparing `tmp/demosaicnet-0.0.8.tar.gz` & `tmp/demosaicnet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/demosaicnet-0.0.8.tar", last modified: Sun Apr  5 23:39:43 2020, max compression
+gzip compressed data, was "dist/demosaicnet-0.0.9.tar", last modified: Mon Apr  6 21:48:33 2020, max compression
```

## Comparing `demosaicnet-0.0.8.tar` & `demosaicnet-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      111 2019-03-14 11:46:22.000000 demosaicnet-0.0.8/MANIFEST.in
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     1092 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/PKG-INFO
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      410 2019-08-22 18:04:28.000000 demosaicnet-0.0.8/README.md
-drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet/
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      149 2019-09-20 22:04:49.000000 demosaicnet-0.0.8/demosaicnet/__init__.py
-drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet/data/
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)  2251181 2019-03-14 11:46:23.000000 demosaicnet-0.0.8/demosaicnet/data/bayer.pth
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)    36594 2019-03-14 11:46:23.000000 demosaicnet-0.0.8/demosaicnet/data/test_input.png
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)  1644547 2019-03-14 11:46:23.000000 demosaicnet-0.0.8/demosaicnet/data/xtrans.pth
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)    24897 2020-04-05 20:41:49.000000 demosaicnet-0.0.8/demosaicnet/dataset.py
--rw-r--r--   0 mgharbi   (1000) mgharbi   (1000)     4909 2020-01-03 20:34:17.000000 demosaicnet-0.0.8/demosaicnet/modules.py
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     2233 2020-04-05 23:37:28.000000 demosaicnet-0.0.8/demosaicnet/mosaic.py
--rw-r--r--   0 mgharbi   (1000) mgharbi   (1000)       22 2020-04-05 23:39:26.000000 demosaicnet-0.0.8/demosaicnet/version.py
-drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     1092 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/PKG-INFO
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      431 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/SOURCES.txt
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)        1 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/dependency_links.txt
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       17 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/requires.txt
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       12 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/demosaicnet.egg-info/top_level.txt
-drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/scripts/
--rwxr-xr-x   0 mgharbi   (1000) mgharbi   (1000)     1823 2020-04-05 20:42:17.000000 demosaicnet-0.0.8/scripts/demosaicnet_demo
--rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       38 2020-04-05 23:39:43.000000 demosaicnet-0.0.8/setup.cfg
--rwxr-xr-x   0 mgharbi   (1000) mgharbi   (1000)      989 2019-09-20 22:18:10.000000 demosaicnet-0.0.8/setup.py
+drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      111 2019-03-14 11:46:22.000000 demosaicnet-0.0.9/MANIFEST.in
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     1092 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/PKG-INFO
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      410 2019-08-22 18:04:28.000000 demosaicnet-0.0.9/README.md
+drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet/
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      149 2019-09-20 22:04:49.000000 demosaicnet-0.0.9/demosaicnet/__init__.py
+drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet/data/
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)  2251181 2019-03-14 11:46:23.000000 demosaicnet-0.0.9/demosaicnet/data/bayer.pth
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)    36594 2019-03-14 11:46:23.000000 demosaicnet-0.0.9/demosaicnet/data/test_input.png
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)  1644547 2019-03-14 11:46:23.000000 demosaicnet-0.0.9/demosaicnet/data/xtrans.pth
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)    24897 2020-04-05 20:41:49.000000 demosaicnet-0.0.9/demosaicnet/dataset.py
+-rw-r--r--   0 mgharbi   (1000) mgharbi   (1000)     4909 2020-01-03 20:34:17.000000 demosaicnet-0.0.9/demosaicnet/modules.py
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     2450 2020-04-06 21:48:08.000000 demosaicnet-0.0.9/demosaicnet/mosaic.py
+-rw-r--r--   0 mgharbi   (1000) mgharbi   (1000)       22 2020-04-06 21:48:12.000000 demosaicnet-0.0.9/demosaicnet/version.py
+drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)     1092 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/PKG-INFO
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)      431 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)        1 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       17 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/requires.txt
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       12 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/demosaicnet.egg-info/top_level.txt
+drwxrwxr-x   0 mgharbi   (1000) mgharbi   (1000)        0 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/scripts/
+-rwxr-xr-x   0 mgharbi   (1000) mgharbi   (1000)     1823 2020-04-05 20:42:17.000000 demosaicnet-0.0.9/scripts/demosaicnet_demo
+-rw-rw-r--   0 mgharbi   (1000) mgharbi   (1000)       38 2020-04-06 21:48:33.000000 demosaicnet-0.0.9/setup.cfg
+-rwxr-xr-x   0 mgharbi   (1000) mgharbi   (1000)      989 2019-09-20 22:18:10.000000 demosaicnet-0.0.9/setup.py
```

### Comparing `demosaicnet-0.0.8/PKG-INFO` & `demosaicnet-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: demosaicnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Minimal implementation of Deep Joint Demosaicking and Denoising [Gharbi2016]
 Home-page: https://github.com/mgharbi/
 Author: Michaël Gharbi
 Author-email: gharbi@csail.mit.edu
 License: UNKNOWN
 Description: # Deep Joint Demosaicking and Denoising
         SiGGRAPH Asia 2016
```

### Comparing `demosaicnet-0.0.8/demosaicnet/data/bayer.pth` & `demosaicnet-0.0.9/demosaicnet/data/bayer.pth`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/demosaicnet/data/test_input.png` & `demosaicnet-0.0.9/demosaicnet/data/test_input.png`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/demosaicnet/data/xtrans.pth` & `demosaicnet-0.0.9/demosaicnet/data/xtrans.pth`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/demosaicnet/dataset.py` & `demosaicnet-0.0.9/demosaicnet/dataset.py`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/demosaicnet/modules.py` & `demosaicnet-0.0.9/demosaicnet/modules.py`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/demosaicnet/mosaic.py` & `demosaicnet-0.0.9/demosaicnet/mosaic.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     im(np.array, th.Tensor): image to mosaic. Dimensions are [c, h, w]
     mask(bool): if true return the binary mosaic mask, instead of the mosaic image.
 
   Returns:
     np.array: mosaicked image (if mask==False), or binary mask if (mask==True)
   """
 
-  mask = np.zeros((3, 6, 6), dtype=np.float32)
   g_pos = [(0,0),        (0,2), (0,3),        (0,5),
                   (1,1),               (1,4),
            (2,0),        (2,2), (2,3),        (2,5),
            (3,0),        (3,2), (3,3),        (3,5),
                   (4,1),               (4,4),
            (5,0),        (5,2), (5,3),        (5,5)]
   r_pos = [(0,4),
@@ -81,19 +80,37 @@
   b_pos = [(0,1),
            (1,3), (1,5),
            (2,1),
            (3,4),
            (4,0), (4,2),
            (5,4)]
 
+  numpy = False
+  if type(im) == np.ndarray:
+    numpy = True
+    mask = np.zeros((3, 6, 6), dtype=np.float32)
+  else:
+    mask = th.zeros(3, 6, 6)
+
   for idx, coord in enumerate([r_pos, g_pos, b_pos]):
     for y, x in coord:
-      mask[idx, y, x] = 1
+      mask[..., idx, y, x] = 1
+
+  h, w = im.shape[-2:]
+
+  new_sz = [np.ceil(h / 6).astype(np.int32), np.ceil(w / 6).astype(np.int32)]
+
+  sz = np.array(mask.shape)
+  sz[:-2] = 1
+  sz[-2:] = new_sz
+
+  if numpy:
+    mask = np.tile(mask, sz)
+  else:
+    mask = mask.repeat(*sz)
+
+  mask = mask[..., :, :h, :w]
 
-  _, h, w = im.shape
-  mask = np.tile(mask, [1, np.ceil(h / 6).astype(np.int32),
-                        np.ceil(w / 6).astype(np.int32)])
-  mask = mask[:, :h, :w]
   if return_mask:
     return mask
 
   return mask*im
```

### Comparing `demosaicnet-0.0.8/demosaicnet.egg-info/PKG-INFO` & `demosaicnet-0.0.9/demosaicnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: demosaicnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Minimal implementation of Deep Joint Demosaicking and Denoising [Gharbi2016]
 Home-page: https://github.com/mgharbi/
 Author: Michaël Gharbi
 Author-email: gharbi@csail.mit.edu
 License: UNKNOWN
 Description: # Deep Joint Demosaicking and Denoising
         SiGGRAPH Asia 2016
```

### Comparing `demosaicnet-0.0.8/scripts/demosaicnet_demo` & `demosaicnet-0.0.9/scripts/demosaicnet_demo`

 * *Files identical despite different names*

### Comparing `demosaicnet-0.0.8/setup.py` & `demosaicnet-0.0.9/setup.py`

 * *Files identical despite different names*

