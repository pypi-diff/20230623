# Comparing `tmp/face-crop-plus-1.0.3.tar.gz` & `tmp/face-crop-plus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face-crop-plus-1.0.3.tar", last modified: Wed Apr 26 19:24:41 2023, max compression
+gzip compressed data, was "face-crop-plus-1.1.0.tar", last modified: Fri Jun 23 08:40:01 2023, max compression
```

## Comparing `face-crop-plus-1.0.3.tar` & `face-crop-plus-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42437 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/cropper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus/models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/bise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/models/rrdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-04-26 19:24:24.000000 face-crop-plus-1.0.3/src/face_crop_plus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:24:41.804395 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:24:41.000000 face-crop-plus-1.0.3/src/face_crop_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:40:01.084445 face-crop-plus-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-06-23 08:40:01.084445 face-crop-plus-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 08:40:01.084445 face-crop-plus-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:40:01.080444 face-crop-plus-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:40:01.080444 face-crop-plus-1.1.0/src/face_crop_plus/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43193 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/cropper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:40:01.084445 face-crop-plus-1.1.0/src/face_crop_plus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/models/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/models/bise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/models/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/models/rrdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-06-23 08:39:45.000000 face-crop-plus-1.1.0/src/face_crop_plus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:40:01.080444 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 08:40:01.000000 face-crop-plus-1.1.0/src/face_crop_plus.egg-info/top_level.txt
```

### Comparing `face-crop-plus-1.0.3/LICENCE` & `face-crop-plus-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.3/PKG-INFO` & `face-crop-plus-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: face-crop-plus
-Version: 1.0.3
+Version: 1.1.0
 Summary: Automatic face aligner and cropper with quality enhancement and attribute parsing.
 Home-page: https://github.com/mantasu/face-crop-plus
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/face-crop-plus
 Project-URL: Bug Tracker, https://github.com/mantasu/face-crop-plus/issues
 Keywords: face,python,pytorch,alignment,cropping,super resolution,quality enhancement,parsing,grouping,attributes,mask,segmentation,celeba
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Face Crop Plus
 
