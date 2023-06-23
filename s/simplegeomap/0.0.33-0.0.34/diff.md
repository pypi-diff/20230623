# Comparing `tmp/simplegeomap-0.0.33.tar.gz` & `tmp/simplegeomap-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.33.tar", last modified: Wed Jun 21 11:08:01 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.34.tar", last modified: Fri Jun 23 07:54:18 2023, max compression
```

## Comparing `simplegeomap-0.0.33.tar` & `simplegeomap-0.0.34.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.33/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.33/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     7137 2023-06-21 11:03:52.000000 simplegeomap-0.0.33/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     7598 2023-06-21 10:06:04.000000 simplegeomap-0.0.33/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-21 08:57:01.000000 simplegeomap-0.0.33/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.34/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.34/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7137 2023-06-23 07:43:24.000000 simplegeomap-0.0.34/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7636 2023-06-23 07:44:48.000000 simplegeomap-0.0.34/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-23 07:53:19.000000 simplegeomap-0.0.34/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-23 07:54:18.000000 simplegeomap-0.0.34/setup.cfg
```

### Comparing `simplegeomap-0.0.33/PKG-INFO` & `simplegeomap-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.33
+Version: 0.0.34
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.33/README.md` & `simplegeomap-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.33/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.34/simplegeomap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.33
+Version: 0.0.34
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.33/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.34/simplegeomap/simplegeomap.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.33/simplegeomap/util.py` & `simplegeomap-0.0.34/simplegeomap/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,19 @@
     return np.einsum('ij,ijkl->kl', ftr, sub_image)
     
 def cdist(p1,p2):    
     distances = np.linalg.norm(p1 - p2, axis=1)
     return distances
 
 class QuadTreeInterpolator:
+    #def __init__(self):
     def __init__(self):
         self.tree = quads.QuadTree((0,0), 500, 500)
 
-    def append(self, x, y, z):        
+    def append(self, x, y, z):
         for xx,yy,zz in zip(x,y,z):
             self.tree.insert((xx,yy),data=zz)
 
     def interp_cell(self, x, y, points):
         a = np.array([x,y]).reshape(-1,2)
         b = np.array(points)[:,:2]
         ds = cdist(a,b)
@@ -159,16 +160,17 @@
     clats = list(clats)
     clons = list(clons)
     print ('clat clons',clats,clons)
     skip = np.min([len(clats),len(clons)])
     lat_min, lat_max, lon_min, lon_max, elev_min, elev_max, cols, rows = gltiles[tile]    
     lon = lon_min + 1/120*np.arange(cols)
     lat = lat_max - 1/120*np.arange(rows)
-    d = [[x,y,zm[i,j]] for i,y in enumerate(lat) for j,x in enumerate(lon) if j%skip==0 and int(y) in clats and int(x) in clons]
+    d = [[x,y,zm[i,j]] for i,y in enumerate(lat) for j,x in enumerate(lon) if i%skip==0 and int(y) in clats and int(x) in clons]
     d = np.array(d)
+    d = d[d[:,2]>-1]
     print ('d',d.shape)
     q = QuadTreeInterpolator()
     q.append(d[:,0],d[:,1],d[:,2])
     return q
 
 def test1():
     x = np.array(list(range(4,10)))
```

### Comparing `simplegeomap-0.0.33/setup.py` & `simplegeomap-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.33',
+    version='0.0.34',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

