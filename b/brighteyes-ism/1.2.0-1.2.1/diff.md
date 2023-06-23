# Comparing `tmp/brighteyes-ism-1.2.0.tar.gz` & `tmp/brighteyes-ism-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brighteyes-ism-1.2.0.tar", last modified: Tue Jun 13 17:54:16 2023, max compression
+gzip compressed data, was "brighteyes-ism-1.2.1.tar", last modified: Fri Jun 23 14:12:04 2023, max compression
```

## Comparing `brighteyes-ism-1.2.0.tar` & `brighteyes-ism-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.856156 brighteyes-ism-1.2.0/
--rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4246 2023-06-13 17:54:16.856156 brighteyes-ism-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-23 10:37:26.000000 brighteyes-ism-1.2.0/README.md
--rw-rw-rw-   0        0        0     1006 2023-06-09 19:13:34.000000 brighteyes-ism-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1658 2023-06-13 17:54:16.857158 brighteyes-ism-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.833188 brighteyes-ism-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.839172 brighteyes-ism-1.2.0/src/brighteyes_ism/
--rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.851141 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/
--rw-rw-rw-   0        0        0     7231 2023-06-12 09:19:15.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/APR_lib.py
--rw-rw-rw-   0        0        0    16108 2023-06-12 10:11:08.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Deconv_lib.py
--rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FRC_lib.py
--rw-rw-rw-   0        0        0    11499 2023-05-31 13:30:30.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FocusISM_lib.py
--rw-rw-rw-   0        0        0    10496 2023-06-12 09:58:17.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Graph_lib.py
--rw-rw-rw-   0        0        0     6848 2023-06-10 15:14:36.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Tools_lib.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.852137 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/__init__.py
--rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/mcs.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.855168 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/
--rw-rw-rw-   0        0        0    21695 2023-06-13 17:51:50.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/PSF_sim.py
--rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/Tubulin_sim.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.844184 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/
--rw-rw-rw-   0        0        0     4246 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:04.017681 brighteyes-ism-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4246 2023-06-23 14:12:04.017681 brighteyes-ism-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-23 10:37:26.000000 brighteyes-ism-1.2.1/README.md
+-rw-rw-rw-   0        0        0     1006 2023-06-20 13:07:08.000000 brighteyes-ism-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1658 2023-06-23 14:12:04.018679 brighteyes-ism-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:03.991779 brighteyes-ism-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:03.998733 brighteyes-ism-1.2.1/src/brighteyes_ism/
+-rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:04.011698 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/
+-rw-rw-rw-   0        0        0     4934 2023-06-21 08:59:14.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/APR_lib.py
+-rw-rw-rw-   0        0        0    16108 2023-06-12 10:11:08.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Deconv_lib.py
+-rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/FRC_lib.py
+-rw-rw-rw-   0        0        0    11499 2023-05-31 13:30:30.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/FocusISM_lib.py
+-rw-rw-rw-   0        0        0    10496 2023-06-12 09:58:17.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Graph_lib.py
+-rw-rw-rw-   0        0        0     8661 2023-06-21 08:58:10.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Tools_lib.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:04.012694 brighteyes-ism-1.2.1/src/brighteyes_ism/dataio/
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/dataio/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/dataio/mcs.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:04.016684 brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/
+-rw-rw-rw-   0        0        0    21695 2023-06-13 17:51:50.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/PSF_sim.py
+-rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/Tubulin_sim.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:12:04.002721 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-06-23 14:12:03.000000 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-06-23 14:12:03.000000 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:12:03.000000 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-06-23 14:12:03.000000 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 14:12:03.000000 brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/top_level.txt
```

### Comparing `brighteyes-ism-1.2.0/LICENSE` & `brighteyes-ism-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/PKG-INFO` & `brighteyes-ism-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.2.0
+Version: 1.2.1
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.2.0/README.md` & `brighteyes-ism-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/pyproject.toml` & `brighteyes-ism-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "scikit-image>=0.19.2", "scikit-learn", "numpy", "scipy", "matplotlib", "joblib", "poppy", 	"PyCustomFocus", "h5py", "statsmodels", "tqdm", "matplotlib-scalebar"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brighteyes-ism"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Alessandro Zunino", email="alessandro.zunino@iit.it" },
 ]
 description = "A toolbox for analysing and simulating ISM images"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `brighteyes-ism-1.2.0/setup.cfg` & `brighteyes-ism-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7269 6768 7465 7965 732d 6973   = brighteyes-is
 00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e32  m..version = 1.2
-00000030: 2e30 0d0a 6175 7468 6f72 203d 2041 6c65  .0..author = Ale
+00000030: 2e31 0d0a 6175 7468 6f72 203d 2041 6c65  .1..author = Ale
 00000040: 7373 616e 6472 6f20 5a75 6e69 6e6f 0d0a  ssandro Zunino..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2061  author_email = a
 00000060: 6c65 7373 616e 6472 6f2e 7a75 6e69 6e6f  lessandro.zunino
 00000070: 4069 6974 2e69 740d 0a75 726c 203d 2068  @iit.it..url = h
 00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000090: 6d2f 5669 6369 646f 6d69 6e69 4c61 622f  m/VicidominiLab/
 000000a0: 6272 6967 6874 6579 6573 2d69 736d 0d0a  brighteyes-ism..
```

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Deconv_lib.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Deconv_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FRC_lib.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/FRC_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FocusISM_lib.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/FocusISM_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Graph_lib.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Graph_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Tools_lib.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/analysis/Tools_lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,87 @@
 import numpy as np
 
 from .FRC_lib import radial_profile
 
