# Comparing `tmp/webcam-1.2.tar.gz` & `tmp/webcam-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.2.tar", last modified: Tue Jun 20 14:08:41 2023, max compression
+gzip compressed data, was "webcam-1.3.tar", last modified: Fri Jun 23 12:38:46 2023, max compression
```

## Comparing `webcam-1.2.tar` & `webcam-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.755682 webcam-1.2/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.2/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-06-20 14:08:41.754251 webcam-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 14:08:41.756696 webcam-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-06-20 14:08:30.000000 webcam-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.690523 webcam-1.2/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.2/webcam/__init__.py
--rw-rw-rw-   0        0        0     7465 2023-06-20 13:39:41.000000 webcam-1.2/webcam/_perspective_manager.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.2/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.2/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    15396 2023-06-20 14:05:46.000000 webcam-1.2/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.747957 webcam-1.2/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.938822 webcam-1.3/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.3/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-23 12:38:46.937762 webcam-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 12:38:46.938822 webcam-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-23 12:36:27.000000 webcam-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.905465 webcam-1.3/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.3/webcam/__init__.py
+-rw-rw-rw-   0        0        0    10127 2023-06-23 12:36:27.000000 webcam-1.3/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.3/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.3/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    18641 2023-06-23 12:38:38.000000 webcam-1.3/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.933008 webcam-1.3/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.2/LICENSE` & `webcam-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.2/PKG-INFO` & `webcam-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.2
+Version: 1.3
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.2/README.md` & `webcam-1.3/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.2/setup.py` & `webcam-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.2',
+    version='1.3',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.2/webcam/_perspective_manager.py` & `webcam-1.3/webcam/_perspective_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Author: Eric Canas
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 20-06-2023
 """
 from __future__ import annotations
-from functools import lru_cache
+from functools import lru_cache, cache
 import cv2
 import numpy as np
 
 
 class _PerspectiveManager:
     def __init__(self, homography_matrix: np.ndarray|list[list[float], ...], default_w: int, default_h: int,
                  crop_boundaries: bool = False,
@@ -21,14 +21,24 @@
         self.default_w, self.default_h = default_w, default_h
         homography_matrix = np.array(homography_matrix, dtype=np.float32)
         self.homography_matrix = self.__apply_non_negative_translation_to_homography_matrix(m=homography_matrix,
                                                                                              w=default_w, h=default_h)
         self.crop_boundaries = crop_boundaries
         self.boundaries_color = boundaries_color
 
+    @property
+    def output_w(self) -> int:
+        w, h = self.after_warp_image_shape(w=self.default_w, h=self.default_h)
+        return w
+
+    @property
+    def output_h(self) -> int:
+        w, h = self.after_warp_image_shape(w=self.default_w, h=self.default_h)
+        return h
+
     @lru_cache(maxsize=32)
     def __build_corners(self, w: float|int, h: float|int):
         assert w == self.default_w and h == self.default_h, \
             f'By the moment, that is assumed that h and w are kept since the initialization. ' \
             f'Changing them could lead to unexpected results. '
         w, h = float(w), float(h)
         return np.array(((0., 0.), (w - 1., 0.), (w - 1., h - 1.), (0., h - 1.)), dtype=np.float32)
@@ -130,14 +140,49 @@
         translation_matrix = np.array(((1., 0., -x_min), (0., 1., -y_min), (0., 0., 1.)), dtype=np.float32)
 
         # Combine the original matrix with the translation matrix
         combined_matrix = np.dot(a=translation_matrix, b=m)
 
         return combined_matrix
 
+    @lru_cache(maxsize=64)
+    def get_hw_magnification_at_point(self, x:int|float, y:int|float) -> tuple[float, float]:
+        """
+        Get the magnification factor for the given point. It is calculated by setting two vectors extending along
+        x and y axes around the point (x, y), a horizontal and a vertical one, with length 2. The vectors are then
+        transformed by the homography matrix and the magnification factor is calculated as the ratio between the
+        length of the transformed vectors and the original ones.
+        :param x: int or float. The x coordinate of the point.
+        :param y: int or float. The y coordinate of the point.
+        :return: tuple[float, float]. The magnification factor for the given point. In the form (h_magnification, w_magnification).
+        """
+        assert self.homography_matrix is not None, "Homography matrix must be set before calling this method."
+        assert self.homography_matrix.shape == (3, 3), f"Homography matrix must be a 3x3 matrix. Got {'x'.join(self.homography_matrix.shape)}"
+
+        # Define two vectors extending along x and y axes around the point (x, y) with length 2
+        vec_x = np.array(((x-1., y, 1.), (x, y, 1.), (x+1., y, 1.)), dtype=np.float32).T
+        vec_y = np.array(((x, y-1., 1.), (x, y, 1.), (x, y+1., 1.)), dtype=np.float32).T
+
+        # Apply the homography matrix to the two vectors
+        vec_x_transformed = np.dot(self.homography_matrix, vec_x)
+        vec_y_transformed = np.dot(self.homography_matrix, vec_y)
+
+        # Convert the transformed coordinates from homogeneous to Cartesian coordinates
+        vec_x_transformed /= vec_x_transformed[2]
+        vec_y_transformed /= vec_y_transformed[2]
+
+        # Compute the lengths of the transformed vectors
+        length_transformed_x = np.linalg.norm(vec_x_transformed[:, -1] - vec_x_transformed[:, 0])
+        length_transformed_y = np.linalg.norm(vec_y_transformed[:, -1] - vec_y_transformed[:, 0])
+
+        # The magnification in x and y directions is the ratio of transformed length to original length
+        homography_magnification_w = length_transformed_x / (vec_x[0, -1] - vec_x[0, 0])
+        homography_magnification_h = length_transformed_y / (vec_y[1, -1] - vec_y[1, 0])
+
+        return homography_magnification_w, homography_magnification_h
 
 class _DummyPerspectiveManager:
     def __init__(self, *args, **kwargs):
         pass
 
     def after_warp_image_shape(self, w: int, h: int) -> tuple[int, int]:
         return w, h
```

### Comparing `webcam-1.2/webcam/_video_webcam.py` & `webcam-1.3/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.2/webcam/_webcam_background.py` & `webcam-1.3/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.2/webcam/webcam.py` & `webcam-1.3/webcam/webcam.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 04-03-2023
 """
 
 
 from __future__ import annotations
