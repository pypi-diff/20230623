# Comparing `tmp/pillar1-0.1.7.6.tar.gz` & `tmp/pillar1-0.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.6.tar", last modified: Fri Jun 23 15:02:40 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.7.tar", last modified: Fri Jun 23 15:05:31 2023, max compression
```

## Comparing `pillar1-0.1.7.6.tar` & `pillar1-0.1.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:02:40.783152 pillar1-0.1.7.6/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:02:40.783038 pillar1-0.1.7.6/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.6/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:02:40.782256 pillar1-0.1.7.6/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.6/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3118 2023-06-23 15:00:04.000000 pillar1-0.1.7.6/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.6/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.6/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:02:40.782864 pillar1-0.1.7.6/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:02:40.000000 pillar1-0.1.7.6/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:02:40.000000 pillar1-0.1.7.6/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:02:40.000000 pillar1-0.1.7.6/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:02:40.000000 pillar1-0.1.7.6/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:02:40.783189 pillar1-0.1.7.6/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:00:47.000000 pillar1-0.1.7.6/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.853871 pillar1-0.1.7.7/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:05:31.853745 pillar1-0.1.7.7/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.7/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.852995 pillar1-0.1.7.7/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.7/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2855 2023-06-23 15:05:11.000000 pillar1-0.1.7.7/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.7/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.7/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.853572 pillar1-0.1.7.7/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:05:31.853915 pillar1-0.1.7.7/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:05:25.000000 pillar1-0.1.7.7/setup.py
```

### Comparing `pillar1-0.1.7.6/PKG-INFO` & `pillar1-0.1.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.6/README.md` & `pillar1-0.1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.6/pillar1/constants.py` & `pillar1-0.1.7.7/pillar1/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -61,16 +61,14 @@
 third_party_liability_ind,boolean,
 xray_enclosure_ind,boolean,
 job_related_ind,boolean,
 national_care_network_ind,boolean,
 price_and_ship_ind,boolean,
 pricing_exclusion_ind,boolean,
 repricing_ind,boolean,
-qualified_health_expense_ind,boolean,
-personal_savings_account_noncovered_ind,boolean,
 pre_price_code,string,
 patient_member_source_id,string,
 patient_number,int,
 patient_ssn,string,
 patient_full_name,string,
 patient_first_name,string,
 patient_last_name,string,
@@ -85,28 +83,21 @@
 patient_gender,string,
 patient_marital_status,string,
 patient_employment_status,string,
 patient_relationship_code,string,
 patient_account_number,string,
 patient_medical_record_number,string,
 patient_policy_number,string,
-other_payers,string,
 insurance_policies,string,
-other_diagnoses,string,
-other_procedures,string,
-disposition_messages,string,
-supporting_information,string,
 applied_benefits,string,
 prescriptions,string,
 contracts,string,
 claim_split_ind,boolean,
 carve_out_ind,boolean,
 delivery_date,date,
-daily_interest_rate,double,
-scd_key,int,
-drg_grouper_review_code,string,
+daily_interest_rate,double
 
 """
 
 STARCODER_BETA += """
 when answering the request use the information listed above only, do not make up column names and do not place additional conditions
     """
```

### Comparing `pillar1-0.1.7.6/pillar1/constants_original.py` & `pillar1-0.1.7.7/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.6/pillar1/pillar1.py` & `pillar1-0.1.7.7/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.6/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.7/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.6/setup.py` & `pillar1-0.1.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7.6',
+    version='0.1.7.7',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

