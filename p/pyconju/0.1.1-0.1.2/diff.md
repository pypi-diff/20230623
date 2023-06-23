# Comparing `tmp/pyconju-0.1.1.tar.gz` & `tmp/pyconju-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconju-0.1.1.tar", last modified: Mon Jun 19 15:52:23 2023, max compression
+gzip compressed data, was "pyconju-0.1.2.tar", last modified: Fri Jun 23 11:10:32 2023, max compression
```

## Comparing `pyconju-0.1.1.tar` & `pyconju-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.317040 pyconju-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-06-14 08:43:06.000000 pyconju-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-14 11:07:36.000000 pyconju-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2944 2023-06-19 15:52:23.317112 pyconju-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-06-18 07:59:28.000000 pyconju-0.1.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-14 08:56:44.000000 pyconju-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1115 2023-06-19 15:52:23.325221 pyconju-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 15:52:22.709156 pyconju-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.061297 pyconju-0.1.1/src/pyconju/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:55:38.000000 pyconju-0.1.1/src/pyconju/__init__.py
--rw-rw-rw-   0        0        0      861 2023-06-19 14:06:37.000000 pyconju-0.1.1/src/pyconju/csv.py
--rw-rw-rw-   0        0        0      906 2023-06-19 14:01:42.000000 pyconju-0.1.1/src/pyconju/xls.py
--rw-rw-rw-   0        0        0      835 2023-06-19 14:07:21.000000 pyconju-0.1.1/src/pyconju/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.206245 pyconju-0.1.1/src/pyconju.egg-info/
--rw-rw-rw-   0        0        0     2944 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.306859 pyconju-0.1.1/test/
--rw-rw-rw-   0        0        0      225 2023-06-18 07:34:46.000000 pyconju-0.1.1/test/test_example.py
--rw-rw-rw-   0        0        0      224 2023-06-19 14:02:59.000000 pyconju-0.1.1/test/test_example2.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:10:32.932049 pyconju-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-14 08:43:06.000000 pyconju-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-14 11:07:36.000000 pyconju-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2932 2023-06-23 11:10:32.932049 pyconju-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-06-18 07:59:28.000000 pyconju-0.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-14 08:56:44.000000 pyconju-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1110 2023-06-23 11:10:32.948045 pyconju-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 11:10:32.660069 pyconju-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 11:10:32.740060 pyconju-0.1.2/src/pyconju/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:55:38.000000 pyconju-0.1.2/src/pyconju/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-06-19 14:06:37.000000 pyconju-0.1.2/src/pyconju/csv.py
+-rw-rw-rw-   0        0        0      906 2023-06-19 14:01:42.000000 pyconju-0.1.2/src/pyconju/xls.py
+-rw-rw-rw-   0        0        0      835 2023-06-19 14:07:21.000000 pyconju-0.1.2/src/pyconju/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:10:32.900049 pyconju-0.1.2/src/pyconju.egg-info/
+-rw-rw-rw-   0        0        0     2932 2023-06-23 11:10:32.000000 pyconju-0.1.2/src/pyconju.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-06-23 11:10:32.000000 pyconju-0.1.2/src/pyconju.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:10:32.000000 pyconju-0.1.2/src/pyconju.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-23 11:10:32.000000 pyconju-0.1.2/src/pyconju.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 11:10:32.000000 pyconju-0.1.2/src/pyconju.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 11:10:32.924052 pyconju-0.1.2/test/
+-rw-rw-rw-   0        0        0      225 2023-06-18 07:34:46.000000 pyconju-0.1.2/test/test_example.py
+-rw-rw-rw-   0        0        0      224 2023-06-19 14:02:59.000000 pyconju-0.1.2/test/test_example2.py
```

### Comparing `pyconju-0.1.1/LICENSE` & `pyconju-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.1/PKG-INFO` & `pyconju-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyconju
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for merging multiple files
 Home-page: https://github.com/dyagee/pyconju
-Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.2.tar.gz
 Author: Agee Aondo
 Author-email: ageeaondo45@gmail.com
 Project-URL: Bugs, https://github.com/dyagee/pyconju/issues
-Project-URL: Docs, https://github.com/dyagee/pyconju/README.md
+Project-URL: Docs, https://pyconju.readthedocs.io/
 Keywords: python3,excel,xls,csv,xlsx,merge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

### Comparing `pyconju-0.1.1/README.md` & `pyconju-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.1/setup.cfg` & `pyconju-0.1.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f6e 6a75 0d0a 7665 7273   = pyconju..vers
-00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
+00000020: 696f 6e20 3d20 302e 312e 320d 0a61 7574  ion = 0.1.2..aut
 00000030: 686f 7220 3d20 4167 6565 2041 6f6e 646f  hor = Agee Aondo
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2061 6765 6561 6f6e 646f 3435 4067 6d61   ageeaondo45@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5079 7468 6f6e 2070 6163  ion = Python pac
 00000080: 6b61 6765 2066 6f72 206d 6572 6769 6e67  kage for merging
 00000090: 206d 756c 7469 706c 6520 6669 6c65 730d   multiple files.
@@ -16,55 +16,55 @@
 000000f0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
 00000100: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7961  //github.com/dya
 00000110: 6765 652f 7079 636f 6e6a 750d 0a64 6f77  gee/pyconju..dow
 00000120: 6e6c 6f61 645f 7572 6c20 3d20 6874 7470  nload_url = http
 00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
 00000140: 7961 6765 652f 7079 636f 6e6a 752f 6172  yagee/pyconju/ar
 00000150: 6368 6976 652f 7265 6673 2f74 6167 732f  chive/refs/tags/