+
+from functools import lru_cache
+
 import cv2
 import numpy as np
 import time
 from typing import Tuple
 
 import os
 
@@ -71,15 +74,15 @@
         else:
             self.perspective_manager = _PerspectiveManager(homography_matrix=homography_matrix,
                                                           default_h=int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
                                                           default_w=int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
                                                           crop_boundaries=crop_on_warping)
 
         # Calculate and set output frame size
-        self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
+        self.frame_size_hw = self._calculate_and_set_desired_resolution(h=h, w=w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
         self.start_timestamp = time.time()
         self.max_frame_rate = max_frame_rate
         self.last_frame_timestamp = self.start_timestamp
 
@@ -107,14 +110,29 @@
         return self.frame_size_hw[0]
 
     @property
     def w(self) -> int:
         return self.frame_size_hw[1]
 
     @property
+    def pixel_magnification(self) -> float:
+        m_h, m_w = self.get_magnification_hw(x=None, y=None)
+        return (m_h + m_w) / 2
+
+    @property
+    def pixel_magnification_h(self) -> float:
+        m_h, m_w = self.get_magnification_hw(x=None, y=None)
+        return m_h
+
+    @property
+    def pixel_magnification_w(self) -> float:
+        m_h, m_w = self.get_magnification_hw(x=None, y=None)
+        return m_w
+
+    @property
     def current_timestamp_seconds(self):
         return time.time() - self.start_timestamp
 
     def read_next_frame(self) -> np.ndarray:
         """
         Read the next frame from the video. (Skipping the frames_offset if it is greater than one.)
         """
@@ -296,26 +314,81 @@
 
     def release(self):
         self.cap.release()
 
     def isOpened(self):
         return self.cap.isOpened()
 
+    @lru_cache(maxsize=8)
+    def _get_pixel_magnification_one_axis(self, length:int, axis: str) -> float:
+        """
+        Calculate the pixel magnification factor for one axis (height or width) of the frame.
+        Pixel magnification factor is the ratio between the length of the axis in the original video and the length
+        of the axis in the output frame.
+
+        :param length: int. The length of the axis (height or width) of the frame.
+        :param axis: str. The axis to calculate the pixel magnification factor for.
+        Valid values are 'h' and 'w'.
+
+        :return: float. The pixel magnification factor for the given axis.
+        """
+        assert axis in ('h', 'w'), f"Invalid value for 'axis' parameter: {axis}. Valid values are 'h' and 'w'."
+
+    @lru_cache(maxsize=64)
+    def get_magnification_hw(self, x: int | float | None = None, y: int | float | None = None) -> float:
+        """
+        Calculate the magnification of the pixel at (x, y). If x and y are not given, the magnification of the
+        center pixel is calculated. (x, y) coordinates are only relevant if the perspective is adjusted.
+
+        :param x: int or float or None. The x coordinate of the pixel.
+        :param y: int or float or None. The y coordinate of the pixel.
+        :return: float. The magnification of the pixel at (x, y).
+        """
+
+        # Calculate the homography magnification if appliable
+        if self.perspective_manager is not None:
+            x = self._w // 2 if x is None else x
+            y = self._h // 2 if y is None else y
+
+            magnification_h, magnification_w = self.perspective_manager.get_hw_magnification_at_point(x=x, y=y)
+            input_h, input_w = self.perspective_manager.output_h, self.perspective_manager.output_w
+        # Or use the default magnification
+        else:
+            magnification_h, magnification_w = 1.0, 1.0
+            input_h, input_w = self._h, self._w
+
+        # Calculate the pixel magnification for each axis when adjusting size
+        if self.on_aspect_ratio_lost == RESIZE:
+            magnification_h *= self.h / input_h
+            magnification_w *= self.w / input_w
+
+        elif self.on_aspect_ratio_lost == CROP:
+            resize_ratio = self.h / input_h if input_h < input_w else self.w / input_w
+            magnification_h *= resize_ratio
+            magnification_w *= resize_ratio
+        else:
+            raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}."
+                             f" Valid values are '{RESIZE}' and '{CROP}'.")
+
+
+        # Return the magnification of the pixel at (x, y)
+        return magnification_h, magnification_w
+
+
     # --------------- AUXILIARY METHODS ---------------
     def calculate_frame_size_keeping_aspect_ratio(self, h:int | None, w:int|None) -> tuple[int, int]:
         """
         When only one of the frame size dimensions is given, the other one is calculated keeping the
         aspect ratio with the original video.
 
         :param h: int or None. Height of the frame. If None, _w must be provided.
         :param w: int or None. Width of the frame. If None, _h must be provided.
         :return: The height and width of the frame.
         """
 
-
         if h is None and w is not None:
             h = int(round(self._h * w / self._w))
         elif h is not None and w is None:
             w = int(round(self._w * h / self._h))
         else:
             raise ValueError(f'Only one of the frame size dimensions must be provided.'
                              f' Got _h={h} and _w={w}.')
```

### Comparing `webcam-1.2/webcam.egg-info/PKG-INFO` & `webcam-1.3/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.2
+Version: 1.3
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

