# Comparing `tmp/eagerx_tutorials-0.1.8.tar.gz` & `tmp/eagerx_tutorials-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagerx_tutorials-0.1.8.tar", max compression
+gzip compressed data, was "eagerx_tutorials-0.1.9.tar", max compression
```

## Comparing `eagerx_tutorials-0.1.8.tar` & `eagerx_tutorials-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/LICENSE
--rw-r--r--   0        0        0       22 2022-05-03 06:56:04.913635 eagerx_tutorials-0.1.8/eagerx_tutorials/__init__.py
--rw-r--r--   0        0        0     1668 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/helper.py
--rw-r--r--   0        0        0      105 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/__init__.py
--rw-r--r--   0        0        0     1562 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/engine_nodes.py
--rw-r--r--   0        0        0     7404 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/objects.py
--rw-r--r--   0        0        0      337 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/pendulum_ode.py
--rw-r--r--   0        0        0     2207 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/pendulum_render.py
--rw-r--r--   0        0        0     1079 2022-05-03 06:56:04.913635 eagerx_tutorials-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      157 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/scripts/run_tests.sh
--rwxr-xr-x   0        0        0     2750 2022-05-03 06:55:55.129517 eagerx_tutorials-0.1.8/scripts/setup_colab.sh
--rw-r--r--   0        0        0      826 2022-05-03 06:56:11.286327 eagerx_tutorials-0.1.8/setup.py
--rw-r--r--   0        0        0      915 2022-05-03 06:56:11.286595 eagerx_tutorials-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/LICENSE
+-rw-r--r--   0        0        0       22 2022-05-03 15:42:47.683698 eagerx_tutorials-0.1.9/eagerx_tutorials/__init__.py
+-rw-r--r--   0        0        0     1668 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/helper.py
+-rw-r--r--   0        0        0      158 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/__init__.py
+-rw-r--r--   0        0        0     1154 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/converters.py
+-rw-r--r--   0        0        0     1562 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/engine_nodes.py
+-rw-r--r--   0        0        0     7404 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/objects.py
+-rw-r--r--   0        0        0      337 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/pendulum_ode.py
+-rw-r--r--   0        0        0     1235 2022-05-03 15:42:36.403869 eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/pendulum_render.py
+-rw-r--r--   0        0        0     1079 2022-05-03 15:42:47.683698 eagerx_tutorials-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2022-05-03 15:42:36.407869 eagerx_tutorials-0.1.9/scripts/run_tests.sh
+-rwxr-xr-x   0        0        0     2750 2022-05-03 15:42:36.407869 eagerx_tutorials-0.1.9/scripts/setup_colab.sh
+-rw-r--r--   0        0        0      826 2022-05-03 15:42:53.963291 eagerx_tutorials-0.1.9/setup.py
+-rw-r--r--   0        0        0      915 2022-05-03 15:42:53.963580 eagerx_tutorials-0.1.9/PKG-INFO
```

### Comparing `eagerx_tutorials-0.1.8/LICENSE` & `eagerx_tutorials-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eagerx_tutorials-0.1.8/eagerx_tutorials/helper.py` & `eagerx_tutorials-0.1.9/eagerx_tutorials/helper.py`

 * *Files identical despite different names*

### Comparing `eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/engine_nodes.py` & `eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/engine_nodes.py`

 * *Files identical despite different names*

### Comparing `eagerx_tutorials-0.1.8/eagerx_tutorials/pendulum/objects.py` & `eagerx_tutorials-0.1.9/eagerx_tutorials/pendulum/objects.py`

 * *Files identical despite different names*

### Comparing `eagerx_tutorials-0.1.8/pyproject.toml` & `eagerx_tutorials-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eagerx_tutorials"
-version = "0.1.8"
+version = "0.1.9"
 license = "Apache2.0"
 description = "Tutorials on how to use EAGERx."
 authors = ["Jelle Luijkx <j.d.luijkx@tudelft.nl>", "Bas van der Heijden <d.s.vanderheijden@tudelft.nl>"]
 homepage = "https://github.com/eager-dev/eagerx_tutorials"
 repository = "https://github.com/eager-dev/eagerx_tutorials"
 documentation = "https://eagerx.readthedocs.io/en/master/"
 include = ["scripts"]
```

### Comparing `eagerx_tutorials-0.1.8/scripts/setup_colab.sh` & `eagerx_tutorials-0.1.9/scripts/setup_colab.sh`

 * *Files identical despite different names*

### Comparing `eagerx_tutorials-0.1.8/setup.py` & `eagerx_tutorials-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'eagerx>=0.1.18,<0.2.0',
  'jupyterlab>=3.3.4,<4.0.0',
  'nbconvert>=6.5.0,<7.0.0',
  'stable-baselines3>=1.2,<2.0']
 
 setup_kwargs = {
     'name': 'eagerx-tutorials',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Tutorials on how to use EAGERx.',
     'long_description': None,
     'author': 'Jelle Luijkx',
     'author_email': 'j.d.luijkx@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/eager-dev/eagerx_tutorials',
```

### Comparing `eagerx_tutorials-0.1.8/PKG-INFO` & `eagerx_tutorials-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eagerx-tutorials
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tutorials on how to use EAGERx.
 Home-page: https://github.com/eager-dev/eagerx_tutorials
 License: Apache2.0
 Author: Jelle Luijkx
 Author-email: j.d.luijkx@tudelft.nl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

