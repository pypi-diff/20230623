# Comparing `tmp/cgroups_exporter-0.8.5-py3-none-any.whl.zip` & `tmp/cgroups_exporter-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 21111 bytes, number of entries: 21
+Zip file size: 21076 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 cgroups_exporter/__init__.py
 -rw-r--r--  2.0 unx     2285 b- defN 80-Jan-01 00:00 cgroups_exporter/__main__.py
 -rw-r--r--  2.0 unx     1568 b- defN 80-Jan-01 00:00 cgroups_exporter/args.py
 -rw-r--r--  2.0 unx      825 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/_metrics.py
--rw-r--r--  2.0 unx     4055 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/base.py
+-rw-r--r--  2.0 unx     2463 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/_metrics.py
+-rw-r--r--  2.0 unx     3868 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/base.py
 -rw-r--r--  2.0 unx     4110 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/blkio.py
 -rw-r--r--  2.0 unx     1088 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/cpu.py
 -rw-r--r--  2.0 unx     1029 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/cpuset.py
 -rw-r--r--  2.0 unx     2265 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/meminfo.py
 -rw-r--r--  2.0 unx     2468 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/memory.py
 -rw-r--r--  2.0 unx      662 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/pids.py
 -rw-r--r--  2.0 unx     1594 b- defN 80-Jan-01 00:00 cgroups_exporter/metrics/unified.py
 -rw-r--r--  2.0 unx        1 b- defN 80-Jan-01 00:00 cgroups_exporter/services/__init__.py
 -rw-r--r--  2.0 unx     2435 b- defN 80-Jan-01 00:00 cgroups_exporter/services/collector.py
 -rw-r--r--  2.0 unx     1022 b- defN 80-Jan-01 00:00 cgroups_exporter/services/metrics.py
--rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    21354 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1869 b- defN 16-Jan-01 00:00 cgroups_exporter-0.8.5.dist-info/RECORD
-21 files, 62550 bytes uncompressed, 18021 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    21354 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 cgroups_exporter-0.8.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1869 b- defN 16-Jan-01 00:00 cgroups_exporter-0.8.6.dist-info/RECORD
+21 files, 62403 bytes uncompressed, 17986 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: cgroups_exporter/services/collector.py
 Comment: 
 
 Filename: cgroups_exporter/services/metrics.py
 Comment: 
 
-Filename: cgroups_exporter-0.8.5.dist-info/LICENSE
+Filename: cgroups_exporter-0.8.6.dist-info/LICENSE
 Comment: 
 
-Filename: cgroups_exporter-0.8.5.dist-info/METADATA
+Filename: cgroups_exporter-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: cgroups_exporter-0.8.5.dist-info/WHEEL
+Filename: cgroups_exporter-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: cgroups_exporter-0.8.5.dist-info/entry_points.txt
+Filename: cgroups_exporter-0.8.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: cgroups_exporter-0.8.5.dist-info/RECORD
+Filename: cgroups_exporter-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cgroups_exporter/metrics/_metrics.py

```diff
@@ -12,15 +12,17 @@
 class MetricBase:
     __slots__ = ("name", "label_names", "type", "help")
 
     def __init__(
         self, *, name: str, labelnames: Iterable[str], help: str = None,
         type: str = "gauge", namespace: str, subsystem: str, unit: str,
     ):
-        self.name = "_".join(filter(None, (namespace, subsystem, name, unit)))
+        self.name = "_".join(
+            filter(None, (namespace, subsystem, name, unit))
+        ).replace(".", "_")
         self.help = help
         self.type = type
         self.label_names = frozenset(labelnames)
 
 
 class Record(NamedTuple):
     metric: MetricBase
```

## cgroups_exporter/metrics/base.py

```diff
@@ -50,31 +50,25 @@
             self.task.group.replace(",", "_"),
             self.DOCUMENTATION,
             labelnames=("base_path", "path"),
         )
         metric.labels(base_path=self.base_path, path=self.path).set(value)
 
 
-def _normalize_name(name: Optional[str]) -> Optional[str]:
-    if name is None:
-        return None
-    return name.replace(".", "_")
-
-
 @lru_cache(2 ** 20)
 def gauge_factory(
     name: str, unit: str, group, documentation: str, labelnames=(),
 ) -> Metric:
     return Metric(
-        name=_normalize_name(name),
+        name=name,
         help=documentation,
         labelnames=labelnames,
         namespace="cgroups",
-        subsystem=_normalize_name(group),
-        unit=_normalize_name(unit),
+        subsystem=group,
+        unit=unit,
     )
 
 
 class UsageBase(IntProviderBase):
     NAME = "usage"
```

