# Comparing `tmp/pyspk-1.6.tar.gz` & `tmp/pyspk-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.6.tar", last modified: Wed Jun 21 12:49:58 2023, max compression
+gzip compressed data, was "pyspk-1.7.tar", last modified: Fri Jun 23 09:52:03 2023, max compression
```

## Comparing `pyspk-1.6.tar` & `pyspk-1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.363867 pyspk-1.6/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.6/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.6/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-21 12:49:58.363703 pyspk-1.6/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.6/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.361849 pyspk-1.6/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/__init__.py
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.363451 pyspk-1.6/pyspk/__pycache__/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/fit_vals.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    14959 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16579 2023-06-21 11:54:52.000000 pyspk-1.6/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.362954 pyspk-1.6/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      411 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-21 12:49:58.363903 pyspk-1.6/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-21 12:46:36.000000 pyspk-1.6/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.540349 pyspk-1.7/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.7/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.7/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9142 2023-06-23 09:52:03.540180 pyspk-1.7/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     8621 2023-06-23 09:38:54.000000 pyspk-1.7/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.538313 pyspk-1.7/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/__init__.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.539961 pyspk-1.7/pyspk/__pycache__/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/fit_vals.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    14959 2023-06-21 11:12:32.000000 pyspk-1.7/pyspk/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    16374 2023-06-23 09:38:28.000000 pyspk-1.7/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.7/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-23 09:52:03.539411 pyspk-1.7/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9142 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      411 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-23 09:52:03.000000 pyspk-1.7/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-23 09:52:03.540384 pyspk-1.7/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-23 09:39:01.000000 pyspk-1.7/setup.py
```

### Comparing `pyspk-1.6/LICENSE.md` & `pyspk-1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/PKG-INFO` & `pyspk-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.6
+Version: 1.7
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
-$$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+$$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
 Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
```

### Comparing `pyspk-1.6/README.md` & `pyspk-1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
-$$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+$$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
 Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
```

### Comparing `pyspk-1.6/pyspk/__pycache__/fit_vals.cpython-38.pyc` & `pyspk-1.7/pyspk/__pycache__/fit_vals.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/pyspk/__pycache__/model.cpython-38.pyc` & `pyspk-1.7/pyspk/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/pyspk/fit_vals.py` & `pyspk-1.7/pyspk/fit_vals.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/pyspk/model.py` & `pyspk-1.7/pyspk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,20 +257,19 @@
         
     Returns
     -------
     output: array of float
         baryon fraction normalised by the Universal baryon fraction: f_b / (Omega_b / Omega_m)
     """
 
-    A = 0.1658 / (cosmo.Ob0 / cosmo.Om0)
-    B = _np.exp(alpha) / 100
-    C = _np.power(m_halo / 1e14, beta - 1)
-    D = _np.power(cosmo.efunc(z) / cosmo.efunc(0.3), gamma)
+    A = _np.exp(alpha) / 100
+    B = _np.power(m_halo / 1e14, beta - 1)
+    C = _np.power(cosmo.efunc(z) / cosmo.efunc(0.3), gamma)
 
-    return A * B * C * D
+    return A * B * C
 
 
 def sup_model(SO, z, fb_a=None, fb_pow=None, fb_pivot=1, M_halo=None, fb=None, extrapolate=False,
               alpha=None, beta=None, gamma=None, cosmo=None, k_array=None, k_min=0.1, k_max=8, n=100, 
               errors=False, verbose=False):
     """
     Returns the suppression of the total matter power spectrum as a function of scale 'k' using the SP(k) model.
@@ -352,19 +351,14 @@
         raise Exception('\033[91mpy-spk was calibrated up to z = 3.0. '
                         'Please specify z <= 3.0 \033[0m') from None
 
     if z < 0.125:
         _warnings.warn('\033[33mpy-spk was calibrated down to z = 0.125. Redshifts '
                        'z < 0.125 may not be accurately reproduced by the model. \033[0m', stacklevel=2)
 
-    if cosmo is not None:
-        if not cosmo.Ob0:
-            raise Exception('\033[91mIncorrect cosmology. Please specify Omega_baryon.\033[0m') from None
-
-
     if k_array is not None:
         k_max = k_array.max()
         k_min = k_array.min()
         k = k_array
 
     else:
         k = _np.round(_np.logspace(_np.log10(k_min), _np.log10(k_max), n), 6)
```

### Comparing `pyspk-1.6/pyspk/stat_errors_200.csv` & `pyspk-1.7/pyspk/stat_errors_200.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/pyspk/stat_errors_500.csv` & `pyspk-1.7/pyspk/stat_errors_500.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.6/pyspk.egg-info/PKG-INFO` & `pyspk-1.7/pyspk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.6
+Version: 1.7
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
 For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
 We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
-$$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
+$$f_b/(\Omega_b/\Omega_m)= \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
 Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
```

### Comparing `pyspk-1.6/setup.py` & `pyspk-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.6,
+    version=1.7,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

