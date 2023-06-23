# Comparing `tmp/atlaspy-0.0.6.tar.gz` & `tmp/atlaspy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlaspy-0.0.6.tar", last modified: Fri Jun 23 00:39:55 2023, max compression
+gzip compressed data, was "atlaspy-0.0.7.tar", last modified: Fri Jun 23 00:52:25 2023, max compression
```

## Comparing `atlaspy-0.0.6.tar` & `atlaspy-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.885684 atlaspy-0.0.6/
--rw-r--r--   0 allucas    (501) staff       (20)       32 2023-06-23 00:09:29.000000 atlaspy-0.0.6/MANIFEST.in
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:39:55.885562 atlaspy-0.0.6/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.6/README.md
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882083 atlaspy-0.0.6/atlaspy/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.6/atlaspy/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    10569 2023-06-23 00:33:38.000000 atlaspy-0.0.6/atlaspy/core.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882722 atlaspy-0.0.6/atlaspy.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      449 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/top_level.txt
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 00:39:55.885722 atlaspy-0.0.6/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)     1846 2023-06-23 00:39:45.000000 atlaspy-0.0.6/setup.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882873 atlaspy-0.0.6/source_data/
--rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 00:34:34.000000 atlaspy-0.0.6/source_data/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.883019 atlaspy-0.0.6/source_data/atlases/
--rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 00:39:14.000000 atlaspy-0.0.6/source_data/atlases/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.884404 atlaspy-0.0.6/source_data/atlases/luts/
--rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/.DS_Store
--rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/aal.csv
--rw-r--r--   0 allucas    (501) staff       (20)     3133 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/dkt.csv
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.884803 atlaspy-0.0.6/source_data/atlases/niftis/
--rwxrwxr-x   0 allucas    (501) staff       (20)   342689 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/niftis/dkt.nii.gz
--rwxrwxr-x   0 allucas    (501) staff       (20)  1337896 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/niftis/vep.nii.gz
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.652444 atlaspy-0.0.7/
+-rw-r--r--   0 allucas    (501) staff       (20)       32 2023-06-23 00:09:29.000000 atlaspy-0.0.7/MANIFEST.in
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:52:25.652273 atlaspy-0.0.7/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.7/README.md
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.649252 atlaspy-0.0.7/atlaspy/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.7/atlaspy/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    10569 2023-06-23 00:33:38.000000 atlaspy-0.0.7/atlaspy/core.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.649891 atlaspy-0.0.7/atlaspy.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:52:25.000000 atlaspy-0.0.7/atlaspy.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      449 2023-06-23 00:52:25.000000 atlaspy-0.0.7/atlaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 00:52:25.000000 atlaspy-0.0.7/atlaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-23 00:52:25.000000 atlaspy-0.0.7/atlaspy.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 00:52:25.000000 atlaspy-0.0.7/atlaspy.egg-info/top_level.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 00:52:25.652486 atlaspy-0.0.7/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)     1846 2023-06-23 00:51:51.000000 atlaspy-0.0.7/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.650010 atlaspy-0.0.7/source_data/
+-rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 00:34:34.000000 atlaspy-0.0.7/source_data/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.650130 atlaspy-0.0.7/source_data/atlases/
+-rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 00:52:08.000000 atlaspy-0.0.7/source_data/atlases/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.650877 atlaspy-0.0.7/source_data/atlases/luts/
+-rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.7/source_data/atlases/luts/.DS_Store
+-rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.7/source_data/atlases/luts/aal.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     3133 2023-06-22 23:19:38.000000 atlaspy-0.0.7/source_data/atlases/luts/dkt.csv
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:52:25.651394 atlaspy-0.0.7/source_data/atlases/niftis/
+-rwxrwxr-x   0 allucas    (501) staff       (20)   342689 2023-06-22 23:19:38.000000 atlaspy-0.0.7/source_data/atlases/niftis/dkt.nii.gz
+-rwxrwxr-x   0 allucas    (501) staff       (20)  1337896 2023-06-22 23:19:38.000000 atlaspy-0.0.7/source_data/atlases/niftis/vep.nii.gz
```

### Comparing `atlaspy-0.0.6/atlaspy/core.py` & `atlaspy-0.0.7/atlaspy/core.py`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/setup.py` & `atlaspy-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def __init__(self, *args, **kwargs):
         print('Downloading required files')
         super().__init__(*args, **kwargs)
         atexit.register(download_files)
 
 setup(
     name='atlaspy',
-    version='0.0.6',
+    version='0.0.7',
     description='Python library for working with brain atlases',
     author='Alfredo Lucas',
     author_email='alfredo1238@gmail.com',
     packages=find_packages(),
     package_data={'atlaspy': ["source_data/*"]},
     include_package_data=True,
     install_requires=['pyvista', 'seaborn', 'pandas', 'matplotlib', 'nibabel'],
```

