# Comparing `tmp/phc-ingestion-0.3.39.tar.gz` & `tmp/phc-ingestion-0.3.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.39.tar", last modified: Thu Jun 22 18:21:39 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.40.tar", last modified: Fri Jun 23 16:45:26 2023, max compression
```

## Comparing `phc-ingestion-0.3.39.tar` & `phc-ingestion-0.3.40.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5907 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3142 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     5489 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-06-22 18:21:13.074808 phc-ingestion-0.3.39/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-22 18:21:13.078808 phc-ingestion-0.3.39/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.39/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-23 16:45:03.800337 phc-ingestion-0.3.40/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21663 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5907 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5489 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-23 16:45:03.804337 phc-ingestion-0.3.40/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-23 16:45:03.808337 phc-ingestion-0.3.40/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.40/PKG-INFO
```

### Comparing `phc-ingestion-0.3.39/ingestion/caris/process.py` & `phc-ingestion-0.3.40/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.40/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.40/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.40/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.40/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/json.py` & `phc-ingestion-0.3.40/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.40/ingestion/caris/util/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,25 +321,32 @@
 
     if trigger == False:
         log.info("All IHC tests matched the expected patterns.")
 
     return ihc_results
 
 
+def get_test_type(data):
+    if re.search(r"Hybrid_Transcriptome", data):
+        return "MI Profile - Hybrid"
+    else:
+        return "MI Profile"
+
+
 # Build up the manifest iteratively because almost everything is optional
 def extract_metadata(data, prefix, files, source_file_id, ingest_status, log: Logger):
 
     metadata = {}
 
     test_details = data["testDetails"]
     specimen_details = data["specimenInformation"]["tumorSpecimenInformation"]
 
     physician_details = get_physician_details(data)
 
-    metadata["testType"] = "MI Profile"
+    metadata["testType"] = get_test_type(str(data))
 
     #  Get the date without the time
     metadata["indexedDate"] = test_details["receivedDate"].split()[0]
 
     # Get date of collected and received for the specimen
     metadata["receivedDate"] = get_received_date(specimen_details)
     metadata["collDate"] = get_collected_date(specimen_details)
```

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.40/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.40/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.40/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/foundation/process.py` & `phc-ingestion-0.3.40/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.40/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.40/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.40/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.40/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/process.py` & `phc-ingestion-0.3.40/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.40/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.40/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.40/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.40/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.40/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.40/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.40/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.40/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.40/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.39/pyproject.toml` & `phc-ingestion-0.3.40/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.39"
+version = "0.3.40"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

