# Comparing `tmp/temp_econdata-1.4.tar.gz` & `tmp/temp_econdata-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temp_econdata-1.4.tar", last modified: Thu Jun 22 21:50:26 2023, max compression
+gzip compressed data, was "temp_econdata-1.5.tar", last modified: Thu Jun 22 21:58:42 2023, max compression
```

## Comparing `temp_econdata-1.4.tar` & `temp_econdata-1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 21:50:26.262083 temp_econdata-1.4/
--rw-rw-rw-   0        0        0     2179 2023-06-22 21:50:26.261086 temp_econdata-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-06-22 21:31:54.000000 temp_econdata-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 21:50:26.262083 temp_econdata-1.4/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-06-22 21:50:13.000000 temp_econdata-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:50:26.244131 temp_econdata-1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 21:50:26.254105 temp_econdata-1.4/src/temp_econdata/
--rw-rw-rw-   0        0        0     6245 2023-06-22 21:50:03.000000 temp_econdata-1.4/src/temp_econdata/BCRP.py
--rw-rw-rw-   0        0        0     2826 2023-06-10 06:41:18.000000 temp_econdata-1.4/src/temp_econdata/BM.py
--rw-rw-rw-   0        0        0     4002 2023-06-10 06:41:18.000000 temp_econdata-1.4/src/temp_econdata/FRED.py
--rw-rw-rw-   0        0        0     2117 2023-06-10 07:31:38.000000 temp_econdata-1.4/src/temp_econdata/OECD.py
--rw-rw-rw-   0        0        0     3521 2023-06-22 21:32:54.000000 temp_econdata-1.4/src/temp_econdata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-06-10 06:41:18.000000 temp_econdata-1.4/src/temp_econdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:50:26.260089 temp_econdata-1.4/src/temp_econdata.egg-info/
--rw-rw-rw-   0        0        0     2179 2023-06-22 21:50:26.000000 temp_econdata-1.4/src/temp_econdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-06-22 21:50:26.000000 temp_econdata-1.4/src/temp_econdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 21:50:26.000000 temp_econdata-1.4/src/temp_econdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-22 21:50:26.000000 temp_econdata-1.4/src/temp_econdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-22 21:50:26.000000 temp_econdata-1.4/src/temp_econdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 21:58:42.188710 temp_econdata-1.5/
+-rw-rw-rw-   0        0        0     2179 2023-06-22 21:58:42.187713 temp_econdata-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1863 2023-06-22 21:31:54.000000 temp_econdata-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 21:58:42.188710 temp_econdata-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-06-22 21:58:14.000000 temp_econdata-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:58:42.170566 temp_econdata-1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 21:58:42.182070 temp_econdata-1.5/src/temp_econdata/
+-rw-rw-rw-   0        0        0     6249 2023-06-22 21:58:04.000000 temp_econdata-1.5/src/temp_econdata/BCRP.py
+-rw-rw-rw-   0        0        0     2826 2023-06-10 06:41:18.000000 temp_econdata-1.5/src/temp_econdata/BM.py
+-rw-rw-rw-   0        0        0     4002 2023-06-10 06:41:18.000000 temp_econdata-1.5/src/temp_econdata/FRED.py
+-rw-rw-rw-   0        0        0     2117 2023-06-10 07:31:38.000000 temp_econdata-1.5/src/temp_econdata/OECD.py
+-rw-rw-rw-   0        0        0     3521 2023-06-22 21:32:54.000000 temp_econdata-1.5/src/temp_econdata/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-06-10 06:41:18.000000 temp_econdata-1.5/src/temp_econdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:58:42.187713 temp_econdata-1.5/src/temp_econdata.egg-info/
+-rw-rw-rw-   0        0        0     2179 2023-06-22 21:58:42.000000 temp_econdata-1.5/src/temp_econdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-06-22 21:58:42.000000 temp_econdata-1.5/src/temp_econdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 21:58:42.000000 temp_econdata-1.5/src/temp_econdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 21:58:42.000000 temp_econdata-1.5/src/temp_econdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-22 21:58:42.000000 temp_econdata-1.5/src/temp_econdata.egg-info/top_level.txt
```

### Comparing `temp_econdata-1.4/PKG-INFO` & `temp_econdata-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temp_econdata
-Version: 1.4
+Version: 1.5
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `temp_econdata-1.4/README.md` & `temp_econdata-1.5/README.md`

 * *Files identical despite different names*

### Comparing `temp_econdata-1.4/setup.py` & `temp_econdata-1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='temp_econdata',
-    version = '1.4',
+    version = '1.5',
     author = 'Mauricio Alvarado, Andrei Romero',
     long_description = long_description,
     long_description_content_type='text/markdown',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
```

### Comparing `temp_econdata-1.4/src/temp_econdata/BCRP.py` & `temp_econdata-1.5/src/temp_econdata/BCRP.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     return df
 
 
 
 def metadatos():
 
-    metadatos = 'metadata/BCRPData-metadata.csv'
+    metadatos = r'../metadata/BCRPData-metadata.csv'
     df = pd.read_csv(metadatos, index_col=0, sep=";", encoding="latin-1").reset_index()
     df = df[['Código de serie', 'Grupo de serie', 'Nombre de serie', 'Frecuencia', 'Fecha de inicio', 'Fecha de fin']]
 
     return df
```

### Comparing `temp_econdata-1.4/src/temp_econdata/BM.py` & `temp_econdata-1.5/src/temp_econdata/BM.py`

 * *Files identical despite different names*

### Comparing `temp_econdata-1.4/src/temp_econdata/FRED.py` & `temp_econdata-1.5/src/temp_econdata/FRED.py`

 * *Files identical despite different names*

### Comparing `temp_econdata-1.4/src/temp_econdata/OECD.py` & `temp_econdata-1.5/src/temp_econdata/OECD.py`

 * *Files identical despite different names*

### Comparing `temp_econdata-1.4/src/temp_econdata/YFinance.py` & `temp_econdata-1.5/src/temp_econdata/YFinance.py`

 * *Files identical despite different names*

### Comparing `temp_econdata-1.4/src/temp_econdata.egg-info/PKG-INFO` & `temp_econdata-1.5/src/temp_econdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temp-econdata
-Version: 1.4
+Version: 1.5
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

