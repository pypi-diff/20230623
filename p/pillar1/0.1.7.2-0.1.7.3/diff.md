# Comparing `tmp/pillar1-0.1.7.2.tar.gz` & `tmp/pillar1-0.1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.2.tar", last modified: Fri Jun 23 14:40:55 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.3.tar", last modified: Fri Jun 23 14:48:26 2023, max compression
```

## Comparing `pillar1-0.1.7.2.tar` & `pillar1-0.1.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:40:55.239825 pillar1-0.1.7.2/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:40:55.239717 pillar1-0.1.7.2/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.2/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:40:55.238985 pillar1-0.1.7.2/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.2/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     7776 2023-06-23 14:40:51.000000 pillar1-0.1.7.2/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.2/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.2/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:40:55.239536 pillar1-0.1.7.2/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:40:55.000000 pillar1-0.1.7.2/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 14:40:55.000000 pillar1-0.1.7.2/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 14:40:55.000000 pillar1-0.1.7.2/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 14:40:55.000000 pillar1-0.1.7.2/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 14:40:55.239864 pillar1-0.1.7.2/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 14:39:50.000000 pillar1-0.1.7.2/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:48:26.172301 pillar1-0.1.7.3/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:48:26.172171 pillar1-0.1.7.3/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.3/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:48:26.171266 pillar1-0.1.7.3/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.3/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6423 2023-06-23 14:48:16.000000 pillar1-0.1.7.3/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.3/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.3/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:48:26.171975 pillar1-0.1.7.3/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:48:26.000000 pillar1-0.1.7.3/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 14:48:26.000000 pillar1-0.1.7.3/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 14:48:26.000000 pillar1-0.1.7.3/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 14:48:26.000000 pillar1-0.1.7.3/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 14:48:26.172340 pillar1-0.1.7.3/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 14:48:22.000000 pillar1-0.1.7.3/setup.py
```

### Comparing `pillar1-0.1.7.2/PKG-INFO` & `pillar1-0.1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.2/README.md` & `pillar1-0.1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.2/pillar1/constants.py` & `pillar1-0.1.7.3/pillar1/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -196,63 +196,13 @@
 scd_key,int,
 record_effective_datetime,timestamp,
 record_end_datetime,timestamp,
 record_create_datetime,timestamp,
 record_update_datetime,timestamp,
 recent_record_flag,string,
 drg_grouper_review_code,string,
-admitting_full_name,string,
-admitting_first_name,string,
-admitting_last_name,string,
-admitting_middle_name,string,
-admitting_group_name,string,
-admitting_tin,int,
-admitting_npi,bigint,
-admitting_group_id,int,
-admitting_id_code_type,string,
-admitting_id_code_desc,string,
-attending_full_name,string,
-attending_first_name,string,
-attending_last_name,string,
-attending_middle_name,string,
-attending_group_name,string,
-attending_tin,int,
-attending_npi,bigint,
-attending_group_id,int,
-attending_id_code_type,string,
-attending_id_code_desc,string,
-billing_full_name,string,
-billing_first_name,string,
-billing_last_name,string,
-billing_middle_name,string,
-billing_group_name,string,
-billing_tin,int,
-billing_npi,bigint,
-billing_group_id,string,
-billing_id_code_type,string,
-billing_id_code_desc,string,
-ordering_full_name,string,
-ordering_first_name,string,
-ordering_last_name,string,
-ordering_middle_name,string,
-ordering_group_name,string,
-ordering_tin,int,
-ordering_npi,bigint,
-ordering_group_id,string,
-ordering_id_code_type,string,
-ordering_id_code_desc,string,
-prescribing_full_name,string,
-prescribing_first_name,string,
-prescribing_last_name,string,
-prescribing_middle_name,string,
-prescribing_group_name,string,
-prescribing_tin,int,
-prescribing_npi,bigint,
-prescribing_group_id,string,
-prescribing_id_code_type,string,
-prescribing_id_code_desc,string
 
 """
 
 STARCODER_BETA += """
 when answering the request use the information listed above only, do not make up column names and do not place additional conditions
     """
```

### Comparing `pillar1-0.1.7.2/pillar1/constants_original.py` & `pillar1-0.1.7.3/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.2/pillar1/pillar1.py` & `pillar1-0.1.7.3/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.2/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.3/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.2/setup.py` & `pillar1-0.1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7.2',
+    version='0.1.7.3',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

