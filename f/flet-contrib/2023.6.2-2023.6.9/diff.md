# Comparing `tmp/flet_contrib-2023.6.2.tar.gz` & `tmp/flet_contrib-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib-2023.6.2.tar", max compression
+gzip compressed data, was "flet_contrib-2023.6.9.tar", max compression
```

## Comparing `flet_contrib-2023.6.2.tar` & `flet_contrib-2023.6.9.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/LICENSE
--rw-r--r--   0        0        0     1497 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/README.md
--rw-r--r--   0        0        0     1642 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/README.md
--rw-r--r--   0        0        0      215 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/__init__.py
--rw-r--r--   0        0        0      859 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/examples/color_picker_dialog.py
--rw-r--r--   0        0        0      538 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/examples/hue_slider_example.py
--rw-r--r--   0        0        0      416 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/examples/update_color_property.py
--rw-r--r--   0        0        0   128246 2023-06-02 19:54:22.130944 flet_contrib-2023.6.2/flet_contrib/color_picker/media/color_picker.png
--rw-r--r--   0        0        0     7249 2023-06-02 19:54:22.134944 flet_contrib-2023.6.2/flet_contrib/color_picker/src/color_picker.py
--rw-r--r--   0        0        0     2644 2023-06-02 19:54:22.134944 flet_contrib-2023.6.2/flet_contrib/color_picker/src/hue_slider.py
--rw-r--r--   0        0        0     4709 2023-06-02 19:54:22.134944 flet_contrib-2023.6.2/flet_contrib/color_picker/src/palette_color_picker.py
--rw-r--r--   0        0        0      464 2023-06-02 19:54:22.134944 flet_contrib-2023.6.2/flet_contrib/color_picker/src/utils.py
--rw-r--r--   0        0        0      442 2023-06-02 19:54:49.210813 flet_contrib-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 flet_contrib-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/LICENSE
+-rw-r--r--   0        0        0     1497 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/README.md
+-rw-r--r--   0        0        0     1642 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/flet_contrib/color_picker/README.md
+-rw-r--r--   0        0        0      215 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/flet_contrib/color_picker/__init__.py
+-rw-r--r--   0        0        0      859 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/flet_contrib/color_picker/examples/color_picker_dialog.py
+-rw-r--r--   0        0        0      538 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/flet_contrib/color_picker/examples/hue_slider_example.py
+-rw-r--r--   0        0        0      416 2023-06-09 17:06:18.601987 flet_contrib-2023.6.9/flet_contrib/color_picker/examples/update_color_property.py
+-rw-r--r--   0        0        0   128246 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/color_picker/media/color_picker.png
+-rw-r--r--   0        0        0     7249 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/color_picker/src/color_picker.py
+-rw-r--r--   0        0        0     2644 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/color_picker/src/hue_slider.py
+-rw-r--r--   0        0        0     4709 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/color_picker/src/palette_color_picker.py
+-rw-r--r--   0        0        0      464 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/color_picker/src/utils.py
+-rw-r--r--   0        0        0     2135 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/vertical_splitter/README.md
+-rw-r--r--   0        0        0      106 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/vertical_splitter/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/vertical_splitter/examples/vertical_splitter_with_containers.py
+-rw-r--r--   0        0        0     2545 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/vertical_splitter/examples/vertical_splitter_with_navigationrail_and_text.py
+-rw-r--r--   0        0        0     2942 2023-06-09 17:06:18.605987 flet_contrib-2023.6.9/flet_contrib/vertical_splitter/src/vertical_splitter.py
+-rw-r--r--   0        0        0      442 2023-06-09 17:06:44.669118 flet_contrib-2023.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 flet_contrib-2023.6.9/PKG-INFO
```

### Comparing `flet_contrib-2023.6.2/LICENSE` & `flet_contrib-2023.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/README.md` & `flet_contrib-2023.6.9/README.md`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/README.md` & `flet_contrib-2023.6.9/flet_contrib/color_picker/README.md`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/examples/color_picker_dialog.py` & `flet_contrib-2023.6.9/flet_contrib/color_picker/examples/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/examples/hue_slider_example.py` & `flet_contrib-2023.6.9/flet_contrib/color_picker/examples/hue_slider_example.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/media/color_picker.png` & `flet_contrib-2023.6.9/flet_contrib/color_picker/media/color_picker.png`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/src/color_picker.py` & `flet_contrib-2023.6.9/flet_contrib/color_picker/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/src/hue_slider.py` & `flet_contrib-2023.6.9/flet_contrib/color_picker/src/hue_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/flet_contrib/color_picker/src/palette_color_picker.py` & `flet_contrib-2023.6.9/flet_contrib/color_picker/src/palette_color_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib-2023.6.2/PKG-INFO` & `flet_contrib-2023.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-contrib
-Version: 2023.6.2
+Version: 2023.6.9
 Summary: Flet controls by the community
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

