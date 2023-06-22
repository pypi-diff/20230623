# Comparing `tmp/spyx-0.0.4.tar.gz` & `tmp/spyx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.4.tar", last modified: Thu Jun 22 22:48:10 2023, max compression
+gzip compressed data, was "spyx-0.0.5.tar", last modified: Thu Jun 22 22:56:57 2023, max compression
```

## Comparing `spyx-0.0.4.tar` & `spyx-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:48:10.420294 spyx-0.0.4/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.4/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:48:10.420294 spyx-0.0.4/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.4/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-22 22:48:10.420294 spyx-0.0.4/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-22 22:47:25.000000 spyx-0.0.4/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:48:10.420294 spyx-0.0.4/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.4/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-21 21:10:32.000000 spyx-0.0.4/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8521 2023-06-22 19:23:00.000000 spyx-0.0.4/spyx/activation.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    12312 2023-06-22 22:46:01.000000 spyx-0.0.4/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2663 2023-06-22 06:44:31.000000 spyx-0.0.4/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     6673 2023-06-22 11:37:32.000000 spyx-0.0.4/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:48:10.420294 spyx-0.0.4/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:48:10.000000 spyx-0.0.4/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-22 22:48:10.000000 spyx-0.0.4/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-22 22:48:10.000000 spyx-0.0.4/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-22 22:48:10.000000 spyx-0.0.4/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-22 22:48:10.000000 spyx-0.0.4/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:48:10.420294 spyx-0.0.4/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.4/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.5/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:56:57.470841 spyx-0.0.5/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.5/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-22 22:56:57.470841 spyx-0.0.5/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-22 22:55:57.000000 spyx-0.0.5/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.5/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-21 21:10:32.000000 spyx-0.0.5/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8521 2023-06-22 19:23:00.000000 spyx-0.0.5/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.5/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2663 2023-06-22 06:44:31.000000 spyx-0.0.5/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     6673 2023-06-22 11:37:32.000000 spyx-0.0.5/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.5/tests/test_networks.py
```

### Comparing `spyx-0.0.4/LICENSE` & `spyx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.4/PKG-INFO` & `spyx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spyx-0.0.4/README.md` & `spyx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spyx-0.0.4/setup.py` & `spyx-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.4",
+    version="0.0.5",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `spyx-0.0.4/spyx/activation.py` & `spyx-0.0.5/spyx/activation.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.4/spyx/data.py` & `spyx-0.0.5/spyx/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             SHD2Raster(net_channels, sample_T = sample_T)
         ])
         
         self.train_val_dataset = datasets.SHD("./data", train=True, transform=transform)
         test_dataset = datasets.SHD("./data", train=False, transform=transform)
         
         logo = LeaveOneGroupOut()
-        self.logo = logo.split([*range(len(self.train_val_dataset))], groups=self.train_val_dataset.speaker)
+        self.logo = cycle(logo.split([*range(len(self.train_val_dataset))], groups=self.train_val_dataset.speaker))
         train_indices, val_indices = next(self.logo)
         
         
         train_split = Subset(self.train_val_dataset, train_indices)
         self.train_len = len(train_indices)
         
         val_split = Subset(self.train_val_dataset, val_indices)
```

### Comparing `spyx-0.0.4/spyx/loss.py` & `spyx-0.0.5/spyx/loss.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.4/spyx/nn.py` & `spyx-0.0.5/spyx/nn.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.4/spyx.egg-info/PKG-INFO` & `spyx-0.0.5/spyx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

