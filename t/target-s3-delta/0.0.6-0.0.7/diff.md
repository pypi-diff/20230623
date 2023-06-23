# Comparing `tmp/target_s3_delta-0.0.6.tar.gz` & `tmp/target_s3_delta-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_s3_delta-0.0.6.tar", max compression
+gzip compressed data, was "target_s3_delta-0.0.7.tar", max compression
```

## Comparing `target_s3_delta-0.0.6.tar` & `target_s3_delta-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.6/README.md
--rw-r--r--   0        0        0     1050 2023-06-21 14:04:18.164708 target_s3_delta-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.6/target_s3_delta/__init__.py
--rw-r--r--   0        0        0     3837 2023-06-21 09:02:13.335808 target_s3_delta-0.0.6/target_s3_delta/sinks.py
--rw-r--r--   0        0        0     4050 2023-06-21 14:03:49.110942 target_s3_delta-0.0.6/target_s3_delta/target.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.7/README.md
+-rw-r--r--   0        0        0     1050 2023-06-22 13:56:29.820122 target_s3_delta-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.7/target_s3_delta/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-22 12:08:20.986818 target_s3_delta-0.0.7/target_s3_delta/common.py
+-rw-r--r--   0        0        0     5947 2023-06-22 12:57:01.960280 target_s3_delta-0.0.7/target_s3_delta/sinks.py
+-rw-r--r--   0        0        0     3905 2023-06-22 13:55:02.356109 target_s3_delta-0.0.7/target_s3_delta/target.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.7/PKG-INFO
```

### Comparing `target_s3_delta-0.0.6/pyproject.toml` & `target_s3_delta-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-s3-delta"
-version = "0.0.6"
+version = "0.0.7"
 description = "`target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["resul yurttakalan"]
 keywords = [
     "ELT",
     "s3-delta",
 ]
```

### Comparing `target_s3_delta-0.0.6/target_s3_delta/target.py` & `target_s3_delta-0.0.7/target_s3_delta/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 import copy
 import os
 from typing import List, Optional, Dict
 
 from deltalake import write_deltalake
 import pyarrow as pa
 import pyarrow.parquet as pq
+import pandas as pd
 from singer_sdk import typing as th
 from singer_sdk.target_base import Target
 
+from target_s3_delta.common import ExtractMode
 from target_s3_delta.sinks import (
     S3DeltaSink,
     TEMP_DATA_DIRECTORY,
 )
 
 
 def read_parquet_generator(file_paths):
     for file_path in file_paths:
-        # Read the Parquet file
-        table = pq.read_table(file_path)
+        df = pd.read_parquet(file_path, engine="pyarrow")
+        sorted_columns = sorted(df.columns)
+        df = df[sorted_columns]
 
-        # Convert the Table to a single RecordBatch and yield it
-        record_batch = pa.RecordBatch.from_pandas(table.to_pandas())
+        record_batch = pa.RecordBatch.from_pandas(df)
         yield record_batch
 
 
 class TargetS3Delta(Target):
     """Sample target for s3-delta."""
 
     name = "target-s3-delta"
@@ -39,15 +41,15 @@
             th.StringType,
             description="The s3 path to the target output file",
             required=True,
         ),
         th.Property("aws_access_key_id", th.StringType, required=True),
         th.Property("aws_secret_access_key", th.StringType, required=True),
         th.Property("aws_region", th.StringType, default="us-east-1"),
-        th.Property("mode", th.StringType, default="overwrite"),
+        th.Property("mode", th.StringType, default=ExtractMode.OVERWRITE),
         th.Property("partition_by", th.StringType),
         th.Property("batch_size", th.IntegerType),
         th.Property("max_rows_per_file", th.IntegerType, default=10 * 1024 * 1024),
     ).to_dict()
 
     default_sink_class = S3DeltaSink
 
@@ -68,33 +70,27 @@
 
     def write_batches_to_delta(self):
         storage_options = self.get_storage_options()
         path = self.config.get("s3_path")
         mode = self.config.get("mode")
         partition_by = self.get_partition_config()
 
-        files = [
-            file
-            for file in os.listdir(TEMP_DATA_DIRECTORY)
-            if file.endswith(".parquet")
-        ]
+        files = [file for file in os.listdir(TEMP_DATA_DIRECTORY) if file.endswith(".parquet")]
 
         if len(files) == 0:
             self.logger.warn(f"Could not create any file.")
             return
 
         absolute_files = [f"{TEMP_DATA_DIRECTORY}{file}" for file in files]
 
         data = read_parquet_generator(absolute_files)
         first_batch = pq.read_table(absolute_files[0])
 
-        # Since singer returns at least one last record in incremental cases, we're truncating it.
-        # https://www.stitchdata.com/docs/replication/replication-methods/key-based-incremental
-        if len(first_batch) <= 1 and mode == "append":
-            self.logger.warn(f"No new records.")
+        if len(first_batch) == 0:
+            self.logger.info(f"Result doesn't have any record. Not created any transaction in Delta table")
             return
 
         write_deltalake(
             path,
             data,
             schema=first_batch.schema,
             storage_options=storage_options,
```

### Comparing `target_s3_delta-0.0.6/PKG-INFO` & `target_s3_delta-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-s3-delta
-Version: 0.0.6
+Version: 0.0.7
 Summary: `target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,s3-delta
 Author: resul yurttakalan
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

