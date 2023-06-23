# Comparing `tmp/spyx-0.0.6.tar.gz` & `tmp/spyx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.6.tar", last modified: Fri Jun 23 20:13:50 2023, max compression
+gzip compressed data, was "spyx-0.0.7.tar", last modified: Fri Jun 23 20:21:32 2023, max compression
```

## Comparing `spyx-0.0.6.tar` & `spyx-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.6/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:13:50.394219 spyx-0.0.6/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.6/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:13:50.394219 spyx-0.0.6/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-23 20:11:52.000000 spyx-0.0.6/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.6/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.6/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.6/spyx/activation.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.6/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2695 2023-06-23 06:49:08.000000 spyx-0.0.6/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     7303 2023-06-23 19:28:10.000000 spyx-0.0.6/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.6/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.7/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:21:32.839973 spyx-0.0.7/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.7/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:21:32.839973 spyx-0.0.7/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-23 20:20:57.000000 spyx-0.0.7/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.7/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.7/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.7/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.7/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2690 2023-06-23 20:19:39.000000 spyx-0.0.7/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     7303 2023-06-23 19:28:10.000000 spyx-0.0.7/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.7/tests/test_networks.py
```

### Comparing `spyx-0.0.6/LICENSE` & `spyx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.6/PKG-INFO` & `spyx-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spyx-0.0.6/README.md` & `spyx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spyx-0.0.6/setup.py` & `spyx-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.6",
+    version="0.0.7",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `spyx-0.0.6/spyx/activation.py` & `spyx-0.0.7/spyx/activation.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.6/spyx/data.py` & `spyx-0.0.7/spyx/data.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.6/spyx/loss.py` & `spyx-0.0.7/spyx/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,21 @@
 
 @jax.jit
 def regularized_xentropy(traces, targets, avg_spike_counts, time_steps, r):
     """
     Weighted loss of integral crossentropy plus inverse spike rate regularization.
     """
 
-    xe = integral_crossentropy(traces, targets)
+    xe = integral_xentropy(traces, targets)
     reg = SRR_INV(avg_spike_counts, time_steps)
     return xe + r*reg
 
 # needs fixing.
 @jax.jit
-def exweight_integral_crossentropy(spikes, targets):
+def exponential_integral_xentropy(spikes, targets):
     """
     Integral crossentropy with exponential weighting to promote pushing voltage
     deflections and therefore spikes to earlier in the network rollout.
 
     Still under construction.
 
     Adapted from:
```

### Comparing `spyx-0.0.6/spyx/nn.py` & `spyx-0.0.7/spyx/nn.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.6/spyx.egg-info/PKG-INFO` & `spyx-0.0.7/spyx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

