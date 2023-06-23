# Comparing `tmp/atlaspy-0.0.5.tar.gz` & `tmp/atlaspy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlaspy-0.0.5.tar", last modified: Fri Jun 23 00:35:41 2023, max compression
+gzip compressed data, was "atlaspy-0.0.6.tar", last modified: Fri Jun 23 00:39:55 2023, max compression
```

## Comparing `atlaspy-0.0.5.tar` & `atlaspy-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.409739 atlaspy-0.0.5/
--rw-r--r--   0 allucas    (501) staff       (20)       32 2023-06-23 00:09:29.000000 atlaspy-0.0.5/MANIFEST.in
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:35:41.409586 atlaspy-0.0.5/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.5/README.md
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.406819 atlaspy-0.0.5/atlaspy/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.5/atlaspy/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    10569 2023-06-23 00:33:38.000000 atlaspy-0.0.5/atlaspy/core.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.407476 atlaspy-0.0.5/atlaspy.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:35:41.000000 atlaspy-0.0.5/atlaspy.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      484 2023-06-23 00:35:41.000000 atlaspy-0.0.5/atlaspy.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 00:35:41.000000 atlaspy-0.0.5/atlaspy.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-23 00:35:41.000000 atlaspy-0.0.5/atlaspy.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 00:35:41.000000 atlaspy-0.0.5/atlaspy.egg-info/top_level.txt
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 00:35:41.409783 atlaspy-0.0.5/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)     1772 2023-06-23 00:35:31.000000 atlaspy-0.0.5/setup.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.407595 atlaspy-0.0.5/source_data/
--rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 00:34:34.000000 atlaspy-0.0.5/source_data/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.407714 atlaspy-0.0.5/source_data/atlases/
--rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 00:34:34.000000 atlaspy-0.0.5/source_data/atlases/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.408098 atlaspy-0.0.5/source_data/atlases/luts/
--rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.5/source_data/atlases/luts/.DS_Store
--rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.5/source_data/atlases/luts/aal.csv
--rw-r--r--   0 allucas    (501) staff       (20)     3133 2023-06-22 23:19:38.000000 atlaspy-0.0.5/source_data/atlases/luts/dkt.csv
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.408528 atlaspy-0.0.5/source_data/atlases/niftis/
--rwxrwxr-x   0 allucas    (501) staff       (20)   342689 2023-06-22 23:19:38.000000 atlaspy-0.0.5/source_data/atlases/niftis/dkt.nii.gz
--rwxrwxr-x   0 allucas    (501) staff       (20)  1337896 2023-06-22 23:19:38.000000 atlaspy-0.0.5/source_data/atlases/niftis/vep.nii.gz
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:35:41.409381 atlaspy-0.0.5/source_data/atlases/stls/
--rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 00:16:11.000000 atlaspy-0.0.5/source_data/atlases/stls/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.885684 atlaspy-0.0.6/
+-rw-r--r--   0 allucas    (501) staff       (20)       32 2023-06-23 00:09:29.000000 atlaspy-0.0.6/MANIFEST.in
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:39:55.885562 atlaspy-0.0.6/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.6/README.md
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882083 atlaspy-0.0.6/atlaspy/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.6/atlaspy/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    10569 2023-06-23 00:33:38.000000 atlaspy-0.0.6/atlaspy/core.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882722 atlaspy-0.0.6/atlaspy.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      449 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 00:39:55.000000 atlaspy-0.0.6/atlaspy.egg-info/top_level.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 00:39:55.885722 atlaspy-0.0.6/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)     1846 2023-06-23 00:39:45.000000 atlaspy-0.0.6/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.882873 atlaspy-0.0.6/source_data/
+-rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 00:34:34.000000 atlaspy-0.0.6/source_data/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.883019 atlaspy-0.0.6/source_data/atlases/
+-rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 00:39:14.000000 atlaspy-0.0.6/source_data/atlases/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.884404 atlaspy-0.0.6/source_data/atlases/luts/
+-rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/.DS_Store
+-rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/aal.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     3133 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/luts/dkt.csv
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 00:39:55.884803 atlaspy-0.0.6/source_data/atlases/niftis/
+-rwxrwxr-x   0 allucas    (501) staff       (20)   342689 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/niftis/dkt.nii.gz
+-rwxrwxr-x   0 allucas    (501) staff       (20)  1337896 2023-06-22 23:19:38.000000 atlaspy-0.0.6/source_data/atlases/niftis/vep.nii.gz
```

### Comparing `atlaspy-0.0.5/atlaspy/core.py` & `atlaspy-0.0.6/atlaspy/core.py`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/setup.py` & `atlaspy-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import atexit
 
 def download_files():
     # Define the URL from which to download the files
     zip_url = 'http://dl.dropboxusercontent.com/scl/fi/s88fszf6t1q6ef4znl6cr/stls.zip?dl=0&rlkey=j93ehij42d3g0rp1hqn9u0f5t'
 
     # Create the target directory if it doesn't exist
-    stl_dir = os.path.join(os.path.dirname(__file__), 'source_data/atlases/stls')
+    stl_dir = os.path.join(os.path.dirname(os.path.abspath(__name__)), 'source_data/atlases/')
     os.makedirs(stl_dir, exist_ok=True)
 
     # Download the ZIP file
     zip_path = os.path.join(stl_dir, 'stls.zip')
     response = requests.get(zip_url)
     with open(zip_path, 'wb') as file:
         file.write(response.content)
@@ -31,21 +31,24 @@
     def __init__(self, *args, **kwargs):
         print('Downloading required files')
         super().__init__(*args, **kwargs)
         atexit.register(download_files)
 
 setup(
     name='atlaspy',
-    version='0.0.5',
+    version='0.0.6',
     description='Python library for working with brain atlases',
     author='Alfredo Lucas',
     author_email='alfredo1238@gmail.com',
     packages=find_packages(),
     package_data={'atlaspy': ["source_data/*"]},
     include_package_data=True,
     install_requires=['pyvista', 'seaborn', 'pandas', 'matplotlib', 'nibabel'],
+    cmdclass={
+        'install': PostInstallCommand,
+    },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

### Comparing `atlaspy-0.0.5/source_data/.DS_Store` & `atlaspy-0.0.6/source_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/source_data/atlases/.DS_Store` & `atlaspy-0.0.6/source_data/atlases/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 00001930: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
 00001940: 0909 095f 1018 7b7b 3435 352c 2034 3632  ..._..{{455, 462
 00001950: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
 00001960: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 00001970: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 008b 0000 0004  ................
 00001990: 0073 0074 006c 0073 6473 636c 626f 6f6c  .s.t.l.sdsclbool
-000019a0: 0100 0000 0400 7300 7400 6c00 736c 6731  ......s.t.l.slg1
+000019a0: 0000 0000 0400 7300 7400 6c00 736c 6731  ......s.t.l.slg1
 000019b0: 5363 6f6d 7000 0000 003a ed8b 7000 0000  Scomp....:..p...
 000019c0: 0400 7300 7400 6c00 736d 6f44 4462 6c6f  ..s.t.l.smoDDblo
 000019d0: 6200 0000 08fd 4c00 4687 22c5 4100 0000  b.....L.F.".A...
 000019e0: 0400 7300 7400 6c00 736d 6f64 4462 6c6f  ..s.t.l.smodDblo
 000019f0: 6200 0000 08fd 4c00 4687 22c5 4100 0000  b.....L.F.".A...
 00001a00: 0400 7300 7400 6c00 7370 6831 5363 6f6d  ..s.t.l.sph1Scom
 00001a10: 7000 0000 003b 08e0 0000 0000 0400 7300  p....;........s.
```

### Comparing `atlaspy-0.0.5/source_data/atlases/luts/.DS_Store` & `atlaspy-0.0.6/source_data/atlases/luts/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/source_data/atlases/luts/aal.csv` & `atlaspy-0.0.6/source_data/atlases/luts/aal.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/source_data/atlases/luts/dkt.csv` & `atlaspy-0.0.6/source_data/atlases/luts/dkt.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/source_data/atlases/niftis/dkt.nii.gz` & `atlaspy-0.0.6/source_data/atlases/niftis/dkt.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.5/source_data/atlases/niftis/vep.nii.gz` & `atlaspy-0.0.6/source_data/atlases/niftis/vep.nii.gz`

 * *Files identical despite different names*

