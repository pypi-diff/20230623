# Comparing `tmp/SparkMinIOHandle-0.0.4.tar.gz` & `tmp/SparkMinIOHandle-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkMinIOHandle-0.0.4.tar", last modified: Thu Jun 22 14:50:46 2023, max compression
+gzip compressed data, was "SparkMinIOHandle-0.0.5.tar", last modified: Fri Jun 23 16:46:28 2023, max compression
```

## Comparing `SparkMinIOHandle-0.0.4.tar` & `SparkMinIOHandle-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 14:50:46.199660 SparkMinIOHandle-0.0.4/
--rw-rw-rw-   0        0        0      653 2023-06-22 14:50:46.188661 SparkMinIOHandle-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 14:50:46.180659 SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/
--rw-rw-rw-   0        0        0      653 2023-06-22 14:50:45.000000 SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-22 14:50:45.000000 SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 14:50:45.000000 SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 14:50:45.000000 SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 14:50:46.200662 SparkMinIOHandle-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-06-22 14:50:37.000000 SparkMinIOHandle-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 14:50:46.187658 SparkMinIOHandle-0.0.4/sparkminiohandler/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.4/sparkminiohandler/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-06-22 14:48:20.000000 SparkMinIOHandle-0.0.4/sparkminiohandler/sparkminiohandler.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.175163 SparkMinIOHandle-0.0.5/
+-rw-rw-rw-   0        0        0      653 2023-06-23 16:46:28.173165 SparkMinIOHandle-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.157169 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 16:46:28.175163 SparkMinIOHandle-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2023-06-23 16:46:20.000000 SparkMinIOHandle-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.171166 SparkMinIOHandle-0.0.5/sparkminiohandler/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.5/sparkminiohandler/__init__.py
+-rw-rw-rw-   0        0        0     2032 2023-06-23 16:46:05.000000 SparkMinIOHandle-0.0.5/sparkminiohandler/sparkminiohandler.py
```

### Comparing `SparkMinIOHandle-0.0.4/PKG-INFO` & `SparkMinIOHandle-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkMinIOHandle
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
 Keywords: python,minio,spark
 Platform: UNKNOWN
```

### Comparing `SparkMinIOHandle-0.0.4/SparkMinIOHandle.egg-info/PKG-INFO` & `SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkMinIOHandle
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
 Keywords: python,minio,spark
 Platform: UNKNOWN
```

### Comparing `SparkMinIOHandle-0.0.4/setup.py` & `SparkMinIOHandle-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Spark MinIO Handler Package'
 LONG_DESCRIPTION = 'Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="SparkMinIOHandle",
```

### Comparing `SparkMinIOHandle-0.0.4/sparkminiohandler/sparkminiohandler.py` & `SparkMinIOHandle-0.0.5/sparkminiohandler/sparkminiohandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.spark_context = spark_context 
 
 
     def get_recent_table(self, tablename: str):
         # Padrão de nome dos arquivos
         
         # Obter lista de arquivos correspondentes ao padrão
-        arquivos =  [object.object_name for object in self.client_minio.list_objects(self.bucket_name) if tablename in object.object_name]
+        arquivos =  [object.object_name for object in self.client_minio.list_objects(self.bucket_name) if f'{tablename}_' in object.object_name]
         
         # Função para extrair a data do nome do arquivo
         def extrair_data(nome_arquivo):
             # O formato do nome do arquivo é NOME_YYYY-MM-DD.json
             data_str = nome_arquivo.split('_')[1].split('.')[0]
             data = datetime.strptime(data_str, '%Y-%m-%d')
             return data
```

