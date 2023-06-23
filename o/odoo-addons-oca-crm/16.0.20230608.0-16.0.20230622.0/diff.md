# Comparing `tmp/odoo_addons_oca_crm-16.0.20230608.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_crm-16.0.20230622.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1359 bytes, number of entries: 4
--rw-r--r--  2.0 unx      796 b- defN 23-Jun-09 03:10 odoo_addons_oca_crm-16.0.20230608.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 03:10 odoo_addons_oca_crm-16.0.20230608.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-09 03:10 odoo_addons_oca_crm-16.0.20230608.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      384 b- defN 23-Jun-09 03:10 odoo_addons_oca_crm-16.0.20230608.0.dist-info/RECORD
-4 files, 1273 bytes uncompressed, 601 bytes compressed:  52.8%
+Zip file size: 1364 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      861 b- defN 23-Jun-23 03:06 odoo_addons_oca_crm-16.0.20230622.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 03:06 odoo_addons_oca_crm-16.0.20230622.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 03:06 odoo_addons_oca_crm-16.0.20230622.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      384 b- defN 23-Jun-23 03:06 odoo_addons_oca_crm-16.0.20230622.0.dist-info/RECORD
+4 files, 1338 bytes uncompressed, 606 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_crm-16.0.20230608.0.dist-info/METADATA
+Filename: odoo_addons_oca_crm-16.0.20230622.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_crm-16.0.20230608.0.dist-info/WHEEL
+Filename: odoo_addons_oca_crm-16.0.20230622.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_crm-16.0.20230608.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_crm-16.0.20230622.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_crm-16.0.20230608.0.dist-info/RECORD
+Filename: odoo_addons_oca_crm-16.0.20230622.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_crm-16.0.20230608.0.dist-info/METADATA` & `odoo_addons_oca_crm-16.0.20230622.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-crm
-Version: 16.0.20230608.0
+Version: 16.0.20230622.0
 Summary: Meta package for oca-crm Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-crm-claim (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-industry (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-lead-code (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-crm-lead-currency (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-lead-firstname (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-lead-search-archive (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-location (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-partner-assign (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-crm-phonecall (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

