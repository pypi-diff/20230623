# Comparing `tmp/PowDevLif-0.0.2.tar.gz` & `tmp/PowDevLif-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDevLif-0.0.2.tar", last modified: Fri Jun 23 10:54:43 2023, max compression
+gzip compressed data, was "PowDevLif-0.0.3.tar", last modified: Fri Jun 23 11:03:48 2023, max compression
```

## Comparing `PowDevLif-0.0.2.tar` & `PowDevLif-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.2/README.md
--rw-------   0 runner    (1000) runner    (1000)      451 2023-06-23 10:54:33.000000 PowDevLif-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1072 2023-06-23 10:54:30.000000 PowDevLif-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.251475 PowDevLif-0.0.2/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.255475 PowDevLif-0.0.2/src/PowDevLif.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/src/powdevlif/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/src/powdevlif/function/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/counters.py
--rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/cumul_endommagement.py
--rw-------   0 runner    (1000) runner    (1000)     3275 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/graphs.py
--rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/losses.py
--rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/materials.py
--rw-------   0 runner    (1000) runner    (1000)     2782 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/matrix.py
--rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/path_reader.py
--rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/poly_somme.py
--rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/temperature.py
--rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/zth_materials.py
--rw-------   0 runner    (1000) runner    (1000)     3221 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/lifetime.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.3/README.md
+-rw-------   0 runner    (1000) runner    (1000)      451 2023-06-23 11:03:40.000000 PowDevLif-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1072 2023-06-23 11:03:35.000000 PowDevLif-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.494956 PowDevLif-0.0.3/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.498957 PowDevLif-0.0.3/src/PowDevLif.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-23 11:03:48.000000 PowDevLif-0.0.3/src/PowDevLif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.498957 PowDevLif-0.0.3/src/powdevlif/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 11:03:48.510956 PowDevLif-0.0.3/src/powdevlif/function/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/counters.py
+-rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/cumul_endommagement.py
+-rw-------   0 runner    (1000) runner    (1000)     3275 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/graphs.py
+-rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/losses.py
+-rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/materials.py
+-rw-------   0 runner    (1000) runner    (1000)     2788 2023-06-23 11:03:20.000000 PowDevLif-0.0.3/src/powdevlif/function/matrix.py
+-rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/path_reader.py
+-rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.3/src/powdevlif/function/poly_somme.py
+-rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/temperature.py
+-rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/function/zth_materials.py
+-rw-------   0 runner    (1000) runner    (1000)     3221 2023-06-23 10:54:01.000000 PowDevLif-0.0.3/src/powdevlif/lifetime.py
```

### Comparing `PowDevLif-0.0.2/LICENSE` & `PowDevLif-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/PKG-INFO` & `PowDevLif-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.2
+Version: 0.0.3
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.2/README.md` & `PowDevLif-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/setup.py` & `PowDevLif-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='PowDevLif',
-    version='0.0.2',
+    version='0.0.3',
     description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)',
     readme='README.md',
     license='MIT',
     author='Garnier Paul, Baudais Briac',
     author_email='paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages('src'),
```

### Comparing `PowDevLif-0.0.2/src/PowDevLif.egg-info/PKG-INFO` & `PowDevLif-0.0.3/src/PowDevLif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.2
+Version: 0.0.3
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.2/src/PowDevLif.egg-info/SOURCES.txt` & `PowDevLif-0.0.3/src/PowDevLif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/counters.py` & `PowDevLif-0.0.3/src/powdevlif/function/counters.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/cumul_endommagement.py` & `PowDevLif-0.0.3/src/powdevlif/function/cumul_endommagement.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/graphs.py` & `PowDevLif-0.0.3/src/powdevlif/function/graphs.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/losses.py` & `PowDevLif-0.0.3/src/powdevlif/function/losses.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/matrix.py` & `PowDevLif-0.0.3/src/powdevlif/function/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 
     matrix_1, mean_bins_1, range_bins_1 = create_quantized_rainflow_matrix(counter_IGBT)
     matrix_2, mean_bins_2, range_bins_2 = create_quantized_rainflow_matrix(counter_diode)
 
     # Create a new figure with two subplots
     fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(12, 6))
     ax = axes[0]
-    im = ax.imshow(matrix_1, cmap='hot', interpolation='nearest')
+    im = ax.imshow(matrix_1, cmap='plasma', interpolation='nearest')
     ax.set_title('IGBT')
     ax.set_xlabel('Delta T')
     ax.set_ylabel('Mean Tj')
     fig.colorbar(im, ax=ax, label='Count')
     ax.set_xticks(np.arange(len(range_bins_1)))
     ax.set_yticks(np.arange(len(mean_bins_1)))
     ax.set_xticklabels([str(int(val)) for val in range_bins_1])
     ax.set_yticklabels([str(int(val)) for val in mean_bins_1])
 
     # Plot the second matrix
     ax = axes[1]
-    im = ax.imshow(matrix_2, cmap='hot', interpolation='nearest')
+    im = ax.imshow(matrix_2, cmap='plasma', interpolation='nearest')
     ax.set_title('Diode')
     ax.set_xlabel('Delta T')
     ax.set_ylabel('Mean Tj')
     fig.colorbar(im, ax=ax, label='Count')
     ax.set_xticks(np.arange(len(range_bins_2)))
     ax.set_yticks(np.arange(len(mean_bins_2)))
     ax.set_xticklabels([str(int(val)) for val in range_bins_2])
```

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/poly_somme.py` & `PowDevLif-0.0.3/src/powdevlif/function/poly_somme.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/temperature.py` & `PowDevLif-0.0.3/src/powdevlif/function/temperature.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/function/zth_materials.py` & `PowDevLif-0.0.3/src/powdevlif/function/zth_materials.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.2/src/powdevlif/lifetime.py` & `PowDevLif-0.0.3/src/powdevlif/lifetime.py`

 * *Files identical despite different names*

