# Comparing `tmp/dramatiq_kafka-0.1.8.tar.gz` & `tmp/dramatiq_kafka-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_kafka-0.1.8.tar", max compression
+gzip compressed data, was "dramatiq_kafka-0.1.9.tar", max compression
```

## Comparing `dramatiq_kafka-0.1.8.tar` & `dramatiq_kafka-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1201 2023-06-20 03:42:55.693621 dramatiq_kafka-0.1.8/README.md
--rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.8/dramatiq_kafka/__init__.py
--rw-r--r--   0        0        0     4318 2023-06-20 03:31:24.214817 dramatiq_kafka-0.1.8/dramatiq_kafka/broker.py
--rw-r--r--   0        0        0      350 2023-06-20 04:19:01.618992 dramatiq_kafka-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1201 2023-06-20 03:42:55.693621 dramatiq_kafka-0.1.9/README.md
+-rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.9/dramatiq_kafka/__init__.py
+-rw-r--r--   0        0        0     4318 2023-06-20 03:31:24.214817 dramatiq_kafka-0.1.9/dramatiq_kafka/broker.py
+-rw-r--r--   0        0        0      373 2023-06-23 00:27:48.643236 dramatiq_kafka-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.9/PKG-INFO
```

### Comparing `dramatiq_kafka-0.1.8/README.md` & `dramatiq_kafka-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_kafka-0.1.8/dramatiq_kafka/broker.py` & `dramatiq_kafka-0.1.9/dramatiq_kafka/broker.py`

 * *Files identical despite different names*

### Comparing `dramatiq_kafka-0.1.8/PKG-INFO` & `dramatiq_kafka-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dramatiq-kafka
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Kafka broker for Dramatiq.
 Author: Viktor Babchanik
 Author-email: vbabchanik@ucdavis.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: kafka-python (==2.0.2)
 Description-Content-Type: text/markdown
 
 Uses kafka-python package to write a Kafka broker for dramatiq.
 
 ```python
 
 import dramatiq
```

