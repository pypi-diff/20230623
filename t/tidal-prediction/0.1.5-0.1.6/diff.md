# Comparing `tmp/tidal-prediction-0.1.5.tar.gz` & `tmp/tidal-prediction-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal-prediction-0.1.5.tar", last modified: Thu Jun 22 16:15:02 2023, max compression
+gzip compressed data, was "tidal-prediction-0.1.6.tar", last modified: Fri Jun 23 06:16:06 2023, max compression
```

## Comparing `tidal-prediction-0.1.5.tar` & `tidal-prediction-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     1077 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      779 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE.BASEMAP
--rw-rw-r--   0 jbl       (1000) jbl       (1000)    19092 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE.OTPS.pdf
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/PKG-INFO
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     5102 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/README.md
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/scripts/
--rwxrwxr-x   0 jbl       (1000) jbl       (1000)    28396 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/scripts/extract_local_model.py
--rwxrwxr-x   0 jbl       (1000) jbl       (1000)     1740 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/scripts/predict_tide.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/setup.cfg
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      503 2023-06-22 16:13:19.000000 tidal-prediction-0.1.5/setup.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/__init__.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/convert/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/convert/__init__.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      429 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/convert/io_nc.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/tide/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/__init__.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     3951 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/nc.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     3912 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tideconstit.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)    12311 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tidemodel.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)    26373 2023-06-22 16:12:04.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tideutils.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction.egg-info/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/PKG-INFO
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      582 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/SOURCES.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        1 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/dependency_links.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/requires.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       17 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/top_level.txt
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.553393 tidal-prediction-0.1.6/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     1077 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/LICENSE
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      779 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/LICENSE.BASEMAP
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    19092 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/LICENSE.OTPS.pdf
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/PKG-INFO
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     5102 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/README.md
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/scripts/
+-rwxrwxr-x   0 jbl       (1000) jbl       (1000)    28396 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/scripts/extract_local_model.py
+-rwxrwxr-x   0 jbl       (1000) jbl       (1000)     1740 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/scripts/predict_tide.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-23 06:16:06.553393 tidal-prediction-0.1.6/setup.cfg
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      503 2023-06-23 06:12:21.000000 tidal-prediction-0.1.6/setup.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/tidal_prediction/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/__init__.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/tidal_prediction/convert/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/convert/__init__.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      429 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/convert/io_nc.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/tidal_prediction/tide/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/tide/__init__.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     3951 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/tide/nc.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     3912 2021-02-15 11:47:25.000000 tidal-prediction-0.1.6/tidal_prediction/tide/tideconstit.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    12308 2023-06-23 06:13:50.000000 tidal-prediction-0.1.6/tidal_prediction/tide/tidemodel.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    26373 2023-06-22 16:12:04.000000 tidal-prediction-0.1.6/tidal_prediction/tide/tideutils.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-23 06:16:06.549393 tidal-prediction-0.1.6/tidal_prediction.egg-info/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-23 06:16:06.000000 tidal-prediction-0.1.6/tidal_prediction.egg-info/PKG-INFO
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      582 2023-06-23 06:16:06.000000 tidal-prediction-0.1.6/tidal_prediction.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        1 2023-06-23 06:16:06.000000 tidal-prediction-0.1.6/tidal_prediction.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-23 06:16:06.000000 tidal-prediction-0.1.6/tidal_prediction.egg-info/requires.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       17 2023-06-23 06:16:06.000000 tidal-prediction-0.1.6/tidal_prediction.egg-info/top_level.txt
```

### Comparing `tidal-prediction-0.1.5/LICENSE` & `tidal-prediction-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/LICENSE.BASEMAP` & `tidal-prediction-0.1.6/LICENSE.BASEMAP`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/LICENSE.OTPS.pdf` & `tidal-prediction-0.1.6/LICENSE.OTPS.pdf`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/README.md` & `tidal-prediction-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/scripts/extract_local_model.py` & `tidal-prediction-0.1.6/scripts/extract_local_model.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/scripts/predict_tide.py` & `tidal-prediction-0.1.6/scripts/predict_tide.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/tidal_prediction/tide/nc.py` & `tidal-prediction-0.1.6/tidal_prediction/tide/nc.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/tidal_prediction/tide/tideconstit.py` & `tidal-prediction-0.1.6/tidal_prediction/tide/tideconstit.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/tidal_prediction/tide/tidemodel.py` & `tidal-prediction-0.1.6/tidal_prediction/tide/tidemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             # Calculate inverse depth for current calculations
             if 'u' in self.outputs or 'v' in self.outputs:
                 depths_inv = 1.0 / depths
 
             # Read in elevations.
             if 'z' in self.outputs:
                 # Read in elevation constituents from NetCDF file
