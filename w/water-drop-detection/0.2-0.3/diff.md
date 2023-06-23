# Comparing `tmp/water_drop_detection-0.2.tar.gz` & `tmp/water_drop_detection-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "water_drop_detection-0.2.tar", last modified: Fri Jun 23 13:43:52 2023, max compression
+gzip compressed data, was "water_drop_detection-0.3.tar", last modified: Fri Jun 23 14:29:35 2023, max compression
```

## Comparing `water_drop_detection-0.2.tar` & `water_drop_detection-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:43:52.126049 water_drop_detection-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-23 13:43:52.126049 water_drop_detection-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-23 13:43:37.000000 water_drop_detection-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:43:52.126049 water_drop_detection-0.2/Water_drop_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:43:39.000000 water_drop_detection-0.2/Water_drop_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 13:43:39.000000 water_drop_detection-0.2/Water_drop_detection/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:43:52.126049 water_drop_detection-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 13:43:39.000000 water_drop_detection-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:43:52.126049 water_drop_detection-0.2/water_drop_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-23 13:43:52.000000 water_drop_detection-0.2/water_drop_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 13:43:52.000000 water_drop_detection-0.2/water_drop_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:43:52.000000 water_drop_detection-0.2/water_drop_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 13:43:52.000000 water_drop_detection-0.2/water_drop_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 13:43:52.000000 water_drop_detection-0.2/water_drop_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:29:35.968643 water_drop_detection-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 14:29:23.000000 water_drop_detection-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:29:35.968643 water_drop_detection-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 14:29:23.000000 water_drop_detection-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/water_drop_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:25.000000 water_drop_detection-0.3/water_drop_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:29:25.000000 water_drop_detection-0.3/water_drop_detection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/water_drop_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/top_level.txt
```

### Comparing `water_drop_detection-0.2/PKG-INFO` & `water_drop_detection-0.3/water_drop_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: water_drop_detection
-Version: 0.2
+Name: water-drop-detection
+Version: 0.3
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
@@ -46,15 +46,15 @@
 
 ## Neural Net
 
 Для детекции капель была выбрана нейросеть с архитектурой Unet, имеющая энкодер ResNet50. Она представляет из себя сверточную нейронную сеть из  двух блоков: энкодера и декодера. Первый из них уменьшает разрешение изображения и увеличивает информационный объем каждого пикселя. Декодер, наоборот, разворачивает выход из энкодера до первоначального размера и выдает маску искомого объекта.  
 
 ---
 
