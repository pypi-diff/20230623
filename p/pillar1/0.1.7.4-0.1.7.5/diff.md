# Comparing `tmp/pillar1-0.1.7.4.tar.gz` & `tmp/pillar1-0.1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.4.tar", last modified: Fri Jun 23 14:51:22 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.5.tar", last modified: Fri Jun 23 14:57:27 2023, max compression
```

## Comparing `pillar1-0.1.7.4.tar` & `pillar1-0.1.7.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:51:22.783898 pillar1-0.1.7.4/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:51:22.783779 pillar1-0.1.7.4/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.4/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:51:22.783027 pillar1-0.1.7.4/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.4/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3970 2023-06-23 14:51:11.000000 pillar1-0.1.7.4/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.4/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.4/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:51:22.783608 pillar1-0.1.7.4/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:51:22.000000 pillar1-0.1.7.4/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 14:51:22.000000 pillar1-0.1.7.4/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 14:51:22.000000 pillar1-0.1.7.4/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 14:51:22.000000 pillar1-0.1.7.4/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 14:51:22.783933 pillar1-0.1.7.4/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 14:51:20.000000 pillar1-0.1.7.4/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:57:27.058098 pillar1-0.1.7.5/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:57:27.057942 pillar1-0.1.7.5/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.5/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:57:27.056970 pillar1-0.1.7.5/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.5/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3467 2023-06-23 14:57:21.000000 pillar1-0.1.7.5/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.5/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.5/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 14:57:27.057751 pillar1-0.1.7.5/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 14:57:27.000000 pillar1-0.1.7.5/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 14:57:27.000000 pillar1-0.1.7.5/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 14:57:27.000000 pillar1-0.1.7.5/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 14:57:27.000000 pillar1-0.1.7.5/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 14:57:27.058142 pillar1-0.1.7.5/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 14:57:24.000000 pillar1-0.1.7.5/setup.py
```

### Comparing `pillar1-0.1.7.4/PKG-INFO` & `pillar1-0.1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.4
+Version: 0.1.7.5
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.4/README.md` & `pillar1-0.1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.4/pillar1/constants.py` & `pillar1-0.1.7.5/pillar1/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,17 +70,14 @@
 reference_based_benefits_bundled_ind,boolean,
 national_care_network_ind,boolean,
 price_and_ship_ind,boolean,
 pricing_exclusion_ind,boolean,
 repricing_ind,boolean,
 qualified_health_expense_ind,boolean,
 personal_savings_account_noncovered_ind,boolean,
-mac_reduce_ind,boolean,
-network_ind,boolean,
-network_id,string,
 pre_price_code,string,
 patient_member_source_id,string,
 patient_number,int,
 patient_ssn,string,
 patient_full_name,string,
 patient_first_name,string,
 patient_last_name,string,
@@ -96,45 +93,31 @@
 patient_marital_status,string,
 patient_employment_status,string,
 patient_relationship_code,string,
 patient_account_number,string,
 patient_medical_record_number,string,
 patient_policy_number,string,
 other_payers,string,
-assoc_service_providers,string,
-assoc_service_facilities,string,
-assoc_service_orgs,string,
 insurance_policies,string,
 coordination_of_benefits_code,string,
 coordination_of_benefits_desc,string,
-payee_payee_type,string,
-payee_payee_id_code_type,int,
-payee_payee_id_code_desc,string,
 other_diagnoses,string,
 other_procedures,string,
 disposition_messages,string,
 supporting_information,string,
 applied_benefits,string,
 prescriptions,string,
 contracts,string,
 claim_processes_type,string,
 claim_processes_text,string,
-provenance_target,string,
-provenance_recorded,timestamp,
-provenance_source_organization,string,
 claim_split_ind,boolean,
 carve_out_ind,boolean,
 delivery_date,date,
 daily_interest_rate,double,
 scd_key,int,
-record_effective_datetime,timestamp,
-record_end_datetime,timestamp,
-record_create_datetime,timestamp,
-record_update_datetime,timestamp,
-recent_record_flag,string,
 drg_grouper_review_code,string,
 
 """
 
 STARCODER_BETA += """
 when answering the request use the information listed above only, do not make up column names and do not place additional conditions
     """
```

### Comparing `pillar1-0.1.7.4/pillar1/constants_original.py` & `pillar1-0.1.7.5/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.4/pillar1/pillar1.py` & `pillar1-0.1.7.5/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.4/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.5/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.4
+Version: 0.1.7.5
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.4/setup.py` & `pillar1-0.1.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7.4',
+    version='0.1.7.5',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

