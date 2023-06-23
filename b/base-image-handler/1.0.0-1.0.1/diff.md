# Comparing `tmp/base_image_handler-1.0.0.tar.gz` & `tmp/base_image_handler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Project\package\package_test2\dist\.tmp-cv2gjqq2\base_image_handler-1.0.0.tar", last modified: Fri Jun 23 08:08:10 2023, max compression
+gzip compressed data, was "D:\Project\package\package_test2\dist\.tmp-_9mu7b5t\base_image_handler-1.0.1.tar", last modified: Fri Jun 23 08:49:43 2023, max compression
```

## Comparing `base_image_handler-1.0.0.tar` & `base_image_handler-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-21 16:02:04.000000 base_image_handler-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      448 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-06-21 15:51:55.000000 base_image_handler-1.0.0/README.md
--rw-rw-rw-   0        0        0      462 2023-06-23 08:07:42.000000 base_image_handler-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler/
--rw-rw-rw-   0        0        0        0 2023-06-21 15:44:40.000000 base_image_handler-1.0.0/src/base_image_handler/__init__.py
--rw-rw-rw-   0        0        0      945 2023-06-23 07:50:12.000000 base_image_handler-1.0.0/src/base_image_handler/mask_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler.egg-info/
--rw-rw-rw-   0        0        0      448 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-23 08:08:10.000000 base_image_handler-1.0.0/src/base_image_handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-21 16:02:04.000000 base_image_handler-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-06-21 15:51:55.000000 base_image_handler-1.0.1/README.md
+-rw-rw-rw-   0        0        0      462 2023-06-23 08:49:12.000000 base_image_handler-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:44:40.000000 base_image_handler-1.0.1/src/base_image_handler/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-06-23 08:48:54.000000 base_image_handler-1.0.1/src/base_image_handler/mask_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 08:49:43.000000 base_image_handler-1.0.1/src/base_image_handler.egg-info/top_level.txt
```

### Comparing `base_image_handler-1.0.0/LICENSE` & `base_image_handler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `base_image_handler-1.0.0/src/base_image_handler/mask_handler.py` & `base_image_handler-1.0.1/src/base_image_handler/mask_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cv2
 import numpy as np
 
 def add_one(number):
     return number + 10
 
-def mask_postprocess(self, mask, thres=20):
+def mask_postprocess(mask, thres=20):
     mask[:thres, :] = 0; mask[-thres:, :] = 0
     mask[:, :thres] = 0; mask[:, -thres:] = 0        
     mask = cv2.GaussianBlur(mask, (91, 91), 11)
     mask = cv2.GaussianBlur(mask, (91, 91), 11)
     return mask.astype(np.float32)
 
 def preprocess_border(full_img, y1, y2, x1, x2, default_padding = 50): ## extend border
```

