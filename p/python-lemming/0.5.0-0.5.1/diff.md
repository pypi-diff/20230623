# Comparing `tmp/python-lemming-0.5.0.tar.gz` & `tmp/python-lemming-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.5.0.tar", last modified: Mon Jun 12 17:16:12 2023, max compression
+gzip compressed data, was "python-lemming-0.5.1.tar", last modified: Fri Jun 23 13:15:56 2023, max compression
```

## Comparing `python-lemming-0.5.0.tar` & `python-lemming-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.808163 python-lemming-0.5.0/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     6305 2023-06-12 17:16:12.809163 python-lemming-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5341 2023-06-11 12:10:56.000000 python-lemming-0.5.0/README.md
--rw-rw-rw-   0        0        0     1625 2023-06-12 17:12:49.000000 python-lemming-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0     1455 2023-06-12 17:16:12.823163 python-lemming-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.720165 python-lemming-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.742164 python-lemming-0.5.0/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-06-12 17:15:21.000000 python-lemming-0.5.0/src/lemming/__init__.py
--rw-rw-rw-   0        0        0     9671 2023-06-12 17:12:49.000000 python-lemming-0.5.0/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    11252 2023-06-12 17:12:49.000000 python-lemming-0.5.0/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.5.0/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.807165 python-lemming-0.5.0/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0     6305 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.5.0/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.623979 python-lemming-0.5.1/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     6305 2023-06-23 13:15:56.624979 python-lemming-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5341 2023-06-11 12:10:56.000000 python-lemming-0.5.1/README.md
+-rw-rw-rw-   0        0        0     1625 2023-06-12 17:12:49.000000 python-lemming-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1456 2023-06-23 13:15:56.629979 python-lemming-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.575980 python-lemming-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.602980 python-lemming-0.5.1/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-06-23 12:58:00.000000 python-lemming-0.5.1/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0     9713 2023-06-23 12:58:11.000000 python-lemming-0.5.1/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    11284 2023-06-23 13:00:24.000000 python-lemming-0.5.1/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.5.1/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.622979 python-lemming-0.5.1/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0     6305 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.5.1/src/python_lemming.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.5.0/LICENSE` & `python-lemming-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.5.0/PKG-INFO` & `python-lemming-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

### Comparing `python-lemming-0.5.0/README.md` & `python-lemming-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-lemming-0.5.0/pyproject.toml` & `python-lemming-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-lemming-0.5.0/setup.cfg` & `python-lemming-0.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,77 +15,77 @@
 000000e0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 000000f0: 622e 636f 6d2f 6b6f 7669 7562 6935 362f  b.com/koviubi56/
 00000100: 6c65 6d6d 696e 670d 0a61 7574 686f 7220  lemming..author 
 00000110: 3d20 4b6f 7669 7562 6935 360d 0a61 7574  = Koviubi56..aut
 00000120: 686f 725f 656d 6169 6c20 3d20 6b6f 7669  hor_email = kovi
 00000130: 7562 6935 3640 6475 636b 2e63 6f6d 0d0a  ubi56@duck.com..
 00000140: 6c69 6365 6e73 6520 3d20 4750 4c0d 0a6c  license = GPL..l