### Comparing `atlaspy-0.0.6/source_data/.DS_Store` & `atlaspy-0.0.7/source_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/source_data/atlases/.DS_Store` & `atlaspy-0.0.7/source_data/atlases/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
 00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0016  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 000f  ................
 00000050: 0000 0001 0000 1000 6277 7370 626c 6f62  ........bwspblob
 00000060: 0000 00b8 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0016 0000 0004  ................
+00001000: 0000 0000 0000 0000 0000 000f 0000 0004  ................
 00001010: 006c 0075 0074 0073 6277 7370 626c 6f62  .l.u.t.sbwspblob
 00001020: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00001030: 0405 0607 0808 080b 085d 5368 6f77 5374  .........]ShowSt
 00001040: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00001050: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001060: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00001070: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
@@ -389,39 +389,39 @@
 00001840: 0066 0074 0069 0073 6d6f 4444 626c 6f62  .f.t.i.smoDDblob
 00001850: 0000 0008 94d2 3e45 8722 c541 0000 0006  ......>E.".A....
 00001860: 006e 0069 0066 0074 0069 0073 6d6f 6444  .n.i.f.t.i.smodD
 00001870: 626c 6f62 0000 0008 94d2 3e45 8722 c541  blob......>E.".A
 00001880: 0000 0006 006e 0069 0066 0074 0069 0073  .....n.i.f.t.i.s
 00001890: 7068 3153 636f 6d70 0000 0000 0019 b000  ph1Scomp........
 000018a0: 0000 0006 006e 0069 0066 0074 0069 0073  .....n.i.f.t.i.s
-000018b0: 7653 726e 6c6f 6e67 0000 0001 0000 0004  vSrnlong........
-000018c0: 0073 0074 006c 0073 6277 7370 626c 6f62  .s.t.l.sbwspblob
-000018d0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-000018e0: 0405 0607 0808 080b 085d 5368 6f77 5374  .........]ShowSt
-000018f0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00001900: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00001910: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00001920: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00001930: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001940: 0909 095f 1018 7b7b 3435 352c 2034 3632  ..._..{{455, 462
-00001950: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
-00001960: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00001970: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00001980: 0000 0000 0000 0000 0000 008b 0000 0004  ................
-00001990: 0073 0074 006c 0073 6473 636c 626f 6f6c  .s.t.l.sdsclbool
-000019a0: 0000 0000 0400 7300 7400 6c00 736c 6731  ......s.t.l.slg1
-000019b0: 5363 6f6d 7000 0000 003a ed8b 7000 0000  Scomp....:..p...
-000019c0: 0400 7300 7400 6c00 736d 6f44 4462 6c6f  ..s.t.l.smoDDblo
-000019d0: 6200 0000 08fd 4c00 4687 22c5 4100 0000  b.....L.F.".A...
-000019e0: 0400 7300 7400 6c00 736d 6f64 4462 6c6f  ..s.t.l.smodDblo
-000019f0: 6200 0000 08fd 4c00 4687 22c5 4100 0000  b.....L.F.".A...
-00001a00: 0400 7300 7400 6c00 7370 6831 5363 6f6d  ..s.t.l.sph1Scom
-00001a10: 7000 0000 003b 08e0 0000 0000 0400 7300  p....;........s.
-00001a20: 7400 6c00 7376 5372 6e6c 6f6e 6700 0000  t.l.svSrnlong...
-00001a30: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+000018b0: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
+000018c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `atlaspy-0.0.6/source_data/atlases/luts/.DS_Store` & `atlaspy-0.0.7/source_data/atlases/luts/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/source_data/atlases/luts/aal.csv` & `atlaspy-0.0.7/source_data/atlases/luts/aal.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/source_data/atlases/luts/dkt.csv` & `atlaspy-0.0.7/source_data/atlases/luts/dkt.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/source_data/atlases/niftis/dkt.nii.gz` & `atlaspy-0.0.7/source_data/atlases/niftis/dkt.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.6/source_data/atlases/niftis/vep.nii.gz` & `atlaspy-0.0.7/source_data/atlases/niftis/vep.nii.gz`

 * *Files identical despite different names*

