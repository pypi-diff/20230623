# Comparing `tmp/bluepyefe-2.2.61.tar.gz` & `tmp/bluepyefe-2.2.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.61.tar", last modified: Fri Jun 23 14:13:10 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.63.tar", last modified: Fri Jun 23 14:38:48 2023, max compression
```

## Comparing `bluepyefe-2.2.61.tar` & `bluepyefe-2.2.63.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/nwbreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.854638 bluepyefe-2.2.61/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 14:13:10.000000 bluepyefe-2.2.61/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-23 14:13:10.000000 bluepyefe-2.2.61/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:13:10.000000 bluepyefe-2.2.61/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 14:13:10.000000 bluepyefe-2.2.61/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 14:13:10.000000 bluepyefe-2.2.61/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 14:13:10.858638 bluepyefe-2.2.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-06-23 14:13:06.000000 bluepyefe-2.2.61/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/nwbreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 14:38:48.000000 bluepyefe-2.2.63/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-23 14:38:48.000000 bluepyefe-2.2.63/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:38:48.000000 bluepyefe-2.2.63/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 14:38:48.000000 bluepyefe-2.2.63/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 14:38:48.000000 bluepyefe-2.2.63/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 14:38:48.847961 bluepyefe-2.2.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-06-23 14:38:41.000000 bluepyefe-2.2.63/versioneer.py
```

### Comparing `bluepyefe-2.2.61/LICENSE.txt` & `bluepyefe-2.2.63/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/PKG-INFO` & `bluepyefe-2.2.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.61
+Version: 2.2.63
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.61/README.rst` & `bluepyefe-2.2.63/README.rst`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/__init__.py` & `bluepyefe-2.2.63/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/auto_targets.py` & `bluepyefe-2.2.63/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/cell.py` & `bluepyefe-2.2.63/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.63/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.63/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.63/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.63/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.63/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.63/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.63/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.63/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.63/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/step.py` & `bluepyefe-2.2.63/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.63/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/extract.py` & `bluepyefe-2.2.63/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.63/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/nwbreader.py` & `bluepyefe-2.2.63/bluepyefe/nwbreader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/plotting.py` & `bluepyefe-2.2.63/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/protocol.py` & `bluepyefe-2.2.63/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/reader.py` & `bluepyefe-2.2.63/bluepyefe/reader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/recording.py` & `bluepyefe-2.2.63/bluepyefe/recording.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/rheobase.py` & `bluepyefe-2.2.63/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/target.py` & `bluepyefe-2.2.63/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/tools.py` & `bluepyefe-2.2.63/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.63/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.63/bluepyefe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.61
+Version: 2.2.63
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.61/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.63/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/examples/__init__.py` & `bluepyefe-2.2.63/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/setup.py` & `bluepyefe-2.2.63/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.61/versioneer.py` & `bluepyefe-2.2.63/versioneer.py`

 * *Files identical despite different names*

