# Comparing `tmp/iosense_connect-4.0.3.tar.gz` & `tmp/iosense_connect-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-4.0.3.tar", last modified: Mon Jun 19 07:39:28 2023, max compression
+gzip compressed data, was "dist\iosense_connect-4.0.4.tar", last modified: Fri Jun 23 13:49:07 2023, max compression
```

## Comparing `iosense_connect-4.0.3.tar` & `iosense_connect-4.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.256207 iosense_connect-4.0.3/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-19 07:39:28.255022 iosense_connect-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.201719 iosense_connect-4.0.3/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.3/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    28130 2023-06-19 07:39:22.000000 iosense_connect-4.0.3/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:39:28.250216 iosense_connect-4.0.3/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-19 07:39:28.000000 iosense_connect-4.0.3/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-19 07:39:27.000000 iosense_connect-4.0.3/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 07:39:28.256207 iosense_connect-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-06-19 07:39:22.000000 iosense_connect-4.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.504855 iosense_connect-4.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-23 13:49:07.498490 iosense_connect-4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.232468 iosense_connect-4.0.4/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.4/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    28183 2023-06-23 13:46:36.000000 iosense_connect-4.0.4/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.430477 iosense_connect-4.0.4/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      262 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:49:07.507918 iosense_connect-4.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-06-23 13:44:34.000000 iosense_connect-4.0.4/setup.py
```

### Comparing `iosense_connect-4.0.3/LICENSE.txt` & `iosense_connect-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.3/PKG-INFO` & `iosense_connect-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 4.0.3
+Version: 4.0.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.3/README.md` & `iosense_connect-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.3/iosense_connect/data_access.py` & `iosense_connect-4.0.4/iosense_connect/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,31 +47,30 @@
         if len(metadata) == 0:
             metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
         data = metadata['params']
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             df_meta = pd.DataFrame(data[str(value1)])
             df_meta = df_meta.set_index('paramName').transpose()
-
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 m = float(df_meta.iloc[0]['m'])
-                c = int(str(df_meta.iloc[0]['c']).replace(',', ''))
-
+                c = float(str(df_meta.iloc[0]['c']).replace(',', ''))
                 df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
                     'BAD undefined', '-99999').replace('BAD 0', '-99999').replace('true', True).replace('false', False)
-
                 df[str(value2)] = df[str(value2)].astype('float')
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
-                    min_value = int(df_meta.iloc[0]['min'])
+                    min_value = float(df_meta.iloc[0]['min'])
                     df[str(value2)] = np.where(df[str(value2)] <= min_value, min_value, df[str(value2)])
                 if 'max' in df_meta.columns:
-                    max_value = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
-                        '1000000000000000000000000000', '99999').replace('100000000000', '99999'))
+                    max_value_str = str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
+                        '1000000000000000000000000000', '99999').replace('100000000000', '99999')
+                    max_value = float(max_value_str)
                     df[str(value2)] = np.where(df[str(value2)] >= max_value, max_value, df[str(value2)])
+
         return df
 
     def get_device_metadata(self, device_id, onpremise=False):
         """
 
         :param onpremise:
         :param device_id: string
```

### Comparing `iosense_connect-4.0.3/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-4.0.4/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 4.0.3
+Version: 4.0.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.3/setup.py` & `iosense_connect-4.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "4.0.3",
+    version = "4.0.4",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
         'cryptography>=41.0',
         'fsspec>=2023.6',
         'numpy>=1.24',
         'pandas>=2.0',
         'python_dateutil>=2.8',
         'Requests>=2.31',
         'urllib3>=1.26',
-        'pyarrow>=12.0',
+        'pyarrow',
         'azure-storage-blob>=12.16',
         'adlfs>=2023.4',
         'azure-core>=1.27',
         'azure-datalake-store>=0.0',
         'azure-identity>=1.13',
         'botocore>=1.29',
         'gcsfs>=2023.6',
```

