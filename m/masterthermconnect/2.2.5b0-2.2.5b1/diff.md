# Comparing `tmp/masterthermconnect-2.2.5b0.tar.gz` & `tmp/masterthermconnect-2.2.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterthermconnect-2.2.5b0.tar", last modified: Wed Jun 14 12:11:26 2023, max compression
+gzip compressed data, was "masterthermconnect-2.2.5b1.tar", last modified: Wed Jun 14 15:08:58 2023, max compression
```

## Comparing `masterthermconnect-2.2.5b0.tar` & `masterthermconnect-2.2.5b1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/masterthermconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15173 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/datamapread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/datamapwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/masterthermconnect/special.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 12:11:26.000000 masterthermconnect-2.2.5b0/masterthermconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:26.777562 masterthermconnect-2.2.5b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_api_new.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_api_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29214 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-14 12:10:46.000000 masterthermconnect-2.2.5b0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:08:58.023452 masterthermconnect-2.2.5b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 15:08:58.023452 masterthermconnect-2.2.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:08:58.019452 masterthermconnect-2.2.5b1/masterthermconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/datamapread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/datamapwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/masterthermconnect/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:08:58.019452 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 15:08:58.000000 masterthermconnect-2.2.5b1/masterthermconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 15:08:58.023452 masterthermconnect-2.2.5b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:08:58.023452 masterthermconnect-2.2.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/tests/test_api_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/tests/test_api_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/tests/test_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-14 15:08:15.000000 masterthermconnect-2.2.5b1/tests/test_main.py
```

### Comparing `masterthermconnect-2.2.5b0/LICENSE` & `masterthermconnect-2.2.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/PKG-INFO` & `masterthermconnect-2.2.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.5b0
+Version: 2.2.5b1
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b0 Summary: Python
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b1 Summary: Python
 3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.5b0/README.md` & `masterthermconnect-2.2.5b1/README.md`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/__init__.py` & `masterthermconnect-2.2.5b1/masterthermconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/__main__.py` & `masterthermconnect-2.2.5b1/masterthermconnect/__main__.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/api.py` & `masterthermconnect-2.2.5b1/masterthermconnect/api.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/const.py` & `masterthermconnect-2.2.5b1/masterthermconnect/const.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/controller.py` & `masterthermconnect-2.2.5b1/masterthermconnect/controller.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/datamapread.py` & `masterthermconnect-2.2.5b1/masterthermconnect/datamapread.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,29 @@
     "circulation_pump_running": [bool, "D_10"],
     "fan_running": [bool, "D_8"],  # Filtered by HP Type
     "brine_pump_running": [bool, "D_8"],  # Filtered by HP Type,
     "defrost_mode": [bool, "D_11"],
     "aux_heater_1": [bool, "D_6"],
     "aux_heater_2": [bool, "D_7"],
     "outside_temp": [float, "A_3"],
-    "requested_temp": [float, "A_5"],
+    "requested_temp_old": [float, "A_5"],
+    "requested_temp": [  # Cooling temp does not show in A_5
+        Special(str, Special.FORMULA),
+        [
+            "{0} if ({2} or {3} or {4} or {5}) else {1}",
+            [
+                [float, "A_5"],  # 0 - Main Requested Temp
+                [float, "A_212"],  # 1 - Heating/Cooling Temp
+                [bool, "D_66"],  # 2 - Hot Water
+                [bool, "D_43"],  # 3 - Pool
+                [bool, "D_6"],  # 4 - Aux Heater 1
+                [bool, "D_7"],  # 5 - Aux Heater 2
+            ],
+        ],
+    ],
     "actual_temp": [float, "A_1"],
     "dewp_control": [bool, "D_196"],
     "high_tariff_control": [
         Special(bool, Special.FORMULA),
         [
             "not {0}",
             [[bool, "D_15"]],
```

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/datamapwrite.py` & `masterthermconnect-2.2.5b1/masterthermconnect/datamapwrite.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/exceptions.py` & `masterthermconnect-2.2.5b1/masterthermconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect/special.py` & `masterthermconnect-2.2.5b1/masterthermconnect/special.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect.egg-info/PKG-INFO` & `masterthermconnect-2.2.5b1/masterthermconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterthermconnect
-Version: 2.2.5b0
+Version: 2.2.5b1
 Summary: Python 3 API wrapper for Mastertherm API
 Author-email: Richard Holmes <richard@shedc.uk>
 License: MIT License
         
         Copyright (c) 2021 shedc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b0 Summary: Python
