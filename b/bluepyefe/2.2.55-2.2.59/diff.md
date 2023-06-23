# Comparing `tmp/bluepyefe-2.2.55.tar.gz` & `tmp/bluepyefe-2.2.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.55.tar", last modified: Thu Jun 22 08:40:16 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.59.tar", last modified: Fri Jun 23 07:30:02 2023, max compression
```

## Comparing `bluepyefe-2.2.55.tar` & `bluepyefe-2.2.59.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/nwbreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.867447 bluepyefe-2.2.55/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-22 08:40:16.000000 bluepyefe-2.2.55/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 08:40:16.000000 bluepyefe-2.2.55/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:40:16.000000 bluepyefe-2.2.55/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 08:40:16.000000 bluepyefe-2.2.55/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 08:40:16.000000 bluepyefe-2.2.55/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 08:40:16.871447 bluepyefe-2.2.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-06-22 08:40:13.000000 bluepyefe-2.2.55/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/nwbreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.256283 bluepyefe-2.2.59/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 07:30:02.000000 bluepyefe-2.2.59/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-23 07:30:02.000000 bluepyefe-2.2.59/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:30:02.000000 bluepyefe-2.2.59/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 07:30:02.000000 bluepyefe-2.2.59/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 07:30:02.000000 bluepyefe-2.2.59/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 07:30:02.260283 bluepyefe-2.2.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-06-23 07:29:59.000000 bluepyefe-2.2.59/versioneer.py
```

### Comparing `bluepyefe-2.2.55/LICENSE.txt` & `bluepyefe-2.2.59/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/PKG-INFO` & `bluepyefe-2.2.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.55
+Version: 2.2.59
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.55/README.md` & `bluepyefe-2.2.59/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,138 +1,140 @@
-<img src="docs/source/logo/BluePyEfeBanner.jpg"/>
+|banner|
 
 -----------------
 
-# BluePyEfe: Blue Brain Python E-feature extraction
+BluePyEfe: Blue Brain Python E-feature extraction
+=================================================
 
-<table>
-<tr>
-  <td>Latest Release</td>
-  <td>
-    <a href="https://pypi.org/project/bluepyefe/">
-    <img src="https://img.shields.io/pypi/v/bluepyefe.svg" alt="latest release" />
-    </a>
-  </td>
-</tr>
-<tr>
-  <td>Documentation</td>
-  <td>
-    <a href="https://bluepyefe.readthedocs.io/">
-    <img src="https://readthedocs.org/projects/bluepyefe/badge/?version=latest" alt="latest documentation" />
-    </a>
-  </td>
-</tr>
-<tr>
-  <td>License</td>
-  <td>
-    <a href="https://github.com/BlueBrain/bluepyefe/blob/master/LICENSE.txt">
-    <img src="https://img.shields.io/pypi/l/bluepyefe.svg" alt="license" />
-    </a>
-</td>
-</tr>
-<tr>
-  <td>Build Status</td>
-  <td>
-   <a href="https://github.com/BlueBrain/BluePyEfe/actions">
-    <img src="https://github.com/BlueBrain/BluePyEfe/workflows/Build/badge.svg?branch=master" alt="Actions build status" />
-    </a>
-  </td>
-</tr>
-<tr>
-<tr>
-  <td>DOI</td>
-  <td>
-    <a href="https://zenodo.org/badge/latestdoi/237923583">
-    	<img src="https://zenodo.org/badge/237923583.svg" alt="DOI"/>
-    </a>
-  </td>
-</tr>
-<tr>
-	<td>Gitter</td>
-	<td>
-		<a href="https://gitter.im/bluebrain/bluepyefe">
-		<img src="https://badges.gitter.im/Join%20Chat.svg">
-	</a>
-	</td>
-</tr>
-<tr>
-  <td>Coverage</td>
-	  <td>
-	    <a href="https://codecov.io/gh/BlueBrain/BluePyEfe">
-	    <img src="https://codecov.io/github/BlueBrain/BluePyEfe/coverage.svg?branch=master" alt="coverage" />
-	    </a>
-  </td>
-</tr>
-</table>
+.. raw:: html
+
+    <table>
+    <tr>
+      <td>Latest Release</td>
+      <td>
+        <a href="https://pypi.org/project/bluepyefe/">
+        <img src="https://img.shields.io/pypi/v/bluepyefe.svg" alt="latest release" />
+        </a>
+      </td>
+    </tr>
+    <tr>
+      <td>Documentation</td>
+      <td>
+        <a href="https://bluepyefe.readthedocs.io/">
+        <img src="https://readthedocs.org/projects/bluepyefe/badge/?version=latest" alt="latest documentation" />
+        </a>
+      </td>
+    </tr>
+    <tr>
+      <td>License</td>
+      <td>
+        <a href="https://github.com/BlueBrain/bluepyefe/blob/master/LICENSE.txt">
+        <img src="https://img.shields.io/pypi/l/bluepyefe.svg" alt="license" />
+        </a>
+    </td>
+    </tr>
+    <tr>
+      <td>Build Status</td>
+      <td>
+      <a href="https://github.com/BlueBrain/BluePyEfe/actions">
+        <img src="https://github.com/BlueBrain/BluePyEfe/workflows/Build/badge.svg?branch=master" alt="Actions build status" />
+        </a>
+      </td>
+    </tr>
+    <tr>
+    <tr>
+      <td>DOI</td>
+      <td>
+        <a href="https://zenodo.org/badge/latestdoi/237923583">
+          <img src="https://zenodo.org/badge/237923583.svg" alt="DOI"/>
+        </a>
+      </td>
+    </tr>
+    <tr>
+      <td>Gitter</td>
+      <td>
+        <a href="https://gitter.im/bluebrain/bluepyefe">
+        <img src="https://badges.gitter.im/Join%20Chat.svg">
+      </a>
+      </td>
+    </tr>
+    <tr>
+      <td>Coverage</td>
+        <td>
+          <a href="https://codecov.io/gh/BlueBrain/BluePyEfe">
+          <img src="https://codecov.io/github/BlueBrain/BluePyEfe/coverage.svg?branch=master" alt="coverage" />
+          </a>
+      </td>
+    </tr>
+    </table>
 
 Introduction
 ============
 
 BluePyEfe aims at easing the process of reading experimental recordings and extracting 
