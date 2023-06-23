# Comparing `tmp/irene_pro-0.0.67.tar.gz` & `tmp/irene_pro-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.67.tar", last modified: Fri Jun 23 07:17:03 2023, max compression
+gzip compressed data, was "irene_pro-0.0.68.tar", last modified: Fri Jun 23 08:30:13 2023, max compression
```

## Comparing `irene_pro-0.0.67.tar` & `irene_pro-0.0.68.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:17:03.807664 irene_pro-0.0.67/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.67/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.67/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-23 07:17:03.805669 irene_pro-0.0.67/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.67/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 07:17:03.676017 irene_pro-0.0.67/irene_gui_pkg/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.67/irene_gui_pkg/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.67/irene_gui_pkg/logic.py
--rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.67/irene_gui_pkg/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:17:03.758795 irene_pro-0.0.67/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.67/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.67/irene_pro/logic.py
--rw-rw-rw-   0        0        0    34317 2023-06-23 07:14:03.000000 irene_pro-0.0.67/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:17:03.802678 irene_pro-0.0.67/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-23 07:17:03.000000 irene_pro-0.0.67/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-23 07:17:03.000000 irene_pro-0.0.67/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:17:03.000000 irene_pro-0.0.67/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-23 07:17:03.000000 irene_pro-0.0.67/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-23 07:17:03.000000 irene_pro-0.0.67/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 07:17:03.808662 irene_pro-0.0.67/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-23 07:14:35.000000 irene_pro-0.0.67/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:30:13.637037 irene_pro-0.0.68/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.68/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.68/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-23 08:30:13.635047 irene_pro-0.0.68/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.68/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 08:30:13.558248 irene_pro-0.0.68/irene_gui_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.68/irene_gui_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.68/irene_gui_pkg/logic.py
+-rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.68/irene_gui_pkg/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:30:13.595150 irene_pro-0.0.68/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.68/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.68/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    34313 2023-06-23 08:27:21.000000 irene_pro-0.0.68/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:30:13.625071 irene_pro-0.0.68/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-23 08:30:13.000000 irene_pro-0.0.68/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-23 08:30:13.000000 irene_pro-0.0.68/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:30:13.000000 irene_pro-0.0.68/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-23 08:30:13.000000 irene_pro-0.0.68/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-23 08:30:13.000000 irene_pro-0.0.68/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:30:13.639033 irene_pro-0.0.68/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-23 08:27:24.000000 irene_pro-0.0.68/setup.py
```

### Comparing `irene_pro-0.0.67/PKG-INFO` & `irene_pro-0.0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.67
+Version: 0.0.68
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.67/README.md` & `irene_pro-0.0.68/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.67/irene_gui_pkg/logic.py` & `irene_pro-0.0.68/irene_gui_pkg/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.67/irene_gui_pkg/widgets.py` & `irene_pro-0.0.68/irene_gui_pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.67/irene_pro/logic.py` & `irene_pro-0.0.68/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.67/irene_pro/widgets.py` & `irene_pro-0.0.68/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         except IndexError:
             pass
 
 class btn(Button):
     def __init__(self, master,image = None, **kwargs):
         super().__init__(master=master, compound = "left", bd = 0,font = w(12),image = image, **kwargs)
         
-        prev_color = 'gray70'
+        prev_color = None
         # configure save button
         if 'save' in str(self['text']).lower():
             self.config(bg = "#9400D3", fg = "#fff", image = image)
             prev_color = self.cget('bg')
         
         elif 'edit' in str(self['text']).lower():
             self.config(bg = "#0b4", fg = "#fff", image = image)
```

### Comparing `irene_pro-0.0.67/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.68/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.67
+Version: 0.0.68
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.67/setup.py` & `irene_pro-0.0.68/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3637 270d 0a44 4553 4352   '0.0.67'..DESCR
+00000100: 2027 302e 302e 3638 270d 0a44 4553 4352   '0.0.68'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```
