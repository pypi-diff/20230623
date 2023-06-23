# Comparing `tmp/plotscanner-0.0.0.tar.gz` & `tmp/plotscanner-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotscanner-0.0.0.tar", last modified: Fri Jun 23 11:46:43 2023, max compression
+gzip compressed data, was "plotscanner-0.0.1.tar", last modified: Fri Jun 23 13:48:13 2023, max compression
```

## Comparing `plotscanner-0.0.0.tar` & `plotscanner-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:46:43.204323 plotscanner-0.0.0/
--rw-rw-rw-   0        0        0     1397 2023-06-23 11:46:43.205353 plotscanner-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1110 2023-06-23 11:22:05.000000 plotscanner-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 11:46:43.172154 plotscanner-0.0.0/plotscanner/
--rw-rw-rw-   0        0        0    14840 2023-06-23 10:27:02.000000 plotscanner-0.0.0/plotscanner/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-23 10:14:26.000000 plotscanner-0.0.0/plotscanner/__init__.py
--rw-rw-rw-   0        0        0     2290 2023-06-22 13:34:43.000000 plotscanner-0.0.0/plotscanner/data_frame_table.py
--rw-rw-rw-   0        0        0     3165 2023-06-21 12:51:20.000000 plotscanner-0.0.0/plotscanner/geometry.py
--rw-rw-rw-   0        0        0     3418 2023-06-22 06:35:06.000000 plotscanner-0.0.0/plotscanner/grid.py
--rw-rw-rw-   0        0        0    11361 2023-06-22 13:34:43.000000 plotscanner-0.0.0/plotscanner/plotdigitizer.py
--rw-rw-rw-   0        0        0     3517 2023-06-21 12:51:20.000000 plotscanner-0.0.0/plotscanner/trajectory.py
--rw-rw-rw-   0        0        0    11738 2023-06-22 13:34:43.000000 plotscanner-0.0.0/plotscanner/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:46:43.202046 plotscanner-0.0.0/plotscanner.egg-info/
--rw-rw-rw-   0        0        0     1397 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-23 11:46:43.000000 plotscanner-0.0.0/plotscanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 11:46:43.207311 plotscanner-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      948 2023-06-23 11:44:14.000000 plotscanner-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:48:13.307353 plotscanner-0.0.1/
+-rw-rw-rw-   0        0        0     1357 2023-06-23 13:48:13.307353 plotscanner-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1070 2023-06-23 11:52:11.000000 plotscanner-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 13:48:13.262318 plotscanner-0.0.1/plotscanner/
+-rw-rw-rw-   0        0        0    12881 2023-06-23 13:44:11.000000 plotscanner-0.0.1/plotscanner/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 10:14:26.000000 plotscanner-0.0.1/plotscanner/__init__.py
+-rw-rw-rw-   0        0        0     2897 2023-06-23 13:42:29.000000 plotscanner-0.0.1/plotscanner/data_frame_table.py
+-rw-rw-rw-   0        0        0     3165 2023-06-21 12:51:20.000000 plotscanner-0.0.1/plotscanner/geometry.py
+-rw-rw-rw-   0        0        0     3418 2023-06-22 06:35:06.000000 plotscanner-0.0.1/plotscanner/grid.py
+-rw-rw-rw-   0        0        0    11361 2023-06-22 13:34:43.000000 plotscanner-0.0.1/plotscanner/plotdigitizer.py
+-rw-rw-rw-   0        0        0     3517 2023-06-21 12:51:20.000000 plotscanner-0.0.1/plotscanner/trajectory.py
+-rw-rw-rw-   0        0        0    11252 2023-06-23 13:43:16.000000 plotscanner-0.0.1/plotscanner/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:48:13.302720 plotscanner-0.0.1/plotscanner.egg-info/
+-rw-rw-rw-   0        0        0     1357 2023-06-23 13:48:11.000000 plotscanner-0.0.1/plotscanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-23 13:48:12.000000 plotscanner-0.0.1/plotscanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:48:12.000000 plotscanner-0.0.1/plotscanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-23 13:48:12.000000 plotscanner-0.0.1/plotscanner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 13:48:11.000000 plotscanner-0.0.1/plotscanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-06-23 13:48:12.000000 plotscanner-0.0.1/plotscanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-23 13:48:12.000000 plotscanner-0.0.1/plotscanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:48:13.311566 plotscanner-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      948 2023-06-23 13:47:46.000000 plotscanner-0.0.1/setup.py
```

### Comparing `plotscanner-0.0.0/PKG-INFO` & `plotscanner-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotscanner
-Version: 0.0.0
+Version: 0.0.1
 Summary: The application for digitizing images of plots.
 Home-page: https://github.com/IlS0/Plot-digitization
 Author-email: silru@internet.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -14,24 +14,20 @@
 Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
 
 ## Documentation 
 You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
 
 ## Installation
 ```
-$ python3 -m pip install plotscanner
-$ plotscanner --help
+$ pip install plotscanner
 ```
 
 ## Run
 Start the application by running the command in the terminal:
 `$ plotscanner`
 
 Follow the instructions in the app window to work correctly.
 ### Image preparing
 Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
 ![Example image](./plotscanner/readme_imgs/example.jpg)
 