-batches of electrical features from these recordings. To do so, it combines
- trace reading
-functions and features extraction functions from the [eFel library](https://github.com/BlueBrain/eFEL).
+batches of electrical features from these recordings. To do so, it combines trace reading
+functions and features extraction functions from the `eFel library <https://github.com/BlueBrain/eFEL>`_.
 
 BluePyEfe outputs protocols and features files in the format used
-by [BluePyOpt](https://github.com/BlueBrain/BluePyOpt) for neuron electrical
- model building.
+by `BluePyOpt <https://github.com/BlueBrain/BluePyOpt>`_ for neuron electrical model building.
 
 How to cite
 ===========
-This software is citable using a [DOI generated by Zenodo](https://zenodo.org/record/3728192).
+This software is citable using a `DOI generated by Zenodo <https://zenodo.org/record/3728192>`_.
 
 Requirements
 ============
 
-* [Python 3.8+](https://www.python.org/downloads/release/python-380/)
-* [eFEL eFeature Extraction Library](https://github.com/BlueBrain/eFEL) (automatically installed by pip)
-* [Numpy](http://www.numpy.org) (automatically installed by pip)
-* [Scipy](https://www.scipy.org/) (automatically installed by pip)
-* [Neo](https://neo.readthedocs.io/en/stable/) (automatically installed by pip)
-* The instruction below are written assuming you have access to a command shell
-on Linux / UNIX / MacOSX / Cygwin
+* `Python 3.8+ <https://www.python.org/downloads/release/python-380/>`_
+* `eFEL eFeature Extraction Library <https://github.com/BlueBrain/eFEL>`_ (automatically installed by pip)
+* `Numpy <http://www.numpy.org>`_ (automatically installed by pip)
+* `Scipy <https://www.scipy.org/>`_ (automatically installed by pip)
+* `Neo <https://neo.readthedocs.io/en/stable/>`_ (automatically installed by pip)
+* The instruction below are written assuming you have access to a command shell on Linux / UNIX / MacOSX / Cygwin
 
 Installation
 ============
 
-To install BluePyEfe run:
+To install BluePyEfe, run:
+
+.. code-block:: bash
+
+    pip install bluepyefe
 
-```bash
-pip install bluepyefe
-```
 
 Quick Start and Operating Principle
 ===========
 
-For a hands-on introduction to BluePyEfe, have a look at the notebook [examples/example_of_extraction.ipynb](examples/example_of_extraction.ipynb)
+For a hands-on introduction to BluePyEfe, have a look at the notebook `examples/example_of_extraction.ipynb <examples/example_of_extraction.ipynb>`_
 
 The goal of the present package is to extract meaningful electrophysiological features (e-features) from voltage time series.
-The e-features considered in the present package are the one implemented in the [eFEL python library](https://github.com/BlueBrain/eFEL). See [this pdf](https://bluebrain.github.io/eFEL/efeature-documentation.pdf) for a list of available e-features.
+The e-features considered in the present package are the one implemented in the `eFEL python library <https://github.com/BlueBrain/eFEL>`_. See `this pdf <https://bluebrain.github.io/eFEL/efeature-documentation.pdf>`_ for a list of available e-features.
 
 The present package makes one major assumption: E-features are more meaningful if they are coming from a set of traces rather than a single trace. And they are even more meaningful if these traces come from different cells of the same cellular type.
 This assumption dictates the organisation of the package and has several consequences:
 
 The efeatures extracted through the package will always be averaged over the trace considered. For example, the AP_amplitude will be an average over all the action potentials present in a trace. If you wish to work on an AP by AP basis, please consider using the eFEL library directly. 
 
 A large part of the present software is therefore dedicated to averaging the features across set of "equivalent" recordings. To be able to average e-features across different cells in a meaningful way, an equivalence must be established between the traces coming from these different cells. It would not make sense to average the mean firing frequency obtain cell A on a 1s long step protocol with the one obtain for cell B on a ramp protocol that lasts for 500ms. We chose to define recordings as equivalent based on two criteria: (1) They have the same name and (2) they are of the same amplitude when the amplitude is expressed as a percentage of the rheobase of the cell.
 
 A pseudo-code for the main function of the package (bluepyefe.extract.extract_efeatures) could look as follows:
-```
-1. Load the data to memory by reading all the files containing the traces
-2. Extract the required e-features for all the traces
-3. Compute the rheobases of the cells based on one or several protocols
-4. Use these rheobases to associate to each protocol an amplitude expressed in % of the rheobase
-5. Compute the mean and standard deviations for the e-features across traces having the same amplitude
-6. Save the results and plot the traces and e-features
-```
+
+#. Load the data to memory by reading all the files containing the traces
+#. Extract the required e-features for all the traces
+#. Compute the rheobases of the cells based on one or several protocols
+#. Use these rheobases to associate to each protocol an amplitude expressed in % of the rheobase
+#. Compute the mean and standard deviations for the e-features across traces having the same amplitude
+#. Save the results and plot the traces and e-features
+
 Each of these steps are parametrized by a number of settings, therefore we recommend that you read carefully the docstring of the function.
 
 Coming from the legacy version
 ===============================
 The legacy version (v0.4*) is moved to the legacy branch.
-Changes introduced in v2.0.0 are listed in the [CHANGELOG.rst](CHANGELOG.rst). 
+Changes introduced in v2.0.0 are listed in the `CHANGELOG.rst <CHANGELOG.rst>`_. 
 That is the only file you need to look at for the changes as the future changes will also be noted there.
 
 Funding
 =======
 This work has been partially funded by the European Union Seventh Framework Program (FP7/2007­2013) under grant agreement no. 604102 (HBP), and by the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreements No. 720270 (Human Brain Project SGA1) and No. 785907 (Human Brain Project SGA2) and by the EBRAINS research infrastructure, funded from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
 
+.. |banner| image:: docs/source/logo/BluePyEfeBanner.jpg
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-[docs/source/logo/BluePyEfeBanner.jpg] ----------------- # BluePyEfe: Blue
-Brain Python E-feature extraction
+|banner| ----------------- BluePyEfe: Blue Brain Python E-feature extraction
+================================================= .. raw:: html
 Latest Release [latest_release]
 Documentation  [latest_documentation]
 License        [license]
 Build Status   [Actions_build_status]
 DOI            [DOI]
 Gitter         [https://badges.gitter.im/Join%20Chat.svg]
 Coverage       [coverage]
 Introduction ============ BluePyEfe aims at easing the process of reading
 experimental recordings and extracting batches of electrical features from
 these recordings. To do so, it combines trace reading functions and features
-extraction functions from the [eFel library](https://github.com/BlueBrain/
-eFEL). BluePyEfe outputs protocols and features files in the format used by
-[BluePyOpt](https://github.com/BlueBrain/BluePyOpt) for neuron electrical model
-building. How to cite =========== This software is citable using a [DOI
-generated by Zenodo](https://zenodo.org/record/3728192). Requirements
-============ * [Python 3.8+](https://www.python.org/downloads/release/python-
-380/) * [eFEL eFeature Extraction Library](https://github.com/BlueBrain/eFEL)
-(automatically installed by pip) * [Numpy](http://www.numpy.org) (automatically
-installed by pip) * [Scipy](https://www.scipy.org/) (automatically installed by
-pip) * [Neo](https://neo.readthedocs.io/en/stable/) (automatically installed by
-pip) * The instruction below are written assuming you have access to a command
-shell on Linux / UNIX / MacOSX / Cygwin Installation ============ To install
-BluePyEfe run: ```bash pip install bluepyefe ``` Quick Start and Operating
+extraction functions from the `eFel library
+github.com/BlueBrain/eFEL>`_. BluePyEfe outputs protocols and features files in
+the format used by `BluePyOpt
+github.com/BlueBrain/BluePyOpt>`_ for neuron electrical model building. How to
+cite =========== This software is citable using a `DOI generated by Zenodo
+zenodo.org/record/3728192>`_. Requirements ============ * `Python 3.8+
+www.python.org/downloads/release/python-380/>`_ * `eFEL eFeature Extraction
+Library
+github.com/BlueBrain/eFEL>`_ (automatically installed by pip) * `Numpy
+www.numpy.org>`_ (automatically installed by pip) * `Scipy
+www.scipy.org/>`_ (automatically installed by pip) * `Neo
+neo.readthedocs.io/en/stable/>`_ (automatically installed by pip) * The
+instruction below are written assuming you have access to a command shell on
+Linux / UNIX / MacOSX / Cygwin Installation ============ To install BluePyEfe,
+run: .. code-block:: bash pip install bluepyefe Quick Start and Operating
 Principle =========== For a hands-on introduction to BluePyEfe, have a look at
-the notebook [examples/example_of_extraction.ipynb](examples/
-example_of_extraction.ipynb) The goal of the present package is to extract
+the notebook `examples/example_of_extraction.ipynb
+xample_of_extraction.ipynb>`_ The goal of the present package is to extract
 meaningful electrophysiological features (e-features) from voltage time series.
 The e-features considered in the present package are the one implemented in the
-[eFEL python library](https://github.com/BlueBrain/eFEL). See [this pdf](https:
-//bluebrain.github.io/eFEL/efeature-documentation.pdf) for a list of available
+`eFEL python library
+github.com/BlueBrain/eFEL>`_. See `this pdf
+bluebrain.github.io/eFEL/efeature-documentation.pdf>`_ for a list of available
 e-features. The present package makes one major assumption: E-features are more
 meaningful if they are coming from a set of traces rather than a single trace.
 And they are even more meaningful if these traces come from different cells of
 the same cellular type. This assumption dictates the organisation of the
 package and has several consequences: The efeatures extracted through the
 package will always be averaged over the trace considered. For example, the
 AP_amplitude will be an average over all the action potentials present in a
@@ -44,27 +47,28 @@
 must be established between the traces coming from these different cells. It
 would not make sense to average the mean firing frequency obtain cell A on a 1s
 long step protocol with the one obtain for cell B on a ramp protocol that lasts
 for 500ms. We chose to define recordings as equivalent based on two criteria:
 (1) They have the same name and (2) they are of the same amplitude when the
 amplitude is expressed as a percentage of the rheobase of the cell. A pseudo-
 code for the main function of the package (bluepyefe.extract.extract_efeatures)
-could look as follows: ``` 1. Load the data to memory by reading all the files
-containing the traces 2. Extract the required e-features for all the traces 3.
-Compute the rheobases of the cells based on one or several protocols 4. Use
+could look as follows: #. Load the data to memory by reading all the files
+containing the traces #. Extract the required e-features for all the traces #.
+Compute the rheobases of the cells based on one or several protocols #. Use
 these rheobases to associate to each protocol an amplitude expressed in % of
-the rheobase 5. Compute the mean and standard deviations for the e-features
-across traces having the same amplitude 6. Save the results and plot the traces
-and e-features ``` Each of these steps are parametrized by a number of
-settings, therefore we recommend that you read carefully the docstring of the
-function. Coming from the legacy version =============================== The
-legacy version (v0.4*) is moved to the legacy branch. Changes introduced in
-v2.0.0 are listed in the [CHANGELOG.rst](CHANGELOG.rst). That is the only file
-you need to look at for the changes as the future changes will also be noted
-there. Funding ======= This work has been partially funded by the European
-Union Seventh Framework Program (FP7/2007Â­2013) under grant agreement no.
-604102 (HBP), and by the European Unionâs Horizon 2020 Framework Programme
-for Research and Innovation under the Specific Grant Agreements No. 720270
-(Human Brain Project SGA1) and No. 785907 (Human Brain Project SGA2) and by the
-EBRAINS research infrastructure, funded from the European Unionâs Horizon
-2020 Framework Programme for Research and Innovation under the Specific Grant
-Agreement No. 945539 (Human Brain Project SGA3).
+the rheobase #. Compute the mean and standard deviations for the e-features
+across traces having the same amplitude #. Save the results and plot the traces
+and e-features Each of these steps are parametrized by a number of settings,
+therefore we recommend that you read carefully the docstring of the function.
+Coming from the legacy version =============================== The legacy
+version (v0.4*) is moved to the legacy branch. Changes introduced in v2.0.0 are
+listed in the `CHANGELOG.rst
+rst>`_. That is the only file you need to look at for the changes as the future
+changes will also be noted there. Funding ======= This work has been partially
+funded by the European Union Seventh Framework Program (FP7/2007Â­2013) under
+grant agreement no. 604102 (HBP), and by the European Unionâs Horizon 2020
+Framework Programme for Research and Innovation under the Specific Grant
+Agreements No. 720270 (Human Brain Project SGA1) and No. 785907 (Human Brain
+Project SGA2) and by the EBRAINS research infrastructure, funded from the
+European Unionâs Horizon 2020 Framework Programme for Research and Innovation
+under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3). ..
+|banner| image:: docs/source/logo/BluePyEfeBanner.jpg
```

### Comparing `bluepyefe-2.2.55/bluepyefe/__init__.py` & `bluepyefe-2.2.59/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/auto_targets.py` & `bluepyefe-2.2.59/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/cell.py` & `bluepyefe-2.2.59/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.59/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.59/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.59/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.59/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.59/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.59/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.59/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.59/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.59/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/step.py` & `bluepyefe-2.2.59/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.59/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/extract.py` & `bluepyefe-2.2.59/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.59/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/nwbreader.py` & `bluepyefe-2.2.59/bluepyefe/nwbreader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/plotting.py` & `bluepyefe-2.2.59/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/protocol.py` & `bluepyefe-2.2.59/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/reader.py` & `bluepyefe-2.2.59/bluepyefe/reader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/recording.py` & `bluepyefe-2.2.59/bluepyefe/recording.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/rheobase.py` & `bluepyefe-2.2.59/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/target.py` & `bluepyefe-2.2.59/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/tools.py` & `bluepyefe-2.2.59/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.59/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.59/bluepyefe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.55
+Version: 2.2.59
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.55/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.59/bluepyefe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AUTHORS.txt
 LICENSE.txt
 MANIFEST.in
-README.md
+README.rst
 setup.cfg
 setup.py
 versioneer.py
 bluepyefe/__init__.py
 bluepyefe/_version.py
 bluepyefe/auto_targets.py
 bluepyefe/cell.py
```

### Comparing `bluepyefe-2.2.55/examples/__init__.py` & `bluepyefe-2.2.59/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/setup.py` & `bluepyefe-2.2.59/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.55/versioneer.py` & `bluepyefe-2.2.59/versioneer.py`

 * *Files identical despite different names*