-00000160: 7630 2e31 2e31 2e74 6172 2e67 7a0d 0a6b  v0.1.1.tar.gz..k
+00000160: 7630 2e31 2e32 2e74 6172 2e67 7a0d 0a6b  v0.1.2.tar.gz..k
 00000170: 6579 776f 7264 7320 3d20 7079 7468 6f6e  eywords = python
 00000180: 332c 2065 7863 656c 2c20 786c 732c 2063  3, excel, xls, c
 00000190: 7376 2c20 786c 7378 2c20 6d65 7267 650d  sv, xlsx, merge.
 000001a0: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
 000001b0: 0d0a 0942 7567 7320 3d20 6874 7470 733a  ...Bugs = https:
 000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7961  //github.com/dya
 000001d0: 6765 652f 7079 636f 6e6a 752f 6973 7375  gee/pyconju/issu
 000001e0: 6573 0d0a 0944 6f63 7320 3d20 6874 7470  es...Docs = http
-000001f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00000200: 7961 6765 652f 7079 636f 6e6a 752f 5245  yagee/pyconju/RE
-00000210: 4144 4d45 2e6d 640d 0a63 6c61 7373 6966  ADME.md..classif
-00000220: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000230: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000240: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000250: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000260: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000270: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-00000280: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000290: 496e 6465 7065 6e64 656e 740d 0a09 4e61  Independent...Na
-000002a0: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-000002b0: 3a20 456e 676c 6973 680d 0a09 546f 7069  : English...Topi
-000002c0: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
-000002d0: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
-000002e0: 7261 7269 6573 203a 3a20 5079 7468 6f6e  raries :: Python
-000002f0: 204d 6f64 756c 6573 0d0a 0949 6e74 656e   Modules...Inten
-00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
-00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000340: 6368 0d0a 0949 6e74 656e 6465 6420 4175  ch...Intended Au
-00000350: 6469 656e 6365 203a 3a20 4f74 6865 7220  dience :: Other 
-00000360: 4175 6469 656e 6365 0d0a 0d0a 5b6f 7074  Audience....[opt
-00000370: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000380: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
-00000390: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000003a0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003b0: 203d 203e 3d33 2e37 0d0a 696e 636c 7564   = >=3.7..includ
-000003c0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-000003d0: 2054 7275 650d 0a69 6e73 7461 6c6c 5f72   True..install_r
-000003e0: 6571 7569 7265 7320 3d20 0d0a 0970 616e  equires = ...pan
-000003f0: 6461 730d 0a09 6f70 656e 7079 786c 0d0a  das...openpyxl..
-00000400: 0978 6c72 640d 0a0d 0a5b 6f70 7469 6f6e  .xlrd....[option
-00000410: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000420: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000430: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000440: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000450: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000001f0: 733a 2f2f 7079 636f 6e6a 752e 7265 6164  s://pyconju.read
+00000200: 7468 6564 6f63 732e 696f 2f0d 0a63 6c61  thedocs.io/..cla
+00000210: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000240: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
+00000250: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000260: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000270: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000280: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000290: 0a09 4e61 7475 7261 6c20 4c61 6e67 7561  ..Natural Langua
+000002a0: 6765 203a 3a20 456e 676c 6973 680d 0a09  ge :: English...
+000002b0: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+000002c0: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+000002d0: 204c 6962 7261 7269 6573 203a 3a20 5079   Libraries :: Py
+000002e0: 7468 6f6e 204d 6f64 756c 6573 0d0a 0949  thon Modules...I
+000002f0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000300: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+00000310: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000320: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+00000330: 7365 6172 6368 0d0a 0949 6e74 656e 6465  search...Intende
+00000340: 6420 4175 6469 656e 6365 203a 3a20 4f74  d Audience :: Ot
+00000350: 6865 7220 4175 6469 656e 6365 0d0a 0d0a  her Audience....
+00000360: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000370: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
+00000380: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
+00000390: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
+000003a0: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
+000003b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+000003c0: 7461 203d 2054 7275 650d 0a69 6e73 7461  ta = True..insta
+000003d0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+000003e0: 0970 616e 6461 730d 0a09 6f70 656e 7079  .pandas...openpy
+000003f0: 786c 0d0a 0978 6c72 643d 3d32 2e30 2e31  xl...xlrd==2.0.1
+00000400: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000410: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+00000420: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
+00000430: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000440: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000450: 2030 0d0a 0d0a                            0....
```

### Comparing `pyconju-0.1.1/src/pyconju/csv.py` & `pyconju-0.1.2/src/pyconju/csv.py`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.1/src/pyconju/xls.py` & `pyconju-0.1.2/src/pyconju/xls.py`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.1/src/pyconju/xlsx.py` & `pyconju-0.1.2/src/pyconju/xlsx.py`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.1/src/pyconju.egg-info/PKG-INFO` & `pyconju-0.1.2/src/pyconju.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyconju
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for merging multiple files
 Home-page: https://github.com/dyagee/pyconju
-Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.2.tar.gz
 Author: Agee Aondo
 Author-email: ageeaondo45@gmail.com
 Project-URL: Bugs, https://github.com/dyagee/pyconju/issues
-Project-URL: Docs, https://github.com/dyagee/pyconju/README.md
+Project-URL: Docs, https://pyconju.readthedocs.io/
 Keywords: python3,excel,xls,csv,xlsx,merge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