-![](https://github.com/HerrPhoton/Water_drop_detection/blob/Documentation/images/unet.jpg)
+![](https://github.com/HerrPhoton/Water_drop_detection/blob/master/images/unet.jpg))
 
 ---
 
 Данная нейронная сеть проста в реализации и удобна в использовании для решения поставленных целей проекта. Для Unet характерна высокая точность работы при малом объеме данных. В результате её работы есть возможность не только получить маску изображения, 
 но и найти площадь сегментированного объекта.
 
 ---
@@ -90,20 +90,20 @@
 
 Для пользователя:
 ```
 pip install water-drop-detection
 ```
 + Для запуска проекта через py файл:
 ```
-from water-drop-detection import main
+from water_drop_detection import main
 main.main()
 ```
 + Или при клонировании репозитория можно вызвать:
 ```
-python Water_drop_detection/main.py
+python water_drop_detection/main.py
 ```
 
 Для разработчика:
 + Вы можете скачать проект по этой ссылке: https://github.com/HerrPhoton/Water_drop_detection
 + Или клонировать репозиторий нижеприведенной командой:
 ```
 git clone https://github.com/HerrPhoton/Water_drop_detection
```

### Comparing `water_drop_detection-0.2/README.md` & `water_drop_detection-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 ## Neural Net
 
 Для детекции капель была выбрана нейросеть с архитектурой Unet, имеющая энкодер ResNet50. Она представляет из себя сверточную нейронную сеть из  двух блоков: энкодера и декодера. Первый из них уменьшает разрешение изображения и увеличивает информационный объем каждого пикселя. Декодер, наоборот, разворачивает выход из энкодера до первоначального размера и выдает маску искомого объекта.  
 
 ---
 
-![](https://github.com/HerrPhoton/Water_drop_detection/blob/Documentation/images/unet.jpg)
+![](https://github.com/HerrPhoton/Water_drop_detection/blob/master/images/unet.jpg))
 
 ---
 
 Данная нейронная сеть проста в реализации и удобна в использовании для решения поставленных целей проекта. Для Unet характерна высокая точность работы при малом объеме данных. В результате её работы есть возможность не только получить маску изображения, 
 но и найти площадь сегментированного объекта.
 
 ---
@@ -73,20 +73,20 @@
 
 Для пользователя:
 ```
 pip install water-drop-detection
 ```
 + Для запуска проекта через py файл:
 ```
-from water-drop-detection import main
+from water_drop_detection import main
 main.main()
 ```
 + Или при клонировании репозитория можно вызвать:
 ```
-python Water_drop_detection/main.py
+python water_drop_detection/main.py
 ```
 
 Для разработчика:
 + Вы можете скачать проект по этой ссылке: https://github.com/HerrPhoton/Water_drop_detection
 + Или клонировать репозиторий нижеприведенной командой:
 ```
 git clone https://github.com/HerrPhoton/Water_drop_detection
```

### Comparing `water_drop_detection-0.2/setup.py` & `water_drop_detection-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     read_me = file.read()
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setuptools.setup(
     name = "water_drop_detection",
-    version = "0.2",
+    version = "0.3",
     author = "Aleksandr Leisle, Sofia Volodina, Alina Shitenko",
     author_email = "a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru",
     description = "A neural network that detects water drops on the surface from an image.",
     long_description = read_me,
     long_description_content_type = "text/markdown",
     project_urls = {
         'Documentation': 'https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf',
         'Bug Tracker': 'https://github.com/HerrPhoton/Water_drop_detection/issues',
         'Homepage': 'https://github.com/HerrPhoton/Water_drop_detection',
     },
-    packages = ['Water_drop_detection'],
+    packages = ['water_drop_detection'],
     install_requires = requirements,
     classifiers = [
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     python_requires = '==3.9.*',
 )
```

### Comparing `water_drop_detection-0.2/water_drop_detection.egg-info/PKG-INFO` & `water_drop_detection-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: water-drop-detection
-Version: 0.2
+Name: water_drop_detection
+Version: 0.3
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
@@ -46,15 +46,15 @@
 
 ## Neural Net
 
 Для детекции капель была выбрана нейросеть с архитектурой Unet, имеющая энкодер ResNet50. Она представляет из себя сверточную нейронную сеть из  двух блоков: энкодера и декодера. Первый из них уменьшает разрешение изображения и увеличивает информационный объем каждого пикселя. Декодер, наоборот, разворачивает выход из энкодера до первоначального размера и выдает маску искомого объекта.  
 
 ---
 
-![](https://github.com/HerrPhoton/Water_drop_detection/blob/Documentation/images/unet.jpg)
+![](https://github.com/HerrPhoton/Water_drop_detection/blob/master/images/unet.jpg))
 
 ---
 
 Данная нейронная сеть проста в реализации и удобна в использовании для решения поставленных целей проекта. Для Unet характерна высокая точность работы при малом объеме данных. В результате её работы есть возможность не только получить маску изображения, 
 но и найти площадь сегментированного объекта.
 
 ---
@@ -90,20 +90,20 @@
 
 Для пользователя:
 ```
 pip install water-drop-detection
 ```
 + Для запуска проекта через py файл:
 ```
-from water-drop-detection import main
+from water_drop_detection import main
 main.main()
 ```
 + Или при клонировании репозитория можно вызвать:
 ```
-python Water_drop_detection/main.py
+python water_drop_detection/main.py
 ```
 
 Для разработчика:
 + Вы можете скачать проект по этой ссылке: https://github.com/HerrPhoton/Water_drop_detection
 + Или клонировать репозиторий нижеприведенной командой:
 ```
 git clone https://github.com/HerrPhoton/Water_drop_detection
```