-                h = np.ma.empty((ncon, jj - j, nlon), dtype=np.complex)
+                h = np.ma.empty((ncon, jj - j, nlon), dtype=np.cdouble)
                 for k, constid in enumerate(self.constids):
                     # Read in elevation values and convert from mm to m
                     h[k] = read_complex_chunk(self.infile, ['hRe', 'hIm'],
                                               jslice, k)
                 ptideH = tideutils.Ptide(h, self.constids,
                                          self.interpolate_minor)
 
@@ -192,23 +192,23 @@
                     # Calculate elevation
                     hout = ptideH(fc_list[itime], fs_list[itime],
                                   A_list[itime])
                     write_chunk(outfile, 'z', itime, jslice, hout)
 
             if 'u' in self.outputs or 'U' in self.outputs:
                 # Read in u-transport constituents from NetCDF file
-                U = np.ma.empty((ncon, jj - j, nlon), dtype=np.complex)
+                U = np.ma.empty((ncon, jj - j, nlon), dtype=np.cdouble)
                 for k in range(ncon):
                     # Read in u-transport values (m**2/s)
                     U[k] = read_complex_chunk(self.infile, ['uRe', 'uIm'],
                                               jslice, k)
 
             if 'v' in self.outputs or 'V' in self.outputs:
                 # Read in v-transport constituents from NetCDF file
-                V = np.ma.empty((ncon, jj - j, nlon), dtype=np.complex)
+                V = np.ma.empty((ncon, jj - j, nlon), dtype=np.cdouble)
                 for k in range(ncon):
                     # Read in v-transport values (m**2/s)
                     V[k] = read_complex_chunk(self.infile, ['vRe', 'vIm'],
                                               jslice, k)
 
             # Limit suspicious constituents before running model
             if 'u' in self.outputs or 'U' in self.outputs:
@@ -246,29 +246,29 @@
 
 def read_real_chunk(ncfile, ncvar, jslice):
     return ncfile.variables[ncvar][jslice, :]
 
 
 def read_complex_chunk(ncfile, ncvars, jslice, k):
     value = np.ma.array(
-        ncfile.variables[ncvars[0]][k, jslice, :], dtype=np.complex)
+        ncfile.variables[ncvars[0]][k, jslice, :], dtype=np.cdouble)
     value += ncfile.variables[ncvars[1]][k, jslice, :] * 1.0j
     return value
 
 
 def write_chunk(ncfile, ncvar, itime, jslice, hout):
     # Write elevations to NetCDF file
     ncfile.variables[ncvar][itime, jslice, :] = hout
 
 
 def limit_suspicious_constituents(U, V, depths, maxnorm=4.0):
     """\
    Finds the summed norm of the complex transport constituents
    and divides it by the depth to find the summed current speed.
-   
+
    The transport constituents are then capped at a current speed
    of 1 m/s.
    """
     # Find norm at each grid point
     #norm = 0.25*(np.ma.sqrt(np.ma.sqrt(U.real**2).sum(axis=0)**2 + \
     #                        np.ma.sqrt(U.imag**2).sum(axis=0)**2) + \
     #             np.ma.sqrt(np.ma.sqrt(V.real**2).sum(axis=0)**2 + \
```

### Comparing `tidal-prediction-0.1.5/tidal_prediction/tide/tideutils.py` & `tidal-prediction-0.1.6/tidal_prediction/tide/tideutils.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.5/tidal_prediction.egg-info/SOURCES.txt` & `tidal-prediction-0.1.6/tidal_prediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

