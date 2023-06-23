# Comparing `tmp/speech_collator-0.1.8.tar.gz` & `tmp/speech_collator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_collator-0.1.8.tar", last modified: Wed May 24 17:34:41 2023, max compression
+gzip compressed data, was "speech_collator-0.1.9.tar", last modified: Wed May 24 18:37:19 2023, max compression
```

## Comparing `speech_collator-0.1.8.tar` & `speech_collator-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.8/README.md
--rw-r--r--   0        0        0      522 2023-05-24 17:34:41.574020 speech_collator-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    15109 2023-05-14 17:05:41.228749 speech_collator-0.1.8/speech_collator/__init__.py
--rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.8/speech_collator/data/dvector-step250000.pt
--rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.8/speech_collator/data/wav2mel.pt
--rw-r--r--   0        0        0     5190 2023-05-24 17:32:24.473027 speech_collator-0.1.8/speech_collator/measures/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.8/speech_collator/measures/snr.py
--rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.8/speech_collator/measures/srmr.py
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.9/README.md
+-rw-r--r--   0        0        0      522 2023-05-24 18:37:19.756509 speech_collator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    15109 2023-05-14 17:05:41.228749 speech_collator-0.1.9/speech_collator/__init__.py
+-rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.9/speech_collator/data/dvector-step250000.pt
+-rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.9/speech_collator/data/wav2mel.pt
+-rw-r--r--   0        0        0     5252 2023-05-24 17:37:16.916211 speech_collator-0.1.9/speech_collator/measures/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.9/speech_collator/measures/snr.py
+-rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.9/speech_collator/measures/srmr.py
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.9/PKG-INFO
```

### Comparing `speech_collator-0.1.8/pyproject.toml` & `speech_collator-0.1.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "speech-collator"
-version = "0.1.8"
+version = "0.1.9"
 description = "A collator for speech datasets with different batching strategies and attribute extraction."
 authors = [
     { name = "Christoph Minixhofer", email = "christoph.minixhofer@gmail.com" },
 ]
 dependencies = [
     "numpy<1.24",
     "pyworld>=0.3.3",
```

### Comparing `speech_collator-0.1.8/speech_collator/__init__.py` & `speech_collator-0.1.9/speech_collator/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.8/speech_collator/data/dvector-step250000.pt` & `speech_collator-0.1.9/speech_collator/data/dvector-step250000.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.8/speech_collator/data/wav2mel.pt` & `speech_collator-0.1.9/speech_collator/data/wav2mel.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.8/speech_collator/measures/__init__.py` & `speech_collator-0.1.9/speech_collator/measures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .srmr import srmr
 
 class Measure(ABC):
     def __init__(self, name, description, is_binary=False):
         self.name = name
         self.description = description
         self.is_binary = is_binary
+        if self.is_binary:
+            self.name += "_binary"
 
     @staticmethod
     def interpolate(x):
         def nan_helper(y):
             return np.isnan(y), lambda z: z.nonzero()[0]
         nans, y = nan_helper(x)
         x[nans] = np.interp(y(nans), y(~nans), x[~nans])
```

### Comparing `speech_collator-0.1.8/speech_collator/measures/snr.py` & `speech_collator-0.1.9/speech_collator/measures/snr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.8/speech_collator/measures/srmr.py` & `speech_collator-0.1.9/speech_collator/measures/srmr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.8/PKG-INFO` & `speech_collator-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech-collator
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collator for speech datasets with different batching strategies and attribute extraction.
 Author-Email: Christoph Minixhofer <christoph.minixhofer@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: numpy<1.24
 Requires-Dist: pyworld>=0.3.3
 Requires-Dist: librosa<0.10
```