- 
-
-
```

### Comparing `plotscanner-0.0.0/README.md` & `plotscanner-0.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,18 @@
 Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
 
 ## Documentation 
 You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
 
 ## Installation
 ```
-$ python3 -m pip install plotscanner
-$ plotscanner --help
+$ pip install plotscanner
 ```
 
 ## Run
 Start the application by running the command in the terminal:
 `$ plotscanner`
 
 Follow the instructions in the app window to work correctly.
 ### Image preparing
 Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
 ![Example image](./plotscanner/readme_imgs/example.jpg)
-
- 
-
```

### Comparing `plotscanner-0.0.0/plotscanner/geometry.py` & `plotscanner-0.0.1/plotscanner/geometry.py`

 * *Files identical despite different names*

### Comparing `plotscanner-0.0.0/plotscanner/grid.py` & `plotscanner-0.0.1/plotscanner/grid.py`

 * *Files identical despite different names*

### Comparing `plotscanner-0.0.0/plotscanner/plotdigitizer.py` & `plotscanner-0.0.1/plotscanner/plotdigitizer.py`

 * *Files identical despite different names*

### Comparing `plotscanner-0.0.0/plotscanner/trajectory.py` & `plotscanner-0.0.1/plotscanner/trajectory.py`

 * *Files identical despite different names*

### Comparing `plotscanner-0.0.0/plotscanner.egg-info/PKG-INFO` & `plotscanner-0.0.1/plotscanner.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotscanner
-Version: 0.0.0
+Version: 0.0.1
 Summary: The application for digitizing images of plots.
 Home-page: https://github.com/IlS0/Plot-digitization
 Author-email: silru@internet.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -14,24 +14,20 @@
 Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
 
 ## Documentation 
 You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
 
 ## Installation
 ```
-$ python3 -m pip install plotscanner
-$ plotscanner --help
+$ pip install plotscanner
 ```
 
 ## Run
 Start the application by running the command in the terminal:
 `$ plotscanner`
 
 Follow the instructions in the app window to work correctly.
 ### Image preparing
 Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
 ![Example image](./plotscanner/readme_imgs/example.jpg)
 
- 
-
-
```

### Comparing `plotscanner-0.0.0/setup.py` & `plotscanner-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fin:
     long_description = fin.read()
 
 setup(name='plotscanner',
-      version='0.0.0',
+      version='0.0.1',
       description='The application for digitizing images of plots.',
       packages=['plotscanner'],
       py_modules = ['plotscanner'],
       author_email='silru@internet.ru',
       zip_safe=False,
       long_description=long_description,
       long_description_content_type="text/markdown",
```

