# Comparing `tmp/drizzutojr_vader-0.0.8-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6587 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 04:34 vader/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 04:34 vader/core_service.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 04:34 vader/exceptions.py
--rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 04:34 vader/external.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 04:34 vader/general.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 04:34 vader/mongo.py
--rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 04:34 vader/mongo_resource.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 04:34 vader/policy_service.py
--rw-r--r--  2.0 unx      518 b- defN 23-Jun-20 04:34 vader/project_resource.py
--rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 04:34 vader/raise_exception.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-20 04:34 vader/vault_resource.py
--rw-r--r--  2.0 unx      236 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/RECORD
-15 files, 12709 bytes uncompressed, 4653 bytes compressed:  63.4%
+Zip file size: 7031 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 19:45 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-23 19:45 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-23 19:45 vader/exceptions.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-23 19:45 vader/external.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-Jun-23 19:45 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-23 19:45 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-23 19:45 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-23 19:45 vader/policy_service.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Jun-23 19:45 vader/project_resource.py
+-rw-r--r--  2.0 unx     2400 b- defN 23-Jun-23 19:45 vader/raise_exception.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-23 19:45 vader/vault_resource.py
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-23 19:47 drizzutojr_vader-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 19:47 drizzutojr_vader-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-23 19:47 drizzutojr_vader-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-23 19:47 drizzutojr_vader-0.0.9.dist-info/RECORD
+15 files, 14499 bytes uncompressed, 5097 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: vader/raise_exception.py
 Comment: 
 
 Filename: vader/vault_resource.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.8.dist-info/METADATA
+Filename: drizzutojr_vader-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.8.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.8.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.8.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/general.py

```diff
@@ -1,10 +1,12 @@
 import re
 import copy
 
+from .exceptions import *
+
 SPECIAL_CHARACTERS = "[-@!#$%^&*()<>?/\\\|}{~:]"
 BLACKLIST_KEYS = ["password", "token", "secret_id", "secret-id", "credential"]
 SANITIZE_VALUE = "SANITIZE"
 
 
 def contains_special_character(
     custom_string: str, special_characters: str = SPECIAL_CHARACTERS
@@ -39,7 +41,43 @@
     for key, value in the_dict.items():
         if isinstance(value, dict):
             the_dict[key] = sanitize_dict(value, whitelist_keys, blacklist_keys)
         elif key.lower() in blacklist_keys:
             the_dict[key] = SANITIZE_VALUE
 
     return the_dict
+
+
+def convert_to_seconds(time: str):
+    try:
+        integer = int(time[:-1])
+    except ValueError:
+        raise VaderConfigError(
+            f"Time value {time} is not in valid Vader format",
+            details="valid format is XXm, XXh, XXd",
+        )
+    if time.endswith("m"):
+        return convert_mins_to_seconds(time)
+    elif time.endswith("h"):
+        return convert_hours_to_seconds(time)
+    elif time.endswith("d"):
+        return convert_days_to_seconds(time)
+    else:
+        raise VaderConfigError(
+            f"Time value {time} is not in valid Vader format",
+            details="valid format is XXm, XXh, XXd",
+        )
+
+
+def convert_mins_to_seconds(mins: str):
+    mins = int(mins.rstrip("m"))
+    return mins * 60
+
+
+def convert_hours_to_seconds(hours):
+    hours = int(hours.rstrip("h"))
+    return hours * 60 * 60
+
+
+def convert_days_to_seconds(days: str):
+    days = int(days.rstrip("d"))
+    return days * 24 * 60 * 60
```

## vader/raise_exception.py

```diff
@@ -46,7 +46,30 @@
     if not validate_app_id_exists(app_id):
         raise VaderConfigError(f"App ID {app_id} not found")
 
 
 def raise_exception_group_does_not_exist(group_name):
     if not validate_group_exists(group_name):
         raise VaderConfigError(f"Group {group_name} not found")
+
+
+def raise_exception_invalid_min(value_name: str, value: int, min_value: int):
+    if min_value and value < min_value:
+        raise VaderConfigError(
+            f"Value {value} for {value_name} may not be less than {min_value}"
+        )
+
+
+def raise_exception_invalid_max(value_name: str, value: int, max_value: int):
+    if max_value and value > max_value:
+        raise VaderConfigError(
+            f"Value {value} for {value_name} may not be more than {max_value}"
+        )
+
+
+def raise_exception_invalid_option(
+    value_name: str, chosen_option: str, available_options: list
+):
+    if chosen_option not in available_options:
+        raise VaderConfigError(
+            f"Option {chosen_option} for {value_name} must be one of {', '.join(available_options)}"
+        )
```

## Comparing `drizzutojr_vader-0.0.8.dist-info/RECORD` & `drizzutojr_vader-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 vader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vader/core_service.py,sha256=VzIyTc6GAxJUk7B6bO-nP6dHNTJkIpETdznHV1HTl0I,1094
 vader/exceptions.py,sha256=qMmVOiEvdBxZ_3c-EX2kI1QIRjm2QaN7zPD1_fcle_E,1015
 vader/external.py,sha256=W2lB4pKB2q4BFvBPyhbZd2liBTyy8W30LEXMthbGdJI,214
-vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
+vader/general.py,sha256=Xy4mk7pjimP7SQothof56fOmVp3wYO5siAI9vuXKeGk,2404
 vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
 vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
 vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
 vader/project_resource.py,sha256=HIPDD9wxee3OaSZ0t3ij11oim9FzqpehuJcTGF3rgSY,518
-vader/raise_exception.py,sha256=fUSe6NprEZw1DsR4VURWBMiHLJVC-d_2qoGnmkRosFA,1622
+vader/raise_exception.py,sha256=OH4iqtwQjlKMLlX-Gbk68BES0o6Nvs7MMxaqmKU5hsA,2400
 vader/vault_resource.py,sha256=xArBVKJXRuEh_M5HJss5cxycAoH8Uh36Jg4Z_13ga7I,422
-drizzutojr_vader-0.0.8.dist-info/METADATA,sha256=Xzb7ftZBXrdv3OUtuwr_TRZH_Gz1_bgWXUtrOx3HLHI,236
-drizzutojr_vader-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.8.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.8.dist-info/RECORD,,
+drizzutojr_vader-0.0.9.dist-info/METADATA,sha256=KrlnudY-6yegwxtcYL4dzjlpSxvCAvzAQPHM9F07Ycc,269
+drizzutojr_vader-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.9.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.9.dist-info/RECORD,,
```