+Metadata-Version: 2.1 Name: masterthermconnect Version: 2.2.5b1 Summary: Python
 3 API wrapper for Mastertherm API Author-email: Richard Holmes
 shedc.uk> License: MIT License Copyright (c) 2021 shedc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `masterthermconnect-2.2.5b0/masterthermconnect.egg-info/SOURCES.txt` & `masterthermconnect-2.2.5b1/masterthermconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/pyproject.toml` & `masterthermconnect-2.2.5b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masterthermconnect"
-version = "2.2.5b0"
+version = "2.2.5b1"
 description = "Python 3 API wrapper for Mastertherm API"
 readme = "README.md"
 authors = [{ name = "Richard Holmes", email = "richard@shedc.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,15 +24,15 @@
 [project.urls]
 Homepage = "https://github.com/sHedC/python-masterthermconnect"
 
 [project.scripts]
 masterthermconnect = "masterthermconnect.__main__:main"
 
 [tool.bumpver]
-current_version = "2.2.5-b0"
+current_version = "2.2.5-b1"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `masterthermconnect-2.2.5b0/setup.cfg` & `masterthermconnect-2.2.5b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/tests/test_api_new.py` & `masterthermconnect-2.2.5b1/tests/test_api_new.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/tests/test_api_old.py` & `masterthermconnect-2.2.5b1/tests/test_api_old.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/tests/test_config_data.py` & `masterthermconnect-2.2.5b1/tests/test_config_data.py`

 * *Files identical despite different names*

### Comparing `masterthermconnect-2.2.5b0/tests/test_controller.py` & `masterthermconnect-2.2.5b1/tests/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     ):
         assert await controller.connect() is True
         assert await controller.refresh() is True
 
     data = controller.get_device_data("10021", "2")
 
     assert data["operating_mode"] == "cooling"
+    assert data["requested_temp"] == 15.1
 
 
 async def test_operating_mode_heating():
     """Test the Controller Operating Mode."""
     controller = MasterthermController(
         VALID_LOGIN["uname"], VALID_LOGIN["upwd"], ClientSession()
     )
@@ -227,14 +228,15 @@
     assert len(mock_api_connect.mock_calls) > 0
     assert len(mock_get_device_info.mock_calls) > 0
     assert len(mock_get_device_data.mock_calls) > 0
 
     data = controller.get_device_data("1234", "1")
 
     assert data["operating_mode"] == "heating"
+    assert data["requested_temp"] == 34.7
 
 
 async def test_operating_mode_dhw():
     """Test the Controller Operating Mode DHW."""
     controller = MasterthermController(
         VALID_LOGIN["uname"], VALID_LOGIN["upwd"], ClientSession()
     )
@@ -256,14 +258,15 @@
     assert len(mock_api_connect.mock_calls) > 0
     assert len(mock_get_device_info.mock_calls) > 0
     assert len(mock_get_device_data.mock_calls) > 0
 
     data = controller.get_device_data("0002", "1")
 
     assert data["operating_mode"] == "dhw"
+    assert data["requested_temp"] == 45.0
 
 
 async def test_new_api_get_info_data():
     """Test the Controller Connects and setup devices for the New API."""
     controller = MasterthermController(
         VALID_LOGIN["uname"], VALID_LOGIN["upwd"], ClientSession()
     )
```

### Comparing `masterthermconnect-2.2.5b0/tests/test_main.py` & `masterthermconnect-2.2.5b1/tests/test_main.py`

 * *Files identical despite different names*

