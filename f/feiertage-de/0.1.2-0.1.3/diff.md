# Comparing `tmp/feiertage-de-0.1.2.tar.gz` & `tmp/feiertage-de-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiertage-de-0.1.2.tar", last modified: Thu Jun 22 23:21:09 2023, max compression
+gzip compressed data, was "feiertage-de-0.1.3.tar", last modified: Fri Jun 23 07:39:45 2023, max compression
```

## Comparing `feiertage-de-0.1.2.tar` & `feiertage-de-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.630459 feiertage-de-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/src/feiertage/
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/src/feiertage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/src/feiertage/easter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/src/feiertage_de.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 07:39:28.000000 feiertage-de-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-23 07:39:28.000000 feiertage-de-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 07:39:28.000000 feiertage-de-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/src/feiertage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-23 07:39:28.000000 feiertage-de-0.1.3/src/feiertage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-23 07:39:28.000000 feiertage-de-0.1.3/src/feiertage/easter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:39:45.442504 feiertage-de-0.1.3/src/feiertage_de.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-23 07:39:45.000000 feiertage-de-0.1.3/src/feiertage_de.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-23 07:39:45.000000 feiertage-de-0.1.3/src/feiertage_de.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:39:45.000000 feiertage-de-0.1.3/src/feiertage_de.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 07:39:45.000000 feiertage-de-0.1.3/src/feiertage_de.egg-info/top_level.txt
```

### Comparing `feiertage-de-0.1.2/LICENSE` & `feiertage-de-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.2/PKG-INFO` & `feiertage-de-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiertage-de
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/python-feiertage
 Project-URL: Repository, https://github.com/MitchiLaser/python-feiertage
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
@@ -49,8 +49,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `Read the Docs <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

### Comparing `feiertage-de-0.1.2/README.rst` & `feiertage-de-0.1.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `Read the Docs <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

### Comparing `feiertage-de-0.1.2/pyproject.toml` & `feiertage-de-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feiertage-de"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = ""
 readme = "README.rst"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `feiertage-de-0.1.2/src/feiertage/__init__.py` & `feiertage-de-0.1.3/src/feiertage/__init__.py`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.2/src/feiertage/easter.py` & `feiertage-de-0.1.3/src/feiertage/easter.py`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.2/src/feiertage_de.egg-info/PKG-INFO` & `feiertage-de-0.1.3/src/feiertage_de.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiertage-de
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/python-feiertage
 Project-URL: Repository, https://github.com/MitchiLaser/python-feiertage
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
@@ -49,8 +49,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `Read the Docs <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