-[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![PyPI](https://img.shields.io/pypi/v/face-crop-plus?color=orange)](https://pypi.org/project/face-crop-plus/)
-[![Python: 3.10](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org/downloads/release/python-3100/)
+[![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
+[![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/face-crop-plus/)
+[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center" width="100%">
 
 ![Banner](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/banner.png)
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
 2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
-3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
+3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and necklace_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
 
@@ -137,40 +139,40 @@
 
 > Quality enhancement can be used as a separate feature to enhance images that contain faces. For an end user, it is a useful feature to boost the quality of photos. It is not suggested to enhance ultra high resolution images (>2000) because your GPU will explode. See _Pure Enhancement/Parsing_ section on how to run it as a stand-alone.
 
 
 ### Attribute Parsing
 
 Face parsing to attributes allows to group output images by category and generate attribute masks for that category. Categorized images are put to their corresponding sub-folders in the output directory.
-* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and neckless_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
+* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and necklace_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :---------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
-    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
+    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
 
 * `mask_groups` - Dictionary specifying mask groups, based on which the face images and their masks should be grouped. Each key represents a mask group name, e.g., _nose_, _eyes and eyebrows_, and each value represents attribute indices, e.g., `[10]`, `[2, 3, 4, 5]`, each index mapping to some attribute. Since this model labels face image pixels, a mask will be created with 255 (white) at pixels that match the specified attributes and zeros (black) elsewhere. Note that negative values would make no sense here and having them would cause an error. Images are saved to sub-directories named by the mask group and masks are saved to sub-directories under the same name, except with `_mask` suffix. If it is None, then there will be no grouping according to mask groups. Here are some group examples with 1 sample image and its mask per group (for consistency, same images as before):
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
 
 > If both `attr_groups` and `mask_groups` are specified, first images are grouped according to face attributes, then images in each groups are further sub-grouped to different mask groups (along with their masks).
 
 
 Here are the 19 possible face attributes (with `0` representing the neutral category):
 
 <p align="center" width="100%">
 
 |                     |                  |                  |
 | ------------------- | ---------------- | ---------------- |
 | `1` - skin          | `7` - left ear   | `13` - lower lip |
 | `2` - left eyebrow  | `8` - right ear  | `14` - neck      |
-| `3` - right eyebrow | `9` - earrings   | `15` - neckless  |
+| `3` - right eyebrow | `9` - earrings   | `15` - necklace  |
 | `4` - left eye      | `10` - nose      | `16` - clothes   |
 | `5` - right eye     | `11` - mouth     | `17` - hair      |
 | `6` - eyeglasses    | `12` - upper lip | `18` - hat       |
 
 </p>
 
 ## Examples
@@ -195,14 +197,33 @@
 For all the available command line arguments, just type (although refer to documentation for more details):
 ```bash
 face-crop-plus -h
 ```
 
 > **Note**: you can use `fcp` as `face-crop-plus` alias , e.g., `fcp -c config.json`
 
+### Cleaning File Names
+
+If your image files contain non-ascii symbols, lengthy names, os-reserved characters, it may be better to standardize them. To do so, it is possible to rename the image files before processing them:
+```bash
+face-crop-plus -i path/to/images --clean-names # --clean-names-inplace (avoids temp dir)
+```
+
+It is possible to specify more arguments via python script. The function can be used in general with any file types:
+
+```python
+from face_crop_plus.utils import clean_names
+
+clean_names(
+    input_dir="path/to/input/dir",
+    output_dir=None, # will rename in-place
+    max_chars=250,
+)
+```
+
 ### Pure Enhancement/Parsing
 
 If you already have aligned and center-cropped face images, you can perform quality enhancement and face parsing without re-cropping them. Here is an example of enhancing quality of every face and parsing them to (note that none of the parameters described in _Alignment and Cropping_ section have any affect here):
 
 ```python
 from face_crop_plus import Cropper
```

### Comparing `face-crop-plus-1.0.3/README.md` & `face-crop-plus-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Face Crop Plus
 
-[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![PyPI](https://img.shields.io/pypi/v/face-crop-plus?color=orange)](https://pypi.org/project/face-crop-plus/)
-[![Python: 3.10](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org/downloads/release/python-3100/)
+[![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
+[![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/face-crop-plus/)
+[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center" width="100%">
 
 ![Banner](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/banner.png)
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
 2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
-3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
+3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and necklace_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
 
@@ -115,40 +116,40 @@
 
 > Quality enhancement can be used as a separate feature to enhance images that contain faces. For an end user, it is a useful feature to boost the quality of photos. It is not suggested to enhance ultra high resolution images (>2000) because your GPU will explode. See _Pure Enhancement/Parsing_ section on how to run it as a stand-alone.
 
 
 ### Attribute Parsing
 
 Face parsing to attributes allows to group output images by category and generate attribute masks for that category. Categorized images are put to their corresponding sub-folders in the output directory.
-* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and neckless_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
+* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and necklace_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :---------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
-    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
+    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
 
 * `mask_groups` - Dictionary specifying mask groups, based on which the face images and their masks should be grouped. Each key represents a mask group name, e.g., _nose_, _eyes and eyebrows_, and each value represents attribute indices, e.g., `[10]`, `[2, 3, 4, 5]`, each index mapping to some attribute. Since this model labels face image pixels, a mask will be created with 255 (white) at pixels that match the specified attributes and zeros (black) elsewhere. Note that negative values would make no sense here and having them would cause an error. Images are saved to sub-directories named by the mask group and masks are saved to sub-directories under the same name, except with `_mask` suffix. If it is None, then there will be no grouping according to mask groups. Here are some group examples with 1 sample image and its mask per group (for consistency, same images as before):
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
 
 > If both `attr_groups` and `mask_groups` are specified, first images are grouped according to face attributes, then images in each groups are further sub-grouped to different mask groups (along with their masks).
 
 
 Here are the 19 possible face attributes (with `0` representing the neutral category):
 
 <p align="center" width="100%">
 
 |                     |                  |                  |
 | ------------------- | ---------------- | ---------------- |
 | `1` - skin          | `7` - left ear   | `13` - lower lip |
 | `2` - left eyebrow  | `8` - right ear  | `14` - neck      |
-| `3` - right eyebrow | `9` - earrings   | `15` - neckless  |
+| `3` - right eyebrow | `9` - earrings   | `15` - necklace  |
 | `4` - left eye      | `10` - nose      | `16` - clothes   |
 | `5` - right eye     | `11` - mouth     | `17` - hair      |
 | `6` - eyeglasses    | `12` - upper lip | `18` - hat       |
 
 </p>
 
 ## Examples
@@ -173,14 +174,33 @@
 For all the available command line arguments, just type (although refer to documentation for more details):
 ```bash
 face-crop-plus -h
 ```
 
 > **Note**: you can use `fcp` as `face-crop-plus` alias , e.g., `fcp -c config.json`
 
+### Cleaning File Names
+
+If your image files contain non-ascii symbols, lengthy names, os-reserved characters, it may be better to standardize them. To do so, it is possible to rename the image files before processing them:
+```bash
+face-crop-plus -i path/to/images --clean-names # --clean-names-inplace (avoids temp dir)
+```
+
+It is possible to specify more arguments via python script. The function can be used in general with any file types:
+
+```python
+from face_crop_plus.utils import clean_names
+
+clean_names(
+    input_dir="path/to/input/dir",
+    output_dir=None, # will rename in-place
+    max_chars=250,
+)
+```
+
 ### Pure Enhancement/Parsing
 
 If you already have aligned and center-cropped face images, you can perform quality enhancement and face parsing without re-cropping them. Here is an example of enhancing quality of every face and parsing them to (note that none of the parameters described in _Alignment and Cropping_ section have any affect here):
 
 ```python
 from face_crop_plus import Cropper
```

### Comparing `face-crop-plus-1.0.3/setup.py` & `face-crop-plus-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name = "face-crop-plus",
-    version = "1.0.3",
+    version = "1.1.0",
     author = "Mantas Birškus",
     author_email = "mantix7@gmail.com",
     license = "MIT",
     description = f"Automatic face aligner and cropper with quality "
                   f"enhancement and attribute parsing.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
@@ -31,23 +31,25 @@
         "attributes",
         "mask",
         "segmentation",
         "celeba",
     ],
     install_requires = [
         "tqdm",
+        "unidecode",
         "opencv-python",
         "torch",
         "torchvision",
     ],
     classifiers = [
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     entry_points={
```

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/__main__.py` & `face-crop-plus-1.1.0/src/face_crop_plus/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import sys
 import json
+import torch
+import shutil
 import argparse
 from typing import Any
 from .cropper import Cropper
+from .utils import clean_names
 
 class ArgumentParserWithConfig(argparse.ArgumentParser):
     """An ArgumentParser that loads default values from a config file.
 
     This class extends the :class:`argparse.ArgumentParser` class to 
     load default values from a config file specified by a command-line 
     argument.
@@ -107,24 +110,41 @@
     Returns:
         A dictionary where keys represent argument names and values 
         represent those argument values.
     """
     # Arg parser that can load default values
     parser = ArgumentParserWithConfig()
 
-    # TODO: check list args, check transparent, check attr_groups
     parser.add_argument(
         "-i", "--input_dir", type=str, 
         help="Path to input directory with image files.")
     parser.add_argument(
         "-o", "--output-dir", type=str, 
         help=f"Path to output directory to save the extracted face images. If "
              f"not specified, the same path is used as for input_dir, except "
              f"'_faces' suffix is added the name.")
     parser.add_argument(
+        "-cn", "--clean-names", action="store_true", 
+        help=f"Whether to rename the files to os-compatible before processing. "
+             f"For instance, this will rename '北亰.jpg' to 'Bei Jing.jpg', "
+             f"'<>a?bc.jpg.jpg' to 'abcjpg.jpg' etc. Useful because some path "
+             f"errors could occur while reading those images when processing. "
+             f"Note that this will create a temporary directory with renamed "
+             f"images; to rename the images in-place, use `-ci`."
+    )
+    parser.add_argument(
+        "-ci", "--clean-names-inplace", action="store_true",
+        help=f"Same functionality as `--clean-names`, except that all the "
+             f"files are renamed in `input_dir`. This is not advised, however, "
+             f"if the directory contains many images, copying them to a "
+             f"temporary directory may be inefficient, thus this option can "
+             f"just rename the files in-place. Note that specifying this, "
+             f"will override `-cn` option, regardless if it's specified of not."
+    )
+    parser.add_argument(
         "-s", "--output-size", type=int, nargs='+', default=[256, 256], 
         help=f"The output size (width, height) of cropped image faces. If "
              f"provided as a single number, the same value is used for both "
              f"width and height. Defaults to [256, 256].")
     parser.add_argument(
         "-f", "--output-format", type=str, 
         help=f"The output format of the saved face images, e.g., 'jpg', 'png'."
@@ -142,18 +162,18 @@
              f"Defaults to 0.65.")
     parser.add_argument(
         "-st", "--strategy", type=str, default="largest",
         choices=["all", "best", "largest"],
         help=f"The strategy to use to extract faces from each image. Defaults "
              f"to 'largest'.")
     parser.add_argument(
-        "-p", "--padding", type=str, default="reflect",
+        "-p", "--padding", type=str, default="constant",
         choices=["constant", "replicate", "reflect", "wrap", "reflect_101"], 
         help=f"The padding type (border mode) to apply when cropping out faces"
-             f" near edges. Defaults to 'reflect'.")
+             f" near edges. Defaults to 'constant'.")
     parser.add_argument(
         "-a", "--allow-skew", action="store_true", 
         help=f"Whether to allow skewing the faces to better match the the "
              f"standard (average) face landmarks.")
     parser.add_argument(
         "-l", "--landmarks", type=str, 
         help=f"Path to landmarks file if landmarks are already known and "
@@ -175,41 +195,49 @@
     parser.add_argument(
         "-dt", "--det-threshold", type=float, default=0.6, 
         help=f"The visual threshold, i.e., minimum confidence score, for a "
              f"detected face to be considered an actual face. If a negative "
              f"value is provided, e.g., -1, landmark prediction is not "
              f"performed. Defaults to 0.6.")
     parser.add_argument(
-        "-et", "--enh-threshold", type=float, default=0.001, 
-        help=f"Quality enhancement threshold that tells when the image quality"
+        "-et", "--enh-threshold", type=float, default=-1, 
+        help=f"Quality enhancement threshold that tells when the image quality "
              f"should be enhanced. It is the minimum average face factor in "
-             f"the input image. Defaults to 0.001.")
+             f"the input image, below which the image is enhanced. It is "
+             f"advised to set this to a low number, like 0.001 - very high "
+             f"fractions might unnecessarily cause the image quality to be "
+             f"improved. If a negative value is provided, no enhancement is "
+             f"performed. Defaults to -1.")
     parser.add_argument(
         "-b", "--batch-size", type=int, default=8, 
         help=f"The batch size. It is the maximum number of images that can be "
              f"processed by every processor at a single time-step. Defaults "
              f"to 8.")
     parser.add_argument(
         "-n", "--num-processes", type=int, default=1, 
         help=f"The number of processes to launch to perform image processing. "
              f"If landmarks are provided and no quality enhancement or "
              f"attribute grouping is done, feel free to set this to the "
              f"number of CPUs your machine has. Defaults to 1.")
     parser.add_argument(
-        "-d", "--device", type=str, default="cpu", 
+        "-d", "--device", type=str, default="auto", 
         help=f"The device on which to perform the predictions, i.e., landmark "
-             f"detection, quality enhancement and face  parsing. Defaults to "
-             f"'cpu'.")
+             f"detection, quality enhancement and face parsing. If specified "
+             f"as 'auto', it will be checked if CUDA is available and thus "
+             f"used, otherwise CPU will be assigned. Defaults to 'auto'.")
 
     # Parse arguments and convert to dict
     kwargs = vars(parser.parse_args())
     
     if kwargs["input_dir"] is None:
         raise ValueError("Input directory must be specified.")
     
+    if kwargs["device"] == "auto":
+        kwargs["device"] = "cuda" if torch.cuda.is_available() else "cpu"
+    
     if kwargs["det_threshold"] is not None and kwargs["det_threshold"] < 0:
         # If negative, set it to None
         kwargs["det_threshold"] = None
     
     if kwargs["enh_threshold"] is not None and kwargs["enh_threshold"] < 0:
         # If negative, set it to None
         kwargs["enh_threshold"] = None
@@ -225,17 +253,33 @@
     3 main features the cropper can do (either together or separately): 
     align and center-crop face images, enhance quality, group by 
     attributes. For more details, see :class:`.Cropper`.
     """
     # Parse arguments
     kwargs = parse_args()
 
-    # Pop the input and output dirs
+    # Pop some dir and naming arguments
     input_dir = kwargs.pop("input_dir")
     output_dir = kwargs.pop("output_dir")
+    needs_clean = kwargs.pop("clean_names")
+    is_inplace = kwargs.pop("clean_names_inplace")
+
+    if needs_clean or is_inplace:
+        # Clean file names (either in-place or copy to temp dir)
+        cn_output_dir = None if is_inplace else input_dir + "_temp"
+        clean_names(input_dir=input_dir, output_dir=cn_output_dir)
+    
+    if needs_clean and not is_inplace:
+        # Update the provided input and output directories
+        output_dir = input_dir + "_faces" if output_dir is None else output_dir
+        input_dir += "_temp"
 
     # Init cropper and process
     cropper = Cropper(**kwargs)
     cropper.process_dir(input_dir, output_dir)
 
+    if needs_clean and not is_inplace:
+        # Remove temporary dir
+        shutil.rmtree(input_dir)
+
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/cropper.py` & `face-crop-plus-1.1.0/src/face_crop_plus/cropper.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
            faces, if zoomed in, is low. Quality enhancement feature 
            allows to remove the blurriness. It can also enhance the 
            quality of every image, if desired (see 
            :class:`.RRDBNet`).
         3. **Face parsing** - automatic face attribute parsing and 
            grouping to sub-directories according selected attributes. 
            Attributes can indicate to group faces that contain specific 
-           properties, e.g., "earrings and neckless", "glasses". They 
+           properties, e.g., "earrings and necklace", "glasses". They 
            can also indicate what properties the faces should not 
            include to form a group, e.g., "no accessories" group would 
            indicate to include faces without hats, glasses, earrings, 
-           neckless etc. It is also possible to generate masks for 
+           necklace etc. It is also possible to generate masks for 
            selected face attributes, e.g., "glasses", 
            "eyes and eyebrows". For more intuition on how grouping 
            works, see :class:`.BiSeNet` and 
            :meth:`save_groups`.
 
     The class is designed to perform all or some combination of the 
     functions in one go, however, each feature is independent of one 
@@ -139,21 +139,21 @@
     def __init__(
         self,
         output_size: int | tuple[int, int] | list[int] = 256,
         output_format: str | None = None,
         resize_size: int | tuple[int, int] | list[int] = 1024,
         face_factor: float = 0.65,
         strategy: str = "largest",
-        padding: str = "reflect",
+        padding: str = "constant",
         allow_skew: bool = False,
         landmarks: str | tuple[np.ndarray, np.ndarray] | None = None,
         attr_groups: dict[str, list[int]] | None = None,
         mask_groups: dict[str, list[int]] | None = None,
         det_threshold: float | None = 0.6,
-        enh_threshold: float | None = 0.001,
+        enh_threshold: float | None = None,
         batch_size: int = 8,
         num_processes: int = 1,
         device: str | torch.device = "cpu",
     ):
         """Initializes the cropper.
 
         Initializes class attributes. 
@@ -274,15 +274,18 @@
                 an actual face. See :meth:`.RetinaFace.__init__` for 
                 more details. If None, no face detection will be 
                 performed. Defaults to 0.6.
             enh_threshold: Quality enhancement threshold that tells when 
                 the image quality should be enhanced (it is an expensive 
                 operation). It is the minimum average face factor, i.e., 
                 face area relative to the image, below which the whole 
-                image is enhanced. Defaults to 0.001.
+                image is enhanced. It is advised to set this to a low 
+                number, like 0.001 - very high fractions might 
+                unnecessarily cause the image quality to be improved.
+                Defaults to None.
             batch_size: The batch size. It is the maximum number of 
                 images that can be processed by every processor at a 
                 single time-step. Large values may result in memory 
                 errors, especially, when GPU acceleration is used. 
                 Increase this if less models (i.e., landmark detection, 
                 quality enhancement, face parsing models) are used and 
                 decrease otherwise. Defaults to 8.
@@ -413,15 +416,15 @@
             ValueError: If the number of standard landmarks is not 
                 supported. The number of standard landmarks is 
                 ``self.num_std_landmarks``.
         """
         match self.num_std_landmarks:
             case 5:
                 # If the number of std landmarks is 5
-                std_landmarks = STANDARD_LANDMARKS_5
+                std_landmarks = STANDARD_LANDMARKS_5.copy()
             case _:
                 # Otherwise the number of STD landmarks is not supported
                 raise ValueError(f"Unsupported number of standard landmarks "
                                  f"for estimating alignment transform matrix: "
                                  f"{self.num_std_landmarks}.")
         
         # Apply appropriate scaling based on face factor and out size
@@ -787,21 +790,25 @@
         # Read images and filter valid corresponding file names
         images, file_names = read_images(file_names, input_dir)
 
         if self.landmarks is None and self.det_model is None:
             # One-to-one image to index mapping and no landmarks
             indices, landmarks = list(range(len(file_names))), None
         elif self.landmarks is not None:
-            # Initialize empty idx lists
-            indices, indices_ldm = [], []
+            # Initialize empty idx lists and None paddings
+            indices, indices_ldm, paddings = [], [], None
 
             for i, file_name in enumerate(file_names):
                 # Check the indices of landmark sets in landmarks file
                 indices_i = np.where(file_name == self.landmarks[1])[0]
 
+                if len(indices_i) == 0:
+                    # Has no landmarks
+                    continue
+
                 # Update img & ldm file name indices
                 indices.extend([i] * len(indices_i))
                 indices_ldm.extend(indices_i.tolist())
             
             # Set landmarks according to the indices
             landmarks = self.landmarks[0][indices_ldm]
             
@@ -838,15 +845,20 @@
         if self.par_model is not None:
             # Predict attribute and mask groups if face parsing desired
             groups = self.par_model.predict(as_tensor(images, self.device))
 
         # Pick file names for each face, save faces (by groups if exist)
         self.save_groups(images, file_names[indices], output_dir, *groups)
     
-    def process_dir(self, input_dir: str, output_dir: str | None = None):
+    def process_dir(
+        self, 
+        input_dir: str, 
+        output_dir: str | None = None,
+        desc: str | None = "Processing",
+    ):
         """Processes images in the specified input directory.
 
         Splits all the file names in the input directory to batches 
         and processes batches on multiple cores. For every file name 
         batch, images are loaded, some are optionally enhanced, 
         landmarks are generated and used to optionally align and 
         center-crop faces, and grouping is optionally applied based on
@@ -861,14 +873,17 @@
 
         Args:
             input_dir: Path to input directory with image files.
             output_dir: Path to output directory to save the extracted 
                 (and optionally grouped to sub-directories) face images. 
                 If None, then the same path as for ``input_dir`` is used 
                 and additionally "_faces" suffix is added to the name.
+            desc: The description to use for the progress bar. If 
+                specified as ``None``, no progress bar is shown. 
+                Defaults to "Processing".
         """
         if output_dir is None:
             # Create a default output dir name
             output_dir = input_dir + "_faces"
 
         # Create batches of image file names in input dir
         files, bs = os.listdir(input_dir), self.batch_size
@@ -881,8 +896,14 @@
         # Define worker function and its additional arguments
         kwargs = {"input_dir": input_dir, "output_dir": output_dir}
         worker = partial(self.process_batch, **kwargs)
         
         with ThreadPool(self.num_processes, self._init_models) as pool:
             # Create imap object and apply workers to it
             imap = pool.imap_unordered(worker, file_batches)
-            list(tqdm.tqdm(imap, total=len(file_batches), desc="Processing"))
+            
+            if desc is not None:
+                # If description is provided, wrap progress bar around
+                imap = tqdm.tqdm(imap, total=len(file_batches), desc=desc)
+            
+            # Process
+            list(imap)
```

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/models/_layers.py` & `face-crop-plus-1.1.0/src/face_crop_plus/models/_layers.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/models/bise.py` & `face-crop-plus-1.1.0/src/face_crop_plus/models/bise.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         * 8 - right ear
         * 9 - earing
         * 10 - nose
         * 11 - mouth
         * 12 - upper lip
         * 13 - lower lip
         * 14 - neck
-        * 15 - neckless
+        * 15 - necklace
         * 16 - clothes
         * 17 - hair
         * 18 - hat
 
     Some examples of grouping by attributes:
 
         * ``'glasses': [6]`` - this will put each face image that 
           contains pixels labeled as 6 to a category called 'glasses'.
-        * ``'earings_and_neckless': [9, 15]`` - this will put each image 
+        * ``'earings_and_necklace': [9, 15]`` - this will put each image 
           that contains pixels labeled as 9 and also contains pixels
-          labeled as 15 to a category called 'earings_and_neckless'.
+          labeled as 15 to a category called 'earings_and_necklace'.
         * ``'no_accessories': [-6, -9, -15, -18]`` - this will put each 
           face image that does not contain pixels labeled as either 6, 
           9, 15, or 18 to a category called 'no_accessories'.
     
     Some examples of grouping by mask:
 
         * ``'nose': [10]`` - this will put each face image that contains 
@@ -137,15 +137,15 @@
             specified variables here are mainly relevant only for 
             :meth:`predict`.
 
         Args:
             attr_groups: Dictionary specifying attribute groups, based 
                 on which the face images should be grouped. Each key 
                 represents an attribute group name, e.g., 'glasses', 
-                'earings_and_neckless', 'no_accessories', and each value 
+                'earings_and_necklace', 'no_accessories', and each value 
                 represents attribute indices, e.g., `[6]`, `[9, 15]`, 
                 `[-6, -9, -15, -18]`, each index mapping to some 
                 attribute. Since this model labels face image pixels, if 
                 there is enough pixels with the specified values in the 
                 list, the whole face image will be put into that 
                 attribute category. For negative values, it will be 
                 checked that the labeled face image does not contain
```

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/models/retinaface.py` & `face-crop-plus-1.1.0/src/face_crop_plus/models/retinaface.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus/models/rrdb.py` & `face-crop-plus-1.1.0/src/face_crop_plus/models/rrdb.py`

 * *Files identical despite different names*

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus.egg-info/PKG-INFO` & `face-crop-plus-1.1.0/src/face_crop_plus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: face-crop-plus
-Version: 1.0.3
+Version: 1.1.0
 Summary: Automatic face aligner and cropper with quality enhancement and attribute parsing.
 Home-page: https://github.com/mantasu/face-crop-plus
 Author: Mantas Birškus
 Author-email: mantix7@gmail.com
 License: MIT
 Project-URL: Documentation, https://mantasu.github.io/face-crop-plus
 Project-URL: Bug Tracker, https://github.com/mantasu/face-crop-plus/issues
 Keywords: face,python,pytorch,alignment,cropping,super resolution,quality enhancement,parsing,grouping,attributes,mask,segmentation,celeba
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Face Crop Plus
 
-[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![PyPI](https://img.shields.io/pypi/v/face-crop-plus?color=orange)](https://pypi.org/project/face-crop-plus/)
-[![Python: 3.10](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org/downloads/release/python-3100/)
+[![Python](https://img.shields.io/badge/python-3.10%20|%203.11-yellow)](https://docs.python.org/3/)
 [![CUDA: yes](https://img.shields.io/badge/cuda-yes-green)](https://developer.nvidia.com/cuda-toolkit)
+[![Docs: passing](https://img.shields.io/badge/docs-passing-skyblue)](https://mantasu.github.io/face-crop-plus/)
+[![DOI](https://zenodo.org/badge/621262834.svg)](https://zenodo.org/badge/latestdoi/621262834)
 [![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center" width="100%">
 
 ![Banner](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/banner.png)
 
 </p>
 
 ## About
 
 Image preprocessing package for automatic face alignment and cropping with additional features. It provides the following functionality:
 1. **Face cropping** - face alignment and center-cropping using facial landmarks. Landmarks can be automatically predicted or, if they are already know, can be supplied through a separate file. It is possible to specify face factor, i.e., face area relative to the cropped image, and face extraction strategy, e.g., all faces or largest face per image.
 2. **Face enhancement** - face image quality enhancement. If images are blurry or contain many small faces, quality enhancement model can be used to make the images clearer. Small faces in the image are automatically checked and enhanced if desired.
-3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and neckless_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
+3. **Face parsing** - face attribute parsing and cropped image grouping to sub-directories. Face images can be grouped according to some facial attributes or some combination, such as _glasses_, _earrings and necklace_, _hats_. It is also possible to generate masks for facial attributes or some combination of them, for instance, _glasses_, _nose_, _nose and eyes_.
 
 Please see _References_ section for more details about which models are used for each feature.
 
 > **Note**: each feature can be used separately, e.g., if you just need to enhance the quality of blurry photos, or if you just need to generate attribute masks (like hats, glasses, face parts).
 
 ## Installation
 
@@ -137,40 +139,40 @@
 
 > Quality enhancement can be used as a separate feature to enhance images that contain faces. For an end user, it is a useful feature to boost the quality of photos. It is not suggested to enhance ultra high resolution images (>2000) because your GPU will explode. See _Pure Enhancement/Parsing_ section on how to run it as a stand-alone.
 
 
 ### Attribute Parsing
 
 Face parsing to attributes allows to group output images by category and generate attribute masks for that category. Categorized images are put to their corresponding sub-folders in the output directory.
-* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and neckless_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
+* `attr_groups` - dictionary specifying attribute groups, based on which the face images should be grouped. Each key represents an attribute group name, e.g., _glasses_, _earings and necklace_, _no accessories_, and each value represents attribute indices, e.g., `[6]`, `[9, 15]`, `[-6, -9, -15, -18]`, each index mapping to some attribute. Since this model labels face image pixels, if there is enough pixels with the specified values in the list, the whole face image will be put into that attribute category. For negative values, it will be checked that the labeled face image does not contain those (absolute) values. If it is None, then there will be no grouping according to attributes. Here are some group examples with 2 sample images per group:
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Hats, no glasses <br/> `[18, -6]`     | No accessories <br/> `[-6, -9, -15, -18]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :---------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
-    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)      |
+    | ![ag12](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_2.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_2.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_2.jpg)      |
 
 * `mask_groups` - Dictionary specifying mask groups, based on which the face images and their masks should be grouped. Each key represents a mask group name, e.g., _nose_, _eyes and eyebrows_, and each value represents attribute indices, e.g., `[10]`, `[2, 3, 4, 5]`, each index mapping to some attribute. Since this model labels face image pixels, a mask will be created with 255 (white) at pixels that match the specified attributes and zeros (black) elsewhere. Note that negative values would make no sense here and having them would cause an error. Images are saved to sub-directories named by the mask group and masks are saved to sub-directories under the same name, except with `_mask` suffix. If it is None, then there will be no grouping according to mask groups. Here are some group examples with 1 sample image and its mask per group (for consistency, same images as before):
 
-    | Glasses <br/> `[6]`           | Earrings and neckless <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
+    | Glasses <br/> `[6]`           | Earrings and necklace <br/> `[9, 15]`       | Nose <br/> `[10]`                     | Eyes and eyebrows <br/> `[2, 3, 4, 5]` |
     | :---------------------------: | :-----------------------------------------: | :-----------------------------------: | :------------------------------------: |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
-    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_neckless_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_1.jpg) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_1.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_1.jpg)   |
+    | ![ag11](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/glasses_m.jpg ) | ![ag21](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/earrings_and_necklace_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/hats_no_glasses_m.jpg) | ![ag31](https://raw.githubusercontent.com/mantasu/face-crop-plus/main/assets/no_accessories_m.jpg)   |
 
 > If both `attr_groups` and `mask_groups` are specified, first images are grouped according to face attributes, then images in each groups are further sub-grouped to different mask groups (along with their masks).
 
 
 Here are the 19 possible face attributes (with `0` representing the neutral category):
 
 <p align="center" width="100%">
 
 |                     |                  |                  |
 | ------------------- | ---------------- | ---------------- |
 | `1` - skin          | `7` - left ear   | `13` - lower lip |
 | `2` - left eyebrow  | `8` - right ear  | `14` - neck      |
-| `3` - right eyebrow | `9` - earrings   | `15` - neckless  |
+| `3` - right eyebrow | `9` - earrings   | `15` - necklace  |
 | `4` - left eye      | `10` - nose      | `16` - clothes   |
 | `5` - right eye     | `11` - mouth     | `17` - hair      |
 | `6` - eyeglasses    | `12` - upper lip | `18` - hat       |
 
 </p>
 
 ## Examples
@@ -195,14 +197,33 @@
 For all the available command line arguments, just type (although refer to documentation for more details):
 ```bash
 face-crop-plus -h
 ```
 
 > **Note**: you can use `fcp` as `face-crop-plus` alias , e.g., `fcp -c config.json`
 
+### Cleaning File Names
+
+If your image files contain non-ascii symbols, lengthy names, os-reserved characters, it may be better to standardize them. To do so, it is possible to rename the image files before processing them:
+```bash
+face-crop-plus -i path/to/images --clean-names # --clean-names-inplace (avoids temp dir)
+```
+
+It is possible to specify more arguments via python script. The function can be used in general with any file types:
+
+```python
+from face_crop_plus.utils import clean_names
+
+clean_names(
+    input_dir="path/to/input/dir",
+    output_dir=None, # will rename in-place
+    max_chars=250,
+)
+```
+
 ### Pure Enhancement/Parsing
 
 If you already have aligned and center-cropped face images, you can perform quality enhancement and face parsing without re-cropping them. Here is an example of enhancing quality of every face and parsing them to (note that none of the parameters described in _Alignment and Cropping_ section have any affect here):
 
 ```python
 from face_crop_plus import Cropper
```

### Comparing `face-crop-plus-1.0.3/src/face_crop_plus.egg-info/SOURCES.txt` & `face-crop-plus-1.1.0/src/face_crop_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