+def sigmoid(R: float, T: float, S: float):
+    '''
+    It generates a circularly-symmetric sigmoid function.
+
+    Parameters
+    ----------
+    R : float
+        Radial axis.
+    T : float
+        Cut-off frequency.
+    S : float
+        Sigmoid slope.
+
+    Returns
+    -------
+    np.ndarray
+        Sigmoid array. It has the same dimensions of R.
+
+    '''
+
+    return 1 / (1 + np.exp((R - T) / S))
+
+
+def low_pass(img: np.ndarray, T: float, S: float, data: str = 'real'):
+    '''
+    It applies a low-pass sigmoidal filter to a 2D image.
+
+    Parameters
+    ----------
+    img : np.ndarray
+        2D image.
+    T : float
+        Cut-off frequency.
+    S : float
+        Sigmoid slope.
+    data : str, optional
+        Domain of the image: It can be 'real' or 'fourier'.
+        The default is 'real'.
+
+    Returns
+    -------
+    img_filt : np.ndarray
+        Filtered 2D image, in the domain specified by 'data'.
+
+    '''
+
+    if data == 'real':
+        img_fft = np.fft.fftn(img, axes=(0, 1))
+        img_fft = np.fft.fftshift(img_fft, axes=(0, 1))
+    elif data == 'fourier':
+        img_fft = img
+    else:
+        raise ValueError('data has to be \'real\' or \'fourier\'')
+
+    Nx = np.shape(img_fft)[0]
+    Ny = np.shape(img_fft)[1]
+    cx = int((Nx + np.mod(Nx, 2)) / 2)
+    cy = int((Ny + np.mod(Ny, 2)) / 2)
+
+    x = (np.arange(Nx) - cx) / Nx
+    y = (np.arange(Ny) - cy) / Ny
+
+    X, Y = np.meshgrid(x, y)
+    R = np.sqrt(X ** 2 + Y ** 2)
+
+    sig = sigmoid(R, T, S)
+
+    img_filt = np.einsum('ij..., ij -> ij...', img_fft, sig)
+
+    if data == 'real':
+        img_filt = np.fft.ifftshift(img_filt, axes=(0, 1))
+        img_filt = np.fft.ifftn(img_filt, axes=(0, 1))
+        img_filt = np.abs(img_filt)
+
+    return img_filt
+
 
 # %%
 
 def Reorder(data, inOrder: str, outOrder: str = 'rzxytc'):
     '''
     It reorders a dataset to match the desired order of dimensions.
     If some dimensions are missing, it adds new dimensions.
```

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/mcs.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/dataio/mcs.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/PSF_sim.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/PSF_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/Tubulin_sim.py` & `brighteyes-ism-1.2.1/src/brighteyes_ism/simulation/Tubulin_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/PKG-INFO` & `brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.2.0
+Version: 1.2.1
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/SOURCES.txt` & `brighteyes-ism-1.2.1/src/brighteyes_ism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

