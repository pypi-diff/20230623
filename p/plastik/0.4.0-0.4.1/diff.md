# Comparing `tmp/plastik-0.4.0.tar.gz` & `tmp/plastik-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastik-0.4.0.tar", max compression
+gzip compressed data, was "plastik-0.4.1.tar", max compression
```

## Comparing `plastik-0.4.0.tar` & `plastik-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-23 10:15:55.485187 plastik-0.4.0/LICENSE
--rw-r--r--   0        0        0      818 2023-06-23 10:15:55.485187 plastik-0.4.0/README.md
--rw-r--r--   0        0        0     1031 2023-06-23 10:16:11.965225 plastik-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      263 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/axes.py
--rw-r--r--   0        0        0     8874 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/colors.py
--rw-r--r--   0        0        0      942 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/default.mplstyle
--rw-r--r--   0        0        0     5514 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/legends.py
--rw-r--r--   0        0        0    12220 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/ridge.py
--rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 plastik-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 13:30:47.011739 plastik-0.4.1/LICENSE
+-rw-r--r--   0        0        0      818 2023-06-23 13:30:47.011739 plastik-0.4.1/README.md
+-rw-r--r--   0        0        0     1031 2023-06-23 13:31:01.216265 plastik-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-06-23 13:30:47.027740 plastik-0.4.1/src/plastik/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-23 13:30:47.027740 plastik-0.4.1/src/plastik/axes.py
+-rw-r--r--   0        0        0     9415 2023-06-23 13:31:01.216265 plastik-0.4.1/src/plastik/colors.py
+-rw-r--r--   0        0        0      942 2023-06-23 13:30:47.027740 plastik-0.4.1/src/plastik/default.mplstyle
+-rw-r--r--   0        0        0     5514 2023-06-23 13:30:47.027740 plastik-0.4.1/src/plastik/legends.py
+-rw-r--r--   0        0        0    12220 2023-06-23 13:30:47.027740 plastik-0.4.1/src/plastik/ridge.py
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 plastik-0.4.1/PKG-INFO
```

### Comparing `plastik-0.4.0/LICENSE` & `plastik-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/README.md` & `plastik-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/pyproject.toml` & `plastik-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plastik"
-version = "0.4.0"
+version = "0.4.1"
 description = "plastic surgery for plt"
 authors = ["Eirik Rolland Enger <eirroleng@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/engeir/plastik"
 repository = "https://github.com/engeir/plastik"
 documentation = "https://plastik.readthedocs.io/en/latest/"
```

### Comparing `plastik-0.4.0/src/plastik/axes.py` & `plastik-0.4.1/src/plastik/axes.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/src/plastik/colors.py` & `plastik-0.4.1/src/plastik/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from typing import Literal, Sequence, overload
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pywaffle
 
@@ -21,29 +22,31 @@
 
 
 def create_colorlist(
     color_specifier: Sequence | str, n: int, map: bool = False
 ) -> list[str] | mpl.colors.Colormap:
     """Create `n` colors from a color map.
 
-    The `n` colors are drawn from one of the matplotlib color maps, or a new color map
-    is created using the input colors.
+    The `n` colours are drawn from one of the matplotlib colour maps, or a new colour
+    map is created using the input colours. Specifying 'help' as the ``color_specifier``
+    will print the list of available colour names in a nicer format.
 
     Parameters
     ----------
     color_specifier : Sequence | str
-        The name of a matplotlib color map or a list of two colors. To get the full list
-        of available color maps, try with a nonsense color map, or see
+        The name of a matplotlib colour map or a list of two colors. To get the full
+        list of available color maps, try with a nonsense color map, or see
         https://matplotlib.org/stable/tutorials/colors/colormaps.html#classes-of-colormaps.
         If two colors in a list is provided, any color that
-        ``matplotlib.colors.LinearSegmentedColormap.from_list`` accepts is valid.
+        ``matplotlib.colors.LinearSegmentedColormap.from_list`` accepts is valid. You
+        may also use the special name 'help' to get a list of available colour names.
     n : int
         The number of colors to be created.
     map : bool
-        If True, return the color map itself instead of the list. To draw colors from
+        If True, return the colour map itself instead of the list. To draw colours from
         it, use ``color_map(range(n))``, or to place HEX values in a list::
 
             import matplotlib.colors as mpl.colors
             n = 5
             c_list = [mpl.colors.to_hex(c) for c in color_map(range(n))]
 
     Returns
@@ -101,14 +104,23 @@
             c_list = [mpl.colors.to_hex(c) for c in color_map(range(n))]
 
     Returns
     -------
     list[str]
         A list of `n` colors in HEX format.
     """
+    if cmap_name == "help":
+        try:
+            plt.get_cmap(cmap_name, 1)
+        except Exception as e:
+            s1, s2 = str(e).split(" supported values are ")
+            print("Supported colour names are:")
+            for word in s2.split(", "):
+                print("\t", word[1:-1])
+        sys.exit()
     if map:
         return plt.get_cmap(cmap_name, n)
     return [mpl.colors.to_hex(c) for c in plt.get_cmap(cmap_name, n)(range(n))]
 
 
 def _create_colorlist_between(colors: Sequence, n: int, map: bool = False) -> list[str]:
     """Create `n` colors between two colors (inclusive).
```

### Comparing `plastik-0.4.0/src/plastik/default.mplstyle` & `plastik-0.4.1/src/plastik/default.mplstyle`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/src/plastik/legends.py` & `plastik-0.4.1/src/plastik/legends.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/src/plastik/ridge.py` & `plastik-0.4.1/src/plastik/ridge.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.0/PKG-INFO` & `plastik-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastik
-Version: 0.4.0
+Version: 0.4.1
 Summary: plastic surgery for plt
 Home-page: https://github.com/engeir/plastik
 License: GPLv3
 Author: Eirik Rolland Enger
 Author-email: eirroleng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

