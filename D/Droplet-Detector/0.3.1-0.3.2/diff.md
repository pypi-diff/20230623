# Comparing `tmp/Droplet-Detector-0.3.1.tar.gz` & `tmp/Droplet_Detector-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Droplet-Detector-0.3.1.tar", last modified: Fri Jun 23 18:56:18 2023, max compression
+gzip compressed data, was "Droplet_Detector-0.3.2.tar", last modified: Fri Jun 23 19:33:31 2023, max compression
```

## Comparing `Droplet-Detector-0.3.1.tar` & `Droplet_Detector-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:56:18.609571 Droplet-Detector-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-06-23 18:56:18.577557 Droplet-Detector-0.3.1/Droplet-Detector/
--rw-rw-rw-   0        0        0     7192 2023-06-21 22:35:57.000000 Droplet-Detector-0.3.1/Droplet-Detector/Bot.py
--rw-rw-rw-   0        0        0      281 2023-06-23 16:56:01.000000 Droplet-Detector-0.3.1/Droplet-Detector/__init__.py
--rw-rw-rw-   0        0        0      407 2023-06-21 12:37:46.000000 Droplet-Detector-0.3.1/Droplet-Detector/calculate.py
--rw-rw-rw-   0        0        0     1207 2023-06-21 22:37:50.000000 Droplet-Detector-0.3.1/Droplet-Detector/do_xslx.py
--rw-rw-rw-   0        0        0     2306 2023-06-21 22:47:13.000000 Droplet-Detector-0.3.1/Droplet-Detector/draw.py
--rw-rw-rw-   0        0        0     1782 2023-06-21 22:44:54.000000 Droplet-Detector-0.3.1/Droplet-Detector/get_contours.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:56:18.605565 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/
--rw-rw-rw-   0        0        0     6427 2023-06-23 18:56:18.000000 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-23 18:56:18.000000 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:56:18.000000 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2023-06-23 18:56:18.000000 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-23 18:56:18.000000 Droplet-Detector-0.3.1/Droplet_Detector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6427 2023-06-23 18:56:18.609571 Droplet-Detector-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5818 2023-06-23 17:00:22.000000 Droplet-Detector-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 18:56:18.613574 Droplet-Detector-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-06-23 18:56:09.000000 Droplet-Detector-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:33:31.519251 Droplet_Detector-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-06-23 19:33:31.455236 Droplet_Detector-0.3.2/Droplet_Detector/
+-rw-rw-rw-   0        0        0     7243 2023-06-23 19:28:37.000000 Droplet_Detector-0.3.2/Droplet_Detector/Bot.py
+-rw-rw-rw-   0        0        0      281 2023-06-23 16:56:01.000000 Droplet_Detector-0.3.2/Droplet_Detector/__init__.py
+-rw-rw-rw-   0        0        0      424 2023-06-23 19:28:54.000000 Droplet_Detector-0.3.2/Droplet_Detector/calculate.py
+-rw-rw-rw-   0        0        0     1207 2023-06-21 22:37:50.000000 Droplet_Detector-0.3.2/Droplet_Detector/do_xslx.py
+-rw-rw-rw-   0        0        0     2323 2023-06-23 19:29:12.000000 Droplet_Detector-0.3.2/Droplet_Detector/draw.py
+-rw-rw-rw-   0        0        0     1799 2023-06-23 19:29:24.000000 Droplet_Detector-0.3.2/Droplet_Detector/get_contours.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:33:31.515275 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/
+-rw-rw-rw-   0        0        0     6427 2023-06-23 19:33:31.000000 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-23 19:33:31.000000 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:33:31.000000 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-06-23 19:33:31.000000 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-23 19:33:31.000000 Droplet_Detector-0.3.2/Droplet_Detector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6427 2023-06-23 19:33:31.523252 Droplet_Detector-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5818 2023-06-23 17:00:22.000000 Droplet_Detector-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:33:31.531255 Droplet_Detector-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-06-23 19:31:40.000000 Droplet_Detector-0.3.2/setup.py
```

### Comparing `Droplet-Detector-0.3.1/Droplet-Detector/Bot.py` & `Droplet_Detector-0.3.2/Droplet_Detector/Bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import telebot
 from telebot import types
-from draw import draw_contours_of_drops
-from do_xslx import get_num
-from calculate import get_sum
+from Droplet_Detector.draw import draw_contours_of_drops
+from Droplet_Detector.do_xslx import get_num
+from Droplet_Detector.calculate import get_sum
 
 # Создаем экземпляр бота
 bot = telebot.TeleBot('6050349643:AAHh6MT-s12_9niKl_GwiYRt79NLXDvUk7A')
 global_src = ' '
 
 
 @bot.message_handler(commands=['start'])
```

### Comparing `Droplet-Detector-0.3.1/Droplet-Detector/do_xslx.py` & `Droplet_Detector-0.3.2/Droplet_Detector/do_xslx.py`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.3.1/Droplet-Detector/draw.py` & `Droplet_Detector-0.3.2/Droplet_Detector/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from get_contours import get_contours
+from Droplet_Detector.get_contours import get_contours
 
 
 def draw_contours_of_drops(img_path):
     # читаем пикчу и сохраняем копию
 
     img = cv2.imread(img_path)
     copy = img
```

### Comparing `Droplet-Detector-0.3.1/Droplet-Detector/get_contours.py` & `Droplet_Detector-0.3.2/Droplet_Detector/get_contours.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from calculate import calculate_area
+from Droplet_Detector.calculate import calculate_area
 
 
 def get_contours(img):
     copy = img
 
     img = cv2.medianBlur(img, 3)
```

### Comparing `Droplet-Detector-0.3.1/Droplet_Detector.egg-info/PKG-INFO` & `Droplet_Detector-0.3.2/Droplet_Detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Droplet-Detector
-Version: 0.3.1
+Version: 0.3.2
 Summary: Telegram bot that draws the outlines of drips on a photo 
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Droplet-Detector-0.3.1/PKG-INFO` & `Droplet_Detector-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Droplet-Detector
-Version: 0.3.1
+Name: Droplet_Detector
+Version: 0.3.2
 Summary: Telegram bot that draws the outlines of drips on a photo 
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Droplet-Detector-0.3.1/README.md` & `Droplet_Detector-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.3.1/setup.py` & `Droplet_Detector-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 
 """
 :authors: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2023 kvasik3000
 """
 
-version = '0.3.1'
+version = '0.3.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 # with open("requirements.txt", "r") as file:
 #     requirements = file.read().splitlines()
 
 setup(
-    name='Droplet-Detector',
+    name='Droplet_Detector',
     version=version,
 
     author='Kvas Andrey, Belkova Ksenia, Nekrasova Anna',
     author_email='superadrenoline3000@gmail.com',
 
     description='Telegram bot that draws the outlines of drips on a photo ',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/kvasik3000/Droplet-Detector',
 
     license='Apache License, Version 2.0, see LICENSE file',
 
-    packages=['Droplet-Detector'],
+    packages=['Droplet_Detector'],
     install_requires=[
         'numpy==1.24.3',
         'opencv-python==4.7.0.72',
         'openpyxl==3.1.2',
         'pandas==2.0.2',
         'pyTelegramBotAPI==4.11.0',
         'pytest==7.3.2',
```

