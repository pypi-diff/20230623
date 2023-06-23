# Comparing `tmp/pulsars-0.0.3.tar.gz` & `tmp/pulsars-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsars-0.0.3.tar", max compression
+gzip compressed data, was "pulsars-0.0.4.tar", max compression
```

## Comparing `pulsars-0.0.3.tar` & `pulsars-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3460 2023-06-23 16:01:03.332171 pulsars-0.0.3/README.md
--rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.3/pulsars/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.3/pulsars/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.3/pulsars/gui/__pycache__/home_page.cpython-310.pyc
--rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.3/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
--rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.3/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
--rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.3/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
--rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.3/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
--rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.3/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
--rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.3/pulsars/gui/__pycache__/show_page.cpython-310.pyc
--rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.3/pulsars/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.3/pulsars/gui/app.py
--rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.3/pulsars/gui/assets/pulsars-logo.png
--rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.3/pulsars/gui/assets/pulsars-white.png
--rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.3/pulsars/gui/assets/pulsars.png
--rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.3/pulsars/gui/assets/sps-geo.png
--rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.3/pulsars/gui/nabla_geo_page.py
--rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.3/pulsars/gui/nabla_home.py
--rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.3/pulsars/gui/nabla_materials.py
--rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.3/pulsars/gui/nabla_results.py
--rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.3/pulsars/gui/nabla_solver.py
--rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.3/pulsars/gui/nabla_style.css
--rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.3/pulsars/gui/pulsarsGUI.sh
--rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.3/pulsars/gui/readtoml.py
--rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.3/pulsars/gui/test.toml
--rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.3/pulsars/gui/test1.py
--rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.3/pulsars/gui/widgets.py
--rw-r--r--   0        0        0      403 2023-06-22 19:47:42.932339 pulsars-0.0.3/pulsars/templates/sps/sps_v0.py
--rw-r--r--   0        0        0      400 2023-06-23 16:34:37.557153 pulsars-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 pulsars-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3462 2023-06-23 16:38:51.814347 pulsars-0.0.4/README.md
+-rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.4/pulsars/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.4/pulsars/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.4/pulsars/gui/__pycache__/home_page.cpython-310.pyc
+-rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
+-rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
+-rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
+-rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
+-rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.4/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
+-rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.4/pulsars/gui/__pycache__/show_page.cpython-310.pyc
+-rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.4/pulsars/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.4/pulsars/gui/app.py
+-rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.4/pulsars/gui/assets/pulsars-logo.png
+-rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.4/pulsars/gui/assets/pulsars-white.png
+-rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.4/pulsars/gui/assets/pulsars.png
+-rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.4/pulsars/gui/assets/sps-geo.png
+-rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.4/pulsars/gui/nabla_geo_page.py
+-rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.4/pulsars/gui/nabla_home.py
+-rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.4/pulsars/gui/nabla_materials.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.4/pulsars/gui/nabla_results.py
+-rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.4/pulsars/gui/nabla_solver.py
+-rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.4/pulsars/gui/nabla_style.css
+-rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.4/pulsars/gui/pulsarsGUI.sh
+-rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.4/pulsars/gui/readtoml.py
+-rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.4/pulsars/gui/test.toml
+-rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.4/pulsars/gui/test1.py
+-rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.4/pulsars/gui/widgets.py
+-rw-r--r--   0        0        0      403 2023-06-22 19:47:42.932339 pulsars-0.0.4/pulsars/templates/sps/sps_v0.py
+-rw-r--r--   0        0        0      400 2023-06-23 16:38:35.889025 pulsars-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 pulsars-0.0.4/PKG-INFO
```

### Comparing `pulsars-0.0.3/README.md` & `pulsars-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <img src="Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
+# <img src="./Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
 **Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system to help researchers, engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) algorithms and/or solve [Partial Differential Equations](https://en.wikipedia.org/wiki/Partial_differential_equation) using the [Finite Element Method (FEM)](https://en.wikipedia.org/wiki/Finite_element_method).
 
 
 **Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [YAML](https://yaml.org/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
```

### Comparing `pulsars-0.0.3/pulsars/.DS_Store` & `pulsars-0.0.4/pulsars/.DS_Store`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/__pycache__/home_page.cpython-310.pyc` & `pulsars-0.0.4/pulsars/gui/__pycache__/home_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc` & `pulsars-0.0.4/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc` & `pulsars-0.0.4/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/__pycache__/widgets.cpython-310.pyc` & `pulsars-0.0.4/pulsars/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/app.py` & `pulsars-0.0.4/pulsars/gui/app.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/assets/pulsars-logo.png` & `pulsars-0.0.4/pulsars/gui/assets/pulsars-logo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/assets/pulsars-white.png` & `pulsars-0.0.4/pulsars/gui/assets/pulsars-white.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/assets/pulsars.png` & `pulsars-0.0.4/pulsars/gui/assets/pulsars.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/assets/sps-geo.png` & `pulsars-0.0.4/pulsars/gui/assets/sps-geo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/nabla_home.py` & `pulsars-0.0.4/pulsars/gui/nabla_home.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/pulsars/gui/widgets.py` & `pulsars-0.0.4/pulsars/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.3/PKG-INFO` & `pulsars-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pulsars
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Practical Machine Learning & Simulation Building System
 License: MIT
 Author: altar31
 Author-email: damien.sicard31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# <img src="Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
+# <img src="./Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
 **Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system to help researchers, engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) algorithms and/or solve [Partial Differential Equations](https://en.wikipedia.org/wiki/Partial_differential_equation) using the [Finite Element Method (FEM)](https://en.wikipedia.org/wiki/Finite_element_method).
 
 
 **Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [YAML](https://yaml.org/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
```

