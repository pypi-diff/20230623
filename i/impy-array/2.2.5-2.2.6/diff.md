# Comparing `tmp/impy_array-2.2.5.tar.gz` & `tmp/impy_array-2.2.6.tar.gz`

## Comparing `impy_array-2.2.5.tar` & `impy_array-2.2.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/__init__.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/_const.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/_types.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/array_api.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/binder.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/collections.py
--rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/core.py
--rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/correlation.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/io.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/random.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/roi.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/__init__.py
--rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_deprecated.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_imshow.py
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/axesmixin.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/big.py
--rw-r--r--   0        0        0   155930 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/imgarray.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/label.py
--rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/labeledarray.py
--rw-r--r--   0        0        0    55446 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/lazy.py
--rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/phasearray.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/specials.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/tiled.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_corr.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_deconv.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_docs.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_filters.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_glcm.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_linalg.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_misc.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_plot.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_process_numba.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_skimage.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_structures.py
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_transform.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/__init__.py
--rw-r--r--   0        0        0    27104 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/metaarray.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/overload.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/__init__.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axes.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axes_tuple.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axis.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_slicer.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/frame/__init__.py
--rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/frame/frames.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/axesop.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/deco.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/gauss.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/misc.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/slicer.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/utilcls.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/__init__.py
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/utils.py
--rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/viewer.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.5/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.5/LICENSE
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.5/README.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 impy_array-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 impy_array-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/__init__.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/_const.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/_types.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/array_api.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/binder.py
+-rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/collections.py
+-rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/core.py
+-rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/correlation.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/io.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/random.py
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/roi.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/__init__.py
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_deprecated.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_imshow.py
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/axesmixin.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/big.py
+-rw-r--r--   0        0        0   157136 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/imgarray.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/label.py
+-rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/labeledarray.py
+-rw-r--r--   0        0        0    55517 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/lazy.py
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/phasearray.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/specials.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/tiled.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/__init__.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_corr.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_deconv.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_docs.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_filters.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_glcm.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_linalg.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_misc.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_plot.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_process_numba.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_skimage.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_structures.py
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/_utils/_transform.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/bases/__init__.py
+-rw-r--r--   0        0        0    27098 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/bases/metaarray.py
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/arrays/bases/overload.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/axes/__init__.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/axes/_axes.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/axes/_axes_tuple.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/axes/_axis.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/axes/_slicer.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/frame/__init__.py
+-rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/frame/frames.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/axesop.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/deco.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/gauss.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/misc.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/slicer.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/utils/utilcls.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/viewer/__init__.py
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/viewer/utils.py
+-rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.6/impy/viewer/viewer.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.6/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.6/LICENSE
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.6/README.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 impy_array-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 impy_array-2.2.6/PKG-INFO
```

### Comparing `impy_array-2.2.5/impy/__init__.py` & `impy_array-2.2.6/impy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 import logging
 
 from ._const import Const, SetConst, use
```

### Comparing `impy_array-2.2.5/impy/__main__.py` & `impy_array-2.2.6/impy/__main__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/_const.py` & `impy_array-2.2.6/impy/_const.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/_types.py` & `impy_array-2.2.6/impy/_types.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/array_api.py` & `impy_array-2.2.6/impy/array_api.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/binder.py` & `impy_array-2.2.6/impy/binder.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/collections.py` & `impy_array-2.2.6/impy/collections.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/core.py` & `impy_array-2.2.6/impy/core.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/correlation.py` & `impy_array-2.2.6/impy/correlation.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/io.py` & `impy_array-2.2.6/impy/io.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/random.py` & `impy_array-2.2.6/impy/random.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/roi.py` & `impy_array-2.2.6/impy/roi.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/__init__.py` & `impy_array-2.2.6/impy/arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_deprecated.py` & `impy_array-2.2.6/impy/arrays/_deprecated.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_imshow.py` & `impy_array-2.2.6/impy/arrays/_imshow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Callable
 import numpy as np
 
-from .labeledarray import LabeledArray
-from ..utils.axesop import find_first_appeared, complement_axes
-from ..axes import slicer
+from impy.arrays.labeledarray import LabeledArray
+from impy.utils.axesop import find_first_appeared, complement_axes
+from impy.axes import slicer
 
 __all__ = ["imshow", "register"]
 
 class ImshowManager:
     """Manage imshow plugins."""
     
     def __init__(self):
@@ -27,21 +27,22 @@
         return self._mgr[plugin](*args, **kwargs)
     
 MANAGER = ImshowManager()
 
 imshow = MANAGER.call
 register = MANAGER.register
 
-# ##############
+# ################################################################################
 #   magicgui
-# ##############
+# ################################################################################
 
 @register("magicgui")
 def _imshow_magicgui(arr: LabeledArray, dims, **kwargs) -> LabeledArray:
-    from magicgui import  widgets as wdt
+    from magicgui import widgets as wdt
+
     h, w = arr.sizesof(dims)
     if h > w:
         min_height = 400
         min_width = 400 / h * w
     else:
         min_height = 400 / w * h
         min_width = 400
@@ -62,104 +63,85 @@
         )
         sliders.margins = (0, 0, 0, 0)
         @sliders.changed.connect
         def _on_slider_change():
             vals = tuple(sl.value for sl in sliders)
             img_slice = arr[fmt[vals]]
             img.value = img_slice
-    
-    min_slider = wdt.FloatSlider(min=min_, max=max_, value=min_, name="min")
-    max_slider = wdt.FloatSlider(min=min_, max=max_, value=max_, name="max")
-    clim = wdt.Container(
-        widgets=[min_slider, max_slider],
-    )
-    clim.margins = (0, 0, 0, 0)
-    
-    @min_slider.changed.connect
-    def _on_contrast_min_change():
-        if min_slider.value > max_slider.value:
-            max_slider.value = min_slider.value
-
-    @max_slider.changed.connect
-    def _on_contrast_max_change():
-        if min_slider.value > max_slider.value:
-            min_slider.value = max_slider.value
-    
+
+    clim = wdt.FloatRangeSlider(min=min_, max=max_, value=(min_, max_), step=(max_ - min_) / 1000, name="clim")
     imgc = wdt.Container(widgets=[img])
     imgc.min_height = min_height
     imgc.min_width = min_width
     imgc.margins = (0, 0, 0, 0)
     if arr.labels is not None:
         cbox = wdt.CheckBox(text="Show labels", value=kwargs.get("label", False))
         alpha = wdt.FloatSlider(name="Label alpha", value=0.3, min=0.0, max=1.0)
         label_wdt = wdt.Container(widgets=[cbox, alpha])
         
         @cbox.changed.connect
         @alpha.changed.connect
         @sliders.changed.connect
-        @min_slider.changed.connect
-        @max_slider.changed.connect
+        @clim.changed.connect
         def _on_slider_change():
             vals = tuple(sl.value for sl in sliders)
             img_slice = arr[fmt[vals]]
             if cbox.value:
                 from skimage.color import label2rgb
-                vmin = min_slider.value
-                vmax = max_slider.value
+
+                vmin, vmax = clim.value
                 image = (np.clip(img_slice, vmin, vmax) - vmin)/(vmax - vmin)
                 img.value = label2rgb(
                     img_slice.labels, image, alpha=alpha.value, bg_label=0, image_alpha=1,
                     bg_color=None,
                 )
             else:
                 img.value = img_slice
-            img.set_clim(min_slider.value, max_slider.value)
+            img.set_clim(*clim.value)
 
     else:
         label_wdt = wdt.EmptyWidget()
         
         @sliders.changed.connect
         def _on_slider_change():
             vals = tuple(sl.value for sl in sliders)
             img_slice = arr[fmt[vals]]
             img.value = img_slice
         
-        @min_slider.changed.connect
-        @max_slider.changed.connect
+        @clim.changed.connect
         def _on_clim_change():
-            img.set_clim(min_slider.value, max_slider.value)
+            img.set_clim(*clim.value)
     
     widget = wdt.Container(
         widgets=[imgc, sliders, clim, label_wdt], 
         labels=False,
     )
     
     if "cmap" in kwargs:
         img.set_cmap(kwargs["cmap"])
     widget.show(kwargs.get("run", False))
     return arr
 
-# ################
+# ################################################################################
 #   matplotlib
-# ################
+# ################################################################################
 
 @register("matplotlib")
 def _imshow_matplotlib(self: LabeledArray, label, dims, **kwargs) -> LabeledArray:
     from ._utils import _plot as _plt
     alpha = 0.3
     if label and self.labels is None:
         label = False
     if self.ndim == 1:
         _plt.plot_1d(self.value, **kwargs)
     elif self.ndim == 2:
         if label:
             _plt.plot_2d_label(self.value, self.labels.value, alpha, **kwargs)
         else:
             _plt.plot_2d(self.value, **kwargs)
-        self.hist()
         
     elif self.ndim == 3:
         if "c" not in self.axes:
             imglist = self.split(
                 axis=find_first_appeared(self.axes, include=self.axes, exclude=dims)
             )
             if len(imglist) > 24:
```

### Comparing `impy_array-2.2.5/impy/arrays/axesmixin.py` & `impy_array-2.2.6/impy/arrays/axesmixin.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/big.py` & `impy_array-2.2.6/impy/arrays/big.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/imgarray.py` & `impy_array-2.2.6/impy/arrays/imgarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -6277,3470 +6277,3545 @@
 00018840: 656c 662c 0d0a 2020 2020 2020 2020 7368  elf,..        sh
 00018850: 6170 653a 2069 6e74 207c 2049 7465 7261  ape: int | Itera
 00018860: 626c 655b 696e 745d 207c 2046 6674 5368  ble[int] | FftSh
 00018870: 6170 6520 3d20 2273 616d 6522 2c0d 0a20  ape = "same",.. 
 00018880: 2020 2020 2020 206e 6f72 6d3a 2062 6f6f         norm: boo
 00018890: 6c20 3d20 4661 6c73 652c 200d 0a20 2020  l = False, ..   
 000188a0: 2020 2020 207a 6572 6f5f 6e6f 726d 3a20       zero_norm: 
-000188b0: 626f 6f6c 203d 2046 616c 7365 2c20 2a2c  bool = False, *,
-000188c0: 0d0a 2020 2020 2020 2020 646f 7562 6c65  ..        double
-000188d0: 5f70 7265 6369 7369 6f6e 3a20 626f 6f6c  _precision: bool
-000188e0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-000188f0: 2020 2064 696d 733a 2044 696d 7320 3d20     dims: Dims = 
-00018900: 4e6f 6e65 0d0a 2020 2020 2920 2d3e 2049  None..    ) -> I
-00018910: 6d67 4172 7261 793a 0d0a 2020 2020 2020  mgArray:..      
-00018920: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
-00018930: 6574 7572 6e20 6e2d 4420 706f 7765 7220  eturn n-D power 
-00018940: 7370 6563 7472 6120 6f66 2069 6d61 6765  spectra of image
-00018950: 732c 2077 6869 6368 2069 7320 6465 6669  s, which is defi
-00018960: 6e65 6420 6173 3a0d 0a20 2020 2020 2020  ned as:..       
-00018970: 200d 0a20 2020 2020 2020 202e 2e20 6d61   ..        .. ma
-00018980: 7468 3a3a 0d0a 2020 2020 2020 2020 0d0a  th::..        ..
-00018990: 2020 2020 2020 2020 2020 2020 5020 3d20              P = 
-000189a0: 5265 2846 5b49 5f7b 696d 677d 5d29 5e32  Re(F[I_{img}])^2
-000189b0: 202b 2049 6d28 465b 495f 7b69 6d67 7d5d   + Im(F[I_{img}]
-000189c0: 295e 320d 0a0d 0a20 2020 2020 2020 2050  )^2....        P
-000189d0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-000189e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000189f0: 2020 2020 2020 2073 6861 7065 203a 2069         shape : i
-00018a00: 6e74 2c20 6974 6572 6162 6c65 206f 6620  nt, iterable of 
-00018a10: 696e 742c 2022 7371 7561 7265 2220 6f72  int, "square" or
-00018a20: 2022 7361 6d65 220d 0a20 2020 2020 2020   "same"..       
-00018a30: 2020 2020 204f 7574 7075 7420 7368 6170       Output shap
-00018a40: 652e 2049 6e70 7574 2069 6d61 6765 2069  e. Input image i
-00018a50: 7320 7061 6464 6564 206f 7220 6372 6f70  s padded or crop
-00018a60: 7065 6420 6163 636f 7264 696e 6720 746f  ped according to
-00018a70: 2074 6869 7320 7661 6c75 653a 0d0a 2020   this value:..  
-00018a80: 2020 2020 2020 2020 2020 2d20 696e 7465            - inte
-00018a90: 6765 7273 3a20 7061 6464 6564 206f 7220  gers: padded or 
-00018aa0: 6372 6f70 7065 6420 746f 2074 6865 2073  cropped to the s
-00018ab0: 7065 6369 6669 6564 2073 6861 7065 2e0d  pecified shape..
-00018ac0: 0a20 2020 2020 2020 2020 2020 202d 2022  .            - "
-00018ad0: 7371 7561 7265 223a 2070 6164 6465 6420  square": padded 
-00018ae0: 746f 2073 6d61 6c6c 6573 7420 325e 4e2d  to smallest 2^N-
-00018af0: 6c6f 6e67 2073 7175 6172 652e 0d0a 2020  long square...  
-00018b00: 2020 2020 2020 2020 2020 2d20 2273 616d            - "sam
-00018b10: 6522 2028 6465 6661 756c 7429 3a20 6e6f  e" (default): no
-00018b20: 2070 6164 6469 6e67 206f 7220 6372 6f70   padding or crop
-00018b30: 7069 6e67 2e0d 0a20 2020 2020 2020 206e  ping...        n
-00018b40: 6f72 6d20 3a20 626f 6f6c 2c20 6465 6661  orm : bool, defa
-00018b50: 756c 7420 6973 2046 616c 7365 0d0a 2020  ult is False..  
-00018b60: 2020 2020 2020 2020 2020 4966 2054 7275            If Tru
-00018b70: 652c 206d 6178 696d 756d 2076 616c 7565  e, maximum value
-00018b80: 206f 6620 706f 7765 7220 7370 6563 7472   of power spectr
-00018b90: 6120 6973 2061 646a 7573 7465 6420 746f  a is adjusted to
-00018ba0: 2031 2e0d 0a20 2020 2020 2020 207b 646f   1...        {do
-00018bb0: 7562 6c65 5f70 7265 6369 7369 6f6e 7d0d  uble_precision}.
-00018bc0: 0a20 2020 2020 2020 207b 6469 6d73 7d0d  .        {dims}.
-00018bd0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00018be0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00018bf0: 2d2d 2d0d 0a20 2020 2020 2020 2049 6d67  ---..        Img
-00018c00: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
-00018c10: 2020 2050 6f77 6572 2073 7065 6374 7261     Power spectra
-00018c20: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00018c30: 2020 2020 5365 6520 416c 736f 0d0a 2020      See Also..  
-00018c40: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
-00018c50: 2020 2020 2020 2020 6c6f 6361 6c5f 706f          local_po
-00018c60: 7765 725f 7370 6563 7472 610d 0a20 2020  wer_spectra..   
-00018c70: 2020 2020 2022 2222 2020 2020 2020 2020       """        
-00018c80: 0d0a 2020 2020 2020 2020 6672 6571 203d  ..        freq =
-00018c90: 2073 656c 662e 6666 7428 6469 6d73 3d64   self.fft(dims=d
-00018ca0: 696d 732c 2073 6861 7065 3d73 6861 7065  ims, shape=shape
-00018cb0: 2c20 646f 7562 6c65 5f70 7265 6369 7369  , double_precisi
-00018cc0: 6f6e 3d64 6f75 626c 655f 7072 6563 6973  on=double_precis
-00018cd0: 696f 6e29 0d0a 2020 2020 2020 2020 7077  ion)..        pw
-00018ce0: 203d 2066 7265 712e 7265 616c 2a2a 3220   = freq.real**2 
-00018cf0: 2b20 6672 6571 2e69 6d61 672a 2a32 0d0a  + freq.imag**2..
-00018d00: 2020 2020 2020 2020 6966 206e 6f72 6d3a          if norm:
-00018d10: 0d0a 2020 2020 2020 2020 2020 2020 7077  ..            pw
-00018d20: 202f 3d20 7077 2e6d 6178 2829 0d0a 2020   /= pw.max()..  
-00018d30: 2020 2020 2020 7077 3a20 496d 6741 7272        pw: ImgArr
-00018d40: 6179 0d0a 2020 2020 2020 2020 6966 207a  ay..        if z
-00018d50: 6572 6f5f 6e6f 726d 3a0d 0a20 2020 2020  ero_norm:..     
-00018d60: 2020 2020 2020 2073 6c20 3d20 7377 6974         sl = swit
-00018d70: 6368 5f73 6c69 6365 2864 696d 732c 2070  ch_slice(dims, p
-00018d80: 772e 6178 6573 2c20 6966 696e 3d6e 702e  w.axes, ifin=np.
-00018d90: 6172 7261 7928 7077 2e73 6861 7065 292f  array(pw.shape)/
-00018da0: 2f32 2c20 6966 6e6f 743d 736c 6963 6528  /2, ifnot=slice(
-00018db0: 4e6f 6e65 2929 0d0a 2020 2020 2020 2020  None))..        
-00018dc0: 2020 2020 7077 5b73 6c5d 203d 2030 0d0a      pw[sl] = 0..
-00018dd0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00018de0: 770d 0a0d 0a20 2020 2040 5f64 6f63 732e  w....    @_docs.
-00018df0: 7772 6974 655f 646f 6373 0d0a 2020 2020  write_docs..    
-00018e00: 4064 696d 735f 746f 5f73 7061 7469 616c  @dims_to_spatial
-00018e10: 5f61 7865 730d 0a20 2020 2064 6566 2072  _axes..    def r
-00018e20: 6164 6f6e 280d 0a20 2020 2020 2020 2073  adon(..        s
-00018e30: 656c 662c 0d0a 2020 2020 2020 2020 6465  elf,..        de
-00018e40: 6772 6565 733a 2066 6c6f 6174 207c 2049  grees: float | I
-00018e50: 7465 7261 626c 655b 666c 6f61 745d 2c20  terable[float], 
-00018e60: 0d0a 2020 2020 2020 2020 2a2c 0d0a 2020  ..        *,..  
-00018e70: 2020 2020 2020 6365 6e74 7261 6c5f 6178        central_ax
-00018e80: 6973 3a20 4178 6973 4c69 6b65 207c 2053  is: AxisLike | S
-00018e90: 6571 7565 6e63 655b 666c 6f61 745d 207c  equence[float] |
-00018ea0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20   None = None,.. 
-00018eb0: 2020 2020 2020 206f 7264 6572 3a20 696e         order: in
-00018ec0: 7420 3d20 332c 0d0a 2020 2020 2020 2020  t = 3,..        
-00018ed0: 6469 6d73 3a20 4469 6d73 203d 204e 6f6e  dims: Dims = Non
-00018ee0: 652c 0d0a 2020 2020 2920 2d3e 2049 6d67  e,..    ) -> Img
-00018ef0: 4172 7261 793a 0d0a 2020 2020 2020 2020  Array:..        
-00018f00: 2222 220d 0a20 2020 2020 2020 2044 6973  """..        Dis
-00018f10: 6372 6574 6520 5261 646f 6e20 7472 616e  crete Radon tran
-00018f20: 7366 6f72 6d61 7469 6f6e 206f 6620 3244  sformation of 2D
-00018f30: 206f 7220 3344 2069 6d61 6765 2e0d 0a20   or 3D image... 
-00018f40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00018f50: 2052 6164 6f6e 2074 7261 6e73 666f 726d   Radon transform
-00018f60: 6174 696f 6e20 6973 2061 206c 6973 7420  ation is a list 
-00018f70: 6f66 2070 726f 6a65 6374 696f 6e20 6f66  of projection of
-00018f80: 2061 2073 616d 6520 696d 6167 6520 6672   a same image fr
-00018f90: 6f6d 2064 6966 6665 7265 6e74 2061 6e67  om different ang
-00018fa0: 6c65 732e 0d0a 2020 2020 2020 2020 4974  les...        It
-00018fb0: 2067 656e 6572 6174 6573 2074 6f6d 6f67   generates tomog
-00018fc0: 7261 7068 6963 206e 2d44 2069 6d61 6765  raphic n-D image
-00018fd0: 2073 6c69 6365 7320 6672 6f6d 2028 6e2b   slices from (n+
-00018fe0: 3129 2d44 2069 6d61 6765 2e0d 0a0d 0a20  1)-D image..... 
-00018ff0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00019000: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00019010: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2064  -----..        d
-00019020: 6567 7265 6573 203a 2066 6c6f 6174 206f  egrees : float o
-00019030: 7220 6974 6572 6162 6c65 206f 6620 666c  r iterable of fl
-00019040: 6f61 740d 0a20 2020 2020 2020 2020 2020  oat..           
-00019050: 2052 6f74 6174 696f 6e20 616e 676c 6573   Rotation angles
-00019060: 2061 726f 756e 6420 7468 6520 6365 6e74   around the cent
-00019070: 7261 6c20 6178 6973 2069 6e20 6465 6772  ral axis in degr
-00019080: 6565 732e 0d0a 2020 2020 2020 2020 6365  ees...        ce
-00019090: 6e74 7261 6c5f 6178 6973 203a 2061 7869  ntral_axis : axi
-000190a0: 732d 6c69 6b65 206f 7220 7365 7175 656e  s-like or sequen
-000190b0: 6365 206f 6620 666c 6f61 742c 206f 7074  ce of float, opt
-000190c0: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-000190d0: 2020 2056 6563 746f 7220 7468 6174 2064     Vector that d
-000190e0: 6566 696e 6573 2074 6865 2063 656e 7472  efines the centr
-000190f0: 616c 2061 7869 7320 6f66 2072 6f74 6174  al axis of rotat
-00019100: 696f 6e2e 0d0a 2020 2020 2020 2020 7b6f  ion...        {o
-00019110: 7264 6572 7d7b 6469 6d73 7d0d 0a0d 0a20  rder}{dims}.... 
-00019120: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-00019130: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-00019140: 0a20 2020 2020 2020 2049 6d67 4172 7261  .        ImgArra
-00019150: 790d 0a20 2020 2020 2020 2020 2020 2054  y..            T
-00019160: 6f6d 6f67 7261 7068 6963 2069 6d61 6765  omographic image
-00019170: 2073 6c69 6365 732e 2054 6865 2066 6972   slices. The fir
-00019180: 7374 2073 7061 7469 616c 2061 7869 7320  st spatial axis 
-00019190: 2822 7a22 2066 6f72 207a 7978 2d69 6d61  ("z" for zyx-ima
-000191a0: 6765 2920 7769 6c6c 2062 6520 6472 6f70  ge) will be drop
-000191b0: 7065 642e 0d0a 2020 2020 2020 2020 2020  ped...          
-000191c0: 2020 4966 2073 6571 7565 6e63 6520 6f66    If sequence of
-000191d0: 2066 6c6f 6174 2069 7320 6769 7665 6e20   float is given 
-000191e0: 6173 2060 6064 6567 7265 6573 6060 2c20  as ``degrees``, 
-000191f0: 2264 6567 7265 6522 2061 7869 7320 7769  "degree" axis wi
-00019200: 6c6c 2062 6520 6e65 776c 7920 6164 6465  ll be newly adde
-00019210: 6420 6174 0d0a 2020 2020 2020 2020 2020  d at..          
-00019220: 2020 7468 6520 706f 7369 7469 6f6e 2030    the position 0
-00019230: 2e20 466f 7220 696e 7374 616e 6365 2c20  . For instance, 
-00019240: 6966 2061 207a 7978 2d69 6d61 6765 2061  if a zyx-image a
-00019250: 6e64 2060 6064 6567 7265 6573 3d6e 702e  nd ``degrees=np.
-00019260: 6c69 6e73 7061 6365 2830 2c20 3138 302c  linspace(0, 180,
-00019270: 2031 3030 2960 600d 0a20 2020 2020 2020   100)``..       
-00019280: 2020 2020 2061 7265 2067 6976 656e 2c20       are given, 
-00019290: 7265 7475 726e 6564 2069 6d61 6765 2068  returned image h
-000192a0: 6173 2061 7865 7320 5b22 6465 6772 6565  as axes ["degree
-000192b0: 222c 2022 7922 2c20 2278 225d 2e0d 0a20  ", "y", "x"]... 
-000192c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000192d0: 2053 6565 2041 6c73 6f0d 0a20 2020 2020   See Also..     
-000192e0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-000192f0: 2020 2020 2069 7261 646f 6e0d 0a20 2020       iradon..   
-00019300: 2020 2020 2022 2222 2020 2020 2020 2020       """        
-00019310: 0d0a 2020 2020 2020 2020 6672 6f6d 2064  ..        from d
-00019320: 6173 6b20 696d 706f 7274 2061 7272 6179  ask import array
-00019330: 2061 7320 6461 2c20 6465 6c61 7965 640d   as da, delayed.
-00019340: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00019350: 2020 2070 6172 616d 732c 206f 7574 7075     params, outpu
-00019360: 745f 7368 6170 652c 2073 7175 6565 7a65  t_shape, squeeze
-00019370: 203d 205f 7472 616e 7366 6f72 6d2e 6e6f   = _transform.no
-00019380: 726d 616c 697a 655f 7261 646f 6e5f 696e  rmalize_radon_in
-00019390: 7075 7428 0d0a 2020 2020 2020 2020 2020  put(..          
-000193a0: 2020 7365 6c66 2c20 6469 6d73 2c20 6365    self, dims, ce
-000193b0: 6e74 7261 6c5f 6178 6973 2c20 6465 6772  ntral_axis, degr
-000193c0: 6565 730d 0a20 2020 2020 2020 2029 0d0a  ees..        )..
-000193d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000193e0: 2020 2320 6170 706c 7920 7370 6c69 6e65    # apply spline
-000193f0: 2066 696c 7465 7220 696e 2061 6476 616e   filter in advan
-00019400: 6365 2e0d 0a20 2020 2020 2020 2069 6e70  ce...        inp
-00019410: 7574 203d 2073 656c 662e 6173 5f66 6c6f  ut = self.as_flo
-00019420: 6174 2829 2e73 706c 696e 655f 6669 6c74  at().spline_filt
-00019430: 6572 286f 7264 6572 3d6f 7264 6572 290d  er(order=order).
-00019440: 0a20 2020 2020 2020 2064 656c 6179 6564  .        delayed
-00019450: 5f66 756e 6320 3d20 6465 6c61 7965 6428  _func = delayed(
-00019460: 5f74 7261 6e73 666f 726d 2e72 6164 6f6e  _transform.radon
-00019470: 5f73 696e 676c 6529 0d0a 2020 2020 2020  _single)..      
-00019480: 2020 7461 736b 7320 3d20 5b0d 0a20 2020    tasks = [..   
-00019490: 2020 2020 2020 2020 2064 656c 6179 6564           delayed
-000194a0: 5f66 756e 6328 696e 7075 742c 2070 2c20  _func(input, p, 
-000194b0: 6f72 6465 723d 6f72 6465 722c 206f 7574  order=order, out
-000194c0: 7075 745f 7368 6170 653d 6f75 7470 7574  put_shape=output
-000194d0: 5f73 6861 7065 2920 0d0a 2020 2020 2020  _shape) ..      
-000194e0: 2020 2020 2020 666f 7220 7020 696e 2070        for p in p
-000194f0: 6172 616d 730d 0a20 2020 2020 2020 205d  arams..        ]
-00019500: 0d0a 2020 2020 2020 2020 6f75 7420 3d20  ..        out = 
-00019510: 7870 2e73 7461 636b 2864 612e 636f 6d70  xp.stack(da.comp
-00019520: 7574 6528 7461 736b 7329 5b30 5d2c 2061  ute(tasks)[0], a
-00019530: 7869 733d 3029 0d0a 0d0a 2020 2020 2020  xis=0)....      
-00019540: 2020 6f75 7420 3d20 7870 2e61 736e 756d    out = xp.asnum
-00019550: 7079 286f 7574 292e 7669 6577 2873 656c  py(out).view(sel
-00019560: 662e 5f5f 636c 6173 735f 5f29 0d0a 2020  f.__class__)..  
-00019570: 2020 2020 2020 6f75 742e 5f73 6574 5f69        out._set_i
-00019580: 6e66 6f28 7365 6c66 2c20 7365 6c66 2e61  nfo(self, self.a
-00019590: 7865 732e 6472 6f70 2830 292e 696e 7365  xes.drop(0).inse
-000195a0: 7274 2830 2c20 2264 6567 7265 6522 2929  rt(0, "degree"))
-000195b0: 0d0a 2020 2020 2020 2020 6f75 742e 6178  ..        out.ax
-000195c0: 6573 5b30 5d2e 6c61 6265 6c73 203d 206c  es[0].labels = l
-000195d0: 6973 7428 6465 6772 6565 7329 0d0a 2020  ist(degrees)..  
-000195e0: 2020 2020 2020 6966 2073 7175 6565 7a65        if squeeze
-000195f0: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-00019600: 7574 203d 206f 7574 5b30 5d0d 0a20 2020  ut = out[0]..   
-00019610: 2020 2020 2072 6574 7572 6e20 6f75 740d       return out.
-00019620: 0a20 2020 200d 0a20 2020 2040 5f64 6f63  .    ..    @_doc
-00019630: 732e 7772 6974 655f 646f 6373 0d0a 2020  s.write_docs..  
-00019640: 2020 6465 6620 6972 6164 6f6e 280d 0a20    def iradon(.. 
-00019650: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-00019660: 2020 2020 2020 6465 6772 6565 733a 2053        degrees: S
-00019670: 6571 7565 6e63 655b 666c 6f61 745d 2c0d  equence[float],.
-00019680: 0a20 2020 2020 2020 202a 2c0d 0a20 2020  .        *,..   
-00019690: 2020 2020 2063 656e 7472 616c 5f61 7869       central_axi
-000196a0: 733a 2041 7869 734c 696b 6520 3d20 2279  s: AxisLike = "y
-000196b0: 222c 0d0a 2020 2020 2020 2020 6465 6772  ",..        degr
-000196c0: 6565 5f61 7869 733a 2041 7869 734c 696b  ee_axis: AxisLik
-000196d0: 6520 7c20 4e6f 6e65 203d 204e 6f6e 652c  e | None = None,
-000196e0: 0d0a 2020 2020 2020 2020 6865 6967 6874  ..        height
-000196f0: 5f61 7869 733a 2041 7869 734c 696b 6520  _axis: AxisLike 
-00019700: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0d0a  | None = None,..
-00019710: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
-00019720: 696e 7420 7c20 4e6f 6e65 203d 204e 6f6e  int | None = Non
-00019730: 652c 0d0a 2020 2020 2020 2020 7769 6e64  e,..        wind
-00019740: 6f77 3a20 7374 7220 3d20 2268 616d 6d69  ow: str = "hammi
-00019750: 6e67 222c 0d0a 2020 2020 2020 2020 6f72  ng",..        or
-00019760: 6465 723a 2069 6e74 203d 2033 2c0d 0a20  der: int = 3,.. 
-00019770: 2020 2029 202d 3e20 496d 6741 7272 6179     ) -> ImgArray
-00019780: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00019790: 2020 2020 2020 2020 496e 7665 7273 6520          Inverse 
-000197a0: 5261 646f 6e20 7472 616e 7366 6f72 6d61  Radon transforma
-000197b0: 7469 6f6e 2028 7765 6967 6874 6564 2062  tion (weighted b
-000197c0: 6163 6b20 7072 6f6a 6563 7469 6f6e 2920  ack projection) 
-000197d0: 6f66 2061 2074 696c 6520 7365 7269 6573  of a tile series
-000197e0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
-000197f0: 2020 2020 2049 6e70 7574 2061 7272 6179       Input array
-00019800: 206d 7573 7420 6265 2061 2074 696c 7420   must be a tilt 
-00019810: 7365 7269 6573 206f 6620 3144 206f 7220  series of 1D or 
-00019820: 3244 2069 6d61 6765 732e 2054 6865 7920  2D images. They 
-00019830: 6172 6520 6261 636b 2d0d 0a20 2020 2020  are back-..     
-00019840: 2020 2070 726f 6a65 6374 6564 2069 6e74     projected int
-00019850: 6f20 6120 3244 206f 7220 3344 2069 6d61  o a 2D or 3D ima
-00019860: 6765 2077 6974 6820 6172 6269 7472 6172  ge with arbitrar
-00019870: 7920 6865 6967 6874 2e0d 0a0d 0a20 2020  y height.....   
-00019880: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-00019890: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000198a0: 2d2d 2d0d 0a20 2020 2020 2020 2064 6567  ---..        deg
-000198b0: 7265 6573 203a 2073 6571 7565 6e63 6520  rees : sequence 
-000198c0: 6f66 2066 6c6f 6174 0d0a 2020 2020 2020  of float..      
-000198d0: 2020 2020 2020 5072 6f6a 6563 7469 6f6e        Projection
-000198e0: 2061 6e67 6c65 7320 696e 2064 6567 7265   angles in degre
-000198f0: 652e 204c 656e 6774 6820 6d75 7374 206d  e. Length must m
-00019900: 6174 6368 2074 6865 206c 656e 6774 6820  atch the length 
-00019910: 6f66 2074 6865 2064 6567 7265 650d 0a20  of the degree.. 
-00019920: 2020 2020 2020 2020 2020 2061 7869 7320             axis 
-00019930: 6f66 2074 6865 2069 6e70 7574 2069 6d61  of the input ima
-00019940: 6765 2e0d 0a20 2020 2020 2020 2063 656e  ge...        cen
-00019950: 7472 616c 5f61 7869 7320 3a20 4178 6973  tral_axis : Axis
-00019960: 4c69 6b65 2c20 6f70 7469 6f6e 616c 0d0a  Like, optional..
-00019970: 2020 2020 2020 2020 2020 2020 4178 6973              Axis
-00019980: 2070 6172 616c 6c65 6c20 746f 2074 6865   parallel to the
-00019990: 2072 6f74 6174 696f 6e20 6178 6973 2e0d   rotation axis..
-000199a0: 0a20 2020 2020 2020 2064 6567 7265 655f  .        degree_
-000199b0: 6178 6973 203a 2041 7869 734c 696b 652c  axis : AxisLike,
-000199c0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-000199d0: 2020 2020 2020 2041 7869 7320 6f66 2072         Axis of r
-000199e0: 6f74 6174 696f 6e20 6465 6772 6565 2e20  otation degree. 
-000199f0: 4279 2064 6566 6175 6c74 2c20 7468 6520  By default, the 
-00019a00: 6669 7273 7420 6178 6973 2077 696c 6c20  first axis will 
-00019a10: 6265 2075 7365 642e 0d0a 2020 2020 2020  be used...      
-00019a20: 2020 6865 6967 6874 5f61 7869 7320 3a20    height_axis : 
-00019a30: 4178 6973 4c69 6b65 2c20 6f70 7469 6f6e  AxisLike, option
-00019a40: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-00019a50: 4178 6973 2074 6861 7420 7769 6c6c 2062  Axis that will b
-00019a60: 6520 7573 6564 2074 6f20 6c61 6265 6c20  e used to label 
-00019a70: 7468 6520 6e65 7720 6178 6973 2061 6674  the new axis aft
-00019a80: 6572 2072 6563 6f6e 7374 7275 6374 696f  er reconstructio
-00019a90: 6e2e 2046 6f72 0d0a 2020 2020 2020 2020  n. For..        
-00019aa0: 2020 2020 696e 7374 616e 6365 2c20 6966      instance, if
-00019ab0: 2069 6e70 7574 2069 6d61 6765 2068 6173   input image has
-00019ac0: 2061 7865 7320 6060 5b22 6465 6772 6565   axes ``["degree
-00019ad0: 222c 2022 7922 2c20 2278 225d 6060 2061  ", "y", "x"]`` a
-00019ae0: 6e64 200d 0a20 2020 2020 2020 2020 2020  nd ..           
-00019af0: 2060 6068 6569 6768 745f 6178 6973 3d22   ``height_axis="
-00019b00: 7a22 6060 2074 6865 6e20 7265 636f 6e73  z"`` then recons
-00019b10: 7472 7563 7465 6420 696d 6167 6520 7769  tructed image wi
-00019b20: 6c6c 2068 6176 6520 6178 6573 200d 0a20  ll have axes .. 
-00019b30: 2020 2020 2020 2020 2020 2060 605b 227a             ``["z
-00019b40: 222c 2022 7922 2c20 2278 225d 6060 2e20  ", "y", "x"]``. 
-00019b50: 4279 2064 6566 6175 6c74 2c20 2279 2220  By default, "y" 
-00019b60: 7769 6c6c 2062 6520 7573 6564 2066 6f72  will be used for
-00019b70: 2032 4420 696e 7075 7420 6f72 2022 7a22   2D input or "z"
-00019b80: 2066 6f72 0d0a 2020 2020 2020 2020 2020   for..          
-00019b90: 2020 3344 2069 6e70 7574 2e0d 0a20 2020    3D input...   
-00019ba0: 2020 2020 2068 6569 6768 7420 3a20 696e       height : in
-00019bb0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00019bc0: 2020 2020 2020 2020 2048 6569 6768 7420           Height 
-00019bd0: 6f66 2072 6563 6f6e 7374 7275 6374 696f  of reconstructio
-00019be0: 6e2e 2042 7920 6465 6661 756c 742c 2073  n. By default, s
-00019bf0: 697a 6520 6571 7561 6c20 746f 2074 6865  ize equal to the
-00019c00: 2061 7869 7320 7065 7270 656e 6469 6375   axis perpendicu
-00019c10: 6c61 720d 0a20 2020 2020 2020 2020 2020  lar..           
-00019c20: 2074 6f20 7468 6520 726f 7461 7469 6f6e   to the rotation
-00019c30: 2061 7869 7320 7769 6c6c 2062 6520 7573   axis will be us
-00019c40: 6564 2e0d 0a20 2020 2020 2020 2077 696e  ed...        win
-00019c50: 646f 7720 3a20 7374 722c 2064 6566 6175  dow : str, defau
-00019c60: 6c74 2069 7320 2268 616d 6d69 6e67 220d  lt is "hamming".
-00019c70: 0a20 2020 2020 2020 2020 2020 2057 696e  .            Win
-00019c80: 646f 7720 6675 6e63 7469 6f6e 2074 6861  dow function tha
-00019c90: 7420 7769 6c6c 2062 6520 6170 706c 6965  t will be applie
-00019ca0: 6420 746f 2074 6865 2046 6f75 7269 6572  d to the Fourier
-00019cb0: 2064 6f6d 6169 6e20 616c 6f6e 6720 7468   domain along th
-00019cc0: 6520 6178 6973 0d0a 2020 2020 2020 2020  e axis..        
-00019cd0: 2020 2020 7065 7270 656e 6469 6375 6c61      perpendicula
-00019ce0: 7220 746f 2074 6865 2072 6f74 6174 696f  r to the rotatio
-00019cf0: 6e20 6178 6973 2e0d 0a20 2020 2020 2020  n axis...       
-00019d00: 207b 6f72 6465 727d 0d0a 0d0a 2020 2020   {order}....    
-00019d10: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-00019d20: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-00019d30: 2020 2020 2020 496d 6741 7272 6179 0d0a        ImgArray..
-00019d40: 2020 2020 2020 2020 2020 2020 5265 636f              Reco
-00019d50: 6e73 7472 7563 7469 6f6e 2e0d 0a20 2020  nstruction...   
-00019d60: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019d70: 2020 2053 6565 2041 6c73 6f0d 0a20 2020     See Also..   
-00019d80: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-00019d90: 2020 2020 2020 2072 6164 6f6e 0d0a 2020         radon..  
-00019da0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00019db0: 2020 2069 6e74 6572 7020 3d20 7b30 3a20     interp = {0: 
-00019dc0: 226e 6561 7265 7374 222c 2031 3a20 226c  "nearest", 1: "l
-00019dd0: 696e 6561 7222 2c20 333a 2022 6375 6269  inear", 3: "cubi
-00019de0: 6322 7d5b 6f72 6465 725d 0d0a 2020 2020  c"}[order]..    
-00019df0: 2020 2020 6365 6e74 7261 6c5f 6178 6973      central_axis
-00019e00: 2c20 6465 6772 6565 5f61 7869 732c 206f  , degree_axis, o
-00019e10: 7574 7075 745f 7368 6170 652c 206e 6577  utput_shape, new
-00019e20: 5f61 7865 7320 3d20 5f74 7261 6e73 666f  _axes = _transfo
-00019e30: 726d 2e6e 6f72 6d61 6c69 7a65 5f69 7261  rm.normalize_ira
-00019e40: 646f 6e5f 696e 7075 7428 0d0a 2020 2020  don_input(..    
-00019e50: 2020 2020 2020 2020 7365 6c66 2c20 6365          self, ce
-00019e60: 6e74 7261 6c5f 6178 6973 2c20 6865 6967  ntral_axis, heig
-00019e70: 6874 5f61 7869 732c 2064 6567 7265 655f  ht_axis, degree_
-00019e80: 6178 6973 2c20 6865 6967 6874 0d0a 2020  axis, height..  
-00019e90: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00019ea0: 2073 656c 663a 2049 6d67 4172 7261 7920   self: ImgArray 
-00019eb0: 3d20 6e70 2e6d 6f76 6561 7869 7328 7365  = np.moveaxis(se
-00019ec0: 6c66 2c20 7365 6c66 2e61 7869 736f 6628  lf, self.axisof(
-00019ed0: 6465 6772 6565 5f61 7869 7329 2c20 2d31  degree_axis), -1
-00019ee0: 290d 0a20 2020 2020 2020 2066 696c 7465  )..        filte
-00019ef0: 725f 6675 6e63 203d 205f 7472 616e 7366  r_func = _transf
-00019f00: 6f72 6d2e 6765 745f 666f 7572 6965 725f  orm.get_fourier_
-00019f10: 6669 6c74 6572 2873 656c 662e 7368 6170  filter(self.shap
-00019f20: 655b 2d32 5d2c 2077 696e 646f 7729 0d0a  e[-2], window)..
-00019f30: 2020 2020 2020 2020 6f75 7420 3d20 7365          out = se
-00019f40: 6c66 2e5f 6170 706c 795f 6461 736b 280d  lf._apply_dask(.
-00019f50: 0a20 2020 2020 2020 2020 2020 205f 7472  .            _tr
-00019f60: 616e 7366 6f72 6d2e 6972 6164 6f6e 2c0d  ansform.iradon,.
-00019f70: 0a20 2020 2020 2020 2020 2020 2063 5f61  .            c_a
-00019f80: 7865 733d 5b63 656e 7472 616c 5f61 7869  xes=[central_axi
-00019f90: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00019fa0: 206b 7761 7267 733d 6469 6374 280d 0a20   kwargs=dict(.. 
-00019fb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00019fc0: 6567 7265 6573 3d64 6567 7265 6573 2c0d  egrees=degrees,.
-00019fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019fe0: 2069 6e74 6572 706f 6c61 7469 6f6e 3d69   interpolation=i
-00019ff0: 6e74 6572 702c 0d0a 2020 2020 2020 2020  nterp,..        
-0001a000: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
-0001a010: 756e 633d 6669 6c74 6572 5f66 756e 632c  unc=filter_func,
-0001a020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a030: 2020 6f75 7470 7574 5f73 6861 7065 3d6f    output_shape=o
-0001a040: 7574 7075 745f 7368 6170 652c 0d0a 2020  utput_shape,..  
-0001a050: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001a060: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001a070: 0d0a 2020 2020 2020 2020 6966 206f 7574  ..        if out
-0001a080: 2e6e 6469 6d20 3d3d 2033 3a0d 0a20 2020  .ndim == 3:..   
-0001a090: 2020 2020 2020 2020 206f 7574 203d 206e           out = n
-0001a0a0: 702e 6d6f 7665 6178 6973 286f 7574 2c20  p.moveaxis(out, 
-0001a0b0: 302c 2031 290d 0a20 2020 2020 2020 206f  0, 1)..        o
-0001a0c0: 7574 203d 206f 7574 5b3a 3a2d 315d 0d0a  ut = out[::-1]..
-0001a0d0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0001a0e0: 7574 2e5f 7365 745f 696e 666f 2873 656c  ut._set_info(sel
-0001a0f0: 662c 206e 6577 5f61 7865 7329 0d0a 0d0a  f, new_axes)....
-0001a100: 2020 2020 4063 6865 636b 5f69 6e70 7574      @check_input
-0001a110: 5f61 6e64 5f6f 7574 7075 740d 0a20 2020  _and_output..   
-0001a120: 2064 6566 2074 6872 6573 686f 6c64 280d   def threshold(.
-0001a130: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001a140: 2020 2020 2020 2020 7468 723a 2066 6c6f          thr: flo
-0001a150: 6174 207c 2073 7472 207c 2054 6872 6561  at | str | Threa
-0001a160: 7368 6f6c 644d 6574 686f 6420 3d20 226f  sholdMethod = "o
-0001a170: 7473 7522 2c0d 0a20 2020 2020 2020 202a  tsu",..        *
-0001a180: 2c0d 0a20 2020 2020 2020 2061 6c6f 6e67  ,..        along
-0001a190: 3a20 4178 6973 4c69 6b65 207c 204e 6f6e  : AxisLike | Non
-0001a1a0: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
-0001a1b0: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-0001a1c0: 2029 202d 3e20 496d 6741 7272 6179 3a0d   ) -> ImgArray:.
-0001a1d0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0001a1e0: 2020 2020 2020 4170 706c 7920 7468 7265        Apply thre
-0001a1f0: 7368 6f6c 6469 6e67 2074 6f20 7468 6520  sholding to the 
-0001a200: 696d 6167 6520 616e 6420 6372 6561 7465  image and create
-0001a210: 2061 2062 696e 6172 7920 696d 6167 652e   a binary image.
-0001a220: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0001a230: 2020 2020 5468 6520 7468 7265 7368 6f6c      The threshol
-0001a240: 6420 7661 6c75 6520 6361 6e20 6265 2067  d value can be g
-0001a250: 6976 656e 2077 6974 6820 6120 666c 6f61  iven with a floa
-0001a260: 7420 6f72 2061 2073 7472 696e 6720 7468  t or a string th
-0001a270: 6174 2069 6e64 6963 6174 6573 2077 6861  at indicates wha
-0001a280: 740d 0a20 2020 2020 2020 2074 6872 6573  t..        thres
-0001a290: 686f 6c64 696e 6720 6d65 7468 6f64 2077  holding method w
-0001a2a0: 696c 6c20 6265 2075 7365 642e 0d0a 2020  ill be used...  
-0001a2b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a2c0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0001a2d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-0001a2e0: 2020 2020 2020 2020 7468 723a 2066 6c6f          thr: flo
-0001a2f0: 6174 206f 7220 7374 722c 206f 7074 696f  at or str, optio
-0001a300: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-0001a310: 2054 6872 6573 686f 6c64 2076 616c 7565   Threshold value
-0001a320: 2c20 7065 7263 656e 7461 6765 206f 7220  , percentage or 
-0001a330: 7468 7265 7368 6f6c 6469 6e67 2061 6c67  thresholding alg
-0001a340: 6f72 6974 686d 2e0d 0a20 2020 2020 2020  orithm...       
-0001a350: 2061 6c6f 6e67 203a 2041 7869 734c 696b   along : AxisLik
-0001a360: 652c 206f 7074 696f 6e61 6c0d 0a20 2020  e, optional..   
-0001a370: 2020 2020 2020 2020 2044 696d 656e 7369           Dimensi
-0001a380: 6f6e 7320 7468 6174 2077 696c 6c20 6e6f  ons that will no
-0001a390: 7420 7368 6172 6520 7468 6520 7361 6d65  t share the same
-0001a3a0: 2074 6872 6573 686f 6c64 2e20 466f 7220   threshold. For 
-0001a3b0: 696e 7374 616e 6365 2c20 6966 0d0a 2020  instance, if..  
-0001a3c0: 2020 2020 2020 2020 2020 6060 616c 6f6e            ``alon
-0001a3d0: 673d 2263 2260 6020 7468 656e 2074 6872  g="c"`` then thr
-0001a3e0: 6573 686f 6c64 2069 6e74 656e 7369 7469  eshold intensiti
-0001a3f0: 6573 2061 7265 2064 6574 6572 6d69 6e65  es are determine
-0001a400: 6420 666f 7220 6576 6572 7920 6368 616e  d for every chan
-0001a410: 6e65 6c2e 0d0a 2020 2020 2020 2020 2020  nel...          
-0001a420: 2020 4966 2060 6074 6872 6060 2069 7320    If ``thr`` is 
-0001a430: 666c 6f61 742c 2060 6061 6c6f 6e67 6060  float, ``along``
-0001a440: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
-0001a450: 2e0d 0a20 2020 2020 2020 202a 2a6b 7761  ...        **kwa
-0001a460: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-0001a470: 2020 4b65 7977 6f72 6420 6172 6775 6d65    Keyword argume
-0001a480: 6e74 7320 7468 6174 2077 696c 6c20 7061  nts that will pa
-0001a490: 7373 6564 2074 6f20 6675 6e63 7469 6f6e  ssed to function
-0001a4a0: 2069 6e64 6963 6174 6564 2069 6e20 276d   indicated in 'm
-0001a4b0: 6574 686f 6427 2e0d 0a0d 0a20 2020 2020  ethod'.....     
-0001a4c0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-0001a4d0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-0001a4e0: 2020 2020 2049 6d67 4172 7261 790d 0a20       ImgArray.. 
-0001a4f0: 2020 2020 2020 2020 2020 2042 6f6f 6c69             Booli
-0001a500: 616e 2061 7272 6179 2e0d 0a20 2020 2020  an array...     
-0001a510: 2020 200d 0a20 2020 2020 2020 2045 7861     ..        Exa
-0001a520: 6d70 6c65 730d 0a20 2020 2020 2020 202d  mples..        -
-0001a530: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0001a540: 2053 7562 7374 6974 7574 6520 6f75 746c   Substitute outl
-0001a550: 6965 7273 2074 6f20 302e 0d0a 2020 2020  iers to 0...    
-0001a560: 2020 2020 2020 2020 3e3e 3e20 7468 7220          >>> thr 
-0001a570: 3d20 696d 672e 7468 7265 7368 6f6c 6428  = img.threshold(
-0001a580: 2239 3925 2229 0d0a 2020 2020 2020 2020  "99%")..        
-0001a590: 2020 2020 3e3e 3e20 696d 675b 7468 725d      >>> img[thr]
-0001a5a0: 203d 2030 0d0a 2020 2020 2020 2020 2222   = 0..        ""
-0001a5b0: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
-0001a5c0: 6c66 2e64 7479 7065 203d 3d20 626f 6f6c  lf.dtype == bool
-0001a5d0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001a5e0: 6574 7572 6e20 7365 6c66 0d0a 2020 2020  eturn self..    
-0001a5f0: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-0001a600: 2061 6c6f 6e67 2069 7320 4e6f 6e65 3a0d   along is None:.
-0001a610: 0a20 2020 2020 2020 2020 2020 2061 6c6f  .            alo
-0001a620: 6e67 203d 2022 6322 2069 6620 2263 2220  ng = "c" if "c" 
-0001a630: 696e 2073 656c 662e 6178 6573 2065 6c73  in self.axes els
-0001a640: 6520 2222 0d0a 0d0a 2020 2020 2020 2020  e ""....        
-0001a650: 6d65 7468 6f64 735f 203d 207b 2269 736f  methods_ = {"iso
-0001a660: 6461 7461 223a 2073 6b66 696c 2e74 6872  data": skfil.thr
-0001a670: 6573 686f 6c64 5f69 736f 6461 7461 2c0d  eshold_isodata,.
-0001a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a690: 2020 2020 2022 6c69 223a 2073 6b66 696c       "li": skfil
-0001a6a0: 2e74 6872 6573 686f 6c64 5f6c 692c 0d0a  .threshold_li,..
-0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6c0: 2020 2020 226c 6f63 616c 223a 2073 6b66      "local": skf
-0001a6d0: 696c 2e74 6872 6573 686f 6c64 5f6c 6f63  il.threshold_loc
-0001a6e0: 616c 2c0d 0a20 2020 2020 2020 2020 2020  al,..           
-0001a6f0: 2020 2020 2020 2020 2022 6d65 616e 223a           "mean":
-0001a700: 2073 6b66 696c 2e74 6872 6573 686f 6c64   skfil.threshold
-0001a710: 5f6d 6561 6e2c 0d0a 2020 2020 2020 2020  _mean,..        
-0001a720: 2020 2020 2020 2020 2020 2020 226d 696e              "min
+000188b0: 626f 6f6c 203d 2046 616c 7365 2c20 0d0a  bool = False, ..
+000188c0: 2020 2020 2020 2020 2a2c 0d0a 2020 2020          *,..    
+000188d0: 2020 2020 7368 6966 743a 2062 6f6f 6c20      shift: bool 
+000188e0: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+000188f0: 2064 6f75 626c 655f 7072 6563 6973 696f   double_precisio
+00018900: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
+00018910: 0d0a 2020 2020 2020 2020 6469 6d73 3a20  ..        dims: 
+00018920: 4469 6d73 203d 204e 6f6e 650d 0a20 2020  Dims = None..   
+00018930: 2029 202d 3e20 496d 6741 7272 6179 3a0d   ) -> ImgArray:.
+00018940: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00018950: 2020 2020 2020 5265 7475 726e 206e 2d44        Return n-D
+00018960: 2070 6f77 6572 2073 7065 6374 7261 206f   power spectra o
+00018970: 6620 696d 6167 6573 2c20 7768 6963 6820  f images, which 
+00018980: 6973 2064 6566 696e 6564 2061 733a 0d0a  is defined as:..
+00018990: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000189a0: 2020 2e2e 206d 6174 683a 3a0d 0a20 2020    .. math::..   
+000189b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000189c0: 2020 2050 203d 2052 6528 465b 495f 7b69     P = Re(F[I_{i
+000189d0: 6d67 7d5d 295e 3220 2b20 496d 2846 5b49  mg}])^2 + Im(F[I
+000189e0: 5f7b 696d 677d 5d29 5e32 0d0a 0d0a 2020  _{img}])^2....  
+000189f0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00018a00: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00018a10: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7368  ----..        sh
+00018a20: 6170 6520 3a20 696e 742c 2069 7465 7261  ape : int, itera
+00018a30: 626c 6520 6f66 2069 6e74 2c20 2273 7175  ble of int, "squ
+00018a40: 6172 6522 206f 7220 2273 616d 6522 0d0a  are" or "same"..
+00018a50: 2020 2020 2020 2020 2020 2020 4f75 7470              Outp
+00018a60: 7574 2073 6861 7065 2e20 496e 7075 7420  ut shape. Input 
+00018a70: 696d 6167 6520 6973 2070 6164 6465 6420  image is padded 
+00018a80: 6f72 2063 726f 7070 6564 2061 6363 6f72  or cropped accor
+00018a90: 6469 6e67 2074 6f20 7468 6973 2076 616c  ding to this val
+00018aa0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00018ab0: 202d 2069 6e74 6567 6572 733a 2070 6164   - integers: pad
+00018ac0: 6465 6420 6f72 2063 726f 7070 6564 2074  ded or cropped t
+00018ad0: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
+00018ae0: 7368 6170 652e 0d0a 2020 2020 2020 2020  shape...        
+00018af0: 2020 2020 2d20 2273 7175 6172 6522 3a20      - "square": 
+00018b00: 7061 6464 6564 2074 6f20 736d 616c 6c65  padded to smalle
+00018b10: 7374 2032 5e4e 2d6c 6f6e 6720 7371 7561  st 2^N-long squa
+00018b20: 7265 2e0d 0a20 2020 2020 2020 2020 2020  re...           
+00018b30: 202d 2022 7361 6d65 2220 2864 6566 6175   - "same" (defau
+00018b40: 6c74 293a 206e 6f20 7061 6464 696e 6720  lt): no padding 
+00018b50: 6f72 2063 726f 7070 696e 672e 0d0a 2020  or cropping...  
+00018b60: 2020 2020 2020 6e6f 726d 203a 2062 6f6f        norm : boo
+00018b70: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+00018b80: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00018b90: 2049 6620 5472 7565 2c20 6d61 7869 6d75   If True, maximu
+00018ba0: 6d20 7661 6c75 6520 6f66 2070 6f77 6572  m value of power
+00018bb0: 2073 7065 6374 7261 2069 7320 6164 6a75   spectra is adju
+00018bc0: 7374 6564 2074 6f20 312e 0d0a 2020 2020  sted to 1...    
+00018bd0: 2020 2020 7b64 6f75 626c 655f 7072 6563      {double_prec
+00018be0: 6973 696f 6e7d 0d0a 2020 2020 2020 2020  ision}..        
+00018bf0: 7368 6966 7420 3a20 626f 6f6c 2c20 6465  shift : bool, de
+00018c00: 6661 756c 7420 6973 2054 7275 650d 0a20  fault is True.. 
+00018c10: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+00018c20: 7565 2c20 6361 6c6c 2060 606e 702e 6666  ue, call ``np.ff
+00018c30: 742e 6666 7473 6869 6674 6060 2061 7420  t.fftshift`` at 
+00018c40: 7468 6520 6669 7273 742e 0d0a 2020 2020  the first...    
+00018c50: 2020 2020 7b64 696d 737d 0d0a 0d0a 2020      {dims}....  
+00018c60: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+00018c70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+00018c80: 2020 2020 2020 2020 496d 6741 7272 6179          ImgArray
+00018c90: 0d0a 2020 2020 2020 2020 2020 2020 506f  ..            Po
+00018ca0: 7765 7220 7370 6563 7472 610d 0a20 2020  wer spectra..   
+00018cb0: 2020 2020 200d 0a20 2020 2020 2020 2053       ..        S
+00018cc0: 6565 2041 6c73 6f0d 0a20 2020 2020 2020  ee Also..       
+00018cd0: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
+00018ce0: 2020 206c 6f63 616c 5f70 6f77 6572 5f73     local_power_s
+00018cf0: 7065 6374 7261 0d0a 2020 2020 2020 2020  pectra..        
+00018d00: 2222 2220 2020 2020 2020 200d 0a20 2020  """        ..   
+00018d10: 2020 2020 2066 7265 7120 3d20 7365 6c66       freq = self
+00018d20: 2e66 6674 2864 696d 733d 6469 6d73 2c20  .fft(dims=dims, 
+00018d30: 7368 6170 653d 7368 6170 652c 2073 6869  shape=shape, shi
+00018d40: 6674 3d73 6869 6674 2c20 646f 7562 6c65  ft=shift, double
+00018d50: 5f70 7265 6369 7369 6f6e 3d64 6f75 626c  _precision=doubl
+00018d60: 655f 7072 6563 6973 696f 6e29 0d0a 2020  e_precision)..  
+00018d70: 2020 2020 2020 7077 203d 2066 7265 712e        pw = freq.
+00018d80: 7265 616c 2a2a 3220 2b20 6672 6571 2e69  real**2 + freq.i
+00018d90: 6d61 672a 2a32 0d0a 2020 2020 2020 2020  mag**2..        
+00018da0: 6966 206e 6f72 6d3a 0d0a 2020 2020 2020  if norm:..      
+00018db0: 2020 2020 2020 7077 202f 3d20 7077 2e6d        pw /= pw.m
+00018dc0: 6178 2829 0d0a 2020 2020 2020 2020 7077  ax()..        pw
+00018dd0: 3a20 496d 6741 7272 6179 0d0a 2020 2020  : ImgArray..    
+00018de0: 2020 2020 6966 207a 6572 6f5f 6e6f 726d      if zero_norm
+00018df0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00018e00: 6c20 3d20 7377 6974 6368 5f73 6c69 6365  l = switch_slice
+00018e10: 2864 696d 732c 2070 772e 6178 6573 2c20  (dims, pw.axes, 
+00018e20: 6966 696e 3d6e 702e 6172 7261 7928 7077  ifin=np.array(pw
+00018e30: 2e73 6861 7065 292f 2f32 2c20 6966 6e6f  .shape)//2, ifno
+00018e40: 743d 736c 6963 6528 4e6f 6e65 2929 0d0a  t=slice(None))..
+00018e50: 2020 2020 2020 2020 2020 2020 7077 5b73              pw[s
+00018e60: 6c5d 203d 2030 0d0a 2020 2020 2020 2020  l] = 0..        
+00018e70: 7265 7475 726e 2070 770d 0a0d 0a20 2020  return pw....   
+00018e80: 2040 5f64 6f63 732e 7772 6974 655f 646f   @_docs.write_do
+00018e90: 6373 0d0a 2020 2020 4064 696d 735f 746f  cs..    @dims_to
+00018ea0: 5f73 7061 7469 616c 5f61 7865 730d 0a20  _spatial_axes.. 
+00018eb0: 2020 2064 6566 2072 6164 6f6e 280d 0a20     def radon(.. 
+00018ec0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+00018ed0: 2020 2020 2020 6465 6772 6565 733a 2066        degrees: f
+00018ee0: 6c6f 6174 207c 2049 7465 7261 626c 655b  loat | Iterable[
+00018ef0: 666c 6f61 745d 2c20 0d0a 2020 2020 2020  float], ..      
+00018f00: 2020 2a2c 0d0a 2020 2020 2020 2020 6365    *,..        ce
+00018f10: 6e74 7261 6c5f 6178 6973 3a20 4178 6973  ntral_axis: Axis
+00018f20: 4c69 6b65 207c 2053 6571 7565 6e63 655b  Like | Sequence[
+00018f30: 666c 6f61 745d 207c 204e 6f6e 6520 3d20  float] | None = 
+00018f40: 4e6f 6e65 2c0d 0a20 2020 2020 2020 206f  None,..        o
+00018f50: 7264 6572 3a20 696e 7420 3d20 332c 0d0a  rder: int = 3,..
+00018f60: 2020 2020 2020 2020 6469 6d73 3a20 4469          dims: Di
+00018f70: 6d73 203d 204e 6f6e 652c 0d0a 2020 2020  ms = None,..    
+00018f80: 2920 2d3e 2049 6d67 4172 7261 793a 0d0a  ) -> ImgArray:..
+00018f90: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00018fa0: 2020 2020 2044 6973 6372 6574 6520 5261       Discrete Ra
+00018fb0: 646f 6e20 7472 616e 7366 6f72 6d61 7469  don transformati
+00018fc0: 6f6e 206f 6620 3244 206f 7220 3344 2069  on of 2D or 3D i
+00018fd0: 6d61 6765 2e0d 0a20 2020 2020 2020 200d  mage...        .
+00018fe0: 0a20 2020 2020 2020 2052 6164 6f6e 2074  .        Radon t
+00018ff0: 7261 6e73 666f 726d 6174 696f 6e20 6973  ransformation is
+00019000: 2061 206c 6973 7420 6f66 2070 726f 6a65   a list of proje
+00019010: 6374 696f 6e20 6f66 2061 2073 616d 6520  ction of a same 
+00019020: 696d 6167 6520 6672 6f6d 2064 6966 6665  image from diffe
+00019030: 7265 6e74 2061 6e67 6c65 732e 0d0a 2020  rent angles...  
+00019040: 2020 2020 2020 4974 2067 656e 6572 6174        It generat
+00019050: 6573 2074 6f6d 6f67 7261 7068 6963 206e  es tomographic n
+00019060: 2d44 2069 6d61 6765 2073 6c69 6365 7320  -D image slices 
+00019070: 6672 6f6d 2028 6e2b 3129 2d44 2069 6d61  from (n+1)-D ima
+00019080: 6765 2e0d 0a0d 0a20 2020 2020 2020 2050  ge.....        P
+00019090: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+000190a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+000190b0: 2020 2020 2020 2064 6567 7265 6573 203a         degrees :
+000190c0: 2066 6c6f 6174 206f 7220 6974 6572 6162   float or iterab
+000190d0: 6c65 206f 6620 666c 6f61 740d 0a20 2020  le of float..   
+000190e0: 2020 2020 2020 2020 2052 6f74 6174 696f           Rotatio
+000190f0: 6e20 616e 676c 6573 2061 726f 756e 6420  n angles around 
+00019100: 7468 6520 6365 6e74 7261 6c20 6178 6973  the central axis
+00019110: 2069 6e20 6465 6772 6565 732e 0d0a 2020   in degrees...  
+00019120: 2020 2020 2020 6365 6e74 7261 6c5f 6178        central_ax
+00019130: 6973 203a 2061 7869 732d 6c69 6b65 206f  is : axis-like o
+00019140: 7220 7365 7175 656e 6365 206f 6620 666c  r sequence of fl
+00019150: 6f61 742c 206f 7074 696f 6e61 6c0d 0a20  oat, optional.. 
+00019160: 2020 2020 2020 2020 2020 2056 6563 746f             Vecto
+00019170: 7220 7468 6174 2064 6566 696e 6573 2074  r that defines t
+00019180: 6865 2063 656e 7472 616c 2061 7869 7320  he central axis 
+00019190: 6f66 2072 6f74 6174 696f 6e2e 0d0a 2020  of rotation...  
+000191a0: 2020 2020 2020 7b6f 7264 6572 7d7b 6469        {order}{di
+000191b0: 6d73 7d0d 0a0d 0a20 2020 2020 2020 2052  ms}....        R
+000191c0: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+000191d0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+000191e0: 2049 6d67 4172 7261 790d 0a20 2020 2020   ImgArray..     
+000191f0: 2020 2020 2020 2054 6f6d 6f67 7261 7068         Tomograph
+00019200: 6963 2069 6d61 6765 2073 6c69 6365 732e  ic image slices.
+00019210: 2054 6865 2066 6972 7374 2073 7061 7469   The first spati
+00019220: 616c 2061 7869 7320 2822 7a22 2066 6f72  al axis ("z" for
+00019230: 207a 7978 2d69 6d61 6765 2920 7769 6c6c   zyx-image) will
+00019240: 2062 6520 6472 6f70 7065 642e 0d0a 2020   be dropped...  
+00019250: 2020 2020 2020 2020 2020 4966 2073 6571            If seq
+00019260: 7565 6e63 6520 6f66 2066 6c6f 6174 2069  uence of float i
+00019270: 7320 6769 7665 6e20 6173 2060 6064 6567  s given as ``deg
+00019280: 7265 6573 6060 2c20 2264 6567 7265 6522  rees``, "degree"
+00019290: 2061 7869 7320 7769 6c6c 2062 6520 6e65   axis will be ne
+000192a0: 776c 7920 6164 6465 6420 6174 0d0a 2020  wly added at..  
+000192b0: 2020 2020 2020 2020 2020 7468 6520 706f            the po
+000192c0: 7369 7469 6f6e 2030 2e20 466f 7220 696e  sition 0. For in
+000192d0: 7374 616e 6365 2c20 6966 2061 207a 7978  stance, if a zyx
+000192e0: 2d69 6d61 6765 2061 6e64 2060 6064 6567  -image and ``deg
+000192f0: 7265 6573 3d6e 702e 6c69 6e73 7061 6365  rees=np.linspace
+00019300: 2830 2c20 3138 302c 2031 3030 2960 600d  (0, 180, 100)``.
+00019310: 0a20 2020 2020 2020 2020 2020 2061 7265  .            are
+00019320: 2067 6976 656e 2c20 7265 7475 726e 6564   given, returned
+00019330: 2069 6d61 6765 2068 6173 2061 7865 7320   image has axes 
+00019340: 5b22 6465 6772 6565 222c 2022 7922 2c20  ["degree", "y", 
+00019350: 2278 225d 2e0d 0a20 2020 2020 2020 200d  "x"]...        .
+00019360: 0a20 2020 2020 2020 2053 6565 2041 6c73  .        See Als
+00019370: 6f0d 0a20 2020 2020 2020 202d 2d2d 2d2d  o..        -----
+00019380: 2d2d 2d0d 0a20 2020 2020 2020 2069 7261  ---..        ira
+00019390: 646f 6e0d 0a20 2020 2020 2020 2022 2222  don..        """
+000193a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000193b0: 2020 6672 6f6d 2064 6173 6b20 696d 706f    from dask impo
+000193c0: 7274 2061 7272 6179 2061 7320 6461 2c20  rt array as da, 
+000193d0: 6465 6c61 7965 640d 0a20 2020 2020 2020  delayed..       
+000193e0: 200d 0a20 2020 2020 2020 2070 6172 616d   ..        param
+000193f0: 732c 206f 7574 7075 745f 7368 6170 652c  s, output_shape,
+00019400: 2073 7175 6565 7a65 203d 205f 7472 616e   squeeze = _tran
+00019410: 7366 6f72 6d2e 6e6f 726d 616c 697a 655f  sform.normalize_
+00019420: 7261 646f 6e5f 696e 7075 7428 0d0a 2020  radon_input(..  
+00019430: 2020 2020 2020 2020 2020 7365 6c66 2c20            self, 
+00019440: 6469 6d73 2c20 6365 6e74 7261 6c5f 6178  dims, central_ax
+00019450: 6973 2c20 6465 6772 6565 730d 0a20 2020  is, degrees..   
+00019460: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00019470: 0d0a 2020 2020 2020 2020 2320 6170 706c  ..        # appl
+00019480: 7920 7370 6c69 6e65 2066 696c 7465 7220  y spline filter 
+00019490: 696e 2061 6476 616e 6365 2e0d 0a20 2020  in advance...   
+000194a0: 2020 2020 2069 6e70 7574 203d 2073 656c       input = sel
+000194b0: 662e 6173 5f66 6c6f 6174 2829 2e73 706c  f.as_float().spl
+000194c0: 696e 655f 6669 6c74 6572 286f 7264 6572  ine_filter(order
+000194d0: 3d6f 7264 6572 290d 0a20 2020 2020 2020  =order)..       
+000194e0: 2064 656c 6179 6564 5f66 756e 6320 3d20   delayed_func = 
+000194f0: 6465 6c61 7965 6428 5f74 7261 6e73 666f  delayed(_transfo
+00019500: 726d 2e72 6164 6f6e 5f73 696e 676c 6529  rm.radon_single)
+00019510: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
+00019520: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+00019530: 2064 656c 6179 6564 5f66 756e 6328 696e   delayed_func(in
+00019540: 7075 742c 2070 2c20 6f72 6465 723d 6f72  put, p, order=or
+00019550: 6465 722c 206f 7574 7075 745f 7368 6170  der, output_shap
+00019560: 653d 6f75 7470 7574 5f73 6861 7065 2920  e=output_shape) 
+00019570: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00019580: 7220 7020 696e 2070 6172 616d 730d 0a20  r p in params.. 
+00019590: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+000195a0: 2020 6f75 7420 3d20 7870 2e73 7461 636b    out = xp.stack
+000195b0: 2864 612e 636f 6d70 7574 6528 7461 736b  (da.compute(task
+000195c0: 7329 5b30 5d2c 2061 7869 733d 3029 0d0a  s)[0], axis=0)..
+000195d0: 0d0a 2020 2020 2020 2020 6f75 7420 3d20  ..        out = 
+000195e0: 7870 2e61 736e 756d 7079 286f 7574 292e  xp.asnumpy(out).
+000195f0: 7669 6577 2873 656c 662e 5f5f 636c 6173  view(self.__clas
+00019600: 735f 5f29 0d0a 2020 2020 2020 2020 6f75  s__)..        ou
+00019610: 742e 5f73 6574 5f69 6e66 6f28 7365 6c66  t._set_info(self
+00019620: 2c20 7365 6c66 2e61 7865 732e 6472 6f70  , self.axes.drop
+00019630: 2830 292e 696e 7365 7274 2830 2c20 2264  (0).insert(0, "d
+00019640: 6567 7265 6522 2929 0d0a 2020 2020 2020  egree"))..      
+00019650: 2020 6f75 742e 6178 6573 5b30 5d2e 6c61    out.axes[0].la
+00019660: 6265 6c73 203d 206c 6973 7428 6465 6772  bels = list(degr
+00019670: 6565 7329 0d0a 2020 2020 2020 2020 6966  ees)..        if
+00019680: 2073 7175 6565 7a65 3a0d 0a20 2020 2020   squeeze:..     
+00019690: 2020 2020 2020 206f 7574 203d 206f 7574         out = out
+000196a0: 5b30 5d0d 0a20 2020 2020 2020 2072 6574  [0]..        ret
+000196b0: 7572 6e20 6f75 740d 0a20 2020 200d 0a20  urn out..    .. 
+000196c0: 2020 2040 5f64 6f63 732e 7772 6974 655f     @_docs.write_
+000196d0: 646f 6373 0d0a 2020 2020 6465 6620 6972  docs..    def ir
+000196e0: 6164 6f6e 280d 0a20 2020 2020 2020 2073  adon(..        s
+000196f0: 656c 662c 0d0a 2020 2020 2020 2020 6465  elf,..        de
+00019700: 6772 6565 733a 2053 6571 7565 6e63 655b  grees: Sequence[
+00019710: 666c 6f61 745d 2c0d 0a20 2020 2020 2020  float],..       
+00019720: 202a 2c0d 0a20 2020 2020 2020 2063 656e   *,..        cen
+00019730: 7472 616c 5f61 7869 733a 2041 7869 734c  tral_axis: AxisL
+00019740: 696b 6520 3d20 2279 222c 0d0a 2020 2020  ike = "y",..    
+00019750: 2020 2020 6465 6772 6565 5f61 7869 733a      degree_axis:
+00019760: 2041 7869 734c 696b 6520 7c20 4e6f 6e65   AxisLike | None
+00019770: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00019780: 2020 6865 6967 6874 5f61 7869 733a 2041    height_axis: A
+00019790: 7869 734c 696b 6520 7c20 4e6f 6e65 203d  xisLike | None =
+000197a0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000197b0: 6865 6967 6874 3a20 696e 7420 7c20 4e6f  height: int | No
+000197c0: 6e65 203d 204e 6f6e 652c 0d0a 2020 2020  ne = None,..    
+000197d0: 2020 2020 7769 6e64 6f77 3a20 7374 7220      window: str 
+000197e0: 3d20 2268 616d 6d69 6e67 222c 0d0a 2020  = "hamming",..  
+000197f0: 2020 2020 2020 6f72 6465 723a 2069 6e74        order: int
+00019800: 203d 2033 2c0d 0a20 2020 2029 202d 3e20   = 3,..    ) -> 
+00019810: 496d 6741 7272 6179 3a0d 0a20 2020 2020  ImgArray:..     
+00019820: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00019830: 496e 7665 7273 6520 5261 646f 6e20 7472  Inverse Radon tr
+00019840: 616e 7366 6f72 6d61 7469 6f6e 2028 7765  ansformation (we
+00019850: 6967 6874 6564 2062 6163 6b20 7072 6f6a  ighted back proj
+00019860: 6563 7469 6f6e 2920 6f66 2061 2074 696c  ection) of a til
+00019870: 6520 7365 7269 6573 2e0d 0a20 2020 2020  e series...     
+00019880: 2020 200d 0a20 2020 2020 2020 2049 6e70     ..        Inp
+00019890: 7574 2061 7272 6179 206d 7573 7420 6265  ut array must be
+000198a0: 2061 2074 696c 7420 7365 7269 6573 206f   a tilt series o
+000198b0: 6620 3144 206f 7220 3244 2069 6d61 6765  f 1D or 2D image
+000198c0: 732e 2054 6865 7920 6172 6520 6261 636b  s. They are back
+000198d0: 2d0d 0a20 2020 2020 2020 2070 726f 6a65  -..        proje
+000198e0: 6374 6564 2069 6e74 6f20 6120 3244 206f  cted into a 2D o
+000198f0: 7220 3344 2069 6d61 6765 2077 6974 6820  r 3D image with 
+00019900: 6172 6269 7472 6172 7920 6865 6967 6874  arbitrary height
+00019910: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00019920: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+00019930: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00019940: 2020 2020 2064 6567 7265 6573 203a 2073       degrees : s
+00019950: 6571 7565 6e63 6520 6f66 2066 6c6f 6174  equence of float
+00019960: 0d0a 2020 2020 2020 2020 2020 2020 5072  ..            Pr
+00019970: 6f6a 6563 7469 6f6e 2061 6e67 6c65 7320  ojection angles 
+00019980: 696e 2064 6567 7265 652e 204c 656e 6774  in degree. Lengt
+00019990: 6820 6d75 7374 206d 6174 6368 2074 6865  h must match the
+000199a0: 206c 656e 6774 6820 6f66 2074 6865 2064   length of the d
+000199b0: 6567 7265 650d 0a20 2020 2020 2020 2020  egree..         
+000199c0: 2020 2061 7869 7320 6f66 2074 6865 2069     axis of the i
+000199d0: 6e70 7574 2069 6d61 6765 2e0d 0a20 2020  nput image...   
+000199e0: 2020 2020 2063 656e 7472 616c 5f61 7869       central_axi
+000199f0: 7320 3a20 4178 6973 4c69 6b65 2c20 6f70  s : AxisLike, op
+00019a00: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00019a10: 2020 2020 4178 6973 2070 6172 616c 6c65      Axis paralle
+00019a20: 6c20 746f 2074 6865 2072 6f74 6174 696f  l to the rotatio
+00019a30: 6e20 6178 6973 2e0d 0a20 2020 2020 2020  n axis...       
+00019a40: 2064 6567 7265 655f 6178 6973 203a 2041   degree_axis : A
+00019a50: 7869 734c 696b 652c 206f 7074 696f 6e61  xisLike, optiona
+00019a60: 6c0d 0a20 2020 2020 2020 2020 2020 2041  l..            A
+00019a70: 7869 7320 6f66 2072 6f74 6174 696f 6e20  xis of rotation 
+00019a80: 6465 6772 6565 2e20 4279 2064 6566 6175  degree. By defau
+00019a90: 6c74 2c20 7468 6520 6669 7273 7420 6178  lt, the first ax
+00019aa0: 6973 2077 696c 6c20 6265 2075 7365 642e  is will be used.
+00019ab0: 0d0a 2020 2020 2020 2020 6865 6967 6874  ..        height
+00019ac0: 5f61 7869 7320 3a20 4178 6973 4c69 6b65  _axis : AxisLike
+00019ad0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00019ae0: 2020 2020 2020 2020 4178 6973 2074 6861          Axis tha
+00019af0: 7420 7769 6c6c 2062 6520 7573 6564 2074  t will be used t
+00019b00: 6f20 6c61 6265 6c20 7468 6520 6e65 7720  o label the new 
+00019b10: 6178 6973 2061 6674 6572 2072 6563 6f6e  axis after recon
+00019b20: 7374 7275 6374 696f 6e2e 2046 6f72 0d0a  struction. For..
+00019b30: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+00019b40: 616e 6365 2c20 6966 2069 6e70 7574 2069  ance, if input i
+00019b50: 6d61 6765 2068 6173 2061 7865 7320 6060  mage has axes ``
+00019b60: 5b22 6465 6772 6565 222c 2022 7922 2c20  ["degree", "y", 
+00019b70: 2278 225d 6060 2061 6e64 200d 0a20 2020  "x"]`` and ..   
+00019b80: 2020 2020 2020 2020 2060 6068 6569 6768           ``heigh
+00019b90: 745f 6178 6973 3d22 7a22 6060 2074 6865  t_axis="z"`` the
+00019ba0: 6e20 7265 636f 6e73 7472 7563 7465 6420  n reconstructed 
+00019bb0: 696d 6167 6520 7769 6c6c 2068 6176 6520  image will have 
+00019bc0: 6178 6573 200d 0a20 2020 2020 2020 2020  axes ..         
+00019bd0: 2020 2060 605b 227a 222c 2022 7922 2c20     ``["z", "y", 
+00019be0: 2278 225d 6060 2e20 4279 2064 6566 6175  "x"]``. By defau
+00019bf0: 6c74 2c20 2279 2220 7769 6c6c 2062 6520  lt, "y" will be 
+00019c00: 7573 6564 2066 6f72 2032 4420 696e 7075  used for 2D inpu
+00019c10: 7420 6f72 2022 7a22 2066 6f72 0d0a 2020  t or "z" for..  
+00019c20: 2020 2020 2020 2020 2020 3344 2069 6e70            3D inp
+00019c30: 7574 2e0d 0a20 2020 2020 2020 2068 6569  ut...        hei
+00019c40: 6768 7420 3a20 696e 742c 206f 7074 696f  ght : int, optio
+00019c50: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+00019c60: 2048 6569 6768 7420 6f66 2072 6563 6f6e   Height of recon
+00019c70: 7374 7275 6374 696f 6e2e 2042 7920 6465  struction. By de
+00019c80: 6661 756c 742c 2073 697a 6520 6571 7561  fault, size equa
+00019c90: 6c20 746f 2074 6865 2061 7869 7320 7065  l to the axis pe
+00019ca0: 7270 656e 6469 6375 6c61 720d 0a20 2020  rpendicular..   
+00019cb0: 2020 2020 2020 2020 2074 6f20 7468 6520           to the 
+00019cc0: 726f 7461 7469 6f6e 2061 7869 7320 7769  rotation axis wi
+00019cd0: 6c6c 2062 6520 7573 6564 2e0d 0a20 2020  ll be used...   
+00019ce0: 2020 2020 2077 696e 646f 7720 3a20 7374       window : st
+00019cf0: 722c 2064 6566 6175 6c74 2069 7320 2268  r, default is "h
+00019d00: 616d 6d69 6e67 220d 0a20 2020 2020 2020  amming"..       
+00019d10: 2020 2020 2057 696e 646f 7720 6675 6e63       Window func
+00019d20: 7469 6f6e 2074 6861 7420 7769 6c6c 2062  tion that will b
+00019d30: 6520 6170 706c 6965 6420 746f 2074 6865  e applied to the
+00019d40: 2046 6f75 7269 6572 2064 6f6d 6169 6e20   Fourier domain 
+00019d50: 616c 6f6e 6720 7468 6520 6178 6973 0d0a  along the axis..
+00019d60: 2020 2020 2020 2020 2020 2020 7065 7270              perp
+00019d70: 656e 6469 6375 6c61 7220 746f 2074 6865  endicular to the
+00019d80: 2072 6f74 6174 696f 6e20 6178 6973 2e0d   rotation axis..
+00019d90: 0a20 2020 2020 2020 207b 6f72 6465 727d  .        {order}
+00019da0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00019db0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00019dc0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 496d  ----..        Im
+00019dd0: 6741 7272 6179 0d0a 2020 2020 2020 2020  gArray..        
+00019de0: 2020 2020 5265 636f 6e73 7472 7563 7469      Reconstructi
+00019df0: 6f6e 2e0d 0a20 2020 2020 2020 2020 2020  on...           
+00019e00: 200d 0a20 2020 2020 2020 2053 6565 2041   ..        See A
+00019e10: 6c73 6f0d 0a20 2020 2020 2020 202d 2d2d  lso..        ---
+00019e20: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2072  -----..        r
+00019e30: 6164 6f6e 0d0a 2020 2020 2020 2020 2222  adon..        ""
+00019e40: 220d 0a20 2020 2020 2020 2069 6e74 6572  "..        inter
+00019e50: 7020 3d20 7b30 3a20 226e 6561 7265 7374  p = {0: "nearest
+00019e60: 222c 2031 3a20 226c 696e 6561 7222 2c20  ", 1: "linear", 
+00019e70: 333a 2022 6375 6269 6322 7d5b 6f72 6465  3: "cubic"}[orde
+00019e80: 725d 0d0a 2020 2020 2020 2020 6365 6e74  r]..        cent
+00019e90: 7261 6c5f 6178 6973 2c20 6465 6772 6565  ral_axis, degree
+00019ea0: 5f61 7869 732c 206f 7574 7075 745f 7368  _axis, output_sh
+00019eb0: 6170 652c 206e 6577 5f61 7865 7320 3d20  ape, new_axes = 
+00019ec0: 5f74 7261 6e73 666f 726d 2e6e 6f72 6d61  _transform.norma
+00019ed0: 6c69 7a65 5f69 7261 646f 6e5f 696e 7075  lize_iradon_inpu
+00019ee0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00019ef0: 7365 6c66 2c20 6365 6e74 7261 6c5f 6178  self, central_ax
+00019f00: 6973 2c20 6865 6967 6874 5f61 7869 732c  is, height_axis,
+00019f10: 2064 6567 7265 655f 6178 6973 2c20 6865   degree_axis, he
+00019f20: 6967 6874 0d0a 2020 2020 2020 2020 290d  ight..        ).
+00019f30: 0a20 2020 2020 2020 2073 656c 663a 2049  .        self: I
+00019f40: 6d67 4172 7261 7920 3d20 6e70 2e6d 6f76  mgArray = np.mov
+00019f50: 6561 7869 7328 7365 6c66 2c20 7365 6c66  eaxis(self, self
+00019f60: 2e61 7869 736f 6628 6465 6772 6565 5f61  .axisof(degree_a
+00019f70: 7869 7329 2c20 2d31 290d 0a20 2020 2020  xis), -1)..     
+00019f80: 2020 2066 696c 7465 725f 6675 6e63 203d     filter_func =
+00019f90: 205f 7472 616e 7366 6f72 6d2e 6765 745f   _transform.get_
+00019fa0: 666f 7572 6965 725f 6669 6c74 6572 2873  fourier_filter(s
+00019fb0: 656c 662e 7368 6170 655b 2d32 5d2c 2077  elf.shape[-2], w
+00019fc0: 696e 646f 7729 0d0a 2020 2020 2020 2020  indow)..        
+00019fd0: 6f75 7420 3d20 7365 6c66 2e5f 6170 706c  out = self._appl
+00019fe0: 795f 6461 736b 280d 0a20 2020 2020 2020  y_dask(..       
+00019ff0: 2020 2020 205f 7472 616e 7366 6f72 6d2e       _transform.
+0001a000: 6972 6164 6f6e 2c0d 0a20 2020 2020 2020  iradon,..       
+0001a010: 2020 2020 2063 5f61 7865 733d 5b63 656e       c_axes=[cen
+0001a020: 7472 616c 5f61 7869 735d 2c0d 0a20 2020  tral_axis],..   
+0001a030: 2020 2020 2020 2020 206b 7761 7267 733d           kwargs=
+0001a040: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
+0001a050: 2020 2020 2020 2064 6567 7265 6573 3d64         degrees=d
+0001a060: 6567 7265 6573 2c0d 0a20 2020 2020 2020  egrees,..       
+0001a070: 2020 2020 2020 2020 2069 6e74 6572 706f           interpo
+0001a080: 6c61 7469 6f6e 3d69 6e74 6572 702c 0d0a  lation=interp,..
+0001a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0a0: 6669 6c74 6572 5f66 756e 633d 6669 6c74  filter_func=filt
+0001a0b0: 6572 5f66 756e 632c 0d0a 2020 2020 2020  er_func,..      
+0001a0c0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+0001a0d0: 5f73 6861 7065 3d6f 7574 7075 745f 7368  _shape=output_sh
+0001a0e0: 6170 652c 0d0a 2020 2020 2020 2020 2020  ape,..          
+0001a0f0: 2020 290d 0a20 2020 2020 2020 2029 0d0a    )..        )..
+0001a100: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a110: 2020 6966 206f 7574 2e6e 6469 6d20 3d3d    if out.ndim ==
+0001a120: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
+0001a130: 206f 7574 203d 206e 702e 6d6f 7665 6178   out = np.moveax
+0001a140: 6973 286f 7574 2c20 302c 2031 290d 0a20  is(out, 0, 1).. 
+0001a150: 2020 2020 2020 206f 7574 203d 206f 7574         out = out
+0001a160: 5b3a 3a2d 315d 0d0a 2020 2020 2020 2020  [::-1]..        
+0001a170: 7265 7475 726e 206f 7574 2e5f 7365 745f  return out._set_
+0001a180: 696e 666f 2873 656c 662c 206e 6577 5f61  info(self, new_a
+0001a190: 7865 7329 0d0a 0d0a 2020 2020 4063 6865  xes)....    @che
+0001a1a0: 636b 5f69 6e70 7574 5f61 6e64 5f6f 7574  ck_input_and_out
+0001a1b0: 7075 740d 0a20 2020 2064 6566 2074 6872  put..    def thr
+0001a1c0: 6573 686f 6c64 280d 0a20 2020 2020 2020  eshold(..       
+0001a1d0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+0001a1e0: 7468 723a 2066 6c6f 6174 207c 2073 7472  thr: float | str
+0001a1f0: 207c 2054 6872 6561 7368 6f6c 644d 6574   | ThreasholdMet
+0001a200: 686f 6420 3d20 226f 7473 7522 2c0d 0a20  hod = "otsu",.. 
+0001a210: 2020 2020 2020 202a 2c0d 0a20 2020 2020         *,..     
+0001a220: 2020 2061 6c6f 6e67 3a20 4178 6973 4c69     along: AxisLi
+0001a230: 6b65 207c 204e 6f6e 6520 3d20 4e6f 6e65  ke | None = None
+0001a240: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
+0001a250: 7267 730d 0a20 2020 2029 202d 3e20 496d  rgs..    ) -> Im
+0001a260: 6741 7272 6179 3a0d 0a20 2020 2020 2020  gArray:..       
+0001a270: 2022 2222 0d0a 2020 2020 2020 2020 4170   """..        Ap
+0001a280: 706c 7920 7468 7265 7368 6f6c 6469 6e67  ply thresholding
+0001a290: 2074 6f20 7468 6520 696d 6167 6520 616e   to the image an
+0001a2a0: 6420 6372 6561 7465 2061 2062 696e 6172  d create a binar
+0001a2b0: 7920 696d 6167 652e 0d0a 2020 2020 2020  y image...      
+0001a2c0: 2020 0d0a 2020 2020 2020 2020 5468 6520    ..        The 
+0001a2d0: 7468 7265 7368 6f6c 6420 7661 6c75 6520  threshold value 
+0001a2e0: 6361 6e20 6265 2067 6976 656e 2077 6974  can be given wit
+0001a2f0: 6820 6120 666c 6f61 7420 6f72 2061 2073  h a float or a s
+0001a300: 7472 696e 6720 7468 6174 2069 6e64 6963  tring that indic
+0001a310: 6174 6573 2077 6861 740d 0a20 2020 2020  ates what..     
+0001a320: 2020 2074 6872 6573 686f 6c64 696e 6720     thresholding 
+0001a330: 6d65 7468 6f64 2077 696c 6c20 6265 2075  method will be u
+0001a340: 7365 642e 0d0a 2020 2020 2020 2020 0d0a  sed...        ..
+0001a350: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001a360: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0001a370: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0001a380: 7468 723a 2066 6c6f 6174 206f 7220 7374  thr: float or st
+0001a390: 722c 206f 7074 696f 6e61 6c0d 0a20 2020  r, optional..   
+0001a3a0: 2020 2020 2020 2020 2054 6872 6573 686f           Thresho
+0001a3b0: 6c64 2076 616c 7565 2c20 7065 7263 656e  ld value, percen
+0001a3c0: 7461 6765 206f 7220 7468 7265 7368 6f6c  tage or threshol
+0001a3d0: 6469 6e67 2061 6c67 6f72 6974 686d 2e0d  ding algorithm..
+0001a3e0: 0a20 2020 2020 2020 2061 6c6f 6e67 203a  .        along :
+0001a3f0: 2041 7869 734c 696b 652c 206f 7074 696f   AxisLike, optio
+0001a400: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+0001a410: 2044 696d 656e 7369 6f6e 7320 7468 6174   Dimensions that
+0001a420: 2077 696c 6c20 6e6f 7420 7368 6172 6520   will not share 
+0001a430: 7468 6520 7361 6d65 2074 6872 6573 686f  the same thresho
+0001a440: 6c64 2e20 466f 7220 696e 7374 616e 6365  ld. For instance
+0001a450: 2c20 6966 0d0a 2020 2020 2020 2020 2020  , if..          
+0001a460: 2020 6060 616c 6f6e 673d 2263 2260 6020    ``along="c"`` 
+0001a470: 7468 656e 2074 6872 6573 686f 6c64 2069  then threshold i
+0001a480: 6e74 656e 7369 7469 6573 2061 7265 2064  ntensities are d
+0001a490: 6574 6572 6d69 6e65 6420 666f 7220 6576  etermined for ev
+0001a4a0: 6572 7920 6368 616e 6e65 6c2e 0d0a 2020  ery channel...  
+0001a4b0: 2020 2020 2020 2020 2020 4966 2060 6074            If ``t
+0001a4c0: 6872 6060 2069 7320 666c 6f61 742c 2060  hr`` is float, `
+0001a4d0: 6061 6c6f 6e67 6060 2077 696c 6c20 6265  `along`` will be
+0001a4e0: 2069 676e 6f72 6564 2e0d 0a20 2020 2020   ignored...     
+0001a4f0: 2020 202a 2a6b 7761 7267 733a 0d0a 2020     **kwargs:..  
+0001a500: 2020 2020 2020 2020 2020 4b65 7977 6f72            Keywor
+0001a510: 6420 6172 6775 6d65 6e74 7320 7468 6174  d arguments that
+0001a520: 2077 696c 6c20 7061 7373 6564 2074 6f20   will passed to 
+0001a530: 6675 6e63 7469 6f6e 2069 6e64 6963 6174  function indicat
+0001a540: 6564 2069 6e20 276d 6574 686f 6427 2e0d  ed in 'method'..
+0001a550: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0001a560: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+0001a570: 2d2d 2d0d 0a20 2020 2020 2020 2049 6d67  ---..        Img
+0001a580: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
+0001a590: 2020 2042 6f6f 6c69 616e 2061 7272 6179     Boolian array
+0001a5a0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
+0001a5b0: 2020 2020 2045 7861 6d70 6c65 730d 0a20       Examples.. 
+0001a5c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
+0001a5d0: 0a20 2020 2020 2020 2053 7562 7374 6974  .        Substit
+0001a5e0: 7574 6520 6f75 746c 6965 7273 2074 6f20  ute outliers to 
+0001a5f0: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
+0001a600: 3e3e 3e20 7468 7220 3d20 696d 672e 7468  >>> thr = img.th
+0001a610: 7265 7368 6f6c 6428 2239 3925 2229 0d0a  reshold("99%")..
+0001a620: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+0001a630: 696d 675b 7468 725d 203d 2030 0d0a 2020  img[thr] = 0..  
+0001a640: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0001a650: 2020 2069 6620 7365 6c66 2e64 7479 7065     if self.dtype
+0001a660: 203d 3d20 626f 6f6c 3a0d 0a20 2020 2020   == bool:..     
+0001a670: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001a680: 6c66 0d0a 2020 2020 2020 2020 0d0a 2020  lf..        ..  
+0001a690: 2020 2020 2020 6966 2061 6c6f 6e67 2069        if along i
+0001a6a0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+0001a6b0: 2020 2020 2061 6c6f 6e67 203d 2022 6322       along = "c"
+0001a6c0: 2069 6620 2263 2220 696e 2073 656c 662e   if "c" in self.
+0001a6d0: 6178 6573 2065 6c73 6520 2222 0d0a 0d0a  axes else ""....
+0001a6e0: 2020 2020 2020 2020 6d65 7468 6f64 735f          methods_
+0001a6f0: 203d 207b 2269 736f 6461 7461 223a 2073   = {"isodata": s
+0001a700: 6b66 696c 2e74 6872 6573 686f 6c64 5f69  kfil.threshold_i
+0001a710: 736f 6461 7461 2c0d 0a20 2020 2020 2020  sodata,..       
+0001a720: 2020 2020 2020 2020 2020 2020 2022 6c69               "li
 0001a730: 223a 2073 6b66 696c 2e74 6872 6573 686f  ": skfil.thresho
-0001a740: 6c64 5f6d 696e 696d 756d 2c0d 0a20 2020  ld_minimum,..   
-0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2022 6d69 6e69 6d75 6d22 3a20 736b 6669   "minimum": skfi
-0001a770: 6c2e 7468 7265 7368 6f6c 645f 6d69 6e69  l.threshold_mini
-0001a780: 6d75 6d2c 0d0a 2020 2020 2020 2020 2020  mum,..          
-0001a790: 2020 2020 2020 2020 2020 226e 6962 6c61            "nibla
-0001a7a0: 636b 223a 2073 6b66 696c 2e74 6872 6573  ck": skfil.thres
-0001a7b0: 686f 6c64 5f6e 6962 6c61 636b 2c0d 0a20  hold_niblack,.. 
-0001a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7d0: 2020 2022 6f74 7375 223a 2073 6b66 696c     "otsu": skfil
-0001a7e0: 2e74 6872 6573 686f 6c64 5f6f 7473 752c  .threshold_otsu,
-0001a7f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a800: 2020 2020 2020 2273 6175 766f 6c61 223a        "sauvola":
-0001a810: 2073 6b66 696c 2e74 6872 6573 686f 6c64   skfil.threshold
-0001a820: 5f73 6175 766f 6c61 2c0d 0a20 2020 2020  _sauvola,..     
-0001a830: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001a840: 7472 6961 6e67 6c65 223a 2073 6b66 696c  triangle": skfil
-0001a850: 2e74 6872 6573 686f 6c64 5f74 7269 616e  .threshold_trian
-0001a860: 676c 652c 0d0a 2020 2020 2020 2020 2020  gle,..          
-0001a870: 2020 2020 2020 2020 2020 2279 656e 223a            "yen":
-0001a880: 2073 6b66 696c 2e74 6872 6573 686f 6c64   skfil.threshold
-0001a890: 5f79 656e 0d0a 2020 2020 2020 2020 2020  _yen..          
-0001a8a0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-0001a8b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001a8c0: 6620 6973 696e 7374 616e 6365 2874 6872  f isinstance(thr
-0001a8d0: 2c20 7374 7229 2061 6e64 2074 6872 2e65  , str) and thr.e
-0001a8e0: 6e64 7377 6974 6828 2225 2229 3a0d 0a20  ndswith("%"):.. 
-0001a8f0: 2020 2020 2020 2020 2020 2070 203d 2066             p = f
-0001a900: 6c6f 6174 2874 6872 5b3a 2d31 5d2e 7374  loat(thr[:-1].st
-0001a910: 7269 7028 2929 0d0a 2020 2020 2020 2020  rip())..        
-0001a920: 2020 2020 6f75 7420 3d20 6e70 2e7a 6572      out = np.zer
-0001a930: 6f73 2873 656c 662e 7368 6170 652c 2064  os(self.shape, d
-0001a940: 7479 7065 3d62 6f6f 6c29 0d0a 2020 2020  type=bool)..    
-0001a950: 2020 2020 2020 2020 666f 7220 736c 2c20          for sl, 
-0001a960: 696d 6720 696e 2073 656c 662e 6974 6572  img in self.iter
-0001a970: 2861 6c6f 6e67 293a 0d0a 2020 2020 2020  (along):..      
-0001a980: 2020 2020 2020 2020 2020 7468 7220 3d20            thr = 
-0001a990: 6e70 2e70 6572 6365 6e74 696c 6528 696d  np.percentile(im
-0001a9a0: 672c 2070 290d 0a20 2020 2020 2020 2020  g, p)..         
-0001a9b0: 2020 2020 2020 206f 7574 5b73 6c5d 203d         out[sl] =
-0001a9c0: 2069 6d67 203e 3d20 7468 720d 0a20 2020   img >= thr..   
-0001a9d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001a9e0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-0001a9f0: 7374 616e 6365 2874 6872 2c20 7374 7229  stance(thr, str)
-0001aa00: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-0001aa10: 6574 686f 6420 3d20 7468 722e 6c6f 7765  ethod = thr.lowe
-0001aa20: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
-0001aa30: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0001aa40: 2020 2020 2020 2066 756e 6320 3d20 6d65         func = me
-0001aa50: 7468 6f64 735f 5b6d 6574 686f 645d 0d0a  thods_[method]..
-0001aa60: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0001aa70: 7074 204b 6579 4572 726f 723a 0d0a 2020  pt KeyError:..  
-0001aa80: 2020 2020 2020 2020 2020 2020 2020 7320                s 
-0001aa90: 3d20 222c 2022 2e6a 6f69 6e28 6c69 7374  = ", ".join(list
-0001aaa0: 286d 6574 686f 6473 5f2e 6b65 7973 2829  (methods_.keys()
-0001aab0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001aac0: 2020 2020 7261 6973 6520 4b65 7945 7272      raise KeyErr
-0001aad0: 6f72 2866 227b 6d65 7468 6f64 7d5c 6e6d  or(f"{method}\nm
-0001aae0: 6574 686f 6420 6d75 7374 2062 653a 207b  ethod must be: {
-0001aaf0: 737d 2229 0d0a 2020 2020 2020 2020 2020  s}")..          
-0001ab00: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0001ab10: 6f75 7420 3d20 6e70 2e7a 6572 6f73 2873  out = np.zeros(s
-0001ab20: 656c 662e 7368 6170 652c 2064 7479 7065  elf.shape, dtype
-0001ab30: 3d62 6f6f 6c29 0d0a 2020 2020 2020 2020  =bool)..        
-0001ab40: 2020 2020 666f 7220 736c 2c20 696d 6720      for sl, img 
-0001ab50: 696e 2073 656c 662e 6974 6572 2861 6c6f  in self.iter(alo
-0001ab60: 6e67 293a 0d0a 2020 2020 2020 2020 2020  ng):..          
-0001ab70: 2020 2020 2020 7468 7220 3d20 6675 6e63        thr = func
-0001ab80: 2869 6d67 2c20 2a2a 6b77 6172 6773 290d  (img, **kwargs).
-0001ab90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aba0: 206f 7574 5b73 6c5d 203d 2069 6d67 203e   out[sl] = img >
-0001abb0: 3d20 7468 720d 0a20 2020 2020 2020 2020  = thr..         
-0001abc0: 2020 200d 0a0d 0a20 2020 2020 2020 2065     ....        e
-0001abd0: 6c69 6620 6e70 2e69 7373 6361 6c61 7228  lif np.isscalar(
-0001abe0: 7468 7229 3a0d 0a20 2020 2020 2020 2020  thr):..         
-0001abf0: 2020 206f 7574 203d 2073 656c 6620 3e3d     out = self >=
-0001ac00: 2074 6872 0d0a 2020 2020 2020 2020 656c   thr..        el
-0001ac10: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001ac20: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-0001ac30: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001ac40: 2020 2022 2774 6872 2720 6d75 7374 2062     "'thr' must b
-0001ac50: 6520 6e75 6d65 7269 632c 206f 7220 7374  e numeric, or st
-0001ac60: 7220 7370 6563 6966 7969 6e67 2061 2074  r specifying a t
-0001ac70: 6872 6573 686f 6c64 696e 6720 6d65 7468  hresholding meth
-0001ac80: 6f64 2e22 0d0a 2020 2020 2020 2020 2020  od."..          
-0001ac90: 2020 290d 0a20 2020 2020 2020 200d 0a20    )..        .. 
-0001aca0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0001acb0: 740d 0a20 2020 200d 0a20 2020 2040 5f64  t..    ..    @_d
-0001acc0: 6f63 732e 7772 6974 655f 646f 6373 0d0a  ocs.write_docs..
-0001acd0: 2020 2020 4064 696d 735f 746f 5f73 7061      @dims_to_spa
-0001ace0: 7469 616c 5f61 7865 730d 0a20 2020 2040  tial_axes..    @
-0001acf0: 6368 6563 6b5f 696e 7075 745f 616e 645f  check_input_and_
-0001ad00: 6f75 7470 7574 286f 6e6c 795f 6269 6e61  output(only_bina
-0001ad10: 7279 3d54 7275 6529 0d0a 2020 2020 6465  ry=True)..    de
-0001ad20: 6620 6469 7374 616e 6365 5f6d 6170 2873  f distance_map(s
-0001ad30: 656c 662c 202a 2c20 6469 6d73 3a20 4469  elf, *, dims: Di
-0001ad40: 6d73 203d 204e 6f6e 6529 202d 3e20 496d  ms = None) -> Im
-0001ad50: 6741 7272 6179 3a0d 0a20 2020 2020 2020  gArray:..       
-0001ad60: 2022 2222 0d0a 2020 2020 2020 2020 4361   """..        Ca
-0001ad70: 6c63 756c 6174 6520 6469 7374 616e 6365  lculate distance
-0001ad80: 206d 6170 2066 726f 6d20 6269 6e61 7279   map from binary
-0001ad90: 2069 6d61 6765 732e 0d0a 2020 2020 2020   images...      
-0001ada0: 2020 466f 7220 696e 7374 616e 6365 2c20    For instance, 
-0001adb0: 6060 5b31 2c20 312c 2031 2c20 302c 2030  ``[1, 1, 1, 0, 0
-0001adc0: 2c20 302c 2031 2c20 312c 2031 5d60 6020  , 0, 1, 1, 1]`` 
-0001add0: 7769 6c6c 2062 6520 636f 6e76 6572 7465  will be converte
-0001ade0: 6420 746f 200d 0a20 2020 2020 2020 2060  d to ..        `
-0001adf0: 605b 332c 2032 2c20 312c 2030 2c20 302c  `[3, 2, 1, 0, 0,
-0001ae00: 2030 2c20 312c 2032 2c20 335d 6060 2e20   0, 1, 2, 3]``. 
-0001ae10: 4e6f 7465 2074 6861 7420 7265 7475 726e  Note that return
-0001ae20: 6564 2061 7272 6179 2077 696c 6c20 6265  ed array will be
-0001ae30: 2066 6c6f 6174 2069 6e20 6e2d 4420 0d0a   float in n-D ..
-0001ae40: 2020 2020 2020 2020 696d 6167 6573 2e0d          images..
-0001ae50: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001ae60: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-0001ae70: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-0001ae80: 2020 207b 6469 6d73 7d0d 0a0d 0a20 2020     {dims}....   
-0001ae90: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-0001aea0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-0001aeb0: 2020 2020 2020 2049 6d67 4172 7261 790d         ImgArray.
-0001aec0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
-0001aed0: 7461 6e63 6520 6d61 702c 2074 6865 2066  tance map, the f
-0001aee0: 7572 7468 6572 2074 6865 2062 7269 6768  urther the brigh
-0001aef0: 7465 720d 0a20 2020 2020 2020 2022 2222  ter..        """
-0001af00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001af10: 2020 7265 7475 726e 2073 656c 662e 5f61    return self._a
-0001af20: 7070 6c79 5f64 6173 6b28 6e64 692e 6469  pply_dask(ndi.di
-0001af30: 7374 616e 6365 5f74 7261 6e73 666f 726d  stance_transform
-0001af40: 5f65 6474 2c20 0d0a 2020 2020 2020 2020  _edt, ..        
-0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af60: 2020 2020 2020 2063 5f61 7865 733d 636f         c_axes=co
-0001af70: 6d70 6c65 6d65 6e74 5f61 7865 7328 6469  mplement_axes(di
-0001af80: 6d73 2c20 7365 6c66 2e61 7865 7329 0d0a  ms, self.axes)..
-0001af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afa0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001afb0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0001afc0: 4064 696d 735f 746f 5f73 7061 7469 616c  @dims_to_spatial
-0001afd0: 5f61 7865 730d 0a20 2020 2040 6368 6563  _axes..    @chec
-0001afe0: 6b5f 696e 7075 745f 616e 645f 6f75 7470  k_input_and_outp
-0001aff0: 7574 0d0a 2020 2020 6465 6620 6e63 635f  ut..    def ncc_
-0001b000: 6669 6c74 6572 280d 0a20 2020 2020 2020  filter(..       
-0001b010: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-0001b020: 7465 6d70 6c61 7465 3a20 6e70 2e6e 6461  template: np.nda
-0001b030: 7272 6179 2c0d 0a20 2020 2020 2020 206d  rray,..        m
-0001b040: 6f64 653a 2073 7472 203d 2022 636f 6e73  ode: str = "cons
-0001b050: 7461 6e74 222c 200d 0a20 2020 2020 2020  tant", ..       
-0001b060: 2063 7661 6c3a 2066 6c6f 6174 207c 2073   cval: float | s
-0001b070: 7472 207c 2043 616c 6c61 626c 655b 5b6e  tr | Callable[[n
-0001b080: 702e 6e64 6172 7261 795d 2c20 666c 6f61  p.ndarray], floa
-0001b090: 745d 203d 206e 702e 6d65 616e 2c20 0d0a  t] = np.mean, ..
-0001b0a0: 2020 2020 2020 2020 2a2c 200d 0a20 2020          *, ..   
-0001b0b0: 2020 2020 2064 696d 733a 2044 696d 7320       dims: Dims 
-0001b0c0: 3d20 4e6f 6e65 0d0a 2020 2020 2920 2d3e  = None..    ) ->
-0001b0d0: 2049 6d67 4172 7261 793a 0d0a 2020 2020   ImgArray:..    
-0001b0e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0001b0f0: 2054 656d 706c 6174 6520 6d61 7463 6869   Template matchi
-0001b100: 6e67 2075 7369 6e67 206e 6f72 6d61 6c69  ng using normali
-0001b110: 7a65 6420 6372 6f73 7320 636f 7272 656c  zed cross correl
-0001b120: 6174 696f 6e20 284e 4343 2920 6d65 7468  ation (NCC) meth
-0001b130: 6f64 2e20 5468 6973 2066 756e 6374 696f  od. This functio
-0001b140: 6e20 6973 2062 6173 6963 616c 6c79 0d0a  n is basically..
-0001b150: 2020 2020 2020 2020 6964 656e 7469 6361          identica
-0001b160: 6c20 746f 2074 6861 7420 696e 2060 736b  l to that in `sk
-0001b170: 696d 6167 652e 6665 6174 7572 6560 2c20  image.feature`, 
-0001b180: 6275 7420 6973 206f 7074 696d 697a 6564  but is optimized
-0001b190: 2066 6f72 2062 6174 6368 2070 726f 6365   for batch proce
-0001b1a0: 7373 696e 6720 616e 6420 696d 7072 6f76  ssing and improv
-0001b1b0: 6564 200d 0a20 2020 2020 2020 2072 6561  ed ..        rea
-0001b1c0: 6461 6269 6c69 7479 2e0d 0a0d 0a20 2020  dability.....   
-0001b1d0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-0001b1e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0001b1f0: 2d2d 2d0d 0a20 2020 2020 2020 2074 656d  ---..        tem
-0001b200: 706c 6174 6520 3a20 6e70 2e6e 6461 7272  plate : np.ndarr
-0001b210: 6179 0d0a 2020 2020 2020 2020 2020 2020  ay..            
-0001b220: 5465 6d70 6c61 7465 2069 6d61 6765 2e20  Template image. 
-0001b230: 4d75 7374 2062 6520 3220 6f72 2033 2064  Must be 2 or 3 d
-0001b240: 696d 656e 7369 6f6e 616c 2e20 0d0a 2020  imensional. ..  
-0001b250: 2020 2020 2020 7b6d 6f64 657d 0d0a 2020        {mode}..  
-0001b260: 2020 2020 2020 6376 616c 203a 2066 6c6f        cval : flo
-0001b270: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
-0001b280: 2020 2020 2020 2020 2020 4261 636b 6772            Backgr
-0001b290: 6f75 6e64 2069 6e74 656e 7369 7479 2e20  ound intensity. 
-0001b2a0: 4966 206e 6f74 2067 6976 656e 2c20 6974  If not given, it
-0001b2b0: 2077 696c 6c20 6361 6c63 756c 6174 6564   will calculated
-0001b2c0: 2061 7320 7468 6520 6d65 616e 2076 616c   as the mean val
-0001b2d0: 7565 206f 6620 0d0a 2020 2020 2020 2020  ue of ..        
-0001b2e0: 2020 2020 7468 6520 6f72 6967 696e 616c      the original
-0001b2f0: 2069 6d61 6765 2e0d 0a20 2020 2020 2020   image...       
-0001b300: 207b 6469 6d73 7d0d 0a0d 0a20 2020 2020   {dims}....     
-0001b310: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-0001b320: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-0001b330: 2020 2020 2049 6d67 4172 7261 790d 0a20       ImgArray.. 
-0001b340: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-0001b350: 6e73 6520 696d 6167 6520 7769 7468 2076  nse image with v
-0001b360: 616c 7565 7320 6265 7477 6565 6e20 2d31  alues between -1
-0001b370: 2061 6e64 2031 2e0d 0a20 2020 2020 2020   and 1...       
-0001b380: 2022 2222 2020 2020 2020 2020 0d0a 2020   """        ..  
-0001b390: 2020 2020 2020 7465 6d70 6c61 7465 203d        template =
-0001b3a0: 205f 6368 6563 6b5f 7465 6d70 6c61 7465   _check_template
-0001b3b0: 2874 656d 706c 6174 6529 0d0a 2020 2020  (template)..    
-0001b3c0: 2020 2020 6966 2063 616c 6c61 626c 6528      if callable(
-0001b3d0: 6376 616c 293a 0d0a 2020 2020 2020 2020  cval):..        
-0001b3e0: 2020 2020 6376 616c 203d 2063 7661 6c28      cval = cval(
-0001b3f0: 7365 6c66 290d 0a20 2020 2020 2020 2063  self)..        c
-0001b400: 7661 6c20 3d20 5f63 6865 636b 5f62 6728  val = _check_bg(
-0001b410: 7365 6c66 2c20 6376 616c 290d 0a20 2020  self, cval)..   
-0001b420: 2020 2020 2069 6620 6c65 6e28 6469 6d73       if len(dims
-0001b430: 2920 213d 2074 656d 706c 6174 652e 6e64  ) != template.nd
-0001b440: 696d 3a0d 0a20 2020 2020 2020 2020 2020  im:..           
-0001b450: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001b460: 7228 2264 696d 7320 616e 6420 7468 6520  r("dims and the 
-0001b470: 6e75 6d62 6572 206f 6620 7465 6d70 6c61  number of templa
-0001b480: 7465 2064 696d 656e 7369 6f6e 2064 6f6e  te dimension don
-0001b490: 2774 206d 6174 6368 2e22 290d 0a20 2020  't match.")..   
-0001b4a0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-0001b4b0: 6574 7572 6e20 7365 6c66 2e61 735f 666c  eturn self.as_fl
-0001b4c0: 6f61 7428 292e 5f61 7070 6c79 5f64 6173  oat()._apply_das
-0001b4d0: 6b28 0d0a 2020 2020 2020 2020 2020 2020  k(..            
-0001b4e0: 5f66 696c 7465 7273 2e6e 6363 5f66 696c  _filters.ncc_fil
-0001b4f0: 7465 722c 0d0a 2020 2020 2020 2020 2020  ter,..          
-0001b500: 2020 635f 6178 6573 3d63 6f6d 706c 656d    c_axes=complem
-0001b510: 656e 745f 6178 6573 2864 696d 732c 2073  ent_axes(dims, s
-0001b520: 656c 662e 6178 6573 292c 200d 0a20 2020  elf.axes), ..   
-0001b530: 2020 2020 2020 2020 2061 7267 733d 2874           args=(t
-0001b540: 656d 706c 6174 652c 2063 7661 6c2c 206d  emplate, cval, m
-0001b550: 6f64 6529 0d0a 2020 2020 2020 2020 290d  ode)..        ).
-0001b560: 0a20 2020 200d 0a20 2020 2040 5f64 6f63  .    ..    @_doc
-0001b570: 732e 7772 6974 655f 646f 6373 0d0a 2020  s.write_docs..  
-0001b580: 2020 4064 696d 735f 746f 5f73 7061 7469    @dims_to_spati
-0001b590: 616c 5f61 7865 730d 0a20 2020 2040 6368  al_axes..    @ch
-0001b5a0: 6563 6b5f 696e 7075 745f 616e 645f 6f75  eck_input_and_ou
-0001b5b0: 7470 7574 286f 6e6c 795f 6269 6e61 7279  tput(only_binary
-0001b5c0: 3d54 7275 6529 0d0a 2020 2020 6465 6620  =True)..    def 
-0001b5d0: 7265 6d6f 7665 5f6c 6172 6765 5f6f 626a  remove_large_obj
-0001b5e0: 6563 7473 2873 656c 662c 2072 6164 6975  ects(self, radiu
-0001b5f0: 733a 2066 6c6f 6174 203d 2035 2c20 2a2c  s: float = 5, *,
-0001b600: 2064 696d 733a 2044 696d 7320 3d20 4e6f   dims: Dims = No
-0001b610: 6e65 2c20 7570 6461 7465 3a20 626f 6f6c  ne, update: bool
-0001b620: 203d 2046 616c 7365 2920 2d3e 2049 6d67   = False) -> Img
-0001b630: 4172 7261 793a 0d0a 2020 2020 2020 2020  Array:..        
-0001b640: 2222 220d 0a20 2020 2020 2020 2052 656d  """..        Rem
-0001b650: 6f76 6520 6c61 7267 6520 6f62 6a65 6374  ove large object
-0001b660: 7320 7573 696e 6720 6f70 656e 696e 672e  s using opening.
-0001b670: 2054 686f 7365 206f 626a 6563 7473 2074   Those objects t
-0001b680: 6861 7420 7765 7265 206e 6f74 2072 656d  hat were not rem
-0001b690: 6f76 6564 2062 7920 6f70 656e 696e 670d  oved by opening.
-0001b6a0: 0a20 2020 2020 2020 2077 696c 6c20 6265  .        will be
-0001b6b0: 2072 656d 6f76 6564 2069 6e20 6f75 7470   removed in outp
-0001b6c0: 7574 2e0d 0a0d 0a20 2020 2020 2020 2050  ut.....        P
-0001b6d0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0001b6e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-0001b6f0: 2020 2020 2020 2072 6164 6975 7320 3a20         radius : 
-0001b700: 666c 6f61 742c 206f 7074 696f 6e61 6c0d  float, optional.
-0001b710: 0a20 2020 2020 2020 2020 2020 204f 626a  .            Obj
-0001b720: 6563 7473 2077 6974 6820 7261 6469 7573  ects with radius
-0001b730: 206c 6172 6765 7220 7468 616e 2074 6869   larger than thi
-0001b740: 7320 7661 6c75 6520 7769 6c6c 2062 6520  s value will be 
-0001b750: 7265 6d6f 7665 642e 0d0a 2020 2020 2020  removed...      
-0001b760: 2020 7b64 696d 737d 7b75 7064 6174 657d    {dims}{update}
-0001b770: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0001b780: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-0001b790: 2d2d 2d2d 0d0a 2020 2020 2020 2020 496d  ----..        Im
-0001b7a0: 6741 7272 6179 0d0a 2020 2020 2020 2020  gArray..        
-0001b7b0: 2020 2020 496d 6167 6520 7769 7468 206c      Image with l
-0001b7c0: 6172 6765 206f 626a 6563 7473 2072 656d  arge objects rem
-0001b7d0: 6f76 6564 2e0d 0a0d 0a20 2020 2020 2020  oved.....       
-0001b7e0: 2053 6565 2041 6c73 6f0d 0a20 2020 2020   See Also..     
-0001b7f0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-0001b800: 2020 2020 2072 656d 6f76 655f 6669 6e65       remove_fine
-0001b810: 5f6f 626a 6563 7473 0d0a 2020 2020 2020  _objects..      
-0001b820: 2020 2222 2220 2020 2020 2020 200d 0a20    """        .. 
-0001b830: 2020 2020 2020 206f 7574 203d 2073 656c         out = sel
-0001b840: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
-0001b850: 2020 6c61 7267 655f 6f62 6a20 3d20 7365    large_obj = se
-0001b860: 6c66 2e6f 7065 6e69 6e67 2872 6164 6975  lf.opening(radiu
-0001b870: 732c 2064 696d 733d 6469 6d73 290d 0a20  s, dims=dims).. 
-0001b880: 2020 2020 2020 206f 7574 2e76 616c 7565         out.value
-0001b890: 5b6c 6172 6765 5f6f 626a 5d20 3d20 300d  [large_obj] = 0.
-0001b8a0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001b8b0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0001b8c0: 740d 0a20 2020 200d 0a20 2020 2040 5f64  t..    ..    @_d
-0001b8d0: 6f63 732e 7772 6974 655f 646f 6373 0d0a  ocs.write_docs..
-0001b8e0: 2020 2020 4064 696d 735f 746f 5f73 7061      @dims_to_spa
-0001b8f0: 7469 616c 5f61 7865 730d 0a20 2020 2040  tial_axes..    @
-0001b900: 6368 6563 6b5f 696e 7075 745f 616e 645f  check_input_and_
-0001b910: 6f75 7470 7574 286f 6e6c 795f 6269 6e61  output(only_bina
-0001b920: 7279 3d54 7275 6529 0d0a 2020 2020 6465  ry=True)..    de
-0001b930: 6620 7265 6d6f 7665 5f66 696e 655f 6f62  f remove_fine_ob
-0001b940: 6a65 6374 7328 7365 6c66 2c20 6c65 6e67  jects(self, leng
-0001b950: 7468 3a20 666c 6f61 7420 3d20 3130 2c20  th: float = 10, 
-0001b960: 2a2c 2064 696d 733a 2044 696d 7320 3d20  *, dims: Dims = 
-0001b970: 4e6f 6e65 2c20 7570 6461 7465 3a20 626f  None, update: bo
-0001b980: 6f6c 203d 2046 616c 7365 2920 2d3e 2049  ol = False) -> I
-0001b990: 6d67 4172 7261 793a 0d0a 2020 2020 2020  mgArray:..      
-0001b9a0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
-0001b9b0: 656d 6f76 6520 6669 6e65 206f 626a 6563  emove fine objec
-0001b9c0: 7473 2075 7369 6e67 2064 6961 6d65 7465  ts using diamete
-0001b9d0: 725f 6f70 656e 696e 672e 0d0a 0d0a 2020  r_opening.....  
-0001b9e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0001b9f0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0001ba00: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6c65  ----..        le
-0001ba10: 6e67 7468 203a 2066 6c6f 6174 2c20 6465  ngth : float, de
-0001ba20: 6661 756c 7420 6973 2031 300d 0a20 2020  fault is 10..   
-0001ba30: 2020 2020 2020 2020 204f 626a 6563 7473           Objects
-0001ba40: 206c 6f6e 6765 7220 7468 616e 2074 6869   longer than thi
-0001ba50: 7320 7769 6c6c 2062 6520 7265 6d6f 7665  s will be remove
-0001ba60: 642e 0d0a 2020 2020 2020 2020 7b64 696d  d...        {dim
-0001ba70: 737d 7b75 7064 6174 657d 0d0a 0d0a 2020  s}{update}....  
-0001ba80: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0001ba90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0001baa0: 2020 2020 2020 2020 496d 6741 7272 6179          ImgArray
-0001bab0: 0d0a 2020 2020 2020 2020 2020 2020 496d  ..            Im
-0001bac0: 6167 6520 7769 7468 206c 6172 6765 206f  age with large o
-0001bad0: 626a 6563 7473 2072 656d 6f76 6564 2e0d  bjects removed..
-0001bae0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0001baf0: 2020 2053 6565 2041 6c73 6f0d 0a20 2020     See Also..   
-0001bb00: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-0001bb10: 2020 2020 2020 2072 656d 6f76 655f 6c61         remove_la
-0001bb20: 7267 655f 6f62 6a65 6374 730d 0a20 2020  rge_objects..   
-0001bb30: 2020 2020 2022 2222 2020 2020 2020 2020       """        
-0001bb40: 0d0a 2020 2020 2020 2020 6f75 7420 3d20  ..        out = 
-0001bb50: 7365 6c66 2e63 6f70 7928 290d 0a20 2020  self.copy()..   
-0001bb60: 2020 2020 2066 696e 655f 6f62 6a20 3d20       fine_obj = 
-0001bb70: 7365 6c66 2e64 6961 6d65 7465 725f 6f70  self.diameter_op
-0001bb80: 656e 696e 6728 6c65 6e67 7468 2c20 636f  ening(length, co
-0001bb90: 6e6e 6563 7469 7669 7479 3d6c 656e 2864  nnectivity=len(d
-0001bba0: 696d 7329 290d 0a20 2020 2020 2020 206c  ims))..        l
-0001bbb0: 6172 6765 5f6f 626a 203d 2073 656c 662e  arge_obj = self.
-0001bbc0: 6f70 656e 696e 6728 6c65 6e67 7468 2f2f  opening(length//
-0001bbd0: 3229 0d0a 2020 2020 2020 2020 6f75 742e  2)..        out.
-0001bbe0: 7661 6c75 655b 7e6c 6172 6765 5f6f 626a  value[~large_obj
-0001bbf0: 2026 2066 696e 655f 6f62 6a5d 203d 2030   & fine_obj] = 0
-0001bc00: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001bc10: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0001bc20: 7574 0d0a 2020 2020 0d0a 2020 2020 405f  ut..    ..    @_
-0001bc30: 646f 6373 2e77 7269 7465 5f64 6f63 730d  docs.write_docs.
-0001bc40: 0a20 2020 2040 6469 6d73 5f74 6f5f 7370  .    @dims_to_sp
-0001bc50: 6174 6961 6c5f 6178 6573 0d0a 2020 2020  atial_axes..    
-0001bc60: 4063 6865 636b 5f69 6e70 7574 5f61 6e64  @check_input_and
-0001bc70: 5f6f 7574 7075 7428 6f6e 6c79 5f62 696e  _output(only_bin
-0001bc80: 6172 793d 5472 7565 290d 0a20 2020 2064  ary=True)..    d
-0001bc90: 6566 2063 6f6e 7665 785f 6875 6c6c 2873  ef convex_hull(s
-0001bca0: 656c 662c 202a 2c20 6469 6d73 3a20 4469  elf, *, dims: Di
-0001bcb0: 6d73 203d 204e 6f6e 652c 2075 7064 6174  ms = None, updat
-0001bcc0: 653d 4661 6c73 6529 202d 3e20 496d 6741  e=False) -> ImgA
-0001bcd0: 7272 6179 3a0d 0a20 2020 2020 2020 2022  rray:..        "
-0001bce0: 2222 0d0a 2020 2020 2020 2020 436f 6d70  ""..        Comp
-0001bcf0: 7574 6520 636f 6e76 6578 2068 756c 6c20  ute convex hull 
-0001bd00: 696d 6167 652e 0d0a 0d0a 2020 2020 2020  image.....      
-0001bd10: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-0001bd20: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0001bd30: 0d0a 2020 2020 2020 2020 7b64 696d 737d  ..        {dims}
-0001bd40: 7b75 7064 6174 657d 0d0a 0d0a 2020 2020  {update}....    
-0001bd50: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-0001bd60: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-0001bd70: 2020 2020 2020 496d 6741 7272 6179 0d0a        ImgArray..
-0001bd80: 2020 2020 2020 2020 2020 2020 436f 6e76              Conv
+0001a740: 6c64 5f6c 692c 0d0a 2020 2020 2020 2020  ld_li,..        
+0001a750: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+0001a760: 616c 223a 2073 6b66 696c 2e74 6872 6573  al": skfil.thres
+0001a770: 686f 6c64 5f6c 6f63 616c 2c0d 0a20 2020  hold_local,..   
+0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a790: 2022 6d65 616e 223a 2073 6b66 696c 2e74   "mean": skfil.t
+0001a7a0: 6872 6573 686f 6c64 5f6d 6561 6e2c 0d0a  hreshold_mean,..
+0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7c0: 2020 2020 226d 696e 223a 2073 6b66 696c      "min": skfil
+0001a7d0: 2e74 6872 6573 686f 6c64 5f6d 696e 696d  .threshold_minim
+0001a7e0: 756d 2c0d 0a20 2020 2020 2020 2020 2020  um,..           
+0001a7f0: 2020 2020 2020 2020 2022 6d69 6e69 6d75           "minimu
+0001a800: 6d22 3a20 736b 6669 6c2e 7468 7265 7368  m": skfil.thresh
+0001a810: 6f6c 645f 6d69 6e69 6d75 6d2c 0d0a 2020  old_minimum,..  
+0001a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a830: 2020 226e 6962 6c61 636b 223a 2073 6b66    "niblack": skf
+0001a840: 696c 2e74 6872 6573 686f 6c64 5f6e 6962  il.threshold_nib
+0001a850: 6c61 636b 2c0d 0a20 2020 2020 2020 2020  lack,..         
+0001a860: 2020 2020 2020 2020 2020 2022 6f74 7375             "otsu
+0001a870: 223a 2073 6b66 696c 2e74 6872 6573 686f  ": skfil.thresho
+0001a880: 6c64 5f6f 7473 752c 0d0a 2020 2020 2020  ld_otsu,..      
+0001a890: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+0001a8a0: 6175 766f 6c61 223a 2073 6b66 696c 2e74  auvola": skfil.t
+0001a8b0: 6872 6573 686f 6c64 5f73 6175 766f 6c61  hreshold_sauvola
+0001a8c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a8d0: 2020 2020 2020 2022 7472 6961 6e67 6c65         "triangle
+0001a8e0: 223a 2073 6b66 696c 2e74 6872 6573 686f  ": skfil.thresho
+0001a8f0: 6c64 5f74 7269 616e 676c 652c 0d0a 2020  ld_triangle,..  
+0001a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a910: 2020 2279 656e 223a 2073 6b66 696c 2e74    "yen": skfil.t
+0001a920: 6872 6573 686f 6c64 5f79 656e 0d0a 2020  hreshold_yen..  
+0001a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a940: 2020 7d0d 0a20 2020 2020 2020 200d 0a20    }..        .. 
+0001a950: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0001a960: 616e 6365 2874 6872 2c20 7374 7229 2061  ance(thr, str) a
+0001a970: 6e64 2074 6872 2e65 6e64 7377 6974 6828  nd thr.endswith(
+0001a980: 2225 2229 3a0d 0a20 2020 2020 2020 2020  "%"):..         
+0001a990: 2020 2070 203d 2066 6c6f 6174 2874 6872     p = float(thr
+0001a9a0: 5b3a 2d31 5d2e 7374 7269 7028 2929 0d0a  [:-1].strip())..
+0001a9b0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+0001a9c0: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
+0001a9d0: 7368 6170 652c 2064 7479 7065 3d62 6f6f  shape, dtype=boo
+0001a9e0: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
+0001a9f0: 666f 7220 736c 2c20 696d 6720 696e 2073  for sl, img in s
+0001aa00: 656c 662e 6974 6572 2861 6c6f 6e67 293a  elf.iter(along):
+0001aa10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aa20: 2020 7468 7220 3d20 6e70 2e70 6572 6365    thr = np.perce
+0001aa30: 6e74 696c 6528 696d 672c 2070 290d 0a20  ntile(img, p).. 
+0001aa40: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001aa50: 7574 5b73 6c5d 203d 2069 6d67 203e 3d20  ut[sl] = img >= 
+0001aa60: 7468 720d 0a20 2020 2020 2020 2020 2020  thr..           
+0001aa70: 2020 2020 200d 0a20 2020 2020 2020 2065       ..        e
+0001aa80: 6c69 6620 6973 696e 7374 616e 6365 2874  lif isinstance(t
+0001aa90: 6872 2c20 7374 7229 3a0d 0a20 2020 2020  hr, str):..     
+0001aaa0: 2020 2020 2020 206d 6574 686f 6420 3d20         method = 
+0001aab0: 7468 722e 6c6f 7765 7228 290d 0a20 2020  thr.lower()..   
+0001aac0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001aae0: 756e 6320 3d20 6d65 7468 6f64 735f 5b6d  unc = methods_[m
+0001aaf0: 6574 686f 645d 0d0a 2020 2020 2020 2020  ethod]..        
+0001ab00: 2020 2020 6578 6365 7074 204b 6579 4572      except KeyEr
+0001ab10: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+0001ab20: 2020 2020 2020 7320 3d20 222c 2022 2e6a        s = ", ".j
+0001ab30: 6f69 6e28 6c69 7374 286d 6574 686f 6473  oin(list(methods
+0001ab40: 5f2e 6b65 7973 2829 2929 0d0a 2020 2020  _.keys()))..    
+0001ab50: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001ab60: 6520 4b65 7945 7272 6f72 2866 227b 6d65  e KeyError(f"{me
+0001ab70: 7468 6f64 7d5c 6e6d 6574 686f 6420 6d75  thod}\nmethod mu
+0001ab80: 7374 2062 653a 207b 737d 2229 0d0a 2020  st be: {s}")..  
+0001ab90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001aba0: 2020 2020 2020 2020 6f75 7420 3d20 6e70          out = np
+0001abb0: 2e7a 6572 6f73 2873 656c 662e 7368 6170  .zeros(self.shap
+0001abc0: 652c 2064 7479 7065 3d62 6f6f 6c29 0d0a  e, dtype=bool)..
+0001abd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001abe0: 736c 2c20 696d 6720 696e 2073 656c 662e  sl, img in self.
+0001abf0: 6974 6572 2861 6c6f 6e67 293a 0d0a 2020  iter(along):..  
+0001ac00: 2020 2020 2020 2020 2020 2020 2020 7468                th
+0001ac10: 7220 3d20 6675 6e63 2869 6d67 2c20 2a2a  r = func(img, **
+0001ac20: 6b77 6172 6773 290d 0a20 2020 2020 2020  kwargs)..       
+0001ac30: 2020 2020 2020 2020 206f 7574 5b73 6c5d           out[sl]
+0001ac40: 203d 2069 6d67 203e 3d20 7468 720d 0a20   = img >= thr.. 
+0001ac50: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+0001ac60: 2020 2020 2020 2065 6c69 6620 6e70 2e69         elif np.i
+0001ac70: 7373 6361 6c61 7228 7468 7229 3a0d 0a20  sscalar(thr):.. 
+0001ac80: 2020 2020 2020 2020 2020 206f 7574 203d             out =
+0001ac90: 2073 656c 6620 3e3d 2074 6872 0d0a 2020   self >= thr..  
+0001aca0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001acb0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0001acc0: 7970 6545 7272 6f72 280d 0a20 2020 2020  ypeError(..     
+0001acd0: 2020 2020 2020 2020 2020 2022 2774 6872             "'thr
+0001ace0: 2720 6d75 7374 2062 6520 6e75 6d65 7269  ' must be numeri
+0001acf0: 632c 206f 7220 7374 7220 7370 6563 6966  c, or str specif
+0001ad00: 7969 6e67 2061 2074 6872 6573 686f 6c64  ying a threshold
+0001ad10: 696e 6720 6d65 7468 6f64 2e22 0d0a 2020  ing method."..  
+0001ad20: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001ad30: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+0001ad40: 6574 7572 6e20 6f75 740d 0a20 2020 200d  eturn out..    .
+0001ad50: 0a20 2020 2040 5f64 6f63 732e 7772 6974  .    @_docs.writ
+0001ad60: 655f 646f 6373 0d0a 2020 2020 4064 696d  e_docs..    @dim
+0001ad70: 735f 746f 5f73 7061 7469 616c 5f61 7865  s_to_spatial_axe
+0001ad80: 730d 0a20 2020 2040 6368 6563 6b5f 696e  s..    @check_in
+0001ad90: 7075 745f 616e 645f 6f75 7470 7574 286f  put_and_output(o
+0001ada0: 6e6c 795f 6269 6e61 7279 3d54 7275 6529  nly_binary=True)
+0001adb0: 0d0a 2020 2020 6465 6620 6469 7374 616e  ..    def distan
+0001adc0: 6365 5f6d 6170 2873 656c 662c 202a 2c20  ce_map(self, *, 
+0001add0: 6469 6d73 3a20 4469 6d73 203d 204e 6f6e  dims: Dims = Non
+0001ade0: 6529 202d 3e20 496d 6741 7272 6179 3a0d  e) -> ImgArray:.
+0001adf0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0001ae00: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
+0001ae10: 6469 7374 616e 6365 206d 6170 2066 726f  distance map fro
+0001ae20: 6d20 6269 6e61 7279 2069 6d61 6765 732e  m binary images.
+0001ae30: 0d0a 2020 2020 2020 2020 466f 7220 696e  ..        For in
+0001ae40: 7374 616e 6365 2c20 6060 5b31 2c20 312c  stance, ``[1, 1,
+0001ae50: 2031 2c20 302c 2030 2c20 302c 2031 2c20   1, 0, 0, 0, 1, 
+0001ae60: 312c 2031 5d60 6020 7769 6c6c 2062 6520  1, 1]`` will be 
+0001ae70: 636f 6e76 6572 7465 6420 746f 200d 0a20  converted to .. 
+0001ae80: 2020 2020 2020 2060 605b 332c 2032 2c20         ``[3, 2, 
+0001ae90: 312c 2030 2c20 302c 2030 2c20 312c 2032  1, 0, 0, 0, 1, 2
+0001aea0: 2c20 335d 6060 2e20 4e6f 7465 2074 6861  , 3]``. Note tha
+0001aeb0: 7420 7265 7475 726e 6564 2061 7272 6179  t returned array
+0001aec0: 2077 696c 6c20 6265 2066 6c6f 6174 2069   will be float i
+0001aed0: 6e20 6e2d 4420 0d0a 2020 2020 2020 2020  n n-D ..        
+0001aee0: 696d 6167 6573 2e0d 0a0d 0a20 2020 2020  images.....     
+0001aef0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+0001af00: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001af10: 2d0d 0a20 2020 2020 2020 207b 6469 6d73  -..        {dims
+0001af20: 7d0d 0a0d 0a20 2020 2020 2020 2052 6574  }....        Ret
+0001af30: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+0001af40: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
+0001af50: 6d67 4172 7261 790d 0a20 2020 2020 2020  mgArray..       
+0001af60: 2020 2020 2044 6973 7461 6e63 6520 6d61       Distance ma
+0001af70: 702c 2074 6865 2066 7572 7468 6572 2074  p, the further t
+0001af80: 6865 2062 7269 6768 7465 720d 0a20 2020  he brighter..   
+0001af90: 2020 2020 2022 2222 2020 2020 2020 2020       """        
+0001afa0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001afb0: 2073 656c 662e 5f61 7070 6c79 5f64 6173   self._apply_das
+0001afc0: 6b28 6e64 692e 6469 7374 616e 6365 5f74  k(ndi.distance_t
+0001afd0: 7261 6e73 666f 726d 5f65 6474 2c20 0d0a  ransform_edt, ..
+0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aff0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001b000: 5f61 7865 733d 636f 6d70 6c65 6d65 6e74  _axes=complement
+0001b010: 5f61 7865 7328 6469 6d73 2c20 7365 6c66  _axes(dims, self
+0001b020: 2e61 7865 7329 0d0a 2020 2020 2020 2020  .axes)..        
+0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b040: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001b050: 2020 0d0a 2020 2020 4064 696d 735f 746f    ..    @dims_to
+0001b060: 5f73 7061 7469 616c 5f61 7865 730d 0a20  _spatial_axes.. 
+0001b070: 2020 2040 6368 6563 6b5f 696e 7075 745f     @check_input_
+0001b080: 616e 645f 6f75 7470 7574 0d0a 2020 2020  and_output..    
+0001b090: 6465 6620 6e63 635f 6669 6c74 6572 280d  def ncc_filter(.
+0001b0a0: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
+0001b0b0: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
+0001b0c0: 3a20 6e70 2e6e 6461 7272 6179 2c0d 0a20  : np.ndarray,.. 
+0001b0d0: 2020 2020 2020 206d 6f64 653a 2073 7472         mode: str
+0001b0e0: 203d 2022 636f 6e73 7461 6e74 222c 200d   = "constant", .
+0001b0f0: 0a20 2020 2020 2020 2063 7661 6c3a 2066  .        cval: f
+0001b100: 6c6f 6174 207c 2073 7472 207c 2043 616c  loat | str | Cal
+0001b110: 6c61 626c 655b 5b6e 702e 6e64 6172 7261  lable[[np.ndarra
+0001b120: 795d 2c20 666c 6f61 745d 203d 206e 702e  y], float] = np.
+0001b130: 6d65 616e 2c20 0d0a 2020 2020 2020 2020  mean, ..        
+0001b140: 2a2c 200d 0a20 2020 2020 2020 2064 696d  *, ..        dim
+0001b150: 733a 2044 696d 7320 3d20 4e6f 6e65 0d0a  s: Dims = None..
+0001b160: 2020 2020 2920 2d3e 2049 6d67 4172 7261      ) -> ImgArra
+0001b170: 793a 0d0a 2020 2020 2020 2020 2222 220d  y:..        """.
+0001b180: 0a20 2020 2020 2020 2054 656d 706c 6174  .        Templat
+0001b190: 6520 6d61 7463 6869 6e67 2075 7369 6e67  e matching using
+0001b1a0: 206e 6f72 6d61 6c69 7a65 6420 6372 6f73   normalized cros
+0001b1b0: 7320 636f 7272 656c 6174 696f 6e20 284e  s correlation (N
+0001b1c0: 4343 2920 6d65 7468 6f64 2e20 5468 6973  CC) method. This
+0001b1d0: 2066 756e 6374 696f 6e20 6973 2062 6173   function is bas
+0001b1e0: 6963 616c 6c79 0d0a 2020 2020 2020 2020  ically..        
+0001b1f0: 6964 656e 7469 6361 6c20 746f 2074 6861  identical to tha
+0001b200: 7420 696e 2060 736b 696d 6167 652e 6665  t in `skimage.fe
+0001b210: 6174 7572 6560 2c20 6275 7420 6973 206f  ature`, but is o
+0001b220: 7074 696d 697a 6564 2066 6f72 2062 6174  ptimized for bat
+0001b230: 6368 2070 726f 6365 7373 696e 6720 616e  ch processing an
+0001b240: 6420 696d 7072 6f76 6564 200d 0a20 2020  d improved ..   
+0001b250: 2020 2020 2072 6561 6461 6269 6c69 7479       readability
+0001b260: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+0001b270: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+0001b280: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+0001b290: 2020 2020 2074 656d 706c 6174 6520 3a20       template : 
+0001b2a0: 6e70 2e6e 6461 7272 6179 0d0a 2020 2020  np.ndarray..    
+0001b2b0: 2020 2020 2020 2020 5465 6d70 6c61 7465          Template
+0001b2c0: 2069 6d61 6765 2e20 4d75 7374 2062 6520   image. Must be 
+0001b2d0: 3220 6f72 2033 2064 696d 656e 7369 6f6e  2 or 3 dimension
+0001b2e0: 616c 2e20 0d0a 2020 2020 2020 2020 7b6d  al. ..        {m
+0001b2f0: 6f64 657d 0d0a 2020 2020 2020 2020 6376  ode}..        cv
+0001b300: 616c 203a 2066 6c6f 6174 2c20 6f70 7469  al : float, opti
+0001b310: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+0001b320: 2020 4261 636b 6772 6f75 6e64 2069 6e74    Background int
+0001b330: 656e 7369 7479 2e20 4966 206e 6f74 2067  ensity. If not g
+0001b340: 6976 656e 2c20 6974 2077 696c 6c20 6361  iven, it will ca
+0001b350: 6c63 756c 6174 6564 2061 7320 7468 6520  lculated as the 
+0001b360: 6d65 616e 2076 616c 7565 206f 6620 0d0a  mean value of ..
+0001b370: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0001b380: 6f72 6967 696e 616c 2069 6d61 6765 2e0d  original image..
+0001b390: 0a20 2020 2020 2020 207b 6469 6d73 7d0d  .        {dims}.
+0001b3a0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0001b3b0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+0001b3c0: 2d2d 2d0d 0a20 2020 2020 2020 2049 6d67  ---..        Img
+0001b3d0: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
+0001b3e0: 2020 2052 6573 706f 6e73 6520 696d 6167     Response imag
+0001b3f0: 6520 7769 7468 2076 616c 7565 7320 6265  e with values be
+0001b400: 7477 6565 6e20 2d31 2061 6e64 2031 2e0d  tween -1 and 1..
+0001b410: 0a20 2020 2020 2020 2022 2222 2020 2020  .        """    
+0001b420: 2020 2020 0d0a 2020 2020 2020 2020 7465      ..        te
+0001b430: 6d70 6c61 7465 203d 205f 6368 6563 6b5f  mplate = _check_
+0001b440: 7465 6d70 6c61 7465 2874 656d 706c 6174  template(templat
+0001b450: 6529 0d0a 2020 2020 2020 2020 6966 2063  e)..        if c
+0001b460: 616c 6c61 626c 6528 6376 616c 293a 0d0a  allable(cval):..
+0001b470: 2020 2020 2020 2020 2020 2020 6376 616c              cval
+0001b480: 203d 2063 7661 6c28 7365 6c66 290d 0a20   = cval(self).. 
+0001b490: 2020 2020 2020 2063 7661 6c20 3d20 5f63         cval = _c
+0001b4a0: 6865 636b 5f62 6728 7365 6c66 2c20 6376  heck_bg(self, cv
+0001b4b0: 616c 290d 0a20 2020 2020 2020 2069 6620  al)..        if 
+0001b4c0: 6c65 6e28 6469 6d73 2920 213d 2074 656d  len(dims) != tem
+0001b4d0: 706c 6174 652e 6e64 696d 3a0d 0a20 2020  plate.ndim:..   
+0001b4e0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0001b4f0: 616c 7565 4572 726f 7228 2264 696d 7320  alueError("dims 
+0001b500: 616e 6420 7468 6520 6e75 6d62 6572 206f  and the number o
+0001b510: 6620 7465 6d70 6c61 7465 2064 696d 656e  f template dimen
+0001b520: 7369 6f6e 2064 6f6e 2774 206d 6174 6368  sion don't match
+0001b530: 2e22 290d 0a20 2020 2020 2020 200d 0a20  .")..        .. 
+0001b540: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001b550: 6c66 2e61 735f 666c 6f61 7428 292e 5f61  lf.as_float()._a
+0001b560: 7070 6c79 5f64 6173 6b28 0d0a 2020 2020  pply_dask(..    
+0001b570: 2020 2020 2020 2020 5f66 696c 7465 7273          _filters
+0001b580: 2e6e 6363 5f66 696c 7465 722c 0d0a 2020  .ncc_filter,..  
+0001b590: 2020 2020 2020 2020 2020 635f 6178 6573            c_axes
+0001b5a0: 3d63 6f6d 706c 656d 656e 745f 6178 6573  =complement_axes
+0001b5b0: 2864 696d 732c 2073 656c 662e 6178 6573  (dims, self.axes
+0001b5c0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
+0001b5d0: 2061 7267 733d 2874 656d 706c 6174 652c   args=(template,
+0001b5e0: 2063 7661 6c2c 206d 6f64 6529 0d0a 2020   cval, mode)..  
+0001b5f0: 2020 2020 2020 290d 0a20 2020 200d 0a20        )..    .. 
+0001b600: 2020 2040 5f64 6f63 732e 7772 6974 655f     @_docs.write_
+0001b610: 646f 6373 0d0a 2020 2020 4064 696d 735f  docs..    @dims_
+0001b620: 746f 5f73 7061 7469 616c 5f61 7865 730d  to_spatial_axes.
+0001b630: 0a20 2020 2040 6368 6563 6b5f 696e 7075  .    @check_inpu
+0001b640: 745f 616e 645f 6f75 7470 7574 286f 6e6c  t_and_output(onl
+0001b650: 795f 6269 6e61 7279 3d54 7275 6529 0d0a  y_binary=True)..
+0001b660: 2020 2020 6465 6620 7265 6d6f 7665 5f6c      def remove_l
+0001b670: 6172 6765 5f6f 626a 6563 7473 2873 656c  arge_objects(sel
+0001b680: 662c 2072 6164 6975 733a 2066 6c6f 6174  f, radius: float
+0001b690: 203d 2035 2c20 2a2c 2064 696d 733a 2044   = 5, *, dims: D
+0001b6a0: 696d 7320 3d20 4e6f 6e65 2c20 7570 6461  ims = None, upda
+0001b6b0: 7465 3a20 626f 6f6c 203d 2046 616c 7365  te: bool = False
+0001b6c0: 2920 2d3e 2049 6d67 4172 7261 793a 0d0a  ) -> ImgArray:..
+0001b6d0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0001b6e0: 2020 2020 2052 656d 6f76 6520 6c61 7267       Remove larg
+0001b6f0: 6520 6f62 6a65 6374 7320 7573 696e 6720  e objects using 
+0001b700: 6f70 656e 696e 672e 2054 686f 7365 206f  opening. Those o
+0001b710: 626a 6563 7473 2074 6861 7420 7765 7265  bjects that were
+0001b720: 206e 6f74 2072 656d 6f76 6564 2062 7920   not removed by 
+0001b730: 6f70 656e 696e 670d 0a20 2020 2020 2020  opening..       
+0001b740: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
+0001b750: 2069 6e20 6f75 7470 7574 2e0d 0a0d 0a20   in output..... 
+0001b760: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001b770: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0001b780: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2072  -----..        r
+0001b790: 6164 6975 7320 3a20 666c 6f61 742c 206f  adius : float, o
+0001b7a0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0001b7b0: 2020 2020 204f 626a 6563 7473 2077 6974       Objects wit
+0001b7c0: 6820 7261 6469 7573 206c 6172 6765 7220  h radius larger 
+0001b7d0: 7468 616e 2074 6869 7320 7661 6c75 6520  than this value 
+0001b7e0: 7769 6c6c 2062 6520 7265 6d6f 7665 642e  will be removed.
+0001b7f0: 0d0a 2020 2020 2020 2020 7b64 696d 737d  ..        {dims}
+0001b800: 7b75 7064 6174 657d 0d0a 0d0a 2020 2020  {update}....    
+0001b810: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0001b820: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0001b830: 2020 2020 2020 496d 6741 7272 6179 0d0a        ImgArray..
+0001b840: 2020 2020 2020 2020 2020 2020 496d 6167              Imag
+0001b850: 6520 7769 7468 206c 6172 6765 206f 626a  e with large obj
+0001b860: 6563 7473 2072 656d 6f76 6564 2e0d 0a0d  ects removed....
+0001b870: 0a20 2020 2020 2020 2053 6565 2041 6c73  .        See Als
+0001b880: 6f0d 0a20 2020 2020 2020 202d 2d2d 2d2d  o..        -----
+0001b890: 2d2d 2d0d 0a20 2020 2020 2020 2072 656d  ---..        rem
+0001b8a0: 6f76 655f 6669 6e65 5f6f 626a 6563 7473  ove_fine_objects
+0001b8b0: 0d0a 2020 2020 2020 2020 2222 2220 2020  ..        """   
+0001b8c0: 2020 2020 200d 0a20 2020 2020 2020 206f       ..        o
+0001b8d0: 7574 203d 2073 656c 662e 636f 7079 2829  ut = self.copy()
+0001b8e0: 0d0a 2020 2020 2020 2020 6c61 7267 655f  ..        large_
+0001b8f0: 6f62 6a20 3d20 7365 6c66 2e6f 7065 6e69  obj = self.openi
+0001b900: 6e67 2872 6164 6975 732c 2064 696d 733d  ng(radius, dims=
+0001b910: 6469 6d73 290d 0a20 2020 2020 2020 206f  dims)..        o
+0001b920: 7574 2e76 616c 7565 5b6c 6172 6765 5f6f  ut.value[large_o
+0001b930: 626a 5d20 3d20 300d 0a20 2020 2020 2020  bj] = 0..       
+0001b940: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+0001b950: 6574 7572 6e20 6f75 740d 0a20 2020 200d  eturn out..    .
+0001b960: 0a20 2020 2040 5f64 6f63 732e 7772 6974  .    @_docs.writ
+0001b970: 655f 646f 6373 0d0a 2020 2020 4064 696d  e_docs..    @dim
+0001b980: 735f 746f 5f73 7061 7469 616c 5f61 7865  s_to_spatial_axe
+0001b990: 730d 0a20 2020 2040 6368 6563 6b5f 696e  s..    @check_in
+0001b9a0: 7075 745f 616e 645f 6f75 7470 7574 286f  put_and_output(o
+0001b9b0: 6e6c 795f 6269 6e61 7279 3d54 7275 6529  nly_binary=True)
+0001b9c0: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+0001b9d0: 5f66 696e 655f 6f62 6a65 6374 7328 7365  _fine_objects(se
+0001b9e0: 6c66 2c20 6c65 6e67 7468 3a20 666c 6f61  lf, length: floa
+0001b9f0: 7420 3d20 3130 2c20 2a2c 2064 696d 733a  t = 10, *, dims:
+0001ba00: 2044 696d 7320 3d20 4e6f 6e65 2c20 7570   Dims = None, up
+0001ba10: 6461 7465 3a20 626f 6f6c 203d 2046 616c  date: bool = Fal
+0001ba20: 7365 2920 2d3e 2049 6d67 4172 7261 793a  se) -> ImgArray:
+0001ba30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0001ba40: 2020 2020 2020 2052 656d 6f76 6520 6669         Remove fi
+0001ba50: 6e65 206f 626a 6563 7473 2075 7369 6e67  ne objects using
+0001ba60: 2064 6961 6d65 7465 725f 6f70 656e 696e   diameter_openin
+0001ba70: 672e 0d0a 0d0a 2020 2020 2020 2020 5061  g.....        Pa
+0001ba80: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+0001ba90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+0001baa0: 2020 2020 2020 6c65 6e67 7468 203a 2066        length : f
+0001bab0: 6c6f 6174 2c20 6465 6661 756c 7420 6973  loat, default is
+0001bac0: 2031 300d 0a20 2020 2020 2020 2020 2020   10..           
+0001bad0: 204f 626a 6563 7473 206c 6f6e 6765 7220   Objects longer 
+0001bae0: 7468 616e 2074 6869 7320 7769 6c6c 2062  than this will b
+0001baf0: 6520 7265 6d6f 7665 642e 0d0a 2020 2020  e removed...    
+0001bb00: 2020 2020 7b64 696d 737d 7b75 7064 6174      {dims}{updat
+0001bb10: 657d 0d0a 0d0a 2020 2020 2020 2020 5265  e}....        Re
+0001bb20: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0001bb30: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0001bb40: 496d 6741 7272 6179 0d0a 2020 2020 2020  ImgArray..      
+0001bb50: 2020 2020 2020 496d 6167 6520 7769 7468        Image with
+0001bb60: 206c 6172 6765 206f 626a 6563 7473 2072   large objects r
+0001bb70: 656d 6f76 6564 2e0d 0a20 2020 2020 2020  emoved...       
+0001bb80: 200d 0a20 2020 2020 2020 2053 6565 2041   ..        See A
+0001bb90: 6c73 6f0d 0a20 2020 2020 2020 202d 2d2d  lso..        ---
+0001bba0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2072  -----..        r
+0001bbb0: 656d 6f76 655f 6c61 7267 655f 6f62 6a65  emove_large_obje
+0001bbc0: 6374 730d 0a20 2020 2020 2020 2022 2222  cts..        """
+0001bbd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001bbe0: 2020 6f75 7420 3d20 7365 6c66 2e63 6f70    out = self.cop
+0001bbf0: 7928 290d 0a20 2020 2020 2020 2066 696e  y()..        fin
+0001bc00: 655f 6f62 6a20 3d20 7365 6c66 2e64 6961  e_obj = self.dia
+0001bc10: 6d65 7465 725f 6f70 656e 696e 6728 6c65  meter_opening(le
+0001bc20: 6e67 7468 2c20 636f 6e6e 6563 7469 7669  ngth, connectivi
+0001bc30: 7479 3d6c 656e 2864 696d 7329 290d 0a20  ty=len(dims)).. 
+0001bc40: 2020 2020 2020 206c 6172 6765 5f6f 626a         large_obj
+0001bc50: 203d 2073 656c 662e 6f70 656e 696e 6728   = self.opening(
+0001bc60: 6c65 6e67 7468 2f2f 3229 0d0a 2020 2020  length//2)..    
+0001bc70: 2020 2020 6f75 742e 7661 6c75 655b 7e6c      out.value[~l
+0001bc80: 6172 6765 5f6f 626a 2026 2066 696e 655f  arge_obj & fine_
+0001bc90: 6f62 6a5d 203d 2030 0d0a 2020 2020 2020  obj] = 0..      
+0001bca0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001bcb0: 7265 7475 726e 206f 7574 0d0a 2020 2020  return out..    
+0001bcc0: 0d0a 2020 2020 405f 646f 6373 2e77 7269  ..    @_docs.wri
+0001bcd0: 7465 5f64 6f63 730d 0a20 2020 2040 6469  te_docs..    @di
+0001bce0: 6d73 5f74 6f5f 7370 6174 6961 6c5f 6178  ms_to_spatial_ax
+0001bcf0: 6573 0d0a 2020 2020 4063 6865 636b 5f69  es..    @check_i
+0001bd00: 6e70 7574 5f61 6e64 5f6f 7574 7075 7428  nput_and_output(
+0001bd10: 6f6e 6c79 5f62 696e 6172 793d 5472 7565  only_binary=True
+0001bd20: 290d 0a20 2020 2064 6566 2063 6f6e 7665  )..    def conve
+0001bd30: 785f 6875 6c6c 2873 656c 662c 202a 2c20  x_hull(self, *, 
+0001bd40: 6469 6d73 3a20 4469 6d73 203d 204e 6f6e  dims: Dims = Non
+0001bd50: 652c 2075 7064 6174 653d 4661 6c73 6529  e, update=False)
+0001bd60: 202d 3e20 496d 6741 7272 6179 3a0d 0a20   -> ImgArray:.. 
+0001bd70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0001bd80: 2020 2020 436f 6d70 7574 6520 636f 6e76      Compute conv
 0001bd90: 6578 2068 756c 6c20 696d 6167 652e 0d0a  ex hull image...
-0001bda0: 2020 2020 2020 2020 2222 2220 2020 2020          """     
-0001bdb0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001bdc0: 7572 6e20 7365 6c66 2e5f 6170 706c 795f  urn self._apply_
-0001bdd0: 6461 736b 280d 0a20 2020 2020 2020 2020  dask(..         
-0001bde0: 2020 2073 6b69 6d61 6765 2e6d 6f72 7068     skimage.morph
-0001bdf0: 6f6c 6f67 792e 636f 6e76 6578 5f68 756c  ology.convex_hul
-0001be00: 6c5f 696d 6167 652c 200d 0a20 2020 2020  l_image, ..     
-0001be10: 2020 2020 2020 2063 5f61 7865 733d 636f         c_axes=co
-0001be20: 6d70 6c65 6d65 6e74 5f61 7865 7328 6469  mplement_axes(di
-0001be30: 6d73 2c20 7365 6c66 2e61 7865 7329 2c20  ms, self.axes), 
-0001be40: 0d0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
-0001be50: 7970 653d 626f 6f6c 2c0d 0a20 2020 2020  ype=bool,..     
-0001be60: 2020 2029 2e61 7374 7970 6528 626f 6f6c     ).astype(bool
-0001be70: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-0001be80: 2040 5f64 6f63 732e 7772 6974 655f 646f   @_docs.write_do
-0001be90: 6373 0d0a 2020 2020 4064 696d 735f 746f  cs..    @dims_to
-0001bea0: 5f73 7061 7469 616c 5f61 7865 730d 0a20  _spatial_axes.. 
-0001beb0: 2020 2040 6368 6563 6b5f 696e 7075 745f     @check_input_
-0001bec0: 616e 645f 6f75 7470 7574 286f 6e6c 795f  and_output(only_
-0001bed0: 6269 6e61 7279 3d54 7275 6529 0d0a 2020  binary=True)..  
-0001bee0: 2020 6465 6620 736b 656c 6574 6f6e 697a    def skeletoniz
-0001bef0: 6528 7365 6c66 2c20 7261 6469 7573 3a20  e(self, radius: 
-0001bf00: 666c 6f61 7420 3d20 302c 202a 2c20 6469  float = 0, *, di
-0001bf10: 6d73 3a20 4469 6d73 203d 204e 6f6e 652c  ms: Dims = None,
-0001bf20: 2075 7064 6174 653d 4661 6c73 6529 202d   update=False) -
-0001bf30: 3e20 496d 6741 7272 6179 3a0d 0a20 2020  > ImgArray:..   
-0001bf40: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0001bf50: 2020 536b 656c 6574 6f6e 697a 6520 696d    Skeletonize im
-0001bf60: 6167 6573 2e20 4f6e 6c79 2077 6f72 6b73  ages. Only works
-0001bf70: 2066 6f72 2062 696e 6172 7920 696d 6167   for binary imag
-0001bf80: 6573 2e0d 0a0d 0a20 2020 2020 2020 2050  es.....        P
-0001bf90: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0001bfa0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-0001bfb0: 2020 2020 2020 2072 6164 6975 7320 3a20         radius : 
-0001bfc0: 666c 6f61 742c 206f 7074 696f 6e61 6c0d  float, optional.
-0001bfd0: 0a20 2020 2020 2020 2020 2020 2052 6164  .            Rad
-0001bfe0: 6975 7320 6f66 2073 6b65 6c65 746f 6e2e  ius of skeleton.
-0001bff0: 2054 6869 7320 6973 2061 6368 6965 7665   This is achieve
-0001c000: 6420 7369 6d70 6c79 2062 7920 6469 6c61  d simply by dila
-0001c010: 7469 6f6e 206f 6620 736b 656c 6574 6f6e  tion of skeleton
-0001c020: 697a 6564 2072 6573 756c 7473 2e0d 0a20  ized results... 
-0001c030: 2020 2020 2020 207b 6469 6d73 7d7b 7570         {dims}{up
-0001c040: 6461 7465 7d0d 0a0d 0a20 2020 2020 2020  date}....       
-0001c050: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0001c060: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0001c070: 2020 2049 6d67 4172 7261 790d 0a20 2020     ImgArray..   
-0001c080: 2020 2020 2020 2020 2053 6b65 6c65 746f           Skeleto
-0001c090: 6e69 7a65 6420 696d 6167 652e 0d0a 2020  nized image...  
-0001c0a0: 2020 2020 2020 2222 2220 2020 2020 2020        """       
-0001c0b0: 200d 0a20 2020 2020 2020 2069 6620 7261   ..        if ra
-0001c0c0: 6469 7573 203e 3d20 313a 0d0a 2020 2020  dius >= 1:..    
-0001c0d0: 2020 2020 2020 2020 7365 6c65 6d20 3d20          selem = 
-0001c0e0: 7870 2e61 736e 756d 7079 285f 7374 7275  xp.asnumpy(_stru
-0001c0f0: 6374 7572 6573 2e62 616c 6c5f 6c69 6b65  ctures.ball_like
-0001c100: 2872 6164 6975 732c 206c 656e 2864 696d  (radius, len(dim
-0001c110: 7329 2929 0d0a 2020 2020 2020 2020 656c  s)))..        el
-0001c120: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001c130: 2073 656c 656d 203d 204e 6f6e 650d 0a20   selem = None.. 
-0001c140: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001c150: 2072 6574 7572 6e20 7365 6c66 2e5f 6170   return self._ap
-0001c160: 706c 795f 6461 736b 280d 0a20 2020 2020  ply_dask(..     
-0001c170: 2020 2020 2020 205f 6669 6c74 6572 732e         _filters.
-0001c180: 736b 656c 6574 6f6e 697a 652c 200d 0a20  skeletonize, .. 
-0001c190: 2020 2020 2020 2020 2020 2063 5f61 7865             c_axe
-0001c1a0: 733d 636f 6d70 6c65 6d65 6e74 5f61 7865  s=complement_axe
-0001c1b0: 7328 6469 6d73 2c20 7365 6c66 2e61 7865  s(dims, self.axe
-0001c1c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0001c1d0: 2061 7267 733d 2873 656c 656d 2c29 2c0d   args=(selem,),.
-0001c1e0: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
-0001c1f0: 7065 3d62 6f6f 6c0d 0a20 2020 2020 2020  pe=bool..       
-0001c200: 2029 2e61 7374 7970 6528 626f 6f6c 290d   ).astype(bool).
-0001c210: 0a20 2020 2020 2020 200d 0a20 2020 2040  .        ..    @
-0001c220: 5f64 6f63 732e 7772 6974 655f 646f 6373  _docs.write_docs
-0001c230: 0d0a 2020 2020 4064 696d 735f 746f 5f73  ..    @dims_to_s
-0001c240: 7061 7469 616c 5f61 7865 730d 0a20 2020  patial_axes..   
-0001c250: 2040 6368 6563 6b5f 696e 7075 745f 616e   @check_input_an
-0001c260: 645f 6f75 7470 7574 286f 6e6c 795f 6269  d_output(only_bi
-0001c270: 6e61 7279 3d54 7275 6529 0d0a 2020 2020  nary=True)..    
-0001c280: 6465 6620 636f 756e 745f 6e65 6967 6862  def count_neighb
-0001c290: 6f72 7328 0d0a 2020 2020 2020 2020 7365  ors(..        se
-0001c2a0: 6c66 2c0d 0a20 2020 2020 2020 202a 2c20  lf,..        *, 
-0001c2b0: 0d0a 2020 2020 2020 2020 636f 6e6e 6563  ..        connec
-0001c2c0: 7469 7669 7479 3a20 696e 7420 7c20 4e6f  tivity: int | No
-0001c2d0: 6e65 203d 204e 6f6e 652c 0d0a 2020 2020  ne = None,..    
-0001c2e0: 2020 2020 6d61 736b 3a20 626f 6f6c 203d      mask: bool =
-0001c2f0: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-0001c300: 6469 6d73 3a20 4469 6d73 203d 204e 6f6e  dims: Dims = Non
-0001c310: 652c 0d0a 2020 2020 2920 2d3e 2049 6d67  e,..    ) -> Img
-0001c320: 4172 7261 793a 0d0a 2020 2020 2020 2020  Array:..        
-0001c330: 2222 220d 0a20 2020 2020 2020 2043 6f75  """..        Cou
-0001c340: 6e74 2074 6865 206e 756d 6265 7220 6f72  nt the number or
-0001c350: 206e 6569 6768 626f 7273 206f 6620 6269   neighbors of bi
-0001c360: 6e61 7279 2069 6d61 6765 732e 2054 6869  nary images. Thi
-0001c370: 7320 6675 6e63 7469 6f6e 2063 616e 2062  s function can b
-0001c380: 6520 7573 6564 2066 6f72 2063 726f 7373  e used for cross
-0001c390: 2073 6563 7469 6f6e 0d0a 2020 2020 2020   section..      
-0001c3a0: 2020 6f72 2062 7261 6e63 6820 6465 7465    or branch dete
-0001c3b0: 6374 696f 6e2e 204f 6e6c 7920 776f 726b  ction. Only work
-0001c3c0: 7320 666f 7220 6269 6e61 7279 2069 6d61  s for binary ima
-0001c3d0: 6765 732e 0d0a 0d0a 2020 2020 2020 2020  ges.....        
-0001c3e0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0001c3f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-0001c400: 2020 2020 2020 2020 7b63 6f6e 6e65 6374          {connect
-0001c410: 6976 6974 797d 0d0a 2020 2020 2020 2020  ivity}..        
-0001c420: 6d61 736b 203a 2062 6f6f 6c2c 2064 6566  mask : bool, def
-0001c430: 6175 6c74 2069 7320 5472 7565 0d0a 2020  ault is True..  
-0001c440: 2020 2020 2020 2020 2020 4966 2054 7275            If Tru
-0001c450: 652c 206f 6e6c 7920 6e65 6967 6862 6f72  e, only neighbor
-0001c460: 7320 6f66 2070 6978 656c 7320 7468 6174  s of pixels that
-0001c470: 2073 6174 6973 6679 2073 656c 663d 3d54   satisfy self==T
-0001c480: 7275 6520 6973 2072 6574 7572 6e65 642e  rue is returned.
-0001c490: 0d0a 2020 2020 2020 2020 7b64 696d 737d  ..        {dims}
-0001c4a0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0001c4b0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-0001c4c0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 496d  ----..        Im
-0001c4d0: 6741 7272 6179 0d0a 2020 2020 2020 2020  gArray..        
-0001c4e0: 2020 2020 7569 6e74 3820 6172 7261 7920      uint8 array 
-0001c4f0: 6f66 2074 6865 206e 756d 6265 7220 6f66  of the number of
-0001c500: 206e 6569 6768 626f 7273 2e0d 0a20 2020   neighbors...   
-0001c510: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001c520: 2020 2045 7861 6d70 6c65 730d 0a20 2020     Examples..   
-0001c530: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-0001c540: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
-0001c550: 6b6c 203d 2069 6d67 2e74 6872 6573 686f  kl = img.thresho
-0001c560: 6c64 2829 2e73 6b65 6c65 746f 6e69 7a65  ld().skeletonize
-0001c570: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0001c580: 3e3e 3e20 6564 6765 203d 2073 6b6c 2e63  >>> edge = skl.c
-0001c590: 6f75 6e74 5f6e 6569 6768 626f 7273 2829  ount_neighbors()
-0001c5a0: 0d0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-0001c5b0: 3e20 6e70 2e61 7267 7768 6572 6528 6564  > np.argwhere(ed
-0001c5c0: 6765 203d 3d20 3129 2023 2067 6574 2063  ge == 1) # get c
-0001c5d0: 6f6f 7264 696e 6174 6573 206f 6620 6669  oordinates of fi
-0001c5e0: 6c61 6d65 6e74 2065 6467 6573 2e0d 0a20  lament edges... 
-0001c5f0: 2020 2020 2020 2020 2020 203e 3e3e 206e             >>> n
-0001c600: 702e 6172 6777 6865 7265 2865 6467 6520  p.argwhere(edge 
-0001c610: 3e3d 2033 2920 2320 6765 7420 636f 6f72  >= 3) # get coor
-0001c620: 6469 6e61 7465 7320 6f66 2066 696c 616d  dinates of filam
-0001c630: 656e 7420 6372 6f73 7320 7365 6374 696f  ent cross sectio
-0001c640: 6e73 2e0d 0a20 2020 2020 2020 200d 0a20  ns...        .. 
-0001c650: 2020 2020 2020 2022 2222 2020 2020 2020         """      
-0001c660: 2020 0d0a 2020 2020 2020 2020 6e64 696d    ..        ndim
-0001c670: 203d 206c 656e 2864 696d 7329 0d0a 2020   = len(dims)..  
-0001c680: 2020 2020 2020 636f 6e6e 6563 7469 7669        connectivi
-0001c690: 7479 203d 206e 6469 6d20 6966 2063 6f6e  ty = ndim if con
-0001c6a0: 6e65 6374 6976 6974 7920 6973 204e 6f6e  nectivity is Non
-0001c6b0: 6520 656c 7365 2063 6f6e 6e65 6374 6976  e else connectiv
-0001c6c0: 6974 790d 0a20 2020 2020 2020 2073 656c  ity..        sel
-0001c6d0: 656d 203d 206e 6469 2e6d 6f72 7068 6f6c  em = ndi.morphol
-0001c6e0: 6f67 792e 6765 6e65 7261 7465 5f62 696e  ogy.generate_bin
-0001c6f0: 6172 795f 7374 7275 6374 7572 6528 6e64  ary_structure(nd
-0001c700: 696d 2c20 636f 6e6e 6563 7469 7669 7479  im, connectivity
-0001c710: 290d 0a20 2020 2020 2020 2073 656c 656d  )..        selem
-0001c720: 5b28 312c 292a 6e64 696d 5d20 3d20 300d  [(1,)*ndim] = 0.
-0001c730: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001c740: 656c 662e 6173 5f75 696e 7438 2829 2e5f  elf.as_uint8()._
-0001c750: 6170 706c 795f 6461 736b 280d 0a20 2020  apply_dask(..   
-0001c760: 2020 2020 2020 2020 205f 6669 6c74 6572           _filter
-0001c770: 732e 706f 7075 6c61 7469 6f6e 2c20 0d0a  s.population, ..
-0001c780: 2020 2020 2020 2020 2020 2020 635f 6178              c_ax
-0001c790: 6573 3d63 6f6d 706c 656d 656e 745f 6178  es=complement_ax
-0001c7a0: 6573 2864 696d 732c 2073 656c 662e 6178  es(dims, self.ax
-0001c7b0: 6573 292c 200d 0a20 2020 2020 2020 2020  es), ..         
-0001c7c0: 2020 2061 7267 733d 2873 656c 656d 2c29     args=(selem,)
-0001c7d0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-0001c7e0: 2020 2020 2069 6620 6d61 736b 3a0d 0a20       if mask:.. 
-0001c7f0: 2020 2020 2020 2020 2020 206f 7574 5b7e             out[~
-0001c800: 7365 6c66 2e76 616c 7565 5d20 3d20 300d  self.value] = 0.
-0001c810: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001c820: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0001c830: 742e 6173 7479 7065 286e 702e 7569 6e74  t.astype(np.uint
-0001c840: 3829 0d0a 2020 2020 0d0a 2020 2020 405f  8)..    ..    @_
-0001c850: 646f 6373 2e77 7269 7465 5f64 6f63 730d  docs.write_docs.
-0001c860: 0a20 2020 2040 6469 6d73 5f74 6f5f 7370  .    @dims_to_sp
-0001c870: 6174 6961 6c5f 6178 6573 0d0a 2020 2020  atial_axes..    
-0001c880: 4063 6865 636b 5f69 6e70 7574 5f61 6e64  @check_input_and
-0001c890: 5f6f 7574 7075 7428 6f6e 6c79 5f62 696e  _output(only_bin
-0001c8a0: 6172 793d 5472 7565 290d 0a20 2020 2064  ary=True)..    d
-0001c8b0: 6566 2072 656d 6f76 655f 736b 656c 6574  ef remove_skelet
-0001c8c0: 6f6e 5f73 7472 7563 7475 7265 280d 0a20  on_structure(.. 
-0001c8d0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-0001c8e0: 2020 2020 2020 7374 7275 6374 7572 653a        structure:
-0001c8f0: 204c 6974 6572 616c 5b22 7469 7022 2c20   Literal["tip", 
-0001c900: 2262 7261 6e63 6822 2c20 2263 726f 7373  "branch", "cross
-0001c910: 225d 203d 2022 7469 7022 2c0d 0a20 2020  "] = "tip",..   
-0001c920: 2020 2020 202a 2c0d 0a20 2020 2020 2020       *,..       
-0001c930: 2063 6f6e 6e65 6374 6976 6974 793a 2069   connectivity: i
-0001c940: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
-0001c950: 2020 2020 6469 6d73 3a20 4469 6d73 203d      dims: Dims =
-0001c960: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0001c970: 7570 6461 7465 3a20 626f 6f6c 203d 2046  update: bool = F
-0001c980: 616c 7365 2c0d 0a20 2020 2029 202d 3e20  alse,..    ) -> 
-0001c990: 496d 6741 7272 6179 3a0d 0a20 2020 2020  ImgArray:..     
-0001c9a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0001c9b0: 5265 6d6f 7665 2063 6572 7461 696e 2073  Remove certain s
-0001c9c0: 7472 7563 7475 7265 2066 726f 6d20 736b  tructure from sk
-0001c9d0: 656c 6574 6f6e 697a 6564 2069 6d61 6765  eletonized image
-0001c9e0: 732e 0d0a 0d0a 2020 2020 2020 2020 5061  s.....        Pa
-0001c9f0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-0001ca00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-0001ca10: 2020 2020 2020 7374 7275 6374 7572 6520        structure 
-0001ca20: 3a20 7374 722c 2064 6566 6175 6c74 2069  : str, default i
-0001ca30: 7320 2274 6970 220d 0a20 2020 2020 2020  s "tip"..       
-0001ca40: 2020 2020 2057 6861 7420 7479 7065 206f       What type o
-0001ca50: 6620 7374 7275 6374 7572 6520 746f 2072  f structure to r
-0001ca60: 656d 6f76 652e 0d0a 2020 2020 2020 2020  emove...        
-0001ca70: 7b63 6f6e 6e65 6374 6976 6974 797d 0d0a  {connectivity}..
-0001ca80: 2020 2020 2020 2020 7b64 696d 737d 7b75          {dims}{u
-0001ca90: 7064 6174 657d 0d0a 0d0a 2020 2020 2020  pdate}....      
-0001caa0: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-0001cab0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-0001cac0: 2020 2020 496d 6741 7272 6179 0d0a 2020      ImgArray..  
-0001cad0: 2020 2020 2020 2020 2020 5072 6f63 6573            Proces
-0001cae0: 7365 6420 696d 6167 652e 0d0a 2020 2020  sed image...    
-0001caf0: 2020 2020 2222 2220 2020 2020 2020 200d      """        .
-0001cb00: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001cb10: 656c 662e 636f 7079 2829 0d0a 2020 2020  elf.copy()..    
-0001cb20: 2020 2020 6e65 6967 6862 6f72 203d 2073      neighbor = s
-0001cb30: 656c 662e 636f 756e 745f 6e65 6967 6862  elf.count_neighb
-0001cb40: 6f72 7328 636f 6e6e 6563 7469 7669 7479  ors(connectivity
-0001cb50: 3d63 6f6e 6e65 6374 6976 6974 792c 2064  =connectivity, d
-0001cb60: 696d 733d 6469 6d73 290d 0a20 2020 2020  ims=dims)..     
-0001cb70: 2020 2069 6620 7374 7275 6374 7572 6520     if structure 
-0001cb80: 3d3d 2022 7469 7022 3a0d 0a20 2020 2020  == "tip":..     
-0001cb90: 2020 2020 2020 2073 6c20 3d20 6e65 6967         sl = neig
-0001cba0: 6862 6f72 203d 3d20 310d 0a20 2020 2020  hbor == 1..     
-0001cbb0: 2020 2065 6c69 6620 7374 7275 6374 7572     elif structur
-0001cbc0: 6520 3d3d 2022 6272 616e 6368 223a 0d0a  e == "branch":..
-0001cbd0: 2020 2020 2020 2020 2020 2020 736c 203d              sl =
-0001cbe0: 206e 6569 6768 626f 7220 3e20 320d 0a20   neighbor > 2.. 
-0001cbf0: 2020 2020 2020 2065 6c69 6620 7374 7275         elif stru
-0001cc00: 6374 7572 6520 3d3d 2022 6372 6f73 7322  cture == "cross"
-0001cc10: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0001cc20: 6c20 3d20 6e65 6967 6862 6f72 203e 2033  l = neighbor > 3
-0001cc30: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001cc40: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001cc50: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
-0001cc60: 6d6f 6465 6020 6d75 7374 2062 6520 6f6e  mode` must be on
-0001cc70: 6520 6f66 207b 2774 6970 272c 2027 6272  e of {'tip', 'br
-0001cc80: 616e 6368 272c 2027 6372 6f73 7327 7d2e  anch', 'cross'}.
-0001cc90: 2229 0d0a 2020 2020 2020 2020 6f75 742e  ")..        out.
-0001cca0: 7661 6c75 655b 736c 5d20 3d20 300d 0a20  value[sl] = 0.. 
-0001ccb0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0001ccc0: 740d 0a20 2020 200d 0a20 2020 2040 6469  t..    ..    @di
-0001ccd0: 6d73 5f74 6f5f 7370 6174 6961 6c5f 6178  ms_to_spatial_ax
-0001cce0: 6573 0d0a 2020 2020 4063 6865 636b 5f69  es..    @check_i
-0001ccf0: 6e70 7574 5f61 6e64 5f6f 7574 7075 7428  nput_and_output(
-0001cd00: 6e65 6564 5f6c 6162 656c 733d 5472 7565  need_labels=True
-0001cd10: 290d 0a20 2020 2064 6566 2077 6174 6572  )..    def water
-0001cd20: 7368 6564 280d 0a20 2020 2020 2020 2073  shed(..        s
-0001cd30: 656c 662c 0d0a 2020 2020 2020 2020 636f  elf,..        co
-0001cd40: 6f72 6473 3a20 4d61 726b 6572 4672 616d  ords: MarkerFram
-0001cd50: 6520 7c20 4e6f 6e65 203d 204e 6f6e 652c  e | None = None,
-0001cd60: 0d0a 2020 2020 2020 2020 2a2c 0d0a 2020  ..        *,..  
-0001cd70: 2020 2020 2020 636f 6e6e 6563 7469 7669        connectivi
-0001cd80: 7479 3a20 696e 7420 3d20 312c 0d0a 2020  ty: int = 1,..  
-0001cd90: 2020 2020 2020 696e 7075 743a 204c 6974        input: Lit
-0001cda0: 6572 616c 5b22 7365 6c66 222c 2022 6469  eral["self", "di
-0001cdb0: 7374 616e 6365 225d 203d 2022 6469 7374  stance"] = "dist
-0001cdc0: 616e 6365 222c 200d 0a20 2020 2020 2020  ance", ..       
-0001cdd0: 206d 696e 5f64 6973 7461 6e63 653a 2066   min_distance: f
-0001cde0: 6c6f 6174 203d 2032 2c0d 0a20 2020 2020  loat = 2,..     
-0001cdf0: 2020 2064 696d 733a 2044 696d 7320 3d20     dims: Dims = 
-0001ce00: 4e6f 6e65 2c0d 0a20 2020 2029 202d 3e20  None,..    ) -> 
-0001ce10: 4c61 6265 6c3a 0d0a 2020 2020 2020 2020  Label:..        
-0001ce20: 2222 220d 0a20 2020 2020 2020 204c 6162  """..        Lab
-0001ce30: 656c 2073 6567 6d65 6e74 6174 696f 6e20  el segmentation 
-0001ce40: 7573 696e 6720 7761 7465 7273 6865 6420  using watershed 
-0001ce50: 616c 676f 7269 7468 6d2e 0d0a 0d0a 2020  algorithm.....  
-0001ce60: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0001ce70: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-0001ce80: 2d2d 2d2d 0d0a 2020 2020 2020 2020 636f  ----..        co
-0001ce90: 6f72 6473 203a 204d 6172 6b65 7246 7261  ords : MarkerFra
-0001cea0: 6d65 2c20 6f70 7469 6f6e 616c 0d0a 2020  me, optional..  
-0001ceb0: 2020 2020 2020 2020 2020 5265 7475 726e            Return
-0001cec0: 6564 2062 7920 7375 6368 2061 7320 6070  ed by such as `p
-0001ced0: 6561 6b5f 6c6f 6361 6c5f 6d61 7828 2960  eak_local_max()`
-0001cee0: 2e20 4172 7261 7920 6f66 2063 6f6f 7264  . Array of coord
-0001cef0: 696e 6174 6573 206f 6620 7065 616b 732e  inates of peaks.
-0001cf00: 0d0a 2020 2020 2020 2020 7b63 6f6e 6e65  ..        {conne
-0001cf10: 6374 6976 6974 797d 0d0a 2020 2020 2020  ctivity}..      
-0001cf20: 2020 696e 7075 7420 3a20 7374 722c 206f    input : str, o
-0001cf30: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0001cf40: 2020 2020 2057 6861 7420 696d 6167 6520       What image 
-0001cf50: 7769 6c6c 2062 6520 7468 6520 696e 7075  will be the inpu
-0001cf60: 7420 6f66 2077 6174 6572 7368 6564 2061  t of watershed a
-0001cf70: 6c67 6f72 6974 686d 2e20 2020 2020 2020  lgorithm.       
-0001cf80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0001cf90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001cfa0: 202d 2022 7365 6c66 2220 2e2e 2e20 7365   - "self" ... se
-0001cfb0: 6c66 2069 7320 7573 6564 2e0d 0a20 2020  lf is used...   
-0001cfc0: 2020 2020 2020 2020 202d 2022 6469 7374           - "dist
-0001cfd0: 616e 6365 2220 2e2e 2e20 6469 7374 616e  ance" ... distan
-0001cfe0: 6365 206d 6170 206f 6620 7365 6c66 2e6c  ce map of self.l
-0001cff0: 6162 656c 7320 6973 2075 7365 642e 0d0a  abels is used...
-0001d000: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0001d010: 2020 2020 2020 7b64 696d 737d 0d0a 2020        {dims}..  
-0001d020: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001d030: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-0001d040: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-0001d050: 2020 2020 2020 4c61 6265 6c0d 0a20 2020        Label..   
-0001d060: 2020 2020 2020 2020 2055 7064 6174 6564           Updated
-0001d070: 206c 6162 656c 732e 0d0a 2020 2020 2020   labels...      
-0001d080: 2020 2222 220d 0a20 2020 2020 2020 200d    """..        .
-0001d090: 0a20 2020 2020 2020 2023 2050 7265 7061  .        # Prepa
-0001d0a0: 7265 2074 6865 2069 6e70 7574 2069 6d61  re the input ima
-0001d0b0: 6765 2e0d 0a20 2020 2020 2020 2069 6620  ge...        if 
-0001d0c0: 696e 7075 7420 3d3d 2022 7365 6c66 223a  input == "self":
-0001d0d0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0001d0e0: 7075 745f 696d 6720 3d20 7365 6c66 2e63  put_img = self.c
-0001d0f0: 6f70 7928 290d 0a20 2020 2020 2020 2065  opy()..        e
-0001d100: 6c69 6620 696e 7075 7420 3d3d 2022 6469  lif input == "di
-0001d110: 7374 616e 6365 223a 0d0a 2020 2020 2020  stance":..      
-0001d120: 2020 2020 2020 696e 7075 745f 696d 6720        input_img 
-0001d130: 3d20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  = self.__class__
-0001d140: 2873 656c 662e 6c61 6265 6c73 3e30 2c20  (self.labels>0, 
-0001d150: 6178 6573 3d73 656c 662e 6178 6573 292e  axes=self.axes).
-0001d160: 6469 7374 616e 6365 5f6d 6170 2864 696d  distance_map(dim
-0001d170: 733d 6469 6d73 290d 0a20 2020 2020 2020  s=dims)..       
-0001d180: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001d190: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0001d1a0: 7272 6f72 2822 2769 6e70 7574 5f27 206d  rror("'input_' m
-0001d1b0: 7573 7420 6265 2065 6974 6865 7220 2773  ust be either 's
-0001d1c0: 656c 6627 206f 7220 2764 6973 7461 6e63  elf' or 'distanc
-0001d1d0: 6527 2e22 290d 0a20 2020 2020 2020 2020  e'.")..         
-0001d1e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001d1f0: 2069 6620 696e 7075 745f 696d 672e 6474   if input_img.dt
-0001d200: 7970 6520 3d3d 2062 6f6f 6c3a 0d0a 2020  ype == bool:..  
-0001d210: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0001d220: 696d 6720 3d20 696e 7075 745f 696d 672e  img = input_img.
-0001d230: 6173 7479 7065 286e 702e 7569 6e74 3829  astype(np.uint8)
-0001d240: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001d250: 2020 2020 2020 2020 696e 7075 745f 696d          input_im
-0001d260: 672e 6c61 6265 6c73 203d 2073 656c 662e  g.labels = self.
-0001d270: 6c61 6265 6c73 0d0a 2020 2020 2020 2020  labels..        
-0001d280: 0d0a 2020 2020 2020 2020 6966 2063 6f6f  ..        if coo
-0001d290: 7264 7320 6973 204e 6f6e 653a 0d0a 2020  rds is None:..  
-0001d2a0: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-0001d2b0: 203d 2069 6e70 7574 5f69 6d67 2e70 6561   = input_img.pea
-0001d2c0: 6b5f 6c6f 6361 6c5f 6d61 7828 6d69 6e5f  k_local_max(min_
-0001d2d0: 6469 7374 616e 6365 3d6d 696e 5f64 6973  distance=min_dis
-0001d2e0: 7461 6e63 652c 2064 696d 733d 6469 6d73  tance, dims=dims
-0001d2f0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-0001d300: 2020 2020 206c 6162 656c 7320 3d20 6c61       labels = la
-0001d310: 7267 6573 745f 7a65 726f 7328 696e 7075  rgest_zeros(inpu
-0001d320: 745f 696d 672e 7368 6170 6529 0d0a 2020  t_img.shape)..  
-0001d330: 2020 2020 2020 7368 6170 6520 3d20 7365        shape = se
-0001d340: 6c66 2e73 697a 6573 6f66 2864 696d 7329  lf.sizesof(dims)
-0001d350: 0d0a 2020 2020 2020 2020 6e5f 6c61 6265  ..        n_labe
-0001d360: 6c73 203d 2030 0d0a 2020 2020 2020 2020  ls = 0..        
-0001d370: 635f 6178 6573 203d 2063 6f6d 706c 656d  c_axes = complem
-0001d380: 656e 745f 6178 6573 2864 696d 732c 2073  ent_axes(dims, s
-0001d390: 656c 662e 6178 6573 290d 0a20 2020 2020  elf.axes)..     
-0001d3a0: 2020 206d 6172 6b65 7273 203d 206e 702e     markers = np.
-0001d3b0: 7a65 726f 7328 7368 6170 652c 2064 7479  zeros(shape, dty
-0001d3c0: 7065 3d6c 6162 656c 732e 6474 7970 6529  pe=labels.dtype)
-0001d3d0: 2023 2070 6c61 6365 686f 6c64 6572 2066   # placeholder f
-0001d3e0: 6f72 206d 6178 696d 610d 0a20 2020 2020  or maxima..     
-0001d3f0: 2020 2066 6f72 2073 6c2c 2063 7264 2069     for sl, crd i
-0001d400: 6e20 636f 6f72 6473 2e69 7465 7228 635f  n coords.iter(c_
-0001d410: 6178 6573 293a 0d0a 2020 2020 2020 2020  axes):..        
-0001d420: 2020 2020 2320 6372 642e 7661 6c75 6573      # crd.values
-0001d430: 2069 7320 284e 2c20 3229 2061 7272 6179   is (N, 2) array
-0001d440: 2073 6f20 7475 706c 6528 6372 642e 7661   so tuple(crd.va
-0001d450: 6c75 6573 2e54 2e74 6f6c 6973 7428 2929  lues.T.tolist())
-0001d460: 2069 7320 7477 6f20 284e 2c29 206c 6973   is two (N,) lis
-0001d470: 742e 0d0a 2020 2020 2020 2020 2020 2020  t...            
-0001d480: 6372 6420 3d20 6372 642e 7661 6c75 6573  crd = crd.values
-0001d490: 2e54 2e74 6f6c 6973 7428 290d 0a20 2020  .T.tolist()..   
-0001d4a0: 2020 2020 2020 2020 206d 6172 6b65 7273           markers
-0001d4b0: 5b74 7570 6c65 2863 7264 295d 203d 206e  [tuple(crd)] = n
-0001d4c0: 702e 6172 616e 6765 2831 2c20 6c65 6e28  p.arange(1, len(
-0001d4d0: 6372 645b 305d 292b 312c 2064 7479 7065  crd[0])+1, dtype
-0001d4e0: 3d6c 6162 656c 732e 6474 7970 6529 0d0a  =labels.dtype)..
-0001d4f0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-0001d500: 6c73 5b73 6c5d 203d 2073 6b73 6567 2e77  ls[sl] = skseg.w
-0001d510: 6174 6572 7368 6564 282d 696e 7075 745f  atershed(-input_
-0001d520: 696d 672e 7661 6c75 655b 736c 5d2c 206d  img.value[sl], m
-0001d530: 6172 6b65 7273 2c20 0d0a 2020 2020 2020  arkers, ..      
-0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d560: 2020 6d61 736b 3d69 6e70 7574 5f69 6d67    mask=input_img
-0001d570: 2e6c 6162 656c 732e 7661 6c75 655b 736c  .labels.value[sl
-0001d580: 5d2c 200d 0a20 2020 2020 2020 2020 2020  ], ..           
-0001d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0001d5b0: 6e65 6374 6976 6974 793d 636f 6e6e 6563  nectivity=connec
-0001d5c0: 7469 7669 7479 290d 0a20 2020 2020 2020  tivity)..       
-0001d5d0: 2020 2020 206c 6162 656c 735b 736c 5d5b       labels[sl][
-0001d5e0: 6c61 6265 6c73 5b73 6c5d 3e30 5d20 2b3d  labels[sl]>0] +=
-0001d5f0: 206e 5f6c 6162 656c 730d 0a20 2020 2020   n_labels..     
-0001d600: 2020 2020 2020 206e 5f6c 6162 656c 7320         n_labels 
-0001d610: 3d20 6c61 6265 6c73 5b73 6c5d 2e6d 6178  = labels[sl].max
-0001d620: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0001d630: 6d61 726b 6572 735b 3a5d 203d 2030 2023  markers[:] = 0 #
-0001d640: 2072 6573 6574 2070 6c61 6365 686f 6c64   reset placehold
-0001d650: 6572 0d0a 2020 2020 2020 2020 0d0a 2020  er..        ..  
-0001d660: 2020 2020 2020 6c61 6265 6c73 203d 206c        labels = l
-0001d670: 6162 656c 732e 7669 6577 284c 6162 656c  abels.view(Label
-0001d680: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001d690: 6c61 6265 6c73 203d 206c 6162 656c 732e  labels = labels.
-0001d6a0: 6f70 7469 6d69 7a65 2829 0d0a 2020 2020  optimize()..    
-0001d6b0: 2020 2020 7365 6c66 2e6c 6162 656c 732e      self.labels.
-0001d6c0: 5f73 6574 5f69 6e66 6f28 7365 6c66 290d  _set_info(self).
-0001d6d0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0001d6e0: 6265 6c73 2e73 6574 5f73 6361 6c65 2873  bels.set_scale(s
-0001d6f0: 656c 6629 0d0a 2020 2020 2020 2020 7265  elf)..        re
-0001d700: 7475 726e 2073 656c 662e 6c61 6265 6c73  turn self.labels
-0001d710: 0d0a 2020 2020 0d0a 2020 2020 405f 646f  ..    ..    @_do
-0001d720: 6373 2e77 7269 7465 5f64 6f63 730d 0a20  cs.write_docs.. 
-0001d730: 2020 2040 6469 6d73 5f74 6f5f 7370 6174     @dims_to_spat
-0001d740: 6961 6c5f 6178 6573 0d0a 2020 2020 4063  ial_axes..    @c
-0001d750: 6865 636b 5f69 6e70 7574 5f61 6e64 5f6f  heck_input_and_o
-0001d760: 7574 7075 7428 6e65 6564 5f6c 6162 656c  utput(need_label
-0001d770: 733d 5472 7565 290d 0a20 2020 2064 6566  s=True)..    def
-0001d780: 2072 616e 646f 6d5f 7761 6c6b 6572 280d   random_walker(.
-0001d790: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001d7a0: 2020 2020 2020 2020 6265 7461 3a20 666c          beta: fl
-0001d7b0: 6f61 7420 3d20 3133 302c 0d0a 2020 2020  oat = 130,..    
-0001d7c0: 2020 2020 6d6f 6465 3a20 4c69 7465 7261      mode: Litera
-0001d7d0: 6c5b 2263 6722 2c20 2263 675f 6a22 2c20  l["cg", "cg_j", 
-0001d7e0: 2263 675f 6d67 222c 2022 6266 225d 203d  "cg_mg", "bf"] =
-0001d7f0: 2022 6367 5f6a 222c 200d 0a20 2020 2020   "cg_j", ..     
-0001d800: 2020 2074 6f6c 3a20 666c 6f61 7420 3d20     tol: float = 
-0001d810: 3165 2d33 2c20 0d0a 2020 2020 2020 2020  1e-3, ..        
-0001d820: 2a2c 0d0a 2020 2020 2020 2020 6469 6d73  *,..        dims
-0001d830: 3a20 4469 6d73 203d 204e 6f6e 652c 0d0a  : Dims = None,..
-0001d840: 2020 2020 2920 2d3e 204c 6162 656c 3a0d      ) -> Label:.
-0001d850: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0001d860: 2020 2020 2020 5261 6e64 6f6d 2077 616c        Random wal
-0001d870: 6b65 7220 7365 676d 656e 7461 7469 6f6e  ker segmentation
-0001d880: 2e20 4f6e 6c79 2077 7261 7070 6564 2073  . Only wrapped s
-0001d890: 6b69 6d61 6765 2073 6567 6d65 6e74 6174  kimage segmentat
-0001d8a0: 696f 6e2e 200d 0a20 2020 2020 2020 200d  ion. ..        .
-0001d8b0: 0a20 2020 2020 2020 2060 6073 656c 662e  .        ``self.
-0001d8c0: 6c61 6265 6c73 6060 2077 696c 6c20 6265  labels`` will be
-0001d8d0: 2073 6567 6d65 6e74 6564 2061 6e64 2075   segmented and u
-0001d8e0: 7064 6174 6564 2069 6e70 6c61 6365 2e0d  pdated inplace..
-0001d8f0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001d900: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-0001d910: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-0001d920: 2020 2062 6574 612c 206d 6f64 652c 2074     beta, mode, t
-0001d930: 6f6c 0d0a 2020 2020 2020 2020 2020 2020  ol..            
-0001d940: 7365 6520 736b 696d 6167 652e 7365 676d  see skimage.segm
-0001d950: 656e 7461 7469 6f6e 2e72 616e 646f 6d5f  entation.random_
-0001d960: 7761 6c6b 6572 0d0a 2020 2020 2020 2020  walker..        
-0001d970: 7b64 696d 737d 0d0a 0d0a 2020 2020 2020  {dims}....      
-0001d980: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-0001d990: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-0001d9a0: 2020 2020 496d 6741 7272 6179 0d0a 2020      ImgArray..  
-0001d9b0: 2020 2020 2020 2020 2020 5265 6c61 6265            Relabe
-0001d9c0: 6c65 6420 696d 6167 652e 0d0a 2020 2020  led image...    
-0001d9d0: 2020 2020 2222 2220 2020 2020 2020 200d      """        .
-0001d9e0: 0a20 2020 2020 2020 2063 5f61 7865 7320  .        c_axes 
-0001d9f0: 3d20 636f 6d70 6c65 6d65 6e74 5f61 7865  = complement_axe
-0001da00: 7328 6469 6d73 2c20 7365 6c66 2e61 7865  s(dims, self.axe
-0001da10: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
-0001da20: 2020 2020 2020 666f 7220 736c 2c20 696d        for sl, im
-0001da30: 6720 696e 2073 656c 662e 6974 6572 2863  g in self.iter(c
-0001da40: 5f61 7865 732c 2069 7372 6177 3d54 7275  _axes, israw=Tru
-0001da50: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-0001da60: 2069 6d67 2e6c 6162 656c 735b 3a5d 203d   img.labels[:] =
-0001da70: 2073 6b73 6567 2e72 616e 646f 6d5f 7761   skseg.random_wa
-0001da80: 6c6b 6572 280d 0a20 2020 2020 2020 2020  lker(..         
-0001da90: 2020 2020 2020 2069 6d67 2e76 616c 7565         img.value
-0001daa0: 2c20 696d 672e 6c61 6265 6c73 2e76 616c  , img.labels.val
-0001dab0: 7565 2c20 6265 7461 3d62 6574 612c 206d  ue, beta=beta, m
-0001dac0: 6f64 653d 6d6f 6465 2c20 746f 6c3d 746f  ode=mode, tol=to
-0001dad0: 6c0d 0a20 2020 2020 2020 2020 2020 2029  l..            )
-0001dae0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001daf0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-0001db00: 656c 732e 5f73 6574 5f69 6e66 6f28 7365  els._set_info(se
-0001db10: 6c66 290d 0a20 2020 2020 2020 2072 6574  lf)..        ret
-0001db20: 7572 6e20 7365 6c66 2e6c 6162 656c 730d  urn self.labels.
-0001db30: 0a20 2020 200d 0a20 2020 2064 6566 206c  .    ..    def l
-0001db40: 6162 656c 5f74 6872 6573 686f 6c64 280d  abel_threshold(.
-0001db50: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001db60: 2020 2020 2020 2020 7468 723a 2066 6c6f          thr: flo
-0001db70: 6174 207c 2054 6872 6561 7368 6f6c 644d  at | ThreasholdM
-0001db80: 6574 686f 6420 3d20 226f 7473 7522 2c0d  ethod = "otsu",.
-0001db90: 0a20 2020 2020 2020 2066 696c 743a 2043  .        filt: C
-0001dba0: 616c 6c61 626c 655b 2e2e 2e2c 2062 6f6f  allable[..., boo
-0001dbb0: 6c5d 207c 204e 6f6e 6520 3d20 4e6f 6e65  l] | None = None
-0001dbc0: 2c0d 0a20 2020 2020 2020 202a 2c0d 0a20  ,..        *,.. 
-0001dbd0: 2020 2020 2020 2064 696d 733a 2044 696d         dims: Dim
-0001dbe0: 7320 3d20 4e6f 6e65 2c0d 0a20 2020 2020  s = None,..     
-0001dbf0: 2020 202a 2a6b 7761 7267 732c 0d0a 2020     **kwargs,..  
-0001dc00: 2020 2920 2d3e 204c 6162 656c 3a0d 0a20    ) -> Label:.. 
-0001dc10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0001dc20: 2020 2020 4d61 6b65 206c 6162 656c 7320      Make labels 
-0001dc30: 7769 7468 2074 6872 6573 686f 6c64 2829  with threshold()
-0001dc40: 2e20 4265 2073 7572 6520 7468 6174 206b  . Be sure that k
-0001dc50: 6579 776f 7264 2061 7267 756d 656e 7420  eyword argument 
-0001dc60: 6060 6469 6d73 6060 2063 616e 2062 650d  ``dims`` can be.
-0001dc70: 0a20 2020 2020 2020 2064 6966 6665 7265  .        differe
-0001dc80: 6e74 2028 696e 206d 6f73 7420 6361 7365  nt (in most case
-0001dc90: 7320 666f 7220 3e34 4420 696d 6167 6573  s for >4D images
-0001dca0: 2920 6265 7477 6565 6e20 7468 7265 7368  ) between thresh
-0001dcb0: 6f6c 6428 2920 616e 6420 6c61 6265 6c28  old() and label(
-0001dcc0: 292e 0d0a 2020 2020 2020 2020 496e 2074  )...        In t
-0001dcd0: 6869 7320 6675 6e63 7469 6f6e 2c20 626f  his function, bo
-0001dce0: 7468 2066 756e 6374 696f 6e20 7769 6c6c  th function will
-0001dcf0: 2068 6176 6520 7468 6520 7361 6d65 2060   have the same `
-0001dd00: 6064 696d 7360 6020 666f 7220 7369 6d70  `dims`` for simp
-0001dd10: 6c69 6369 7479 2e0d 0a0d 0a20 2020 2020  licity.....     
-0001dd20: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-0001dd30: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0001dd40: 2d0d 0a20 2020 2020 2020 2074 6872 3a20  -..        thr: 
-0001dd50: 666c 6f61 7420 6f72 2073 7472 206f 7220  float or str or 
-0001dd60: 4e6f 6e65 2c20 6f70 7469 6f6e 616c 0d0a  None, optional..
-0001dd70: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-0001dd80: 7368 6f6c 6420 7661 6c75 652c 206f 7220  shold value, or 
-0001dd90: 7468 7265 7368 6f6c 6469 6e67 2061 6c67  thresholding alg
-0001dda0: 6f72 6974 686d 2e0d 0a20 2020 2020 2020  orithm...       
-0001ddb0: 207b 6469 6d73 7d0d 0a20 2020 2020 2020   {dims}..       
-0001ddc0: 202a 2a6b 7761 7267 733a 0d0a 2020 2020   **kwargs:..    
-0001ddd0: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
-0001dde0: 6172 6775 6d65 6e74 7320 7468 6174 2077  arguments that w
-0001ddf0: 696c 6c20 7061 7373 6564 2074 6f20 6675  ill passed to fu
-0001de00: 6e63 7469 6f6e 2069 6e64 6963 6174 6564  nction indicated
-0001de10: 2069 6e20 276d 6574 686f 6427 2e0d 0a20   in 'method'... 
-0001de20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001de30: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-0001de40: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-0001de50: 2020 204c 6162 656c 0d0a 2020 2020 2020     Label..      
-0001de60: 2020 2020 2020 4e65 776c 7920 6372 6561        Newly crea
-0001de70: 7465 6420 6c61 6265 6c2e 0d0a 2020 2020  ted label...    
-0001de80: 2020 2020 2222 2220 2020 2020 2020 200d      """        .
-0001de90: 0a20 2020 2020 2020 206c 6162 656c 7320  .        labels 
-0001dea0: 3d20 7365 6c66 2e74 6872 6573 686f 6c64  = self.threshold
-0001deb0: 2874 6872 3d74 6872 2c20 2a2a 6b77 6172  (thr=thr, **kwar
-0001dec0: 6773 290d 0a20 2020 2020 2020 2072 6574  gs)..        ret
-0001ded0: 7572 6e20 7365 6c66 2e6c 6162 656c 286c  urn self.label(l
-0001dee0: 6162 656c 732c 2066 696c 743d 6669 6c74  abels, filt=filt
-0001def0: 2c20 6469 6d73 3d64 696d 7329 0d0a 2020  , dims=dims)..  
-0001df00: 2020 0d0a 2020 2020 6465 6620 7265 6769    ..    def regi
-0001df10: 6f6e 7072 6f70 7328 0d0a 2020 2020 2020  onprops(..      
-0001df20: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-0001df30: 2070 726f 7065 7274 6965 733a 2049 7465   properties: Ite
-0001df40: 7261 626c 655b 7374 725d 207c 2073 7472  rable[str] | str
-0001df50: 203d 2028 226d 6561 6e5f 696e 7465 6e73   = ("mean_intens
-0001df60: 6974 7922 2c29 2c0d 0a20 2020 2020 2020  ity",),..       
-0001df70: 202a 2c20 0d0a 2020 2020 2020 2020 6578   *, ..        ex
-0001df80: 7472 615f 7072 6f70 6572 7469 6573 3a20  tra_properties: 
-0001df90: 4974 6572 6162 6c65 5b43 616c 6c61 626c  Iterable[Callabl
-0001dfa0: 655d 207c 204e 6f6e 6520 3d20 4e6f 6e65  e] | None = None
-0001dfb0: 2c0d 0a20 2020 2029 202d 3e20 4461 7461  ,..    ) -> Data
-0001dfc0: 4469 6374 5b73 7472 2c20 5072 6f70 4172  Dict[str, PropAr
-0001dfd0: 7261 795d 3a0d 0a20 2020 2020 2020 2022  ray]:..        "
-0001dfe0: 2222 0d0a 2020 2020 2020 2020 4d75 6c74  ""..        Mult
-0001dff0: 692d 6469 6d65 6e73 696f 6e61 6c20 7265  i-dimensional re
-0001e000: 6769 6f6e 2070 726f 7065 7274 7920 7175  gion property qu
-0001e010: 616e 7469 6669 6361 7469 6f6e 2e0d 0a20  antification... 
-0001e020: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001e030: 2052 756e 2073 6b69 6d61 6765 2773 2072   Run skimage's r
-0001e040: 6567 696f 6e70 726f 7073 2829 2066 756e  egionprops() fun
-0001e050: 6374 696f 6e20 616e 6420 7265 7475 726e  ction and return
-0001e060: 2074 6865 2072 6573 756c 7473 2061 7320   the results as 
-0001e070: 5072 6f70 4172 7261 792c 2073 6f0d 0a20  PropArray, so.. 
-0001e080: 2020 2020 2020 2074 6861 7420 796f 7520         that you 
-0001e090: 6361 6e20 6163 6365 7373 2075 7369 6e67  can access using
-0001e0a0: 2066 6c65 7869 626c 6520 736c 6963 696e   flexible slicin
-0001e0b0: 672e 2046 6f72 2065 7861 6d70 6c65 2c20  g. For example, 
-0001e0c0: 6966 2061 2074 6379 782d 696d 6167 6520  if a tcyx-image 
-0001e0d0: 6973 0d0a 2020 2020 2020 2020 616e 616c  is..        anal
-0001e0e0: 797a 6564 2077 6974 6820 6060 7072 6f70  yzed with ``prop
-0001e0f0: 6572 7469 6573 3d28 2258 222c 2022 5922  erties=("X", "Y"
-0001e100: 2960 602c 2074 6865 6e20 796f 7520 6361  )``, then you ca
-0001e110: 6e20 6765 7420 5827 7320 7469 6d65 2d63  n get X's time-c
-0001e120: 6f75 7273 6520 7072 6f66 696c 650d 0a20  ourse profile.. 
-0001e130: 2020 2020 2020 206f 6620 6368 616e 6e65         of channe
-0001e140: 6c20 3120 6174 206c 6162 656c 2033 2062  l 1 at label 3 b
-0001e150: 7920 6060 7072 6f70 5b22 5822 5d5b 2270  y ``prop["X"]["p
-0001e160: 3d35 3b63 3d31 225d 6060 206f 7220 6060  =5;c=1"]`` or ``
-0001e170: 7072 6f70 2e58 5b22 703d 353b 633d 3122  prop.X["p=5;c=1"
-0001e180: 5d60 602e 0d0a 0d0a 2020 2020 2020 2020  ]``.....        
-0001e190: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-0001e1a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-0001e1b0: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
-0001e1c0: 6573 203a 2069 7465 7261 626c 652c 206f  es : iterable, o
-0001e1d0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0001e1e0: 2020 2020 2070 726f 7065 7274 6965 7320       properties 
-0001e1f0: 746f 2061 6e61 6c79 7a65 2c20 7365 6520  to analyze, see 
-0001e200: 6060 736b 696d 6167 652e 6d65 6173 7572  ``skimage.measur
-0001e210: 652e 7265 6769 6f6e 7072 6f70 7360 602e  e.regionprops``.
-0001e220: 0d0a 2020 2020 2020 2020 6578 7472 615f  ..        extra_
-0001e230: 7072 6f70 6572 7469 6573 203a 2069 7465  properties : ite
-0001e240: 7261 626c 6520 6f66 2063 616c 6c61 626c  rable of callabl
-0001e250: 652c 206f 7074 696f 6e61 6c0d 0a20 2020  e, optional..   
-0001e260: 2020 2020 2020 2020 2065 7874 7261 2070           extra p
-0001e270: 726f 7065 7274 6965 7320 746f 2061 6e61  roperties to ana
-0001e280: 6c79 7a65 2c20 7365 6520 6060 736b 696d  lyze, see ``skim
-0001e290: 6167 652e 6d65 6173 7572 652e 7265 6769  age.measure.regi
-0001e2a0: 6f6e 7072 6f70 7360 602e 0d0a 0d0a 2020  onprops``.....  
-0001e2b0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0001e2c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0001e2d0: 2020 2020 2020 2020 4461 7461 4469 6374          DataDict
-0001e2e0: 206f 6620 5072 6f70 4172 7261 790d 0a20   of PropArray.. 
-0001e2f0: 2020 2020 2020 2020 2020 2044 6963 7469             Dicti
-0001e300: 6f6e 6172 7920 6861 7320 6b65 7973 206f  onary has keys o
-0001e310: 6620 7072 6f70 6572 7469 6573 2074 6861  f properties tha
-0001e320: 7420 6172 6520 7370 6563 6966 6965 6420  t are specified 
-0001e330: 6279 2060 7072 6f70 6572 7469 6573 602e  by `properties`.
-0001e340: 2045 6163 6820 7661 6c75 650d 0a20 2020   Each value..   
-0001e350: 2020 2020 2020 2020 2068 6173 2074 6865           has the
-0001e360: 2061 7272 6179 206f 6620 7072 6f70 6572   array of proper
-0001e370: 7469 6573 2e0d 0a20 2020 2020 2020 2020  ties...         
-0001e380: 2020 200d 0a20 2020 2020 2020 2045 7861     ..        Exa
-0001e390: 6d70 6c65 730d 0a20 2020 2020 2020 202d  mples..        -
-0001e3a0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0001e3b0: 204d 6561 7375 7265 2072 6567 696f 6e20   Measure region 
-0001e3c0: 7072 6f70 6572 7469 6573 2061 726f 756e  properties aroun
-0001e3d0: 6420 7369 6e67 6c65 206d 6f6c 6563 756c  d single molecul
-0001e3e0: 6573 2e0d 0a20 2020 2020 2020 200d 0a20  es...        .. 
-0001e3f0: 2020 2020 2020 2020 2020 203e 3e3e 2063             >>> c
-0001e400: 6f6f 7264 7320 3d20 696d 672e 6365 6e74  oords = img.cent
-0001e410: 726f 6964 5f73 6d28 290d 0a20 2020 2020  roid_sm()..     
-0001e420: 2020 2020 2020 203e 3e3e 2069 6d67 2e73         >>> img.s
-0001e430: 7065 6369 6679 2863 6f6f 7264 732c 2033  pecify(coords, 3
-0001e440: 2c20 6c61 6265 6c74 7970 653d 2263 6972  , labeltype="cir
-0001e450: 636c 6522 290d 0a20 2020 2020 2020 2020  cle")..         
-0001e460: 2020 203e 3e3e 2070 726f 7073 203d 2069     >>> props = i
-0001e470: 6d67 2e72 6567 696f 6e70 726f 7073 2829  mg.regionprops()
-0001e480: 0d0a 2020 2020 2020 2020 2222 2220 2020  ..        """   
-0001e490: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001e4a0: 645f 6178 6973 203d 2022 4e22 0d0a 2020  d_axis = "N"..  
-0001e4b0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0001e4c0: 6e63 6528 7072 6f70 6572 7469 6573 2c20  nce(properties, 
-0001e4d0: 7374 7229 3a0d 0a20 2020 2020 2020 2020  str):..         
-0001e4e0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-0001e4f0: 2870 726f 7065 7274 6965 732c 290d 0a20  (properties,).. 
-0001e500: 2020 2020 2020 2069 6620 6578 7472 615f         if extra_
-0001e510: 7072 6f70 6572 7469 6573 2069 7320 6e6f  properties is no
-0001e520: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0001e530: 2020 2020 2070 726f 7065 7274 6965 7320       properties 
-0001e540: 3d20 7072 6f70 6572 7469 6573 202b 2074  = properties + t
-0001e550: 7570 6c65 2865 782e 5f5f 6e61 6d65 5f5f  uple(ex.__name__
-0001e560: 2066 6f72 2065 7820 696e 2065 7874 7261   for ex in extra
-0001e570: 5f70 726f 7065 7274 6965 7329 0d0a 0d0a  _properties)....
-0001e580: 2020 2020 2020 2020 6966 2069 645f 6178          if id_ax
-0001e590: 6973 2069 6e20 7365 6c66 2e61 7865 733a  is in self.axes:
-0001e5a0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001e5b0: 7468 6973 2064 696d 656e 7369 6f6e 2077  this dimension w
-0001e5c0: 696c 6c20 6265 206c 6162 656c 0d0a 2020  ill be label..  
-0001e5d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001e5e0: 5661 6c75 6545 7272 6f72 2866 2261 7869  ValueError(f"axi
-0001e5f0: 7320 277b 6964 5f61 7869 737d 2720 6973  s '{id_axis}' is
-0001e600: 2075 7365 6420 666f 7220 6c61 6265 6c20   used for label 
-0001e610: 4944 2069 6e20 4461 7461 4672 616d 6573  ID in DataFrames
-0001e620: 2e22 290d 0a20 2020 2020 2020 200d 0a20  .")..        .. 
-0001e630: 2020 2020 2020 2070 726f 705f 6178 6573         prop_axes
-0001e640: 203d 2063 6f6d 706c 656d 656e 745f 6178   = complement_ax
-0001e650: 6573 2873 656c 662e 6c61 6265 6c73 2e61  es(self.labels.a
-0001e660: 7865 732c 2073 656c 662e 6178 6573 290d  xes, self.axes).
-0001e670: 0a20 2020 2020 2020 2073 6861 7065 203d  .        shape =
-0001e680: 2073 656c 662e 7369 7a65 736f 6628 7072   self.sizesof(pr
-0001e690: 6f70 5f61 7865 7329 0d0a 0d0a 2020 2020  op_axes)....    
-0001e6a0: 2020 2020 6f75 7420 3d20 4461 7461 4469      out = DataDi
-0001e6b0: 6374 287b 703a 2050 726f 7041 7272 6179  ct({p: PropArray
-0001e6c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001e6d0: 2020 206e 702e 656d 7074 7928 2873 656c     np.empty((sel
-0001e6e0: 662e 6c61 6265 6c73 2e6d 6178 2829 2c29  f.labels.max(),)
-0001e6f0: 202b 2073 6861 7065 2c20 6474 7970 653d   + shape, dtype=
-0001e700: 6e70 2e66 6c6f 6174 3332 292c 0d0a 2020  np.float32),..  
-0001e710: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0001e720: 6d65 3d73 656c 662e 6e61 6d65 2b22 2d70  me=self.name+"-p
-0001e730: 726f 7022 2c20 0d0a 2020 2020 2020 2020  rop", ..        
-0001e740: 2020 2020 2020 2020 6178 6573 3d5b 6964          axes=[id
-0001e750: 5f61 7869 735d 2b70 726f 705f 6178 6573  _axis]+prop_axes
-0001e760: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001e770: 2020 2073 6f75 7263 653d 7365 6c66 2e73     source=self.s
-0001e780: 6f75 7263 652c 0d0a 2020 2020 2020 2020  ource,..        
-0001e790: 2020 2020 2020 2020 7072 6f70 6e61 6d65          propname
-0001e7a0: 3d70 0d0a 2020 2020 2020 2020 2020 2020  =p..            
-0001e7b0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001e7c0: 2020 2020 2020 2066 6f72 2070 2069 6e20         for p in 
-0001e7d0: 7072 6f70 6572 7469 6573 0d0a 2020 2020  properties..    
-0001e7e0: 2020 2020 2020 2020 7d29 0d0a 2020 2020          })..    
-0001e7f0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-0001e800: 6361 6c63 756c 6174 6520 7072 6f70 6572  calculate proper
-0001e810: 7479 2076 616c 7565 2066 6f72 2065 6163  ty value for eac
-0001e820: 6820 736c 6963 650d 0a20 2020 2020 2020  h slice..       
-0001e830: 2066 6f72 2073 6c2c 2069 6d67 2069 6e20   for sl, img in 
-0001e840: 7365 6c66 2e69 7465 7228 7072 6f70 5f61  self.iter(prop_a
-0001e850: 7865 732c 2065 7863 6c75 6465 3d73 656c  xes, exclude=sel
-0001e860: 662e 6c61 6265 6c73 2e61 7865 7329 3a0d  f.labels.axes):.
-0001e870: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0001e880: 7073 203d 2073 6b6d 6573 2e72 6567 696f  ps = skmes.regio
-0001e890: 6e70 726f 7073 2873 656c 662e 6c61 6265  nprops(self.labe
-0001e8a0: 6c73 2e76 616c 7565 2c20 696d 672c 2063  ls.value, img, c
-0001e8b0: 6163 6865 3d46 616c 7365 2c0d 0a20 2020  ache=False,..   
-0001e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8e0: 2020 2065 7874 7261 5f70 726f 7065 7274     extra_propert
-0001e8f0: 6965 733d 6578 7472 615f 7072 6f70 6572  ies=extra_proper
-0001e900: 7469 6573 290d 0a20 2020 2020 2020 2020  ties)..         
-0001e910: 2020 206c 6162 656c 5f73 6c20 3d20 2873     label_sl = (s
-0001e920: 6c69 6365 284e 6f6e 6529 2c29 202b 2073  lice(None),) + s
-0001e930: 6c0d 0a20 2020 2020 2020 2020 2020 2066  l..            f
-0001e940: 6f72 2070 726f 705f 6e61 6d65 2069 6e20  or prop_name in 
-0001e950: 7072 6f70 6572 7469 6573 3a0d 0a20 2020  properties:..   
-0001e960: 2020 2020 2020 2020 2020 2020 2023 2042               # B
-0001e970: 6f74 6820 7369 6465 7320 6861 7665 206c  oth sides have l
-0001e980: 656e 6774 6820 6f66 2069 645f 6178 6973  ength of id_axis
-0001e990: 2028 6e75 6d62 6572 206f 6620 6c61 6265   (number of labe
-0001e9a0: 6c73 2920 736f 2074 6861 7420 7661 6c75  ls) so that valu
-0001e9b0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-0001e9c0: 2020 2020 2320 6361 6e20 6265 2063 6f72      # can be cor
-0001e9d0: 7265 6374 6c79 2073 7562 7374 6974 7574  rectly substitut
-0001e9e0: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
-0001e9f0: 2020 2020 206f 7574 5b70 726f 705f 6e61       out[prop_na
-0001ea00: 6d65 5d5b 6c61 6265 6c5f 736c 5d20 3d20  me][label_sl] = 
-0001ea10: 5b67 6574 6174 7472 2870 726f 702c 2070  [getattr(prop, p
-0001ea20: 726f 705f 6e61 6d65 2920 666f 7220 7072  rop_name) for pr
-0001ea30: 6f70 2069 6e20 7072 6f70 735d 0d0a 2020  op in props]..  
-0001ea40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001ea50: 666f 7220 7061 7272 2069 6e20 6f75 742e  for parr in out.
-0001ea60: 7661 6c75 6573 2829 3a0d 0a20 2020 2020  values():..     
-0001ea70: 2020 2020 2020 2070 6172 722e 7365 745f         parr.set_
-0001ea80: 7363 616c 6528 7365 6c66 290d 0a20 2020  scale(self)..   
-0001ea90: 2020 2020 2072 6574 7572 6e20 6f75 740d       return out.
-0001eaa0: 0a20 2020 200d 0a20 2020 2040 5f64 6f63  .    ..    @_doc
-0001eab0: 732e 7772 6974 655f 646f 6373 0d0a 2020  s.write_docs..  
-0001eac0: 2020 4064 696d 735f 746f 5f73 7061 7469    @dims_to_spati
-0001ead0: 616c 5f61 7865 730d 0a20 2020 2040 6368  al_axes..    @ch
-0001eae0: 6563 6b5f 696e 7075 745f 616e 645f 6f75  eck_input_and_ou
-0001eaf0: 7470 7574 0d0a 2020 2020 6465 6620 6c62  tput..    def lb
-0001eb00: 7028 0d0a 2020 2020 2020 2020 7365 6c66  p(..        self
-0001eb10: 2c0d 0a20 2020 2020 2020 2070 3a20 696e  ,..        p: in
-0001eb20: 7420 3d20 3132 2c0d 0a20 2020 2020 2020  t = 12,..       
-0001eb30: 2072 6164 6975 733a 2069 6e74 203d 2031   radius: int = 1
-0001eb40: 2c0d 0a20 2020 2020 2020 202a 2c0d 0a20  ,..        *,.. 
-0001eb50: 2020 2020 2020 206d 6574 686f 643a 204c         method: L
-0001eb60: 6974 6572 616c 5b22 6465 6661 756c 7422  iteral["default"
-0001eb70: 2c20 2272 6f72 222c 2022 756e 6966 6f72  , "ror", "unifor
-0001eb80: 6d22 2c20 2276 6172 225d 203d 2022 6465  m", "var"] = "de
-0001eb90: 6661 756c 7422 2c0d 0a20 2020 2020 2020  fault",..       
-0001eba0: 2064 696d 733a 2044 696d 7320 3d20 4e6f   dims: Dims = No
-0001ebb0: 6e65 2c0d 0a20 2020 2029 202d 3e20 496d  ne,..    ) -> Im
-0001ebc0: 6741 7272 6179 3a0d 0a20 2020 2020 2020  gArray:..       
-0001ebd0: 2022 2222 0d0a 2020 2020 2020 2020 4c6f   """..        Lo
-0001ebe0: 6361 6c20 6269 6e61 7279 2070 6174 7465  cal binary patte
-0001ebf0: 726e 2066 6561 7475 7265 2065 7874 7261  rn feature extra
-0001ec00: 6374 696f 6e2e 0d0a 0d0a 2020 2020 2020  ction.....      
-0001ec10: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-0001ec20: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0001ec30: 0d0a 2020 2020 2020 2020 7020 3a20 696e  ..        p : in
-0001ec40: 742c 2064 6566 6175 6c74 2069 7320 3132  t, default is 12
-0001ec50: 0d0a 2020 2020 2020 2020 2020 2020 4e75  ..            Nu
-0001ec60: 6d62 6572 206f 6620 6369 7263 756c 6172  mber of circular
-0001ec70: 206e 6569 6768 626f 7273 0d0a 2020 2020   neighbors..    
-0001ec80: 2020 2020 7261 6469 7573 203a 2069 6e74      radius : int
-0001ec90: 2c20 6465 6661 756c 7420 6973 2031 0d0a  , default is 1..
-0001eca0: 2020 2020 2020 2020 2020 2020 5261 6469              Radi
-0001ecb0: 7573 206f 6620 6e65 6967 6862 6f75 7273  us of neighbours
-0001ecc0: 2e0d 0a20 2020 2020 2020 206d 6574 686f  ...        metho
-0001ecd0: 6420 3a20 7374 722c 206f 7074 696f 6e61  d : str, optiona
-0001ece0: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
-0001ecf0: 6574 686f 6420 746f 2064 6574 6572 6d69  ethod to determi
-0001ed00: 6e65 6420 7468 6520 7061 7474 6572 6e2e  ned the pattern.
-0001ed10: 0d0a 2020 2020 2020 2020 7b64 696d 737d  ..        {dims}
-0001ed20: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0001ed30: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-0001ed40: 2d2d 2d2d 0d0a 2020 2020 2020 2020 496d  ----..        Im
-0001ed50: 6741 7272 6179 0d0a 2020 2020 2020 2020  gArray..        
-0001ed60: 2020 2020 4c6f 6361 6c20 6269 6e61 7279      Local binary
-0001ed70: 2070 6174 7465 726e 2069 6d61 6765 2e0d   pattern image..
-0001ed80: 0a20 2020 2020 2020 2022 2222 2020 2020  .        """    
-0001ed90: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-0001eda0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001edb0: 656c 662e 5f61 7070 6c79 5f64 6173 6b28  elf._apply_dask(
-0001edc0: 0d0a 2020 2020 2020 2020 2020 2020 736b  ..            sk
-0001edd0: 6665 6174 2e6c 6f63 616c 5f62 696e 6172  feat.local_binar
-0001ede0: 795f 7061 7474 6572 6e2c 0d0a 2020 2020  y_pattern,..    
-0001edf0: 2020 2020 2020 2020 635f 6178 6573 3d63          c_axes=c
-0001ee00: 6f6d 706c 656d 656e 745f 6178 6573 2864  omplement_axes(d
-0001ee10: 696d 7329 2c20 0d0a 2020 2020 2020 2020  ims), ..        
-0001ee20: 2020 2020 6172 6773 3d28 702c 2072 6164      args=(p, rad
-0001ee30: 6975 732c 206d 6574 686f 6429 0d0a 2020  ius, method)..  
-0001ee40: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001ee50: 200d 0a20 2020 2040 5f64 6f63 732e 7772   ..    @_docs.wr
-0001ee60: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
-0001ee70: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
-0001ee80: 7865 730d 0a20 2020 2040 6368 6563 6b5f  xes..    @check_
-0001ee90: 696e 7075 745f 616e 645f 6f75 7470 7574  input_and_output
-0001eea0: 0d0a 2020 2020 6465 6620 676c 636d 5f70  ..    def glcm_p
-0001eeb0: 726f 7073 2873 656c 662c 2064 6973 7461  rops(self, dista
-0001eec0: 6e63 6573 2c20 616e 676c 6573 2c20 7261  nces, angles, ra
-0001eed0: 6469 7573 3a69 6e74 2c20 7072 6f70 6572  dius:int, proper
-0001eee0: 7469 6573 3a74 7570 6c65 3d4e 6f6e 652c  ties:tuple=None,
-0001eef0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001ef00: 2020 2020 2020 2a2c 2062 696e 733a 696e        *, bins:in
-0001ef10: 743d 4e6f 6e65 2c20 7265 7363 616c 655f  t=None, rescale_
-0001ef20: 6d61 783a 626f 6f6c 3d46 616c 7365 2c20  max:bool=False, 
-0001ef30: 6469 6d73 3a20 4469 6d73 203d 204e 6f6e  dims: Dims = Non
-0001ef40: 6529 202d 3e20 496d 6741 7272 6179 3a0d  e) -> ImgArray:.
-0001ef50: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0001ef60: 2020 2020 2020 436f 6d70 7574 6520 7072        Compute pr
-0001ef70: 6f70 6572 7469 6573 206f 6620 2247 7261  operties of "Gra
-0001ef80: 7920 4c65 7665 6c20 436f 6f63 7572 7265  y Level Coocurre
-0001ef90: 6e63 6520 4d61 7472 6978 222e 2054 6869  nce Matrix". Thi
-0001efa0: 7320 7769 6c6c 2074 616b 6520 6c6f 6e67  s will take long
-0001efb0: 2074 696d 650d 0a20 2020 2020 2020 2062   time..        b
-0001efc0: 6563 6175 7365 206f 6620 7075 7265 2050  ecause of pure P
-0001efd0: 7974 686f 6e20 666f 722d 6c6f 6f70 2e0d  ython for-loop..
-0001efe0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001eff0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-0001f000: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-0001f010: 2020 2064 6973 7461 6e63 6573 203a 2061     distances : a
-0001f020: 7272 6179 5f6c 696b 650d 0a20 2020 2020  rray_like..     
-0001f030: 2020 2020 2020 204c 6973 7420 6f66 2070         List of p
-0001f040: 6978 656c 2070 6169 7220 6469 7374 616e  ixel pair distan
-0001f050: 6365 206f 6666 7365 7473 2e0d 0a20 2020  ce offsets...   
-0001f060: 2020 2020 2061 6e67 6c65 7320 3a20 6172       angles : ar
-0001f070: 7261 795f 6c69 6b65 0d0a 2020 2020 2020  ray_like..      
-0001f080: 2020 2020 2020 4c69 7374 206f 6620 7069        List of pi
-0001f090: 7865 6c20 7061 6972 2061 6e67 6c65 7320  xel pair angles 
-0001f0a0: 696e 2072 6164 6961 6e73 2e0d 0a20 2020  in radians...   
-0001f0b0: 2020 2020 2072 6164 6975 7320 3a20 696e       radius : in
-0001f0c0: 740d 0a20 2020 2020 2020 2020 2020 2057  t..            W
-0001f0d0: 696e 646f 7720 7261 6469 7573 2e0d 0a20  indow radius... 
-0001f0e0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-0001f0f0: 7320 3a20 7475 706c 6520 6f66 2073 7472  s : tuple of str
-0001f100: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0001f110: 6e74 7261 7374 2c20 6469 7373 696d 696c  ntrast, dissimil
-0001f120: 6172 6974 792c 2068 6f6d 6f67 656e 6569  arity, homogenei
-0001f130: 7479 2c20 656e 6572 6779 2c20 6d65 616e  ty, energy, mean
-0001f140: 2c20 7374 642c 2061 736d 2c20 6d61 782c  , std, asm, max,
-0001f150: 2065 6e74 726f 7079 0d0a 2020 2020 2020   entropy..      
-0001f160: 2020 6269 6e73 203a 2069 6e74 2c20 6f70    bins : int, op
-0001f170: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-0001f180: 2020 2020 4e75 6d62 6572 206f 6620 6269      Number of bi
-0001f190: 6e73 2e0d 0a20 2020 2020 2020 2072 6573  ns...        res
-0001f1a0: 6361 6c65 5f6d 6178 203a 2062 6f6f 6c2c  cale_max : bool,
-0001f1b0: 2064 6566 6175 6c74 2069 7320 4661 6c73   default is Fals
-0001f1c0: 650d 0a20 2020 2020 2020 2020 2020 2049  e..            I
-0001f1d0: 6620 5472 7565 2c20 7468 6520 636f 6e74  f True, the cont
-0001f1e0: 7261 7374 206f 6620 7468 6520 696e 7075  rast of the inpu
-0001f1f0: 7420 696d 6167 6520 6973 206d 6178 696d  t image is maxim
-0001f200: 697a 6564 2062 7920 6d75 6c74 6970 6c79  ized by multiply
-0001f210: 696e 6720 616e 2069 6e74 6567 6572 2e0d  ing an integer..
-0001f220: 0a20 2020 2020 2020 207b 6469 6d73 7d0d  .        {dims}.
-0001f230: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0001f240: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-0001f250: 2d2d 2d0d 0a20 2020 2020 2020 2044 6174  ---..        Dat
-0001f260: 6144 6963 7420 6f66 2049 6d67 4172 7261  aDict of ImgArra
-0001f270: 790d 0a20 2020 2020 2020 2020 2020 2047  y..            G
-0001f280: 4c43 4d20 7769 7468 2061 6464 6974 696f  LCM with additio
-0001f290: 6e61 6c20 6178 6573 2022 6461 222c 2077  nal axes "da", w
-0001f2a0: 6865 7265 2022 6422 206d 6561 6e73 2064  here "d" means d
-0001f2b0: 6973 7461 6e63 6520 616e 6420 2261 2220  istance and "a" 
-0001f2c0: 6d65 616e 7320 616e 676c 652e 0d0a 2020  means angle...  
-0001f2d0: 2020 2020 2020 2020 2020 4966 2069 6e70            If inp
-0001f2e0: 7574 2069 6d61 6765 2068 6173 2022 747a  ut image has "tz
-0001f2f0: 7978 2220 6178 6573 2074 6865 6e20 6f75  yx" axes then ou
-0001f300: 7470 7574 2077 696c 6c20 6861 7665 2022  tput will have "
-0001f310: 747a 643c 7978 2220 6178 6573 2e0d 0a20  tzd<yx" axes... 
-0001f320: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001f330: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
-0001f340: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-0001f350: 2020 2020 2050 6c6f 7420 474c 434d 2773       Plot GLCM's
-0001f360: 2049 444d 2061 6e64 2041 534d 2069 6d61   IDM and ASM ima
-0001f370: 6765 730d 0a20 2020 2020 2020 2020 2020  ges..           
-0001f380: 203e 3e3e 206f 7574 203d 2069 6d67 2e67   >>> out = img.g
-0001f390: 6c63 6d5f 7072 6f70 7328 5b31 5d2c 205b  lcm_props([1], [
-0001f3a0: 305d 2c20 332c 2070 726f 7065 7274 6965  0], 3, propertie
-0001f3b0: 733d 2822 6964 6d22 2c22 6173 6d22 2929  s=("idm","asm"))
-0001f3c0: 0d0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-0001f3d0: 3e20 6f75 742e 6964 6d5b 2264 3d30 3b3c  > out.idm["d=0;<
-0001f3e0: 3d30 225d 2e69 6d73 686f 7728 290d 0a20  =0"].imshow().. 
-0001f3f0: 2020 2020 2020 2020 2020 203e 3e3e 206f             >>> o
-0001f400: 7574 2e61 736d 5b22 643d 303b 3c3d 3022  ut.asm["d=0;<=0"
-0001f410: 5d2e 696d 7368 6f77 2829 0d0a 2020 2020  ].imshow()..    
-0001f420: 2020 2020 2222 2220 2020 2020 2020 200d      """        .
-0001f430: 0a20 2020 2020 2020 2073 656c 662c 2062  .        self, b
-0001f440: 696e 732c 2072 6573 6361 6c65 5f6d 6178  ins, rescale_max
-0001f450: 203d 205f 676c 636d 2e63 6865 636b 5f67   = _glcm.check_g
-0001f460: 6c63 6d28 7365 6c66 2c20 6269 6e73 2c20  lcm(self, bins, 
-0001f470: 7265 7363 616c 655f 6d61 7829 0d0a 2020  rescale_max)..  
-0001f480: 2020 2020 2020 6966 2070 726f 7065 7274        if propert
-0001f490: 6965 7320 6973 204e 6f6e 653a 0d0a 2020  ies is None:..  
-0001f4a0: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
-0001f4b0: 7469 6573 203d 2028 2263 6f6e 7472 6173  ties = ("contras
-0001f4c0: 7422 2c20 2264 6973 7369 6d69 6c61 7269  t", "dissimilari
-0001f4d0: 7479 222c 2022 6964 6d22 2c20 0d0a 2020  ty", "idm", ..  
-0001f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f4f0: 2020 2020 2020 2020 2261 736d 222c 2022          "asm", "
-0001f500: 6d61 7822 2c20 2265 6e74 726f 7079 222c  max", "entropy",
-0001f510: 2022 636f 7272 656c 6174 696f 6e22 290d   "correlation").
-0001f520: 0a20 2020 2020 2020 2063 5f61 7865 7320  .        c_axes 
-0001f530: 3d20 636f 6d70 6c65 6d65 6e74 5f61 7865  = complement_axe
-0001f540: 7328 6469 6d73 2c20 7365 6c66 2e61 7865  s(dims, self.axe
-0001f550: 7329 0d0a 2020 2020 2020 2020 6469 7374  s)..        dist
-0001f560: 616e 6365 7320 3d20 6e70 2e61 7361 7272  ances = np.asarr
-0001f570: 6179 2864 6973 7461 6e63 6573 2c20 6474  ay(distances, dt
-0001f580: 7970 653d 6e70 2e75 696e 7438 290d 0a20  ype=np.uint8).. 
-0001f590: 2020 2020 2020 2061 6e67 6c65 7320 3d20         angles = 
-0001f5a0: 6e70 2e61 7361 7272 6179 2861 6e67 6c65  np.asarray(angle
-0001f5b0: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-0001f5c0: 7433 3229 0d0a 2020 2020 2020 2020 6f75  t32)..        ou
-0001f5d0: 7473 6861 7065 203d 2073 656c 662e 7369  tshape = self.si
-0001f5e0: 7a65 736f 6628 635f 6178 6573 2920 2b20  zesof(c_axes) + 
-0001f5f0: 286c 656e 2864 6973 7461 6e63 6573 292c  (len(distances),
-0001f600: 206c 656e 2861 6e67 6c65 7329 2920 2b20   len(angles)) + 
-0001f610: 7365 6c66 2e73 697a 6573 6f66 2864 696d  self.sizesof(dim
-0001f620: 7329 0d0a 2020 2020 2020 2020 6f75 7420  s)..        out 
-0001f630: 3d20 7b7d 0d0a 2020 2020 2020 2020 666f  = {}..        fo
-0001f640: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
-0001f650: 7469 6573 3a0d 0a20 2020 2020 2020 2020  ties:..         
-0001f660: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0001f670: 2870 726f 702c 2073 7472 293a 0d0a 2020  (prop, str):..  
-0001f680: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-0001f690: 745b 7072 6f70 5d20 3d20 6e70 2e65 6d70  t[prop] = np.emp
-0001f6a0: 7479 286f 7574 7368 6170 652c 2064 7479  ty(outshape, dty
-0001f6b0: 7065 3d6e 702e 666c 6f61 7433 3229 2e76  pe=np.float32).v
-0001f6c0: 6965 7728 7365 6c66 2e5f 5f63 6c61 7373  iew(self.__class
-0001f6d0: 5f5f 290d 0a20 2020 2020 2020 2020 2020  __)..           
-0001f6e0: 2065 6c69 6620 6361 6c6c 6162 6c65 2870   elif callable(p
-0001f6f0: 726f 7029 3a0d 0a20 2020 2020 2020 2020  rop):..         
-0001f700: 2020 2020 2020 206f 7574 5b70 726f 702e         out[prop.
-0001f710: 5f5f 6e61 6d65 5f5f 5d20 3d20 6e70 2e65  __name__] = np.e
-0001f720: 6d70 7479 286f 7574 7368 6170 652c 2064  mpty(outshape, d
-0001f730: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-0001f740: 2e76 6965 7728 7365 6c66 2e5f 5f63 6c61  .view(self.__cla
-0001f750: 7373 5f5f 290d 0a20 2020 2020 2020 2020  ss__)..         
-0001f760: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0001f770: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001f780: 5479 7065 4572 726f 7228 2270 726f 7065  TypeError("prope
-0001f790: 7274 6965 7320 6d75 7374 2062 6520 7374  rties must be st
-0001f7a0: 7220 6f72 2063 616c 6c61 626c 652e 2229  r or callable.")
-0001f7b0: 0d0a 2020 2020 2020 2020 6f75 7420 3d20  ..        out = 
-0001f7c0: 4461 7461 4469 6374 286f 7574 290d 0a20  DataDict(out).. 
-0001f7d0: 2020 2020 2020 2073 656c 6620 3d20 7365         self = se
-0001f7e0: 6c66 2e70 6164 2872 6164 6975 732c 206d  lf.pad(radius, m
-0001f7f0: 6f64 653d 2272 6566 6c65 6374 222c 2064  ode="reflect", d
-0001f800: 696d 733d 6469 6d73 290d 0a20 2020 2020  ims=dims)..     
-0001f810: 2020 2066 6f72 2073 6c2c 2069 6d67 2069     for sl, img i
-0001f820: 6e20 7365 6c66 2e69 7465 7228 635f 6178  n self.iter(c_ax
-0001f830: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-0001f840: 2020 7072 6f70 6f75 7420 3d20 5f67 6c63    propout = _glc
-0001f850: 6d2e 676c 636d 5f70 726f 7073 5f28 696d  m.glcm_props_(im
-0001f860: 672c 2064 6973 7461 6e63 6573 2c20 616e  g, distances, an
-0001f870: 676c 6573 2c20 6269 6e73 2c20 7261 6469  gles, bins, radi
-0001f880: 7573 2c20 7072 6f70 6572 7469 6573 290d  us, properties).
-0001f890: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0001f8a0: 2070 726f 7020 696e 2070 726f 7065 7274   prop in propert
-0001f8b0: 6965 733a 0d0a 2020 2020 2020 2020 2020  ies:..          
-0001f8c0: 2020 2020 2020 6f75 745b 7072 6f70 5d2e        out[prop].
-0001f8d0: 7661 6c75 655b 736c 5d20 3d20 7072 6f70  value[sl] = prop
-0001f8e0: 6f75 745b 7072 6f70 5d0d 0a20 2020 2020  out[prop]..     
-0001f8f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001f900: 2066 6f72 206b 2c20 7620 696e 206f 7574   for k, v in out
-0001f910: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-0001f920: 2020 2020 2020 2076 2e5f 7365 745f 696e         v._set_in
-0001f930: 666f 2873 656c 662c 206e 6577 5f61 7865  fo(self, new_axe
-0001f940: 733d 635f 6178 6573 2b22 6461 222b 6469  s=c_axes+"da"+di
-0001f950: 6d73 290d 0a20 2020 2020 2020 2072 6574  ms)..        ret
-0001f960: 7572 6e20 6f75 740d 0a20 2020 200d 0a20  urn out..    .. 
-0001f970: 2020 200d 0a20 2020 2040 7361 6d65 5f64     ..    @same_d
-0001f980: 7479 7065 0d0a 2020 2020 6465 6620 7072  type..    def pr
-0001f990: 6f6a 280d 0a20 2020 2020 2020 2073 656c  oj(..        sel
-0001f9a0: 662c 0d0a 2020 2020 2020 2020 6178 6973  f,..        axis
-0001f9b0: 3a20 4178 6973 4c69 6b65 207c 204e 6f6e  : AxisLike | Non
-0001f9c0: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
-0001f9d0: 2020 206d 6574 686f 643a 2073 7472 207c     method: str |
-0001f9e0: 2043 616c 6c61 626c 6520 3d20 226d 6561   Callable = "mea
-0001f9f0: 6e22 2c0d 0a20 2020 2020 2020 206d 6173  n",..        mas
-0001fa00: 6b20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  k = None,..     
-0001fa10: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-0001fa20: 2029 202d 3e20 496d 6741 7272 6179 3a0d   ) -> ImgArray:.
-0001fa30: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0001fa40: 2020 2020 2020 5072 6f6a 6563 7469 6f6e        Projection
-0001fa50: 2061 6c6f 6e67 2061 6e79 2061 7869 732e   along any axis.
-0001fa60: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-0001fa70: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-0001fa80: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-0001fa90: 2020 2020 6178 6973 203a 2073 7472 2c20      axis : str, 
-0001faa0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-0001fab0: 2020 2020 2020 416c 6f6e 6720 7768 6963        Along whic
-0001fac0: 6820 6178 6973 2070 726f 6a65 6374 696f  h axis projectio
-0001fad0: 6e20 7769 6c6c 2062 6520 6361 6c63 756c  n will be calcul
-0001fae0: 6174 6564 2e20 4966 204e 6f6e 652c 206d  ated. If None, m
-0001faf0: 6f73 7420 706c 6175 7369 626c 6520 6f6e  ost plausible on
-0001fb00: 6520 7769 6c6c 2062 6520 6368 6f73 656e  e will be chosen
-0001fb10: 2e0d 0a20 2020 2020 2020 206d 6574 686f  ...        metho
-0001fb20: 6420 3a20 7374 7220 6f72 2063 616c 6c61  d : str or calla
-0001fb30: 626c 652c 2064 6566 6175 6c74 2069 7320  ble, default is 
-0001fb40: 6d65 616e 2d70 726f 6a65 6374 696f 6e2e  mean-projection.
-0001fb50: 0d0a 2020 2020 2020 2020 2020 2020 5072  ..            Pr
-0001fb60: 6f6a 6563 7469 6f6e 206d 6574 686f 642e  ojection method.
-0001fb70: 2049 6620 7374 7220 6973 2067 6976 656e   If str is given
-0001fb80: 2c20 6974 2077 696c 6c20 636f 6e76 6572  , it will conver
-0001fb90: 7465 6420 746f 206e 756d 7079 2066 756e  ted to numpy fun
-0001fba0: 6374 696f 6e2e 0d0a 2020 2020 2020 2020  ction...        
-0001fbb0: 6d61 736b 203a 2061 7272 6179 2d6c 696b  mask : array-lik
-0001fbc0: 652c 206f 7074 696f 6e61 6c0d 0a20 2020  e, optional..   
-0001fbd0: 2020 2020 2020 2020 2049 6620 7072 6f76           If prov
-0001fbe0: 6964 6564 2c20 696e 7075 7420 696d 6167  ided, input imag
-0001fbf0: 6520 7769 6c6c 2062 6520 636f 6e76 6572  e will be conver
-0001fc00: 7465 6420 746f 206e 702e 6d61 2e61 7272  ted to np.ma.arr
-0001fc10: 6179 2061 6e64 2060 606d 6574 686f 6460  ay and ``method`
-0001fc20: 6020 7769 6c6c 2061 6c73 6f20 6265 2069  ` will also be i
-0001fc30: 6e74 6572 7072 6574 6564 0d0a 2020 2020  nterpreted..    
-0001fc40: 2020 2020 2020 2020 6173 2061 6e20 6d61          as an ma
-0001fc50: 736b 6564 2066 756e 6374 696f 2069 6620  sked functio if 
-0001fc60: 706f 7373 6962 6c65 2e0d 0a20 2020 2020  possible...     
-0001fc70: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-0001fc80: 2020 2020 2020 2020 204f 7468 6572 206b           Other k
-0001fc90: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0001fca0: 2074 6861 7420 7769 6c6c 2070 6173 7365   that will passe
-0001fcb0: 6420 746f 2070 726f 6a65 6374 696f 6e20  d to projection 
-0001fcc0: 6675 6e63 7469 6f6e 2e0d 0a0d 0a20 2020  function.....   
-0001fcd0: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-0001fce0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-0001fcf0: 2020 2020 2020 2049 6d67 4172 7261 790d         ImgArray.
-0001fd00: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0001fd10: 6a65 6374 6564 2069 6d61 6765 2e0d 0a20  jected image... 
-0001fd20: 2020 2020 2020 2022 2222 2020 2020 2020         """      
-0001fd30: 2020 0d0a 2020 2020 2020 2020 2320 6465    ..        # de
-0001fd40: 7465 726d 696e 6520 6675 6e63 7469 6f6e  termine function
-0001fd50: 0d0a 2020 2020 2020 2020 6966 206d 6173  ..        if mas
-0001fd60: 6b20 6973 206e 6f74 204e 6f6e 653a 0d0a  k is not None:..
-0001fd70: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0001fd80: 7369 6e73 7461 6e63 6528 6d65 7468 6f64  sinstance(method
-0001fd90: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
-0001fda0: 2020 2020 2020 2020 2066 756e 6320 3d20           func = 
-0001fdb0: 6765 7461 7474 7228 6e70 2e6d 612c 206d  getattr(np.ma, m
-0001fdc0: 6574 686f 6429 0d0a 2020 2020 2020 2020  ethod)..        
-0001fdd0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001fde0: 2020 2020 2020 2020 2020 2066 756e 6320             func 
-0001fdf0: 3d20 6d65 7468 6f64 0d0a 2020 2020 2020  = method..      
-0001fe00: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001fe10: 2020 2020 2066 756e 6320 3d20 5f63 6865       func = _che
-0001fe20: 636b 5f66 756e 6374 696f 6e28 6d65 7468  ck_function(meth
-0001fe30: 6f64 290d 0a20 2020 2020 2020 200d 0a20  od)..        .. 
-0001fe40: 2020 2020 2020 2069 6620 6178 6973 2069         if axis i
-0001fe50: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-0001fe60: 2020 2020 2061 7869 7320 3d20 6669 6e64       axis = find
-0001fe70: 5f66 6972 7374 5f61 7070 6561 7265 6428  _first_appeared(
-0001fe80: 227a 7470 6961 6322 2c20 696e 636c 7564  "ztpiac", includ
-0001fe90: 653d 7365 6c66 2e61 7865 732c 2065 7863  e=self.axes, exc
-0001fea0: 6c75 6465 3d22 7978 2229 0d0a 2020 2020  lude="yx")..    
-0001feb0: 2020 2020 656c 6966 206e 6f74 2068 6173      elif not has
-0001fec0: 6174 7472 2861 7869 732c 2022 5f5f 6974  attr(axis, "__it
-0001fed0: 6572 5f5f 2229 3a0d 0a20 2020 2020 2020  er__"):..       
-0001fee0: 2020 2020 2061 7869 7320 3d20 5b61 7869       axis = [axi
-0001fef0: 735d 0d0a 2020 2020 2020 2020 6178 6973  s]..        axis
-0001ff00: 696e 7420 3d20 7475 706c 6528 7365 6c66  int = tuple(self
-0001ff10: 2e61 7869 736f 6628 6129 2066 6f72 2061  .axisof(a) for a
-0001ff20: 2069 6e20 6178 6973 290d 0a20 2020 2020   in axis)..     
-0001ff30: 2020 2069 6620 6675 6e63 2e5f 5f6d 6f64     if func.__mod
-0001ff40: 756c 655f 5f20 3d3d 2022 6e75 6d70 792e  ule__ == "numpy.
-0001ff50: 6d61 2e63 6f72 6522 3a0d 0a20 2020 2020  ma.core":..     
-0001ff60: 2020 2020 2020 2061 7272 203d 206e 702e         arr = np.
-0001ff70: 6d61 2e61 7272 6179 2873 656c 662e 7661  ma.array(self.va
-0001ff80: 6c75 652c 206d 6173 6b3d 6d61 736b 2c20  lue, mask=mask, 
-0001ff90: 6474 7970 653d 7365 6c66 2e64 7479 7065  dtype=self.dtype
-0001ffa0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0001ffb0: 6620 6675 6e63 2069 7320 6e70 2e6d 612e  f func is np.ma.
-0001ffc0: 6d65 616e 3a0d 0a20 2020 2020 2020 2020  mean:..         
-0001ffd0: 2020 2020 2020 206f 7574 203d 2066 756e         out = fun
-0001ffe0: 6328 6172 722c 2061 7869 733d 6178 6973  c(arr, axis=axis
-0001fff0: 696e 742c 2064 7479 7065 3d6e 702e 666c  int, dtype=np.fl
-00020000: 6f61 7433 322c 202a 2a6b 7761 7267 7329  oat32, **kwargs)
-00020010: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00020020: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00020030: 2020 2020 206f 7574 203d 2066 756e 6328       out = func(
-00020040: 6172 722c 2061 7869 733d 6178 6973 696e  arr, axis=axisin
-00020050: 742c 202a 2a6b 7761 7267 7329 0d0a 2020  t, **kwargs)..  
-00020060: 2020 2020 2020 656c 6966 2066 756e 6320        elif func 
-00020070: 6973 206e 702e 6d65 616e 3a0d 0a20 2020  is np.mean:..   
-00020080: 2020 2020 2020 2020 206f 7574 203d 2066           out = f
-00020090: 756e 6328 7365 6c66 2e76 616c 7565 2c20  unc(self.value, 
-000200a0: 6178 6973 3d61 7869 7369 6e74 2c20 6474  axis=axisint, dt
-000200b0: 7970 653d 6e70 2e66 6c6f 6174 3332 2c20  ype=np.float32, 
-000200c0: 2a2a 6b77 6172 6773 290d 0a20 2020 2020  **kwargs)..     
-000200d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000200e0: 2020 2020 2020 6f75 7420 3d20 6675 6e63        out = func
-000200f0: 2873 656c 662e 7661 6c75 652c 2061 7869  (self.value, axi
-00020100: 733d 6178 6973 696e 742c 202a 2a6b 7761  s=axisint, **kwa
-00020110: 7267 7329 0d0a 2020 2020 2020 2020 0d0a  rgs)..        ..
-00020120: 2020 2020 2020 2020 6f75 7420 3d20 6f75          out = ou
-00020130: 742e 7669 6577 2873 656c 662e 5f5f 636c  t.view(self.__cl
-00020140: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
-00020150: 6f75 742e 5f73 6574 5f69 6e66 6f28 7365  out._set_info(se
-00020160: 6c66 2c20 7365 6c66 2e61 7865 732e 6472  lf, self.axes.dr
-00020170: 6f70 2861 7869 7369 6e74 2929 0d0a 2020  op(axisint))..  
-00020180: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-00020190: 0d0a 0d0a 2020 2020 4063 6865 636b 5f69  ....    @check_i
-000201a0: 6e70 7574 5f61 6e64 5f6f 7574 7075 740d  nput_and_output.
-000201b0: 0a20 2020 2064 6566 2063 6c69 7028 7365  .    def clip(se
-000201c0: 6c66 2c20 696e 5f72 616e 6765 3a20 7475  lf, in_range: tu
-000201d0: 706c 655b 696e 7420 7c20 7374 722c 2069  ple[int | str, i
-000201e0: 6e74 207c 2073 7472 5d20 3d20 2822 3025  nt | str] = ("0%
-000201f0: 222c 2022 3130 3025 2229 2920 2d3e 2049  ", "100%")) -> I
-00020200: 6d67 4172 7261 793a 0d0a 2020 2020 2020  mgArray:..      
-00020210: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
-00020220: 6174 7572 6174 6520 6c6f 772f 6869 6768  aturate low/high
-00020230: 2069 6e74 656e 7369 7479 2075 7369 6e67   intensity using
-00020240: 206e 702e 636c 6970 2829 2e0d 0a0d 0a20   np.clip()..... 
-00020250: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00020260: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00020270: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2069  -----..        i
-00020280: 6e5f 7261 6e67 6520 3a20 7477 6f20 7363  n_range : two sc
-00020290: 616c 6172 2076 616c 7565 732c 206f 7074  alar values, opt
-000202a0: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-000202b0: 2020 2072 616e 6765 206f 6620 6c6f 7765     range of lowe
-000202c0: 722f 7570 7065 7220 6c69 6d69 7473 2c20  r/upper limits, 
-000202d0: 6279 2064 6566 6175 6c74 2028 3025 2c20  by default (0%, 
-000202e0: 3130 3025 292e 0d0a 0d0a 2020 2020 2020  100%).....      
-000202f0: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-00020300: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-00020310: 2020 2020 496d 6741 7272 6179 0d0a 2020      ImgArray..  
-00020320: 2020 2020 2020 2020 2020 436c 6970 7065            Clippe
-00020330: 6420 696d 6167 6520 7769 7468 2074 656d  d image with tem
-00020340: 706f 7261 6c20 6174 7472 6962 7574 650d  poral attribute.
-00020350: 0a20 2020 2020 2020 2022 2222 2020 2020  .        """    
-00020360: 2020 2020 0d0a 2020 2020 2020 2020 6c6f      ..        lo
-00020370: 7765 726c 696d 2c20 7570 7065 726c 696d  werlim, upperlim
-00020380: 203d 205f 6368 6563 6b5f 636c 6970 5f72   = _check_clip_r
-00020390: 616e 6765 2869 6e5f 7261 6e67 652c 2073  ange(in_range, s
-000203a0: 656c 662e 7661 6c75 6529 0d0a 2020 2020  elf.value)..    
-000203b0: 2020 2020 6f75 7420 3d20 6e70 2e63 6c69      out = np.cli
-000203c0: 7028 7365 6c66 2e76 616c 7565 2c20 6c6f  p(self.value, lo
-000203d0: 7765 726c 696d 2c20 7570 7065 726c 696d  werlim, upperlim
-000203e0: 290d 0a20 2020 2020 2020 206f 7574 203d  )..        out =
-000203f0: 206f 7574 2e76 6965 7728 7365 6c66 2e5f   out.view(self._
-00020400: 5f63 6c61 7373 5f5f 290d 0a20 2020 2020  _class__)..     
-00020410: 2020 2072 6574 7572 6e20 6f75 740d 0a20     return out.. 
-00020420: 2020 200d 0a20 2020 2040 6368 6563 6b5f     ..    @check_
-00020430: 696e 7075 745f 616e 645f 6f75 7470 7574  input_and_output
-00020440: 0d0a 2020 2020 6465 6620 7265 7363 616c  ..    def rescal
-00020450: 655f 696e 7465 6e73 6974 7928 0d0a 2020  e_intensity(..  
-00020460: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-00020470: 2020 2020 2069 6e5f 7261 6e67 653a 2074       in_range: t
-00020480: 7570 6c65 5b69 6e74 207c 2073 7472 2c20  uple[int | str, 
-00020490: 696e 7420 7c20 7374 725d 203d 2028 2230  int | str] = ("0
-000204a0: 2522 2c20 2231 3030 2522 292c 200d 0a20  %", "100%"), .. 
-000204b0: 2020 2020 2020 2064 7479 7065 203d 206e         dtype = n
-000204c0: 702e 7569 6e74 3136 0d0a 2020 2020 2920  p.uint16..    ) 
-000204d0: 2d3e 2049 6d67 4172 7261 793a 0d0a 2020  -> ImgArray:..  
-000204e0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000204f0: 2020 2052 6573 6361 6c65 2074 6865 2069     Rescale the i
-00020500: 6e74 656e 7369 7479 206f 6620 7468 6520  ntensity of the 
-00020510: 696d 6167 6520 7573 696e 6720 736b 696d  image using skim
-00020520: 6167 652e 6578 706f 7375 7265 2e72 6573  age.exposure.res
-00020530: 6361 6c65 5f69 6e74 656e 7369 7479 2829  cale_intensity()
-00020540: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00020550: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-00020560: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-00020570: 2020 2020 2069 6e5f 7261 6e67 6520 3a20       in_range : 
-00020580: 7477 6f20 7363 616c 6172 2076 616c 7565  two scalar value
-00020590: 732c 2064 6566 6175 6c74 2069 7320 2830  s, default is (0
-000205a0: 252c 2031 3030 2529 0d0a 2020 2020 2020  %, 100%)..      
-000205b0: 2020 2020 2020 5261 6e67 6520 6f66 206c        Range of l
-000205c0: 6f77 6572 2f75 7070 6572 206c 696d 6974  ower/upper limit
-000205d0: 2e0d 0a20 2020 2020 2020 2064 7479 7065  ...        dtype
-000205e0: 203a 206e 756d 7079 2064 7479 7065 2c20   : numpy dtype, 
-000205f0: 6465 6661 756c 7420 6973 206e 702e 7569  default is np.ui
-00020600: 6e74 3136 0d0a 2020 2020 2020 2020 2020  nt16..          
-00020610: 2020 4f75 7470 7574 2064 7479 7065 2e0d    Output dtype..
-00020620: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00020630: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00020640: 2d2d 2d0d 0a20 2020 2020 2020 2049 6d67  ---..        Img
-00020650: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
-00020660: 2020 2052 6573 6361 6c65 6420 696d 6167     Rescaled imag
-00020670: 6520 7769 7468 2074 656d 706f 7261 6c20  e with temporal 
-00020680: 6174 7472 6962 7574 650d 0a20 2020 2020  attribute..     
-00020690: 2020 2022 2222 2020 2020 2020 2020 0d0a     """        ..
-000206a0: 2020 2020 2020 2020 6f75 7420 3d20 7365          out = se
-000206b0: 6c66 2e76 6965 7728 6e70 2e6e 6461 7272  lf.view(np.ndarr
-000206c0: 6179 292e 6173 7479 7065 286e 702e 666c  ay).astype(np.fl
-000206d0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-000206e0: 6c6f 7765 726c 696d 2c20 7570 7065 726c  lowerlim, upperl
-000206f0: 696d 203d 205f 6368 6563 6b5f 636c 6970  im = _check_clip
-00020700: 5f72 616e 6765 2869 6e5f 7261 6e67 652c  _range(in_range,
-00020710: 2073 656c 662e 7661 6c75 6529 0d0a 2020   self.value)..  
-00020720: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00020730: 2020 2020 6f75 7420 3d20 736b 6578 702e      out = skexp.
-00020740: 7265 7363 616c 655f 696e 7465 6e73 6974  rescale_intensit
-00020750: 7928 6f75 742c 2069 6e5f 7261 6e67 653d  y(out, in_range=
-00020760: 286c 6f77 6572 6c69 6d2c 2075 7070 6572  (lowerlim, upper
-00020770: 6c69 6d29 2c20 6f75 745f 7261 6e67 653d  lim), out_range=
-00020780: 2264 7479 7065 2229 0d0a 2020 2020 2020  "dtype")..      
-00020790: 2020 0d0a 2020 2020 2020 2020 6f75 7420    ..        out 
-000207a0: 3d20 6f75 742e 7669 6577 2873 656c 662e  = out.view(self.
-000207b0: 5f5f 636c 6173 735f 5f29 0d0a 2020 2020  __class__)..    
-000207c0: 2020 2020 7265 7475 726e 206f 7574 0d0a      return out..
-000207d0: 2020 2020 0d0a 2020 2020 4063 6865 636b      ..    @check
-000207e0: 5f69 6e70 7574 5f61 6e64 5f6f 7574 7075  _input_and_outpu
-000207f0: 740d 0a20 2020 2064 6566 2074 7261 636b  t..    def track
-00020800: 5f64 7269 6674 280d 0a20 2020 2020 2020  _drift(..       
-00020810: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00020820: 616c 6f6e 673a 2041 7869 734c 696b 6520  along: AxisLike 
-00020830: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0d0a  | None = None,..
-00020840: 2020 2020 2020 2020 7368 6f77 5f64 7269          show_dri
-00020850: 6674 3a20 626f 6f6c 203d 2046 616c 7365  ft: bool = False
-00020860: 2c20 0d0a 2020 2020 2020 2020 7570 7361  , ..        upsa
-00020870: 6d70 6c65 5f66 6163 746f 723a 2069 6e74  mple_factor: int
-00020880: 203d 2031 302c 0d0a 2020 2020 2920 2d3e   = 10,..    ) ->
-00020890: 204d 6172 6b65 7246 7261 6d65 3a0d 0a20   MarkerFrame:.. 
-000208a0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000208b0: 2020 2020 4361 6c63 756c 6174 6520 7978      Calculate yx
-000208c0: 2d64 6972 6563 7469 6f6e 616c 2064 7269  -directional dri
-000208d0: 6674 2075 7369 6e67 2074 6865 206d 6574  ft using the met
-000208e0: 686f 6420 6571 7569 7661 6c65 6e74 2074  hod equivalent t
-000208f0: 6f0d 0a20 2020 2020 2020 2060 6073 6b69  o..        ``ski
-00020900: 6d61 6765 2e72 6567 6973 7472 6174 696f  mage.registratio
-00020910: 6e2e 7068 6173 655f 6372 6f73 735f 636f  n.phase_cross_co
-00020920: 7272 656c 6174 696f 6e60 602e 0d0a 0d0a  rrelation``.....
-00020930: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00020940: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
-00020950: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00020960: 616c 6f6e 6720 3a20 4178 6973 4c69 6b65  along : AxisLike
-00020970: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00020980: 2020 2020 2020 2020 416c 6f6e 6720 7768          Along wh
-00020990: 6963 6820 6178 6973 2064 7269 6674 2077  ich axis drift w
-000209a0: 696c 6c20 6265 2063 616c 6375 6c61 7465  ill be calculate
-000209b0: 642e 0d0a 2020 2020 2020 2020 7368 6f77  d...        show
-000209c0: 5f64 7269 6674 203a 2062 6f6f 6c2c 2064  _drift : bool, d
-000209d0: 6566 6175 6c74 2069 7320 4661 6c73 650d  efault is False.
-000209e0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000209f0: 5472 7565 2c20 706c 6f74 2074 6865 2072  True, plot the r
-00020a00: 6573 756c 742e 0d0a 2020 2020 2020 2020  esult...        
-00020a10: 7570 7361 6d70 6c65 5f66 6163 746f 7220  upsample_factor 
-00020a20: 3a20 696e 742c 2064 6566 6175 6c74 2069  : int, default i
-00020a30: 7320 3130 0d0a 2020 2020 2020 2020 2020  s 10..          
-00020a40: 2020 5570 2d73 616d 706c 696e 6720 6661    Up-sampling fa
-00020a50: 6374 6f72 2077 6865 6e20 6361 6c63 756c  ctor when calcul
-00020a60: 6174 696e 6720 7068 6173 6520 6372 6f73  ating phase cros
-00020a70: 7320 636f 7272 656c 6174 696f 6e2e 0d0a  s correlation...
-00020a80: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00020a90: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-00020aa0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-00020ab0: 2020 2020 2020 2020 4d61 726b 6572 4672          MarkerFr
-00020ac0: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
-00020ad0: 2044 6174 6146 7261 6d65 2073 7472 7563   DataFrame struc
-00020ae0: 7475 7265 2077 6974 6820 782c 7920 636f  ture with x,y co
-00020af0: 6c75 6d6e 730d 0a20 2020 2020 2020 2022  lumns..        "
-00020b00: 2222 2020 2020 2020 2020 0d0a 2020 2020  ""        ..    
-00020b10: 2020 2020 6672 6f6d 202e 2e66 7261 6d65      from ..frame
-00020b20: 2069 6d70 6f72 7420 4d61 726b 6572 4672   import MarkerFr
-00020b30: 616d 650d 0a20 2020 2020 2020 200d 0a20  ame..        .. 
-00020b40: 2020 2020 2020 2069 6620 616c 6f6e 6720         if along 
-00020b50: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00020b60: 2020 2020 2020 616c 6f6e 6720 3d20 6669        along = fi
-00020b70: 6e64 5f66 6972 7374 5f61 7070 6561 7265  nd_first_appeare
-00020b80: 6428 2274 707a 6369 6122 2c20 696e 636c  d("tpzcia", incl
-00020b90: 7564 653d 7365 6c66 2e61 7865 7329 0d0a  ude=self.axes)..
-00020ba0: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
-00020bb0: 2861 6c6f 6e67 2920 213d 2031 3a0d 0a20  (along) != 1:.. 
-00020bc0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00020bd0: 2056 616c 7565 4572 726f 7228 2260 616c   ValueError("`al
-00020be0: 6f6e 6760 206d 7573 7420 6265 2073 696e  ong` must be sin
-00020bf0: 676c 6520 6368 6172 6163 7465 722e 2229  gle character.")
-00020c00: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00020c10: 2069 7369 6e73 7461 6e63 6528 7570 7361   isinstance(upsa
-00020c20: 6d70 6c65 5f66 6163 746f 722c 2069 6e74  mple_factor, int
-00020c30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00020c40: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00020c50: 6622 7570 7361 6d70 6c65 2d66 6163 746f  f"upsample-facto
-00020c60: 7220 6d75 7374 2062 6520 696e 7465 6765  r must be intege
-00020c70: 7220 6275 7420 676f 7420 7b74 7970 6528  r but got {type(
-00020c80: 7570 7361 6d70 6c65 5f66 6163 746f 7229  upsample_factor)
-00020c90: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
-00020ca0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00020cb0: 2020 2072 6573 756c 7420 3d20 6e70 2e7a     result = np.z
-00020cc0: 6572 6f73 2828 7365 6c66 2e73 697a 656f  eros((self.sizeo
-00020cd0: 6628 616c 6f6e 6729 2c20 7365 6c66 2e6e  f(along), self.n
-00020ce0: 6469 6d2d 3129 2c20 6474 7970 653d 6e70  dim-1), dtype=np
-00020cf0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00020d00: 2020 2063 5f61 7865 7320 3d20 636f 6d70     c_axes = comp
-00020d10: 6c65 6d65 6e74 5f61 7865 7328 616c 6f6e  lement_axes(alon
-00020d20: 672c 2073 656c 662e 6178 6573 290d 0a20  g, self.axes).. 
-00020d30: 2020 2020 2020 206c 6173 745f 696d 6720         last_img 
-00020d40: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00020d50: 696d 675f 6666 7420 3d20 7365 6c66 2e66  img_fft = self.f
-00020d60: 6674 2873 6869 6674 3d46 616c 7365 2c20  ft(shift=False, 
-00020d70: 6469 6d73 3d63 5f61 7865 7329 0d0a 2020  dims=c_axes)..  
-00020d80: 2020 2020 2020 666f 7220 692c 2028 5f2c        for i, (_,
-00020d90: 2069 6d67 2920 696e 2065 6e75 6d65 7261   img) in enumera
-00020da0: 7465 2869 6d67 5f66 6674 2e69 7465 7228  te(img_fft.iter(
-00020db0: 616c 6f6e 6729 293a 0d0a 2020 2020 2020  along)):..      
-00020dc0: 2020 2020 2020 696d 6720 3d20 7870 2e61        img = xp.a
-00020dd0: 7361 7272 6179 2869 6d67 290d 0a20 2020  sarray(img)..   
-00020de0: 2020 2020 2020 2020 2069 6620 6c61 7374           if last
-00020df0: 5f69 6d67 2069 7320 6e6f 7420 4e6f 6e65  _img is not None
-00020e00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00020e10: 2020 2072 6573 756c 745b 695d 203d 2078     result[i] = x
-00020e20: 702e 6173 6e75 6d70 7928 0d0a 2020 2020  p.asnumpy(..    
-00020e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e40: 5f63 6f72 722e 7375 6270 6978 656c 5f70  _corr.subpixel_p
-00020e50: 6363 286c 6173 745f 696d 672c 2069 6d67  cc(last_img, img
-00020e60: 2c20 7570 7361 6d70 6c65 5f66 6163 746f  , upsample_facto
-00020e70: 723d 7570 7361 6d70 6c65 5f66 6163 746f  r=upsample_facto
-00020e80: 7229 5b30 5d0d 0a20 2020 2020 2020 2020  r)[0]..         
-00020e90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00020ea0: 2020 2020 2020 2020 2020 6c61 7374 5f69            last_i
-00020eb0: 6d67 203d 2069 6d67 0d0a 2020 2020 2020  mg = img..      
-00020ec0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00020ed0: 2020 2020 2020 2020 2020 2020 206c 6173               las
-00020ee0: 745f 696d 6720 3d20 696d 670d 0a20 2020  t_img = img..   
-00020ef0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-00020f00: 6573 756c 7420 3d20 4d61 726b 6572 4672  esult = MarkerFr
-00020f10: 616d 6528 6e70 2e63 756d 7375 6d28 7265  ame(np.cumsum(re
-00020f20: 7375 6c74 2c20 6178 6973 3d30 292c 2063  sult, axis=0), c
-00020f30: 6f6c 756d 6e73 3d63 5f61 7865 7329 0d0a  olumns=c_axes)..
-00020f40: 2020 2020 2020 2020 6966 2073 686f 775f          if show_
-00020f50: 6472 6966 743a 0d0a 2020 2020 2020 2020  drift:..        
-00020f60: 2020 2020 6672 6f6d 202e 5f75 7469 6c73      from ._utils
-00020f70: 2069 6d70 6f72 7420 5f70 6c6f 7420 6173   import _plot as
-00020f80: 205f 706c 740d 0a20 2020 2020 2020 2020   _plt..         
-00020f90: 2020 205f 706c 742e 706c 6f74 5f64 7269     _plt.plot_dri
-00020fa0: 6674 2872 6573 756c 7429 0d0a 2020 2020  ft(result)..    
-00020fb0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-00020fc0: 7375 6c74 2e69 6e64 6578 2e6e 616d 6520  sult.index.name 
-00020fd0: 3d20 7374 7228 616c 6f6e 6729 0d0a 2020  = str(along)..  
-00020fe0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00020ff0: 756c 740d 0a20 2020 200d 0a20 2020 2040  ult..    ..    @
-00021000: 5f64 6f63 732e 7772 6974 655f 646f 6373  _docs.write_docs
-00021010: 0d0a 2020 2020 4064 696d 735f 746f 5f73  ..    @dims_to_s
-00021020: 7061 7469 616c 5f61 7865 730d 0a20 2020  patial_axes..   
-00021030: 2040 7361 6d65 5f64 7479 7065 2861 7366   @same_dtype(asf
-00021040: 6c6f 6174 3d54 7275 6529 0d0a 2020 2020  loat=True)..    
-00021050: 4063 6865 636b 5f69 6e70 7574 5f61 6e64  @check_input_and
-00021060: 5f6f 7574 7075 740d 0a20 2020 2064 6566  _output..    def
-00021070: 2064 7269 6674 5f63 6f72 7265 6374 696f   drift_correctio
-00021080: 6e28 0d0a 2020 2020 2020 2020 7365 6c66  n(..        self
-00021090: 2c0d 0a20 2020 2020 2020 2073 6869 6674  ,..        shift
-000210a0: 3a20 436f 6f72 6473 203d 204e 6f6e 652c  : Coords = None,
-000210b0: 0d0a 2020 2020 2020 2020 7265 663a 2049  ..        ref: I
-000210c0: 6d67 4172 7261 7920 3d20 4e6f 6e65 2c0d  mgArray = None,.
-000210d0: 0a20 2020 2020 2020 202a 2c0d 0a20 2020  .        *,..   
-000210e0: 2020 2020 207a 6572 6f5f 6176 653a 2062       zero_ave: b
-000210f0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
-00021100: 2020 2020 2061 6c6f 6e67 3a20 4178 6973       along: Axis
-00021110: 4c69 6b65 207c 204e 6f6e 6520 3d20 4e6f  Like | None = No
-00021120: 6e65 2c0d 0a20 2020 2020 2020 206f 7264  ne,..        ord
-00021130: 6572 3a20 696e 7420 3d20 312c 0d0a 2020  er: int = 1,..  
-00021140: 2020 2020 2020 6d6f 6465 3a20 7374 7220        mode: str 
-00021150: 3d20 2263 6f6e 7374 616e 7422 2c0d 0a20  = "constant",.. 
-00021160: 2020 2020 2020 2063 7661 6c3a 2066 6c6f         cval: flo
-00021170: 6174 203d 2030 2c0d 0a20 2020 2020 2020  at = 0,..       
-00021180: 2064 696d 733a 2044 696d 7320 3d20 322c   dims: Dims = 2,
-00021190: 0d0a 2020 2020 2020 2020 7570 6461 7465  ..        update
-000211a0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
-000211b0: 0a20 2020 2029 202d 3e20 496d 6741 7272  .    ) -> ImgArr
-000211c0: 6179 3a0d 0a20 2020 2020 2020 2022 2222  ay:..        """
-000211d0: 0d0a 2020 2020 2020 2020 4472 6966 7420  ..        Drift 
-000211e0: 636f 7272 6563 7469 6f6e 2075 7369 6e67  correction using
-000211f0: 2069 7465 7261 7469 7665 2041 6666 696e   iterative Affin
-00021200: 6520 7472 616e 736c 6174 696f 6e2e 2049  e translation. I
-00021210: 6620 7472 616e 736c 6174 696f 6e20 7665  f translation ve
-00021220: 6374 6f72 7320 6060 7368 6966 7460 600d  ctors ``shift``.
-00021230: 0a20 2020 2020 2020 2069 7320 6e6f 7420  .        is not 
-00021240: 6769 7665 6e2c 2074 6865 6e20 6974 2077  given, then it w
-00021250: 696c 6c20 6265 2064 6574 6572 6d69 6e65  ill be determine
-00021260: 6420 7573 696e 6720 6060 7472 6163 6b5f  d using ``track_
-00021270: 6472 6966 7460 6020 6d65 7468 6f64 206f  drift`` method o
-00021280: 6620 496d 6741 7272 6179 2e0d 0a0d 0a20  f ImgArray..... 
-00021290: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000212a0: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-000212b0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-000212c0: 6869 6674 203a 2044 6174 6146 7261 6d65  hift : DataFrame
-000212d0: 206f 7220 284e 2c20 4429 2061 7272 6179   or (N, D) array
-000212e0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-000212f0: 2020 2020 2020 2020 5472 616e 736c 6174          Translat
-00021300: 696f 6e20 7665 6374 6f72 732e 2049 6620  ion vectors. If 
-00021310: 4461 7461 4672 616d 652c 2069 7420 6d75  DataFrame, it mu
-00021320: 7374 2068 6176 6520 636f 6c75 6d6e 7320  st have columns 
-00021330: 6e61 6d65 6420 7769 7468 2061 6c6c 2074  named with all t
-00021340: 6865 2073 796d 626f 6c73 0d0a 2020 2020  he symbols..    
-00021350: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
-00021360: 6420 696e 2060 6064 696d 7360 602e 0d0a  d in ``dims``...
-00021370: 2020 2020 2020 2020 7265 6620 3a20 496d          ref : Im
-00021380: 6741 7272 6179 2c20 6f70 7469 6f6e 616c  gArray, optional
-00021390: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-000213a0: 6520 7265 6665 7265 6e63 6520 6e2d 4420  e reference n-D 
-000213b0: 696d 6167 6520 746f 2064 6574 6572 6d69  image to determi
-000213c0: 6e65 2064 7269 6674 2c20 6966 2060 6073  ne drift, if ``s
-000213d0: 6869 6674 6060 2077 6173 206e 6f74 2067  hift`` was not g
-000213e0: 6976 656e 2e0d 0a20 2020 2020 2020 207a  iven...        z
-000213f0: 6572 6f5f 6176 6520 3a20 626f 6f6c 2c20  ero_ave : bool, 
-00021400: 6465 6661 756c 7420 6973 2054 7275 650d  default is True.
-00021410: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00021420: 5472 7565 2c20 6176 6572 6167 6520 7368  True, average sh
-00021430: 6966 7420 7769 6c6c 2062 6520 7a65 726f  ift will be zero
-00021440: 2e0d 0a20 2020 2020 2020 2061 6c6f 6e67  ...        along
-00021450: 203a 2041 7869 734c 696b 652c 206f 7074   : AxisLike, opt
-00021460: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-00021470: 2020 2041 6c6f 6e67 2077 6869 6368 2061     Along which a
-00021480: 7869 7320 6472 6966 7420 7769 6c6c 2062  xis drift will b
-00021490: 6520 636f 7272 6563 7465 642e 0d0a 2020  e corrected...  
-000214a0: 2020 2020 2020 7b64 696d 737d 7b75 7064        {dims}{upd
-000214b0: 6174 657d 0d0a 2020 2020 2020 2020 6166  ate}..        af
-000214c0: 6669 6e65 5f6b 7761 7267 7320 3a0d 0a20  fine_kwargs :.. 
-000214d0: 2020 2020 2020 2020 2020 204b 6579 776f             Keywo
-000214e0: 7264 2061 7267 756d 656e 7473 2074 6861  rd arguments tha
-000214f0: 7420 7769 6c6c 2062 6520 7061 7373 6564  t will be passed
-00021500: 2074 6f20 6060 7761 7270 6060 2e0d 0a0d   to ``warp``....
-00021510: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00021520: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00021530: 2d0d 0a20 2020 2020 2020 2049 6d67 4172  -..        ImgAr
-00021540: 7261 790d 0a20 2020 2020 2020 2020 2020  ray..           
-00021550: 2043 6f72 7265 6374 6564 2069 6d61 6765   Corrected image
-00021560: 2e0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
-00021570: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00021580: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00021590: 2d2d 2d0d 0a20 2020 2020 2020 2044 7269  ---..        Dri
-000215a0: 6674 2063 6f72 7265 6374 696f 6e20 6f66  ft correction of
-000215b0: 206d 756c 7469 6368 616e 6e65 6c20 696d   multichannel im
-000215c0: 6167 6520 7573 696e 6720 7468 6520 6669  age using the fi
-000215d0: 7273 7420 6368 616e 6e65 6c20 6173 2074  rst channel as t
-000215e0: 6865 2072 6566 6572 656e 6365 2e0d 0a20  he reference... 
-000215f0: 2020 2020 2020 2020 2020 203e 3e3e 2069             >>> i
-00021600: 6d67 2e64 7269 6674 5f63 6f72 7265 6374  mg.drift_correct
-00021610: 696f 6e28 7265 663d 696d 675b 2263 3d30  ion(ref=img["c=0
-00021620: 225d 290d 0a20 2020 2020 2020 2022 2222  "])..        """
-00021630: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00021640: 2020 0d0a 2020 2020 2020 2020 6966 2061    ..        if a
-00021650: 6c6f 6e67 2069 7320 4e6f 6e65 3a0d 0a20  long is None:.. 
-00021660: 2020 2020 2020 2020 2020 2061 6c6f 6e67             along
-00021670: 203d 2066 696e 645f 6669 7273 745f 6170   = find_first_ap
-00021680: 7065 6172 6564 2822 7470 7a63 6961 222c  peared("tpzcia",
-00021690: 2069 6e63 6c75 6465 3d73 656c 662e 6178   include=self.ax
-000216a0: 6573 2c20 6578 636c 7564 653d 6469 6d73  es, exclude=dims
-000216b0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-000216c0: 6c65 6e28 616c 6f6e 6729 2021 3d20 313a  len(along) != 1:
-000216d0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000216e0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-000216f0: 6061 6c6f 6e67 6020 6d75 7374 2062 6520  `along` must be 
-00021700: 7369 6e67 6c65 2063 6861 7261 6374 6572  single character
-00021710: 2e22 290d 0a20 2020 2020 2020 200d 0a20  .")..        .. 
-00021720: 2020 2020 2020 2069 6620 7368 6966 7420         if shift 
-00021730: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00021740: 2020 2020 2020 2320 6465 7465 726d 696e        # determin
-00021750: 6520 2772 6566 270d 0a20 2020 2020 2020  e 'ref'..       
-00021760: 2020 2020 2069 6620 7265 6620 6973 204e       if ref is N
-00021770: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00021780: 2020 2020 2020 7265 6620 3d20 7365 6c66        ref = self
-00021790: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000217a0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-000217b0: 6528 7265 662c 2049 6d67 4172 7261 7929  e(ref, ImgArray)
-000217c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000217d0: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-000217e0: 6f72 2866 2227 7265 6627 206d 7573 7420  or(f"'ref' must 
-000217f0: 6265 2061 6e20 496d 6741 7272 6179 206f  be an ImgArray o
-00021800: 626a 6563 742c 2062 7574 2067 6f74 207b  bject, but got {
-00021810: 7479 7065 2872 6566 297d 2229 0d0a 2020  type(ref)}")..  
-00021820: 2020 2020 2020 2020 2020 6966 2072 6566            if ref
-00021830: 2e61 7865 7320 213d 205b 616c 6f6e 675d  .axes != [along]
-00021840: 202b 2064 696d 733a 0d0a 2020 2020 2020   + dims:..      
-00021850: 2020 2020 2020 2020 2020 6672 6f6d 2069            from i
-00021860: 7465 7274 6f6f 6c73 2069 6d70 6f72 7420  tertools import 
-00021870: 7072 6f64 7563 740d 0a20 2020 2020 2020  product..       
-00021880: 2020 2020 2020 2020 205f 635f 6178 6573           _c_axes
-00021890: 203d 2063 6f6d 706c 656d 656e 745f 6178   = complement_ax
-000218a0: 6573 285b 616c 6f6e 675d 202b 2064 696d  es([along] + dim
-000218b0: 732c 2073 7472 2872 6566 2e61 7865 7329  s, str(ref.axes)
-000218c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000218d0: 2020 2066 6d74 203d 2073 6c69 6365 722e     fmt = slicer.
-000218e0: 6765 745f 666f 726d 6174 7465 7228 5f63  get_formatter(_c
-000218f0: 5f61 7865 7329 0d0a 2020 2020 2020 2020  _axes)..        
-00021900: 2020 2020 2020 2020 6f75 7420 3d20 6e70          out = np
-00021910: 2e65 6d70 7479 5f6c 696b 6528 7365 6c66  .empty_like(self
-00021920: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00021930: 2020 2066 6f72 2069 6478 2069 6e20 7072     for idx in pr
-00021940: 6f64 7563 7428 2a28 7261 6e67 6528 7265  oduct(*(range(re
-00021950: 662e 7369 7a65 6f66 2861 2929 2066 6f72  f.sizeof(a)) for
-00021960: 2061 2069 6e20 5f63 5f61 7865 7329 293a   a in _c_axes)):
-00021970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021980: 2020 2020 2020 736c 203d 2066 6d74 5b69        sl = fmt[i
-00021990: 6478 5d0d 0a20 2020 2020 2020 2020 2020  dx]..           
-000219a0: 2020 2020 2020 2020 206f 7574 5b73 6c5d           out[sl]
-000219b0: 203d 2073 656c 665b 736c 5d2e 6472 6966   = self[sl].drif
-000219c0: 745f 636f 7272 6563 7469 6f6e 280d 0a20  t_correction(.. 
-000219d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219e0: 2020 2020 2020 2072 6566 3d72 6566 5b73         ref=ref[s
-000219f0: 6c5d 2c20 7a65 726f 5f61 7665 3d7a 6572  l], zero_ave=zer
-00021a00: 6f5f 6176 652c 2061 6c6f 6e67 3d61 6c6f  o_ave, along=alo
-00021a10: 6e67 2c20 6469 6d73 3d64 696d 732c 0d0a  ng, dims=dims,..
-00021a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021a30: 2020 2020 2020 2020 7570 6461 7465 3d75          update=u
-00021a40: 7064 6174 652c 206f 7264 6572 3d6f 7264  pdate, order=ord
-00021a50: 6572 2c20 6d6f 6465 3d6d 6f64 652c 2063  er, mode=mode, c
-00021a60: 7661 6c3d 6376 616c 2c0d 0a20 2020 2020  val=cval,..     
-00021a70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00021a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021a90: 2020 7265 7475 726e 206f 7574 0d0a 0d0a    return out....
-00021aa0: 2020 2020 2020 2020 2020 2020 7368 6966              shif
-00021ab0: 7420 3d20 7265 662e 7472 6163 6b5f 6472  t = ref.track_dr
-00021ac0: 6966 7428 616c 6f6e 673d 616c 6f6e 6729  ift(along=along)
-00021ad0: 2e76 616c 7565 730d 0a20 2020 2020 2020  .values..       
-00021ae0: 2020 2020 200d 0a20 2020 2020 2020 2065       ..        e
-00021af0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00021b00: 2020 7368 6966 7420 3d20 6e70 2e61 7361    shift = np.asa
-00021b10: 7272 6179 2873 6869 6674 2c20 6474 7970  rray(shift, dtyp
-00021b20: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00021b30: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-00021b40: 656c 662e 7369 7a65 6f66 2861 6c6f 6e67  elf.sizeof(along
-00021b50: 292c 2073 656c 662e 6e64 696d 2920 213d  ), self.ndim) !=
-00021b60: 2073 6869 6674 2e73 6861 7065 3a0d 0a20   shift.shape:.. 
-00021b70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00021b80: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00021b90: 2257 726f 6e67 2073 6861 7065 206f 6620  "Wrong shape of 
-00021ba0: 6073 6869 6674 602e 2229 0d0a 0d0a 2020  `shift`.")....  
-00021bb0: 2020 2020 2020 6966 207a 6572 6f5f 6176        if zero_av
-00021bc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00021bd0: 7368 6966 7420 3d20 7368 6966 7420 2d20  shift = shift - 
-00021be0: 6e70 2e6d 6561 6e28 7368 6966 742c 2061  np.mean(shift, a
-00021bf0: 7869 733d 3029 0d0a 2020 2020 2020 2020  xis=0)..        
-00021c00: 2020 2020 0d0a 2020 2020 2020 2020 6f75      ..        ou
-00021c10: 7420 3d20 7870 2e65 6d70 7479 2873 656c  t = xp.empty(sel
-00021c20: 662e 7368 6170 6529 0d0a 2020 2020 2020  f.shape)..      
-00021c30: 2020 745f 696e 6465 7820 3d20 7365 6c66    t_index = self
-00021c40: 2e61 7869 736f 6628 616c 6f6e 6729 0d0a  .axisof(along)..
-00021c50: 2020 2020 2020 2020 6e64 696d 203d 206c          ndim = l
-00021c60: 656e 2864 696d 7329 0d0a 2020 2020 2020  en(dims)..      
-00021c70: 2020 6d78 203d 206e 702e 6579 6528 6e64    mx = np.eye(nd
-00021c80: 696d 202b 2031 2c20 6474 7970 653d 6e70  im + 1, dtype=np
-00021c90: 2e66 6c6f 6174 3332 2920 2320 4166 6669  .float32) # Affi
-00021ca0: 6e65 2074 7261 6e73 666f 726d 6174 696f  ne transformatio
-00021cb0: 6e20 6d61 7472 6978 0d0a 2020 2020 2020  n matrix..      
-00021cc0: 2020 696e 7075 745f 696d 6720 3d20 7365    input_img = se
-00021cd0: 6c66 2e73 706c 696e 655f 6669 6c74 6572  lf.spline_filter
-00021ce0: 286d 6f64 653d 6d6f 6465 2c20 6f72 6465  (mode=mode, orde
-00021cf0: 723d 6f72 6465 7229 0d0a 2020 2020 2020  r=order)..      
-00021d00: 2020 666f 7220 736c 2c20 696d 6720 696e    for sl, img in
-00021d10: 2069 6e70 7574 5f69 6d67 2e69 7465 7228   input_img.iter(
-00021d20: 636f 6d70 6c65 6d65 6e74 5f61 7865 7328  complement_axes(
-00021d30: 6469 6d73 2c20 7365 6c66 2e61 7865 7329  dims, self.axes)
-00021d40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00021d50: 6d78 5b3a 2d31 2c20 2d31 5d20 3d20 2d73  mx[:-1, -1] = -s
-00021d60: 6869 6674 5b73 6c5b 745f 696e 6465 785d  hift[sl[t_index]
-00021d70: 5d0d 0a20 2020 2020 2020 2020 2020 206f  ]..            o
-00021d80: 7574 5b73 6c5d 203d 205f 7472 616e 7366  ut[sl] = _transf
-00021d90: 6f72 6d2e 7761 7270 2869 6d67 2c20 6d78  orm.warp(img, mx
-00021da0: 2c20 6d6f 6465 3d6d 6f64 652c 2063 7661  , mode=mode, cva
-00021db0: 6c3d 6376 616c 2c20 6f72 6465 723d 6f72  l=cval, order=or
-00021dc0: 6465 722c 2070 7265 6669 6c74 6572 3d46  der, prefilter=F
-00021dd0: 616c 7365 290d 0a20 2020 2020 2020 200d  alse)..        .
-00021de0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00021df0: 6f75 740d 0a0d 0a20 2020 2040 5f64 6f63  out....    @_doc
-00021e00: 732e 7772 6974 655f 646f 6373 0d0a 2020  s.write_docs..  
-00021e10: 2020 4064 696d 735f 746f 5f73 7061 7469    @dims_to_spati
-00021e20: 616c 5f61 7865 730d 0a20 2020 2040 6368  al_axes..    @ch
-00021e30: 6563 6b5f 696e 7075 745f 616e 645f 6f75  eck_input_and_ou
-00021e40: 7470 7574 0d0a 2020 2020 6465 6620 6573  tput..    def es
-00021e50: 7469 6d61 7465 5f73 6967 6d61 2873 656c  timate_sigma(sel
-00021e60: 662c 202a 2c20 7371 7565 657a 653a 2062  f, *, squeeze: b
-00021e70: 6f6f 6c20 3d20 5472 7565 2c20 6469 6d73  ool = True, dims
-00021e80: 3a20 4469 6d73 203d 204e 6f6e 6529 202d  : Dims = None) -
-00021e90: 3e20 5072 6f70 4172 7261 7920 7c20 666c  > PropArray | fl
-00021ea0: 6f61 743a 0d0a 2020 2020 2020 2020 2222  oat:..        ""
-00021eb0: 220d 0a20 2020 2020 2020 2057 6176 656c  "..        Wavel
-00021ec0: 6574 2d62 6173 6564 2065 7374 696d 6174  et-based estimat
-00021ed0: 696f 6e20 6f66 2047 6175 7373 6961 6e20  ion of Gaussian 
-00021ee0: 6e6f 6973 652e 0d0a 0d0a 2020 2020 2020  noise.....      
-00021ef0: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00021f00: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00021f10: 0d0a 2020 2020 2020 2020 7371 7565 657a  ..        squeez
-00021f20: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
-00021f30: 7420 6973 2054 7275 650d 0a20 2020 2020  t is True..     
-00021f40: 2020 2020 2020 2049 6620 5472 7565 2061         If True a
-00021f50: 6e64 206f 7574 7075 7420 6361 6e20 6265  nd output can be
-00021f60: 2063 6f6e 7665 7274 6564 2074 6f20 6120   converted to a 
-00021f70: 7363 616c 6172 2c20 7468 656e 2063 6f6e  scalar, then con
-00021f80: 7665 7274 2069 742e 0d0a 2020 2020 2020  vert it...      
-00021f90: 2020 7b64 696d 737d 0d0a 0d0a 2020 2020    {dims}....    
-00021fa0: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-00021fb0: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-00021fc0: 2020 2020 2020 5072 6f70 4172 7261 7920        PropArray 
-00021fd0: 6f72 2066 6c6f 6174 0d0a 2020 2020 2020  or float..      
-00021fe0: 2020 2020 2020 4573 7469 6d61 7465 6420        Estimated 
-00021ff0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-00022000: 6f6e 2e20 7369 676d 615b 2274 3d30 3b63  on. sigma["t=0;c
-00022010: 3d31 225d 206d 6561 6e73 2074 6865 2065  =1"] means the e
-00022020: 7374 696d 6174 6564 2076 616c 7565 206f  stimated value o
-00022030: 660d 0a20 2020 2020 2020 2020 2020 2069  f..            i
-00022040: 6d61 6765 2073 6c69 6365 2061 7420 743d  mage slice at t=
-00022050: 3020 616e 6420 633d 312e 0d0a 2020 2020  0 and c=1...    
-00022060: 2020 2020 2222 2220 2020 2020 2020 200d      """        .
-00022070: 0a20 2020 2020 2020 2063 5f61 7865 7320  .        c_axes 
-00022080: 3d20 636f 6d70 6c65 6d65 6e74 5f61 7865  = complement_axe
-00022090: 7328 6469 6d73 2c20 7365 6c66 2e61 7865  s(dims, self.axe
-000220a0: 7329 0d0a 2020 2020 2020 2020 6f75 7420  s)..        out 
-000220b0: 3d20 7365 6c66 2e5f 6170 706c 795f 6461  = self._apply_da
-000220c0: 736b 280d 0a20 2020 2020 2020 2020 2020  sk(..           
-000220d0: 2073 6b72 6573 2e65 7374 696d 6174 655f   skres.estimate_
-000220e0: 7369 676d 612c 0d0a 2020 2020 2020 2020  sigma,..        
-000220f0: 2020 2020 635f 6178 6573 3d63 5f61 7865      c_axes=c_axe
-00022100: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00022110: 6472 6f70 5f61 7869 733d 6469 6d73 0d0a  drop_axis=dims..
-00022120: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00022130: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00022140: 2069 6620 6f75 742e 6e64 696d 203d 3d20   if out.ndim == 
-00022150: 3020 616e 6420 7371 7565 657a 653a 0d0a  0 and squeeze:..
-00022160: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-00022170: 3d20 6f75 742e 6974 656d 2829 0d0a 2020  = out.item()..  
-00022180: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00022190: 2020 2020 2020 2020 206f 7574 203d 2050           out = P
-000221a0: 726f 7041 7272 6179 280d 0a20 2020 2020  ropArray(..     
-000221b0: 2020 2020 2020 2020 2020 206f 7574 2c20             out, 
-000221c0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-000221d0: 2c20 6e61 6d65 3d73 656c 662e 6e61 6d65  , name=self.name
-000221e0: 2c20 6178 6573 3d63 5f61 7865 732c 2070  , axes=c_axes, p
-000221f0: 726f 706e 616d 653d 2265 7374 696d 6174  ropname="estimat
-00022200: 655f 7369 676d 6122 0d0a 2020 2020 2020  e_sigma"..      
-00022210: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00022220: 2020 2020 206f 7574 2e5f 7365 745f 696e       out._set_in
-00022230: 666f 2873 656c 662c 206e 6577 5f61 7865  fo(self, new_axe
-00022240: 733d 635f 6178 6573 290d 0a20 2020 2020  s=c_axes)..     
-00022250: 2020 2072 6574 7572 6e20 6f75 7420 2020     return out   
-00022260: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-00022270: 2020 2020 0d0a 2020 2020 4064 696d 735f      ..    @dims_
-00022280: 746f 5f73 7061 7469 616c 5f61 7865 730d  to_spatial_axes.
-00022290: 0a20 2020 2040 6368 6563 6b5f 696e 7075  .    @check_inpu
-000222a0: 745f 616e 645f 6f75 7470 7574 0d0a 2020  t_and_output..  
-000222b0: 2020 6465 6620 7061 6428 0d0a 2020 2020    def pad(..    
-000222c0: 2020 2020 7365 6c66 2c20 0d0a 2020 2020      self, ..    
-000222d0: 2020 2020 7061 645f 7769 6474 683a 2069      pad_width: i
-000222e0: 6e74 207c 2074 7570 6c65 5b69 6e74 2c20  nt | tuple[int, 
-000222f0: 696e 745d 207c 2053 6571 7565 6e63 655b  int] | Sequence[
-00022300: 7475 706c 655b 696e 742c 2069 6e74 5d5d  tuple[int, int]]
-00022310: 2c20 0d0a 2020 2020 2020 2020 2a2c 200d  , ..        *, .
-00022320: 0a20 2020 2020 2020 206d 6f64 653a 2050  .        mode: P
-00022330: 6164 6469 6e67 4d6f 6465 203d 2022 636f  addingMode = "co
-00022340: 6e73 7461 6e74 222c 200d 0a20 2020 2020  nstant", ..     
-00022350: 2020 2064 696d 733a 2044 696d 7320 3d20     dims: Dims = 
-00022360: 4e6f 6e65 2c20 0d0a 2020 2020 2020 2020  None, ..        
-00022370: 2a2a 6b77 6172 6773 0d0a 2020 2020 2920  **kwargs..    ) 
-00022380: 2d3e 2049 6d67 4172 7261 793a 0d0a 2020  -> ImgArray:..  
-00022390: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000223a0: 2020 2050 6164 2069 6d61 6765 206f 6e6c     Pad image onl
-000223b0: 7920 666f 7220 7370 6174 6961 6c20 6469  y for spatial di
-000223c0: 6d65 6e73 696f 6e73 2e0d 0a0d 0a20 2020  mensions.....   
-000223d0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-000223e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000223f0: 2d2d 2d0d 0a20 2020 2020 2020 2070 6164  ---..        pad
-00022400: 5f77 6964 7468 2c20 6d6f 6465 2c20 2a2a  _width, mode, **
-00022410: 6b77 6172 6773 203a 200d 0a20 2020 2020  kwargs : ..     
-00022420: 2020 2020 2020 2053 6565 2064 6f63 756d         See docum
-00022430: 656e 7461 7469 6f6e 206f 6620 6e70 2e70  entation of np.p
-00022440: 6164 2829 2e0d 0a20 2020 2020 2020 2064  ad()...        d
-00022450: 696d 7320 3a20 696e 7420 6f72 2073 7472  ims : int or str
-00022460: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00022470: 2020 2020 2020 2020 5768 6963 6820 6469          Which di
-00022480: 6d65 6e73 696f 6e20 746f 2070 6164 2e0d  mension to pad..
-00022490: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000224a0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-000224b0: 2d2d 2d0d 0a20 2020 2020 2020 2049 6d67  ---..        Img
-000224c0: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
-000224d0: 2020 2050 6164 6465 6420 696d 6167 652e     Padded image.
-000224e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000224f0: 2020 2020 4578 616d 706c 6573 0d0a 2020      Examples..  
-00022500: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
-00022510: 2020 2020 2020 2020 5375 7070 6f73 6520          Suppose 
-00022520: 6060 696d 6760 6020 6861 7320 7a79 782d  ``img`` has zyx-
-00022530: 6178 6573 2e0d 0a20 2020 2020 2020 200d  axes...        .
-00022540: 0a20 2020 2020 2020 2031 2e20 5061 6464  .        1. Padd
-00022550: 696e 6720 3520 7069 7865 6c73 2069 6e20  ing 5 pixels in 
-00022560: 7a79 782d 6469 7265 6374 696f 6e3a 0d0a  zyx-direction:..
-00022570: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00022580: 696d 672e 7061 6428 3529 0d0a 2020 2020  img.pad(5)..    
-00022590: 2020 2020 322e 2050 6164 6469 6e67 2035      2. Padding 5
-000225a0: 2070 6978 656c 7320 696e 2079 782d 6469   pixels in yx-di
-000225b0: 7265 6374 696f 6e3a 0d0a 2020 2020 2020  rection:..      
-000225c0: 2020 2020 2020 3e3e 3e20 696d 672e 7061        >>> img.pa
-000225d0: 6428 352c 2064 696d 733d 2279 7822 290d  d(5, dims="yx").
-000225e0: 0a20 2020 2020 2020 2033 2e20 5061 6464  .        3. Padd
-000225f0: 696e 6720 3520 7069 7865 6c73 2069 6e20  ing 5 pixels in 
-00022600: 7978 2d64 6972 6563 7469 6f6e 2061 6e64  yx-direction and
-00022610: 2032 2070 6978 656c 7320 696e 207a 2d64   2 pixels in z-d
-00022620: 6972 6563 7469 6f6e 3a0d 0a20 2020 2020  irection:..     
-00022630: 2020 2020 2020 203e 3e3e 2069 6d67 2e70         >>> img.p
-00022640: 6164 285b 2835 2c35 292c 2028 342c 3429  ad([(5,5), (4,4)
-00022650: 2c20 2834 2c34 295d 290d 0a20 2020 2020  , (4,4)])..     
-00022660: 2020 2034 2e20 5061 6464 696e 6720 3130     4. Padding 10
-00022670: 2070 6978 656c 7320 696e 207a 2d28 2d29   pixels in z-(-)
-00022680: 2d64 6972 6563 7469 6f6e 2061 6e64 2035  -direction and 5
-00022690: 2070 6978 656c 7320 696e 207a 2d28 2b29   pixels in z-(+)
-000226a0: 2d64 6972 6563 7469 6f6e 2e0d 0a20 2020  -direction...   
-000226b0: 2020 2020 2020 2020 203e 3e3e 2069 6d67           >>> img
-000226c0: 2e70 6164 285b 2831 302c 2035 295d 2c20  .pad([(10, 5)], 
-000226d0: 6469 6d73 3d22 7a22 290d 0a20 2020 2020  dims="z")..     
-000226e0: 2020 2022 2222 2020 2020 2020 2020 0d0a     """        ..
-000226f0: 2020 2020 2020 2020 7061 645f 7769 6474          pad_widt
-00022700: 6820 3d20 5f6d 6973 632e 6d61 6b65 5f70  h = _misc.make_p
-00022710: 6164 2870 6164 5f77 6964 7468 2c20 6469  ad(pad_width, di
-00022720: 6d73 2c20 7365 6c66 2e61 7865 732c 202a  ms, self.axes, *
-00022730: 2a6b 7761 7267 7329 0d0a 2020 2020 2020  *kwargs)..      
-00022740: 2020 7061 6469 6d67 203d 206e 702e 7061    padimg = np.pa
-00022750: 6428 7365 6c66 2e76 616c 7565 2c20 7061  d(self.value, pa
-00022760: 645f 7769 6474 682c 206d 6f64 652c 202a  d_width, mode, *
-00022770: 2a6b 7761 7267 7329 2e76 6965 7728 7365  *kwargs).view(se
-00022780: 6c66 2e5f 5f63 6c61 7373 5f5f 290d 0a20  lf.__class__).. 
-00022790: 2020 2020 2020 2072 6574 7572 6e20 7061         return pa
-000227a0: 6469 6d67 0d0a 2020 2020 0d0a 2020 2020  dimg..    ..    
-000227b0: 4073 616d 655f 6474 7970 6528 6173 666c  @same_dtype(asfl
-000227c0: 6f61 743d 5472 7565 290d 0a20 2020 2040  oat=True)..    @
-000227d0: 6368 6563 6b5f 696e 7075 745f 616e 645f  check_input_and_
-000227e0: 6f75 7470 7574 0d0a 2020 2020 6465 6620  output..    def 
-000227f0: 7061 645f 6465 666f 6375 7328 7365 6c66  pad_defocus(self
-00022800: 2c20 6b65 726e 656c 2c20 2a2c 2064 6570  , kernel, *, dep
-00022810: 7468 3a20 696e 7420 3d20 332c 2077 6964  th: int = 3, wid
-00022820: 7468 3a20 696e 7420 3d20 362c 2062 673a  th: int = 6, bg:
-00022830: 2066 6c6f 6174 203d 204e 6f6e 6529 202d   float = None) -
-00022840: 3e20 496d 6741 7272 6179 3a0d 0a20 2020  > ImgArray:..   
-00022850: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00022860: 2020 4d61 6b65 2061 207a 2d64 6972 6563    Make a z-direc
-00022870: 7469 6f6e 616c 2070 6164 6465 6420 696d  tional padded im
-00022880: 6167 6520 6279 2064 6566 6f63 7573 696e  age by defocusin
-00022890: 6720 7468 6520 6f72 6967 696e 616c 2069  g the original i
-000228a0: 6d61 6765 2e20 5468 6973 2070 6164 6469  mage. This paddi
-000228b0: 6e67 2069 730d 0a20 2020 2020 2020 2075  ng is..        u
-000228c0: 7365 6675 6c20 7768 656e 2061 7070 6c79  seful when apply
-000228d0: 696e 6720 4646 5420 746f 2061 2033 4420  ing FFT to a 3D 
-000228e0: 696d 6167 652e 0d0a 2020 2020 2020 2020  image...        
-000228f0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00022900: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00022910: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00022920: 2020 6b65 726e 656c 203a 2030 2d2c 2031    kernel : 0-, 1
-00022930: 2d20 6f72 2033 2d64 696d 656e 7369 6f6e  - or 3-dimension
-00022940: 616c 2061 7272 6179 2e0d 0a20 2020 2020  al array...     
-00022950: 2020 2020 2020 2049 6620 302d 2028 7363         If 0- (sc
-00022960: 616c 6172 2920 6f72 2031 2d64 696d 656e  alar) or 1-dimen
-00022970: 7369 6f6e 616c 2061 7272 6179 2077 6173  sional array was
-00022980: 2067 6976 656e 2c20 7468 6973 2069 7320   given, this is 
-00022990: 696e 7465 7270 7265 7465 6420 6173 2073  interpreted as s
-000229a0: 7461 6e64 6172 640d 0a20 2020 2020 2020  tandard..       
-000229b0: 2020 2020 2064 6576 6961 7469 6f6e 206f       deviation o
-000229c0: 6620 4761 7573 7369 616e 206b 6572 6e65  f Gaussian kerne
-000229d0: 6c2e 2049 6620 332d 6469 6d65 6e73 696f  l. If 3-dimensio
-000229e0: 6e61 6c20 6172 7261 7920 7761 7320 6769  nal array was gi
-000229f0: 7665 6e2c 2074 6869 7320 6973 2064 6972  ven, this is dir
-00022a00: 6563 746c 790d 0a20 2020 2020 2020 2020  ectly..         
-00022a10: 2020 2075 7365 6420 6173 2063 6f6e 766f     used as convo
-00022a20: 6c75 7469 6f6e 206b 6572 6e65 6c2e 204f  lution kernel. O
-00022a30: 7468 6572 2064 696d 656e 7369 6f6e 2077  ther dimension w
-00022a40: 696c 6c20 7261 6973 6520 5661 6c75 6545  ill raise ValueE
-00022a50: 7272 6f72 2e0d 0a20 2020 2020 2020 2064  rror...        d
-00022a60: 6570 7468 203a 2069 6e74 2c20 6465 6661  epth : int, defa
-00022a70: 756c 7420 6973 2033 0d0a 2020 2020 2020  ult is 3..      
-00022a80: 2020 2020 2020 4465 7074 6820 6f66 2064        Depth of d
-00022a90: 6566 6f63 7573 696e 672e 2046 6f72 2061  efocusing. For a
-00022aa0: 6e20 696d 6167 6520 7769 7468 207a 2d61  n image with z-a
-00022ab0: 7869 7320 7369 7a65 204c 2c20 7468 656e  xis size L, then
-00022ac0: 206f 7574 7075 7420 696d 6167 6520 7769   output image wi
-00022ad0: 6c6c 2068 6176 650d 0a20 2020 2020 2020  ll have..       
-00022ae0: 2020 2020 2073 697a 6520 4c20 2b20 322a       size L + 2*
-00022af0: 6465 7074 682e 0d0a 2020 2020 2020 2020  depth...        
-00022b00: 7769 6474 6820 3a20 696e 742c 2064 6566  width : int, def
-00022b10: 6175 6c74 2069 7320 360d 0a20 2020 2020  ault is 6..     
-00022b20: 2020 2020 2020 2057 6964 7468 206f 6620         Width of 
-00022b30: 6465 666f 6375 7369 6e67 2e20 466f 7220  defocusing. For 
-00022b40: 616e 2069 6d61 6765 2077 6974 6820 7978  an image with yx
-00022b50: 2d73 6861 7065 2028 4d2c 204e 292c 2074  -shape (M, N), t
-00022b60: 6865 6e20 6f75 7470 7574 2069 6d61 6765  hen output image
-00022b70: 2077 696c 6c20 6861 7665 0d0a 2020 2020   will have..    
-00022b80: 2020 2020 2020 2020 7368 6170 6520 284d          shape (M
-00022b90: 202a 2032 2a77 6964 7468 2c20 4e20 2b20   * 2*width, N + 
-00022ba0: 322a 7769 6474 6829 2e0d 0a20 2020 2020  2*width)...     
-00022bb0: 2020 2062 6720 3a20 666c 6f61 742c 206f     bg : float, o
-00022bc0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00022bd0: 2020 2020 2042 6163 6b67 726f 756e 6420       Background 
-00022be0: 696e 7465 6e73 6974 792e 2049 6620 6e6f  intensity. If no
-00022bf0: 7420 6769 7665 6e2c 2069 7420 7769 6c6c  t given, it will
-00022c00: 2063 616c 6375 6c61 7465 6420 6173 2074   calculated as t
-00022c10: 6865 206d 696e 696d 756d 2076 616c 7565  he minimum value
-00022c20: 206f 6620 0d0a 2020 2020 2020 2020 2020   of ..          
-00022c30: 2020 7468 6520 6f72 6967 696e 616c 2069    the original i
-00022c40: 6d61 6765 2e0d 0a0d 0a20 2020 2020 2020  mage.....       
-00022c50: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00022c60: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00022c70: 2020 2049 6d67 4172 7261 790d 0a20 2020     ImgArray..   
-00022c80: 2020 2020 2020 2020 2050 6164 6465 6420           Padded 
-00022c90: 696d 6167 652e 0d0a 2020 2020 2020 2020  image...        
-00022ca0: 2020 2020 0d0a 2020 2020 2020 2020 4578      ..        Ex
-00022cb0: 616d 706c 6573 0d0a 2020 2020 2020 2020  amples..        
-00022cc0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00022cd0: 2020 6465 7074 6820 3d20 320d 0a20 2020    depth = 2..   
-00022ce0: 2020 2020 200d 0a20 2020 2020 2020 202e       ..        .
-00022cf0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 0d0a  . code-block::..
-00022d00: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00022d10: 2020 2020 2020 2d2d 2d2d 7c20 2020 7c2d        ----|   |-
-00022d20: 2d2d 2d7c 206f 207c 2d2d 2020 2020 206f  ---| o |--     o
-00022d30: 202e 2e2e 2063 656e 7465 7220 6f66 206b   ... center of k
-00022d40: 6572 6e65 6c0d 0a20 2020 2020 2020 2020  ernel..         
-00022d50: 2020 202d 2d2d 2d7c 206f 207c 2d2d 2d2d     ----| o |----
-00022d60: 7c20 2020 7c2d 2d0d 0a20 2020 2020 2020  |   |--..       
-00022d70: 2020 2020 202b 2b2b 2b7c 2020 207c 2b2b       ++++|   |++
-00022d80: 2b2b 7c5f 5f5f 7c2b 2b20 203c 2d20 7468  ++|___|++  <- th
-00022d90: 6520 7570 7065 7220 6564 6765 206f 6620  e upper edge of 
-00022da0: 6f72 6967 696e 616c 2069 6d61 6765 200d  original image .
-00022db0: 0a20 2020 2020 2020 2020 2020 202b 2b2b  .            +++
-00022dc0: 2b7c 5f5f 5f7c 2b2b 2b2b 2b2b 2b2b 2b2b  +|___|++++++++++
-00022dd0: 2b0d 0a0d 0a20 2020 2020 2020 2022 2222  +....        """
-00022de0: 0d0a 2020 2020 2020 2020 6267 203d 205f  ..        bg = _
-00022df0: 6368 6563 6b5f 6267 2873 656c 662c 2062  check_bg(self, b
-00022e00: 6729 0d0a 2020 2020 2020 2020 0d0a 2020  g)..        ..  
-00022e10: 2020 2020 2020 6966 206e 702e 6973 7363        if np.issc
-00022e20: 616c 6172 286b 6572 6e65 6c29 3a0d 0a20  alar(kernel):.. 
-00022e30: 2020 2020 2020 2020 2020 206b 6572 6e65             kerne
-00022e40: 6c20 3d20 6e70 2e61 7272 6179 285b 6b65  l = np.array([ke
-00022e50: 726e 656c 5d2a 3329 0d0a 2020 2020 2020  rnel]*3)..      
-00022e60: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00022e70: 2020 2020 206b 6572 6e65 6c20 3d20 6e70       kernel = np
-00022e80: 2e61 7361 7272 6179 286b 6572 6e65 6c29  .asarray(kernel)
-00022e90: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00022ea0: 2020 2020 6966 206b 6572 6e65 6c2e 6e64      if kernel.nd
-00022eb0: 696d 203c 3d20 313a 0d0a 2020 2020 2020  im <= 1:..      
-00022ec0: 2020 2020 2020 6465 6620 6669 6c74 6572        def filter
-00022ed0: 5f66 756e 6328 696d 6729 3a0d 0a20 2020  _func(img):..   
-00022ee0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00022ef0: 7572 6e20 7870 2e61 736e 756d 7079 285f  urn xp.asnumpy(_
-00022f00: 6669 6c74 6572 732e 6761 7573 7369 616e  filters.gaussian
-00022f10: 5f66 696c 7465 7228 696d 672c 206b 6572  _filter(img, ker
-00022f20: 6e65 6c2c 206d 6f64 653d 2263 6f6e 7374  nel, mode="const
-00022f30: 616e 7422 2c20 6376 616c 3d62 6729 290d  ant", cval=bg)).
-00022f40: 0a20 2020 2020 2020 2020 2020 2064 7a2c  .            dz,
-00022f50: 2064 792c 2064 7820 3d20 6b65 726e 656c   dy, dx = kernel
-00022f60: 2a33 2023 2033 2d73 6967 6d61 0d0a 2020  *3 # 3-sigma..  
-00022f70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00022f80: 2020 2020 656c 6966 206b 6572 6e65 6c2e      elif kernel.
-00022f90: 6e64 696d 203d 3d20 333a 0d0a 2020 2020  ndim == 3:..    
-00022fa0: 2020 2020 2020 2020 6b65 726e 656c 203d          kernel =
-00022fb0: 206b 6572 6e65 6c2e 6173 7479 7065 286e   kernel.astype(n
-00022fc0: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-00022fd0: 2020 2020 2020 2020 6b65 726e 656c 203d          kernel =
-00022fe0: 206b 6572 6e65 6c20 2f20 6e70 2e73 756d   kernel / np.sum
-00022ff0: 286b 6572 6e65 6c29 0d0a 2020 2020 2020  (kernel)..      
-00023000: 2020 2020 2020 6465 6620 6669 6c74 6572        def filter
-00023010: 5f66 756e 6328 696d 6729 3a0d 0a20 2020  _func(img):..   
-00023020: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00023030: 7572 6e20 7870 2e61 736e 756d 7079 285f  urn xp.asnumpy(_
-00023040: 6669 6c74 6572 732e 636f 6e76 6f6c 7665  filters.convolve
-00023050: 2869 6d67 2c20 6b65 726e 656c 2c20 6d6f  (img, kernel, mo
-00023060: 6465 3d22 636f 6e73 7461 6e74 222c 2063  de="constant", c
-00023070: 7661 6c3d 6267 2929 0d0a 2020 2020 2020  val=bg))..      
-00023080: 2020 2020 2020 647a 2c20 6479 2c20 6478        dz, dy, dx
-00023090: 203d 206e 702e 6172 7261 7928 6b65 726e   = np.array(kern
-000230a0: 656c 2e73 6861 7065 292f 2f32 0d0a 2020  el.shape)//2..  
-000230b0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000230c0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000230d0: 616c 7565 4572 726f 7228 2260 6b65 726e  alueError("`kern
-000230e0: 656c 6020 6f6e 6c79 2074 616b 6520 302c  el` only take 0,
-000230f0: 2031 2c20 3320 6469 6d65 6e73 696f 6e61   1, 3 dimensiona
-00023100: 6c20 6172 7261 7920 6173 2061 6e20 696e  l array as an in
-00023110: 7075 742e 2229 0d0a 2020 2020 2020 2020  put.")..        
-00023120: 0d0a 2020 2020 2020 2020 7061 645f 7769  ..        pad_wi
-00023130: 6474 6820 3d20 5b28 6465 7074 682c 2064  dth = [(depth, d
-00023140: 6570 7468 292c 2028 7769 6474 682c 2077  epth), (width, w
-00023150: 6964 7468 292c 2028 7769 6474 682c 2077  idth), (width, w
-00023160: 6964 7468 295d 0d0a 2020 2020 2020 2020  idth)]..        
-00023170: 7061 6469 6d67 203d 2073 656c 662e 7061  padimg = self.pa
-00023180: 6428 7061 645f 7769 6474 682c 206d 6f64  d(pad_width, mod
-00023190: 653d 2263 6f6e 7374 616e 7422 2c20 636f  e="constant", co
-000231a0: 6e73 7461 6e74 5f76 616c 7565 733d 6267  nstant_values=bg
-000231b0: 2c20 6469 6d73 3d22 7a79 7822 290d 0a20  , dims="zyx").. 
-000231c0: 2020 2020 2020 206f 7574 203d 206e 702e         out = np.
-000231d0: 636f 7079 2870 6164 696d 672e 7661 6c75  copy(padimg.valu
-000231e0: 6529 0d0a 2020 2020 2020 2020 2320 636f  e)..        # co
-000231f0: 6e76 6f6c 7665 2070 7366 0d0a 2020 2020  nvolve psf..    
-00023200: 2020 2020 7a5f 6564 6765 3020 3d20 736c      z_edge0 = sl
-00023210: 6963 6528 4e6f 6e65 2c20 6465 7074 682c  ice(None, depth,
-00023220: 204e 6f6e 6529 0d0a 2020 2020 2020 2020   None)..        
-00023230: 7a5f 6d69 6420 3d20 736c 6963 6528 6465  z_mid = slice(de
-00023240: 7074 682c 202d 6465 7074 682c 204e 6f6e  pth, -depth, Non
-00023250: 6529 0d0a 2020 2020 2020 2020 7a5f 6564  e)..        z_ed
-00023260: 6765 3120 3d20 736c 6963 6528 2d64 6570  ge1 = slice(-dep
-00023270: 7468 2c20 4e6f 6e65 2c20 4e6f 6e65 290d  th, None, None).
-00023280: 0a20 2020 2020 2020 2079 5f65 6467 6530  .        y_edge0
-00023290: 203d 2078 5f65 6467 6530 203d 2073 6c69   = x_edge0 = sli
-000232a0: 6365 284e 6f6e 652c 2077 6964 7468 2c20  ce(None, width, 
-000232b0: 4e6f 6e65 290d 0a20 2020 2020 2020 2079  None)..        y
-000232c0: 5f6d 6964 203d 2073 6c69 6365 2877 6964  _mid = slice(wid
-000232d0: 7468 2c20 2d77 6964 7468 2c20 4e6f 6e65  th, -width, None
-000232e0: 290d 0a20 2020 2020 2020 2079 5f65 6467  )..        y_edg
-000232f0: 6531 203d 2078 5f65 6467 6531 203d 2073  e1 = x_edge1 = s
-00023300: 6c69 6365 282d 7769 6474 682c 204e 6f6e  lice(-width, Non
-00023310: 652c 204e 6f6e 6529 0d0a 2020 2020 2020  e, None)..      
-00023320: 2020 0d0a 2020 2020 2020 2020 666f 7220    ..        for 
-00023330: 736c 2c20 696d 6720 696e 2070 6164 696d  sl, img in padim
-00023340: 672e 6974 6572 2863 6f6d 706c 656d 656e  g.iter(complemen
-00023350: 745f 6178 6573 2822 7a79 7822 2c20 7365  t_axes("zyx", se
-00023360: 6c66 2e61 7865 7329 293a 0d0a 2020 2020  lf.axes)):..    
-00023370: 2020 2020 2020 2020 6f75 745f 203d 206f          out_ = o
-00023380: 7574 5b73 6c5d 0d0a 2020 2020 2020 2020  ut[sl]..        
-00023390: 2020 2020 6f75 745f 5b7a 5f65 6467 6530      out_[z_edge0
-000233a0: 5d20 3d20 6669 6c74 6572 5f66 756e 6328  ] = filter_func(
-000233b0: 696d 675b 3a64 6570 7468 2b64 7a20 5d29  img[:depth+dz ])
-000233c0: 5b7a 5f65 6467 6530 5d0d 0a20 2020 2020  [z_edge0]..     
-000233d0: 2020 2020 2020 206f 7574 5f5b 7a5f 6564         out_[z_ed
-000233e0: 6765 315d 203d 2066 696c 7465 725f 6675  ge1] = filter_fu
-000233f0: 6e63 2869 6d67 5b2d 6465 7074 682d 647a  nc(img[-depth-dz
-00023400: 3a5d 295b 7a5f 6564 6765 315d 0d0a 2020  :])[z_edge1]..  
-00023410: 2020 2020 2020 2020 2020 6f75 745f 5b7a            out_[z
-00023420: 5f6d 6964 2c20 795f 6564 6765 305d 203d  _mid, y_edge0] =
-00023430: 2066 696c 7465 725f 6675 6e63 2869 6d67   filter_func(img
-00023440: 5b3a 2c20 3a77 6964 7468 2b64 7920 5d29  [:, :width+dy ])
-00023450: 5b7a 5f6d 6964 2c20 795f 6564 6765 305d  [z_mid, y_edge0]
-00023460: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
-00023470: 745f 5b7a 5f6d 6964 2c20 795f 6564 6765  t_[z_mid, y_edge
-00023480: 315d 203d 2066 696c 7465 725f 6675 6e63  1] = filter_func
-00023490: 2869 6d67 5b3a 2c20 2d77 6964 7468 2d64  (img[:, -width-d
-000234a0: 793a 5d29 5b7a 5f6d 6964 2c20 795f 6564  y:])[z_mid, y_ed
-000234b0: 6765 315d 0d0a 2020 2020 2020 2020 2020  ge1]..          
-000234c0: 2020 6f75 745f 5b7a 5f6d 6964 2c20 795f    out_[z_mid, y_
-000234d0: 6d69 642c 2078 5f65 6467 6530 5d20 3d20  mid, x_edge0] = 
-000234e0: 6669 6c74 6572 5f66 756e 6328 696d 675b  filter_func(img[
-000234f0: 3a2c 203a 2c20 3a77 6964 7468 2b64 7820  :, :, :width+dx 
-00023500: 5d29 5b7a 5f6d 6964 2c20 795f 6d69 642c  ])[z_mid, y_mid,
-00023510: 2078 5f65 6467 6530 5d0d 0a20 2020 2020   x_edge0]..     
-00023520: 2020 2020 2020 206f 7574 5f5b 7a5f 6d69         out_[z_mi
-00023530: 642c 2079 5f6d 6964 2c20 785f 6564 6765  d, y_mid, x_edge
-00023540: 315d 203d 2066 696c 7465 725f 6675 6e63  1] = filter_func
-00023550: 2869 6d67 5b3a 2c20 3a2c 202d 7769 6474  (img[:, :, -widt
-00023560: 682d 6478 3a5d 295b 7a5f 6d69 642c 2079  h-dx:])[z_mid, y
-00023570: 5f6d 6964 2c20 785f 6564 6765 315d 0d0a  _mid, x_edge1]..
-00023580: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00023590: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-000235a0: 2e76 6965 7728 7365 6c66 2e5f 5f63 6c61  .view(self.__cla
-000235b0: 7373 5f5f 290d 0a20 2020 200d 0a20 2020  ss__)..    ..   
-000235c0: 200d 0a20 2020 2040 5f64 6f63 732e 7772   ..    @_docs.wr
-000235d0: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
-000235e0: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
-000235f0: 7865 730d 0a20 2020 2040 7361 6d65 5f64  xes..    @same_d
-00023600: 7479 7065 2861 7366 6c6f 6174 3d54 7275  type(asfloat=Tru
-00023610: 6529 0d0a 2020 2020 4063 6865 636b 5f69  e)..    @check_i
-00023620: 6e70 7574 5f61 6e64 5f6f 7574 7075 740d  nput_and_output.
-00023630: 0a20 2020 2064 6566 2077 6965 6e65 7228  .    def wiener(
-00023640: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
-00023650: 0a20 2020 2020 2020 2070 7366 3a20 6e70  .        psf: np
-00023660: 2e6e 6461 7272 6179 207c 2043 616c 6c61  .ndarray | Calla
-00023670: 626c 655b 5b74 7570 6c65 5b69 6e74 2c20  ble[[tuple[int, 
-00023680: 2e2e 2e5d 5d2c 206e 702e 6e64 6172 7261  ...]], np.ndarra
-00023690: 795d 2c0d 0a20 2020 2020 2020 206c 6d64  y],..        lmd
-000236a0: 3a20 666c 6f61 7420 3d20 302e 312c 0d0a  : float = 0.1,..
-000236b0: 2020 2020 2020 2020 2a2c 200d 0a20 2020          *, ..   
-000236c0: 2020 2020 2064 696d 733a 2044 696d 7320       dims: Dims 
-000236d0: 3d20 4e6f 6e65 2c20 0d0a 2020 2020 2020  = None, ..      
-000236e0: 2020 7570 6461 7465 3a20 626f 6f6c 203d    update: bool =
-000236f0: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
-00023700: 2049 6d67 4172 7261 793a 0d0a 2020 2020   ImgArray:..    
-00023710: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
-00023720: 2020 436c 6173 7369 6361 6c20 7769 656e    Classical wien
-00023730: 6572 2064 6563 6f6e 766f 6c75 7469 6f6e  er deconvolution
-00023740: 2e20 5468 6973 2061 6c67 6f72 6974 686d  . This algorithm
-00023750: 2068 6173 2074 6865 2073 6572 696f 7573   has the serious
-00023760: 2072 696e 6769 6e67 2070 726f 626c 656d   ringing problem
-00023770: 0d0a 2020 2020 2020 2020 6966 2070 6172  ..        if par
-00023780: 616d 6574 6572 7320 6172 6520 7365 7420  ameters are set 
-00023790: 746f 2077 726f 6e67 2076 616c 7565 732e  to wrong values.
-000237a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000237b0: 2020 2020 3a6d 6174 683a 6046 5b59 5f7b      :math:`F[Y_{
-000237c0: 7265 737d 5d20 3d20 5c66 7261 637b 465b  res}] = \frac{F[
-000237d0: 595f 7b6f 6273 7d5d 205c 6364 6f74 205c  Y_{obs}] \cdot \
-000237e0: 6261 727b 487d 7d7b 7c48 7c5e 3220 2b20  bar{H}}{|H|^2 + 
-000237f0: 5c6c 616d 6264 617d 600d 0a20 2020 2020  \lambda}`..     
-00023800: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00023810: 203a 6d61 7468 3a60 595f 7b6f 6273 7d60   :math:`Y_{obs}`
-00023820: 3a20 6f62 7365 7276 6564 2069 6d61 6765  : observed image
-00023830: 3b0d 0a20 2020 2020 2020 203a 6d61 7468  ;..        :math
-00023840: 3a60 595f 7b72 6573 7d60 3a20 7265 7374  :`Y_{res}`: rest
-00023850: 6f72 6564 2069 6d61 6765 3b0d 0a20 2020  ored image;..   
-00023860: 2020 2020 203a 6d61 7468 3a60 4860 203a       :math:`H` :
-00023870: 2046 4654 206f 6620 706f 696e 7420 7370   FFT of point sp
-00023880: 7265 6164 2066 756e 6374 696f 6e20 2850  read function (P
-00023890: 5346 293b 0d0a 0d0a 2020 2020 2020 2020  SF);....        
-000238a0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-000238b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-000238c0: 2020 2020 2020 2020 7073 6620 3a20 6e64          psf : nd
-000238d0: 6172 7261 7920 6f72 2063 616c 6c61 626c  array or callabl
-000238e0: 650d 0a20 2020 2020 2020 2020 2020 2050  e..            P
-000238f0: 6f69 6e74 2073 7072 6561 6420 6675 6e63  oint spread func
-00023900: 7469 6f6e 2e20 4966 2061 2066 756e 6374  tion. If a funct
-00023910: 696f 6e20 6973 2067 6976 656e 2c20 6070  ion is given, `p
-00023920: 7366 2873 6861 7065 2960 2077 696c 6c20  sf(shape)` will 
-00023930: 6265 0d0a 2020 2020 2020 2020 2020 2020  be..            
-00023940: 6361 6c6c 6564 2074 6f20 6765 6e65 7261  called to genera
-00023950: 7465 2074 6865 2050 5346 2e0d 0a20 2020  te the PSF...   
-00023960: 2020 2020 206c 6d64 203a 2066 6c6f 6174       lmd : float
-00023970: 2c20 6465 6661 756c 7420 6973 2030 2e31  , default is 0.1
-00023980: 0d0a 2020 2020 2020 2020 2020 2020 436f  ..            Co
-00023990: 6e73 7461 6e74 2076 616c 7565 2075 7365  nstant value use
-000239a0: 6420 696e 2074 6865 2064 6563 6f6e 766f  d in the deconvo
-000239b0: 6c75 7469 6f6e 2e20 5365 6520 466f 726d  lution. See Form
-000239c0: 756c 6174 696f 6e20 6265 6c6f 772e 0d0a  ulation below...
-000239d0: 2020 2020 2020 2020 7b64 696d 737d 7b75          {dims}{u
-000239e0: 7064 6174 657d 0d0a 0d0a 2020 2020 2020  pdate}....      
-000239f0: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-00023a00: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-00023a10: 2020 2020 496d 6741 7272 6179 0d0a 2020      ImgArray..  
-00023a20: 2020 2020 2020 2020 2020 4465 636f 6e76            Deconv
-00023a30: 6f6c 7665 6420 696d 6167 652e 0d0a 2020  olved image...  
-00023a40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00023a50: 0d0a 2020 2020 2020 2020 5365 6520 416c  ..        See Al
-00023a60: 736f 0d0a 2020 2020 2020 2020 2d2d 2d2d  so..        ----
-00023a70: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6c75  ----..        lu
-00023a80: 6379 0d0a 2020 2020 2020 2020 6c75 6379  cy..        lucy
-00023a90: 5f74 760d 0a20 2020 2020 2020 2022 2222  _tv..        """
-00023aa0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00023ab0: 2020 6966 206c 6d64 203c 3d20 303a 0d0a    if lmd <= 0:..
-00023ac0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00023ad0: 6520 5661 6c75 6545 7272 6f72 2866 226c  e ValueError(f"l
-00023ae0: 6d64 206d 7573 7420 6265 2070 6f73 6974  md must be posit
-00023af0: 6976 652c 2062 7574 2067 6f74 3a20 7b6c  ive, but got: {l
-00023b00: 6d64 7d22 290d 0a20 2020 2020 2020 200d  md}")..        .
-00023b10: 0a20 2020 2020 2020 2070 7366 5f66 742c  .        psf_ft,
-00023b20: 2070 7366 5f66 745f 636f 6e6a 203d 205f   psf_ft_conj = _
-00023b30: 6465 636f 6e76 2e63 6865 636b 5f70 7366  deconv.check_psf
-00023b40: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00023b50: 656c 662e 7369 7a65 736f 6628 6469 6d73  elf.sizesof(dims
-00023b60: 292c 2074 7570 6c65 2873 656c 662e 7363  ), tuple(self.sc
-00023b70: 616c 655b 6178 6973 5d20 666f 7220 6178  ale[axis] for ax
-00023b80: 6973 2069 6e20 6469 6d73 292c 2070 7366  is in dims), psf
-00023b90: 2c0d 0a20 2020 2020 2020 2029 0d0a 2020  ,..        )..  
-00023ba0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00023bb0: 7265 7475 726e 2073 656c 662e 5f61 7070  return self._app
-00023bc0: 6c79 5f64 6173 6b28 0d0a 2020 2020 2020  ly_dask(..      
-00023bd0: 2020 2020 2020 5f64 6563 6f6e 762e 7769        _deconv.wi
-00023be0: 656e 6572 2c20 0d0a 2020 2020 2020 2020  ener, ..        
-00023bf0: 2020 2020 635f 6178 6573 3d63 6f6d 706c      c_axes=compl
-00023c00: 656d 656e 745f 6178 6573 2864 696d 732c  ement_axes(dims,
-00023c10: 2073 656c 662e 6178 6573 292c 0d0a 2020   self.axes),..  
-00023c20: 2020 2020 2020 2020 2020 6172 6773 3d28            args=(
-00023c30: 7073 665f 6674 2c20 7073 665f 6674 5f63  psf_ft, psf_ft_c
-00023c40: 6f6e 6a2c 206c 6d64 290d 0a20 2020 2020  onj, lmd)..     
-00023c50: 2020 2029 2020 2020 0d0a 0d0a 2020 2020     )    ....    
-00023c60: 405f 646f 6373 2e77 7269 7465 5f64 6f63  @_docs.write_doc
-00023c70: 730d 0a20 2020 2040 6469 6d73 5f74 6f5f  s..    @dims_to_
-00023c80: 7370 6174 6961 6c5f 6178 6573 0d0a 2020  spatial_axes..  
-00023c90: 2020 4073 616d 655f 6474 7970 6528 6173    @same_dtype(as
-00023ca0: 666c 6f61 743d 5472 7565 290d 0a20 2020  float=True)..   
-00023cb0: 2040 6368 6563 6b5f 696e 7075 745f 616e   @check_input_an
-00023cc0: 645f 6f75 7470 7574 0d0a 2020 2020 6465  d_output..    de
-00023cd0: 6620 6c75 6379 280d 0a20 2020 2020 2020  f lucy(..       
-00023ce0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00023cf0: 7073 663a 206e 702e 6e64 6172 7261 7920  psf: np.ndarray 
-00023d00: 7c20 4361 6c6c 6162 6c65 5b5b 7475 706c  | Callable[[tupl
-00023d10: 655b 696e 742c 202e 2e2e 5d5d 2c20 6e70  e[int, ...]], np
-00023d20: 2e6e 6461 7272 6179 5d2c 0d0a 2020 2020  .ndarray],..    
-00023d30: 2020 2020 6e69 7465 723a 2069 6e74 203d      niter: int =
-00023d40: 2035 302c 0d0a 2020 2020 2020 2020 6570   50,..        ep
-00023d50: 733a 2066 6c6f 6174 203d 2031 652d 352c  s: float = 1e-5,
-00023d60: 0d0a 2020 2020 2020 2020 2a2c 200d 0a20  ..        *, .. 
-00023d70: 2020 2020 2020 2064 696d 733a 2044 696d         dims: Dim
-00023d80: 7320 3d20 4e6f 6e65 2c20 0d0a 2020 2020  s = None, ..    
-00023d90: 2020 2020 7570 6461 7465 3a20 626f 6f6c      update: bool
-00023da0: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
-00023db0: 2d3e 2049 6d67 4172 7261 793a 0d0a 2020  -> ImgArray:..  
-00023dc0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00023dd0: 2020 2044 6563 6f6e 766f 6c75 7469 6f6e     Deconvolution
-00023de0: 206f 6620 4e2d 6469 6d65 6e73 696f 6e61   of N-dimensiona
-00023df0: 6c20 696d 6167 652c 2075 7369 6e67 2052  l image, using R
-00023e00: 6963 6861 7264 736f 6e2d 4c75 6379 2773  ichardson-Lucy's
-00023e10: 2061 6c67 6f72 6974 686d 2e0d 0a20 2020   algorithm...   
-00023e20: 2020 2020 200d 0a20 2020 2020 2020 2050       ..        P
-00023e30: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00023e40: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00023e50: 2020 2020 2020 2070 7366 203a 206e 6461         psf : nda
-00023e60: 7272 6179 206f 7220 6361 6c6c 6162 6c65  rray or callable
-00023e70: 0d0a 2020 2020 2020 2020 2020 2020 506f  ..            Po
-00023e80: 696e 7420 7370 7265 6164 2066 756e 6374  int spread funct
-00023e90: 696f 6e2e 2049 6620 6120 6675 6e63 7469  ion. If a functi
-00023ea0: 6f6e 2069 7320 6769 7665 6e2c 2060 7073  on is given, `ps
-00023eb0: 6628 7368 6170 6529 6020 7769 6c6c 2062  f(shape)` will b
-00023ec0: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-00023ed0: 616c 6c65 6420 746f 2067 656e 6572 6174  alled to generat
-00023ee0: 6520 7468 6520 5053 462e 0d0a 2020 2020  e the PSF...    
-00023ef0: 2020 2020 6e69 7465 7220 3a20 696e 742c      niter : int,
-00023f00: 2064 6566 6175 6c74 2069 7320 3530 2e0d   default is 50..
-00023f10: 0a20 2020 2020 2020 2020 2020 204e 756d  .            Num
-00023f20: 6265 7220 6f66 2069 7465 7261 7469 6f6e  ber of iteration
-00023f30: 732e 0d0a 2020 2020 2020 2020 6570 7320  s...        eps 
-00023f40: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-00023f50: 2069 7320 3165 2d35 0d0a 2020 2020 2020   is 1e-5..      
-00023f60: 2020 2020 2020 4475 7269 6e67 2064 6563        During dec
-00023f70: 6f6e 766f 6c75 7469 6f6e 2c20 6469 7669  onvolution, divi
-00023f80: 7369 6f6e 2062 7920 736d 616c 6c20 7661  sion by small va
-00023f90: 6c75 6573 2069 6e20 7468 6520 636f 6e76  lues in the conv
-00023fa0: 6f6c 7665 2069 6d61 6765 200d 0a20 2020  olve image ..   
-00023fb0: 2020 2020 2020 2020 206f 6620 6573 7469           of esti
-00023fc0: 6d61 7469 6f6e 2061 6e64 2050 5346 206d  mation and PSF m
-00023fd0: 6179 2063 6175 7365 2064 6976 6572 6765  ay cause diverge
-00023fe0: 6e63 652e 2054 6865 7265 666f 7265 2c20  nce. Therefore, 
-00023ff0: 6469 7669 7369 6f6e 2062 7920 0d0a 2020  division by ..  
-00024000: 2020 2020 2020 2020 2020 7661 6c75 6573            values
-00024010: 2075 6e64 6572 2060 6570 7360 2069 7320   under `eps` is 
-00024020: 7375 6273 7469 7475 7465 6420 746f 207a  substituted to z
-00024030: 6572 6f2e 0d0a 2020 2020 2020 2020 7b64  ero...        {d
-00024040: 696d 737d 7b75 7064 6174 657d 0d0a 2020  ims}{update}..  
-00024050: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00024060: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-00024070: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-00024080: 2020 496d 6741 7272 6179 0d0a 2020 2020    ImgArray..    
-00024090: 2020 2020 2020 2020 4465 636f 6e76 6f6c          Deconvol
-000240a0: 7665 6420 696d 6167 652e 0d0a 2020 2020  ved image...    
-000240b0: 2020 2020 0d0a 2020 2020 2020 2020 5365      ..        Se
-000240c0: 6520 416c 736f 0d0a 2020 2020 2020 2020  e Also..        
-000240d0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-000240e0: 2020 6c75 6379 5f74 760d 0a20 2020 2020    lucy_tv..     
-000240f0: 2020 2077 6965 6e65 720d 0a20 2020 2020     wiener..     
-00024100: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00024110: 0d0a 2020 2020 2020 2020 7073 665f 6674  ..        psf_ft
-00024120: 2c20 7073 665f 6674 5f63 6f6e 6a20 3d20  , psf_ft_conj = 
-00024130: 5f64 6563 6f6e 762e 6368 6563 6b5f 7073  _deconv.check_ps
-00024140: 6628 0d0a 2020 2020 2020 2020 2020 2020  f(..            
-00024150: 7365 6c66 2e73 697a 6573 6f66 2864 696d  self.sizesof(dim
-00024160: 7329 2c20 7475 706c 6528 7365 6c66 2e73  s), tuple(self.s
-00024170: 6361 6c65 5b61 7869 735d 2066 6f72 2061  cale[axis] for a
-00024180: 7869 7320 696e 2064 696d 7329 2c20 7073  xis in dims), ps
-00024190: 662c 0d0a 2020 2020 2020 2020 290d 0a0d  f,..        )...
-000241a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000241b0: 7365 6c66 2e5f 6170 706c 795f 6461 736b  self._apply_dask
-000241c0: 280d 0a20 2020 2020 2020 2020 2020 205f  (..            _
-000241d0: 6465 636f 6e76 2e72 6963 6861 7264 736f  deconv.richardso
-000241e0: 6e5f 6c75 6379 2c20 0d0a 2020 2020 2020  n_lucy, ..      
-000241f0: 2020 2020 2020 635f 6178 6573 3d63 6f6d        c_axes=com
-00024200: 706c 656d 656e 745f 6178 6573 2864 696d  plement_axes(dim
-00024210: 732c 2073 656c 662e 6178 6573 292c 0d0a  s, self.axes),..
-00024220: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00024230: 3d28 7073 665f 6674 2c20 7073 665f 6674  =(psf_ft, psf_ft
-00024240: 5f63 6f6e 6a2c 206e 6974 6572 2c20 6570  _conj, niter, ep
-00024250: 7329 0d0a 2020 2020 2020 2020 290d 0a20  s)..        ).. 
-00024260: 2020 2020 2020 200d 0a20 2020 2040 5f64         ..    @_d
-00024270: 6f63 732e 7772 6974 655f 646f 6373 0d0a  ocs.write_docs..
-00024280: 2020 2020 4064 696d 735f 746f 5f73 7061      @dims_to_spa
-00024290: 7469 616c 5f61 7865 730d 0a20 2020 2040  tial_axes..    @
-000242a0: 7361 6d65 5f64 7479 7065 2861 7366 6c6f  same_dtype(asflo
-000242b0: 6174 3d54 7275 6529 0d0a 2020 2020 4063  at=True)..    @c
-000242c0: 6865 636b 5f69 6e70 7574 5f61 6e64 5f6f  heck_input_and_o
-000242d0: 7574 7075 740d 0a20 2020 2064 6566 206c  utput..    def l
-000242e0: 7563 795f 7476 280d 0a20 2020 2020 2020  ucy_tv(..       
-000242f0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00024300: 7073 663a 206e 702e 6e64 6172 7261 7920  psf: np.ndarray 
-00024310: 7c20 4361 6c6c 6162 6c65 5b5b 7475 706c  | Callable[[tupl
-00024320: 655b 696e 742c 202e 2e2e 5d5d 2c20 6e70  e[int, ...]], np
-00024330: 2e6e 6461 7272 6179 5d2c 0d0a 2020 2020  .ndarray],..    
-00024340: 2020 2020 6d61 785f 6974 6572 3a20 696e      max_iter: in
-00024350: 7420 3d20 3530 2c0d 0a20 2020 2020 2020  t = 50,..       
-00024360: 206c 6d64 3a20 666c 6f61 7420 3d20 3165   lmd: float = 1e
-00024370: 2d33 2c0d 0a20 2020 2020 2020 2074 6f6c  -3,..        tol
-00024380: 3a20 666c 6f61 7420 3d20 3165 2d33 2c0d  : float = 1e-3,.
-00024390: 0a20 2020 2020 2020 2065 7073 3a20 666c  .        eps: fl
-000243a0: 6f61 7420 3d20 3165 2d35 2c0d 0a20 2020  oat = 1e-5,..   
-000243b0: 2020 2020 202a 2c0d 0a20 2020 2020 2020       *,..       
-000243c0: 2064 696d 733a 2044 696d 7320 3d20 4e6f   dims: Dims = No
-000243d0: 6e65 2c0d 0a20 2020 2020 2020 2075 7064  ne,..        upd
-000243e0: 6174 653a 2062 6f6f 6c20 3d20 4661 6c73  ate: bool = Fals
-000243f0: 650d 0a20 2020 2029 202d 3e20 496d 6741  e..    ) -> ImgA
-00024400: 7272 6179 3a0d 0a20 2020 2020 2020 2072  rray:..        r
-00024410: 2222 220d 0a20 2020 2020 2020 2044 6563  """..        Dec
-00024420: 6f6e 766f 6c75 7469 6f6e 206f 6620 4e2d  onvolution of N-
-00024430: 6469 6d65 6e73 696f 6e61 6c20 696d 6167  dimensional imag
-00024440: 652c 2075 7369 6e67 2052 6963 6861 7264  e, using Richard
-00024450: 736f 6e2d 4c75 6379 2773 2061 6c67 6f72  son-Lucy's algor
-00024460: 6974 686d 2077 6974 680d 0a20 2020 2020  ithm with..     
-00024470: 2020 2074 6f74 616c 2076 6172 6961 6e63     total varianc
-00024480: 6520 7265 6775 6c61 7269 7a61 7469 6f6e  e regularization
-00024490: 2028 736f 2063 616c 6c65 6420 524c 2d54   (so called RL-T
-000244a0: 5620 616c 676f 7269 7468 6d29 2e20 5468  V algorithm). Th
-000244b0: 6520 5456 2072 6567 756c 6172 697a 6174  e TV regularizat
-000244c0: 696f 6e0d 0a20 2020 2020 2020 2066 6163  ion..        fac
-000244d0: 746f 7220 6174 2070 6978 656c 2070 6f73  tor at pixel pos
-000244e0: 6974 696f 6e20 3a6d 6174 683a 6078 602c  ition :math:`x`,
-000244f0: 203a 6d61 7468 3a60 465f 7b72 6567 7d28   :math:`F_{reg}(
-00024500: 7829 602c 2069 7320 6361 6c63 756c 6174  x)`, is calculat
-00024510: 6564 2061 733a 0d0a 2020 2020 2020 2020  ed as:..        
-00024520: 0d0a 2020 2020 2020 2020 2e2e 206d 6174  ..        .. mat
-00024530: 683a 3a0d 0a20 2020 2020 2020 2020 2020  h::..           
-00024540: 200d 0a20 2020 2020 2020 2020 2020 2046   ..            F
-00024550: 5f7b 7265 677d 2878 2920 3d20 5c66 7261  _{reg}(x) = \fra
-00024560: 637b 317d 7b31 2d5c 6c61 6d62 6461 205c  c{1}{1-\lambda \
-00024570: 6364 6f74 2064 6976 285c 6672 6163 7b67  cdot div(\frac{g
-00024580: 7261 6428 4928 7829 7d7b 7c67 7261 6428  rad(I(x)}{|grad(
-00024590: 4928 7829 297c 7d29 7d0d 0a20 2020 2020  I(x))|})}..     
-000245a0: 2020 200d 0a20 2020 2020 2020 2028 3a6d     ..        (:m
-000245b0: 6174 683a 6049 2878 2960 3a20 696d 6167  ath:`I(x)`: imag
-000245c0: 652c 203a 6d61 7468 3a60 5c6c 616d 6264  e, :math:`\lambd
-000245d0: 6160 3a20 636f 6e73 7461 6e74 290d 0a20  a`: constant).. 
-000245e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000245f0: 2061 6e64 2074 6869 7320 6661 6374 6f72   and this factor
-00024600: 2069 7320 6d75 6c74 6970 6c69 6564 2066   is multiplied f
-00024610: 6f72 2065 7665 7279 2065 7374 696d 6174  or every estimat
-00024620: 696f 6e20 6d61 6465 2069 6e20 6561 6368  ion made in each
-00024630: 2069 7465 7261 7469 6f6e 2e0d 0a20 2020   iteration...   
-00024640: 2020 2020 200d 0a20 2020 2020 2020 2050       ..        P
-00024650: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00024660: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00024670: 2020 2020 2020 2070 7366 203a 206e 6461         psf : nda
-00024680: 7272 6179 206f 7220 6361 6c6c 6162 6c65  rray or callable
-00024690: 0d0a 2020 2020 2020 2020 2020 2020 506f  ..            Po
-000246a0: 696e 7420 7370 7265 6164 2066 756e 6374  int spread funct
-000246b0: 696f 6e2e 2049 6620 6120 6675 6e63 7469  ion. If a functi
-000246c0: 6f6e 2069 7320 6769 7665 6e2c 2060 7073  on is given, `ps
-000246d0: 6628 7368 6170 6529 6020 7769 6c6c 2062  f(shape)` will b
-000246e0: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-000246f0: 616c 6c65 6420 746f 2067 656e 6572 6174  alled to generat
-00024700: 6520 7468 6520 5053 462e 0d0a 2020 2020  e the PSF...    
-00024710: 2020 2020 6d61 785f 6974 6572 203a 2069      max_iter : i
-00024720: 6e74 2c20 6465 6661 756c 7420 6973 2035  nt, default is 5
-00024730: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
-00024740: 4d61 7869 6d75 6d20 6e75 6d62 6572 206f  Maximum number o
-00024750: 6620 6974 6572 6174 696f 6e73 2e0d 0a20  f iterations... 
-00024760: 2020 2020 2020 206c 6d64 203a 2066 6c6f         lmd : flo
-00024770: 6174 2c20 6465 6661 756c 7420 6973 2031  at, default is 1
-00024780: 652d 330d 0a20 2020 2020 2020 2020 2020  e-3..           
-00024790: 2054 6865 2063 6f6e 7374 616e 7420 6c61   The constant la
-000247a0: 6d62 6461 206f 6620 5456 2072 6567 756c  mbda of TV regul
-000247b0: 6172 697a 6174 696f 6e20 6661 6374 6f72  arization factor
-000247c0: 2e0d 0a20 2020 2020 2020 2074 6f6c 203a  ...        tol :
-000247d0: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-000247e0: 6973 2031 652d 330d 0a20 2020 2020 2020  is 1e-3..       
-000247f0: 2020 2020 2049 7465 7261 7469 6f6e 2073       Iteration s
-00024800: 746f 7073 2069 6620 7265 6775 6c61 7269  tops if regulari
-00024810: 7a65 6420 6162 736f 6c75 7465 2073 756d  zed absolute sum
-00024820: 6d61 7469 6f6e 2069 7320 6c6f 7765 7220  mation is lower 
-00024830: 7468 616e 2074 6869 7320 0d0a 2020 2020  than this ..    
-00024840: 2020 2020 2020 2020 7661 6c75 652e 0d0a          value...
-00024850: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00024860: 2020 2020 2020 2020 2020 3a6d 6174 683a            :math:
-00024870: 605c 6672 6163 7b5c 7375 6d5f 7b78 7d7c  `\frac{\sum_{x}|
-00024880: 4927 2878 2920 2d20 4928 7829 7c7d 7b5c  I'(x) - I(x)|}{\
-00024890: 7375 6d5f 7b78 7d7c 4928 7829 7c7d 600d  sum_{x}|I(x)|}`.
-000248a0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-000248b0: 2020 2020 2020 2020 2020 2028 3a6d 6174             (:mat
-000248c0: 683a 6049 2728 7829 603a 2065 7374 696d  h:`I'(x)`: estim
-000248d0: 6174 696f 6e20 6f66 203a 6d61 7468 3a60  ation of :math:`
-000248e0: 6b2b 3160 2d74 6820 6974 6572 6174 696f  k+1`-th iteratio
-000248f0: 6e2c 203a 6d61 7468 3a60 4928 7829 603a  n, :math:`I(x)`:
-00024900: 200d 0a20 2020 2020 2020 2020 2020 2065   ..            e
-00024910: 7374 696d 6174 696f 6e20 6f66 203a 6d61  stimation of :ma
-00024920: 7468 3a60 6b60 2d74 6820 6974 6572 6174  th:`k`-th iterat
-00024930: 696f 6e29 0d0a 2020 2020 2020 2020 0d0a  ion)..        ..
-00024940: 2020 2020 2020 2020 6570 7320 3a20 666c          eps : fl
-00024950: 6f61 742c 2064 6566 6175 6c74 2069 7320  oat, default is 
-00024960: 3165 2d35 0d0a 2020 2020 2020 2020 2020  1e-5..          
-00024970: 2020 4475 7269 6e67 2064 6563 6f6e 766f    During deconvo
-00024980: 6c75 7469 6f6e 2c20 6469 7669 7369 6f6e  lution, division
-00024990: 2062 7920 736d 616c 6c20 7661 6c75 6573   by small values
-000249a0: 2069 6e20 7468 6520 636f 6e76 6f6c 7665   in the convolve
-000249b0: 2069 6d61 6765 206f 660d 0a20 2020 2020   image of..     
-000249c0: 2020 2020 2020 2065 7374 696d 6174 696f         estimatio
-000249d0: 6e20 616e 6420 5053 4620 6d61 7920 6361  n and PSF may ca
-000249e0: 7573 6520 6469 7665 7267 656e 6365 2e20  use divergence. 
-000249f0: 5468 6572 6566 6f72 652c 2064 6976 6973  Therefore, divis
-00024a00: 696f 6e20 6279 2076 616c 7565 7320 0d0a  ion by values ..
-00024a10: 2020 2020 2020 2020 2020 2020 756e 6465              unde
-00024a20: 7220 6060 6570 7360 6020 6973 2073 7562  r ``eps`` is sub
-00024a30: 7374 6974 7574 6564 2074 6f20 7a65 726f  stituted to zero
-00024a40: 2e0d 0a20 2020 2020 2020 207b 6469 6d73  ...        {dims
-00024a50: 7d7b 7570 6461 7465 7d0d 0a20 2020 2020  }{update}..     
-00024a60: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
-00024a70: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-00024a80: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
-00024a90: 6d67 4172 7261 790d 0a20 2020 2020 2020  mgArray..       
-00024aa0: 2020 2020 2044 6563 6f6e 766f 6c76 6564       Deconvolved
-00024ab0: 2069 6d61 6765 2e0d 0a20 2020 2020 2020   image...       
-00024ac0: 200d 0a20 2020 2020 2020 2052 6566 6572   ..        Refer
-00024ad0: 656e 6365 730d 0a20 2020 2020 2020 202d  ences..        -
-00024ae0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00024af0: 2020 202d 2044 6579 2c20 4e2e 2c20 426c     - Dey, N., Bl
-00024b00: 616e 632d 46c3 a972 6175 642c 204c 2e2c  anc-F..raud, L.,
-00024b10: 205a 696d 6d65 722c 2043 2e2c 2052 6f75   Zimmer, C., Rou
-00024b20: 782c 2050 2e2c 204b 616d 2c20 5a2e 2c20  x, P., Kam, Z., 
-00024b30: 4f6c 6976 6f2d 4d61 7269 6e2c 204a 2e20  Olivo-Marin, J. 
-00024b40: 432e 2c20 0d0a 2020 2020 2020 2020 2020  C., ..          
-00024b50: 2620 5a65 7275 6269 612c 204a 2e20 2832  & Zerubia, J. (2
-00024b60: 3030 3429 2e20 3344 206d 6963 726f 7363  004). 3D microsc
-00024b70: 6f70 7920 6465 636f 6e76 6f6c 7574 696f  opy deconvolutio
-00024b80: 6e20 7573 696e 6720 5269 6368 6172 6473  n using Richards
-00024b90: 6f6e 2d4c 7563 7920 616c 676f 7269 7468  on-Lucy algorith
-00024ba0: 6d20 0d0a 2020 2020 2020 2020 2020 7769  m ..          wi
-00024bb0: 7468 2074 6f74 616c 2076 6172 6961 7469  th total variati
-00024bc0: 6f6e 2072 6567 756c 6172 697a 6174 696f  on regularizatio
-00024bd0: 6e20 2844 6f63 746f 7261 6c20 6469 7373  n (Doctoral diss
-00024be0: 6572 7461 7469 6f6e 2c20 494e 5249 4129  ertation, INRIA)
-00024bf0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
-00024c00: 2020 2020 2053 6565 2041 6c73 6f0d 0a20       See Also.. 
-00024c10: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
-00024c20: 0a20 2020 2020 2020 206c 7563 790d 0a20  .        lucy.. 
-00024c30: 2020 2020 2020 2077 6965 6e65 720d 0a20         wiener.. 
-00024c40: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00024c50: 2020 2020 6966 206c 6d64 203c 3d20 303a      if lmd <= 0:
-00024c60: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00024c70: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
-00024c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024c90: 2022 496e 2052 6963 6861 6473 6f6e 2d4c   "In Richadson-L
-00024ca0: 7563 7920 7769 7468 2074 6f74 616c 2d76  ucy with total-v
-00024cb0: 6172 6961 6e63 652d 7265 6775 6c61 7269  ariance-regulari
-00024cc0: 7a61 7469 6f6e 2c20 220d 0a20 2020 2020  zation, "..     
-00024cd0: 2020 2020 2020 2020 2020 2022 7061 7261             "para
-00024ce0: 6d65 7465 7220 606c 6d64 6020 6d75 7374  meter `lmd` must
-00024cf0: 2062 6520 706f 7369 7469 7665 2e22 0d0a   be positive."..
-00024d00: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00024d10: 2020 2020 2020 2070 7366 5f66 742c 2070         psf_ft, p
-00024d20: 7366 5f66 745f 636f 6e6a 203d 205f 6465  sf_ft_conj = _de
-00024d30: 636f 6e76 2e63 6865 636b 5f70 7366 280d  conv.check_psf(.
-00024d40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00024d50: 662e 7369 7a65 736f 6628 6469 6d73 292c  f.sizesof(dims),
-00024d60: 2074 7570 6c65 2873 656c 662e 7363 616c   tuple(self.scal
-00024d70: 655b 6178 6973 5d20 666f 7220 6178 6973  e[axis] for axis
-00024d80: 2069 6e20 6469 6d73 292c 2070 7366 0d0a   in dims), psf..
-00024d90: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00024da0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00024db0: 2e5f 6170 706c 795f 6461 736b 280d 0a20  ._apply_dask(.. 
-00024dc0: 2020 2020 2020 2020 2020 205f 6465 636f             _deco
-00024dd0: 6e76 2e72 6963 6861 7264 736f 6e5f 6c75  nv.richardson_lu
-00024de0: 6379 5f74 762c 200d 0a20 2020 2020 2020  cy_tv, ..       
-00024df0: 2020 2020 2063 5f61 7865 733d 636f 6d70       c_axes=comp
-00024e00: 6c65 6d65 6e74 5f61 7865 7328 6469 6d73  lement_axes(dims
-00024e10: 2c20 7365 6c66 2e61 7865 7329 2c0d 0a20  , self.axes),.. 
-00024e20: 2020 2020 2020 2020 2020 2061 7267 733d             args=
-00024e30: 2870 7366 5f66 742c 2070 7366 5f66 745f  (psf_ft, psf_ft_
-00024e40: 636f 6e6a 2c20 6d61 785f 6974 6572 2c20  conj, max_iter, 
-00024e50: 6c6d 642c 2074 6f6c 2c20 6570 7329 0d0a  lmd, tol, eps)..
-00024e60: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00024e70: 2040 5f64 6f63 732e 7772 6974 655f 646f   @_docs.write_do
-00024e80: 6373 0d0a 2020 2020 4064 696d 735f 746f  cs..    @dims_to
-00024e90: 5f73 7061 7469 616c 5f61 7865 730d 0a20  _spatial_axes.. 
-00024ea0: 2020 2040 7361 6d65 5f64 7479 7065 2861     @same_dtype(a
-00024eb0: 7366 6c6f 6174 3d54 7275 6529 0d0a 2020  sfloat=True)..  
-00024ec0: 2020 4063 6865 636b 5f69 6e70 7574 5f61    @check_input_a
-00024ed0: 6e64 5f6f 7574 7075 740d 0a20 2020 2064  nd_output..    d
-00024ee0: 6566 2074 696c 6564 5f6c 7563 7928 0d0a  ef tiled_lucy(..
-00024ef0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00024f00: 2020 2020 2020 2070 7366 3a20 6e70 2e6e         psf: np.n
-00024f10: 6461 7272 6179 207c 2043 616c 6c61 626c  darray | Callabl
-00024f20: 655b 5b74 7570 6c65 5b69 6e74 2c20 2e2e  e[[tuple[int, ..
-00024f30: 2e5d 5d2c 206e 702e 6e64 6172 7261 795d  .]], np.ndarray]
-00024f40: 2c0d 0a20 2020 2020 2020 206e 6974 6572  ,..        niter
-00024f50: 3a20 696e 7420 3d20 3530 2c0d 0a20 2020  : int = 50,..   
-00024f60: 2020 2020 2065 7073 3a20 666c 6f61 7420       eps: float 
-00024f70: 3d20 3165 2d35 2c0d 0a20 2020 2020 2020  = 1e-5,..       
-00024f80: 2063 6875 6e6b 7320 3d20 2261 7574 6f22   chunks = "auto"
-00024f90: 2c0d 0a20 2020 2020 2020 206f 7665 726c  ,..        overl
-00024fa0: 6170 3a20 696e 7420 3d20 3332 2c0d 0a20  ap: int = 32,.. 
-00024fb0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-00024fc0: 0d0a 2020 2020 2920 2d3e 2049 6d67 4172  ..    ) -> ImgAr
-00024fd0: 7261 793a 0d0a 2020 2020 2020 2020 7761  ray:..        wa
-00024fe0: 726e 696e 6773 2e77 6172 6e28 0d0a 2020  rnings.warn(..  
-00024ff0: 2020 2020 2020 2020 2020 2260 7469 6c65            "`tile
-00025000: 645f 6c75 6379 6020 6973 2064 6570 7265  d_lucy` is depre
-00025010: 6361 7465 6420 506c 6561 7365 2075 7365  cated Please use
-00025020: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00025030: 6622 6069 6d67 2e74 696c 6564 287b 6368  f"`img.tiled({ch
-00025040: 756e 6b73 3d7d 2c20 7b6f 7665 726c 6170  unks=}, {overlap
-00025050: 3d7d 292e 6c75 6379 282e 2e2e 2960 2069  =}).lucy(...)` i
-00025060: 6e73 7465 6164 2e22 2c0d 0a20 2020 2020  nstead.",..     
-00025070: 2020 2020 2020 2044 6570 7265 6361 7469         Deprecati
-00025080: 6f6e 5761 726e 696e 672c 0d0a 2020 2020  onWarning,..    
-00025090: 2020 2020 290d 0a20 2020 2020 2020 2072      )..        r
-000250a0: 6574 7572 6e20 7365 6c66 2e74 696c 6564  eturn self.tiled
-000250b0: 2863 6875 6e6b 732c 206f 7665 726c 6170  (chunks, overlap
-000250c0: 292e 6c75 6379 2870 7366 2c20 6e69 7465  ).lucy(psf, nite
-000250d0: 722c 2065 7073 290d 0a0d 0a64 6566 205f  r, eps)....def _
-000250e0: 6368 6563 6b5f 636f 6f72 6469 6e61 7465  check_coordinate
-000250f0: 7328 636f 6f72 6473 2c20 696d 673a 2049  s(coords, img: I
-00025100: 6d67 4172 7261 792c 2064 696d 733a 2044  mgArray, dims: D
-00025110: 696d 7320 3d20 4e6f 6e65 293a 0d0a 2020  ims = None):..  
-00025120: 2020 6672 6f6d 2069 6d70 792e 6672 616d    from impy.fram
-00025130: 6520 696d 706f 7274 204d 6172 6b65 7246  e import MarkerF
-00025140: 7261 6d65 0d0a 0d0a 2020 2020 6966 206e  rame....    if n
-00025150: 6f74 2069 7369 6e73 7461 6e63 6528 636f  ot isinstance(co
-00025160: 6f72 6473 2c20 4d61 726b 6572 4672 616d  ords, MarkerFram
-00025170: 6529 3a0d 0a20 2020 2020 2020 2063 6f6f  e):..        coo
-00025180: 7264 7320 3d20 6e70 2e61 7361 7272 6179  rds = np.asarray
-00025190: 2863 6f6f 7264 7329 0d0a 2020 2020 2020  (coords)..      
-000251a0: 2020 6966 2063 6f6f 7264 732e 6e64 696d    if coords.ndim
-000251b0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-000251c0: 2020 2020 636f 6f72 6473 203d 2063 6f6f      coords = coo
-000251d0: 7264 732e 7265 7368 6170 6528 312c 202d  rds.reshape(1, -
-000251e0: 3129 0d0a 2020 2020 2020 2020 656c 6966  1)..        elif
-000251f0: 2063 6f6f 7264 732e 6e64 696d 2021 3d20   coords.ndim != 
-00025200: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-00025210: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00025220: 2822 496e 7075 7420 6361 6e6e 6f74 2062  ("Input cannot b
-00025230: 6520 696e 7465 7270 7265 7465 6420 6173  e interpreted as
-00025240: 2063 6f6f 7264 696e 6174 6528 7329 2e22   coordinate(s)."
-00025250: 290d 0a20 2020 2020 2020 2069 6620 6469  )..        if di
-00025260: 6d73 2069 7320 4e6f 6e65 3a0d 0a20 2020  ms is None:..   
-00025270: 2020 2020 2020 2020 206e 6469 6d20 3d20           ndim = 
-00025280: 636f 6f72 6473 2e73 6861 7065 5b31 5d0d  coords.shape[1].
-00025290: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000252a0: 6e64 696d 203d 3d20 696d 672e 6e64 696d  ndim == img.ndim
-000252b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000252c0: 2020 2064 696d 7320 3d20 696d 672e 6178     dims = img.ax
-000252d0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-000252e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000252f0: 2020 2020 2020 2064 696d 7320 3d20 636f         dims = co
-00025300: 6d70 6c65 6d65 6e74 5f61 7865 7328 2263  mplement_axes("c
-00025310: 222c 2069 6d67 2e61 7865 7329 5b2d 6e64  ", img.axes)[-nd
-00025320: 696d 3a5d 0d0a 2020 2020 2020 2020 636f  im:]..        co
-00025330: 6f72 6473 203d 204d 6172 6b65 7246 7261  ords = MarkerFra
-00025340: 6d65 2863 6f6f 7264 732c 2063 6f6c 756d  me(coords, colum
-00025350: 6e73 3d64 696d 732c 2064 7479 7065 3d6e  ns=dims, dtype=n
-00025360: 702e 7569 6e74 3136 290d 0a20 2020 2020  p.uint16)..     
-00025370: 2020 2063 6f6f 7264 732e 7365 745f 7363     coords.set_sc
-00025380: 616c 6528 696d 6729 0d0a 2020 2020 0d0a  ale(img)..    ..
-00025390: 2020 2020 7265 7475 726e 2063 6f6f 7264      return coord
-000253a0: 730d 0a0d 0a64 6566 205f 6368 6563 6b5f  s....def _check_
-000253b0: 6675 6e63 7469 6f6e 2866 756e 6329 3a0d  function(func):.
-000253c0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-000253d0: 6365 2866 756e 632c 2073 7472 293a 0d0a  ce(func, str):..
-000253e0: 2020 2020 2020 2020 6675 6e63 203d 2067          func = g
-000253f0: 6574 6174 7472 286e 702c 2066 756e 632c  etattr(np, func,
-00025400: 204e 6f6e 6529 0d0a 2020 2020 6966 2063   None)..    if c
-00025410: 616c 6c61 626c 6528 6675 6e63 293a 0d0a  allable(func):..
-00025420: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00025430: 756e 630d 0a20 2020 2065 6c73 653a 0d0a  unc..    else:..
-00025440: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00025450: 7065 4572 726f 7228 224d 7573 7420 6265  peError("Must be
-00025460: 206f 6e65 206f 6620 6e75 6d70 7920 6d65   one of numpy me
-00025470: 7468 6f64 7320 6f72 2063 616c 6c61 626c  thods or callabl
-00025480: 6520 6f62 6a65 6374 2e22 290d 0a20 2020  e object.")..   
-00025490: 200d 0a64 6566 205f 6368 6563 6b5f 6267   ..def _check_bg
-000254a0: 2869 6d67 3a20 496d 6741 7272 6179 2c20  (img: ImgArray, 
-000254b0: 6267 293a 0d0a 2020 2020 2320 6465 7465  bg):..    # dete
-000254c0: 726d 696e 6520 6267 0d0a 2020 2020 6966  rmine bg..    if
-000254d0: 2062 6720 6973 204e 6f6e 653a 0d0a 2020   bg is None:..  
-000254e0: 2020 2020 2020 6267 203d 2069 6d67 2e6d        bg = img.m
-000254f0: 696e 2829 0d0a 2020 2020 656c 6966 2069  in()..    elif i
-00025500: 7369 6e73 7461 6e63 6528 6267 2c20 7374  sinstance(bg, st
-00025510: 7229 2061 6e64 2062 672e 656e 6473 7769  r) and bg.endswi
-00025520: 7468 2822 2522 293a 0d0a 2020 2020 2020  th("%"):..      
-00025530: 2020 6267 203d 206e 702e 7065 7263 656e    bg = np.percen
-00025540: 7469 6c65 2869 6d67 2e76 616c 7565 2c20  tile(img.value, 
-00025550: 666c 6f61 7428 6267 5b3a 2d31 5d29 290d  float(bg[:-1])).
-00025560: 0a20 2020 2065 6c69 6620 6e6f 7420 6e70  .    elif not np
-00025570: 2e69 7373 6361 6c61 7228 6267 293a 0d0a  .isscalar(bg):..
-00025580: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00025590: 7065 4572 726f 7228 2257 726f 6e67 2074  peError("Wrong t
-000255a0: 7970 6520 6f66 2060 6267 602e 2229 0d0a  ype of `bg`.")..
-000255b0: 2020 2020 7265 7475 726e 2062 670d 0a0d      return bg...
-000255c0: 0a64 6566 205f 6368 6563 6b5f 7465 6d70  .def _check_temp
-000255d0: 6c61 7465 2874 656d 706c 6174 6529 3a0d  late(template):.
-000255e0: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
-000255f0: 7374 616e 6365 2874 656d 706c 6174 652c  stance(template,
-00025600: 206e 702e 6e64 6172 7261 7929 3a0d 0a20   np.ndarray):.. 
-00025610: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00025620: 6545 7272 6f72 2866 2260 7465 6d70 6c61  eError(f"`templa
-00025630: 7465 6020 6d75 7374 2062 6520 6e70 2e6e  te` must be np.n
-00025640: 6461 7272 6179 2c20 6275 7420 676f 7420  darray, but got 
-00025650: 7b74 7970 6528 7465 6d70 6c61 7465 297d  {type(template)}
-00025660: 2229 0d0a 2020 2020 656c 6966 2074 656d  ")..    elif tem
-00025670: 706c 6174 652e 6e64 696d 206e 6f74 2069  plate.ndim not i
-00025680: 6e20 2832 2c20 3329 3a0d 0a20 2020 2020  n (2, 3):..     
-00025690: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000256a0: 726f 7228 2260 7465 6d70 6c61 7465 206d  ror("`template m
-000256b0: 7573 7420 6265 2032 206f 7220 3320 6469  ust be 2 or 3 di
-000256c0: 6d65 6e73 696f 6e61 6c2e 6022 290d 0a20  mensional.`").. 
-000256d0: 2020 2074 656d 706c 6174 6520 3d20 6e70     template = np
-000256e0: 2e61 7361 7272 6179 2874 656d 706c 6174  .asarray(templat
-000256f0: 6529 2e61 7374 7970 6528 6e70 2e66 6c6f  e).astype(np.flo
-00025700: 6174 3332 2c20 636f 7079 3d54 7275 6529  at32, copy=True)
-00025710: 0d0a 2020 2020 7265 7475 726e 2074 656d  ..    return tem
-00025720: 706c 6174 650d 0a0d 0a64 6566 205f 6361  plate....def _ca
-00025730: 6c63 5f63 656e 7472 6f69 6428 696d 673a  lc_centroid(img:
-00025740: 206e 702e 6e64 6172 7261 792c 206e 6469   np.ndarray, ndi
-00025750: 6d3a 2069 6e74 2920 2d3e 206e 702e 6e64  m: int) -> np.nd
-00025760: 6172 7261 793a 0d0a 2020 2020 6d6f 6d20  array:..    mom 
-00025770: 3d20 736b 6d65 732e 6d6f 6d65 6e74 7328  = skmes.moments(
-00025780: 696d 672c 206f 7264 6572 3d31 290d 0a20  img, order=1).. 
-00025790: 2020 2063 656e 7472 6f69 6420 3d20 6e70     centroid = np
-000257a0: 2e61 7272 6179 285b 6d6f 6d5b 2830 2c29  .array([mom[(0,)
-000257b0: 2a69 202b 2028 312c 2920 2b20 2830 2c29  *i + (1,) + (0,)
-000257c0: 2a28 6e64 696d 2d69 2d31 295d 200d 0a20  *(ndim-i-1)] .. 
-000257d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000257f0: 7261 6e67 6528 6e64 696d 295d 2920 2f20  range(ndim)]) / 
-00025800: 6d6f 6d5b 2830 2c29 2a6e 6469 6d5d 0d0a  mom[(0,)*ndim]..
-00025810: 2020 2020 7265 7475 726e 2063 656e 7472      return centr
-00025820: 6f69 640d 0a0d 0a64 6566 205f 6368 6563  oid....def _chec
-00025830: 6b5f 636c 6970 5f72 616e 6765 2869 6e5f  k_clip_range(in_
-00025840: 7261 6e67 652c 2069 6d67 2920 2d3e 2074  range, img) -> t
-00025850: 7570 6c65 5b66 6c6f 6174 2c20 666c 6f61  uple[float, floa
-00025860: 745d 3a0d 0a20 2020 2022 2222 0d0a 2020  t]:..    """..  
-00025870: 2020 4361 6c6c 6564 2069 6e20 636c 6970    Called in clip
-00025880: 5f6f 7574 6c69 6572 7328 2920 616e 6420  _outliers() and 
-00025890: 7265 7363 616c 655f 696e 7465 6e73 6974  rescale_intensit
-000258a0: 7928 292e 0d0a 2020 2020 2222 2220 2020  y()...    """   
-000258b0: 200d 0a20 2020 206c 6f77 6572 2c20 7570   ..    lower, up
-000258c0: 7065 7220 3d20 696e 5f72 616e 6765 0d0a  per = in_range..
-000258d0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000258e0: 6528 6c6f 7765 722c 2073 7472 2920 616e  e(lower, str) an
-000258f0: 6420 6c6f 7765 722e 656e 6473 7769 7468  d lower.endswith
-00025900: 2822 2522 293a 0d0a 2020 2020 2020 2020  ("%"):..        
-00025910: 6c6f 7765 7220 3d20 666c 6f61 7428 6c6f  lower = float(lo
-00025920: 7765 725b 3a2d 315d 290d 0a20 2020 2020  wer[:-1])..     
-00025930: 2020 206c 6f77 6572 6c69 6d20 3d20 6e70     lowerlim = np
-00025940: 2e70 6572 6365 6e74 696c 6528 696d 672c  .percentile(img,
-00025950: 206c 6f77 6572 290d 0a20 2020 2065 6c69   lower)..    eli
-00025960: 6620 6c6f 7765 7220 6973 204e 6f6e 653a  f lower is None:
-00025970: 0d0a 2020 2020 2020 2020 6c6f 7765 726c  ..        lowerl
-00025980: 696d 203d 206e 702e 6d69 6e28 696d 6729  im = np.min(img)
-00025990: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-000259a0: 2020 2020 206c 6f77 6572 6c69 6d20 3d20       lowerlim = 
-000259b0: 666c 6f61 7428 6c6f 7765 7229 0d0a 2020  float(lower)..  
-000259c0: 2020 0d0a 2020 2020 6966 2069 7369 6e73    ..    if isins
-000259d0: 7461 6e63 6528 7570 7065 722c 2073 7472  tance(upper, str
-000259e0: 2920 616e 6420 7570 7065 722e 656e 6473  ) and upper.ends
-000259f0: 7769 7468 2822 2522 293a 0d0a 2020 2020  with("%"):..    
-00025a00: 2020 2020 7570 7065 7220 3d20 666c 6f61      upper = floa
-00025a10: 7428 7570 7065 725b 3a2d 315d 290d 0a20  t(upper[:-1]).. 
-00025a20: 2020 2020 2020 2075 7070 6572 6c69 6d20         upperlim 
-00025a30: 3d20 6e70 2e70 6572 6365 6e74 696c 6528  = np.percentile(
-00025a40: 696d 672c 2075 7070 6572 290d 0a20 2020  img, upper)..   
-00025a50: 2065 6c69 6620 7570 7065 7220 6973 204e   elif upper is N
-00025a60: 6f6e 653a 0d0a 2020 2020 2020 2020 7570  one:..        up
-00025a70: 7065 726c 696d 203d 206e 702e 6d61 7828  perlim = np.max(
-00025a80: 696d 6729 0d0a 2020 2020 656c 7365 3a0d  img)..    else:.
-00025a90: 0a20 2020 2020 2020 2075 7070 6572 6c69  .        upperli
-00025aa0: 6d20 3d20 666c 6f61 7428 7570 7065 7229  m = float(upper)
-00025ab0: 0d0a 2020 2020 0d0a 2020 2020 6966 206c  ..    ..    if l
-00025ac0: 6f77 6572 6c69 6d20 3e3d 2075 7070 6572  owerlim >= upper
-00025ad0: 6c69 6d3a 0d0a 2020 2020 2020 2020 7261  lim:..        ra
-00025ae0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-00025af0: 226c 6f77 6572 6c69 6d20 6973 206c 6172  "lowerlim is lar
-00025b00: 6765 7220 7468 616e 2075 7070 6572 6c69  ger than upperli
-00025b10: 6d3a 207b 6c6f 7765 726c 696d 7d20 3e3d  m: {lowerlim} >=
-00025b20: 207b 7570 7065 726c 696d 7d22 290d 0a20   {upperlim}").. 
-00025b30: 2020 200d 0a20 2020 2072 6574 7572 6e20     ..    return 
-00025b40: 6c6f 7765 726c 696d 2c20 7570 7065 726c  lowerlim, upperl
-00025b50: 696d 0d0a 0d0a 6465 6620 5f73 7065 6369  im....def _speci
-00025b60: 6679 5f6f 6e65 2863 656e 7465 722c 2072  fy_one(center, r
-00025b70: 6164 6975 732c 2073 6861 7065 3a74 7570  adius, shape:tup
-00025b80: 6c65 2920 2d3e 2074 7570 6c65 5b73 6c69  le) -> tuple[sli
-00025b90: 6365 5d3a 0d0a 2020 2020 736c 203d 2074  ce]:..    sl = t
-00025ba0: 7570 6c65 2873 6c69 6365 286d 6178 2830  uple(slice(max(0
-00025bb0: 2c20 7863 2d72 292c 206d 696e 2878 632b  , xc-r), min(xc+
-00025bc0: 722b 312c 2073 6829 2c20 4e6f 6e65 2920  r+1, sh), None) 
-00025bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025be0: 2020 2020 2020 2020 2020 666f 7220 7863            for xc
-00025bf0: 2c20 722c 2073 6820 696e 207a 6970 2863  , r, sh in zip(c
-00025c00: 656e 7465 722c 2072 6164 6975 732c 2073  enter, radius, s
-00025c10: 6861 7065 2929 0d0a 2020 2020 7265 7475  hape))..    retu
-00025c20: 726e 2073 6c0d 0a0d 0a64 6566 2063 6865  rn sl....def che
-00025c30: 636b 5f66 696c 7465 725f 6675 6e63 2866  ck_filter_func(f
-00025c40: 293a 0d0a 2020 2020 6966 2066 2069 7320  ):..    if f is 
-00025c50: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2066  None:..        f
-00025c60: 203d 206c 616d 6264 6120 783a 2054 7275   = lambda x: Tru
-00025c70: 650d 0a20 2020 2065 6c69 6620 6e6f 7420  e..    elif not 
-00025c80: 6361 6c6c 6162 6c65 2866 293a 0d0a 2020  callable(f):..  
-00025c90: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00025ca0: 4572 726f 7228 2260 6669 6c74 6020 6d75  Error("`filt` mu
-00025cb0: 7374 2062 6520 6361 6c6c 6162 6c65 2e22  st be callable."
-00025cc0: 290d 0a20 2020 2072 6574 7572 6e20 660d  )..    return f.
-00025cd0: 0a0d 0a0d 0a64 6566 2077 6176 655f 6e75  .....def wave_nu
-00025ce0: 6d28 736c 3a20 736c 6963 652c 2073 3a20  m(sl: slice, s: 
-00025cf0: 696e 742c 2075 663a 2069 6e74 2920 2d3e  int, uf: int) ->
-00025d00: 2078 702e 6e64 6172 7261 793a 0d0a 2020   xp.ndarray:..  
-00025d10: 2020 2222 220d 0a20 2020 2041 2066 756e    """..    A fun
-00025d20: 6374 696f 6e20 7468 6174 206d 616b 6573  ction that makes
-00025d30: 2077 6176 6520 6e75 6d62 6572 2076 6572   wave number ver
-00025d40: 7469 6361 6c20 7665 6374 6f72 2e20 5265  tical vector. Re
-00025d50: 7475 726e 6564 2076 6563 746f 7220 7769  turned vector wi
-00025d60: 6c6c 0d0a 2020 2020 6265 205b 6b2f 732c  ll..    be [k/s,
-00025d70: 2028 6b20 2b20 312f 7566 292f 732c 2028   (k + 1/uf)/s, (
-00025d80: 6b20 2b20 322f 7566 292f 732c 202e 2e2e  k + 2/uf)/s, ...
-00025d90: 5d20 2877 6865 7265 206b 203d 2073 6c2e  ] (where k = sl.
-00025da0: 7374 6172 7429 0d0a 0d0a 2020 2020 5061  start)....    Pa
-00025db0: 7261 6d65 7465 7273 0d0a 2020 2020 2d2d  rameters..    --
-00025dc0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 736c  --------..    sl
-00025dd0: 203a 2073 6c69 6365 0d0a 2020 2020 2020   : slice..      
-00025de0: 2020 536c 6963 6520 7468 6174 2073 7065    Slice that spe
-00025df0: 6369 6679 2077 6869 6368 2070 6172 7420  cify which part 
-00025e00: 6f66 2074 6865 2069 6d61 6765 2077 696c  of the image wil
-00025e10: 6c20 6265 2074 7261 6e73 666f 726d 6564  l be transformed
-00025e20: 2e0d 0a20 2020 2073 203a 2069 6e74 0d0a  ...    s : int..
-00025e30: 2020 2020 2020 2020 5369 7a65 2061 6c6f          Size alo
-00025e40: 6e67 2063 6572 7461 696e 2064 696d 656e  ng certain dimen
-00025e50: 7369 6f6e 2e0d 0a20 2020 2075 6620 3a20  sion...    uf : 
-00025e60: 696e 740d 0a20 2020 2020 2020 2055 702d  int..        Up-
-00025e70: 7361 6d70 6c69 6e67 2066 6163 746f 7220  sampling factor 
-00025e80: 6f66 2063 6572 7461 696e 2064 696d 656e  of certain dimen
-00025e90: 7369 6f6e 2e0d 0a20 2020 2022 2222 0d0a  sion...    """..
-00025ea0: 2020 2020 7374 6172 7420 3d20 3020 6966      start = 0 if
-00025eb0: 2073 6c2e 7374 6172 7420 6973 204e 6f6e   sl.start is Non
-00025ec0: 6520 656c 7365 2073 6c2e 7374 6172 740d  e else sl.start.
-00025ed0: 0a20 2020 2073 746f 7020 3d20 7320 6966  .    stop = s if
-00025ee0: 2073 6c2e 7374 6f70 2069 7320 4e6f 6e65   sl.stop is None
-00025ef0: 2065 6c73 6520 736c 2e73 746f 700d 0a20   else sl.stop.. 
-00025f00: 2020 200d 0a20 2020 2069 6620 736c 2e73     ..    if sl.s
-00025f10: 7461 7274 2061 6e64 2073 6c2e 7374 6f70  tart and sl.stop
-00025f20: 2061 6e64 2073 7461 7274 203c 2030 2061   and start < 0 a
-00025f30: 6e64 2073 746f 7020 3e20 303a 0d0a 2020  nd stop > 0:..  
-00025f40: 2020 2020 2020 2320 6c69 6b65 2022 783d        # like "x=
-00025f50: 2d35 3a35 220d 0a20 2020 2020 2020 2070  -5:5"..        p
-00025f60: 6173 730d 0a20 2020 2065 6c73 653a 0d0a  ass..    else:..
-00025f70: 2020 2020 2020 2020 6966 202d 7320 3c20          if -s < 
-00025f80: 7374 6172 7420 3c20 303a 0d0a 2020 2020  start < 0:..    
-00025f90: 2020 2020 2020 2020 7374 6172 7420 2b3d          start +=
-00025fa0: 2073 0d0a 2020 2020 2020 2020 656c 6966   s..        elif
-00025fb0: 206e 6f74 2030 203c 3d20 7374 6172 7420   not 0 <= start 
-00025fc0: 3c20 733a 0d0a 2020 2020 2020 2020 2020  < s:..          
-00025fd0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00025fe0: 6f72 2866 2249 6e76 616c 6964 2076 616c  or(f"Invalid val
-00025ff0: 7565 2065 6e63 6f75 6e74 6572 6564 2069  ue encountered i
-00026000: 6e20 736c 6963 6520 7b73 6c7d 2e22 290d  n slice {sl}.").
-00026010: 0a20 2020 2020 2020 2069 6620 2d73 203c  .        if -s <
-00026020: 2073 746f 7020 3c3d 2030 3a0d 0a20 2020   stop <= 0:..   
-00026030: 2020 2020 2020 2020 2073 746f 7020 2b3d           stop +=
-00026040: 2073 0d0a 2020 2020 2020 2020 656c 6966   s..        elif
-00026050: 206e 6f74 2030 203c 2073 746f 7020 3c3d   not 0 < stop <=
-00026060: 2073 3a0d 0a20 2020 2020 2020 2020 2020   s:..           
-00026070: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00026080: 7228 6622 496e 7661 6c69 6420 7661 6c75  r(f"Invalid valu
-00026090: 6520 656e 636f 756e 7465 7265 6420 696e  e encountered in
-000260a0: 2073 6c69 6365 207b 736c 7d2e 2229 0d0a   slice {sl}.")..
-000260b0: 2020 2020 2020 2020 0d0a 2020 2020 6e20          ..    n 
-000260c0: 3d20 7374 6f70 202d 2073 7461 7274 0d0a  = stop - start..
-000260d0: 2020 2020 7265 7475 726e 2078 702e 6c69      return xp.li
-000260e0: 6e73 7061 6365 2873 7461 7274 2c20 7374  nspace(start, st
-000260f0: 6f70 2c20 6e2a 7566 2c20 656e 6470 6f69  op, n*uf, endpoi
-00026100: 6e74 3d46 616c 7365 295b 3a2c 206e 702e  nt=False)[:, np.
-00026110: 6e65 7761 7869 735d 0d0a                 newaxis]..
+0001bda0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0001bdb0: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+0001bdc0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+0001bdd0: 2020 7b64 696d 737d 7b75 7064 6174 657d    {dims}{update}
+0001bde0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+0001bdf0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+0001be00: 2d2d 2d2d 0d0a 2020 2020 2020 2020 496d  ----..        Im
+0001be10: 6741 7272 6179 0d0a 2020 2020 2020 2020  gArray..        
+0001be20: 2020 2020 436f 6e76 6578 2068 756c 6c20      Convex hull 
+0001be30: 696d 6167 652e 0d0a 2020 2020 2020 2020  image...        
+0001be40: 2222 2220 2020 2020 2020 200d 0a20 2020  """        ..   
+0001be50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001be60: 2e5f 6170 706c 795f 6461 736b 280d 0a20  ._apply_dask(.. 
+0001be70: 2020 2020 2020 2020 2020 2073 6b69 6d61             skima
+0001be80: 6765 2e6d 6f72 7068 6f6c 6f67 792e 636f  ge.morphology.co
+0001be90: 6e76 6578 5f68 756c 6c5f 696d 6167 652c  nvex_hull_image,
+0001bea0: 200d 0a20 2020 2020 2020 2020 2020 2063   ..            c
+0001beb0: 5f61 7865 733d 636f 6d70 6c65 6d65 6e74  _axes=complement
+0001bec0: 5f61 7865 7328 6469 6d73 2c20 7365 6c66  _axes(dims, self
+0001bed0: 2e61 7865 7329 2c20 0d0a 2020 2020 2020  .axes), ..      
+0001bee0: 2020 2020 2020 6474 7970 653d 626f 6f6c        dtype=bool
+0001bef0: 2c0d 0a20 2020 2020 2020 2029 2e61 7374  ,..        ).ast
+0001bf00: 7970 6528 626f 6f6c 290d 0a20 2020 2020  ype(bool)..     
+0001bf10: 2020 200d 0a20 2020 2040 5f64 6f63 732e     ..    @_docs.
+0001bf20: 7772 6974 655f 646f 6373 0d0a 2020 2020  write_docs..    
+0001bf30: 4064 696d 735f 746f 5f73 7061 7469 616c  @dims_to_spatial
+0001bf40: 5f61 7865 730d 0a20 2020 2040 6368 6563  _axes..    @chec
+0001bf50: 6b5f 696e 7075 745f 616e 645f 6f75 7470  k_input_and_outp
+0001bf60: 7574 286f 6e6c 795f 6269 6e61 7279 3d54  ut(only_binary=T
+0001bf70: 7275 6529 0d0a 2020 2020 6465 6620 736b  rue)..    def sk
+0001bf80: 656c 6574 6f6e 697a 6528 7365 6c66 2c20  eletonize(self, 
+0001bf90: 7261 6469 7573 3a20 666c 6f61 7420 3d20  radius: float = 
+0001bfa0: 302c 202a 2c20 6469 6d73 3a20 4469 6d73  0, *, dims: Dims
+0001bfb0: 203d 204e 6f6e 652c 2075 7064 6174 653d   = None, update=
+0001bfc0: 4661 6c73 6529 202d 3e20 496d 6741 7272  False) -> ImgArr
+0001bfd0: 6179 3a0d 0a20 2020 2020 2020 2022 2222  ay:..        """
+0001bfe0: 0d0a 2020 2020 2020 2020 536b 656c 6574  ..        Skelet
+0001bff0: 6f6e 697a 6520 696d 6167 6573 2e20 4f6e  onize images. On
+0001c000: 6c79 2077 6f72 6b73 2066 6f72 2062 696e  ly works for bin
+0001c010: 6172 7920 696d 6167 6573 2e0d 0a0d 0a20  ary images..... 
+0001c020: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001c030: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0001c040: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2072  -----..        r
+0001c050: 6164 6975 7320 3a20 666c 6f61 742c 206f  adius : float, o
+0001c060: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0001c070: 2020 2020 2052 6164 6975 7320 6f66 2073       Radius of s
+0001c080: 6b65 6c65 746f 6e2e 2054 6869 7320 6973  keleton. This is
+0001c090: 2061 6368 6965 7665 6420 7369 6d70 6c79   achieved simply
+0001c0a0: 2062 7920 6469 6c61 7469 6f6e 206f 6620   by dilation of 
+0001c0b0: 736b 656c 6574 6f6e 697a 6564 2072 6573  skeletonized res
+0001c0c0: 756c 7473 2e0d 0a20 2020 2020 2020 207b  ults...        {
+0001c0d0: 6469 6d73 7d7b 7570 6461 7465 7d0d 0a0d  dims}{update}...
+0001c0e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001c0f0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0001c100: 2d0d 0a20 2020 2020 2020 2049 6d67 4172  -..        ImgAr
+0001c110: 7261 790d 0a20 2020 2020 2020 2020 2020  ray..           
+0001c120: 2053 6b65 6c65 746f 6e69 7a65 6420 696d   Skeletonized im
+0001c130: 6167 652e 0d0a 2020 2020 2020 2020 2222  age...        ""
+0001c140: 2220 2020 2020 2020 200d 0a20 2020 2020  "        ..     
+0001c150: 2020 2069 6620 7261 6469 7573 203e 3d20     if radius >= 
+0001c160: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0001c170: 7365 6c65 6d20 3d20 7870 2e61 736e 756d  selem = xp.asnum
+0001c180: 7079 285f 7374 7275 6374 7572 6573 2e62  py(_structures.b
+0001c190: 616c 6c5f 6c69 6b65 2872 6164 6975 732c  all_like(radius,
+0001c1a0: 206c 656e 2864 696d 7329 2929 0d0a 2020   len(dims)))..  
+0001c1b0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001c1c0: 2020 2020 2020 2020 2073 656c 656d 203d           selem =
+0001c1d0: 204e 6f6e 650d 0a20 2020 2020 2020 200d   None..        .
+0001c1e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001c1f0: 7365 6c66 2e5f 6170 706c 795f 6461 736b  self._apply_dask
+0001c200: 280d 0a20 2020 2020 2020 2020 2020 205f  (..            _
+0001c210: 6669 6c74 6572 732e 736b 656c 6574 6f6e  filters.skeleton
+0001c220: 697a 652c 200d 0a20 2020 2020 2020 2020  ize, ..         
+0001c230: 2020 2063 5f61 7865 733d 636f 6d70 6c65     c_axes=comple
+0001c240: 6d65 6e74 5f61 7865 7328 6469 6d73 2c20  ment_axes(dims, 
+0001c250: 7365 6c66 2e61 7865 7329 2c0d 0a20 2020  self.axes),..   
+0001c260: 2020 2020 2020 2020 2061 7267 733d 2873           args=(s
+0001c270: 656c 656d 2c29 2c0d 0a20 2020 2020 2020  elem,),..       
+0001c280: 2020 2020 2064 7479 7065 3d62 6f6f 6c0d       dtype=bool.
+0001c290: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
+0001c2a0: 6528 626f 6f6c 290d 0a20 2020 2020 2020  e(bool)..       
+0001c2b0: 200d 0a20 2020 2040 5f64 6f63 732e 7772   ..    @_docs.wr
+0001c2c0: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
+0001c2d0: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
+0001c2e0: 7865 730d 0a20 2020 2040 6368 6563 6b5f  xes..    @check_
+0001c2f0: 696e 7075 745f 616e 645f 6f75 7470 7574  input_and_output
+0001c300: 286f 6e6c 795f 6269 6e61 7279 3d54 7275  (only_binary=Tru
+0001c310: 6529 0d0a 2020 2020 6465 6620 636f 756e  e)..    def coun
+0001c320: 745f 6e65 6967 6862 6f72 7328 0d0a 2020  t_neighbors(..  
+0001c330: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+0001c340: 2020 2020 202a 2c20 0d0a 2020 2020 2020       *, ..      
+0001c350: 2020 636f 6e6e 6563 7469 7669 7479 3a20    connectivity: 
+0001c360: 696e 7420 7c20 4e6f 6e65 203d 204e 6f6e  int | None = Non
+0001c370: 652c 0d0a 2020 2020 2020 2020 6d61 736b  e,..        mask
+0001c380: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+0001c390: 2020 2020 2020 2020 6469 6d73 3a20 4469          dims: Di
+0001c3a0: 6d73 203d 204e 6f6e 652c 0d0a 2020 2020  ms = None,..    
+0001c3b0: 2920 2d3e 2049 6d67 4172 7261 793a 0d0a  ) -> ImgArray:..
+0001c3c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0001c3d0: 2020 2020 2043 6f75 6e74 2074 6865 206e       Count the n
+0001c3e0: 756d 6265 7220 6f72 206e 6569 6768 626f  umber or neighbo
+0001c3f0: 7273 206f 6620 6269 6e61 7279 2069 6d61  rs of binary ima
+0001c400: 6765 732e 2054 6869 7320 6675 6e63 7469  ges. This functi
+0001c410: 6f6e 2063 616e 2062 6520 7573 6564 2066  on can be used f
+0001c420: 6f72 2063 726f 7373 2073 6563 7469 6f6e  or cross section
+0001c430: 0d0a 2020 2020 2020 2020 6f72 2062 7261  ..        or bra
+0001c440: 6e63 6820 6465 7465 6374 696f 6e2e 204f  nch detection. O
+0001c450: 6e6c 7920 776f 726b 7320 666f 7220 6269  nly works for bi
+0001c460: 6e61 7279 2069 6d61 6765 732e 0d0a 0d0a  nary images.....
+0001c470: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001c480: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0001c490: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0001c4a0: 7b63 6f6e 6e65 6374 6976 6974 797d 0d0a  {connectivity}..
+0001c4b0: 2020 2020 2020 2020 6d61 736b 203a 2062          mask : b
+0001c4c0: 6f6f 6c2c 2064 6566 6175 6c74 2069 7320  ool, default is 
+0001c4d0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+0001c4e0: 2020 4966 2054 7275 652c 206f 6e6c 7920    If True, only 
+0001c4f0: 6e65 6967 6862 6f72 7320 6f66 2070 6978  neighbors of pix
+0001c500: 656c 7320 7468 6174 2073 6174 6973 6679  els that satisfy
+0001c510: 2073 656c 663d 3d54 7275 6520 6973 2072   self==True is r
+0001c520: 6574 7572 6e65 642e 0d0a 2020 2020 2020  eturned...      
+0001c530: 2020 7b64 696d 737d 0d0a 0d0a 2020 2020    {dims}....    
+0001c540: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0001c550: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0001c560: 2020 2020 2020 496d 6741 7272 6179 0d0a        ImgArray..
+0001c570: 2020 2020 2020 2020 2020 2020 7569 6e74              uint
+0001c580: 3820 6172 7261 7920 6f66 2074 6865 206e  8 array of the n
+0001c590: 756d 6265 7220 6f66 206e 6569 6768 626f  umber of neighbo
+0001c5a0: 7273 2e0d 0a20 2020 2020 2020 2020 2020  rs...           
+0001c5b0: 200d 0a20 2020 2020 2020 2045 7861 6d70   ..        Examp
+0001c5c0: 6c65 730d 0a20 2020 2020 2020 202d 2d2d  les..        ---
+0001c5d0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2020  -----..         
+0001c5e0: 2020 203e 3e3e 2073 6b6c 203d 2069 6d67     >>> skl = img
+0001c5f0: 2e74 6872 6573 686f 6c64 2829 2e73 6b65  .threshold().ske
+0001c600: 6c65 746f 6e69 7a65 2829 0d0a 2020 2020  letonize()..    
+0001c610: 2020 2020 2020 2020 3e3e 3e20 6564 6765          >>> edge
+0001c620: 203d 2073 6b6c 2e63 6f75 6e74 5f6e 6569   = skl.count_nei
+0001c630: 6768 626f 7273 2829 0d0a 2020 2020 2020  ghbors()..      
+0001c640: 2020 2020 2020 3e3e 3e20 6e70 2e61 7267        >>> np.arg
+0001c650: 7768 6572 6528 6564 6765 203d 3d20 3129  where(edge == 1)
+0001c660: 2023 2067 6574 2063 6f6f 7264 696e 6174   # get coordinat
+0001c670: 6573 206f 6620 6669 6c61 6d65 6e74 2065  es of filament e
+0001c680: 6467 6573 2e0d 0a20 2020 2020 2020 2020  dges...         
+0001c690: 2020 203e 3e3e 206e 702e 6172 6777 6865     >>> np.argwhe
+0001c6a0: 7265 2865 6467 6520 3e3d 2033 2920 2320  re(edge >= 3) # 
+0001c6b0: 6765 7420 636f 6f72 6469 6e61 7465 7320  get coordinates 
+0001c6c0: 6f66 2066 696c 616d 656e 7420 6372 6f73  of filament cros
+0001c6d0: 7320 7365 6374 696f 6e73 2e0d 0a20 2020  s sections...   
+0001c6e0: 2020 2020 200d 0a20 2020 2020 2020 2022       ..        "
+0001c6f0: 2222 2020 2020 2020 2020 0d0a 2020 2020  ""        ..    
+0001c700: 2020 2020 6e64 696d 203d 206c 656e 2864      ndim = len(d
+0001c710: 696d 7329 0d0a 2020 2020 2020 2020 636f  ims)..        co
+0001c720: 6e6e 6563 7469 7669 7479 203d 206e 6469  nnectivity = ndi
+0001c730: 6d20 6966 2063 6f6e 6e65 6374 6976 6974  m if connectivit
+0001c740: 7920 6973 204e 6f6e 6520 656c 7365 2063  y is None else c
+0001c750: 6f6e 6e65 6374 6976 6974 790d 0a20 2020  onnectivity..   
+0001c760: 2020 2020 2073 656c 656d 203d 206e 6469       selem = ndi
+0001c770: 2e6d 6f72 7068 6f6c 6f67 792e 6765 6e65  .morphology.gene
+0001c780: 7261 7465 5f62 696e 6172 795f 7374 7275  rate_binary_stru
+0001c790: 6374 7572 6528 6e64 696d 2c20 636f 6e6e  cture(ndim, conn
+0001c7a0: 6563 7469 7669 7479 290d 0a20 2020 2020  ectivity)..     
+0001c7b0: 2020 2073 656c 656d 5b28 312c 292a 6e64     selem[(1,)*nd
+0001c7c0: 696d 5d20 3d20 300d 0a20 2020 2020 2020  im] = 0..       
+0001c7d0: 206f 7574 203d 2073 656c 662e 6173 5f75   out = self.as_u
+0001c7e0: 696e 7438 2829 2e5f 6170 706c 795f 6461  int8()._apply_da
+0001c7f0: 736b 280d 0a20 2020 2020 2020 2020 2020  sk(..           
+0001c800: 205f 6669 6c74 6572 732e 706f 7075 6c61   _filters.popula
+0001c810: 7469 6f6e 2c20 0d0a 2020 2020 2020 2020  tion, ..        
+0001c820: 2020 2020 635f 6178 6573 3d63 6f6d 706c      c_axes=compl
+0001c830: 656d 656e 745f 6178 6573 2864 696d 732c  ement_axes(dims,
+0001c840: 2073 656c 662e 6178 6573 292c 200d 0a20   self.axes), .. 
+0001c850: 2020 2020 2020 2020 2020 2061 7267 733d             args=
+0001c860: 2873 656c 656d 2c29 0d0a 2020 2020 2020  (selem,)..      
+0001c870: 2020 290d 0a20 2020 2020 2020 2069 6620    )..        if 
+0001c880: 6d61 736b 3a0d 0a20 2020 2020 2020 2020  mask:..         
+0001c890: 2020 206f 7574 5b7e 7365 6c66 2e76 616c     out[~self.val
+0001c8a0: 7565 5d20 3d20 300d 0a20 2020 2020 2020  ue] = 0..       
+0001c8b0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+0001c8c0: 6574 7572 6e20 6f75 742e 6173 7479 7065  eturn out.astype
+0001c8d0: 286e 702e 7569 6e74 3829 0d0a 2020 2020  (np.uint8)..    
+0001c8e0: 0d0a 2020 2020 405f 646f 6373 2e77 7269  ..    @_docs.wri
+0001c8f0: 7465 5f64 6f63 730d 0a20 2020 2040 6469  te_docs..    @di
+0001c900: 6d73 5f74 6f5f 7370 6174 6961 6c5f 6178  ms_to_spatial_ax
+0001c910: 6573 0d0a 2020 2020 4063 6865 636b 5f69  es..    @check_i
+0001c920: 6e70 7574 5f61 6e64 5f6f 7574 7075 7428  nput_and_output(
+0001c930: 6f6e 6c79 5f62 696e 6172 793d 5472 7565  only_binary=True
+0001c940: 290d 0a20 2020 2064 6566 2072 656d 6f76  )..    def remov
+0001c950: 655f 736b 656c 6574 6f6e 5f73 7472 7563  e_skeleton_struc
+0001c960: 7475 7265 280d 0a20 2020 2020 2020 2073  ture(..        s
+0001c970: 656c 662c 0d0a 2020 2020 2020 2020 7374  elf,..        st
+0001c980: 7275 6374 7572 653a 204c 6974 6572 616c  ructure: Literal
+0001c990: 5b22 7469 7022 2c20 2262 7261 6e63 6822  ["tip", "branch"
+0001c9a0: 2c20 2263 726f 7373 225d 203d 2022 7469  , "cross"] = "ti
+0001c9b0: 7022 2c0d 0a20 2020 2020 2020 202a 2c0d  p",..        *,.
+0001c9c0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+0001c9d0: 6976 6974 793a 2069 6e74 203d 204e 6f6e  ivity: int = Non
+0001c9e0: 652c 0d0a 2020 2020 2020 2020 6469 6d73  e,..        dims
+0001c9f0: 3a20 4469 6d73 203d 204e 6f6e 652c 0d0a  : Dims = None,..
+0001ca00: 2020 2020 2020 2020 7570 6461 7465 3a20          update: 
+0001ca10: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+0001ca20: 2020 2029 202d 3e20 496d 6741 7272 6179     ) -> ImgArray
+0001ca30: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+0001ca40: 2020 2020 2020 2020 5265 6d6f 7665 2063          Remove c
+0001ca50: 6572 7461 696e 2073 7472 7563 7475 7265  ertain structure
+0001ca60: 2066 726f 6d20 736b 656c 6574 6f6e 697a   from skeletoniz
+0001ca70: 6564 2069 6d61 6765 732e 0d0a 0d0a 2020  ed images.....  
+0001ca80: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0001ca90: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0001caa0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
+0001cab0: 7275 6374 7572 6520 3a20 7374 722c 2064  ructure : str, d
+0001cac0: 6566 6175 6c74 2069 7320 2274 6970 220d  efault is "tip".
+0001cad0: 0a20 2020 2020 2020 2020 2020 2057 6861  .            Wha
+0001cae0: 7420 7479 7065 206f 6620 7374 7275 6374  t type of struct
+0001caf0: 7572 6520 746f 2072 656d 6f76 652e 0d0a  ure to remove...
+0001cb00: 2020 2020 2020 2020 7b63 6f6e 6e65 6374          {connect
+0001cb10: 6976 6974 797d 0d0a 2020 2020 2020 2020  ivity}..        
+0001cb20: 7b64 696d 737d 7b75 7064 6174 657d 0d0a  {dims}{update}..
+0001cb30: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0001cb40: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0001cb50: 2d2d 0d0a 2020 2020 2020 2020 496d 6741  --..        ImgA
+0001cb60: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
+0001cb70: 2020 5072 6f63 6573 7365 6420 696d 6167    Processed imag
+0001cb80: 652e 0d0a 2020 2020 2020 2020 2222 2220  e...        """ 
+0001cb90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001cba0: 206f 7574 203d 2073 656c 662e 636f 7079   out = self.copy
+0001cbb0: 2829 0d0a 2020 2020 2020 2020 6e65 6967  ()..        neig
+0001cbc0: 6862 6f72 203d 2073 656c 662e 636f 756e  hbor = self.coun
+0001cbd0: 745f 6e65 6967 6862 6f72 7328 636f 6e6e  t_neighbors(conn
+0001cbe0: 6563 7469 7669 7479 3d63 6f6e 6e65 6374  ectivity=connect
+0001cbf0: 6976 6974 792c 2064 696d 733d 6469 6d73  ivity, dims=dims
+0001cc00: 290d 0a20 2020 2020 2020 2069 6620 7374  )..        if st
+0001cc10: 7275 6374 7572 6520 3d3d 2022 7469 7022  ructure == "tip"
+0001cc20: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0001cc30: 6c20 3d20 6e65 6967 6862 6f72 203d 3d20  l = neighbor == 
+0001cc40: 310d 0a20 2020 2020 2020 2065 6c69 6620  1..        elif 
+0001cc50: 7374 7275 6374 7572 6520 3d3d 2022 6272  structure == "br
+0001cc60: 616e 6368 223a 0d0a 2020 2020 2020 2020  anch":..        
+0001cc70: 2020 2020 736c 203d 206e 6569 6768 626f      sl = neighbo
+0001cc80: 7220 3e20 320d 0a20 2020 2020 2020 2065  r > 2..        e
+0001cc90: 6c69 6620 7374 7275 6374 7572 6520 3d3d  lif structure ==
+0001cca0: 2022 6372 6f73 7322 3a0d 0a20 2020 2020   "cross":..     
+0001ccb0: 2020 2020 2020 2073 6c20 3d20 6e65 6967         sl = neig
+0001ccc0: 6862 6f72 203e 2033 0d0a 2020 2020 2020  hbor > 3..      
+0001ccd0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001cce0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001ccf0: 4572 726f 7228 2260 6d6f 6465 6020 6d75  Error("`mode` mu
+0001cd00: 7374 2062 6520 6f6e 6520 6f66 207b 2774  st be one of {'t
+0001cd10: 6970 272c 2027 6272 616e 6368 272c 2027  ip', 'branch', '
+0001cd20: 6372 6f73 7327 7d2e 2229 0d0a 2020 2020  cross'}.")..    
+0001cd30: 2020 2020 6f75 742e 7661 6c75 655b 736c      out.value[sl
+0001cd40: 5d20 3d20 300d 0a20 2020 2020 2020 2072  ] = 0..        r
+0001cd50: 6574 7572 6e20 6f75 740d 0a20 2020 200d  eturn out..    .
+0001cd60: 0a20 2020 2040 6469 6d73 5f74 6f5f 7370  .    @dims_to_sp
+0001cd70: 6174 6961 6c5f 6178 6573 0d0a 2020 2020  atial_axes..    
+0001cd80: 4063 6865 636b 5f69 6e70 7574 5f61 6e64  @check_input_and
+0001cd90: 5f6f 7574 7075 7428 6e65 6564 5f6c 6162  _output(need_lab
+0001cda0: 656c 733d 5472 7565 290d 0a20 2020 2064  els=True)..    d
+0001cdb0: 6566 2077 6174 6572 7368 6564 280d 0a20  ef watershed(.. 
+0001cdc0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+0001cdd0: 2020 2020 2020 636f 6f72 6473 3a20 4d61        coords: Ma
+0001cde0: 726b 6572 4672 616d 6520 7c20 4e6f 6e65  rkerFrame | None
+0001cdf0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001ce00: 2020 2a2c 0d0a 2020 2020 2020 2020 636f    *,..        co
+0001ce10: 6e6e 6563 7469 7669 7479 3a20 696e 7420  nnectivity: int 
+0001ce20: 3d20 312c 0d0a 2020 2020 2020 2020 696e  = 1,..        in
+0001ce30: 7075 743a 204c 6974 6572 616c 5b22 7365  put: Literal["se
+0001ce40: 6c66 222c 2022 6469 7374 616e 6365 225d  lf", "distance"]
+0001ce50: 203d 2022 6469 7374 616e 6365 222c 200d   = "distance", .
+0001ce60: 0a20 2020 2020 2020 206d 696e 5f64 6973  .        min_dis
+0001ce70: 7461 6e63 653a 2066 6c6f 6174 203d 2032  tance: float = 2
+0001ce80: 2c0d 0a20 2020 2020 2020 2064 696d 733a  ,..        dims:
+0001ce90: 2044 696d 7320 3d20 4e6f 6e65 2c0d 0a20   Dims = None,.. 
+0001cea0: 2020 2029 202d 3e20 4c61 6265 6c3a 0d0a     ) -> Label:..
+0001ceb0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0001cec0: 2020 2020 204c 6162 656c 2073 6567 6d65       Label segme
+0001ced0: 6e74 6174 696f 6e20 7573 696e 6720 7761  ntation using wa
+0001cee0: 7465 7273 6865 6420 616c 676f 7269 7468  tershed algorith
+0001cef0: 6d2e 0d0a 0d0a 2020 2020 2020 2020 5061  m.....        Pa
+0001cf00: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+0001cf10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+0001cf20: 2020 2020 2020 636f 6f72 6473 203a 204d        coords : M
+0001cf30: 6172 6b65 7246 7261 6d65 2c20 6f70 7469  arkerFrame, opti
+0001cf40: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+0001cf50: 2020 5265 7475 726e 6564 2062 7920 7375    Returned by su
+0001cf60: 6368 2061 7320 6070 6561 6b5f 6c6f 6361  ch as `peak_loca
+0001cf70: 6c5f 6d61 7828 2960 2e20 4172 7261 7920  l_max()`. Array 
+0001cf80: 6f66 2063 6f6f 7264 696e 6174 6573 206f  of coordinates o
+0001cf90: 6620 7065 616b 732e 0d0a 2020 2020 2020  f peaks...      
+0001cfa0: 2020 7b63 6f6e 6e65 6374 6976 6974 797d    {connectivity}
+0001cfb0: 0d0a 2020 2020 2020 2020 696e 7075 7420  ..        input 
+0001cfc0: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
+0001cfd0: 0a20 2020 2020 2020 2020 2020 2057 6861  .            Wha
+0001cfe0: 7420 696d 6167 6520 7769 6c6c 2062 6520  t image will be 
+0001cff0: 7468 6520 696e 7075 7420 6f66 2077 6174  the input of wat
+0001d000: 6572 7368 6564 2061 6c67 6f72 6974 686d  ershed algorithm
+0001d010: 2e20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0001d020: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001d030: 2020 2020 2020 2020 202d 2022 7365 6c66           - "self
+0001d040: 2220 2e2e 2e20 7365 6c66 2069 7320 7573  " ... self is us
+0001d050: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
+0001d060: 202d 2022 6469 7374 616e 6365 2220 2e2e   - "distance" ..
+0001d070: 2e20 6469 7374 616e 6365 206d 6170 206f  . distance map o
+0001d080: 6620 7365 6c66 2e6c 6162 656c 7320 6973  f self.labels is
+0001d090: 2075 7365 642e 0d0a 2020 2020 2020 2020   used...        
+0001d0a0: 2020 2020 0d0a 2020 2020 2020 2020 7b64      ..        {d
+0001d0b0: 696d 737d 0d0a 2020 2020 2020 2020 2020  ims}..          
+0001d0c0: 2020 0d0a 2020 2020 2020 2020 5265 7475    ..        Retu
+0001d0d0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+0001d0e0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4c61  ----..        La
+0001d0f0: 6265 6c0d 0a20 2020 2020 2020 2020 2020  bel..           
+0001d100: 2055 7064 6174 6564 206c 6162 656c 732e   Updated labels.
+0001d110: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0001d120: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001d130: 2023 2050 7265 7061 7265 2074 6865 2069   # Prepare the i
+0001d140: 6e70 7574 2069 6d61 6765 2e0d 0a20 2020  nput image...   
+0001d150: 2020 2020 2069 6620 696e 7075 7420 3d3d       if input ==
+0001d160: 2022 7365 6c66 223a 0d0a 2020 2020 2020   "self":..      
+0001d170: 2020 2020 2020 696e 7075 745f 696d 6720        input_img 
+0001d180: 3d20 7365 6c66 2e63 6f70 7928 290d 0a20  = self.copy().. 
+0001d190: 2020 2020 2020 2065 6c69 6620 696e 7075         elif inpu
+0001d1a0: 7420 3d3d 2022 6469 7374 616e 6365 223a  t == "distance":
+0001d1b0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+0001d1c0: 7075 745f 696d 6720 3d20 7365 6c66 2e5f  put_img = self._
+0001d1d0: 5f63 6c61 7373 5f5f 2873 656c 662e 6c61  _class__(self.la
+0001d1e0: 6265 6c73 3e30 2c20 6178 6573 3d73 656c  bels>0, axes=sel
+0001d1f0: 662e 6178 6573 292e 6469 7374 616e 6365  f.axes).distance
+0001d200: 5f6d 6170 2864 696d 733d 6469 6d73 290d  _map(dims=dims).
+0001d210: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0001d220: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001d230: 6520 5661 6c75 6545 7272 6f72 2822 2769  e ValueError("'i
+0001d240: 6e70 7574 5f27 206d 7573 7420 6265 2065  nput_' must be e
+0001d250: 6974 6865 7220 2773 656c 6627 206f 7220  ither 'self' or 
+0001d260: 2764 6973 7461 6e63 6527 2e22 290d 0a20  'distance'.").. 
+0001d270: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0001d280: 0a20 2020 2020 2020 2069 6620 696e 7075  .        if inpu
+0001d290: 745f 696d 672e 6474 7970 6520 3d3d 2062  t_img.dtype == b
+0001d2a0: 6f6f 6c3a 0d0a 2020 2020 2020 2020 2020  ool:..          
+0001d2b0: 2020 696e 7075 745f 696d 6720 3d20 696e    input_img = in
+0001d2c0: 7075 745f 696d 672e 6173 7479 7065 286e  put_img.astype(n
+0001d2d0: 702e 7569 6e74 3829 0d0a 2020 2020 2020  p.uint8)..      
+0001d2e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001d2f0: 696e 7075 745f 696d 672e 6c61 6265 6c73  input_img.labels
+0001d300: 203d 2073 656c 662e 6c61 6265 6c73 0d0a   = self.labels..
+0001d310: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001d320: 2020 6966 2063 6f6f 7264 7320 6973 204e    if coords is N
+0001d330: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0001d340: 2020 636f 6f72 6473 203d 2069 6e70 7574    coords = input
+0001d350: 5f69 6d67 2e70 6561 6b5f 6c6f 6361 6c5f  _img.peak_local_
+0001d360: 6d61 7828 6d69 6e5f 6469 7374 616e 6365  max(min_distance
+0001d370: 3d6d 696e 5f64 6973 7461 6e63 652c 2064  =min_distance, d
+0001d380: 696d 733d 6469 6d73 290d 0a20 2020 2020  ims=dims)..     
+0001d390: 2020 200d 0a20 2020 2020 2020 206c 6162     ..        lab
+0001d3a0: 656c 7320 3d20 6c61 7267 6573 745f 7a65  els = largest_ze
+0001d3b0: 726f 7328 696e 7075 745f 696d 672e 7368  ros(input_img.sh
+0001d3c0: 6170 6529 0d0a 2020 2020 2020 2020 7368  ape)..        sh
+0001d3d0: 6170 6520 3d20 7365 6c66 2e73 697a 6573  ape = self.sizes
+0001d3e0: 6f66 2864 696d 7329 0d0a 2020 2020 2020  of(dims)..      
+0001d3f0: 2020 6e5f 6c61 6265 6c73 203d 2030 0d0a    n_labels = 0..
+0001d400: 2020 2020 2020 2020 635f 6178 6573 203d          c_axes =
+0001d410: 2063 6f6d 706c 656d 656e 745f 6178 6573   complement_axes
+0001d420: 2864 696d 732c 2073 656c 662e 6178 6573  (dims, self.axes
+0001d430: 290d 0a20 2020 2020 2020 206d 6172 6b65  )..        marke
+0001d440: 7273 203d 206e 702e 7a65 726f 7328 7368  rs = np.zeros(sh
+0001d450: 6170 652c 2064 7479 7065 3d6c 6162 656c  ape, dtype=label
+0001d460: 732e 6474 7970 6529 2023 2070 6c61 6365  s.dtype) # place
+0001d470: 686f 6c64 6572 2066 6f72 206d 6178 696d  holder for maxim
+0001d480: 610d 0a20 2020 2020 2020 2066 6f72 2073  a..        for s
+0001d490: 6c2c 2063 7264 2069 6e20 636f 6f72 6473  l, crd in coords
+0001d4a0: 2e69 7465 7228 635f 6178 6573 293a 0d0a  .iter(c_axes):..
+0001d4b0: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
+0001d4c0: 642e 7661 6c75 6573 2069 7320 284e 2c20  d.values is (N, 
+0001d4d0: 3229 2061 7272 6179 2073 6f20 7475 706c  2) array so tupl
+0001d4e0: 6528 6372 642e 7661 6c75 6573 2e54 2e74  e(crd.values.T.t
+0001d4f0: 6f6c 6973 7428 2929 2069 7320 7477 6f20  olist()) is two 
+0001d500: 284e 2c29 206c 6973 742e 0d0a 2020 2020  (N,) list...    
+0001d510: 2020 2020 2020 2020 6372 6420 3d20 6372          crd = cr
+0001d520: 642e 7661 6c75 6573 2e54 2e74 6f6c 6973  d.values.T.tolis
+0001d530: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0001d540: 206d 6172 6b65 7273 5b74 7570 6c65 2863   markers[tuple(c
+0001d550: 7264 295d 203d 206e 702e 6172 616e 6765  rd)] = np.arange
+0001d560: 2831 2c20 6c65 6e28 6372 645b 305d 292b  (1, len(crd[0])+
+0001d570: 312c 2064 7479 7065 3d6c 6162 656c 732e  1, dtype=labels.
+0001d580: 6474 7970 6529 0d0a 2020 2020 2020 2020  dtype)..        
+0001d590: 2020 2020 6c61 6265 6c73 5b73 6c5d 203d      labels[sl] =
+0001d5a0: 2073 6b73 6567 2e77 6174 6572 7368 6564   skseg.watershed
+0001d5b0: 282d 696e 7075 745f 696d 672e 7661 6c75  (-input_img.valu
+0001d5c0: 655b 736c 5d2c 206d 6172 6b65 7273 2c20  e[sl], markers, 
+0001d5d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5f0: 2020 2020 2020 2020 2020 6d61 736b 3d69            mask=i
+0001d600: 6e70 7574 5f69 6d67 2e6c 6162 656c 732e  nput_img.labels.
+0001d610: 7661 6c75 655b 736c 5d2c 200d 0a20 2020  value[sl], ..   
+0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d640: 2020 2020 2063 6f6e 6e65 6374 6976 6974       connectivit
+0001d650: 793d 636f 6e6e 6563 7469 7669 7479 290d  y=connectivity).
+0001d660: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+0001d670: 656c 735b 736c 5d5b 6c61 6265 6c73 5b73  els[sl][labels[s
+0001d680: 6c5d 3e30 5d20 2b3d 206e 5f6c 6162 656c  l]>0] += n_label
+0001d690: 730d 0a20 2020 2020 2020 2020 2020 206e  s..            n
+0001d6a0: 5f6c 6162 656c 7320 3d20 6c61 6265 6c73  _labels = labels
+0001d6b0: 5b73 6c5d 2e6d 6178 2829 0d0a 2020 2020  [sl].max()..    
+0001d6c0: 2020 2020 2020 2020 6d61 726b 6572 735b          markers[
+0001d6d0: 3a5d 203d 2030 2023 2072 6573 6574 2070  :] = 0 # reset p
+0001d6e0: 6c61 6365 686f 6c64 6572 0d0a 2020 2020  laceholder..    
+0001d6f0: 2020 2020 0d0a 2020 2020 2020 2020 6c61      ..        la
+0001d700: 6265 6c73 203d 206c 6162 656c 732e 7669  bels = labels.vi
+0001d710: 6577 284c 6162 656c 290d 0a20 2020 2020  ew(Label)..     
+0001d720: 2020 2073 656c 662e 6c61 6265 6c73 203d     self.labels =
+0001d730: 206c 6162 656c 732e 6f70 7469 6d69 7a65   labels.optimize
+0001d740: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0001d750: 2e6c 6162 656c 732e 5f73 6574 5f69 6e66  .labels._set_inf
+0001d760: 6f28 7365 6c66 290d 0a20 2020 2020 2020  o(self)..       
+0001d770: 2073 656c 662e 6c61 6265 6c73 2e73 6574   self.labels.set
+0001d780: 5f73 6361 6c65 2873 656c 6629 0d0a 2020  _scale(self)..  
+0001d790: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001d7a0: 662e 6c61 6265 6c73 0d0a 2020 2020 0d0a  f.labels..    ..
+0001d7b0: 2020 2020 405f 646f 6373 2e77 7269 7465      @_docs.write
+0001d7c0: 5f64 6f63 730d 0a20 2020 2040 6469 6d73  _docs..    @dims
+0001d7d0: 5f74 6f5f 7370 6174 6961 6c5f 6178 6573  _to_spatial_axes
+0001d7e0: 0d0a 2020 2020 4063 6865 636b 5f69 6e70  ..    @check_inp
+0001d7f0: 7574 5f61 6e64 5f6f 7574 7075 7428 6e65  ut_and_output(ne
+0001d800: 6564 5f6c 6162 656c 733d 5472 7565 290d  ed_labels=True).
+0001d810: 0a20 2020 2064 6566 2072 616e 646f 6d5f  .    def random_
+0001d820: 7761 6c6b 6572 280d 0a20 2020 2020 2020  walker(..       
+0001d830: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+0001d840: 6265 7461 3a20 666c 6f61 7420 3d20 3133  beta: float = 13
+0001d850: 302c 0d0a 2020 2020 2020 2020 6d6f 6465  0,..        mode
+0001d860: 3a20 4c69 7465 7261 6c5b 2263 6722 2c20  : Literal["cg", 
+0001d870: 2263 675f 6a22 2c20 2263 675f 6d67 222c  "cg_j", "cg_mg",
+0001d880: 2022 6266 225d 203d 2022 6367 5f6a 222c   "bf"] = "cg_j",
+0001d890: 200d 0a20 2020 2020 2020 2074 6f6c 3a20   ..        tol: 
+0001d8a0: 666c 6f61 7420 3d20 3165 2d33 2c20 0d0a  float = 1e-3, ..
+0001d8b0: 2020 2020 2020 2020 2a2c 0d0a 2020 2020          *,..    
+0001d8c0: 2020 2020 6469 6d73 3a20 4469 6d73 203d      dims: Dims =
+0001d8d0: 204e 6f6e 652c 0d0a 2020 2020 2920 2d3e   None,..    ) ->
+0001d8e0: 204c 6162 656c 3a0d 0a20 2020 2020 2020   Label:..       
+0001d8f0: 2022 2222 0d0a 2020 2020 2020 2020 5261   """..        Ra
+0001d900: 6e64 6f6d 2077 616c 6b65 7220 7365 676d  ndom walker segm
+0001d910: 656e 7461 7469 6f6e 2e20 4f6e 6c79 2077  entation. Only w
+0001d920: 7261 7070 6564 2073 6b69 6d61 6765 2073  rapped skimage s
+0001d930: 6567 6d65 6e74 6174 696f 6e2e 200d 0a20  egmentation. .. 
+0001d940: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001d950: 2060 6073 656c 662e 6c61 6265 6c73 6060   ``self.labels``
+0001d960: 2077 696c 6c20 6265 2073 6567 6d65 6e74   will be segment
+0001d970: 6564 2061 6e64 2075 7064 6174 6564 2069  ed and updated i
+0001d980: 6e70 6c61 6365 2e0d 0a0d 0a20 2020 2020  nplace.....     
+0001d990: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+0001d9a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001d9b0: 2d0d 0a20 2020 2020 2020 2062 6574 612c  -..        beta,
+0001d9c0: 206d 6f64 652c 2074 6f6c 0d0a 2020 2020   mode, tol..    
+0001d9d0: 2020 2020 2020 2020 7365 6520 736b 696d          see skim
+0001d9e0: 6167 652e 7365 676d 656e 7461 7469 6f6e  age.segmentation
+0001d9f0: 2e72 616e 646f 6d5f 7761 6c6b 6572 0d0a  .random_walker..
+0001da00: 2020 2020 2020 2020 7b64 696d 737d 0d0a          {dims}..
+0001da10: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0001da20: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0001da30: 2d2d 0d0a 2020 2020 2020 2020 496d 6741  --..        ImgA
+0001da40: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
+0001da50: 2020 5265 6c61 6265 6c65 6420 696d 6167    Relabeled imag
+0001da60: 652e 0d0a 2020 2020 2020 2020 2222 2220  e...        """ 
+0001da70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001da80: 2063 5f61 7865 7320 3d20 636f 6d70 6c65   c_axes = comple
+0001da90: 6d65 6e74 5f61 7865 7328 6469 6d73 2c20  ment_axes(dims, 
+0001daa0: 7365 6c66 2e61 7865 7329 0d0a 2020 2020  self.axes)..    
+0001dab0: 2020 2020 0d0a 2020 2020 2020 2020 666f      ..        fo
+0001dac0: 7220 736c 2c20 696d 6720 696e 2073 656c  r sl, img in sel
+0001dad0: 662e 6974 6572 2863 5f61 7865 732c 2069  f.iter(c_axes, i
+0001dae0: 7372 6177 3d54 7275 6529 3a0d 0a20 2020  sraw=True):..   
+0001daf0: 2020 2020 2020 2020 2069 6d67 2e6c 6162           img.lab
+0001db00: 656c 735b 3a5d 203d 2073 6b73 6567 2e72  els[:] = skseg.r
+0001db10: 616e 646f 6d5f 7761 6c6b 6572 280d 0a20  andom_walker(.. 
+0001db20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001db30: 6d67 2e76 616c 7565 2c20 696d 672e 6c61  mg.value, img.la
+0001db40: 6265 6c73 2e76 616c 7565 2c20 6265 7461  bels.value, beta
+0001db50: 3d62 6574 612c 206d 6f64 653d 6d6f 6465  =beta, mode=mode
+0001db60: 2c20 746f 6c3d 746f 6c0d 0a20 2020 2020  , tol=tol..     
+0001db70: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001db80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001db90: 7365 6c66 2e6c 6162 656c 732e 5f73 6574  self.labels._set
+0001dba0: 5f69 6e66 6f28 7365 6c66 290d 0a20 2020  _info(self)..   
+0001dbb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001dbc0: 2e6c 6162 656c 730d 0a20 2020 200d 0a20  .labels..    .. 
+0001dbd0: 2020 2064 6566 206c 6162 656c 5f74 6872     def label_thr
+0001dbe0: 6573 686f 6c64 280d 0a20 2020 2020 2020  eshold(..       
+0001dbf0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+0001dc00: 7468 723a 2066 6c6f 6174 207c 2054 6872  thr: float | Thr
+0001dc10: 6561 7368 6f6c 644d 6574 686f 6420 3d20  easholdMethod = 
+0001dc20: 226f 7473 7522 2c0d 0a20 2020 2020 2020  "otsu",..       
+0001dc30: 2066 696c 743a 2043 616c 6c61 626c 655b   filt: Callable[
+0001dc40: 2e2e 2e2c 2062 6f6f 6c5d 207c 204e 6f6e  ..., bool] | Non
+0001dc50: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
+0001dc60: 2020 202a 2c0d 0a20 2020 2020 2020 2064     *,..        d
+0001dc70: 696d 733a 2044 696d 7320 3d20 4e6f 6e65  ims: Dims = None
+0001dc80: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
+0001dc90: 7267 732c 0d0a 2020 2020 2920 2d3e 204c  rgs,..    ) -> L
+0001dca0: 6162 656c 3a0d 0a20 2020 2020 2020 2022  abel:..        "
+0001dcb0: 2222 0d0a 2020 2020 2020 2020 4d61 6b65  ""..        Make
+0001dcc0: 206c 6162 656c 7320 7769 7468 2074 6872   labels with thr
+0001dcd0: 6573 686f 6c64 2829 2e20 4265 2073 7572  eshold(). Be sur
+0001dce0: 6520 7468 6174 206b 6579 776f 7264 2061  e that keyword a
+0001dcf0: 7267 756d 656e 7420 6060 6469 6d73 6060  rgument ``dims``
+0001dd00: 2063 616e 2062 650d 0a20 2020 2020 2020   can be..       
+0001dd10: 2064 6966 6665 7265 6e74 2028 696e 206d   different (in m
+0001dd20: 6f73 7420 6361 7365 7320 666f 7220 3e34  ost cases for >4
+0001dd30: 4420 696d 6167 6573 2920 6265 7477 6565  D images) betwee
+0001dd40: 6e20 7468 7265 7368 6f6c 6428 2920 616e  n threshold() an
+0001dd50: 6420 6c61 6265 6c28 292e 0d0a 2020 2020  d label()...    
+0001dd60: 2020 2020 496e 2074 6869 7320 6675 6e63      In this func
+0001dd70: 7469 6f6e 2c20 626f 7468 2066 756e 6374  tion, both funct
+0001dd80: 696f 6e20 7769 6c6c 2068 6176 6520 7468  ion will have th
+0001dd90: 6520 7361 6d65 2060 6064 696d 7360 6020  e same ``dims`` 
+0001dda0: 666f 7220 7369 6d70 6c69 6369 7479 2e0d  for simplicity..
+0001ddb0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0001ddc0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+0001ddd0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+0001dde0: 2020 2074 6872 3a20 666c 6f61 7420 6f72     thr: float or
+0001ddf0: 2073 7472 206f 7220 4e6f 6e65 2c20 6f70   str or None, op
+0001de00: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0001de10: 2020 2020 5468 7265 7368 6f6c 6420 7661      Threshold va
+0001de20: 6c75 652c 206f 7220 7468 7265 7368 6f6c  lue, or threshol
+0001de30: 6469 6e67 2061 6c67 6f72 6974 686d 2e0d  ding algorithm..
+0001de40: 0a20 2020 2020 2020 207b 6469 6d73 7d0d  .        {dims}.
+0001de50: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+0001de60: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001de70: 4b65 7977 6f72 6420 6172 6775 6d65 6e74  Keyword argument
+0001de80: 7320 7468 6174 2077 696c 6c20 7061 7373  s that will pass
+0001de90: 6564 2074 6f20 6675 6e63 7469 6f6e 2069  ed to function i
+0001dea0: 6e64 6963 6174 6564 2069 6e20 276d 6574  ndicated in 'met
+0001deb0: 686f 6427 2e0d 0a20 2020 2020 2020 200d  hod'...        .
+0001dec0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001ded0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0001dee0: 2d0d 0a20 2020 2020 2020 204c 6162 656c  -..        Label
+0001def0: 0d0a 2020 2020 2020 2020 2020 2020 4e65  ..            Ne
+0001df00: 776c 7920 6372 6561 7465 6420 6c61 6265  wly created labe
+0001df10: 6c2e 0d0a 2020 2020 2020 2020 2222 2220  l...        """ 
+0001df20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001df30: 206c 6162 656c 7320 3d20 7365 6c66 2e74   labels = self.t
+0001df40: 6872 6573 686f 6c64 2874 6872 3d74 6872  hreshold(thr=thr
+0001df50: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
+0001df60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001df70: 2e6c 6162 656c 286c 6162 656c 732c 2066  .label(labels, f
+0001df80: 696c 743d 6669 6c74 2c20 6469 6d73 3d64  ilt=filt, dims=d
+0001df90: 696d 7329 0d0a 2020 2020 0d0a 2020 2020  ims)..    ..    
+0001dfa0: 6465 6620 7265 6769 6f6e 7072 6f70 7328  def regionprops(
+0001dfb0: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
+0001dfc0: 0a20 2020 2020 2020 2070 726f 7065 7274  .        propert
+0001dfd0: 6965 733a 2049 7465 7261 626c 655b 7374  ies: Iterable[st
+0001dfe0: 725d 207c 2073 7472 203d 2028 226d 6561  r] | str = ("mea
+0001dff0: 6e5f 696e 7465 6e73 6974 7922 2c29 2c0d  n_intensity",),.
+0001e000: 0a20 2020 2020 2020 202a 2c20 0d0a 2020  .        *, ..  
+0001e010: 2020 2020 2020 6578 7472 615f 7072 6f70        extra_prop
+0001e020: 6572 7469 6573 3a20 4974 6572 6162 6c65  erties: Iterable
+0001e030: 5b43 616c 6c61 626c 655d 207c 204e 6f6e  [Callable] | Non
+0001e040: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2029  e = None,..    )
+0001e050: 202d 3e20 4461 7461 4469 6374 5b73 7472   -> DataDict[str
+0001e060: 2c20 5072 6f70 4172 7261 795d 3a0d 0a20  , PropArray]:.. 
+0001e070: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0001e080: 2020 2020 4d75 6c74 692d 6469 6d65 6e73      Multi-dimens
+0001e090: 696f 6e61 6c20 7265 6769 6f6e 2070 726f  ional region pro
+0001e0a0: 7065 7274 7920 7175 616e 7469 6669 6361  perty quantifica
+0001e0b0: 7469 6f6e 2e0d 0a20 2020 2020 2020 200d  tion...        .
+0001e0c0: 0a20 2020 2020 2020 2052 756e 2073 6b69  .        Run ski
+0001e0d0: 6d61 6765 2773 2072 6567 696f 6e70 726f  mage's regionpro
+0001e0e0: 7073 2829 2066 756e 6374 696f 6e20 616e  ps() function an
+0001e0f0: 6420 7265 7475 726e 2074 6865 2072 6573  d return the res
+0001e100: 756c 7473 2061 7320 5072 6f70 4172 7261  ults as PropArra
+0001e110: 792c 2073 6f0d 0a20 2020 2020 2020 2074  y, so..        t
+0001e120: 6861 7420 796f 7520 6361 6e20 6163 6365  hat you can acce
+0001e130: 7373 2075 7369 6e67 2066 6c65 7869 626c  ss using flexibl
+0001e140: 6520 736c 6963 696e 672e 2046 6f72 2065  e slicing. For e
+0001e150: 7861 6d70 6c65 2c20 6966 2061 2074 6379  xample, if a tcy
+0001e160: 782d 696d 6167 6520 6973 0d0a 2020 2020  x-image is..    
+0001e170: 2020 2020 616e 616c 797a 6564 2077 6974      analyzed wit
+0001e180: 6820 6060 7072 6f70 6572 7469 6573 3d28  h ``properties=(
+0001e190: 2258 222c 2022 5922 2960 602c 2074 6865  "X", "Y")``, the
+0001e1a0: 6e20 796f 7520 6361 6e20 6765 7420 5827  n you can get X'
+0001e1b0: 7320 7469 6d65 2d63 6f75 7273 6520 7072  s time-course pr
+0001e1c0: 6f66 696c 650d 0a20 2020 2020 2020 206f  ofile..        o
+0001e1d0: 6620 6368 616e 6e65 6c20 3120 6174 206c  f channel 1 at l
+0001e1e0: 6162 656c 2033 2062 7920 6060 7072 6f70  abel 3 by ``prop
+0001e1f0: 5b22 5822 5d5b 2270 3d35 3b63 3d31 225d  ["X"]["p=5;c=1"]
+0001e200: 6060 206f 7220 6060 7072 6f70 2e58 5b22  `` or ``prop.X["
+0001e210: 703d 353b 633d 3122 5d60 602e 0d0a 0d0a  p=5;c=1"]``.....
+0001e220: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001e230: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0001e240: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0001e250: 7072 6f70 6572 7469 6573 203a 2069 7465  properties : ite
+0001e260: 7261 626c 652c 206f 7074 696f 6e61 6c0d  rable, optional.
+0001e270: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0001e280: 7065 7274 6965 7320 746f 2061 6e61 6c79  perties to analy
+0001e290: 7a65 2c20 7365 6520 6060 736b 696d 6167  ze, see ``skimag
+0001e2a0: 652e 6d65 6173 7572 652e 7265 6769 6f6e  e.measure.region
+0001e2b0: 7072 6f70 7360 602e 0d0a 2020 2020 2020  props``...      
+0001e2c0: 2020 6578 7472 615f 7072 6f70 6572 7469    extra_properti
+0001e2d0: 6573 203a 2069 7465 7261 626c 6520 6f66  es : iterable of
+0001e2e0: 2063 616c 6c61 626c 652c 206f 7074 696f   callable, optio
+0001e2f0: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+0001e300: 2065 7874 7261 2070 726f 7065 7274 6965   extra propertie
+0001e310: 7320 746f 2061 6e61 6c79 7a65 2c20 7365  s to analyze, se
+0001e320: 6520 6060 736b 696d 6167 652e 6d65 6173  e ``skimage.meas
+0001e330: 7572 652e 7265 6769 6f6e 7072 6f70 7360  ure.regionprops`
+0001e340: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
+0001e350: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0001e360: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0001e370: 4461 7461 4469 6374 206f 6620 5072 6f70  DataDict of Prop
+0001e380: 4172 7261 790d 0a20 2020 2020 2020 2020  Array..         
+0001e390: 2020 2044 6963 7469 6f6e 6172 7920 6861     Dictionary ha
+0001e3a0: 7320 6b65 7973 206f 6620 7072 6f70 6572  s keys of proper
+0001e3b0: 7469 6573 2074 6861 7420 6172 6520 7370  ties that are sp
+0001e3c0: 6563 6966 6965 6420 6279 2060 7072 6f70  ecified by `prop
+0001e3d0: 6572 7469 6573 602e 2045 6163 6820 7661  erties`. Each va
+0001e3e0: 6c75 650d 0a20 2020 2020 2020 2020 2020  lue..           
+0001e3f0: 2068 6173 2074 6865 2061 7272 6179 206f   has the array o
+0001e400: 6620 7072 6f70 6572 7469 6573 2e0d 0a20  f properties... 
+0001e410: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001e420: 2020 2020 2045 7861 6d70 6c65 730d 0a20       Examples.. 
+0001e430: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0d         --------.
+0001e440: 0a20 2020 2020 2020 204d 6561 7375 7265  .        Measure
+0001e450: 2072 6567 696f 6e20 7072 6f70 6572 7469   region properti
+0001e460: 6573 2061 726f 756e 6420 7369 6e67 6c65  es around single
+0001e470: 206d 6f6c 6563 756c 6573 2e0d 0a20 2020   molecules...   
+0001e480: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0001e490: 2020 203e 3e3e 2063 6f6f 7264 7320 3d20     >>> coords = 
+0001e4a0: 696d 672e 6365 6e74 726f 6964 5f73 6d28  img.centroid_sm(
+0001e4b0: 290d 0a20 2020 2020 2020 2020 2020 203e  )..            >
+0001e4c0: 3e3e 2069 6d67 2e73 7065 6369 6679 2863  >> img.specify(c
+0001e4d0: 6f6f 7264 732c 2033 2c20 6c61 6265 6c74  oords, 3, labelt
+0001e4e0: 7970 653d 2263 6972 636c 6522 290d 0a20  ype="circle").. 
+0001e4f0: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
+0001e500: 726f 7073 203d 2069 6d67 2e72 6567 696f  rops = img.regio
+0001e510: 6e70 726f 7073 2829 0d0a 2020 2020 2020  nprops()..      
+0001e520: 2020 2222 2220 2020 2020 2020 200d 0a20    """        .. 
+0001e530: 2020 2020 2020 2069 645f 6178 6973 203d         id_axis =
+0001e540: 2022 4e22 0d0a 2020 2020 2020 2020 6966   "N"..        if
+0001e550: 2069 7369 6e73 7461 6e63 6528 7072 6f70   isinstance(prop
+0001e560: 6572 7469 6573 2c20 7374 7229 3a0d 0a20  erties, str):.. 
+0001e570: 2020 2020 2020 2020 2020 2070 726f 7065             prope
+0001e580: 7274 6965 7320 3d20 2870 726f 7065 7274  rties = (propert
+0001e590: 6965 732c 290d 0a20 2020 2020 2020 2069  ies,)..        i
+0001e5a0: 6620 6578 7472 615f 7072 6f70 6572 7469  f extra_properti
+0001e5b0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0d  es is not None:.
+0001e5c0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0001e5d0: 7065 7274 6965 7320 3d20 7072 6f70 6572  perties = proper
+0001e5e0: 7469 6573 202b 2074 7570 6c65 2865 782e  ties + tuple(ex.
+0001e5f0: 5f5f 6e61 6d65 5f5f 2066 6f72 2065 7820  __name__ for ex 
+0001e600: 696e 2065 7874 7261 5f70 726f 7065 7274  in extra_propert
+0001e610: 6965 7329 0d0a 0d0a 2020 2020 2020 2020  ies)....        
+0001e620: 6966 2069 645f 6178 6973 2069 6e20 7365  if id_axis in se
+0001e630: 6c66 2e61 7865 733a 0d0a 2020 2020 2020  lf.axes:..      
+0001e640: 2020 2020 2020 2320 7468 6973 2064 696d        # this dim
+0001e650: 656e 7369 6f6e 2077 696c 6c20 6265 206c  ension will be l
+0001e660: 6162 656c 0d0a 2020 2020 2020 2020 2020  abel..          
+0001e670: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0001e680: 6f72 2866 2261 7869 7320 277b 6964 5f61  or(f"axis '{id_a
+0001e690: 7869 737d 2720 6973 2075 7365 6420 666f  xis}' is used fo
+0001e6a0: 7220 6c61 6265 6c20 4944 2069 6e20 4461  r label ID in Da
+0001e6b0: 7461 4672 616d 6573 2e22 290d 0a20 2020  taFrames.")..   
+0001e6c0: 2020 2020 200d 0a20 2020 2020 2020 2070       ..        p
+0001e6d0: 726f 705f 6178 6573 203d 2063 6f6d 706c  rop_axes = compl
+0001e6e0: 656d 656e 745f 6178 6573 2873 656c 662e  ement_axes(self.
+0001e6f0: 6c61 6265 6c73 2e61 7865 732c 2073 656c  labels.axes, sel
+0001e700: 662e 6178 6573 290d 0a20 2020 2020 2020  f.axes)..       
+0001e710: 2073 6861 7065 203d 2073 656c 662e 7369   shape = self.si
+0001e720: 7a65 736f 6628 7072 6f70 5f61 7865 7329  zesof(prop_axes)
+0001e730: 0d0a 0d0a 2020 2020 2020 2020 6f75 7420  ....        out 
+0001e740: 3d20 4461 7461 4469 6374 287b 703a 2050  = DataDict({p: P
+0001e750: 726f 7041 7272 6179 280d 0a20 2020 2020  ropArray(..     
+0001e760: 2020 2020 2020 2020 2020 206e 702e 656d             np.em
+0001e770: 7074 7928 2873 656c 662e 6c61 6265 6c73  pty((self.labels
+0001e780: 2e6d 6178 2829 2c29 202b 2073 6861 7065  .max(),) + shape
+0001e790: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+0001e7a0: 3332 292c 0d0a 2020 2020 2020 2020 2020  32),..          
+0001e7b0: 2020 2020 2020 6e61 6d65 3d73 656c 662e        name=self.
+0001e7c0: 6e61 6d65 2b22 2d70 726f 7022 2c20 0d0a  name+"-prop", ..
+0001e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7e0: 6178 6573 3d5b 6964 5f61 7869 735d 2b70  axes=[id_axis]+p
+0001e7f0: 726f 705f 6178 6573 2c0d 0a20 2020 2020  rop_axes,..     
+0001e800: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+0001e810: 653d 7365 6c66 2e73 6f75 7263 652c 0d0a  e=self.source,..
+0001e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e830: 7072 6f70 6e61 6d65 3d70 0d0a 2020 2020  propname=p..    
+0001e840: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0001e850: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001e860: 6f72 2070 2069 6e20 7072 6f70 6572 7469  or p in properti
+0001e870: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+0001e880: 7d29 0d0a 2020 2020 2020 2020 0d0a 2020  })..        ..  
+0001e890: 2020 2020 2020 2320 6361 6c63 756c 6174        # calculat
+0001e8a0: 6520 7072 6f70 6572 7479 2076 616c 7565  e property value
+0001e8b0: 2066 6f72 2065 6163 6820 736c 6963 650d   for each slice.
+0001e8c0: 0a20 2020 2020 2020 2066 6f72 2073 6c2c  .        for sl,
+0001e8d0: 2069 6d67 2069 6e20 7365 6c66 2e69 7465   img in self.ite
+0001e8e0: 7228 7072 6f70 5f61 7865 732c 2065 7863  r(prop_axes, exc
+0001e8f0: 6c75 6465 3d73 656c 662e 6c61 6265 6c73  lude=self.labels
+0001e900: 2e61 7865 7329 3a0d 0a20 2020 2020 2020  .axes):..       
+0001e910: 2020 2020 2070 726f 7073 203d 2073 6b6d       props = skm
+0001e920: 6573 2e72 6567 696f 6e70 726f 7073 2873  es.regionprops(s
+0001e930: 656c 662e 6c61 6265 6c73 2e76 616c 7565  elf.labels.value
+0001e940: 2c20 696d 672c 2063 6163 6865 3d46 616c  , img, cache=Fal
+0001e950: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+0001e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e970: 2020 2020 2020 2020 2020 2065 7874 7261             extra
+0001e980: 5f70 726f 7065 7274 6965 733d 6578 7472  _properties=extr
+0001e990: 615f 7072 6f70 6572 7469 6573 290d 0a20  a_properties).. 
+0001e9a0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0001e9b0: 5f73 6c20 3d20 2873 6c69 6365 284e 6f6e  _sl = (slice(Non
+0001e9c0: 6529 2c29 202b 2073 6c0d 0a20 2020 2020  e),) + sl..     
+0001e9d0: 2020 2020 2020 2066 6f72 2070 726f 705f         for prop_
+0001e9e0: 6e61 6d65 2069 6e20 7072 6f70 6572 7469  name in properti
+0001e9f0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+0001ea00: 2020 2020 2023 2042 6f74 6820 7369 6465       # Both side
+0001ea10: 7320 6861 7665 206c 656e 6774 6820 6f66  s have length of
+0001ea20: 2069 645f 6178 6973 2028 6e75 6d62 6572   id_axis (number
+0001ea30: 206f 6620 6c61 6265 6c73 2920 736f 2074   of labels) so t
+0001ea40: 6861 7420 7661 6c75 6573 0d0a 2020 2020  hat values..    
+0001ea50: 2020 2020 2020 2020 2020 2020 2320 6361              # ca
+0001ea60: 6e20 6265 2063 6f72 7265 6374 6c79 2073  n be correctly s
+0001ea70: 7562 7374 6974 7574 6564 2e0d 0a20 2020  ubstituted...   
+0001ea80: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001ea90: 5b70 726f 705f 6e61 6d65 5d5b 6c61 6265  [prop_name][labe
+0001eaa0: 6c5f 736c 5d20 3d20 5b67 6574 6174 7472  l_sl] = [getattr
+0001eab0: 2870 726f 702c 2070 726f 705f 6e61 6d65  (prop, prop_name
+0001eac0: 2920 666f 7220 7072 6f70 2069 6e20 7072  ) for prop in pr
+0001ead0: 6f70 735d 0d0a 2020 2020 2020 2020 0d0a  ops]..        ..
+0001eae0: 2020 2020 2020 2020 666f 7220 7061 7272          for parr
+0001eaf0: 2069 6e20 6f75 742e 7661 6c75 6573 2829   in out.values()
+0001eb00: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+0001eb10: 6172 722e 7365 745f 7363 616c 6528 7365  arr.set_scale(se
+0001eb20: 6c66 290d 0a20 2020 2020 2020 2072 6574  lf)..        ret
+0001eb30: 7572 6e20 6f75 740d 0a20 2020 200d 0a20  urn out..    .. 
+0001eb40: 2020 2040 5f64 6f63 732e 7772 6974 655f     @_docs.write_
+0001eb50: 646f 6373 0d0a 2020 2020 4064 696d 735f  docs..    @dims_
+0001eb60: 746f 5f73 7061 7469 616c 5f61 7865 730d  to_spatial_axes.
+0001eb70: 0a20 2020 2040 6368 6563 6b5f 696e 7075  .    @check_inpu
+0001eb80: 745f 616e 645f 6f75 7470 7574 0d0a 2020  t_and_output..  
+0001eb90: 2020 6465 6620 6c62 7028 0d0a 2020 2020    def lbp(..    
+0001eba0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0001ebb0: 2020 2070 3a20 696e 7420 3d20 3132 2c0d     p: int = 12,.
+0001ebc0: 0a20 2020 2020 2020 2072 6164 6975 733a  .        radius:
+0001ebd0: 2069 6e74 203d 2031 2c0d 0a20 2020 2020   int = 1,..     
+0001ebe0: 2020 202a 2c0d 0a20 2020 2020 2020 206d     *,..        m
+0001ebf0: 6574 686f 643a 204c 6974 6572 616c 5b22  ethod: Literal["
+0001ec00: 6465 6661 756c 7422 2c20 2272 6f72 222c  default", "ror",
+0001ec10: 2022 756e 6966 6f72 6d22 2c20 2276 6172   "uniform", "var
+0001ec20: 225d 203d 2022 6465 6661 756c 7422 2c0d  "] = "default",.
+0001ec30: 0a20 2020 2020 2020 2064 696d 733a 2044  .        dims: D
+0001ec40: 696d 7320 3d20 4e6f 6e65 2c0d 0a20 2020  ims = None,..   
+0001ec50: 2029 202d 3e20 496d 6741 7272 6179 3a0d   ) -> ImgArray:.
+0001ec60: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0001ec70: 2020 2020 2020 4c6f 6361 6c20 6269 6e61        Local bina
+0001ec80: 7279 2070 6174 7465 726e 2066 6561 7475  ry pattern featu
+0001ec90: 7265 2065 7874 7261 6374 696f 6e2e 0d0a  re extraction...
+0001eca0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0001ecb0: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+0001ecc0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+0001ecd0: 2020 7020 3a20 696e 742c 2064 6566 6175    p : int, defau
+0001ece0: 6c74 2069 7320 3132 0d0a 2020 2020 2020  lt is 12..      
+0001ecf0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+0001ed00: 6369 7263 756c 6172 206e 6569 6768 626f  circular neighbo
+0001ed10: 7273 0d0a 2020 2020 2020 2020 7261 6469  rs..        radi
+0001ed20: 7573 203a 2069 6e74 2c20 6465 6661 756c  us : int, defaul
+0001ed30: 7420 6973 2031 0d0a 2020 2020 2020 2020  t is 1..        
+0001ed40: 2020 2020 5261 6469 7573 206f 6620 6e65      Radius of ne
+0001ed50: 6967 6862 6f75 7273 2e0d 0a20 2020 2020  ighbours...     
+0001ed60: 2020 206d 6574 686f 6420 3a20 7374 722c     method : str,
+0001ed70: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+0001ed80: 2020 2020 2020 204d 6574 686f 6420 746f         Method to
+0001ed90: 2064 6574 6572 6d69 6e65 6420 7468 6520   determined the 
+0001eda0: 7061 7474 6572 6e2e 0d0a 2020 2020 2020  pattern...      
+0001edb0: 2020 7b64 696d 737d 0d0a 0d0a 2020 2020    {dims}....    
+0001edc0: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+0001edd0: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+0001ede0: 2020 2020 2020 496d 6741 7272 6179 0d0a        ImgArray..
+0001edf0: 2020 2020 2020 2020 2020 2020 4c6f 6361              Loca
+0001ee00: 6c20 6269 6e61 7279 2070 6174 7465 726e  l binary pattern
+0001ee10: 2069 6d61 6765 2e0d 0a20 2020 2020 2020   image...       
+0001ee20: 2022 2222 2020 2020 2020 2020 0d0a 2020   """        ..  
+0001ee30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001ee40: 7265 7475 726e 2073 656c 662e 5f61 7070  return self._app
+0001ee50: 6c79 5f64 6173 6b28 0d0a 2020 2020 2020  ly_dask(..      
+0001ee60: 2020 2020 2020 736b 6665 6174 2e6c 6f63        skfeat.loc
+0001ee70: 616c 5f62 696e 6172 795f 7061 7474 6572  al_binary_patter
+0001ee80: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
+0001ee90: 635f 6178 6573 3d63 6f6d 706c 656d 656e  c_axes=complemen
+0001eea0: 745f 6178 6573 2864 696d 7329 2c20 0d0a  t_axes(dims), ..
+0001eeb0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0001eec0: 3d28 702c 2072 6164 6975 732c 206d 6574  =(p, radius, met
+0001eed0: 686f 6429 0d0a 2020 2020 2020 2020 290d  hod)..        ).
+0001eee0: 0a20 2020 2020 2020 200d 0a20 2020 2040  .        ..    @
+0001eef0: 5f64 6f63 732e 7772 6974 655f 646f 6373  _docs.write_docs
+0001ef00: 0d0a 2020 2020 4064 696d 735f 746f 5f73  ..    @dims_to_s
+0001ef10: 7061 7469 616c 5f61 7865 730d 0a20 2020  patial_axes..   
+0001ef20: 2040 6368 6563 6b5f 696e 7075 745f 616e   @check_input_an
+0001ef30: 645f 6f75 7470 7574 0d0a 2020 2020 6465  d_output..    de
+0001ef40: 6620 676c 636d 5f70 726f 7073 2873 656c  f glcm_props(sel
+0001ef50: 662c 2064 6973 7461 6e63 6573 2c20 616e  f, distances, an
+0001ef60: 676c 6573 2c20 7261 6469 7573 3a69 6e74  gles, radius:int
+0001ef70: 2c20 7072 6f70 6572 7469 6573 3a74 7570  , properties:tup
+0001ef80: 6c65 3d4e 6f6e 652c 200d 0a20 2020 2020  le=None, ..     
+0001ef90: 2020 2020 2020 2020 2020 2020 2020 2a2c                *,
+0001efa0: 2062 696e 733a 696e 743d 4e6f 6e65 2c20   bins:int=None, 
+0001efb0: 7265 7363 616c 655f 6d61 783a 626f 6f6c  rescale_max:bool
+0001efc0: 3d46 616c 7365 2c20 6469 6d73 3a20 4469  =False, dims: Di
+0001efd0: 6d73 203d 204e 6f6e 6529 202d 3e20 496d  ms = None) -> Im
+0001efe0: 6741 7272 6179 3a0d 0a20 2020 2020 2020  gArray:..       
+0001eff0: 2022 2222 0d0a 2020 2020 2020 2020 436f   """..        Co
+0001f000: 6d70 7574 6520 7072 6f70 6572 7469 6573  mpute properties
+0001f010: 206f 6620 2247 7261 7920 4c65 7665 6c20   of "Gray Level 
+0001f020: 436f 6f63 7572 7265 6e63 6520 4d61 7472  Coocurrence Matr
+0001f030: 6978 222e 2054 6869 7320 7769 6c6c 2074  ix". This will t
+0001f040: 616b 6520 6c6f 6e67 2074 696d 650d 0a20  ake long time.. 
+0001f050: 2020 2020 2020 2062 6563 6175 7365 206f         because o
+0001f060: 6620 7075 7265 2050 7974 686f 6e20 666f  f pure Python fo
+0001f070: 722d 6c6f 6f70 2e0d 0a0d 0a20 2020 2020  r-loop.....     
+0001f080: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+0001f090: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001f0a0: 2d0d 0a20 2020 2020 2020 2064 6973 7461  -..        dista
+0001f0b0: 6e63 6573 203a 2061 7272 6179 5f6c 696b  nces : array_lik
+0001f0c0: 650d 0a20 2020 2020 2020 2020 2020 204c  e..            L
+0001f0d0: 6973 7420 6f66 2070 6978 656c 2070 6169  ist of pixel pai
+0001f0e0: 7220 6469 7374 616e 6365 206f 6666 7365  r distance offse
+0001f0f0: 7473 2e0d 0a20 2020 2020 2020 2061 6e67  ts...        ang
+0001f100: 6c65 7320 3a20 6172 7261 795f 6c69 6b65  les : array_like
+0001f110: 0d0a 2020 2020 2020 2020 2020 2020 4c69  ..            Li
+0001f120: 7374 206f 6620 7069 7865 6c20 7061 6972  st of pixel pair
+0001f130: 2061 6e67 6c65 7320 696e 2072 6164 6961   angles in radia
+0001f140: 6e73 2e0d 0a20 2020 2020 2020 2072 6164  ns...        rad
+0001f150: 6975 7320 3a20 696e 740d 0a20 2020 2020  ius : int..     
+0001f160: 2020 2020 2020 2057 696e 646f 7720 7261         Window ra
+0001f170: 6469 7573 2e0d 0a20 2020 2020 2020 2070  dius...        p
+0001f180: 726f 7065 7274 6965 7320 3a20 7475 706c  roperties : tupl
+0001f190: 6520 6f66 2073 7472 0d0a 2020 2020 2020  e of str..      
+0001f1a0: 2020 2020 2020 636f 6e74 7261 7374 2c20        contrast, 
+0001f1b0: 6469 7373 696d 696c 6172 6974 792c 2068  dissimilarity, h
+0001f1c0: 6f6d 6f67 656e 6569 7479 2c20 656e 6572  omogeneity, ener
+0001f1d0: 6779 2c20 6d65 616e 2c20 7374 642c 2061  gy, mean, std, a
+0001f1e0: 736d 2c20 6d61 782c 2065 6e74 726f 7079  sm, max, entropy
+0001f1f0: 0d0a 2020 2020 2020 2020 6269 6e73 203a  ..        bins :
+0001f200: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
+0001f210: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
+0001f220: 6572 206f 6620 6269 6e73 2e0d 0a20 2020  er of bins...   
+0001f230: 2020 2020 2072 6573 6361 6c65 5f6d 6178       rescale_max
+0001f240: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0001f250: 2069 7320 4661 6c73 650d 0a20 2020 2020   is False..     
+0001f260: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+0001f270: 7468 6520 636f 6e74 7261 7374 206f 6620  the contrast of 
+0001f280: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
+0001f290: 6973 206d 6178 696d 697a 6564 2062 7920  is maximized by 
+0001f2a0: 6d75 6c74 6970 6c79 696e 6720 616e 2069  multiplying an i
+0001f2b0: 6e74 6567 6572 2e0d 0a20 2020 2020 2020  nteger...       
+0001f2c0: 207b 6469 6d73 7d0d 0a0d 0a20 2020 2020   {dims}....     
+0001f2d0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+0001f2e0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+0001f2f0: 2020 2020 2044 6174 6144 6963 7420 6f66       DataDict of
+0001f300: 2049 6d67 4172 7261 790d 0a20 2020 2020   ImgArray..     
+0001f310: 2020 2020 2020 2047 4c43 4d20 7769 7468         GLCM with
+0001f320: 2061 6464 6974 696f 6e61 6c20 6178 6573   additional axes
+0001f330: 2022 6461 222c 2077 6865 7265 2022 6422   "da", where "d"
+0001f340: 206d 6561 6e73 2064 6973 7461 6e63 6520   means distance 
+0001f350: 616e 6420 2261 2220 6d65 616e 7320 616e  and "a" means an
+0001f360: 676c 652e 0d0a 2020 2020 2020 2020 2020  gle...          
+0001f370: 2020 4966 2069 6e70 7574 2069 6d61 6765    If input image
+0001f380: 2068 6173 2022 747a 7978 2220 6178 6573   has "tzyx" axes
+0001f390: 2074 6865 6e20 6f75 7470 7574 2077 696c   then output wil
+0001f3a0: 6c20 6861 7665 2022 747a 643c 7978 2220  l have "tzd<yx" 
+0001f3b0: 6178 6573 2e0d 0a20 2020 2020 2020 200d  axes...        .
+0001f3c0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+0001f3d0: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0001f3e0: 2d2d 2d0d 0a20 2020 2020 2020 2050 6c6f  ---..        Plo
+0001f3f0: 7420 474c 434d 2773 2049 444d 2061 6e64  t GLCM's IDM and
+0001f400: 2041 534d 2069 6d61 6765 730d 0a20 2020   ASM images..   
+0001f410: 2020 2020 2020 2020 203e 3e3e 206f 7574           >>> out
+0001f420: 203d 2069 6d67 2e67 6c63 6d5f 7072 6f70   = img.glcm_prop
+0001f430: 7328 5b31 5d2c 205b 305d 2c20 332c 2070  s([1], [0], 3, p
+0001f440: 726f 7065 7274 6965 733d 2822 6964 6d22  roperties=("idm"
+0001f450: 2c22 6173 6d22 2929 0d0a 2020 2020 2020  ,"asm"))..      
+0001f460: 2020 2020 2020 3e3e 3e20 6f75 742e 6964        >>> out.id
+0001f470: 6d5b 2264 3d30 3b3c 3d30 225d 2e69 6d73  m["d=0;<=0"].ims
+0001f480: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
+0001f490: 2020 203e 3e3e 206f 7574 2e61 736d 5b22     >>> out.asm["
+0001f4a0: 643d 303b 3c3d 3022 5d2e 696d 7368 6f77  d=0;<=0"].imshow
+0001f4b0: 2829 0d0a 2020 2020 2020 2020 2222 2220  ()..        """ 
+0001f4c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001f4d0: 2073 656c 662c 2062 696e 732c 2072 6573   self, bins, res
+0001f4e0: 6361 6c65 5f6d 6178 203d 205f 676c 636d  cale_max = _glcm
+0001f4f0: 2e63 6865 636b 5f67 6c63 6d28 7365 6c66  .check_glcm(self
+0001f500: 2c20 6269 6e73 2c20 7265 7363 616c 655f  , bins, rescale_
+0001f510: 6d61 7829 0d0a 2020 2020 2020 2020 6966  max)..        if
+0001f520: 2070 726f 7065 7274 6965 7320 6973 204e   properties is N
+0001f530: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0001f540: 2020 7072 6f70 6572 7469 6573 203d 2028    properties = (
+0001f550: 2263 6f6e 7472 6173 7422 2c20 2264 6973  "contrast", "dis
+0001f560: 7369 6d69 6c61 7269 7479 222c 2022 6964  similarity", "id
+0001f570: 6d22 2c20 0d0a 2020 2020 2020 2020 2020  m", ..          
+0001f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f590: 2261 736d 222c 2022 6d61 7822 2c20 2265  "asm", "max", "e
+0001f5a0: 6e74 726f 7079 222c 2022 636f 7272 656c  ntropy", "correl
+0001f5b0: 6174 696f 6e22 290d 0a20 2020 2020 2020  ation")..       
+0001f5c0: 2063 5f61 7865 7320 3d20 636f 6d70 6c65   c_axes = comple
+0001f5d0: 6d65 6e74 5f61 7865 7328 6469 6d73 2c20  ment_axes(dims, 
+0001f5e0: 7365 6c66 2e61 7865 7329 0d0a 2020 2020  self.axes)..    
+0001f5f0: 2020 2020 6469 7374 616e 6365 7320 3d20      distances = 
+0001f600: 6e70 2e61 7361 7272 6179 2864 6973 7461  np.asarray(dista
+0001f610: 6e63 6573 2c20 6474 7970 653d 6e70 2e75  nces, dtype=np.u
+0001f620: 696e 7438 290d 0a20 2020 2020 2020 2061  int8)..        a
+0001f630: 6e67 6c65 7320 3d20 6e70 2e61 7361 7272  ngles = np.asarr
+0001f640: 6179 2861 6e67 6c65 732c 2064 7479 7065  ay(angles, dtype
+0001f650: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+0001f660: 2020 2020 2020 6f75 7473 6861 7065 203d        outshape =
+0001f670: 2073 656c 662e 7369 7a65 736f 6628 635f   self.sizesof(c_
+0001f680: 6178 6573 2920 2b20 286c 656e 2864 6973  axes) + (len(dis
+0001f690: 7461 6e63 6573 292c 206c 656e 2861 6e67  tances), len(ang
+0001f6a0: 6c65 7329 2920 2b20 7365 6c66 2e73 697a  les)) + self.siz
+0001f6b0: 6573 6f66 2864 696d 7329 0d0a 2020 2020  esof(dims)..    
+0001f6c0: 2020 2020 6f75 7420 3d20 7b7d 0d0a 2020      out = {}..  
+0001f6d0: 2020 2020 2020 666f 7220 7072 6f70 2069        for prop i
+0001f6e0: 6e20 7072 6f70 6572 7469 6573 3a0d 0a20  n properties:.. 
+0001f6f0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0001f700: 696e 7374 616e 6365 2870 726f 702c 2073  instance(prop, s
+0001f710: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
+0001f720: 2020 2020 2020 6f75 745b 7072 6f70 5d20        out[prop] 
+0001f730: 3d20 6e70 2e65 6d70 7479 286f 7574 7368  = np.empty(outsh
+0001f740: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
+0001f750: 6f61 7433 3229 2e76 6965 7728 7365 6c66  oat32).view(self
+0001f760: 2e5f 5f63 6c61 7373 5f5f 290d 0a20 2020  .__class__)..   
+0001f770: 2020 2020 2020 2020 2065 6c69 6620 6361           elif ca
+0001f780: 6c6c 6162 6c65 2870 726f 7029 3a0d 0a20  llable(prop):.. 
+0001f790: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001f7a0: 7574 5b70 726f 702e 5f5f 6e61 6d65 5f5f  ut[prop.__name__
+0001f7b0: 5d20 3d20 6e70 2e65 6d70 7479 286f 7574  ] = np.empty(out
+0001f7c0: 7368 6170 652c 2064 7479 7065 3d6e 702e  shape, dtype=np.
+0001f7d0: 666c 6f61 7433 3229 2e76 6965 7728 7365  float32).view(se
+0001f7e0: 6c66 2e5f 5f63 6c61 7373 5f5f 290d 0a20  lf.__class__).. 
+0001f7f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001f800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f810: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+0001f820: 7228 2270 726f 7065 7274 6965 7320 6d75  r("properties mu
+0001f830: 7374 2062 6520 7374 7220 6f72 2063 616c  st be str or cal
+0001f840: 6c61 626c 652e 2229 0d0a 2020 2020 2020  lable.")..      
+0001f850: 2020 6f75 7420 3d20 4461 7461 4469 6374    out = DataDict
+0001f860: 286f 7574 290d 0a20 2020 2020 2020 2073  (out)..        s
+0001f870: 656c 6620 3d20 7365 6c66 2e70 6164 2872  elf = self.pad(r
+0001f880: 6164 6975 732c 206d 6f64 653d 2272 6566  adius, mode="ref
+0001f890: 6c65 6374 222c 2064 696d 733d 6469 6d73  lect", dims=dims
+0001f8a0: 290d 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
+0001f8b0: 6c2c 2069 6d67 2069 6e20 7365 6c66 2e69  l, img in self.i
+0001f8c0: 7465 7228 635f 6178 6573 293a 0d0a 2020  ter(c_axes):..  
+0001f8d0: 2020 2020 2020 2020 2020 7072 6f70 6f75            propou
+0001f8e0: 7420 3d20 5f67 6c63 6d2e 676c 636d 5f70  t = _glcm.glcm_p
+0001f8f0: 726f 7073 5f28 696d 672c 2064 6973 7461  rops_(img, dista
+0001f900: 6e63 6573 2c20 616e 676c 6573 2c20 6269  nces, angles, bi
+0001f910: 6e73 2c20 7261 6469 7573 2c20 7072 6f70  ns, radius, prop
+0001f920: 6572 7469 6573 290d 0a20 2020 2020 2020  erties)..       
+0001f930: 2020 2020 2066 6f72 2070 726f 7020 696e       for prop in
+0001f940: 2070 726f 7065 7274 6965 733a 0d0a 2020   properties:..  
+0001f950: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+0001f960: 745b 7072 6f70 5d2e 7661 6c75 655b 736c  t[prop].value[sl
+0001f970: 5d20 3d20 7072 6f70 6f75 745b 7072 6f70  ] = propout[prop
+0001f980: 5d0d 0a20 2020 2020 2020 2020 2020 200d  ]..            .
+0001f990: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
+0001f9a0: 7620 696e 206f 7574 2e69 7465 6d73 2829  v in out.items()
+0001f9b0: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
+0001f9c0: 2e5f 7365 745f 696e 666f 2873 656c 662c  ._set_info(self,
+0001f9d0: 206e 6577 5f61 7865 733d 635f 6178 6573   new_axes=c_axes
+0001f9e0: 2b22 6461 222b 6469 6d73 290d 0a20 2020  +"da"+dims)..   
+0001f9f0: 2020 2020 2072 6574 7572 6e20 6f75 740d       return out.
+0001fa00: 0a20 2020 200d 0a20 2020 200d 0a20 2020  .    ..    ..   
+0001fa10: 2040 7361 6d65 5f64 7479 7065 0d0a 2020   @same_dtype..  
+0001fa20: 2020 6465 6620 7072 6f6a 280d 0a20 2020    def proj(..   
+0001fa30: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+0001fa40: 2020 2020 6178 6973 3a20 4178 6973 4c69      axis: AxisLi
+0001fa50: 6b65 207c 204e 6f6e 6520 3d20 4e6f 6e65  ke | None = None
+0001fa60: 2c0d 0a20 2020 2020 2020 206d 6574 686f  ,..        metho
+0001fa70: 643a 2073 7472 207c 2043 616c 6c61 626c  d: str | Callabl
+0001fa80: 6520 3d20 226d 6561 6e22 2c0d 0a20 2020  e = "mean",..   
+0001fa90: 2020 2020 206d 6173 6b20 3d20 4e6f 6e65       mask = None
+0001faa0: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
+0001fab0: 7267 730d 0a20 2020 2029 202d 3e20 496d  rgs..    ) -> Im
+0001fac0: 6741 7272 6179 3a0d 0a20 2020 2020 2020  gArray:..       
+0001fad0: 2022 2222 0d0a 2020 2020 2020 2020 5072   """..        Pr
+0001fae0: 6f6a 6563 7469 6f6e 2061 6c6f 6e67 2061  ojection along a
+0001faf0: 6e79 2061 7869 732e 0d0a 0d0a 2020 2020  ny axis.....    
+0001fb00: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+0001fb10: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0001fb20: 2d2d 0d0a 2020 2020 2020 2020 6178 6973  --..        axis
+0001fb30: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+0001fb40: 0d0a 2020 2020 2020 2020 2020 2020 416c  ..            Al
+0001fb50: 6f6e 6720 7768 6963 6820 6178 6973 2070  ong which axis p
+0001fb60: 726f 6a65 6374 696f 6e20 7769 6c6c 2062  rojection will b
+0001fb70: 6520 6361 6c63 756c 6174 6564 2e20 4966  e calculated. If
+0001fb80: 204e 6f6e 652c 206d 6f73 7420 706c 6175   None, most plau
+0001fb90: 7369 626c 6520 6f6e 6520 7769 6c6c 2062  sible one will b
+0001fba0: 6520 6368 6f73 656e 2e0d 0a20 2020 2020  e chosen...     
+0001fbb0: 2020 206d 6574 686f 6420 3a20 7374 7220     method : str 
+0001fbc0: 6f72 2063 616c 6c61 626c 652c 2064 6566  or callable, def
+0001fbd0: 6175 6c74 2069 7320 6d65 616e 2d70 726f  ault is mean-pro
+0001fbe0: 6a65 6374 696f 6e2e 0d0a 2020 2020 2020  jection...      
+0001fbf0: 2020 2020 2020 5072 6f6a 6563 7469 6f6e        Projection
+0001fc00: 206d 6574 686f 642e 2049 6620 7374 7220   method. If str 
+0001fc10: 6973 2067 6976 656e 2c20 6974 2077 696c  is given, it wil
+0001fc20: 6c20 636f 6e76 6572 7465 6420 746f 206e  l converted to n
+0001fc30: 756d 7079 2066 756e 6374 696f 6e2e 0d0a  umpy function...
+0001fc40: 2020 2020 2020 2020 6d61 736b 203a 2061          mask : a
+0001fc50: 7272 6179 2d6c 696b 652c 206f 7074 696f  rray-like, optio
+0001fc60: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+0001fc70: 2049 6620 7072 6f76 6964 6564 2c20 696e   If provided, in
+0001fc80: 7075 7420 696d 6167 6520 7769 6c6c 2062  put image will b
+0001fc90: 6520 636f 6e76 6572 7465 6420 746f 206e  e converted to n
+0001fca0: 702e 6d61 2e61 7272 6179 2061 6e64 2060  p.ma.array and `
+0001fcb0: 606d 6574 686f 6460 6020 7769 6c6c 2061  `method`` will a
+0001fcc0: 6c73 6f20 6265 2069 6e74 6572 7072 6574  lso be interpret
+0001fcd0: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+0001fce0: 6173 2061 6e20 6d61 736b 6564 2066 756e  as an masked fun
+0001fcf0: 6374 696f 2069 6620 706f 7373 6962 6c65  ctio if possible
+0001fd00: 2e0d 0a20 2020 2020 2020 202a 2a6b 7761  ...        **kwa
+0001fd10: 7267 730d 0a20 2020 2020 2020 2020 2020  rgs..           
+0001fd20: 204f 7468 6572 206b 6579 776f 7264 2061   Other keyword a
+0001fd30: 7267 756d 656e 7473 2074 6861 7420 7769  rguments that wi
+0001fd40: 6c6c 2070 6173 7365 6420 746f 2070 726f  ll passed to pro
+0001fd50: 6a65 6374 696f 6e20 6675 6e63 7469 6f6e  jection function
+0001fd60: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+0001fd70: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+0001fd80: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
+0001fd90: 6d67 4172 7261 790d 0a20 2020 2020 2020  mgArray..       
+0001fda0: 2020 2020 2050 726f 6a65 6374 6564 2069       Projected i
+0001fdb0: 6d61 6765 2e0d 0a20 2020 2020 2020 2022  mage...        "
+0001fdc0: 2222 2020 2020 2020 2020 0d0a 2020 2020  ""        ..    
+0001fdd0: 2020 2020 2320 6465 7465 726d 696e 6520      # determine 
+0001fde0: 6675 6e63 7469 6f6e 0d0a 2020 2020 2020  function..      
+0001fdf0: 2020 6966 206d 6173 6b20 6973 206e 6f74    if mask is not
+0001fe00: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0001fe10: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0001fe20: 6528 6d65 7468 6f64 2c20 7374 7229 3a0d  e(method, str):.
+0001fe30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe40: 2066 756e 6320 3d20 6765 7461 7474 7228   func = getattr(
+0001fe50: 6e70 2e6d 612c 206d 6574 686f 6429 0d0a  np.ma, method)..
+0001fe60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001fe70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001fe80: 2020 2066 756e 6320 3d20 6d65 7468 6f64     func = method
+0001fe90: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0001fea0: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
+0001feb0: 6320 3d20 5f63 6865 636b 5f66 756e 6374  c = _check_funct
+0001fec0: 696f 6e28 6d65 7468 6f64 290d 0a20 2020  ion(method)..   
+0001fed0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+0001fee0: 6620 6178 6973 2069 7320 4e6f 6e65 3a0d  f axis is None:.
+0001fef0: 0a20 2020 2020 2020 2020 2020 2061 7869  .            axi
+0001ff00: 7320 3d20 6669 6e64 5f66 6972 7374 5f61  s = find_first_a
+0001ff10: 7070 6561 7265 6428 227a 7470 6961 6322  ppeared("ztpiac"
+0001ff20: 2c20 696e 636c 7564 653d 7365 6c66 2e61  , include=self.a
+0001ff30: 7865 732c 2065 7863 6c75 6465 3d22 7978  xes, exclude="yx
+0001ff40: 2229 0d0a 2020 2020 2020 2020 656c 6966  ")..        elif
+0001ff50: 206e 6f74 2068 6173 6174 7472 2861 7869   not hasattr(axi
+0001ff60: 732c 2022 5f5f 6974 6572 5f5f 2229 3a0d  s, "__iter__"):.
+0001ff70: 0a20 2020 2020 2020 2020 2020 2061 7869  .            axi
+0001ff80: 7320 3d20 5b61 7869 735d 0d0a 2020 2020  s = [axis]..    
+0001ff90: 2020 2020 6178 6973 696e 7420 3d20 7475      axisint = tu
+0001ffa0: 706c 6528 7365 6c66 2e61 7869 736f 6628  ple(self.axisof(
+0001ffb0: 6129 2066 6f72 2061 2069 6e20 6178 6973  a) for a in axis
+0001ffc0: 290d 0a20 2020 2020 2020 2069 6620 6675  )..        if fu
+0001ffd0: 6e63 2e5f 5f6d 6f64 756c 655f 5f20 3d3d  nc.__module__ ==
+0001ffe0: 2022 6e75 6d70 792e 6d61 2e63 6f72 6522   "numpy.ma.core"
+0001fff0: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
+00020000: 7272 203d 206e 702e 6d61 2e61 7272 6179  rr = np.ma.array
+00020010: 2873 656c 662e 7661 6c75 652c 206d 6173  (self.value, mas
+00020020: 6b3d 6d61 736b 2c20 6474 7970 653d 7365  k=mask, dtype=se
+00020030: 6c66 2e64 7479 7065 290d 0a20 2020 2020  lf.dtype)..     
+00020040: 2020 2020 2020 2069 6620 6675 6e63 2069         if func i
+00020050: 7320 6e70 2e6d 612e 6d65 616e 3a0d 0a20  s np.ma.mean:.. 
+00020060: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00020070: 7574 203d 2066 756e 6328 6172 722c 2061  ut = func(arr, a
+00020080: 7869 733d 6178 6973 696e 742c 2064 7479  xis=axisint, dty
+00020090: 7065 3d6e 702e 666c 6f61 7433 322c 202a  pe=np.float32, *
+000200a0: 2a6b 7761 7267 7329 0d0a 2020 2020 2020  *kwargs)..      
+000200b0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000200c0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+000200d0: 203d 2066 756e 6328 6172 722c 2061 7869   = func(arr, axi
+000200e0: 733d 6178 6973 696e 742c 202a 2a6b 7761  s=axisint, **kwa
+000200f0: 7267 7329 0d0a 2020 2020 2020 2020 656c  rgs)..        el
+00020100: 6966 2066 756e 6320 6973 206e 702e 6d65  if func is np.me
+00020110: 616e 3a0d 0a20 2020 2020 2020 2020 2020  an:..           
+00020120: 206f 7574 203d 2066 756e 6328 7365 6c66   out = func(self
+00020130: 2e76 616c 7565 2c20 6178 6973 3d61 7869  .value, axis=axi
+00020140: 7369 6e74 2c20 6474 7970 653d 6e70 2e66  sint, dtype=np.f
+00020150: 6c6f 6174 3332 2c20 2a2a 6b77 6172 6773  loat32, **kwargs
+00020160: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00020170: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+00020180: 7420 3d20 6675 6e63 2873 656c 662e 7661  t = func(self.va
+00020190: 6c75 652c 2061 7869 733d 6178 6973 696e  lue, axis=axisin
+000201a0: 742c 202a 2a6b 7761 7267 7329 0d0a 2020  t, **kwargs)..  
+000201b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000201c0: 6f75 7420 3d20 6f75 742e 7669 6577 2873  out = out.view(s
+000201d0: 656c 662e 5f5f 636c 6173 735f 5f29 0d0a  elf.__class__)..
+000201e0: 2020 2020 2020 2020 6f75 742e 5f73 6574          out._set
+000201f0: 5f69 6e66 6f28 7365 6c66 2c20 7365 6c66  _info(self, self
+00020200: 2e61 7865 732e 6472 6f70 2861 7869 7369  .axes.drop(axisi
+00020210: 6e74 2929 0d0a 2020 2020 2020 2020 7265  nt))..        re
+00020220: 7475 726e 206f 7574 0d0a 0d0a 2020 2020  turn out....    
+00020230: 4063 6865 636b 5f69 6e70 7574 5f61 6e64  @check_input_and
+00020240: 5f6f 7574 7075 740d 0a20 2020 2064 6566  _output..    def
+00020250: 2063 6c69 7028 7365 6c66 2c20 696e 5f72   clip(self, in_r
+00020260: 616e 6765 3a20 7475 706c 655b 696e 7420  ange: tuple[int 
+00020270: 7c20 7374 722c 2069 6e74 207c 2073 7472  | str, int | str
+00020280: 5d20 3d20 2822 3025 222c 2022 3130 3025  ] = ("0%", "100%
+00020290: 2229 2920 2d3e 2049 6d67 4172 7261 793a  ")) -> ImgArray:
+000202a0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000202b0: 2020 2020 2020 2053 6174 7572 6174 6520         Saturate 
+000202c0: 6c6f 772f 6869 6768 2069 6e74 656e 7369  low/high intensi
+000202d0: 7479 2075 7369 6e67 206e 702e 636c 6970  ty using np.clip
+000202e0: 2829 2e0d 0a0d 0a20 2020 2020 2020 2050  ().....        P
+000202f0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00020300: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00020310: 2020 2020 2020 2069 6e5f 7261 6e67 6520         in_range 
+00020320: 3a20 7477 6f20 7363 616c 6172 2076 616c  : two scalar val
+00020330: 7565 732c 206f 7074 696f 6e61 6c0d 0a20  ues, optional.. 
+00020340: 2020 2020 2020 2020 2020 2072 616e 6765             range
+00020350: 206f 6620 6c6f 7765 722f 7570 7065 7220   of lower/upper 
+00020360: 6c69 6d69 7473 2c20 6279 2064 6566 6175  limits, by defau
+00020370: 6c74 2028 3025 2c20 3130 3025 292e 0d0a  lt (0%, 100%)...
+00020380: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00020390: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+000203a0: 2d2d 0d0a 2020 2020 2020 2020 496d 6741  --..        ImgA
+000203b0: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
+000203c0: 2020 436c 6970 7065 6420 696d 6167 6520    Clipped image 
+000203d0: 7769 7468 2074 656d 706f 7261 6c20 6174  with temporal at
+000203e0: 7472 6962 7574 650d 0a20 2020 2020 2020  tribute..       
+000203f0: 2022 2222 2020 2020 2020 2020 0d0a 2020   """        ..  
+00020400: 2020 2020 2020 6c6f 7765 726c 696d 2c20        lowerlim, 
+00020410: 7570 7065 726c 696d 203d 205f 6368 6563  upperlim = _chec
+00020420: 6b5f 636c 6970 5f72 616e 6765 2869 6e5f  k_clip_range(in_
+00020430: 7261 6e67 652c 2073 656c 662e 7661 6c75  range, self.valu
+00020440: 6529 0d0a 2020 2020 2020 2020 6f75 7420  e)..        out 
+00020450: 3d20 6e70 2e63 6c69 7028 7365 6c66 2e76  = np.clip(self.v
+00020460: 616c 7565 2c20 6c6f 7765 726c 696d 2c20  alue, lowerlim, 
+00020470: 7570 7065 726c 696d 290d 0a20 2020 2020  upperlim)..     
+00020480: 2020 206f 7574 203d 206f 7574 2e76 6965     out = out.vie
+00020490: 7728 7365 6c66 2e5f 5f63 6c61 7373 5f5f  w(self.__class__
+000204a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000204b0: 6e20 6f75 740d 0a20 2020 200d 0a20 2020  n out..    ..   
+000204c0: 2040 6368 6563 6b5f 696e 7075 745f 616e   @check_input_an
+000204d0: 645f 6f75 7470 7574 0d0a 2020 2020 6465  d_output..    de
+000204e0: 6620 7265 7363 616c 655f 696e 7465 6e73  f rescale_intens
+000204f0: 6974 7928 0d0a 2020 2020 2020 2020 7365  ity(..        se
+00020500: 6c66 2c0d 0a20 2020 2020 2020 2069 6e5f  lf,..        in_
+00020510: 7261 6e67 653a 2074 7570 6c65 5b69 6e74  range: tuple[int
+00020520: 207c 2073 7472 2c20 696e 7420 7c20 7374   | str, int | st
+00020530: 725d 203d 2028 2230 2522 2c20 2231 3030  r] = ("0%", "100
+00020540: 2522 292c 200d 0a20 2020 2020 2020 2064  %"), ..        d
+00020550: 7479 7065 203d 206e 702e 7569 6e74 3136  type = np.uint16
+00020560: 0d0a 2020 2020 2920 2d3e 2049 6d67 4172  ..    ) -> ImgAr
+00020570: 7261 793a 0d0a 2020 2020 2020 2020 2222  ray:..        ""
+00020580: 220d 0a20 2020 2020 2020 2052 6573 6361  "..        Resca
+00020590: 6c65 2074 6865 2069 6e74 656e 7369 7479  le the intensity
+000205a0: 206f 6620 7468 6520 696d 6167 6520 7573   of the image us
+000205b0: 696e 6720 736b 696d 6167 652e 6578 706f  ing skimage.expo
+000205c0: 7375 7265 2e72 6573 6361 6c65 5f69 6e74  sure.rescale_int
+000205d0: 656e 7369 7479 2829 2e0d 0a0d 0a20 2020  ensity().....   
+000205e0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+000205f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00020600: 2d2d 2d0d 0a20 2020 2020 2020 2069 6e5f  ---..        in_
+00020610: 7261 6e67 6520 3a20 7477 6f20 7363 616c  range : two scal
+00020620: 6172 2076 616c 7565 732c 2064 6566 6175  ar values, defau
+00020630: 6c74 2069 7320 2830 252c 2031 3030 2529  lt is (0%, 100%)
+00020640: 0d0a 2020 2020 2020 2020 2020 2020 5261  ..            Ra
+00020650: 6e67 6520 6f66 206c 6f77 6572 2f75 7070  nge of lower/upp
+00020660: 6572 206c 696d 6974 2e0d 0a20 2020 2020  er limit...     
+00020670: 2020 2064 7479 7065 203a 206e 756d 7079     dtype : numpy
+00020680: 2064 7479 7065 2c20 6465 6661 756c 7420   dtype, default 
+00020690: 6973 206e 702e 7569 6e74 3136 0d0a 2020  is np.uint16..  
+000206a0: 2020 2020 2020 2020 2020 4f75 7470 7574            Output
+000206b0: 2064 7479 7065 2e0d 0a0d 0a20 2020 2020   dtype.....     
+000206c0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+000206d0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+000206e0: 2020 2020 2049 6d67 4172 7261 790d 0a20       ImgArray.. 
+000206f0: 2020 2020 2020 2020 2020 2052 6573 6361             Resca
+00020700: 6c65 6420 696d 6167 6520 7769 7468 2074  led image with t
+00020710: 656d 706f 7261 6c20 6174 7472 6962 7574  emporal attribut
+00020720: 650d 0a20 2020 2020 2020 2022 2222 2020  e..        """  
+00020730: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00020740: 6f75 7420 3d20 7365 6c66 2e76 6965 7728  out = self.view(
+00020750: 6e70 2e6e 6461 7272 6179 292e 6173 7479  np.ndarray).asty
+00020760: 7065 286e 702e 666c 6f61 7433 3229 0d0a  pe(np.float32)..
+00020770: 2020 2020 2020 2020 6c6f 7765 726c 696d          lowerlim
+00020780: 2c20 7570 7065 726c 696d 203d 205f 6368  , upperlim = _ch
+00020790: 6563 6b5f 636c 6970 5f72 616e 6765 2869  eck_clip_range(i
+000207a0: 6e5f 7261 6e67 652c 2073 656c 662e 7661  n_range, self.va
+000207b0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
+000207c0: 2020 0d0a 2020 2020 2020 2020 6f75 7420    ..        out 
+000207d0: 3d20 736b 6578 702e 7265 7363 616c 655f  = skexp.rescale_
+000207e0: 696e 7465 6e73 6974 7928 6f75 742c 2069  intensity(out, i
+000207f0: 6e5f 7261 6e67 653d 286c 6f77 6572 6c69  n_range=(lowerli
+00020800: 6d2c 2075 7070 6572 6c69 6d29 2c20 6f75  m, upperlim), ou
+00020810: 745f 7261 6e67 653d 2264 7479 7065 2229  t_range="dtype")
+00020820: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00020830: 2020 2020 6f75 7420 3d20 6f75 742e 7669      out = out.vi
+00020840: 6577 2873 656c 662e 5f5f 636c 6173 735f  ew(self.__class_
+00020850: 5f29 0d0a 2020 2020 2020 2020 7265 7475  _)..        retu
+00020860: 726e 206f 7574 0d0a 2020 2020 0d0a 2020  rn out..    ..  
+00020870: 2020 4063 6865 636b 5f69 6e70 7574 5f61    @check_input_a
+00020880: 6e64 5f6f 7574 7075 740d 0a20 2020 2064  nd_output..    d
+00020890: 6566 2074 7261 636b 5f64 7269 6674 280d  ef track_drift(.
+000208a0: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
+000208b0: 2020 2020 2020 2020 616c 6f6e 673a 2041          along: A
+000208c0: 7869 734c 696b 6520 7c20 4e6f 6e65 203d  xisLike | None =
+000208d0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000208e0: 7368 6f77 5f64 7269 6674 3a20 626f 6f6c  show_drift: bool
+000208f0: 203d 2046 616c 7365 2c20 0d0a 2020 2020   = False, ..    
+00020900: 2020 2020 7570 7361 6d70 6c65 5f66 6163      upsample_fac
+00020910: 746f 723a 2069 6e74 203d 2031 302c 0d0a  tor: int = 10,..
+00020920: 2020 2020 2920 2d3e 204d 6172 6b65 7246      ) -> MarkerF
+00020930: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
+00020940: 2222 0d0a 2020 2020 2020 2020 4361 6c63  ""..        Calc
+00020950: 756c 6174 6520 7978 2d64 6972 6563 7469  ulate yx-directi
+00020960: 6f6e 616c 2064 7269 6674 2075 7369 6e67  onal drift using
+00020970: 2074 6865 206d 6574 686f 6420 6571 7569   the method equi
+00020980: 7661 6c65 6e74 2074 6f0d 0a20 2020 2020  valent to..     
+00020990: 2020 2060 6073 6b69 6d61 6765 2e72 6567     ``skimage.reg
+000209a0: 6973 7472 6174 696f 6e2e 7068 6173 655f  istration.phase_
+000209b0: 6372 6f73 735f 636f 7272 656c 6174 696f  cross_correlatio
+000209c0: 6e60 602e 0d0a 0d0a 2020 2020 2020 2020  n``.....        
+000209d0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+000209e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+000209f0: 2020 2020 2020 2020 616c 6f6e 6720 3a20          along : 
+00020a00: 4178 6973 4c69 6b65 2c20 6f70 7469 6f6e  AxisLike, option
+00020a10: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00020a20: 416c 6f6e 6720 7768 6963 6820 6178 6973  Along which axis
+00020a30: 2064 7269 6674 2077 696c 6c20 6265 2063   drift will be c
+00020a40: 616c 6375 6c61 7465 642e 0d0a 2020 2020  alculated...    
+00020a50: 2020 2020 7368 6f77 5f64 7269 6674 203a      show_drift :
+00020a60: 2062 6f6f 6c2c 2064 6566 6175 6c74 2069   bool, default i
+00020a70: 7320 4661 6c73 650d 0a20 2020 2020 2020  s False..       
+00020a80: 2020 2020 2049 6620 5472 7565 2c20 706c       If True, pl
+00020a90: 6f74 2074 6865 2072 6573 756c 742e 0d0a  ot the result...
+00020aa0: 2020 2020 2020 2020 7570 7361 6d70 6c65          upsample
+00020ab0: 5f66 6163 746f 7220 3a20 696e 742c 2064  _factor : int, d
+00020ac0: 6566 6175 6c74 2069 7320 3130 0d0a 2020  efault is 10..  
+00020ad0: 2020 2020 2020 2020 2020 5570 2d73 616d            Up-sam
+00020ae0: 706c 696e 6720 6661 6374 6f72 2077 6865  pling factor whe
+00020af0: 6e20 6361 6c63 756c 6174 696e 6720 7068  n calculating ph
+00020b00: 6173 6520 6372 6f73 7320 636f 7272 656c  ase cross correl
+00020b10: 6174 696f 6e2e 0d0a 2020 2020 2020 2020  ation...        
+00020b20: 2020 2020 0d0a 2020 2020 2020 2020 5265      ..        Re
+00020b30: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+00020b40: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00020b50: 4d61 726b 6572 4672 616d 650d 0a20 2020  MarkerFrame..   
+00020b60: 2020 2020 2020 2020 2044 6174 6146 7261           DataFra
+00020b70: 6d65 2073 7472 7563 7475 7265 2077 6974  me structure wit
+00020b80: 6820 782c 7920 636f 6c75 6d6e 730d 0a20  h x,y columns.. 
+00020b90: 2020 2020 2020 2022 2222 2020 2020 2020         """      
+00020ba0: 2020 0d0a 2020 2020 2020 2020 6672 6f6d    ..        from
+00020bb0: 202e 2e66 7261 6d65 2069 6d70 6f72 7420   ..frame import 
+00020bc0: 4d61 726b 6572 4672 616d 650d 0a20 2020  MarkerFrame..   
+00020bd0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+00020be0: 6620 616c 6f6e 6720 6973 204e 6f6e 653a  f along is None:
+00020bf0: 0d0a 2020 2020 2020 2020 2020 2020 616c  ..            al
+00020c00: 6f6e 6720 3d20 6669 6e64 5f66 6972 7374  ong = find_first
+00020c10: 5f61 7070 6561 7265 6428 2274 707a 6369  _appeared("tpzci
+00020c20: 6122 2c20 696e 636c 7564 653d 7365 6c66  a", include=self
+00020c30: 2e61 7865 7329 0d0a 2020 2020 2020 2020  .axes)..        
+00020c40: 656c 6966 206c 656e 2861 6c6f 6e67 2920  elif len(along) 
+00020c50: 213d 2031 3a0d 0a20 2020 2020 2020 2020  != 1:..         
+00020c60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00020c70: 726f 7228 2260 616c 6f6e 6760 206d 7573  ror("`along` mus
+00020c80: 7420 6265 2073 696e 676c 6520 6368 6172  t be single char
+00020c90: 6163 7465 722e 2229 0d0a 2020 2020 2020  acter.")..      
+00020ca0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00020cb0: 6e63 6528 7570 7361 6d70 6c65 5f66 6163  nce(upsample_fac
+00020cc0: 746f 722c 2069 6e74 293a 0d0a 2020 2020  tor, int):..    
+00020cd0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00020ce0: 7065 4572 726f 7228 6622 7570 7361 6d70  peError(f"upsamp
+00020cf0: 6c65 2d66 6163 746f 7220 6d75 7374 2062  le-factor must b
+00020d00: 6520 696e 7465 6765 7220 6275 7420 676f  e integer but go
+00020d10: 7420 7b74 7970 6528 7570 7361 6d70 6c65  t {type(upsample
+00020d20: 5f66 6163 746f 7229 7d22 290d 0a20 2020  _factor)}")..   
+00020d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d40: 200d 0a20 2020 2020 2020 2072 6573 756c   ..        resul
+00020d50: 7420 3d20 6e70 2e7a 6572 6f73 2828 7365  t = np.zeros((se
+00020d60: 6c66 2e73 697a 656f 6628 616c 6f6e 6729  lf.sizeof(along)
+00020d70: 2c20 7365 6c66 2e6e 6469 6d2d 3129 2c20  , self.ndim-1), 
+00020d80: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00020d90: 290d 0a20 2020 2020 2020 2063 5f61 7865  )..        c_axe
+00020da0: 7320 3d20 636f 6d70 6c65 6d65 6e74 5f61  s = complement_a
+00020db0: 7865 7328 616c 6f6e 672c 2073 656c 662e  xes(along, self.
+00020dc0: 6178 6573 290d 0a20 2020 2020 2020 206c  axes)..        l
+00020dd0: 6173 745f 696d 6720 3d20 4e6f 6e65 0d0a  ast_img = None..
+00020de0: 2020 2020 2020 2020 696d 675f 6666 7420          img_fft 
+00020df0: 3d20 7365 6c66 2e66 6674 2873 6869 6674  = self.fft(shift
+00020e00: 3d46 616c 7365 2c20 6469 6d73 3d63 5f61  =False, dims=c_a
+00020e10: 7865 7329 0d0a 2020 2020 2020 2020 666f  xes)..        fo
+00020e20: 7220 692c 2028 5f2c 2069 6d67 2920 696e  r i, (_, img) in
+00020e30: 2065 6e75 6d65 7261 7465 2869 6d67 5f66   enumerate(img_f
+00020e40: 6674 2e69 7465 7228 616c 6f6e 6729 293a  ft.iter(along)):
+00020e50: 0d0a 2020 2020 2020 2020 2020 2020 696d  ..            im
+00020e60: 6720 3d20 7870 2e61 7361 7272 6179 2869  g = xp.asarray(i
+00020e70: 6d67 290d 0a20 2020 2020 2020 2020 2020  mg)..           
+00020e80: 2069 6620 6c61 7374 5f69 6d67 2069 7320   if last_img is 
+00020e90: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00020ea0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00020eb0: 745b 695d 203d 2078 702e 6173 6e75 6d70  t[i] = xp.asnump
+00020ec0: 7928 0d0a 2020 2020 2020 2020 2020 2020  y(..            
+00020ed0: 2020 2020 2020 2020 5f63 6f72 722e 7375          _corr.su
+00020ee0: 6270 6978 656c 5f70 6363 286c 6173 745f  bpixel_pcc(last_
+00020ef0: 696d 672c 2069 6d67 2c20 7570 7361 6d70  img, img, upsamp
+00020f00: 6c65 5f66 6163 746f 723d 7570 7361 6d70  le_factor=upsamp
+00020f10: 6c65 5f66 6163 746f 7229 5b30 5d0d 0a20  le_factor)[0].. 
+00020f20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00020f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020f40: 2020 6c61 7374 5f69 6d67 203d 2069 6d67    last_img = img
+00020f50: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00020f60: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00020f70: 2020 2020 206c 6173 745f 696d 6720 3d20       last_img = 
+00020f80: 696d 670d 0a20 2020 2020 2020 200d 0a20  img..        .. 
+00020f90: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00020fa0: 4d61 726b 6572 4672 616d 6528 6e70 2e63  MarkerFrame(np.c
+00020fb0: 756d 7375 6d28 7265 7375 6c74 2c20 6178  umsum(result, ax
+00020fc0: 6973 3d30 292c 2063 6f6c 756d 6e73 3d63  is=0), columns=c
+00020fd0: 5f61 7865 7329 0d0a 2020 2020 2020 2020  _axes)..        
+00020fe0: 6966 2073 686f 775f 6472 6966 743a 0d0a  if show_drift:..
+00020ff0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+00021000: 202e 5f75 7469 6c73 2069 6d70 6f72 7420   ._utils import 
+00021010: 5f70 6c6f 7420 6173 205f 706c 740d 0a20  _plot as _plt.. 
+00021020: 2020 2020 2020 2020 2020 205f 706c 742e             _plt.
+00021030: 706c 6f74 5f64 7269 6674 2872 6573 756c  plot_drift(resul
+00021040: 7429 0d0a 2020 2020 2020 2020 0d0a 2020  t)..        ..  
+00021050: 2020 2020 2020 7265 7375 6c74 2e69 6e64        result.ind
+00021060: 6578 2e6e 616d 6520 3d20 7374 7228 616c  ex.name = str(al
+00021070: 6f6e 6729 0d0a 2020 2020 2020 2020 7265  ong)..        re
+00021080: 7475 726e 2072 6573 756c 740d 0a20 2020  turn result..   
+00021090: 200d 0a20 2020 2040 5f64 6f63 732e 7772   ..    @_docs.wr
+000210a0: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
+000210b0: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
+000210c0: 7865 730d 0a20 2020 2040 7361 6d65 5f64  xes..    @same_d
+000210d0: 7479 7065 2861 7366 6c6f 6174 3d54 7275  type(asfloat=Tru
+000210e0: 6529 0d0a 2020 2020 4063 6865 636b 5f69  e)..    @check_i
+000210f0: 6e70 7574 5f61 6e64 5f6f 7574 7075 740d  nput_and_output.
+00021100: 0a20 2020 2064 6566 2064 7269 6674 5f63  .    def drift_c
+00021110: 6f72 7265 6374 696f 6e28 0d0a 2020 2020  orrection(..    
+00021120: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00021130: 2020 2073 6869 6674 3a20 436f 6f72 6473     shift: Coords
+00021140: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00021150: 2020 7265 663a 2049 6d67 4172 7261 7920    ref: ImgArray 
+00021160: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00021170: 202a 2c0d 0a20 2020 2020 2020 207a 6572   *,..        zer
+00021180: 6f5f 6176 653a 2062 6f6f 6c20 3d20 5472  o_ave: bool = Tr
+00021190: 7565 2c0d 0a20 2020 2020 2020 2061 6c6f  ue,..        alo
+000211a0: 6e67 3a20 4178 6973 4c69 6b65 207c 204e  ng: AxisLike | N
+000211b0: 6f6e 6520 3d20 4e6f 6e65 2c0d 0a20 2020  one = None,..   
+000211c0: 2020 2020 206f 7264 6572 3a20 696e 7420       order: int 
+000211d0: 3d20 312c 0d0a 2020 2020 2020 2020 6d6f  = 1,..        mo
+000211e0: 6465 3a20 7374 7220 3d20 2263 6f6e 7374  de: str = "const
+000211f0: 616e 7422 2c0d 0a20 2020 2020 2020 2063  ant",..        c
+00021200: 7661 6c3a 2066 6c6f 6174 203d 2030 2c0d  val: float = 0,.
+00021210: 0a20 2020 2020 2020 2064 696d 733a 2044  .        dims: D
+00021220: 696d 7320 3d20 322c 0d0a 2020 2020 2020  ims = 2,..      
+00021230: 2020 7570 6461 7465 3a20 626f 6f6c 203d    update: bool =
+00021240: 2046 616c 7365 2c0d 0a20 2020 2029 202d   False,..    ) -
+00021250: 3e20 496d 6741 7272 6179 3a0d 0a20 2020  > ImgArray:..   
+00021260: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00021270: 2020 4472 6966 7420 636f 7272 6563 7469    Drift correcti
+00021280: 6f6e 2075 7369 6e67 2069 7465 7261 7469  on using iterati
+00021290: 7665 2041 6666 696e 6520 7472 616e 736c  ve Affine transl
+000212a0: 6174 696f 6e2e 2049 6620 7472 616e 736c  ation. If transl
+000212b0: 6174 696f 6e20 7665 6374 6f72 7320 6060  ation vectors ``
+000212c0: 7368 6966 7460 600d 0a20 2020 2020 2020  shift``..       
+000212d0: 2069 7320 6e6f 7420 6769 7665 6e2c 2074   is not given, t
+000212e0: 6865 6e20 6974 2077 696c 6c20 6265 2064  hen it will be d
+000212f0: 6574 6572 6d69 6e65 6420 7573 696e 6720  etermined using 
+00021300: 6060 7472 6163 6b5f 6472 6966 7460 6020  ``track_drift`` 
+00021310: 6d65 7468 6f64 206f 6620 496d 6741 7272  method of ImgArr
+00021320: 6179 2e0d 0a0d 0a20 2020 2020 2020 2050  ay.....        P
+00021330: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00021340: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00021350: 2020 2020 2020 2073 6869 6674 203a 2044         shift : D
+00021360: 6174 6146 7261 6d65 206f 7220 284e 2c20  ataFrame or (N, 
+00021370: 4429 2061 7272 6179 2c20 6f70 7469 6f6e  D) array, option
+00021380: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00021390: 5472 616e 736c 6174 696f 6e20 7665 6374  Translation vect
+000213a0: 6f72 732e 2049 6620 4461 7461 4672 616d  ors. If DataFram
+000213b0: 652c 2069 7420 6d75 7374 2068 6176 6520  e, it must have 
+000213c0: 636f 6c75 6d6e 7320 6e61 6d65 6420 7769  columns named wi
+000213d0: 7468 2061 6c6c 2074 6865 2073 796d 626f  th all the symbo
+000213e0: 6c73 0d0a 2020 2020 2020 2020 2020 2020  ls..            
+000213f0: 636f 6e74 6169 6e65 6420 696e 2060 6064  contained in ``d
+00021400: 696d 7360 602e 0d0a 2020 2020 2020 2020  ims``...        
+00021410: 7265 6620 3a20 496d 6741 7272 6179 2c20  ref : ImgArray, 
+00021420: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00021430: 2020 2020 2020 5468 6520 7265 6665 7265        The refere
+00021440: 6e63 6520 6e2d 4420 696d 6167 6520 746f  nce n-D image to
+00021450: 2064 6574 6572 6d69 6e65 2064 7269 6674   determine drift
+00021460: 2c20 6966 2060 6073 6869 6674 6060 2077  , if ``shift`` w
+00021470: 6173 206e 6f74 2067 6976 656e 2e0d 0a20  as not given... 
+00021480: 2020 2020 2020 207a 6572 6f5f 6176 6520         zero_ave 
+00021490: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+000214a0: 6973 2054 7275 650d 0a20 2020 2020 2020  is True..       
+000214b0: 2020 2020 2049 6620 5472 7565 2c20 6176       If True, av
+000214c0: 6572 6167 6520 7368 6966 7420 7769 6c6c  erage shift will
+000214d0: 2062 6520 7a65 726f 2e0d 0a20 2020 2020   be zero...     
+000214e0: 2020 2061 6c6f 6e67 203a 2041 7869 734c     along : AxisL
+000214f0: 696b 652c 206f 7074 696f 6e61 6c0d 0a20  ike, optional.. 
+00021500: 2020 2020 2020 2020 2020 2041 6c6f 6e67             Along
+00021510: 2077 6869 6368 2061 7869 7320 6472 6966   which axis drif
+00021520: 7420 7769 6c6c 2062 6520 636f 7272 6563  t will be correc
+00021530: 7465 642e 0d0a 2020 2020 2020 2020 7b64  ted...        {d
+00021540: 696d 737d 7b75 7064 6174 657d 0d0a 2020  ims}{update}..  
+00021550: 2020 2020 2020 6166 6669 6e65 5f6b 7761        affine_kwa
+00021560: 7267 7320 3a0d 0a20 2020 2020 2020 2020  rgs :..         
+00021570: 2020 204b 6579 776f 7264 2061 7267 756d     Keyword argum
+00021580: 656e 7473 2074 6861 7420 7769 6c6c 2062  ents that will b
+00021590: 6520 7061 7373 6564 2074 6f20 6060 7761  e passed to ``wa
+000215a0: 7270 6060 2e0d 0a0d 0a20 2020 2020 2020  rp``.....       
+000215b0: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+000215c0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+000215d0: 2020 2049 6d67 4172 7261 790d 0a20 2020     ImgArray..   
+000215e0: 2020 2020 2020 2020 2043 6f72 7265 6374           Correct
+000215f0: 6564 2069 6d61 6765 2e0d 0a20 2020 2020  ed image...     
+00021600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00021610: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
+00021620: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
+00021630: 2020 2020 2044 7269 6674 2063 6f72 7265       Drift corre
+00021640: 6374 696f 6e20 6f66 206d 756c 7469 6368  ction of multich
+00021650: 616e 6e65 6c20 696d 6167 6520 7573 696e  annel image usin
+00021660: 6720 7468 6520 6669 7273 7420 6368 616e  g the first chan
+00021670: 6e65 6c20 6173 2074 6865 2072 6566 6572  nel as the refer
+00021680: 656e 6365 2e0d 0a20 2020 2020 2020 2020  ence...         
+00021690: 2020 203e 3e3e 2069 6d67 2e64 7269 6674     >>> img.drift
+000216a0: 5f63 6f72 7265 6374 696f 6e28 7265 663d  _correction(ref=
+000216b0: 696d 675b 2263 3d30 225d 290d 0a20 2020  img["c=0"])..   
+000216c0: 2020 2020 2022 2222 2020 2020 2020 2020       """        
+000216d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000216e0: 2020 2020 6966 2061 6c6f 6e67 2069 7320      if along is 
+000216f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00021700: 2020 2061 6c6f 6e67 203d 2066 696e 645f     along = find_
+00021710: 6669 7273 745f 6170 7065 6172 6564 2822  first_appeared("
+00021720: 7470 7a63 6961 222c 2069 6e63 6c75 6465  tpzcia", include
+00021730: 3d73 656c 662e 6178 6573 2c20 6578 636c  =self.axes, excl
+00021740: 7564 653d 6469 6d73 290d 0a20 2020 2020  ude=dims)..     
+00021750: 2020 2065 6c69 6620 6c65 6e28 616c 6f6e     elif len(alon
+00021760: 6729 2021 3d20 313a 0d0a 2020 2020 2020  g) != 1:..      
+00021770: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00021780: 6545 7272 6f72 2822 6061 6c6f 6e67 6020  eError("`along` 
+00021790: 6d75 7374 2062 6520 7369 6e67 6c65 2063  must be single c
+000217a0: 6861 7261 6374 6572 2e22 290d 0a20 2020  haracter.")..   
+000217b0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+000217c0: 6620 7368 6966 7420 6973 204e 6f6e 653a  f shift is None:
+000217d0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000217e0: 6465 7465 726d 696e 6520 2772 6566 270d  determine 'ref'.
+000217f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00021800: 7265 6620 6973 204e 6f6e 653a 0d0a 2020  ref is None:..  
+00021810: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00021820: 6620 3d20 7365 6c66 0d0a 2020 2020 2020  f = self..      
+00021830: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
+00021840: 7369 6e73 7461 6e63 6528 7265 662c 2049  sinstance(ref, I
+00021850: 6d67 4172 7261 7929 3a0d 0a20 2020 2020  mgArray):..     
+00021860: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00021870: 2054 7970 6545 7272 6f72 2866 2227 7265   TypeError(f"'re
+00021880: 6627 206d 7573 7420 6265 2061 6e20 496d  f' must be an Im
+00021890: 6741 7272 6179 206f 626a 6563 742c 2062  gArray object, b
+000218a0: 7574 2067 6f74 207b 7479 7065 2872 6566  ut got {type(ref
+000218b0: 297d 2229 0d0a 2020 2020 2020 2020 2020  )}")..          
+000218c0: 2020 6966 2072 6566 2e61 7865 7320 213d    if ref.axes !=
+000218d0: 205b 616c 6f6e 675d 202b 2064 696d 733a   [along] + dims:
+000218e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000218f0: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
+00021900: 2069 6d70 6f72 7420 7072 6f64 7563 740d   import product.
+00021910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021920: 205f 635f 6178 6573 203d 2063 6f6d 706c   _c_axes = compl
+00021930: 656d 656e 745f 6178 6573 285b 616c 6f6e  ement_axes([alon
+00021940: 675d 202b 2064 696d 732c 2073 7472 2872  g] + dims, str(r
+00021950: 6566 2e61 7865 7329 290d 0a20 2020 2020  ef.axes))..     
+00021960: 2020 2020 2020 2020 2020 2066 6d74 203d             fmt =
+00021970: 2073 6c69 6365 722e 6765 745f 666f 726d   slicer.get_form
+00021980: 6174 7465 7228 5f63 5f61 7865 7329 0d0a  atter(_c_axes)..
+00021990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219a0: 6f75 7420 3d20 6e70 2e65 6d70 7479 5f6c  out = np.empty_l
+000219b0: 696b 6528 7365 6c66 290d 0a20 2020 2020  ike(self)..     
+000219c0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000219d0: 6478 2069 6e20 7072 6f64 7563 7428 2a28  dx in product(*(
+000219e0: 7261 6e67 6528 7265 662e 7369 7a65 6f66  range(ref.sizeof
+000219f0: 2861 2929 2066 6f72 2061 2069 6e20 5f63  (a)) for a in _c
+00021a00: 5f61 7865 7329 293a 0d0a 2020 2020 2020  _axes)):..      
+00021a10: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00021a20: 203d 2066 6d74 5b69 6478 5d0d 0a20 2020   = fmt[idx]..   
+00021a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021a40: 206f 7574 5b73 6c5d 203d 2073 656c 665b   out[sl] = self[
+00021a50: 736c 5d2e 6472 6966 745f 636f 7272 6563  sl].drift_correc
+00021a60: 7469 6f6e 280d 0a20 2020 2020 2020 2020  tion(..         
+00021a70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00021a80: 6566 3d72 6566 5b73 6c5d 2c20 7a65 726f  ef=ref[sl], zero
+00021a90: 5f61 7665 3d7a 6572 6f5f 6176 652c 2061  _ave=zero_ave, a
+00021aa0: 6c6f 6e67 3d61 6c6f 6e67 2c20 6469 6d73  long=along, dims
+00021ab0: 3d64 696d 732c 0d0a 2020 2020 2020 2020  =dims,..        
+00021ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ad0: 7570 6461 7465 3d75 7064 6174 652c 206f  update=update, o
+00021ae0: 7264 6572 3d6f 7264 6572 2c20 6d6f 6465  rder=order, mode
+00021af0: 3d6d 6f64 652c 2063 7661 6c3d 6376 616c  =mode, cval=cval
+00021b00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00021b10: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00021b20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00021b30: 206f 7574 0d0a 0d0a 2020 2020 2020 2020   out....        
+00021b40: 2020 2020 7368 6966 7420 3d20 7265 662e      shift = ref.
+00021b50: 7472 6163 6b5f 6472 6966 7428 616c 6f6e  track_drift(alon
+00021b60: 673d 616c 6f6e 6729 2e76 616c 7565 730d  g=along).values.
+00021b70: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00021b80: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00021b90: 2020 2020 2020 2020 2020 7368 6966 7420            shift 
+00021ba0: 3d20 6e70 2e61 7361 7272 6179 2873 6869  = np.asarray(shi
+00021bb0: 6674 2c20 6474 7970 653d 6e70 2e66 6c6f  ft, dtype=np.flo
+00021bc0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00021bd0: 2020 2069 6620 2873 656c 662e 7369 7a65     if (self.size
+00021be0: 6f66 2861 6c6f 6e67 292c 2073 656c 662e  of(along), self.
+00021bf0: 6e64 696d 2920 213d 2073 6869 6674 2e73  ndim) != shift.s
+00021c00: 6861 7065 3a0d 0a20 2020 2020 2020 2020  hape:..         
+00021c10: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00021c20: 7565 4572 726f 7228 2257 726f 6e67 2073  ueError("Wrong s
+00021c30: 6861 7065 206f 6620 6073 6869 6674 602e  hape of `shift`.
+00021c40: 2229 0d0a 0d0a 2020 2020 2020 2020 6966  ")....        if
+00021c50: 207a 6572 6f5f 6176 653a 0d0a 2020 2020   zero_ave:..    
+00021c60: 2020 2020 2020 2020 7368 6966 7420 3d20          shift = 
+00021c70: 7368 6966 7420 2d20 6e70 2e6d 6561 6e28  shift - np.mean(
+00021c80: 7368 6966 742c 2061 7869 733d 3029 0d0a  shift, axis=0)..
+00021c90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00021ca0: 2020 2020 2020 6f75 7420 3d20 7870 2e65        out = xp.e
+00021cb0: 6d70 7479 2873 656c 662e 7368 6170 6529  mpty(self.shape)
+00021cc0: 0d0a 2020 2020 2020 2020 745f 696e 6465  ..        t_inde
+00021cd0: 7820 3d20 7365 6c66 2e61 7869 736f 6628  x = self.axisof(
+00021ce0: 616c 6f6e 6729 0d0a 2020 2020 2020 2020  along)..        
+00021cf0: 6e64 696d 203d 206c 656e 2864 696d 7329  ndim = len(dims)
+00021d00: 0d0a 2020 2020 2020 2020 6d78 203d 206e  ..        mx = n
+00021d10: 702e 6579 6528 6e64 696d 202b 2031 2c20  p.eye(ndim + 1, 
+00021d20: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00021d30: 2920 2320 4166 6669 6e65 2074 7261 6e73  ) # Affine trans
+00021d40: 666f 726d 6174 696f 6e20 6d61 7472 6978  formation matrix
+00021d50: 0d0a 2020 2020 2020 2020 696e 7075 745f  ..        input_
+00021d60: 696d 6720 3d20 7365 6c66 2e73 706c 696e  img = self.splin
+00021d70: 655f 6669 6c74 6572 286d 6f64 653d 6d6f  e_filter(mode=mo
+00021d80: 6465 2c20 6f72 6465 723d 6f72 6465 7229  de, order=order)
+00021d90: 0d0a 2020 2020 2020 2020 666f 7220 736c  ..        for sl
+00021da0: 2c20 696d 6720 696e 2069 6e70 7574 5f69  , img in input_i
+00021db0: 6d67 2e69 7465 7228 636f 6d70 6c65 6d65  mg.iter(compleme
+00021dc0: 6e74 5f61 7865 7328 6469 6d73 2c20 7365  nt_axes(dims, se
+00021dd0: 6c66 2e61 7865 7329 293a 0d0a 2020 2020  lf.axes)):..    
+00021de0: 2020 2020 2020 2020 6d78 5b3a 2d31 2c20          mx[:-1, 
+00021df0: 2d31 5d20 3d20 2d73 6869 6674 5b73 6c5b  -1] = -shift[sl[
+00021e00: 745f 696e 6465 785d 5d0d 0a20 2020 2020  t_index]]..     
+00021e10: 2020 2020 2020 206f 7574 5b73 6c5d 203d         out[sl] =
+00021e20: 205f 7472 616e 7366 6f72 6d2e 7761 7270   _transform.warp
+00021e30: 2869 6d67 2c20 6d78 2c20 6d6f 6465 3d6d  (img, mx, mode=m
+00021e40: 6f64 652c 2063 7661 6c3d 6376 616c 2c20  ode, cval=cval, 
+00021e50: 6f72 6465 723d 6f72 6465 722c 2070 7265  order=order, pre
+00021e60: 6669 6c74 6572 3d46 616c 7365 290d 0a20  filter=False).. 
+00021e70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00021e80: 2072 6574 7572 6e20 6f75 740d 0a0d 0a20   return out.... 
+00021e90: 2020 2040 5f64 6f63 732e 7772 6974 655f     @_docs.write_
+00021ea0: 646f 6373 0d0a 2020 2020 4064 696d 735f  docs..    @dims_
+00021eb0: 746f 5f73 7061 7469 616c 5f61 7865 730d  to_spatial_axes.
+00021ec0: 0a20 2020 2064 6566 2065 7374 696d 6174  .    def estimat
+00021ed0: 655f 7369 676d 6128 7365 6c66 2c20 2a2c  e_sigma(self, *,
+00021ee0: 2073 7175 6565 7a65 3a20 626f 6f6c 203d   squeeze: bool =
+00021ef0: 2054 7275 652c 2064 696d 733a 2044 696d   True, dims: Dim
+00021f00: 7320 3d20 4e6f 6e65 2920 2d3e 2050 726f  s = None) -> Pro
+00021f10: 7041 7272 6179 207c 2066 6c6f 6174 3a0d  pArray | float:.
+00021f20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00021f30: 2020 2020 2020 5761 7665 6c65 742d 6261        Wavelet-ba
+00021f40: 7365 6420 6573 7469 6d61 7469 6f6e 206f  sed estimation o
+00021f50: 6620 4761 7573 7369 616e 206e 6f69 7365  f Gaussian noise
+00021f60: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00021f70: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+00021f80: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00021f90: 2020 2020 2073 7175 6565 7a65 203a 2062       squeeze : b
+00021fa0: 6f6f 6c2c 2064 6566 6175 6c74 2069 7320  ool, default is 
+00021fb0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+00021fc0: 2020 4966 2054 7275 6520 616e 6420 6f75    If True and ou
+00021fd0: 7470 7574 2063 616e 2062 6520 636f 6e76  tput can be conv
+00021fe0: 6572 7465 6420 746f 2061 2073 6361 6c61  erted to a scala
+00021ff0: 722c 2074 6865 6e20 636f 6e76 6572 7420  r, then convert 
+00022000: 6974 2e0d 0a20 2020 2020 2020 207b 6469  it...        {di
+00022010: 6d73 7d0d 0a0d 0a20 2020 2020 2020 2052  ms}....        R
+00022020: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+00022030: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00022040: 2050 726f 7041 7272 6179 206f 7220 666c   PropArray or fl
+00022050: 6f61 740d 0a20 2020 2020 2020 2020 2020  oat..           
+00022060: 2045 7374 696d 6174 6564 2073 7461 6e64   Estimated stand
+00022070: 6172 6420 6465 7669 6174 696f 6e2e 2073  ard deviation. s
+00022080: 6967 6d61 5b22 743d 303b 633d 3122 5d20  igma["t=0;c=1"] 
+00022090: 6d65 616e 7320 7468 6520 6573 7469 6d61  means the estima
+000220a0: 7465 6420 7661 6c75 6520 6f66 0d0a 2020  ted value of..  
+000220b0: 2020 2020 2020 2020 2020 696d 6167 6520            image 
+000220c0: 736c 6963 6520 6174 2074 3d30 2061 6e64  slice at t=0 and
+000220d0: 2063 3d31 2e0d 0a20 2020 2020 2020 2022   c=1...        "
+000220e0: 2222 2020 2020 2020 2020 0d0a 2020 2020  ""        ..    
+000220f0: 2020 2020 635f 6178 6573 203d 2063 6f6d      c_axes = com
+00022100: 706c 656d 656e 745f 6178 6573 2864 696d  plement_axes(dim
+00022110: 732c 2073 656c 662e 6178 6573 290d 0a20  s, self.axes).. 
+00022120: 2020 2020 2020 206f 7574 203d 2073 656c         out = sel
+00022130: 662e 5f61 7070 6c79 5f64 6173 6b28 0d0a  f._apply_dask(..
+00022140: 2020 2020 2020 2020 2020 2020 736b 7265              skre
+00022150: 732e 6573 7469 6d61 7465 5f73 6967 6d61  s.estimate_sigma
+00022160: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00022170: 5f61 7865 733d 635f 6178 6573 2c0d 0a20  _axes=c_axes,.. 
+00022180: 2020 2020 2020 2020 2020 2064 726f 705f             drop_
+00022190: 6178 6973 3d64 696d 730d 0a20 2020 2020  axis=dims..     
+000221a0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000221b0: 2020 0d0a 2020 2020 2020 2020 6966 206f    ..        if o
+000221c0: 7574 2e6e 6469 6d20 3d3d 2030 2061 6e64  ut.ndim == 0 and
+000221d0: 2073 7175 6565 7a65 3a0d 0a20 2020 2020   squeeze:..     
+000221e0: 2020 2020 2020 206f 7574 203d 206f 7574         out = out
+000221f0: 2e69 7465 6d28 290d 0a20 2020 2020 2020  .item()..       
+00022200: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00022210: 2020 2020 6f75 7420 3d20 5072 6f70 4172      out = PropAr
+00022220: 7261 7928 0d0a 2020 2020 2020 2020 2020  ray(..          
+00022230: 2020 2020 2020 6f75 742c 2064 7479 7065        out, dtype
+00022240: 3d6e 702e 666c 6f61 7433 322c 206e 616d  =np.float32, nam
+00022250: 653d 7365 6c66 2e6e 616d 652c 2061 7865  e=self.name, axe
+00022260: 733d 635f 6178 6573 2c20 7072 6f70 6e61  s=c_axes, propna
+00022270: 6d65 3d22 6573 7469 6d61 7465 5f73 6967  me="estimate_sig
+00022280: 6d61 220d 0a20 2020 2020 2020 2020 2020  ma"..           
+00022290: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000222a0: 6f75 742e 5f73 6574 5f69 6e66 6f28 7365  out._set_info(se
+000222b0: 6c66 2c20 6e65 775f 6178 6573 3d63 5f61  lf, new_axes=c_a
+000222c0: 7865 7329 0d0a 2020 2020 2020 2020 7265  xes)..        re
+000222d0: 7475 726e 206f 7574 2020 2020 2020 200d  turn out       .
+000222e0: 0a0d 0a20 2020 2040 5f64 6f63 732e 7772  ...    @_docs.wr
+000222f0: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
+00022300: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
+00022310: 7865 730d 0a20 2020 2064 6566 2063 656e  xes..    def cen
+00022320: 7465 725f 6f66 5f6d 6173 7328 7365 6c66  ter_of_mass(self
+00022330: 2c20 6469 6d73 3a20 4469 6d73 203d 204e  , dims: Dims = N
+00022340: 6f6e 6529 202d 3e20 5072 6f70 4172 7261  one) -> PropArra
+00022350: 793a 0d0a 2020 2020 2020 2020 2222 220d  y:..        """.
+00022360: 0a20 2020 2020 2020 2043 616c 6375 6c61  .        Calcula
+00022370: 7465 2074 6865 2063 656e 7465 7220 6f66  te the center of
+00022380: 206d 6173 7320 6f66 2074 6865 2069 6d61   mass of the ima
+00022390: 6765 2e0d 0a0d 0a20 2020 2020 2020 2050  ge.....        P
+000223a0: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+000223b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+000223c0: 2020 2020 2020 207b 6469 6d73 7d0d 0a0d         {dims}...
+000223d0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000223e0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+000223f0: 2d0d 0a20 2020 2020 2020 2050 726f 7041  -..        PropA
+00022400: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
+00022410: 2020 4365 6e74 6572 206f 6620 6d61 7373    Center of mass
+00022420: 2e20 4178 6573 2077 696c 6c20 6265 2074  . Axes will be t
+00022430: 6865 2069 6e70 7574 2061 7865 7320 6d69  he input axes mi
+00022440: 6e75 7320 6060 6469 6d73 6060 2c20 706c  nus ``dims``, pl
+00022450: 7573 2061 206e 6577 2061 7869 730d 0a20  us a new axis.. 
+00022460: 2020 2020 2020 2020 2020 2060 6064 696d             ``dim
+00022470: 6060 2061 7420 7468 6520 6669 7273 7420  `` at the first 
+00022480: 706f 7369 7469 6f6e 2c20 7768 6963 6820  position, which 
+00022490: 7265 7072 6573 656e 7473 2074 6865 2064  represents the d
+000224a0: 696d 656e 7369 6f6e 7320 6f66 2074 6865  imensions of the
+000224b0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000224c0: 7375 6c74 732e 0d0a 2020 2020 2020 2020  sults...        
+000224d0: 2222 2220 2020 2020 2020 200d 0a20 2020  """        ..   
+000224e0: 2020 2020 2063 5f61 7865 7320 3d20 636f       c_axes = co
+000224f0: 6d70 6c65 6d65 6e74 5f61 7865 7328 6469  mplement_axes(di
+00022500: 6d73 2c20 7365 6c66 2e61 7865 7329 0d0a  ms, self.axes)..
+00022510: 2020 2020 2020 2020 6f75 745f 7368 6170          out_shap
+00022520: 6520 3d20 286c 656e 2864 696d 7329 2c20  e = (len(dims), 
+00022530: 2920 2b20 7365 6c66 2e73 697a 6573 6f66  ) + self.sizesof
+00022540: 2863 5f61 7865 7329 0d0a 2020 2020 2020  (c_axes)..      
+00022550: 2020 6178 6973 203d 2041 7869 7328 2264    axis = Axis("d
+00022560: 696d 2229 0d0a 2020 2020 2020 2020 6178  im")..        ax
+00022570: 6973 2e6c 6162 656c 7320 3d20 6469 6d73  is.labels = dims
+00022580: 0d0a 2020 2020 2020 2020 6f75 745f 6178  ..        out_ax
+00022590: 6573 203d 205b 6178 6973 5d20 2b20 635f  es = [axis] + c_
+000225a0: 6178 6573 0d0a 2020 2020 2020 2020 6f75  axes..        ou
+000225b0: 7420 3d20 6e70 2e65 6d70 7479 286f 7574  t = np.empty(out
+000225c0: 5f73 6861 7065 2c20 6474 7970 653d 6e70  _shape, dtype=np
+000225d0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+000225e0: 2020 2066 6f72 2073 6c2c 2069 6d67 2069     for sl, img i
+000225f0: 6e20 7365 6c66 2e69 7465 7228 635f 6178  n self.iter(c_ax
+00022600: 6573 2c20 6973 7261 773d 5472 7565 2c20  es, israw=True, 
+00022610: 6578 636c 7564 653d 6469 6d73 293a 0d0a  exclude=dims):..
+00022620: 2020 2020 2020 2020 2020 2020 6f75 745b              out[
+00022630: 2873 6c69 6365 284e 6f6e 6529 2c29 202b  (slice(None),) +
+00022640: 2073 6c5d 203d 206e 6469 2e63 656e 7465   sl] = ndi.cente
+00022650: 725f 6f66 5f6d 6173 7328 696d 6729 0d0a  r_of_mass(img)..
+00022660: 2020 2020 2020 2020 6f75 7420 3d20 5072          out = Pr
+00022670: 6f70 4172 7261 7928 0d0a 2020 2020 2020  opArray(..      
+00022680: 2020 2020 2020 6f75 742c 2064 7479 7065        out, dtype
+00022690: 3d6e 702e 666c 6f61 7433 322c 206e 616d  =np.float32, nam
+000226a0: 653d 7365 6c66 2e6e 616d 652c 2061 7865  e=self.name, axe
+000226b0: 733d 6f75 745f 6178 6573 2c20 7072 6f70  s=out_axes, prop
+000226c0: 6e61 6d65 3d22 6365 6e74 6572 5f6f 665f  name="center_of_
+000226d0: 6d61 7373 220d 0a20 2020 2020 2020 2029  mass"..        )
+000226e0: 0d0a 2020 2020 2020 2020 6f75 742e 5f73  ..        out._s
+000226f0: 6574 5f69 6e66 6f28 7365 6c66 2c20 6e65  et_info(self, ne
+00022700: 775f 6178 6573 3d6f 7574 5f61 7865 7329  w_axes=out_axes)
+00022710: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00022720: 206f 7574 0d0a 2020 2020 0d0a 2020 2020   out..    ..    
+00022730: 4064 696d 735f 746f 5f73 7061 7469 616c  @dims_to_spatial
+00022740: 5f61 7865 730d 0a20 2020 2040 6368 6563  _axes..    @chec
+00022750: 6b5f 696e 7075 745f 616e 645f 6f75 7470  k_input_and_outp
+00022760: 7574 0d0a 2020 2020 6465 6620 7061 6428  ut..    def pad(
+00022770: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
+00022780: 0d0a 2020 2020 2020 2020 7061 645f 7769  ..        pad_wi
+00022790: 6474 683a 2069 6e74 207c 2074 7570 6c65  dth: int | tuple
+000227a0: 5b69 6e74 2c20 696e 745d 207c 2053 6571  [int, int] | Seq
+000227b0: 7565 6e63 655b 7475 706c 655b 696e 742c  uence[tuple[int,
+000227c0: 2069 6e74 5d5d 2c20 0d0a 2020 2020 2020   int]], ..      
+000227d0: 2020 2a2c 200d 0a20 2020 2020 2020 206d    *, ..        m
+000227e0: 6f64 653a 2050 6164 6469 6e67 4d6f 6465  ode: PaddingMode
+000227f0: 203d 2022 636f 6e73 7461 6e74 222c 200d   = "constant", .
+00022800: 0a20 2020 2020 2020 2064 696d 733a 2044  .        dims: D
+00022810: 696d 7320 3d20 4e6f 6e65 2c20 0d0a 2020  ims = None, ..  
+00022820: 2020 2020 2020 2a2a 6b77 6172 6773 0d0a        **kwargs..
+00022830: 2020 2020 2920 2d3e 2049 6d67 4172 7261      ) -> ImgArra
+00022840: 793a 0d0a 2020 2020 2020 2020 2222 220d  y:..        """.
+00022850: 0a20 2020 2020 2020 2050 6164 2069 6d61  .        Pad ima
+00022860: 6765 206f 6e6c 7920 666f 7220 7370 6174  ge only for spat
+00022870: 6961 6c20 6469 6d65 6e73 696f 6e73 2e0d  ial dimensions..
+00022880: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00022890: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+000228a0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+000228b0: 2020 2070 6164 5f77 6964 7468 2c20 6d6f     pad_width, mo
+000228c0: 6465 2c20 2a2a 6b77 6172 6773 203a 200d  de, **kwargs : .
+000228d0: 0a20 2020 2020 2020 2020 2020 2053 6565  .            See
+000228e0: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
+000228f0: 6620 6e70 2e70 6164 2829 2e0d 0a20 2020  f np.pad()...   
+00022900: 2020 2020 2064 696d 7320 3a20 696e 7420       dims : int 
+00022910: 6f72 2073 7472 2c20 6f70 7469 6f6e 616c  or str, optional
+00022920: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00022930: 6963 6820 6469 6d65 6e73 696f 6e20 746f  ich dimension to
+00022940: 2070 6164 2e0d 0a0d 0a20 2020 2020 2020   pad.....       
+00022950: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+00022960: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+00022970: 2020 2049 6d67 4172 7261 790d 0a20 2020     ImgArray..   
+00022980: 2020 2020 2020 2020 2050 6164 6465 6420           Padded 
+00022990: 696d 6167 652e 0d0a 2020 2020 2020 2020  image...        
+000229a0: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+000229b0: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
+000229c0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 5375  ----..        Su
+000229d0: 7070 6f73 6520 6060 696d 6760 6020 6861  ppose ``img`` ha
+000229e0: 7320 7a79 782d 6178 6573 2e0d 0a20 2020  s zyx-axes...   
+000229f0: 2020 2020 200d 0a20 2020 2020 2020 2031       ..        1
+00022a00: 2e20 5061 6464 696e 6720 3520 7069 7865  . Padding 5 pixe
+00022a10: 6c73 2069 6e20 7a79 782d 6469 7265 6374  ls in zyx-direct
+00022a20: 696f 6e3a 0d0a 2020 2020 2020 2020 2020  ion:..          
+00022a30: 2020 3e3e 3e20 696d 672e 7061 6428 3529    >>> img.pad(5)
+00022a40: 0d0a 2020 2020 2020 2020 322e 2050 6164  ..        2. Pad
+00022a50: 6469 6e67 2035 2070 6978 656c 7320 696e  ding 5 pixels in
+00022a60: 2079 782d 6469 7265 6374 696f 6e3a 0d0a   yx-direction:..
+00022a70: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00022a80: 696d 672e 7061 6428 352c 2064 696d 733d  img.pad(5, dims=
+00022a90: 2279 7822 290d 0a20 2020 2020 2020 2033  "yx")..        3
+00022aa0: 2e20 5061 6464 696e 6720 3520 7069 7865  . Padding 5 pixe
+00022ab0: 6c73 2069 6e20 7978 2d64 6972 6563 7469  ls in yx-directi
+00022ac0: 6f6e 2061 6e64 2032 2070 6978 656c 7320  on and 2 pixels 
+00022ad0: 696e 207a 2d64 6972 6563 7469 6f6e 3a0d  in z-direction:.
+00022ae0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00022af0: 2069 6d67 2e70 6164 285b 2835 2c35 292c   img.pad([(5,5),
+00022b00: 2028 342c 3429 2c20 2834 2c34 295d 290d   (4,4), (4,4)]).
+00022b10: 0a20 2020 2020 2020 2034 2e20 5061 6464  .        4. Padd
+00022b20: 696e 6720 3130 2070 6978 656c 7320 696e  ing 10 pixels in
+00022b30: 207a 2d28 2d29 2d64 6972 6563 7469 6f6e   z-(-)-direction
+00022b40: 2061 6e64 2035 2070 6978 656c 7320 696e   and 5 pixels in
+00022b50: 207a 2d28 2b29 2d64 6972 6563 7469 6f6e   z-(+)-direction
+00022b60: 2e0d 0a20 2020 2020 2020 2020 2020 203e  ...            >
+00022b70: 3e3e 2069 6d67 2e70 6164 285b 2831 302c  >> img.pad([(10,
+00022b80: 2035 295d 2c20 6469 6d73 3d22 7a22 290d   5)], dims="z").
+00022b90: 0a20 2020 2020 2020 2022 2222 2020 2020  .        """    
+00022ba0: 2020 2020 0d0a 2020 2020 2020 2020 7061      ..        pa
+00022bb0: 645f 7769 6474 6820 3d20 5f6d 6973 632e  d_width = _misc.
+00022bc0: 6d61 6b65 5f70 6164 2870 6164 5f77 6964  make_pad(pad_wid
+00022bd0: 7468 2c20 6469 6d73 2c20 7365 6c66 2e61  th, dims, self.a
+00022be0: 7865 732c 202a 2a6b 7761 7267 7329 0d0a  xes, **kwargs)..
+00022bf0: 2020 2020 2020 2020 7061 6469 6d67 203d          padimg =
+00022c00: 206e 702e 7061 6428 7365 6c66 2e76 616c   np.pad(self.val
+00022c10: 7565 2c20 7061 645f 7769 6474 682c 206d  ue, pad_width, m
+00022c20: 6f64 652c 202a 2a6b 7761 7267 7329 2e76  ode, **kwargs).v
+00022c30: 6965 7728 7365 6c66 2e5f 5f63 6c61 7373  iew(self.__class
+00022c40: 5f5f 290d 0a20 2020 2020 2020 2072 6574  __)..        ret
+00022c50: 7572 6e20 7061 6469 6d67 0d0a 2020 2020  urn padimg..    
+00022c60: 0d0a 2020 2020 4073 616d 655f 6474 7970  ..    @same_dtyp
+00022c70: 6528 6173 666c 6f61 743d 5472 7565 290d  e(asfloat=True).
+00022c80: 0a20 2020 2040 6368 6563 6b5f 696e 7075  .    @check_inpu
+00022c90: 745f 616e 645f 6f75 7470 7574 0d0a 2020  t_and_output..  
+00022ca0: 2020 6465 6620 7061 645f 6465 666f 6375    def pad_defocu
+00022cb0: 7328 7365 6c66 2c20 6b65 726e 656c 2c20  s(self, kernel, 
+00022cc0: 2a2c 2064 6570 7468 3a20 696e 7420 3d20  *, depth: int = 
+00022cd0: 332c 2077 6964 7468 3a20 696e 7420 3d20  3, width: int = 
+00022ce0: 362c 2062 673a 2066 6c6f 6174 203d 204e  6, bg: float = N
+00022cf0: 6f6e 6529 202d 3e20 496d 6741 7272 6179  one) -> ImgArray
+00022d00: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00022d10: 2020 2020 2020 2020 4d61 6b65 2061 207a          Make a z
+00022d20: 2d64 6972 6563 7469 6f6e 616c 2070 6164  -directional pad
+00022d30: 6465 6420 696d 6167 6520 6279 2064 6566  ded image by def
+00022d40: 6f63 7573 696e 6720 7468 6520 6f72 6967  ocusing the orig
+00022d50: 696e 616c 2069 6d61 6765 2e20 5468 6973  inal image. This
+00022d60: 2070 6164 6469 6e67 2069 730d 0a20 2020   padding is..   
+00022d70: 2020 2020 2075 7365 6675 6c20 7768 656e       useful when
+00022d80: 2061 7070 6c79 696e 6720 4646 5420 746f   applying FFT to
+00022d90: 2061 2033 4420 696d 6167 652e 0d0a 2020   a 3D image...  
+00022da0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00022db0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00022dc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00022dd0: 2020 2020 2020 2020 6b65 726e 656c 203a          kernel :
+00022de0: 2030 2d2c 2031 2d20 6f72 2033 2d64 696d   0-, 1- or 3-dim
+00022df0: 656e 7369 6f6e 616c 2061 7272 6179 2e0d  ensional array..
+00022e00: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00022e10: 302d 2028 7363 616c 6172 2920 6f72 2031  0- (scalar) or 1
+00022e20: 2d64 696d 656e 7369 6f6e 616c 2061 7272  -dimensional arr
+00022e30: 6179 2077 6173 2067 6976 656e 2c20 7468  ay was given, th
+00022e40: 6973 2069 7320 696e 7465 7270 7265 7465  is is interprete
+00022e50: 6420 6173 2073 7461 6e64 6172 640d 0a20  d as standard.. 
+00022e60: 2020 2020 2020 2020 2020 2064 6576 6961             devia
+00022e70: 7469 6f6e 206f 6620 4761 7573 7369 616e  tion of Gaussian
+00022e80: 206b 6572 6e65 6c2e 2049 6620 332d 6469   kernel. If 3-di
+00022e90: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
+00022ea0: 7761 7320 6769 7665 6e2c 2074 6869 7320  was given, this 
+00022eb0: 6973 2064 6972 6563 746c 790d 0a20 2020  is directly..   
+00022ec0: 2020 2020 2020 2020 2075 7365 6420 6173           used as
+00022ed0: 2063 6f6e 766f 6c75 7469 6f6e 206b 6572   convolution ker
+00022ee0: 6e65 6c2e 204f 7468 6572 2064 696d 656e  nel. Other dimen
+00022ef0: 7369 6f6e 2077 696c 6c20 7261 6973 6520  sion will raise 
+00022f00: 5661 6c75 6545 7272 6f72 2e0d 0a20 2020  ValueError...   
+00022f10: 2020 2020 2064 6570 7468 203a 2069 6e74       depth : int
+00022f20: 2c20 6465 6661 756c 7420 6973 2033 0d0a  , default is 3..
+00022f30: 2020 2020 2020 2020 2020 2020 4465 7074              Dept
+00022f40: 6820 6f66 2064 6566 6f63 7573 696e 672e  h of defocusing.
+00022f50: 2046 6f72 2061 6e20 696d 6167 6520 7769   For an image wi
+00022f60: 7468 207a 2d61 7869 7320 7369 7a65 204c  th z-axis size L
+00022f70: 2c20 7468 656e 206f 7574 7075 7420 696d  , then output im
+00022f80: 6167 6520 7769 6c6c 2068 6176 650d 0a20  age will have.. 
+00022f90: 2020 2020 2020 2020 2020 2073 697a 6520             size 
+00022fa0: 4c20 2b20 322a 6465 7074 682e 0d0a 2020  L + 2*depth...  
+00022fb0: 2020 2020 2020 7769 6474 6820 3a20 696e        width : in
+00022fc0: 742c 2064 6566 6175 6c74 2069 7320 360d  t, default is 6.
+00022fd0: 0a20 2020 2020 2020 2020 2020 2057 6964  .            Wid
+00022fe0: 7468 206f 6620 6465 666f 6375 7369 6e67  th of defocusing
+00022ff0: 2e20 466f 7220 616e 2069 6d61 6765 2077  . For an image w
+00023000: 6974 6820 7978 2d73 6861 7065 2028 4d2c  ith yx-shape (M,
+00023010: 204e 292c 2074 6865 6e20 6f75 7470 7574   N), then output
+00023020: 2069 6d61 6765 2077 696c 6c20 6861 7665   image will have
+00023030: 0d0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
+00023040: 6170 6520 284d 202a 2032 2a77 6964 7468  ape (M * 2*width
+00023050: 2c20 4e20 2b20 322a 7769 6474 6829 2e0d  , N + 2*width)..
+00023060: 0a20 2020 2020 2020 2062 6720 3a20 666c  .        bg : fl
+00023070: 6f61 742c 206f 7074 696f 6e61 6c0d 0a20  oat, optional.. 
+00023080: 2020 2020 2020 2020 2020 2042 6163 6b67             Backg
+00023090: 726f 756e 6420 696e 7465 6e73 6974 792e  round intensity.
+000230a0: 2049 6620 6e6f 7420 6769 7665 6e2c 2069   If not given, i
+000230b0: 7420 7769 6c6c 2063 616c 6375 6c61 7465  t will calculate
+000230c0: 6420 6173 2074 6865 206d 696e 696d 756d  d as the minimum
+000230d0: 2076 616c 7565 206f 6620 0d0a 2020 2020   value of ..    
+000230e0: 2020 2020 2020 2020 7468 6520 6f72 6967          the orig
+000230f0: 696e 616c 2069 6d61 6765 2e0d 0a0d 0a20  inal image..... 
+00023100: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+00023110: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+00023120: 0a20 2020 2020 2020 2049 6d67 4172 7261  .        ImgArra
+00023130: 790d 0a20 2020 2020 2020 2020 2020 2050  y..            P
+00023140: 6164 6465 6420 696d 6167 652e 0d0a 2020  added image...  
+00023150: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00023160: 2020 2020 4578 616d 706c 6573 0d0a 2020      Examples..  
+00023170: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
+00023180: 2020 2020 2020 2020 6465 7074 6820 3d20          depth = 
+00023190: 320d 0a20 2020 2020 2020 200d 0a20 2020  2..        ..   
+000231a0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
+000231b0: 636b 3a3a 0d0a 2020 2020 2020 2020 0d0a  ck::..        ..
+000231c0: 2020 2020 2020 2020 2020 2020 2d2d 2d2d              ----
+000231d0: 7c20 2020 7c2d 2d2d 2d7c 206f 207c 2d2d  |   |----| o |--
+000231e0: 2020 2020 206f 202e 2e2e 2063 656e 7465       o ... cente
+000231f0: 7220 6f66 206b 6572 6e65 6c0d 0a20 2020  r of kernel..   
+00023200: 2020 2020 2020 2020 202d 2d2d 2d7c 206f           ----| o
+00023210: 207c 2d2d 2d2d 7c20 2020 7c2d 2d0d 0a20   |----|   |--.. 
+00023220: 2020 2020 2020 2020 2020 202b 2b2b 2b7c             ++++|
+00023230: 2020 207c 2b2b 2b2b 7c5f 5f5f 7c2b 2b20     |++++|___|++ 
+00023240: 203c 2d20 7468 6520 7570 7065 7220 6564   <- the upper ed
+00023250: 6765 206f 6620 6f72 6967 696e 616c 2069  ge of original i
+00023260: 6d61 6765 200d 0a20 2020 2020 2020 2020  mage ..         
+00023270: 2020 202b 2b2b 2b7c 5f5f 5f7c 2b2b 2b2b     ++++|___|++++
+00023280: 2b2b 2b2b 2b2b 2b0d 0a0d 0a20 2020 2020  +++++++....     
+00023290: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000232a0: 6267 203d 205f 6368 6563 6b5f 6267 2873  bg = _check_bg(s
+000232b0: 656c 662c 2062 6729 0d0a 2020 2020 2020  elf, bg)..      
+000232c0: 2020 0d0a 2020 2020 2020 2020 6966 206e    ..        if n
+000232d0: 702e 6973 7363 616c 6172 286b 6572 6e65  p.isscalar(kerne
+000232e0: 6c29 3a0d 0a20 2020 2020 2020 2020 2020  l):..           
+000232f0: 206b 6572 6e65 6c20 3d20 6e70 2e61 7272   kernel = np.arr
+00023300: 6179 285b 6b65 726e 656c 5d2a 3329 0d0a  ay([kernel]*3)..
+00023310: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00023320: 2020 2020 2020 2020 2020 206b 6572 6e65             kerne
+00023330: 6c20 3d20 6e70 2e61 7361 7272 6179 286b  l = np.asarray(k
+00023340: 6572 6e65 6c29 0d0a 2020 2020 2020 2020  ernel)..        
+00023350: 0d0a 2020 2020 2020 2020 6966 206b 6572  ..        if ker
+00023360: 6e65 6c2e 6e64 696d 203c 3d20 313a 0d0a  nel.ndim <= 1:..
+00023370: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00023380: 6669 6c74 6572 5f66 756e 6328 696d 6729  filter_func(img)
+00023390: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000233a0: 2020 2072 6574 7572 6e20 7870 2e61 736e     return xp.asn
+000233b0: 756d 7079 285f 6669 6c74 6572 732e 6761  umpy(_filters.ga
+000233c0: 7573 7369 616e 5f66 696c 7465 7228 696d  ussian_filter(im
+000233d0: 672c 206b 6572 6e65 6c2c 206d 6f64 653d  g, kernel, mode=
+000233e0: 2263 6f6e 7374 616e 7422 2c20 6376 616c  "constant", cval
+000233f0: 3d62 6729 290d 0a20 2020 2020 2020 2020  =bg))..         
+00023400: 2020 2064 7a2c 2064 792c 2064 7820 3d20     dz, dy, dx = 
+00023410: 6b65 726e 656c 2a33 2023 2033 2d73 6967  kernel*3 # 3-sig
+00023420: 6d61 0d0a 2020 2020 2020 2020 2020 2020  ma..            
+00023430: 0d0a 2020 2020 2020 2020 656c 6966 206b  ..        elif k
+00023440: 6572 6e65 6c2e 6e64 696d 203d 3d20 333a  ernel.ndim == 3:
+00023450: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+00023460: 726e 656c 203d 206b 6572 6e65 6c2e 6173  rnel = kernel.as
+00023470: 7479 7065 286e 702e 666c 6f61 7433 3229  type(np.float32)
+00023480: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+00023490: 726e 656c 203d 206b 6572 6e65 6c20 2f20  rnel = kernel / 
+000234a0: 6e70 2e73 756d 286b 6572 6e65 6c29 0d0a  np.sum(kernel)..
+000234b0: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+000234c0: 6669 6c74 6572 5f66 756e 6328 696d 6729  filter_func(img)
+000234d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000234e0: 2020 2072 6574 7572 6e20 7870 2e61 736e     return xp.asn
+000234f0: 756d 7079 285f 6669 6c74 6572 732e 636f  umpy(_filters.co
+00023500: 6e76 6f6c 7665 2869 6d67 2c20 6b65 726e  nvolve(img, kern
+00023510: 656c 2c20 6d6f 6465 3d22 636f 6e73 7461  el, mode="consta
+00023520: 6e74 222c 2063 7661 6c3d 6267 2929 0d0a  nt", cval=bg))..
+00023530: 2020 2020 2020 2020 2020 2020 647a 2c20              dz, 
+00023540: 6479 2c20 6478 203d 206e 702e 6172 7261  dy, dx = np.arra
+00023550: 7928 6b65 726e 656c 2e73 6861 7065 292f  y(kernel.shape)/
+00023560: 2f32 0d0a 2020 2020 2020 2020 656c 7365  /2..        else
+00023570: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00023580: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00023590: 2260 6b65 726e 656c 6020 6f6e 6c79 2074  "`kernel` only t
+000235a0: 616b 6520 302c 2031 2c20 3320 6469 6d65  ake 0, 1, 3 dime
+000235b0: 6e73 696f 6e61 6c20 6172 7261 7920 6173  nsional array as
+000235c0: 2061 6e20 696e 7075 742e 2229 0d0a 2020   an input.")..  
+000235d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000235e0: 7061 645f 7769 6474 6820 3d20 5b28 6465  pad_width = [(de
+000235f0: 7074 682c 2064 6570 7468 292c 2028 7769  pth, depth), (wi
+00023600: 6474 682c 2077 6964 7468 292c 2028 7769  dth, width), (wi
+00023610: 6474 682c 2077 6964 7468 295d 0d0a 2020  dth, width)]..  
+00023620: 2020 2020 2020 7061 6469 6d67 203d 2073        padimg = s
+00023630: 656c 662e 7061 6428 7061 645f 7769 6474  elf.pad(pad_widt
+00023640: 682c 206d 6f64 653d 2263 6f6e 7374 616e  h, mode="constan
+00023650: 7422 2c20 636f 6e73 7461 6e74 5f76 616c  t", constant_val
+00023660: 7565 733d 6267 2c20 6469 6d73 3d22 7a79  ues=bg, dims="zy
+00023670: 7822 290d 0a20 2020 2020 2020 206f 7574  x")..        out
+00023680: 203d 206e 702e 636f 7079 2870 6164 696d   = np.copy(padim
+00023690: 672e 7661 6c75 6529 0d0a 2020 2020 2020  g.value)..      
+000236a0: 2020 2320 636f 6e76 6f6c 7665 2070 7366    # convolve psf
+000236b0: 0d0a 2020 2020 2020 2020 7a5f 6564 6765  ..        z_edge
+000236c0: 3020 3d20 736c 6963 6528 4e6f 6e65 2c20  0 = slice(None, 
+000236d0: 6465 7074 682c 204e 6f6e 6529 0d0a 2020  depth, None)..  
+000236e0: 2020 2020 2020 7a5f 6d69 6420 3d20 736c        z_mid = sl
+000236f0: 6963 6528 6465 7074 682c 202d 6465 7074  ice(depth, -dept
+00023700: 682c 204e 6f6e 6529 0d0a 2020 2020 2020  h, None)..      
+00023710: 2020 7a5f 6564 6765 3120 3d20 736c 6963    z_edge1 = slic
+00023720: 6528 2d64 6570 7468 2c20 4e6f 6e65 2c20  e(-depth, None, 
+00023730: 4e6f 6e65 290d 0a20 2020 2020 2020 2079  None)..        y
+00023740: 5f65 6467 6530 203d 2078 5f65 6467 6530  _edge0 = x_edge0
+00023750: 203d 2073 6c69 6365 284e 6f6e 652c 2077   = slice(None, w
+00023760: 6964 7468 2c20 4e6f 6e65 290d 0a20 2020  idth, None)..   
+00023770: 2020 2020 2079 5f6d 6964 203d 2073 6c69       y_mid = sli
+00023780: 6365 2877 6964 7468 2c20 2d77 6964 7468  ce(width, -width
+00023790: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
+000237a0: 2079 5f65 6467 6531 203d 2078 5f65 6467   y_edge1 = x_edg
+000237b0: 6531 203d 2073 6c69 6365 282d 7769 6474  e1 = slice(-widt
+000237c0: 682c 204e 6f6e 652c 204e 6f6e 6529 0d0a  h, None, None)..
+000237d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000237e0: 2020 666f 7220 736c 2c20 696d 6720 696e    for sl, img in
+000237f0: 2070 6164 696d 672e 6974 6572 2863 6f6d   padimg.iter(com
+00023800: 706c 656d 656e 745f 6178 6573 2822 7a79  plement_axes("zy
+00023810: 7822 2c20 7365 6c66 2e61 7865 7329 293a  x", self.axes)):
+00023820: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+00023830: 745f 203d 206f 7574 5b73 6c5d 0d0a 2020  t_ = out[sl]..  
+00023840: 2020 2020 2020 2020 2020 6f75 745f 5b7a            out_[z
+00023850: 5f65 6467 6530 5d20 3d20 6669 6c74 6572  _edge0] = filter
+00023860: 5f66 756e 6328 696d 675b 3a64 6570 7468  _func(img[:depth
+00023870: 2b64 7a20 5d29 5b7a 5f65 6467 6530 5d0d  +dz ])[z_edge0].
+00023880: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00023890: 5f5b 7a5f 6564 6765 315d 203d 2066 696c  _[z_edge1] = fil
+000238a0: 7465 725f 6675 6e63 2869 6d67 5b2d 6465  ter_func(img[-de
+000238b0: 7074 682d 647a 3a5d 295b 7a5f 6564 6765  pth-dz:])[z_edge
+000238c0: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
+000238d0: 6f75 745f 5b7a 5f6d 6964 2c20 795f 6564  out_[z_mid, y_ed
+000238e0: 6765 305d 203d 2066 696c 7465 725f 6675  ge0] = filter_fu
+000238f0: 6e63 2869 6d67 5b3a 2c20 3a77 6964 7468  nc(img[:, :width
+00023900: 2b64 7920 5d29 5b7a 5f6d 6964 2c20 795f  +dy ])[z_mid, y_
+00023910: 6564 6765 305d 0d0a 2020 2020 2020 2020  edge0]..        
+00023920: 2020 2020 6f75 745f 5b7a 5f6d 6964 2c20      out_[z_mid, 
+00023930: 795f 6564 6765 315d 203d 2066 696c 7465  y_edge1] = filte
+00023940: 725f 6675 6e63 2869 6d67 5b3a 2c20 2d77  r_func(img[:, -w
+00023950: 6964 7468 2d64 793a 5d29 5b7a 5f6d 6964  idth-dy:])[z_mid
+00023960: 2c20 795f 6564 6765 315d 0d0a 2020 2020  , y_edge1]..    
+00023970: 2020 2020 2020 2020 6f75 745f 5b7a 5f6d          out_[z_m
+00023980: 6964 2c20 795f 6d69 642c 2078 5f65 6467  id, y_mid, x_edg
+00023990: 6530 5d20 3d20 6669 6c74 6572 5f66 756e  e0] = filter_fun
+000239a0: 6328 696d 675b 3a2c 203a 2c20 3a77 6964  c(img[:, :, :wid
+000239b0: 7468 2b64 7820 5d29 5b7a 5f6d 6964 2c20  th+dx ])[z_mid, 
+000239c0: 795f 6d69 642c 2078 5f65 6467 6530 5d0d  y_mid, x_edge0].
+000239d0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000239e0: 5f5b 7a5f 6d69 642c 2079 5f6d 6964 2c20  _[z_mid, y_mid, 
+000239f0: 785f 6564 6765 315d 203d 2066 696c 7465  x_edge1] = filte
+00023a00: 725f 6675 6e63 2869 6d67 5b3a 2c20 3a2c  r_func(img[:, :,
+00023a10: 202d 7769 6474 682d 6478 3a5d 295b 7a5f   -width-dx:])[z_
+00023a20: 6d69 642c 2079 5f6d 6964 2c20 785f 6564  mid, y_mid, x_ed
+00023a30: 6765 315d 0d0a 2020 2020 2020 2020 2020  ge1]..          
+00023a40: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+00023a50: 726e 206f 7574 2e76 6965 7728 7365 6c66  rn out.view(self
+00023a60: 2e5f 5f63 6c61 7373 5f5f 290d 0a20 2020  .__class__)..   
+00023a70: 200d 0a20 2020 200d 0a20 2020 2040 5f64   ..    ..    @_d
+00023a80: 6f63 732e 7772 6974 655f 646f 6373 0d0a  ocs.write_docs..
+00023a90: 2020 2020 4064 696d 735f 746f 5f73 7061      @dims_to_spa
+00023aa0: 7469 616c 5f61 7865 730d 0a20 2020 2040  tial_axes..    @
+00023ab0: 7361 6d65 5f64 7479 7065 2861 7366 6c6f  same_dtype(asflo
+00023ac0: 6174 3d54 7275 6529 0d0a 2020 2020 4063  at=True)..    @c
+00023ad0: 6865 636b 5f69 6e70 7574 5f61 6e64 5f6f  heck_input_and_o
+00023ae0: 7574 7075 740d 0a20 2020 2064 6566 2077  utput..    def w
+00023af0: 6965 6e65 7228 0d0a 2020 2020 2020 2020  iener(..        
+00023b00: 7365 6c66 2c0d 0a20 2020 2020 2020 2070  self,..        p
+00023b10: 7366 3a20 6e70 2e6e 6461 7272 6179 207c  sf: np.ndarray |
+00023b20: 2043 616c 6c61 626c 655b 5b74 7570 6c65   Callable[[tuple
+00023b30: 5b69 6e74 2c20 2e2e 2e5d 5d2c 206e 702e  [int, ...]], np.
+00023b40: 6e64 6172 7261 795d 2c0d 0a20 2020 2020  ndarray],..     
+00023b50: 2020 206c 6d64 3a20 666c 6f61 7420 3d20     lmd: float = 
+00023b60: 302e 312c 0d0a 2020 2020 2020 2020 2a2c  0.1,..        *,
+00023b70: 200d 0a20 2020 2020 2020 2064 696d 733a   ..        dims:
+00023b80: 2044 696d 7320 3d20 4e6f 6e65 2c20 0d0a   Dims = None, ..
+00023b90: 2020 2020 2020 2020 7570 6461 7465 3a20          update: 
+00023ba0: 626f 6f6c 203d 2046 616c 7365 0d0a 2020  bool = False..  
+00023bb0: 2020 2920 2d3e 2049 6d67 4172 7261 793a    ) -> ImgArray:
+00023bc0: 0d0a 2020 2020 2020 2020 7222 2222 0d0a  ..        r"""..
+00023bd0: 2020 2020 2020 2020 436c 6173 7369 6361          Classica
+00023be0: 6c20 7769 656e 6572 2064 6563 6f6e 766f  l wiener deconvo
+00023bf0: 6c75 7469 6f6e 2e20 5468 6973 2061 6c67  lution. This alg
+00023c00: 6f72 6974 686d 2068 6173 2074 6865 2073  orithm has the s
+00023c10: 6572 696f 7573 2072 696e 6769 6e67 2070  erious ringing p
+00023c20: 726f 626c 656d 0d0a 2020 2020 2020 2020  roblem..        
+00023c30: 6966 2070 6172 616d 6574 6572 7320 6172  if parameters ar
+00023c40: 6520 7365 7420 746f 2077 726f 6e67 2076  e set to wrong v
+00023c50: 616c 7565 732e 0d0a 2020 2020 2020 2020  alues...        
+00023c60: 0d0a 2020 2020 2020 2020 3a6d 6174 683a  ..        :math:
+00023c70: 6046 5b59 5f7b 7265 737d 5d20 3d20 5c66  `F[Y_{res}] = \f
+00023c80: 7261 637b 465b 595f 7b6f 6273 7d5d 205c  rac{F[Y_{obs}] \
+00023c90: 6364 6f74 205c 6261 727b 487d 7d7b 7c48  cdot \bar{H}}{|H
+00023ca0: 7c5e 3220 2b20 5c6c 616d 6264 617d 600d  |^2 + \lambda}`.
+00023cb0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00023cc0: 2020 2020 2020 203a 6d61 7468 3a60 595f         :math:`Y_
+00023cd0: 7b6f 6273 7d60 3a20 6f62 7365 7276 6564  {obs}`: observed
+00023ce0: 2069 6d61 6765 3b0d 0a20 2020 2020 2020   image;..       
+00023cf0: 203a 6d61 7468 3a60 595f 7b72 6573 7d60   :math:`Y_{res}`
+00023d00: 3a20 7265 7374 6f72 6564 2069 6d61 6765  : restored image
+00023d10: 3b0d 0a20 2020 2020 2020 203a 6d61 7468  ;..        :math
+00023d20: 3a60 4860 203a 2046 4654 206f 6620 706f  :`H` : FFT of po
+00023d30: 696e 7420 7370 7265 6164 2066 756e 6374  int spread funct
+00023d40: 696f 6e20 2850 5346 293b 0d0a 0d0a 2020  ion (PSF);....  
+00023d50: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00023d60: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00023d70: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7073  ----..        ps
+00023d80: 6620 3a20 6e64 6172 7261 7920 6f72 2063  f : ndarray or c
+00023d90: 616c 6c61 626c 650d 0a20 2020 2020 2020  allable..       
+00023da0: 2020 2020 2050 6f69 6e74 2073 7072 6561       Point sprea
+00023db0: 6420 6675 6e63 7469 6f6e 2e20 4966 2061  d function. If a
+00023dc0: 2066 756e 6374 696f 6e20 6973 2067 6976   function is giv
+00023dd0: 656e 2c20 6070 7366 2873 6861 7065 2960  en, `psf(shape)`
+00023de0: 2077 696c 6c20 6265 0d0a 2020 2020 2020   will be..      
+00023df0: 2020 2020 2020 6361 6c6c 6564 2074 6f20        called to 
+00023e00: 6765 6e65 7261 7465 2074 6865 2050 5346  generate the PSF
+00023e10: 2e0d 0a20 2020 2020 2020 206c 6d64 203a  ...        lmd :
+00023e20: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+00023e30: 6973 2030 2e31 0d0a 2020 2020 2020 2020  is 0.1..        
+00023e40: 2020 2020 436f 6e73 7461 6e74 2076 616c      Constant val
+00023e50: 7565 2075 7365 6420 696e 2074 6865 2064  ue used in the d
+00023e60: 6563 6f6e 766f 6c75 7469 6f6e 2e20 5365  econvolution. Se
+00023e70: 6520 466f 726d 756c 6174 696f 6e20 6265  e Formulation be
+00023e80: 6c6f 772e 0d0a 2020 2020 2020 2020 7b64  low...        {d
+00023e90: 696d 737d 7b75 7064 6174 657d 0d0a 0d0a  ims}{update}....
+00023ea0: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+00023eb0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00023ec0: 0d0a 2020 2020 2020 2020 496d 6741 7272  ..        ImgArr
+00023ed0: 6179 0d0a 2020 2020 2020 2020 2020 2020  ay..            
+00023ee0: 4465 636f 6e76 6f6c 7665 6420 696d 6167  Deconvolved imag
+00023ef0: 652e 0d0a 2020 2020 2020 2020 0d0a 2020  e...        ..  
+00023f00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00023f10: 5365 6520 416c 736f 0d0a 2020 2020 2020  See Also..      
+00023f20: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00023f30: 2020 2020 6c75 6379 0d0a 2020 2020 2020      lucy..      
+00023f40: 2020 6c75 6379 5f74 760d 0a20 2020 2020    lucy_tv..     
+00023f50: 2020 2022 2222 2020 2020 2020 2020 0d0a     """        ..
+00023f60: 2020 2020 2020 2020 6966 206c 6d64 203c          if lmd <
+00023f70: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00023f80: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00023f90: 6f72 2866 226c 6d64 206d 7573 7420 6265  or(f"lmd must be
+00023fa0: 2070 6f73 6974 6976 652c 2062 7574 2067   positive, but g
+00023fb0: 6f74 3a20 7b6c 6d64 7d22 290d 0a20 2020  ot: {lmd}")..   
+00023fc0: 2020 2020 200d 0a20 2020 2020 2020 2070       ..        p
+00023fd0: 7366 5f66 742c 2070 7366 5f66 745f 636f  sf_ft, psf_ft_co
+00023fe0: 6e6a 203d 205f 6465 636f 6e76 2e63 6865  nj = _deconv.che
+00023ff0: 636b 5f70 7366 280d 0a20 2020 2020 2020  ck_psf(..       
+00024000: 2020 2020 2073 656c 662e 7369 7a65 736f       self.sizeso
+00024010: 6628 6469 6d73 292c 2074 7570 6c65 2873  f(dims), tuple(s
+00024020: 656c 662e 7363 616c 655b 6178 6973 5d20  elf.scale[axis] 
+00024030: 666f 7220 6178 6973 2069 6e20 6469 6d73  for axis in dims
+00024040: 292c 2070 7366 2c0d 0a20 2020 2020 2020  ), psf,..       
+00024050: 2029 0d0a 2020 2020 2020 2020 0d0a 2020   )..        ..  
+00024060: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00024070: 662e 5f61 7070 6c79 5f64 6173 6b28 0d0a  f._apply_dask(..
+00024080: 2020 2020 2020 2020 2020 2020 5f64 6563              _dec
+00024090: 6f6e 762e 7769 656e 6572 2c20 0d0a 2020  onv.wiener, ..  
+000240a0: 2020 2020 2020 2020 2020 635f 6178 6573            c_axes
+000240b0: 3d63 6f6d 706c 656d 656e 745f 6178 6573  =complement_axes
+000240c0: 2864 696d 732c 2073 656c 662e 6178 6573  (dims, self.axes
+000240d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000240e0: 6172 6773 3d28 7073 665f 6674 2c20 7073  args=(psf_ft, ps
+000240f0: 665f 6674 5f63 6f6e 6a2c 206c 6d64 290d  f_ft_conj, lmd).
+00024100: 0a20 2020 2020 2020 2029 2020 2020 0d0a  .        )    ..
+00024110: 0d0a 2020 2020 405f 646f 6373 2e77 7269  ..    @_docs.wri
+00024120: 7465 5f64 6f63 730d 0a20 2020 2040 6469  te_docs..    @di
+00024130: 6d73 5f74 6f5f 7370 6174 6961 6c5f 6178  ms_to_spatial_ax
+00024140: 6573 0d0a 2020 2020 4073 616d 655f 6474  es..    @same_dt
+00024150: 7970 6528 6173 666c 6f61 743d 5472 7565  ype(asfloat=True
+00024160: 290d 0a20 2020 2040 6368 6563 6b5f 696e  )..    @check_in
+00024170: 7075 745f 616e 645f 6f75 7470 7574 0d0a  put_and_output..
+00024180: 2020 2020 6465 6620 6c75 6379 280d 0a20      def lucy(.. 
+00024190: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+000241a0: 2020 2020 2020 7073 663a 206e 702e 6e64        psf: np.nd
+000241b0: 6172 7261 7920 7c20 4361 6c6c 6162 6c65  array | Callable
+000241c0: 5b5b 7475 706c 655b 696e 742c 202e 2e2e  [[tuple[int, ...
+000241d0: 5d5d 2c20 6e70 2e6e 6461 7272 6179 5d2c  ]], np.ndarray],
+000241e0: 0d0a 2020 2020 2020 2020 6e69 7465 723a  ..        niter:
+000241f0: 2069 6e74 203d 2035 302c 0d0a 2020 2020   int = 50,..    
+00024200: 2020 2020 6570 733a 2066 6c6f 6174 203d      eps: float =
+00024210: 2031 652d 352c 0d0a 2020 2020 2020 2020   1e-5,..        
+00024220: 2a2c 200d 0a20 2020 2020 2020 2064 696d  *, ..        dim
+00024230: 733a 2044 696d 7320 3d20 4e6f 6e65 2c20  s: Dims = None, 
+00024240: 0d0a 2020 2020 2020 2020 7570 6461 7465  ..        update
+00024250: 3a20 626f 6f6c 203d 2046 616c 7365 0d0a  : bool = False..
+00024260: 2020 2020 2920 2d3e 2049 6d67 4172 7261      ) -> ImgArra
+00024270: 793a 0d0a 2020 2020 2020 2020 2222 220d  y:..        """.
+00024280: 0a20 2020 2020 2020 2044 6563 6f6e 766f  .        Deconvo
+00024290: 6c75 7469 6f6e 206f 6620 4e2d 6469 6d65  lution of N-dime
+000242a0: 6e73 696f 6e61 6c20 696d 6167 652c 2075  nsional image, u
+000242b0: 7369 6e67 2052 6963 6861 7264 736f 6e2d  sing Richardson-
+000242c0: 4c75 6379 2773 2061 6c67 6f72 6974 686d  Lucy's algorithm
+000242d0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
+000242e0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+000242f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00024300: 2d2d 2d0d 0a20 2020 2020 2020 2070 7366  ---..        psf
+00024310: 203a 206e 6461 7272 6179 206f 7220 6361   : ndarray or ca
+00024320: 6c6c 6162 6c65 0d0a 2020 2020 2020 2020  llable..        
+00024330: 2020 2020 506f 696e 7420 7370 7265 6164      Point spread
+00024340: 2066 756e 6374 696f 6e2e 2049 6620 6120   function. If a 
+00024350: 6675 6e63 7469 6f6e 2069 7320 6769 7665  function is give
+00024360: 6e2c 2060 7073 6628 7368 6170 6529 6020  n, `psf(shape)` 
+00024370: 7769 6c6c 2062 650d 0a20 2020 2020 2020  will be..       
+00024380: 2020 2020 2063 616c 6c65 6420 746f 2067       called to g
+00024390: 656e 6572 6174 6520 7468 6520 5053 462e  enerate the PSF.
+000243a0: 0d0a 2020 2020 2020 2020 6e69 7465 7220  ..        niter 
+000243b0: 3a20 696e 742c 2064 6566 6175 6c74 2069  : int, default i
+000243c0: 7320 3530 2e0d 0a20 2020 2020 2020 2020  s 50...         
+000243d0: 2020 204e 756d 6265 7220 6f66 2069 7465     Number of ite
+000243e0: 7261 7469 6f6e 732e 0d0a 2020 2020 2020  rations...      
+000243f0: 2020 6570 7320 3a20 666c 6f61 742c 2064    eps : float, d
+00024400: 6566 6175 6c74 2069 7320 3165 2d35 0d0a  efault is 1e-5..
+00024410: 2020 2020 2020 2020 2020 2020 4475 7269              Duri
+00024420: 6e67 2064 6563 6f6e 766f 6c75 7469 6f6e  ng deconvolution
+00024430: 2c20 6469 7669 7369 6f6e 2062 7920 736d  , division by sm
+00024440: 616c 6c20 7661 6c75 6573 2069 6e20 7468  all values in th
+00024450: 6520 636f 6e76 6f6c 7665 2069 6d61 6765  e convolve image
+00024460: 200d 0a20 2020 2020 2020 2020 2020 206f   ..            o
+00024470: 6620 6573 7469 6d61 7469 6f6e 2061 6e64  f estimation and
+00024480: 2050 5346 206d 6179 2063 6175 7365 2064   PSF may cause d
+00024490: 6976 6572 6765 6e63 652e 2054 6865 7265  ivergence. There
+000244a0: 666f 7265 2c20 6469 7669 7369 6f6e 2062  fore, division b
+000244b0: 7920 0d0a 2020 2020 2020 2020 2020 2020  y ..            
+000244c0: 7661 6c75 6573 2075 6e64 6572 2060 6570  values under `ep
+000244d0: 7360 2069 7320 7375 6273 7469 7475 7465  s` is substitute
+000244e0: 6420 746f 207a 6572 6f2e 0d0a 2020 2020  d to zero...    
+000244f0: 2020 2020 7b64 696d 737d 7b75 7064 6174      {dims}{updat
+00024500: 657d 0d0a 2020 2020 2020 2020 0d0a 2020  e}..        ..  
+00024510: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+00024520: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+00024530: 2020 2020 2020 2020 496d 6741 7272 6179          ImgArray
+00024540: 0d0a 2020 2020 2020 2020 2020 2020 4465  ..            De
+00024550: 636f 6e76 6f6c 7665 6420 696d 6167 652e  convolved image.
+00024560: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00024570: 2020 2020 5365 6520 416c 736f 0d0a 2020      See Also..  
+00024580: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
+00024590: 2020 2020 2020 2020 6c75 6379 5f74 760d          lucy_tv.
+000245a0: 0a20 2020 2020 2020 2077 6965 6e65 720d  .        wiener.
+000245b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000245c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000245d0: 7073 665f 6674 2c20 7073 665f 6674 5f63  psf_ft, psf_ft_c
+000245e0: 6f6e 6a20 3d20 5f64 6563 6f6e 762e 6368  onj = _deconv.ch
+000245f0: 6563 6b5f 7073 6628 0d0a 2020 2020 2020  eck_psf(..      
+00024600: 2020 2020 2020 7365 6c66 2e73 697a 6573        self.sizes
+00024610: 6f66 2864 696d 7329 2c20 7475 706c 6528  of(dims), tuple(
+00024620: 7365 6c66 2e73 6361 6c65 5b61 7869 735d  self.scale[axis]
+00024630: 2066 6f72 2061 7869 7320 696e 2064 696d   for axis in dim
+00024640: 7329 2c20 7073 662c 0d0a 2020 2020 2020  s), psf,..      
+00024650: 2020 290d 0a0d 0a20 2020 2020 2020 2072    )....        r
+00024660: 6574 7572 6e20 7365 6c66 2e5f 6170 706c  eturn self._appl
+00024670: 795f 6461 736b 280d 0a20 2020 2020 2020  y_dask(..       
+00024680: 2020 2020 205f 6465 636f 6e76 2e72 6963       _deconv.ric
+00024690: 6861 7264 736f 6e5f 6c75 6379 2c20 0d0a  hardson_lucy, ..
+000246a0: 2020 2020 2020 2020 2020 2020 635f 6178              c_ax
+000246b0: 6573 3d63 6f6d 706c 656d 656e 745f 6178  es=complement_ax
+000246c0: 6573 2864 696d 732c 2073 656c 662e 6178  es(dims, self.ax
+000246d0: 6573 292c 0d0a 2020 2020 2020 2020 2020  es),..          
+000246e0: 2020 6172 6773 3d28 7073 665f 6674 2c20    args=(psf_ft, 
+000246f0: 7073 665f 6674 5f63 6f6e 6a2c 206e 6974  psf_ft_conj, nit
+00024700: 6572 2c20 6570 7329 0d0a 2020 2020 2020  er, eps)..      
+00024710: 2020 290d 0a20 2020 2020 2020 200d 0a20    )..        .. 
+00024720: 2020 2040 5f64 6f63 732e 7772 6974 655f     @_docs.write_
+00024730: 646f 6373 0d0a 2020 2020 4064 696d 735f  docs..    @dims_
+00024740: 746f 5f73 7061 7469 616c 5f61 7865 730d  to_spatial_axes.
+00024750: 0a20 2020 2040 7361 6d65 5f64 7479 7065  .    @same_dtype
+00024760: 2861 7366 6c6f 6174 3d54 7275 6529 0d0a  (asfloat=True)..
+00024770: 2020 2020 4063 6865 636b 5f69 6e70 7574      @check_input
+00024780: 5f61 6e64 5f6f 7574 7075 740d 0a20 2020  _and_output..   
+00024790: 2064 6566 206c 7563 795f 7476 280d 0a20   def lucy_tv(.. 
+000247a0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+000247b0: 2020 2020 2020 7073 663a 206e 702e 6e64        psf: np.nd
+000247c0: 6172 7261 7920 7c20 4361 6c6c 6162 6c65  array | Callable
+000247d0: 5b5b 7475 706c 655b 696e 742c 202e 2e2e  [[tuple[int, ...
+000247e0: 5d5d 2c20 6e70 2e6e 6461 7272 6179 5d2c  ]], np.ndarray],
+000247f0: 0d0a 2020 2020 2020 2020 6d61 785f 6974  ..        max_it
+00024800: 6572 3a20 696e 7420 3d20 3530 2c0d 0a20  er: int = 50,.. 
+00024810: 2020 2020 2020 206c 6d64 3a20 666c 6f61         lmd: floa
+00024820: 7420 3d20 3165 2d33 2c0d 0a20 2020 2020  t = 1e-3,..     
+00024830: 2020 2074 6f6c 3a20 666c 6f61 7420 3d20     tol: float = 
+00024840: 3165 2d33 2c0d 0a20 2020 2020 2020 2065  1e-3,..        e
+00024850: 7073 3a20 666c 6f61 7420 3d20 3165 2d35  ps: float = 1e-5
+00024860: 2c0d 0a20 2020 2020 2020 202a 2c0d 0a20  ,..        *,.. 
+00024870: 2020 2020 2020 2064 696d 733a 2044 696d         dims: Dim
+00024880: 7320 3d20 4e6f 6e65 2c0d 0a20 2020 2020  s = None,..     
+00024890: 2020 2075 7064 6174 653a 2062 6f6f 6c20     update: bool 
+000248a0: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
+000248b0: 3e20 496d 6741 7272 6179 3a0d 0a20 2020  > ImgArray:..   
+000248c0: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
+000248d0: 2020 2044 6563 6f6e 766f 6c75 7469 6f6e     Deconvolution
+000248e0: 206f 6620 4e2d 6469 6d65 6e73 696f 6e61   of N-dimensiona
+000248f0: 6c20 696d 6167 652c 2075 7369 6e67 2052  l image, using R
+00024900: 6963 6861 7264 736f 6e2d 4c75 6379 2773  ichardson-Lucy's
+00024910: 2061 6c67 6f72 6974 686d 2077 6974 680d   algorithm with.
+00024920: 0a20 2020 2020 2020 2074 6f74 616c 2076  .        total v
+00024930: 6172 6961 6e63 6520 7265 6775 6c61 7269  ariance regulari
+00024940: 7a61 7469 6f6e 2028 736f 2063 616c 6c65  zation (so calle
+00024950: 6420 524c 2d54 5620 616c 676f 7269 7468  d RL-TV algorith
+00024960: 6d29 2e20 5468 6520 5456 2072 6567 756c  m). The TV regul
+00024970: 6172 697a 6174 696f 6e0d 0a20 2020 2020  arization..     
+00024980: 2020 2066 6163 746f 7220 6174 2070 6978     factor at pix
+00024990: 656c 2070 6f73 6974 696f 6e20 3a6d 6174  el position :mat
+000249a0: 683a 6078 602c 203a 6d61 7468 3a60 465f  h:`x`, :math:`F_
+000249b0: 7b72 6567 7d28 7829 602c 2069 7320 6361  {reg}(x)`, is ca
+000249c0: 6c63 756c 6174 6564 2061 733a 0d0a 2020  lculated as:..  
+000249d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000249e0: 2e2e 206d 6174 683a 3a0d 0a20 2020 2020  .. math::..     
+000249f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00024a00: 2020 2020 2046 5f7b 7265 677d 2878 2920       F_{reg}(x) 
+00024a10: 3d20 5c66 7261 637b 317d 7b31 2d5c 6c61  = \frac{1}{1-\la
+00024a20: 6d62 6461 205c 6364 6f74 2064 6976 285c  mbda \cdot div(\
+00024a30: 6672 6163 7b67 7261 6428 4928 7829 7d7b  frac{grad(I(x)}{
+00024a40: 7c67 7261 6428 4928 7829 297c 7d29 7d0d  |grad(I(x))|})}.
+00024a50: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00024a60: 2020 2028 3a6d 6174 683a 6049 2878 2960     (:math:`I(x)`
+00024a70: 3a20 696d 6167 652c 203a 6d61 7468 3a60  : image, :math:`
+00024a80: 5c6c 616d 6264 6160 3a20 636f 6e73 7461  \lambda`: consta
+00024a90: 6e74 290d 0a20 2020 2020 2020 200d 0a20  nt)..        .. 
+00024aa0: 2020 2020 2020 2061 6e64 2074 6869 7320         and this 
+00024ab0: 6661 6374 6f72 2069 7320 6d75 6c74 6970  factor is multip
+00024ac0: 6c69 6564 2066 6f72 2065 7665 7279 2065  lied for every e
+00024ad0: 7374 696d 6174 696f 6e20 6d61 6465 2069  stimation made i
+00024ae0: 6e20 6561 6368 2069 7465 7261 7469 6f6e  n each iteration
+00024af0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
+00024b00: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+00024b10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00024b20: 2d2d 2d0d 0a20 2020 2020 2020 2070 7366  ---..        psf
+00024b30: 203a 206e 6461 7272 6179 206f 7220 6361   : ndarray or ca
+00024b40: 6c6c 6162 6c65 0d0a 2020 2020 2020 2020  llable..        
+00024b50: 2020 2020 506f 696e 7420 7370 7265 6164      Point spread
+00024b60: 2066 756e 6374 696f 6e2e 2049 6620 6120   function. If a 
+00024b70: 6675 6e63 7469 6f6e 2069 7320 6769 7665  function is give
+00024b80: 6e2c 2060 7073 6628 7368 6170 6529 6020  n, `psf(shape)` 
+00024b90: 7769 6c6c 2062 650d 0a20 2020 2020 2020  will be..       
+00024ba0: 2020 2020 2063 616c 6c65 6420 746f 2067       called to g
+00024bb0: 656e 6572 6174 6520 7468 6520 5053 462e  enerate the PSF.
+00024bc0: 0d0a 2020 2020 2020 2020 6d61 785f 6974  ..        max_it
+00024bd0: 6572 203a 2069 6e74 2c20 6465 6661 756c  er : int, defaul
+00024be0: 7420 6973 2035 302e 0d0a 2020 2020 2020  t is 50...      
+00024bf0: 2020 2020 2020 4d61 7869 6d75 6d20 6e75        Maximum nu
+00024c00: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+00024c10: 6e73 2e0d 0a20 2020 2020 2020 206c 6d64  ns...        lmd
+00024c20: 203a 2066 6c6f 6174 2c20 6465 6661 756c   : float, defaul
+00024c30: 7420 6973 2031 652d 330d 0a20 2020 2020  t is 1e-3..     
+00024c40: 2020 2020 2020 2054 6865 2063 6f6e 7374         The const
+00024c50: 616e 7420 6c61 6d62 6461 206f 6620 5456  ant lambda of TV
+00024c60: 2072 6567 756c 6172 697a 6174 696f 6e20   regularization 
+00024c70: 6661 6374 6f72 2e0d 0a20 2020 2020 2020  factor...       
+00024c80: 2074 6f6c 203a 2066 6c6f 6174 2c20 6465   tol : float, de
+00024c90: 6661 756c 7420 6973 2031 652d 330d 0a20  fault is 1e-3.. 
+00024ca0: 2020 2020 2020 2020 2020 2049 7465 7261             Itera
+00024cb0: 7469 6f6e 2073 746f 7073 2069 6620 7265  tion stops if re
+00024cc0: 6775 6c61 7269 7a65 6420 6162 736f 6c75  gularized absolu
+00024cd0: 7465 2073 756d 6d61 7469 6f6e 2069 7320  te summation is 
+00024ce0: 6c6f 7765 7220 7468 616e 2074 6869 7320  lower than this 
+00024cf0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00024d00: 6c75 652e 0d0a 2020 2020 2020 2020 2020  lue...          
+00024d10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00024d20: 3a6d 6174 683a 605c 6672 6163 7b5c 7375  :math:`\frac{\su
+00024d30: 6d5f 7b78 7d7c 4927 2878 2920 2d20 4928  m_{x}|I'(x) - I(
+00024d40: 7829 7c7d 7b5c 7375 6d5f 7b78 7d7c 4928  x)|}{\sum_{x}|I(
+00024d50: 7829 7c7d 600d 0a20 2020 2020 2020 2020  x)|}`..         
+00024d60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00024d70: 2028 3a6d 6174 683a 6049 2728 7829 603a   (:math:`I'(x)`:
+00024d80: 2065 7374 696d 6174 696f 6e20 6f66 203a   estimation of :
+00024d90: 6d61 7468 3a60 6b2b 3160 2d74 6820 6974  math:`k+1`-th it
+00024da0: 6572 6174 696f 6e2c 203a 6d61 7468 3a60  eration, :math:`
+00024db0: 4928 7829 603a 200d 0a20 2020 2020 2020  I(x)`: ..       
+00024dc0: 2020 2020 2065 7374 696d 6174 696f 6e20       estimation 
+00024dd0: 6f66 203a 6d61 7468 3a60 6b60 2d74 6820  of :math:`k`-th 
+00024de0: 6974 6572 6174 696f 6e29 0d0a 2020 2020  iteration)..    
+00024df0: 2020 2020 0d0a 2020 2020 2020 2020 6570      ..        ep
+00024e00: 7320 3a20 666c 6f61 742c 2064 6566 6175  s : float, defau
+00024e10: 6c74 2069 7320 3165 2d35 0d0a 2020 2020  lt is 1e-5..    
+00024e20: 2020 2020 2020 2020 4475 7269 6e67 2064          During d
+00024e30: 6563 6f6e 766f 6c75 7469 6f6e 2c20 6469  econvolution, di
+00024e40: 7669 7369 6f6e 2062 7920 736d 616c 6c20  vision by small 
+00024e50: 7661 6c75 6573 2069 6e20 7468 6520 636f  values in the co
+00024e60: 6e76 6f6c 7665 2069 6d61 6765 206f 660d  nvolve image of.
+00024e70: 0a20 2020 2020 2020 2020 2020 2065 7374  .            est
+00024e80: 696d 6174 696f 6e20 616e 6420 5053 4620  imation and PSF 
+00024e90: 6d61 7920 6361 7573 6520 6469 7665 7267  may cause diverg
+00024ea0: 656e 6365 2e20 5468 6572 6566 6f72 652c  ence. Therefore,
+00024eb0: 2064 6976 6973 696f 6e20 6279 2076 616c   division by val
+00024ec0: 7565 7320 0d0a 2020 2020 2020 2020 2020  ues ..          
+00024ed0: 2020 756e 6465 7220 6060 6570 7360 6020    under ``eps`` 
+00024ee0: 6973 2073 7562 7374 6974 7574 6564 2074  is substituted t
+00024ef0: 6f20 7a65 726f 2e0d 0a20 2020 2020 2020  o zero...       
+00024f00: 207b 6469 6d73 7d7b 7570 6461 7465 7d0d   {dims}{update}.
+00024f10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00024f20: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+00024f30: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00024f40: 2020 2020 2049 6d67 4172 7261 790d 0a20       ImgArray.. 
+00024f50: 2020 2020 2020 2020 2020 2044 6563 6f6e             Decon
+00024f60: 766f 6c76 6564 2069 6d61 6765 2e0d 0a20  volved image... 
+00024f70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00024f80: 2052 6566 6572 656e 6365 730d 0a20 2020   References..   
+00024f90: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+00024fa0: 0a20 2020 2020 2020 202d 2044 6579 2c20  .        - Dey, 
+00024fb0: 4e2e 2c20 426c 616e 632d 46c3 a972 6175  N., Blanc-F..rau
+00024fc0: 642c 204c 2e2c 205a 696d 6d65 722c 2043  d, L., Zimmer, C
+00024fd0: 2e2c 2052 6f75 782c 2050 2e2c 204b 616d  ., Roux, P., Kam
+00024fe0: 2c20 5a2e 2c20 4f6c 6976 6f2d 4d61 7269  , Z., Olivo-Mari
+00024ff0: 6e2c 204a 2e20 432e 2c20 0d0a 2020 2020  n, J. C., ..    
+00025000: 2020 2020 2020 2620 5a65 7275 6269 612c        & Zerubia,
+00025010: 204a 2e20 2832 3030 3429 2e20 3344 206d   J. (2004). 3D m
+00025020: 6963 726f 7363 6f70 7920 6465 636f 6e76  icroscopy deconv
+00025030: 6f6c 7574 696f 6e20 7573 696e 6720 5269  olution using Ri
+00025040: 6368 6172 6473 6f6e 2d4c 7563 7920 616c  chardson-Lucy al
+00025050: 676f 7269 7468 6d20 0d0a 2020 2020 2020  gorithm ..      
+00025060: 2020 2020 7769 7468 2074 6f74 616c 2076      with total v
+00025070: 6172 6961 7469 6f6e 2072 6567 756c 6172  ariation regular
+00025080: 697a 6174 696f 6e20 2844 6f63 746f 7261  ization (Doctora
+00025090: 6c20 6469 7373 6572 7461 7469 6f6e 2c20  l dissertation, 
+000250a0: 494e 5249 4129 2e0d 0a20 2020 2020 2020  INRIA)...       
+000250b0: 200d 0a20 2020 2020 2020 2053 6565 2041   ..        See A
+000250c0: 6c73 6f0d 0a20 2020 2020 2020 202d 2d2d  lso..        ---
+000250d0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 206c  -----..        l
+000250e0: 7563 790d 0a20 2020 2020 2020 2077 6965  ucy..        wie
+000250f0: 6e65 720d 0a20 2020 2020 2020 2022 2222  ner..        """
+00025100: 0d0a 2020 2020 2020 2020 6966 206c 6d64  ..        if lmd
+00025110: 203c 3d20 303a 0d0a 2020 2020 2020 2020   <= 0:..        
+00025120: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00025130: 7272 6f72 280d 0a20 2020 2020 2020 2020  rror(..         
+00025140: 2020 2020 2020 2022 496e 2052 6963 6861         "In Richa
+00025150: 6473 6f6e 2d4c 7563 7920 7769 7468 2074  dson-Lucy with t
+00025160: 6f74 616c 2d76 6172 6961 6e63 652d 7265  otal-variance-re
+00025170: 6775 6c61 7269 7a61 7469 6f6e 2c20 220d  gularization, ".
+00025180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025190: 2022 7061 7261 6d65 7465 7220 606c 6d64   "parameter `lmd
+000251a0: 6020 6d75 7374 2062 6520 706f 7369 7469  ` must be positi
+000251b0: 7665 2e22 0d0a 2020 2020 2020 2020 2020  ve."..          
+000251c0: 2020 290d 0a20 2020 2020 2020 2070 7366    )..        psf
+000251d0: 5f66 742c 2070 7366 5f66 745f 636f 6e6a  _ft, psf_ft_conj
+000251e0: 203d 205f 6465 636f 6e76 2e63 6865 636b   = _deconv.check
+000251f0: 5f70 7366 280d 0a20 2020 2020 2020 2020  _psf(..         
+00025200: 2020 2073 656c 662e 7369 7a65 736f 6628     self.sizesof(
+00025210: 6469 6d73 292c 2074 7570 6c65 2873 656c  dims), tuple(sel
+00025220: 662e 7363 616c 655b 6178 6973 5d20 666f  f.scale[axis] fo
+00025230: 7220 6178 6973 2069 6e20 6469 6d73 292c  r axis in dims),
+00025240: 2070 7366 0d0a 2020 2020 2020 2020 290d   psf..        ).
+00025250: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00025260: 6e20 7365 6c66 2e5f 6170 706c 795f 6461  n self._apply_da
+00025270: 736b 280d 0a20 2020 2020 2020 2020 2020  sk(..           
+00025280: 205f 6465 636f 6e76 2e72 6963 6861 7264   _deconv.richard
+00025290: 736f 6e5f 6c75 6379 5f74 762c 200d 0a20  son_lucy_tv, .. 
+000252a0: 2020 2020 2020 2020 2020 2063 5f61 7865             c_axe
+000252b0: 733d 636f 6d70 6c65 6d65 6e74 5f61 7865  s=complement_axe
+000252c0: 7328 6469 6d73 2c20 7365 6c66 2e61 7865  s(dims, self.axe
+000252d0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+000252e0: 2061 7267 733d 2870 7366 5f66 742c 2070   args=(psf_ft, p
+000252f0: 7366 5f66 745f 636f 6e6a 2c20 6d61 785f  sf_ft_conj, max_
+00025300: 6974 6572 2c20 6c6d 642c 2074 6f6c 2c20  iter, lmd, tol, 
+00025310: 6570 7329 0d0a 2020 2020 2020 2020 290d  eps)..        ).
+00025320: 0a0d 0a20 2020 2040 5f64 6f63 732e 7772  ...    @_docs.wr
+00025330: 6974 655f 646f 6373 0d0a 2020 2020 4064  ite_docs..    @d
+00025340: 696d 735f 746f 5f73 7061 7469 616c 5f61  ims_to_spatial_a
+00025350: 7865 730d 0a20 2020 2040 7361 6d65 5f64  xes..    @same_d
+00025360: 7479 7065 2861 7366 6c6f 6174 3d54 7275  type(asfloat=Tru
+00025370: 6529 0d0a 2020 2020 4063 6865 636b 5f69  e)..    @check_i
+00025380: 6e70 7574 5f61 6e64 5f6f 7574 7075 740d  nput_and_output.
+00025390: 0a20 2020 2064 6566 2074 696c 6564 5f6c  .    def tiled_l
+000253a0: 7563 7928 0d0a 2020 2020 2020 2020 7365  ucy(..        se
+000253b0: 6c66 2c0d 0a20 2020 2020 2020 2070 7366  lf,..        psf
+000253c0: 3a20 6e70 2e6e 6461 7272 6179 207c 2043  : np.ndarray | C
+000253d0: 616c 6c61 626c 655b 5b74 7570 6c65 5b69  allable[[tuple[i
+000253e0: 6e74 2c20 2e2e 2e5d 5d2c 206e 702e 6e64  nt, ...]], np.nd
+000253f0: 6172 7261 795d 2c0d 0a20 2020 2020 2020  array],..       
+00025400: 206e 6974 6572 3a20 696e 7420 3d20 3530   niter: int = 50
+00025410: 2c0d 0a20 2020 2020 2020 2065 7073 3a20  ,..        eps: 
+00025420: 666c 6f61 7420 3d20 3165 2d35 2c0d 0a20  float = 1e-5,.. 
+00025430: 2020 2020 2020 2063 6875 6e6b 7320 3d20         chunks = 
+00025440: 2261 7574 6f22 2c0d 0a20 2020 2020 2020  "auto",..       
+00025450: 206f 7665 726c 6170 3a20 696e 7420 3d20   overlap: int = 
+00025460: 3332 2c0d 0a20 2020 2020 2020 202a 2a6b  32,..        **k
+00025470: 7761 7267 732c 0d0a 2020 2020 2920 2d3e  wargs,..    ) ->
+00025480: 2049 6d67 4172 7261 793a 0d0a 2020 2020   ImgArray:..    
+00025490: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+000254a0: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
+000254b0: 2260 7469 6c65 645f 6c75 6379 6020 6973  "`tiled_lucy` is
+000254c0: 2064 6570 7265 6361 7465 6420 506c 6561   deprecated Plea
+000254d0: 7365 2075 7365 2022 0d0a 2020 2020 2020  se use "..      
+000254e0: 2020 2020 2020 6622 6069 6d67 2e74 696c        f"`img.til
+000254f0: 6564 287b 6368 756e 6b73 3d7d 2c20 7b6f  ed({chunks=}, {o
+00025500: 7665 726c 6170 3d7d 292e 6c75 6379 282e  verlap=}).lucy(.
+00025510: 2e2e 2960 2069 6e73 7465 6164 2e22 2c0d  ..)` instead.",.
+00025520: 0a20 2020 2020 2020 2020 2020 2044 6570  .            Dep
+00025530: 7265 6361 7469 6f6e 5761 726e 696e 672c  recationWarning,
+00025540: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+00025550: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00025560: 2e74 696c 6564 2863 6875 6e6b 732c 206f  .tiled(chunks, o
+00025570: 7665 726c 6170 292e 6c75 6379 2870 7366  verlap).lucy(psf
+00025580: 2c20 6e69 7465 722c 2065 7073 290d 0a0d  , niter, eps)...
+00025590: 0a64 6566 205f 6368 6563 6b5f 636f 6f72  .def _check_coor
+000255a0: 6469 6e61 7465 7328 636f 6f72 6473 2c20  dinates(coords, 
+000255b0: 696d 673a 2049 6d67 4172 7261 792c 2064  img: ImgArray, d
+000255c0: 696d 733a 2044 696d 7320 3d20 4e6f 6e65  ims: Dims = None
+000255d0: 293a 0d0a 2020 2020 6672 6f6d 2069 6d70  ):..    from imp
+000255e0: 792e 6672 616d 6520 696d 706f 7274 204d  y.frame import M
+000255f0: 6172 6b65 7246 7261 6d65 0d0a 0d0a 2020  arkerFrame....  
+00025600: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00025610: 6e63 6528 636f 6f72 6473 2c20 4d61 726b  nce(coords, Mark
+00025620: 6572 4672 616d 6529 3a0d 0a20 2020 2020  erFrame):..     
+00025630: 2020 2063 6f6f 7264 7320 3d20 6e70 2e61     coords = np.a
+00025640: 7361 7272 6179 2863 6f6f 7264 7329 0d0a  sarray(coords)..
+00025650: 2020 2020 2020 2020 6966 2063 6f6f 7264          if coord
+00025660: 732e 6e64 696d 203d 3d20 313a 0d0a 2020  s.ndim == 1:..  
+00025670: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
+00025680: 203d 2063 6f6f 7264 732e 7265 7368 6170   = coords.reshap
+00025690: 6528 312c 202d 3129 0d0a 2020 2020 2020  e(1, -1)..      
+000256a0: 2020 656c 6966 2063 6f6f 7264 732e 6e64    elif coords.nd
+000256b0: 696d 2021 3d20 323a 0d0a 2020 2020 2020  im != 2:..      
+000256c0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000256d0: 6545 7272 6f72 2822 496e 7075 7420 6361  eError("Input ca
+000256e0: 6e6e 6f74 2062 6520 696e 7465 7270 7265  nnot be interpre
+000256f0: 7465 6420 6173 2063 6f6f 7264 696e 6174  ted as coordinat
+00025700: 6528 7329 2e22 290d 0a20 2020 2020 2020  e(s).")..       
+00025710: 2069 6620 6469 6d73 2069 7320 4e6f 6e65   if dims is None
+00025720: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+00025730: 6469 6d20 3d20 636f 6f72 6473 2e73 6861  dim = coords.sha
+00025740: 7065 5b31 5d0d 0a20 2020 2020 2020 2020  pe[1]..         
+00025750: 2020 2069 6620 6e64 696d 203d 3d20 696d     if ndim == im
+00025760: 672e 6e64 696d 3a0d 0a20 2020 2020 2020  g.ndim:..       
+00025770: 2020 2020 2020 2020 2064 696d 7320 3d20           dims = 
+00025780: 696d 672e 6178 6573 0d0a 2020 2020 2020  img.axes..      
+00025790: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000257a0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+000257b0: 7320 3d20 636f 6d70 6c65 6d65 6e74 5f61  s = complement_a
+000257c0: 7865 7328 2263 222c 2069 6d67 2e61 7865  xes("c", img.axe
+000257d0: 7329 5b2d 6e64 696d 3a5d 0d0a 2020 2020  s)[-ndim:]..    
+000257e0: 2020 2020 636f 6f72 6473 203d 204d 6172      coords = Mar
+000257f0: 6b65 7246 7261 6d65 2863 6f6f 7264 732c  kerFrame(coords,
+00025800: 2063 6f6c 756d 6e73 3d64 696d 732c 2064   columns=dims, d
+00025810: 7479 7065 3d6e 702e 7569 6e74 3136 290d  type=np.uint16).
+00025820: 0a20 2020 2020 2020 2063 6f6f 7264 732e  .        coords.
+00025830: 7365 745f 7363 616c 6528 696d 6729 0d0a  set_scale(img)..
+00025840: 2020 2020 0d0a 2020 2020 7265 7475 726e      ..    return
+00025850: 2063 6f6f 7264 730d 0a0d 0a64 6566 205f   coords....def _
+00025860: 6368 6563 6b5f 6675 6e63 7469 6f6e 2866  check_function(f
+00025870: 756e 6329 3a0d 0a20 2020 2069 6620 6973  unc):..    if is
+00025880: 696e 7374 616e 6365 2866 756e 632c 2073  instance(func, s
+00025890: 7472 293a 0d0a 2020 2020 2020 2020 6675  tr):..        fu
+000258a0: 6e63 203d 2067 6574 6174 7472 286e 702c  nc = getattr(np,
+000258b0: 2066 756e 632c 204e 6f6e 6529 0d0a 2020   func, None)..  
+000258c0: 2020 6966 2063 616c 6c61 626c 6528 6675    if callable(fu
+000258d0: 6e63 293a 0d0a 2020 2020 2020 2020 7265  nc):..        re
+000258e0: 7475 726e 2066 756e 630d 0a20 2020 2065  turn func..    e
+000258f0: 6c73 653a 0d0a 2020 2020 2020 2020 7261  lse:..        ra
+00025900: 6973 6520 5479 7065 4572 726f 7228 224d  ise TypeError("M
+00025910: 7573 7420 6265 206f 6e65 206f 6620 6e75  ust be one of nu
+00025920: 6d70 7920 6d65 7468 6f64 7320 6f72 2063  mpy methods or c
+00025930: 616c 6c61 626c 6520 6f62 6a65 6374 2e22  allable object."
+00025940: 290d 0a20 2020 200d 0a64 6566 205f 6368  )..    ..def _ch
+00025950: 6563 6b5f 6267 2869 6d67 3a20 496d 6741  eck_bg(img: ImgA
+00025960: 7272 6179 2c20 6267 293a 0d0a 2020 2020  rray, bg):..    
+00025970: 2320 6465 7465 726d 696e 6520 6267 0d0a  # determine bg..
+00025980: 2020 2020 6966 2062 6720 6973 204e 6f6e      if bg is Non
+00025990: 653a 0d0a 2020 2020 2020 2020 6267 203d  e:..        bg =
+000259a0: 2069 6d67 2e6d 696e 2829 0d0a 2020 2020   img.min()..    
+000259b0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+000259c0: 6267 2c20 7374 7229 2061 6e64 2062 672e  bg, str) and bg.
+000259d0: 656e 6473 7769 7468 2822 2522 293a 0d0a  endswith("%"):..
+000259e0: 2020 2020 2020 2020 6267 203d 206e 702e          bg = np.
+000259f0: 7065 7263 656e 7469 6c65 2869 6d67 2e76  percentile(img.v
+00025a00: 616c 7565 2c20 666c 6f61 7428 6267 5b3a  alue, float(bg[:
+00025a10: 2d31 5d29 290d 0a20 2020 2065 6c69 6620  -1]))..    elif 
+00025a20: 6e6f 7420 6e70 2e69 7373 6361 6c61 7228  not np.isscalar(
+00025a30: 6267 293a 0d0a 2020 2020 2020 2020 7261  bg):..        ra
+00025a40: 6973 6520 5479 7065 4572 726f 7228 2257  ise TypeError("W
+00025a50: 726f 6e67 2074 7970 6520 6f66 2060 6267  rong type of `bg
+00025a60: 602e 2229 0d0a 2020 2020 7265 7475 726e  `.")..    return
+00025a70: 2062 670d 0a0d 0a64 6566 205f 6368 6563   bg....def _chec
+00025a80: 6b5f 7465 6d70 6c61 7465 2874 656d 706c  k_template(templ
+00025a90: 6174 6529 3a0d 0a20 2020 2069 6620 6e6f  ate):..    if no
+00025aa0: 7420 6973 696e 7374 616e 6365 2874 656d  t isinstance(tem
+00025ab0: 706c 6174 652c 206e 702e 6e64 6172 7261  plate, np.ndarra
+00025ac0: 7929 3a0d 0a20 2020 2020 2020 2072 6169  y):..        rai
+00025ad0: 7365 2054 7970 6545 7272 6f72 2866 2260  se TypeError(f"`
+00025ae0: 7465 6d70 6c61 7465 6020 6d75 7374 2062  template` must b
+00025af0: 6520 6e70 2e6e 6461 7272 6179 2c20 6275  e np.ndarray, bu
+00025b00: 7420 676f 7420 7b74 7970 6528 7465 6d70  t got {type(temp
+00025b10: 6c61 7465 297d 2229 0d0a 2020 2020 656c  late)}")..    el
+00025b20: 6966 2074 656d 706c 6174 652e 6e64 696d  if template.ndim
+00025b30: 206e 6f74 2069 6e20 2832 2c20 3329 3a0d   not in (2, 3):.
+00025b40: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00025b50: 616c 7565 4572 726f 7228 2260 7465 6d70  alueError("`temp
+00025b60: 6c61 7465 206d 7573 7420 6265 2032 206f  late must be 2 o
+00025b70: 7220 3320 6469 6d65 6e73 696f 6e61 6c2e  r 3 dimensional.
+00025b80: 6022 290d 0a20 2020 2074 656d 706c 6174  `")..    templat
+00025b90: 6520 3d20 6e70 2e61 7361 7272 6179 2874  e = np.asarray(t
+00025ba0: 656d 706c 6174 6529 2e61 7374 7970 6528  emplate).astype(
+00025bb0: 6e70 2e66 6c6f 6174 3332 2c20 636f 7079  np.float32, copy
+00025bc0: 3d54 7275 6529 0d0a 2020 2020 7265 7475  =True)..    retu
+00025bd0: 726e 2074 656d 706c 6174 650d 0a0d 0a64  rn template....d
+00025be0: 6566 205f 6361 6c63 5f63 656e 7472 6f69  ef _calc_centroi
+00025bf0: 6428 696d 673a 206e 702e 6e64 6172 7261  d(img: np.ndarra
+00025c00: 792c 206e 6469 6d3a 2069 6e74 2920 2d3e  y, ndim: int) ->
+00025c10: 206e 702e 6e64 6172 7261 793a 0d0a 2020   np.ndarray:..  
+00025c20: 2020 6d6f 6d20 3d20 736b 6d65 732e 6d6f    mom = skmes.mo
+00025c30: 6d65 6e74 7328 696d 672c 206f 7264 6572  ments(img, order
+00025c40: 3d31 290d 0a20 2020 2063 656e 7472 6f69  =1)..    centroi
+00025c50: 6420 3d20 6e70 2e61 7272 6179 285b 6d6f  d = np.array([mo
+00025c60: 6d5b 2830 2c29 2a69 202b 2028 312c 2920  m[(0,)*i + (1,) 
+00025c70: 2b20 2830 2c29 2a28 6e64 696d 2d69 2d31  + (0,)*(ndim-i-1
+00025c80: 295d 200d 0a20 2020 2020 2020 2020 2020  )] ..           
+00025c90: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00025ca0: 2069 2069 6e20 7261 6e67 6528 6e64 696d   i in range(ndim
+00025cb0: 295d 2920 2f20 6d6f 6d5b 2830 2c29 2a6e  )]) / mom[(0,)*n
+00025cc0: 6469 6d5d 0d0a 2020 2020 7265 7475 726e  dim]..    return
+00025cd0: 2063 656e 7472 6f69 640d 0a0d 0a64 6566   centroid....def
+00025ce0: 205f 6368 6563 6b5f 636c 6970 5f72 616e   _check_clip_ran
+00025cf0: 6765 2869 6e5f 7261 6e67 652c 2069 6d67  ge(in_range, img
+00025d00: 2920 2d3e 2074 7570 6c65 5b66 6c6f 6174  ) -> tuple[float
+00025d10: 2c20 666c 6f61 745d 3a0d 0a20 2020 2022  , float]:..    "
+00025d20: 2222 0d0a 2020 2020 4361 6c6c 6564 2069  ""..    Called i
+00025d30: 6e20 636c 6970 5f6f 7574 6c69 6572 7328  n clip_outliers(
+00025d40: 2920 616e 6420 7265 7363 616c 655f 696e  ) and rescale_in
+00025d50: 7465 6e73 6974 7928 292e 0d0a 2020 2020  tensity()...    
+00025d60: 2222 2220 2020 200d 0a20 2020 206c 6f77  """    ..    low
+00025d70: 6572 2c20 7570 7065 7220 3d20 696e 5f72  er, upper = in_r
+00025d80: 616e 6765 0d0a 2020 2020 6966 2069 7369  ange..    if isi
+00025d90: 6e73 7461 6e63 6528 6c6f 7765 722c 2073  nstance(lower, s
+00025da0: 7472 2920 616e 6420 6c6f 7765 722e 656e  tr) and lower.en
+00025db0: 6473 7769 7468 2822 2522 293a 0d0a 2020  dswith("%"):..  
+00025dc0: 2020 2020 2020 6c6f 7765 7220 3d20 666c        lower = fl
+00025dd0: 6f61 7428 6c6f 7765 725b 3a2d 315d 290d  oat(lower[:-1]).
+00025de0: 0a20 2020 2020 2020 206c 6f77 6572 6c69  .        lowerli
+00025df0: 6d20 3d20 6e70 2e70 6572 6365 6e74 696c  m = np.percentil
+00025e00: 6528 696d 672c 206c 6f77 6572 290d 0a20  e(img, lower).. 
+00025e10: 2020 2065 6c69 6620 6c6f 7765 7220 6973     elif lower is
+00025e20: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00025e30: 6c6f 7765 726c 696d 203d 206e 702e 6d69  lowerlim = np.mi
+00025e40: 6e28 696d 6729 0d0a 2020 2020 656c 7365  n(img)..    else
+00025e50: 3a0d 0a20 2020 2020 2020 206c 6f77 6572  :..        lower
+00025e60: 6c69 6d20 3d20 666c 6f61 7428 6c6f 7765  lim = float(lowe
+00025e70: 7229 0d0a 2020 2020 0d0a 2020 2020 6966  r)..    ..    if
+00025e80: 2069 7369 6e73 7461 6e63 6528 7570 7065   isinstance(uppe
+00025e90: 722c 2073 7472 2920 616e 6420 7570 7065  r, str) and uppe
+00025ea0: 722e 656e 6473 7769 7468 2822 2522 293a  r.endswith("%"):
+00025eb0: 0d0a 2020 2020 2020 2020 7570 7065 7220  ..        upper 
+00025ec0: 3d20 666c 6f61 7428 7570 7065 725b 3a2d  = float(upper[:-
+00025ed0: 315d 290d 0a20 2020 2020 2020 2075 7070  1])..        upp
+00025ee0: 6572 6c69 6d20 3d20 6e70 2e70 6572 6365  erlim = np.perce
+00025ef0: 6e74 696c 6528 696d 672c 2075 7070 6572  ntile(img, upper
+00025f00: 290d 0a20 2020 2065 6c69 6620 7570 7065  )..    elif uppe
+00025f10: 7220 6973 204e 6f6e 653a 0d0a 2020 2020  r is None:..    
+00025f20: 2020 2020 7570 7065 726c 696d 203d 206e      upperlim = n
+00025f30: 702e 6d61 7828 696d 6729 0d0a 2020 2020  p.max(img)..    
+00025f40: 656c 7365 3a0d 0a20 2020 2020 2020 2075  else:..        u
+00025f50: 7070 6572 6c69 6d20 3d20 666c 6f61 7428  pperlim = float(
+00025f60: 7570 7065 7229 0d0a 2020 2020 0d0a 2020  upper)..    ..  
+00025f70: 2020 6966 206c 6f77 6572 6c69 6d20 3e3d    if lowerlim >=
+00025f80: 2075 7070 6572 6c69 6d3a 0d0a 2020 2020   upperlim:..    
+00025f90: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00025fa0: 7272 6f72 2866 226c 6f77 6572 6c69 6d20  rror(f"lowerlim 
+00025fb0: 6973 206c 6172 6765 7220 7468 616e 2075  is larger than u
+00025fc0: 7070 6572 6c69 6d3a 207b 6c6f 7765 726c  pperlim: {lowerl
+00025fd0: 696d 7d20 3e3d 207b 7570 7065 726c 696d  im} >= {upperlim
+00025fe0: 7d22 290d 0a20 2020 200d 0a20 2020 2072  }")..    ..    r
+00025ff0: 6574 7572 6e20 6c6f 7765 726c 696d 2c20  eturn lowerlim, 
+00026000: 7570 7065 726c 696d 0d0a 0d0a 6465 6620  upperlim....def 
+00026010: 5f73 7065 6369 6679 5f6f 6e65 2863 656e  _specify_one(cen
+00026020: 7465 722c 2072 6164 6975 732c 2073 6861  ter, radius, sha
+00026030: 7065 3a74 7570 6c65 2920 2d3e 2074 7570  pe:tuple) -> tup
+00026040: 6c65 5b73 6c69 6365 5d3a 0d0a 2020 2020  le[slice]:..    
+00026050: 736c 203d 2074 7570 6c65 2873 6c69 6365  sl = tuple(slice
+00026060: 286d 6178 2830 2c20 7863 2d72 292c 206d  (max(0, xc-r), m
+00026070: 696e 2878 632b 722b 312c 2073 6829 2c20  in(xc+r+1, sh), 
+00026080: 4e6f 6e65 2920 0d0a 2020 2020 2020 2020  None) ..        
+00026090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000260a0: 666f 7220 7863 2c20 722c 2073 6820 696e  for xc, r, sh in
+000260b0: 207a 6970 2863 656e 7465 722c 2072 6164   zip(center, rad
+000260c0: 6975 732c 2073 6861 7065 2929 0d0a 2020  ius, shape))..  
+000260d0: 2020 7265 7475 726e 2073 6c0d 0a0d 0a64    return sl....d
+000260e0: 6566 2063 6865 636b 5f66 696c 7465 725f  ef check_filter_
+000260f0: 6675 6e63 2866 293a 0d0a 2020 2020 6966  func(f):..    if
+00026100: 2066 2069 7320 4e6f 6e65 3a0d 0a20 2020   f is None:..   
+00026110: 2020 2020 2066 203d 206c 616d 6264 6120       f = lambda 
+00026120: 783a 2054 7275 650d 0a20 2020 2065 6c69  x: True..    eli
+00026130: 6620 6e6f 7420 6361 6c6c 6162 6c65 2866  f not callable(f
+00026140: 293a 0d0a 2020 2020 2020 2020 7261 6973  ):..        rais
+00026150: 6520 5479 7065 4572 726f 7228 2260 6669  e TypeError("`fi
+00026160: 6c74 6020 6d75 7374 2062 6520 6361 6c6c  lt` must be call
+00026170: 6162 6c65 2e22 290d 0a20 2020 2072 6574  able.")..    ret
+00026180: 7572 6e20 660d 0a0d 0a0d 0a64 6566 2077  urn f......def w
+00026190: 6176 655f 6e75 6d28 736c 3a20 736c 6963  ave_num(sl: slic
+000261a0: 652c 2073 3a20 696e 742c 2075 663a 2069  e, s: int, uf: i
+000261b0: 6e74 2920 2d3e 2078 702e 6e64 6172 7261  nt) -> xp.ndarra
+000261c0: 793a 0d0a 2020 2020 2222 220d 0a20 2020  y:..    """..   
+000261d0: 2041 2066 756e 6374 696f 6e20 7468 6174   A function that
+000261e0: 206d 616b 6573 2077 6176 6520 6e75 6d62   makes wave numb
+000261f0: 6572 2076 6572 7469 6361 6c20 7665 6374  er vertical vect
+00026200: 6f72 2e20 5265 7475 726e 6564 2076 6563  or. Returned vec
+00026210: 746f 7220 7769 6c6c 0d0a 2020 2020 6265  tor will..    be
+00026220: 205b 6b2f 732c 2028 6b20 2b20 312f 7566   [k/s, (k + 1/uf
+00026230: 292f 732c 2028 6b20 2b20 322f 7566 292f  )/s, (k + 2/uf)/
+00026240: 732c 202e 2e2e 5d20 2877 6865 7265 206b  s, ...] (where k
+00026250: 203d 2073 6c2e 7374 6172 7429 0d0a 0d0a   = sl.start)....
+00026260: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00026270: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00026280: 2020 2020 736c 203a 2073 6c69 6365 0d0a      sl : slice..
+00026290: 2020 2020 2020 2020 536c 6963 6520 7468          Slice th
+000262a0: 6174 2073 7065 6369 6679 2077 6869 6368  at specify which
+000262b0: 2070 6172 7420 6f66 2074 6865 2069 6d61   part of the ima
+000262c0: 6765 2077 696c 6c20 6265 2074 7261 6e73  ge will be trans
+000262d0: 666f 726d 6564 2e0d 0a20 2020 2073 203a  formed...    s :
+000262e0: 2069 6e74 0d0a 2020 2020 2020 2020 5369   int..        Si
+000262f0: 7a65 2061 6c6f 6e67 2063 6572 7461 696e  ze along certain
+00026300: 2064 696d 656e 7369 6f6e 2e0d 0a20 2020   dimension...   
+00026310: 2075 6620 3a20 696e 740d 0a20 2020 2020   uf : int..     
+00026320: 2020 2055 702d 7361 6d70 6c69 6e67 2066     Up-sampling f
+00026330: 6163 746f 7220 6f66 2063 6572 7461 696e  actor of certain
+00026340: 2064 696d 656e 7369 6f6e 2e0d 0a20 2020   dimension...   
+00026350: 2022 2222 0d0a 2020 2020 7374 6172 7420   """..    start 
+00026360: 3d20 3020 6966 2073 6c2e 7374 6172 7420  = 0 if sl.start 
+00026370: 6973 204e 6f6e 6520 656c 7365 2073 6c2e  is None else sl.
+00026380: 7374 6172 740d 0a20 2020 2073 746f 7020  start..    stop 
+00026390: 3d20 7320 6966 2073 6c2e 7374 6f70 2069  = s if sl.stop i
+000263a0: 7320 4e6f 6e65 2065 6c73 6520 736c 2e73  s None else sl.s
+000263b0: 746f 700d 0a20 2020 200d 0a20 2020 2069  top..    ..    i
+000263c0: 6620 736c 2e73 7461 7274 2061 6e64 2073  f sl.start and s
+000263d0: 6c2e 7374 6f70 2061 6e64 2073 7461 7274  l.stop and start
+000263e0: 203c 2030 2061 6e64 2073 746f 7020 3e20   < 0 and stop > 
+000263f0: 303a 0d0a 2020 2020 2020 2020 2320 6c69  0:..        # li
+00026400: 6b65 2022 783d 2d35 3a35 220d 0a20 2020  ke "x=-5:5"..   
+00026410: 2020 2020 2070 6173 730d 0a20 2020 2065       pass..    e
+00026420: 6c73 653a 0d0a 2020 2020 2020 2020 6966  lse:..        if
+00026430: 202d 7320 3c20 7374 6172 7420 3c20 303a   -s < start < 0:
+00026440: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00026450: 6172 7420 2b3d 2073 0d0a 2020 2020 2020  art += s..      
+00026460: 2020 656c 6966 206e 6f74 2030 203c 3d20    elif not 0 <= 
+00026470: 7374 6172 7420 3c20 733a 0d0a 2020 2020  start < s:..    
+00026480: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00026490: 6c75 6545 7272 6f72 2866 2249 6e76 616c  lueError(f"Inval
+000264a0: 6964 2076 616c 7565 2065 6e63 6f75 6e74  id value encount
+000264b0: 6572 6564 2069 6e20 736c 6963 6520 7b73  ered in slice {s
+000264c0: 6c7d 2e22 290d 0a20 2020 2020 2020 2069  l}.")..        i
+000264d0: 6620 2d73 203c 2073 746f 7020 3c3d 2030  f -s < stop <= 0
+000264e0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000264f0: 746f 7020 2b3d 2073 0d0a 2020 2020 2020  top += s..      
+00026500: 2020 656c 6966 206e 6f74 2030 203c 2073    elif not 0 < s
+00026510: 746f 7020 3c3d 2073 3a0d 0a20 2020 2020  top <= s:..     
+00026520: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00026530: 7565 4572 726f 7228 6622 496e 7661 6c69  ueError(f"Invali
+00026540: 6420 7661 6c75 6520 656e 636f 756e 7465  d value encounte
+00026550: 7265 6420 696e 2073 6c69 6365 207b 736c  red in slice {sl
+00026560: 7d2e 2229 0d0a 2020 2020 2020 2020 0d0a  }.")..        ..
+00026570: 2020 2020 6e20 3d20 7374 6f70 202d 2073      n = stop - s
+00026580: 7461 7274 0d0a 2020 2020 7265 7475 726e  tart..    return
+00026590: 2078 702e 6c69 6e73 7061 6365 2873 7461   xp.linspace(sta
+000265a0: 7274 2c20 7374 6f70 2c20 6e2a 7566 2c20  rt, stop, n*uf, 
+000265b0: 656e 6470 6f69 6e74 3d46 616c 7365 295b  endpoint=False)[
+000265c0: 3a2c 206e 702e 6e65 7761 7869 735d 0d0a  :, np.newaxis]..
```

### Comparing `impy_array-2.2.5/impy/arrays/label.py` & `impy_array-2.2.6/impy/arrays/label.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/labeledarray.py` & `impy_array-2.2.6/impy/arrays/labeledarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/lazy.py` & `impy_array-2.2.6/impy/arrays/lazy.py`

 * *Files identical despite different names*

```diff
@@ -24,15 +24,15 @@
 from impy.axes import ImageAxesError, AxisLike
 from impy.array_api import xp
 from impy._types import nDFloat, Coords, Iterable, Dims, PaddingMode
 from impy._const import Const
 
 if TYPE_CHECKING:
     from dask.array.core import Array as DaskArray
-
+    from impy.axes import AxesTuple
 
 class LazyImgArray(AxesMixin):
     additional_props = ["_source", "_metadata", "_name"]
     
     def __init__(
         self,
         obj: "DaskArray",
@@ -85,15 +85,15 @@
 
     @property
     def ndim(self) -> int:
         """Number of dimensions of the array."""
         return self.value.ndim
     
     @property
-    def shape(self):
+    def shape(self) -> AxesTuple[int]:
         """Shape of the array."""
         return self.axes.tuple(self.value.shape)
         
     @property
     def dtype(self):
         """Data type of the array"""
         return self.value.dtype
@@ -105,15 +105,15 @@
     
     @property
     def itemsize(self):
         """Size of each element in bytes."""
         return self.value.itemsize
     
     @property
-    def chunksize(self):
+    def chunksize(self) -> AxesTuple[int]:
         """Chunk size of the array."""
         return self.axes.tuple(self.value.chunksize)
         
     @property
     def GB(self) -> float:
         """Return the array size in GB."""
         return self.value.nbytes / 1e9
```

### Comparing `impy_array-2.2.5/impy/arrays/phasearray.py` & `impy_array-2.2.6/impy/arrays/phasearray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/specials.py` & `impy_array-2.2.6/impy/arrays/specials.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/tiled.py` & `impy_array-2.2.6/impy/arrays/tiled.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, Any, Callable
 import weakref
 
 import numpy as np
 from impy.utils.axesop import switch_slice
 from impy.utils.misc import check_nd
 from impy.array_api import xp
-from impy._types import nDFloat, Dims
+from impy._types import Dims
 from ._utils import _deconv, _filters
 from ._utils._skimage import _get_ND_butterworth_filter
 
 from dask import array as da
 
 if TYPE_CHECKING:
     from .imgarray import ImgArray
@@ -127,15 +127,15 @@
     ) -> ImgArray:
         if high_sigma is None:
             high_sigma = low_sigma * 1.6
         filter_func = _filters.dog_filter_fourier if fourier else _filters.dog_filter
         return self._map_overlap(filter_func, low_sigma=low_sigma, high_sigma=high_sigma)
 
     def log_filter(self, sigma: float) -> ImgArray:
-        return self._map_overlap(_filters.gaussian_laplace, sigma=sigma)
+        return -self._map_overlap(_filters.gaussian_laplace, sigma=sigma)
 
 def _lowpass(arr, cutoff, order=2):
     arr = xp.asarray(arr)
     shape = arr.shape
     _cutoff = check_nd(cutoff, len(shape))
     weight = _get_ND_butterworth_filter(shape, _cutoff, order, False, True)
     ft = xp.asarray(weight) * xp.fft.rfftn(arr)
```

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_corr.py` & `impy_array-2.2.6/impy/arrays/_utils/_corr.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_deconv.py` & `impy_array-2.2.6/impy/arrays/_utils/_deconv.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_docs.py` & `impy_array-2.2.6/impy/arrays/_utils/_docs.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_filters.py` & `impy_array-2.2.6/impy/arrays/_utils/_filters.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_glcm.py` & `impy_array-2.2.6/impy/arrays/_utils/_glcm.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_linalg.py` & `impy_array-2.2.6/impy/arrays/_utils/_linalg.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_misc.py` & `impy_array-2.2.6/impy/arrays/_utils/_misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_plot.py` & `impy_array-2.2.6/impy/arrays/_utils/_plot.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_process_numba.py` & `impy_array-2.2.6/impy/arrays/_utils/_process_numba.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_skimage.py` & `impy_array-2.2.6/impy/arrays/_utils/_skimage.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_structures.py` & `impy_array-2.2.6/impy/arrays/_utils/_structures.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/_utils/_transform.py` & `impy_array-2.2.6/impy/arrays/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/arrays/bases/metaarray.py` & `impy_array-2.2.6/impy/arrays/bases/metaarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,63 +527,63 @@
         out._set_info(self, new_axes=new_axes)
         return out
     
     def min(
         self,
         axis=None,
         out: None = None,
-        keepdims: bool = _NoValue,
+        keepdims: bool = False,
         *,
         where: np.ndarray = _NoValue,
     ):
         """Minimum value of the array along a given axis."""
         return np.min(self, axis=axis, out=out, keepdims=keepdims, where=where)
     
     def max(
         self,
         axis=None,
         out: None = None,
-        keepdims: bool = _NoValue,
+        keepdims: bool = False,
         *,
         where: np.ndarray = _NoValue,
     ):
         """Maximum value of the array along a given axis."""
         return np.max(self, axis=axis, out=out, keepdims=keepdims, where=where)
     
     def mean(
         self,
         axis=None,
         dtype: DTypeLike = None,
         out: None = None,
-        keepdims: bool = _NoValue,
+        keepdims: bool = False,
         *,
         where: np.ndarray = _NoValue,
     ):
         """Mean value of the array along a given axis."""
         return np.mean(self, axis=axis, dtype=dtype, out=out, keepdims=keepdims, where=where)
     
     def sum(
         self,
         axis=None,
         dtype: DTypeLike = None,
         out: None = None,
-        keepdims: bool = _NoValue,
+        keepdims: bool = False,
         *,
         where: np.ndarray = _NoValue,
     ):
         """Sum value of the array along a given axis."""
         return np.sum(self, axis=axis, dtype=dtype, out=out, keepdims=keepdims, where=where)
     
     def std(
         self,
         axis=None,
         dtype: DTypeLike = None,
         out: None = None,
         ddof: int = 0,
-        keepdims: bool = _NoValue,
+        keepdims: bool = False,
         *,
         where: np.ndarray = _NoValue,
     ):
         """Standard deviation of the array along a given axis."""
         return np.std(self, axis=axis, dtype=dtype, out=out, ddof=ddof, keepdims=keepdims, where=where)
 
     def _dimension_matches(self, array: MetaArray):
@@ -767,15 +767,15 @@
     
     def _inherit_meta(self, obj: AxesMixin, ufunc, **kwargs):
         """
         Copy axis etc. from obj.
         This is called in __array_ufunc__(). Unlike _set_info(), keyword `axis` must be
         considered because it changes `ndim`.
         """
-        if "axis" in kwargs and "keepdims" not in kwargs:
+        if "axis" in kwargs and not kwargs.get("keepdims", False):
             new_axes = obj.axes.drop(kwargs["axis"])
         else:
             new_axes = self._INHERIT
         self._set_info(obj, new_axes=new_axes)
         return self
 
     if TYPE_CHECKING:
```

### Comparing `impy_array-2.2.5/impy/arrays/bases/overload.py` & `impy_array-2.2.6/impy/arrays/bases/overload.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/axes/_axes.py` & `impy_array-2.2.6/impy/axes/_axes.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/axes/_axes_tuple.py` & `impy_array-2.2.6/impy/axes/_axes_tuple.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/axes/_axis.py` & `impy_array-2.2.6/impy/axes/_axis.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/axes/_slicer.py` & `impy_array-2.2.6/impy/axes/_slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/frame/frames.py` & `impy_array-2.2.6/impy/frame/frames.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/utils/axesop.py` & `impy_array-2.2.6/impy/utils/axesop.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/utils/deco.py` & `impy_array-2.2.6/impy/utils/deco.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/utils/gauss.py` & `impy_array-2.2.6/impy/utils/gauss.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/utils/misc.py` & `impy_array-2.2.6/impy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/utils/slicer.py` & `impy_array-2.2.6/impy/utils/slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/viewer/utils.py` & `impy_array-2.2.6/impy/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/impy/viewer/viewer.py` & `impy_array-2.2.6/impy/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/.gitignore` & `impy_array-2.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/LICENSE` & `impy_array-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/README.md` & `impy_array-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.5/pyproject.toml` & `impy_array-2.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 
 [project]
 name = "impy-array"
 dynamic = ["version"]
 description = "Speed up coding/extending image analysis in Python."
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "Hanjin Liu", email = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp" },
 ]
```

### Comparing `impy_array-2.2.5/PKG-INFO` & `impy_array-2.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impy-array
-Version: 2.2.5
+Version: 2.2.6
 Summary: Speed up coding/extending image analysis in Python.
 Project-URL: Download, https://github.com/hanjinliu/impy
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
@@ -31,21 +31,20 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: dask>=2021.6.0
 Requires-Dist: napari>=0.4.17
 Requires-Dist: numpy>=1.22
 Requires-Dist: pandas>=1.3
 Requires-Dist: scikit-image>=0.20.0
 Provides-Extra: all
 Requires-Dist: mrcfile; extra == 'all'
```