-00000150: 6963 656e 7365 5f66 696c 6520 3d20 4c49  icense_file = LI
-00000160: 4345 4e53 450d 0a70 6c61 7466 6f72 6d73  CENSE..platforms
-00000170: 203d 2075 6e69 782c 206c 696e 7578 2c20   = unix, linux, 
-00000180: 6f73 782c 2063 7967 7769 6e2c 2077 696e  osx, cygwin, win
-00000190: 3332 0d0a 636c 6173 7369 6669 6572 7320  32..classifiers 
-000001a0: 3d20 0d0a 094c 6963 656e 7365 203a 3a20  = ...License :: 
-000001b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001c0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-000001d0: 6963 204c 6963 656e 7365 2076 3320 6f72  ic License v3 or
-000001e0: 206c 6174 6572 2028 4750 4c76 332b 290d   later (GPLv3+).
-000001f0: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
-00000200: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
-00000210: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000220: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000230: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
-00000240: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000250: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-00000260: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
-00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000280: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-000002c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002d0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-000002e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000300: 3a20 332e 3131 0d0a 0950 726f 6772 616d  : 3.11...Program
-00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000320: 2050 7974 686f 6e20 3a3a 2033 2e31 320d   Python :: 3.12.
-00000330: 0a6b 6579 776f 7264 7320 3d20 6c65 6d6d  .keywords = lemm
-00000340: 696e 672c 2066 6f72 6d61 742c 2066 6f72  ing, format, for
-00000350: 6d61 7474 6572 2c20 6c69 6e74 2c20 6c69  matter, lint, li
-00000360: 6e74 696e 672c 206c 696e 7465 720d 0a0d  nting, linter...
-00000370: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000380: 6167 6573 203d 200d 0a09 6c65 6d6d 696e  ages = ...lemmin
-00000390: 670d 0a69 6e73 7461 6c6c 5f72 6571 7569  g..install_requi
-000003a0: 7265 7320 3d20 0d0a 0974 6f6d 6c69 3b20  res = ...tomli; 
-000003b0: 7079 7468 6f6e 5f76 6572 7369 6f6e 3c27  python_version<'
-000003c0: 332e 3131 270d 0a09 7079 7468 6f6e 2d6d  3.11'...python-m
-000003d0: 796c 6f67 3e3d 302e 372e 300d 0a09 636f  ylog>=0.7.0...co
-000003e0: 6e66 7a0d 0a09 7479 7069 6e67 2d65 7874  nfz...typing-ext
-000003f0: 656e 7369 6f6e 733e 3d34 2e34 2e30 0d0a  ensions>=4.4.0..
-00000400: 0974 7970 6572 0d0a 7079 7468 6f6e 5f72  .typer..python_r
-00000410: 6571 7569 7265 7320 3d20 3e3d 332e 3131  equires = >=3.11
-00000420: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000430: 0d0a 093d 7372 630d 0a7a 6970 5f73 6166  ...=src..zip_saf
-00000440: 6520 3d20 6e6f 0d0a 0d0a 5b6f 7074 696f  e = no....[optio
-00000450: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000460: 0d0a 6c65 6d6d 696e 6720 3d20 7079 2e74  ..lemming = py.t
-00000470: 7970 6564 0d0a 0d0a 5b6f 7074 696f 6e73  yped....[options
-00000480: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000490: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-000004a0: 3d20 0d0a 096c 656d 6d69 6e67 203d 206c  = ...lemming = l
-000004b0: 656d 6d69 6e67 2e5f 5f6d 6169 6e5f 5f3a  emming.__main__:
-000004c0: 6d61 696e 0d0a 0d0a 5b70 7963 6f64 6573  main....[pycodes
-000004d0: 7479 6c65 5d0d 0a69 676e 6f72 6520 3d20  tyle]..ignore = 
-000004e0: 4532 3033 0d0a 0d0a 5b70 796c 616d 615d  E203....[pylama]
-000004f0: 0d0a 6967 6e6f 7265 203d 2057 3530 330d  ..ignore = W503.
-00000500: 0a0d 0a5b 666c 616b 6538 5d0d 0a65 7874  ...[flake8]..ext
-00000510: 656e 642d 6967 6e6f 7265 203d 2057 3530  end-ignore = W50
-00000520: 330d 0a65 7874 656e 642d 6578 636c 7564  3..extend-exclud
-00000530: 6520 3d20 7665 6e76 2c2a 6361 6368 652a  e = venv,*cache*
-00000540: 0d0a 7065 722d 6669 6c65 2d69 676e 6f72  ..per-file-ignor
-00000550: 6573 203d 200d 0a09 7465 7374 732f 2a3a  es = ...tests/*:
-00000560: 2053 3130 310d 0a0d 0a5b 6973 6f72 745d   S101....[isort]
-00000570: 0d0a 7072 6f66 696c 6520 3d20 626c 6163  ..profile = blac
-00000580: 6b0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  k....[egg_info].
-00000590: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000005a0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000150: 6963 656e 7365 5f66 696c 6573 203d 204c  icense_files = L
+00000160: 4943 454e 5345 0d0a 706c 6174 666f 726d  ICENSE..platform
+00000170: 7320 3d20 756e 6978 2c20 6c69 6e75 782c  s = unix, linux,
+00000180: 206f 7378 2c20 6379 6777 696e 2c20 7769   osx, cygwin, wi
+00000190: 6e33 320d 0a63 6c61 7373 6966 6965 7273  n32..classifiers
+000001a0: 203d 200d 0a09 4c69 6365 6e73 6520 3a3a   = ...License ::
+000001b0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001c0: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+000001d0: 6c69 6320 4c69 6365 6e73 6520 7633 206f  lic License v3 o
+000001e0: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
+000001f0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
+00000200: 7461 7475 7320 3a3a 2034 202d 2042 6574  tatus :: 4 - Bet
+00000210: 610d 0a09 5072 6f67 7261 6d6d 696e 6720  a...Programming 
+00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000230: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
+00000240: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000250: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
+00000260: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
+00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000280: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
+00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002b0: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+000002c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002d0: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+000002e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000300: 3a3a 2033 2e31 310d 0a09 5072 6f67 7261  :: 3.11...Progra
+00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+00000330: 0d0a 6b65 7977 6f72 6473 203d 206c 656d  ..keywords = lem
+00000340: 6d69 6e67 2c20 666f 726d 6174 2c20 666f  ming, format, fo
+00000350: 726d 6174 7465 722c 206c 696e 742c 206c  rmatter, lint, l
+00000360: 696e 7469 6e67 2c20 6c69 6e74 6572 0d0a  inting, linter..
+00000370: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+00000380: 6b61 6765 7320 3d20 0d0a 096c 656d 6d69  kages = ...lemmi
+00000390: 6e67 0d0a 696e 7374 616c 6c5f 7265 7175  ng..install_requ
+000003a0: 6972 6573 203d 200d 0a09 746f 6d6c 693b  ires = ...tomli;
+000003b0: 2070 7974 686f 6e5f 7665 7273 696f 6e3c   python_version<
+000003c0: 2733 2e31 3127 0d0a 0970 7974 686f 6e2d  '3.11'...python-
+000003d0: 6d79 6c6f 673e 3d30 2e37 2e30 0d0a 0963  mylog>=0.7.0...c
+000003e0: 6f6e 667a 0d0a 0974 7970 696e 672d 6578  onfz...typing-ex
+000003f0: 7465 6e73 696f 6e73 3e3d 342e 342e 300d  tensions>=4.4.0.
+00000400: 0a09 7479 7065 720d 0a70 7974 686f 6e5f  ..typer..python_
+00000410: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
+00000420: 310d 0a70 6163 6b61 6765 5f64 6972 203d  1..package_dir =
+00000430: 200d 0a09 3d73 7263 0d0a 7a69 705f 7361   ...=src..zip_sa
+00000440: 6665 203d 206e 6f0d 0a0d 0a5b 6f70 7469  fe = no....[opti
+00000450: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+00000460: 5d0d 0a6c 656d 6d69 6e67 203d 2070 792e  ]..lemming = py.
+00000470: 7479 7065 640d 0a0d 0a5b 6f70 7469 6f6e  typed....[option
+00000480: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000490: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+000004a0: 203d 200d 0a09 6c65 6d6d 696e 6720 3d20   = ...lemming = 
+000004b0: 6c65 6d6d 696e 672e 5f5f 6d61 696e 5f5f  lemming.__main__
+000004c0: 3a6d 6169 6e0d 0a0d 0a5b 7079 636f 6465  :main....[pycode
+000004d0: 7374 796c 655d 0d0a 6967 6e6f 7265 203d  style]..ignore =
+000004e0: 2045 3230 330d 0a0d 0a5b 7079 6c61 6d61   E203....[pylama
+000004f0: 5d0d 0a69 676e 6f72 6520 3d20 5735 3033  ]..ignore = W503
+00000500: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6578  ....[flake8]..ex
+00000510: 7465 6e64 2d69 676e 6f72 6520 3d20 5735  tend-ignore = W5
+00000520: 3033 0d0a 6578 7465 6e64 2d65 7863 6c75  03..extend-exclu
+00000530: 6465 203d 2076 656e 762c 2a63 6163 6865  de = venv,*cache
+00000540: 2a0d 0a70 6572 2d66 696c 652d 6967 6e6f  *..per-file-igno
+00000550: 7265 7320 3d20 0d0a 0974 6573 7473 2f2a  res = ...tests/*
+00000560: 3a20 5331 3031 0d0a 0d0a 5b69 736f 7274  : S101....[isort
+00000570: 5d0d 0a70 726f 6669 6c65 203d 2062 6c61  ]..profile = bla
+00000580: 636b 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ck....[egg_info]
+00000590: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000005a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `python-lemming-0.5.0/src/lemming/__init__.py` & `python-lemming-0.5.1/src/lemming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.5.0/src/lemming/__main__.py` & `python-lemming-0.5.1/src/lemming/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pathlib
 import sys
 import time
 from typing import Annotated, Optional, Self, TypedDict
 
 import mylog
-
-# SPDX-License-Identifier: GPL-3.0-or-later
 import typer
 
 from . import __version__, logger
 from .config import (
     Config,
     Formatter,
     Linter,
@@ -308,9 +307,13 @@
     global SETTINGS  # noqa: PLW0603
     SETTINGS = _Settings(
         what_to_quiet=WhatToQuiet(commands=quiet_commands, pip=quiet_pip),
         config=config_,
     )
 
 
+def main() -> None:
+    return app()
+
+
 if __name__ == "__main__":
-    app()
+    main()
```

### Comparing `python-lemming-0.5.0/src/lemming/config.py` & `python-lemming-0.5.1/src/lemming/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,16 +299,16 @@
             ["packages", "command", "run_first"],
         )
         return cls(**dict_)
 
 
 class Config(ConfZ):
     # we should be safe with mutable default arguments
-    formatters: List[Formatter] = []
-    linters: List[Linter] = []
+    formatters: List[Formatter] = []  # noqa: RUF012
+    linters: List[Linter] = []  # noqa: RUF012
     # ^ also modify within read_config_file()
     fail_fast: bool = True
 
     def get_first_linters(self) -> List[Linter]:
         return [linter for linter in self.linters if linter.run_first]
 
     def get_other_linters(self) -> List[Linter]:
```

### Comparing `python-lemming-0.5.0/src/python_lemming.egg-info/PKG-INFO` & `python-lemming-0.5.1/src/python_lemming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
```

