# Comparing `tmp/feiertage-de-0.1.1.tar.gz` & `tmp/feiertage-de-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiertage-de-0.1.1.tar", last modified: Thu Jun 22 22:42:58 2023, max compression
+gzip compressed data, was "feiertage-de-0.1.2.tar", last modified: Thu Jun 22 23:21:09 2023, max compression
```

## Comparing `feiertage-de-0.1.1.tar` & `feiertage-de-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/feiertage/
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/src/feiertage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/src/feiertage/easter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/feiertage_de.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.630459 feiertage-de-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/src/feiertage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/src/feiertage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-22 23:20:51.000000 feiertage-de-0.1.2/src/feiertage/easter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:21:09.634459 feiertage-de-0.1.2/src/feiertage_de.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 23:21:09.000000 feiertage-de-0.1.2/src/feiertage_de.egg-info/top_level.txt
```

### Comparing `feiertage-de-0.1.1/LICENSE` & `feiertage-de-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.1/PKG-INFO` & `feiertage-de-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiertage-de
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/python-feiertage
 Project-URL: Repository, https://github.com/MitchiLaser/python-feiertage
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 Feiertage
 =========
 
 This python package provides an easy access to the list of German national holidays for each federal state.
 
-::
+.. code-block:: python
 
   >>> import feiertage
   >>> holidays = feiertage.Holidays("BW", year=2023).holidays
   >>> # holidays now contains a list of dictionaries for each holiday with the attribues
   >>> # 'date' -> a datetime.date object with the date of the holiday
   >>> # 'name'-> a string with the name of the holiday
   >>> 
@@ -49,8 +49,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

### Comparing `feiertage-de-0.1.1/README.rst` & `feiertage-de-0.1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Feiertage
 =========
 
 This python package provides an easy access to the list of German national holidays for each federal state.
 
-::
+.. code-block:: python
 
   >>> import feiertage
   >>> holidays = feiertage.Holidays("BW", year=2023).holidays
   >>> # holidays now contains a list of dictionaries for each holiday with the attribues
   >>> # 'date' -> a datetime.date object with the date of the holiday
   >>> # 'name'-> a string with the name of the holiday
   >>> 
@@ -32,8 +32,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

### Comparing `feiertage-de-0.1.1/pyproject.toml` & `feiertage-de-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feiertage-de"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = ""
 readme = "README.rst"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `feiertage-de-0.1.1/src/feiertage/__init__.py` & `feiertage-de-0.1.2/src/feiertage/__init__.py`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.1/src/feiertage/easter.py` & `feiertage-de-0.1.2/src/feiertage/easter.py`

 * *Files identical despite different names*

### Comparing `feiertage-de-0.1.1/src/feiertage_de.egg-info/PKG-INFO` & `feiertage-de-0.1.2/src/feiertage_de.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiertage-de
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Project-URL: Homepage, https://github.com/MitchiLaser/python-feiertage
 Project-URL: Repository, https://github.com/MitchiLaser/python-feiertage
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 Feiertage
 =========
 
 This python package provides an easy access to the list of German national holidays for each federal state.
 
-::
+.. code-block:: python
 
   >>> import feiertage
   >>> holidays = feiertage.Holidays("BW", year=2023).holidays
   >>> # holidays now contains a list of dictionaries for each holiday with the attribues
   >>> # 'date' -> a datetime.date object with the date of the holiday
   >>> # 'name'-> a string with the name of the holiday
   >>> 
@@ -49,8 +49,8 @@
 
 This package can be easily installed with pip:
 
 .. code-block:: bash
 
   $ pip install feiertage-de
 
-Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_
+Further information can be seen at the `PyPi project page <https://pypi.org/project/feiertage-de/>`_ or at `feiertage-de.readthedocs.io <https://feiertage-de.readthedocs.io/en/latest/index.html>`_
```