## Comparing `cgroups_exporter-0.8.5.dist-info/LICENSE` & `cgroups_exporter-0.8.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cgroups_exporter-0.8.5.dist-info/METADATA` & `cgroups_exporter-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgroups-exporter
-Version: 0.8.5
+Version: 0.8.6
 Summary: prometheus exporter for cgroups v1
 Home-page: https://github.com/mosquito/cgroups-exporter
 License: Apache Software License
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

## Comparing `cgroups_exporter-0.8.5.dist-info/RECORD` & `cgroups_exporter-0.8.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 cgroups_exporter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cgroups_exporter/__main__.py,sha256=0hQftXGkq2B3AFy6llXGE3bGzDM7rUeNNPhfN6Do2nI,2285
 cgroups_exporter/args.py,sha256=vTZgVGne-azFaxM15WVpzvoJXUAuRDS_9syZmV6uS9g,1568
 cgroups_exporter/metrics/__init__.py,sha256=BQBo20E8AiaqwaKRbgvq7phoiMCQHTpafKKwFG_M2Lw,825
-cgroups_exporter/metrics/_metrics.py,sha256=Ii3uuhnIGNz1iqNrz6qZiJ-_jkvUUZWSBDNboMvWtEQ,2423
-cgroups_exporter/metrics/base.py,sha256=Fcj-z9EgsJDtWYbAQtJLUKcAL4AAraV9USgUmm6LiDE,4055
+cgroups_exporter/metrics/_metrics.py,sha256=xHvX5gncw_SDLxX-cp_PqtcyA_2zMvigLKK4abdinNA,2463
+cgroups_exporter/metrics/base.py,sha256=uxBHK_PDA8-HbAhURMYvJkqNJafZPP8_wphJZ7OoI4w,3868
 cgroups_exporter/metrics/blkio.py,sha256=2S3yexM80ClusfzK157pTGTOe7-l-qLAnEOw77pYjmg,4110
 cgroups_exporter/metrics/cpu.py,sha256=Ly951AQQgWgIC6if_hDN5Eok0rHdZaZKH_7yfvATZls,1088
 cgroups_exporter/metrics/cpuset.py,sha256=9471vDYRjKa8PYNNfP1ZB3qLqF_1ywRHrtRxl0vNY2c,1029
 cgroups_exporter/metrics/meminfo.py,sha256=iI8e9t4tQUWKDR9Nu_vrN127sgCz-Z6omn1GxU7SDPQ,2265
 cgroups_exporter/metrics/memory.py,sha256=82LqX7YolytAS-SJgQYXbqUKgMusozwsiouKvD6FZjY,2468
 cgroups_exporter/metrics/pids.py,sha256=vPpKw6l-UWCaUa0wVCK2EmqLpn12LHmDNlXWFJ4N3y8,662
 cgroups_exporter/metrics/unified.py,sha256=5XNb5U8NagcDQ3Ig32SBEOXnO1GKHj4YI0Qaq3b95gA,1594
 cgroups_exporter/services/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 cgroups_exporter/services/collector.py,sha256=-RUpElWVWZnFY7yJwEW34w2wda6QMW0mqhhWVGAiHpc,2435
 cgroups_exporter/services/metrics.py,sha256=5Eg0Vz6lU3tQothWXphmX1ISfkT1i3hkBTYT8Y5owdM,1022
-cgroups_exporter-0.8.5.dist-info/LICENSE,sha256=Ko9a9G-QeYbBpbibcTs0xWltlO4IzMolJxE8s0KWK5U,11342
-cgroups_exporter-0.8.5.dist-info/METADATA,sha256=7tD0TNnbCuVjWzC-30N7nuuEOq4BJoAFblXzf_giO38,21354
-cgroups_exporter-0.8.5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-cgroups_exporter-0.8.5.dist-info/entry_points.txt,sha256=4eVZE-9Dk6NG6TBp6lsSAMj2MJtihc-e1uHYjR53vf4,67
-cgroups_exporter-0.8.5.dist-info/RECORD,,
+cgroups_exporter-0.8.6.dist-info/LICENSE,sha256=Ko9a9G-QeYbBpbibcTs0xWltlO4IzMolJxE8s0KWK5U,11342
+cgroups_exporter-0.8.6.dist-info/METADATA,sha256=n_0U6TigMj0Kp0WW6i8haSfjdczw3F0Cy8ZW0vFqj64,21354
+cgroups_exporter-0.8.6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+cgroups_exporter-0.8.6.dist-info/entry_points.txt,sha256=4eVZE-9Dk6NG6TBp6lsSAMj2MJtihc-e1uHYjR53vf4,67
+cgroups_exporter-0.8.6.dist-info/RECORD,,
```

