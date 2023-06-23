# Comparing `tmp/pillar1-0.1.7.8.tar.gz` & `tmp/pillar1-0.1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.8.tar", last modified: Fri Jun 23 15:42:56 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.9.tar", last modified: Fri Jun 23 15:47:47 2023, max compression
```

## Comparing `pillar1-0.1.7.8.tar` & `pillar1-0.1.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.702218 pillar1-0.1.7.8/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:42:56.702101 pillar1-0.1.7.8/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.8/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.701353 pillar1-0.1.7.8/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.8/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2855 2023-06-23 15:05:11.000000 pillar1-0.1.7.8/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.8/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     4150 2023-06-23 15:41:00.000000 pillar1-0.1.7.8/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.701930 pillar1-0.1.7.8/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:42:56.702255 pillar1-0.1.7.8/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:42:54.000000 pillar1-0.1.7.8/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:47:47.636521 pillar1-0.1.7.9/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:47:47.636398 pillar1-0.1.7.9/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.9/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:47:47.635627 pillar1-0.1.7.9/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.9/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2654 2023-06-23 15:47:38.000000 pillar1-0.1.7.9/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.9/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4150 2023-06-23 15:41:00.000000 pillar1-0.1.7.9/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:47:47.636214 pillar1-0.1.7.9/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:47:47.000000 pillar1-0.1.7.9/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:47:47.000000 pillar1-0.1.7.9/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:47:47.000000 pillar1-0.1.7.9/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:47:47.000000 pillar1-0.1.7.9/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:47:47.636564 pillar1-0.1.7.9/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:47:41.000000 pillar1-0.1.7.9/setup.py
```

### Comparing `pillar1-0.1.7.8/PKG-INFO` & `pillar1-0.1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.8
+Version: 0.1.7.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.8/README.md` & `pillar1-0.1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.8/pillar1/constants.py` & `pillar1-0.1.7.9/pillar1/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,18 +29,14 @@
 additional_source_identifiers[0-5],string,
 extension_source_values[0-5],string,
 claim_type,string,
 claim_status,string,
 claim_response_status_code,int,
 claim_category,string,
 claim_subcategory,string,
-prescription_reference_id,string,
-prescription_date_time,bigint,
-billable_start_date,bigint,
-billable_end_date,bigint,
 claim_submitted_date_time,bigint,
 claim_received_date_time,bigint,
 claim_incurred_date_time,bigint,
 claim_adjudication_date_time,bigint,
 claim_paid_date_time,bigint,
 claim_reversal_date_time,bigint,
 claim_last_action_date,bigint,
@@ -53,18 +49,15 @@
 reason_visit,string,
 business_category_codes,string,
 claim_reference_ids,string,
 reference_ids,string,
 claim_sequence_number,string,
 claim_origination_code,string,
 lob,string,
-accident_ind,boolean,
-third_party_liability_ind,boolean,
 xray_enclosure_ind,boolean,
-job_related_ind,boolean,
 national_care_network_ind,boolean,
 price_and_ship_ind,boolean,
 pricing_exclusion_ind,boolean,
 repricing_ind,boolean,
 pre_price_code,string,
 patient_member_source_id,string,
 patient_number,int,
```

### Comparing `pillar1-0.1.7.8/pillar1/constants_original.py` & `pillar1-0.1.7.9/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.8/pillar1/pillar1.py` & `pillar1-0.1.7.9/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.8/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.9/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.8
+Version: 0.1.7.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.8/setup.py` & `pillar1-0.1.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7.8',
+    version='0.1.7.9',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

