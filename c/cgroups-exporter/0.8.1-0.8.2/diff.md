# Comparing `tmp/cgroups_exporter-0.8.1.tar.gz` & `tmp/cgroups_exporter-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgroups_exporter-0.8.1.tar", max compression
+gzip compressed data, was "cgroups_exporter-0.8.2.tar", max compression
```

## Comparing `cgroups_exporter-0.8.1.tar` & `cgroups_exporter-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11342 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/LICENSE
--rw-r--r--   0        0        0    19855 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/__init__.py
--rw-r--r--   0        0        0     2285 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/__main__.py
--rw-r--r--   0        0        0     1568 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/args.py
--rw-r--r--   0        0        0      825 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/__init__.py
--rw-r--r--   0        0        0     2423 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/_metrics.py
--rw-r--r--   0        0        0     3876 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/base.py
--rw-r--r--   0        0        0     4110 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/blkio.py
--rw-r--r--   0        0        0     1088 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/cpu.py
--rw-r--r--   0        0        0     1029 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/cpuset.py
--rw-r--r--   0        0        0     2265 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/meminfo.py
--rw-r--r--   0        0        0     2468 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/memory.py
--rw-r--r--   0        0        0      662 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/pids.py
--rw-r--r--   0        0        0     1594 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/metrics/unified.py
--rw-r--r--   0        0        0        1 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/services/__init__.py
--rw-r--r--   0        0        0     2435 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/services/collector.py
--rw-r--r--   0        0        0     1022 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/cgroups_exporter/services/metrics.py
--rw-r--r--   0        0        0     1473 2023-06-23 19:22:49.518762 cgroups_exporter-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    21354 1970-01-01 00:00:00.000000 cgroups_exporter-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-23 19:31:16.575904 cgroups_exporter-0.8.2/LICENSE
+-rw-r--r--   0        0        0    19855 2023-06-23 19:31:16.575904 cgroups_exporter-0.8.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 19:31:16.575904 cgroups_exporter-0.8.2/cgroups_exporter/__init__.py
+-rw-r--r--   0        0        0     2285 2023-06-23 19:31:16.575904 cgroups_exporter-0.8.2/cgroups_exporter/__main__.py
+-rw-r--r--   0        0        0     1568 2023-06-23 19:31:16.575904 cgroups_exporter-0.8.2/cgroups_exporter/args.py
+-rw-r--r--   0        0        0      825 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/__init__.py
+-rw-r--r--   0        0        0     2423 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/_metrics.py
+-rw-r--r--   0        0        0     3876 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/base.py
+-rw-r--r--   0        0        0     4110 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/blkio.py
+-rw-r--r--   0        0        0     1088 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/cpu.py
+-rw-r--r--   0        0        0     1029 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/cpuset.py
+-rw-r--r--   0        0        0     2265 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/meminfo.py
+-rw-r--r--   0        0        0     2468 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/memory.py
+-rw-r--r--   0        0        0      662 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/pids.py
+-rw-r--r--   0        0        0     1594 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/metrics/unified.py
+-rw-r--r--   0        0        0        1 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/services/__init__.py
+-rw-r--r--   0        0        0     2435 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/services/collector.py
+-rw-r--r--   0        0        0     1022 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/cgroups_exporter/services/metrics.py
+-rw-r--r--   0        0        0     1473 2023-06-23 19:31:16.579904 cgroups_exporter-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    21354 1970-01-01 00:00:00.000000 cgroups_exporter-0.8.2/PKG-INFO
```

### Comparing `cgroups_exporter-0.8.1/LICENSE` & `cgroups_exporter-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/README.md` & `cgroups_exporter-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/__main__.py` & `cgroups_exporter-0.8.2/cgroups_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/args.py` & `cgroups_exporter-0.8.2/cgroups_exporter/args.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/__init__.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/_metrics.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/base.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/base.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/blkio.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/blkio.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/cpu.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/cpu.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/cpuset.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/cpuset.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/meminfo.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/meminfo.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/memory.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/memory.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/pids.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/pids.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/metrics/unified.py` & `cgroups_exporter-0.8.2/cgroups_exporter/metrics/unified.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/services/collector.py` & `cgroups_exporter-0.8.2/cgroups_exporter/services/collector.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/cgroups_exporter/services/metrics.py` & `cgroups_exporter-0.8.2/cgroups_exporter/services/metrics.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.8.1/pyproject.toml` & `cgroups_exporter-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgroups-exporter"
-version = "0.8.1"
+version = "0.8.2"
 description = "prometheus exporter for cgroups v1"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 license = "Apache Software License"
 homepage = "https://github.com/mosquito/cgroups-exporter"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `cgroups_exporter-0.8.1/PKG-INFO` & `cgroups_exporter-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgroups-exporter
-Version: 0.8.1
+Version: 0.8.2
 Summary: prometheus exporter for cgroups v1
 Home-page: https://github.com/mosquito/cgroups-exporter
 License: Apache Software License
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

