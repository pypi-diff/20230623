# Comparing `tmp/django_cloudwatch_metrics-0.0.8.tar.gz` & `tmp/django_cloudwatch_metrics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloudwatch_metrics-0.0.8.tar", max compression
+gzip compressed data, was "django_cloudwatch_metrics-0.0.9.tar", max compression
```

## Comparing `django_cloudwatch_metrics-0.0.8.tar` & `django_cloudwatch_metrics-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       27 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/README.md
--rw-r--r--   0        0        0      197 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/apps.py
--rw-r--r--   0        0        0      635 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/hashing.py
--rw-r--r--   0        0        0        0 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      722 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/commands/increment.py
--rw-r--r--   0        0        0     2336 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/commands/publish_metrics.py
--rw-r--r--   0        0        0     1282 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/metrics.py
--rw-r--r--   0        0        0      926 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0      462 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/0002_alter_metricaggregation_id.py
--rw-r--r--   0        0        0     1650 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/0003_auto_20230606_1148.py
--rw-r--r--   0        0        0        0 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/__init__.py
--rw-r--r--   0        0        0      377 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/models.py
--rw-r--r--   0        0        0    12871 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/signals.py
--rw-r--r--   0        0        0      543 2023-06-06 12:08:59.649495 django_cloudwatch_metrics-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/README.md
+-rw-r--r--   0        0        0      197 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/apps.py
+-rw-r--r--   0        0        0      635 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/hashing.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      722 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/commands/increment.py
+-rw-r--r--   0        0        0     2336 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/commands/publish_metrics.py
+-rw-r--r--   0        0        0     1050 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/metrics.py
+-rw-r--r--   0        0        0      926 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0      462 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/0002_alter_metricaggregation_id.py
+-rw-r--r--   0        0        0     1650 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/0003_auto_20230606_1148.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/models.py
+-rw-r--r--   0        0        0    12871 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/signals.py
+-rw-r--r--   0        0        0      543 2023-06-21 09:47:29.809019 django_cloudwatch_metrics-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.9/PKG-INFO
```

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/hashing.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/hashing.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/commands/increment.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/commands/increment.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/management/commands/publish_metrics.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/management/commands/publish_metrics.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/metrics.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 import base64
 import hashlib
 from datetime import datetime
 from typing import Optional
 
 import pytz
 from django.db.models import F
+from django.db.transaction import atomic
 
 from django_cloudwatch_metrics.hashing import create_cache_key
 from django_cloudwatch_metrics.models import MetricAggregation
 
 
+@atomic
 def increment(metric_name: str, value: int, **kwargs):
     """Publishes a metric increment."""
     datetime_period = datetime.now(pytz.utc).replace(second=0, microsecond=0)
 
-    aggregation_hash_key = create_cache_key(
+    aggregation_key = create_cache_key(
         metric_name,
         datetime_period,
         kwargs,
     )
 
-    try:
-        metric_aggregation, created = MetricAggregation.objects.get_or_create(
-            aggregation_key=aggregation_hash_key,
-            defaults={
-                "datetime_period":  datetime_period,
-                "metric_name": metric_name,
-                "dimension_data": kwargs,
-                "value": value,
-            }
-        )
-    except MetricAggregation.MultipleObjectsReturned:
-        metric_aggregation = MetricAggregation.objects.filter(
-            aggregation_key=aggregation_hash_key
-        ).first()
-        created = False
-
-    if created:
-        return
+    metric_aggregation, created = MetricAggregation.objects.select_for_update().get_or_create(
+        aggregation_key=aggregation_key,
+        defaults={
+            "datetime_period":  datetime_period,
+            "metric_name": metric_name,
+            "dimension_data": kwargs,
+            "value": value,
+        }
+    )
 
-    if metric_aggregation:
+    if not created:
         metric_aggregation.value = F("value") + value
-        metric_aggregation.save(update_fields=["value"])
+        metric_aggregation.save(update_fields=["value"])
```

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/0001_initial.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/migrations/0003_auto_20230606_1148.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/migrations/0003_auto_20230606_1148.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/django_cloudwatch_metrics/signals.py` & `django_cloudwatch_metrics-0.0.9/django_cloudwatch_metrics/signals.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.8/pyproject.toml` & `django_cloudwatch_metrics-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloudwatch-metrics"
-version = "0.0.8"
+version = "0.0.9"
 description = "Metric tracking in Django using caching and CloudWatch"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "django_cloudwatch_metrics" }
```

### Comparing `django_cloudwatch_metrics-0.0.8/PKG-INFO` & `django_cloudwatch_metrics-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloudwatch-metrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Metric tracking in Django using caching and CloudWatch
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.6.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

