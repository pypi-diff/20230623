# Comparing `tmp/aiida-spirit-0.2.1.tar.gz` & `tmp/aiida-spirit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-spirit-0.2.1.tar", last modified: Mon Jul 18 09:09:14 2022, max compression
+gzip compressed data, was "aiida-spirit-0.2.2.tar", last modified: Fri Jun 23 07:57:43 2023, max compression
```

## Comparing `aiida-spirit-0.2.1.tar` & `aiida-spirit-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/aiida_spirit/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28891 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/calculations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/aiida_spirit/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/data/_formatting_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/data/_type_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     7698 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/data/input_original.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10429 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/aiida_spirit/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/_vfr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/get_from_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7664 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5755 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/aiida_spirit/tools/spirit_script_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/aiida_spirit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-18 09:09:14.000000 aiida-spirit-0.2.1/aiida_spirit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-18 09:09:14.048772 aiida-spirit-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/setup.json
--rwxr-xr-x   0 runner    (1001) docker     (121)      671 2022-07-18 09:08:10.000000 aiida-spirit-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.249935 aiida-spirit-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-23 07:57:43.249935 aiida-spirit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.241935 aiida-spirit-0.2.2/aiida_spirit/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28891 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.245935 aiida-spirit-0.2.2/aiida_spirit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/data/_formatting_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/data/_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/data/input_original.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.249935 aiida-spirit-0.2.2/aiida_spirit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/_vfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/get_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/aiida_spirit/tools/spirit_script_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.245935 aiida-spirit-0.2.2/aiida_spirit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 07:57:43.000000 aiida-spirit-0.2.2/aiida_spirit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:57:43.249935 aiida-spirit-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/setup.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:43.249935 aiida-spirit-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-23 07:56:38.000000 aiida-spirit-0.2.2/tests/test_calculations.py
```

### Comparing `aiida-spirit-0.2.1/LICENSE` & `aiida-spirit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/PKG-INFO` & `aiida-spirit-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-spirit
-Version: 0.2.1
+Version: 0.2.2
 Summary: AiiDA plugin for the spirit code
 Home-page: https://github.com/JuDFTteam/aiida-spirit
 Author: The JuDFT Team
 Author-email: p.ruessmann@fz-juelich.de
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 [![Build Status](https://github.com/JuDFTteam/aiida-spirit/workflows/ci/badge.svg?branch=master)](https://github.com/JuDFTteam/aiida-spirit/actions)
 [![Coverage Status](https://codecov.io/gh/JuDFTteam/aiida-spirit/branch/main/graph/badge.svg?token=F7ISM4558S)](https://codecov.io/gh/JuDFTteam/aiida-spirit)
 [![Docs status](https://readthedocs.org/projects/aiida-spirit/badge)](http://aiida-spirit.readthedocs.io/)
 [![PyPI version](https://badge.fury.io/py/aiida-spirit.svg)](https://badge.fury.io/py/aiida-spirit)
+[![DOI](https://zenodo.org/badge/364820045.svg)](https://zenodo.org/badge/latestdoi/364820045)
 
 # aiida-spirit
 
 AiiDA plugin for the [spirit code](http://spirit-code.github.io/)
 
 
 ## Installation
@@ -64,14 +65,22 @@
 ```
 # add postgres path for pg_ctl to PATH
 # this is an example for Postgres 9.6 installed on a mac
 PATH="/Applications/Postgres.app/Contents/Versions/9.6/bin/:$PATH"
 export PATH
 ```
 
+## Citation
+
+If you use AiiDA-Spirit please cite the method paper
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel, *The AiiDA-Spirit Plugin for Automated Spin-Dynamics Simulations and Multi-Scale Modeling Based on First-Principles Calculations*, Front. Mater. **9**, 825043 (2022). [doi: 10.3389/fmats.2022.825043](https://doi.org/10.3389/fmats.2022.825043),
+
+ and the latest code release
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel. JuDFTteam/aiida-spirit. Zenodo. [doi: 10.5281/zenodo.8070770](https://doi.org/10.5281/zenodo.8070770).
+
 ## License
 
 The AiiDA-Spirit code is under the [MIT license](LICENSE).
 
 ## Contact
 
 p.ruessmann@fz-juelich.de
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiida-spirit-0.2.1/README.md` & `aiida-spirit-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Build Status](https://github.com/JuDFTteam/aiida-spirit/workflows/ci/badge.svg?branch=master)](https://github.com/JuDFTteam/aiida-spirit/actions)
 [![Coverage Status](https://codecov.io/gh/JuDFTteam/aiida-spirit/branch/main/graph/badge.svg?token=F7ISM4558S)](https://codecov.io/gh/JuDFTteam/aiida-spirit)
 [![Docs status](https://readthedocs.org/projects/aiida-spirit/badge)](http://aiida-spirit.readthedocs.io/)
 [![PyPI version](https://badge.fury.io/py/aiida-spirit.svg)](https://badge.fury.io/py/aiida-spirit)
+[![DOI](https://zenodo.org/badge/364820045.svg)](https://zenodo.org/badge/latestdoi/364820045)
 
 # aiida-spirit
 
 AiiDA plugin for the [spirit code](http://spirit-code.github.io/)
 
 
 ## Installation
@@ -45,14 +46,22 @@
 ```
 # add postgres path for pg_ctl to PATH
 # this is an example for Postgres 9.6 installed on a mac
 PATH="/Applications/Postgres.app/Contents/Versions/9.6/bin/:$PATH"
 export PATH
 ```
 
+## Citation
+
+If you use AiiDA-Spirit please cite the method paper
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel, *The AiiDA-Spirit Plugin for Automated Spin-Dynamics Simulations and Multi-Scale Modeling Based on First-Principles Calculations*, Front. Mater. **9**, 825043 (2022). [doi: 10.3389/fmats.2022.825043](https://doi.org/10.3389/fmats.2022.825043),
+
+ and the latest code release
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel. JuDFTteam/aiida-spirit. Zenodo. [doi: 10.5281/zenodo.8070770](https://doi.org/10.5281/zenodo.8070770).
+
 ## License
 
 The AiiDA-Spirit code is under the [MIT license](LICENSE).
 
 ## Contact
 
 p.ruessmann@fz-juelich.de
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit/calculations.py` & `aiida-spirit-0.2.2/aiida_spirit/calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/cli.py` & `aiida-spirit-0.2.2/aiida_spirit/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/data/_formatting_info.py` & `aiida-spirit-0.2.2/aiida_spirit/data/_formatting_info.py`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/data/_type_check.py` & `aiida-spirit-0.2.2/aiida_spirit/data/_type_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,18 @@
     """Validate array input"""
     # check if type is ok
     try:
         # this raises a TypeError if input is, for example, integer
         _ = len(val)
         # convert to numpy array
         val = np.array(val)
-    except TypeError:
+    except TypeError as error:
         raise TypeError(
-            f'Array input {key} is not an array-like object ({val}).')
+            f'Array input {key} is not an array-like object ({val}).'
+        ) from error
 
     # check shape of the array
     if len(val) < 1:
         raise ValueError(f'Array input {key} has length 0 ({val}).')
     if len_check is not None:
         if len(val) != len_check:
             raise ValueError(
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit/data/input_original.cfg` & `aiida-spirit-0.2.2/aiida_spirit/data/input_original.cfg`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/parsers.py` & `aiida-spirit-0.2.2/aiida_spirit/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Initialize Parser instance
 
         Checks that the ProcessNode being passed was produced by a SpiritCalculation.
 
         :param node: ProcessNode of calculation
         :param type node: :class:`aiida.orm.ProcessNode`
         """
-        super(SpiritParser, self).__init__(node)
+        super(SpiritParser, self).__init__(node)  # pylint: disable=super-with-arguments
         if not issubclass(node.process_class, SpiritCalculation):
             raise exceptions.ParsingError('Can only parse SpiritCalculation')
 
     def parse(self, **kwargs):
         """
         Parse outputs, store results in database.
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit/tools/_vfr.py` & `aiida-spirit-0.2.2/aiida_spirit/tools/_vfr.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Interface to the spirit web view used in the plotting tool.
 """
 
 import json
 import secrets
 import numpy as np
-from IPython.core.display import display, HTML, Javascript
+from IPython.display import display, HTML, Javascript
 
 _vfr_frame_id_mapping = {}
 _next_frame_id = 1
 _frame_id_suffix = secrets.token_hex(32)
 
 # pylint: disable=line-too-long,global-statement
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit/tools/get_from_remote.py` & `aiida-spirit-0.2.2/aiida_spirit/tools/get_from_remote.py`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/tools/helpers.py` & `aiida-spirit-0.2.2/aiida_spirit/tools/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
     :param computer: (local) AiiDA computer
     :return: The code node
     :rtype: :py:class:`aiida.orm.Code`
     """
 
     try:
         executable = executables[entry_point]
-    except KeyError:
+    except KeyError as error:
         raise KeyError(
             "Entry point '{}' not recognized. Allowed values: {}".format(
-                entry_point, list(executables.keys())))
+                entry_point, list(executables.keys()))) from error
 
     codes = Code.objects.find(filters={'label': executable})  # pylint: disable=no-member
     if codes:
         return codes[0]
 
     path = get_path_to_executable(executable)
     code = Code(
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit/tools/plotting.py` & `aiida-spirit-0.2.2/aiida_spirit/tools/plotting.py`

 * *Files identical despite different names*

### Comparing `aiida-spirit-0.2.1/aiida_spirit/tools/spirit_script_builder.py` & `aiida-spirit-0.2.2/aiida_spirit/tools/spirit_script_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         'mc': 'simulation.METHOD_MC'
     }
 
     def method(self, key):
         """Set Spirit run method (i.e. LLG, MC)"""
         try:
             return self._method_dict[key.lower()]
-        except KeyError:
-            raise ValueError('Invalid method!')
+        except KeyError as error:
+            raise ValueError('Invalid method!') from error
 
     _solver_dict = {
         'depondt': 'simulation.SOLVER_DEPONDT',
         'heun': 'simulation.SOLVER_HEUN',
         'sib': 'simulation.SOLVER_SIB',
         'rk4': 'simulation.SOLVER_SIB',
         'vp': 'simulation.SOLVER_VP',
@@ -99,32 +99,32 @@
         'lbfgs_atlas': 'simulation.SOLVER_LBFGS_Atlas'
     }
 
     def solver(self, key):
         """Set spirit solver (Depodt, VP, ...)"""
         try:
             return self._solver_dict[key.lower()]
-        except KeyError:
-            raise ValueError('Invalid solver!')
+        except KeyError as error:
+            raise ValueError('Invalid solver!') from error
 
     _module_dict = {
         'configuration': 'configuration',
         'simulation': 'simulation',
         'geometry': 'geometry',
         'state': 'state',
         'io': 'io'
     }
 
     # Modules
     def module(self, key):
         """Import the spirit modules"""
         try:
             return self._module_dict[key.lower()]
-        except KeyError:
-            raise ValueError('Invalid module!')
+        except KeyError as error:
+            raise ValueError('Invalid module!') from error
 
     @staticmethod
     def _dict_to_arg_string(dict):  # pylint: disable=redefined-builtin
         """Format a dict as a string of keyword arguments"""
         return ''.join(
             [', {} = {}'.format(key, val) for key, val in dict.items()])
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit.egg-info/PKG-INFO` & `aiida-spirit-0.2.2/aiida_spirit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-spirit
-Version: 0.2.1
+Version: 0.2.2
 Summary: AiiDA plugin for the spirit code
 Home-page: https://github.com/JuDFTteam/aiida-spirit
 Author: The JuDFT Team
 Author-email: p.ruessmann@fz-juelich.de
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 [![Build Status](https://github.com/JuDFTteam/aiida-spirit/workflows/ci/badge.svg?branch=master)](https://github.com/JuDFTteam/aiida-spirit/actions)
 [![Coverage Status](https://codecov.io/gh/JuDFTteam/aiida-spirit/branch/main/graph/badge.svg?token=F7ISM4558S)](https://codecov.io/gh/JuDFTteam/aiida-spirit)
 [![Docs status](https://readthedocs.org/projects/aiida-spirit/badge)](http://aiida-spirit.readthedocs.io/)
 [![PyPI version](https://badge.fury.io/py/aiida-spirit.svg)](https://badge.fury.io/py/aiida-spirit)
+[![DOI](https://zenodo.org/badge/364820045.svg)](https://zenodo.org/badge/latestdoi/364820045)
 
 # aiida-spirit
 
 AiiDA plugin for the [spirit code](http://spirit-code.github.io/)
 
 
 ## Installation
@@ -64,14 +65,22 @@
 ```
 # add postgres path for pg_ctl to PATH
 # this is an example for Postgres 9.6 installed on a mac
 PATH="/Applications/Postgres.app/Contents/Versions/9.6/bin/:$PATH"
 export PATH
 ```
 
+## Citation
+
+If you use AiiDA-Spirit please cite the method paper
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel, *The AiiDA-Spirit Plugin for Automated Spin-Dynamics Simulations and Multi-Scale Modeling Based on First-Principles Calculations*, Front. Mater. **9**, 825043 (2022). [doi: 10.3389/fmats.2022.825043](https://doi.org/10.3389/fmats.2022.825043),
+
+ and the latest code release
+ - P. Rüßmann, J. Ribas Sobreviela, M. Sallermann, M. Hoffmann, F. Rhiem, and S. Blügel. JuDFTteam/aiida-spirit. Zenodo. [doi: 10.5281/zenodo.8070770](https://doi.org/10.5281/zenodo.8070770).
+
 ## License
 
 The AiiDA-Spirit code is under the [MIT license](LICENSE).
 
 ## Contact
 
 p.ruessmann@fz-juelich.de
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiida-spirit-0.2.1/aiida_spirit.egg-info/SOURCES.txt` & `aiida-spirit-0.2.2/aiida_spirit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 aiida_spirit/data/_type_check.py
 aiida_spirit/data/input_original.cfg
 aiida_spirit/tools/__init__.py
 aiida_spirit/tools/_vfr.py
 aiida_spirit/tools/get_from_remote.py
 aiida_spirit/tools/helpers.py
 aiida_spirit/tools/plotting.py
-aiida_spirit/tools/spirit_script_builder.py
+aiida_spirit/tools/spirit_script_builder.py
+tests/test_calculations.py
```

### Comparing `aiida-spirit-0.2.1/setup.json` & `aiida-spirit-0.2.2/setup.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9376984126984127%*

 * *Differences: {"'extras_require'": "{'testing': {insert: [(0, 'pgtest>=1.3.1'), (1, 'wheel>=0.31'), (3, "*

 * *                     "'pytest>=3.6')], delete: [3, 1, 0]}, 'pre-commit': {insert: [(1, "*

 * *                     "'pre-commit>=2.2'), (2, 'pylint>=2.5.0')], delete: [2, 1]}}",*

 * * "'install_requires'": "{insert: [(0, 'aiida-core>=1.1.0,<3.0.0')], delete: [1, 0]}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -22,36 +22,35 @@
             "sphinx",
             "sphinxcontrib-contentui",
             "sphinxcontrib-details-directive; python_version>='3.0'",
             "sphinx-rtd-theme"
         ],
         "pre-commit": [
             "astroid<2.5",
-            "pre-commit~=2.2",
-            "pylint~=2.5.0"
+            "pre-commit>=2.2",
+            "pylint>=2.5.0"
         ],
         "testing": [
-            "pgtest~=1.3.1",
-            "wheel~=0.31",
+            "pgtest>=1.3.1",
+            "wheel>=0.31",
             "coverage",
-            "pytest~=3.6,<5.0.0",
+            "pytest>=3.6",
             "pytest-cov",
             "spirit"
         ]
     },
     "include_package_data": true,
     "install_requires": [
-        "aiida-core>=1.1.0,<2.0.0",
-        "sqlalchemy<1.4",
+        "aiida-core>=1.1.0,<3.0.0",
         "numpy",
         "pandas",
         "masci-tools"
     ],
     "license": "MIT",
     "name": "aiida-spirit",
     "reentry_register": true,
     "setup_requires": [
         "reentry"
     ],
     "url": "https://github.com/JuDFTteam/aiida-spirit",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `aiida-spirit-0.2.1/setup.py` & `aiida-spirit-0.2.2/setup.py`

 * *Files identical despite different names*

