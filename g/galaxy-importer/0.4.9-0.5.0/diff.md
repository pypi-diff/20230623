# Comparing `tmp/galaxy_importer-0.4.9.tar.gz` & `tmp/galaxy_importer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_importer-0.4.9.tar", last modified: Tue Apr 18 15:38:20 2023, max compression
+gzip compressed data, was "galaxy_importer-0.5.0.tar", last modified: Mon Apr  3 14:21:12 2023, max compression
```

## Comparing `galaxy_importer-0.4.9.tar` & `galaxy_importer-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.272026 galaxy_importer-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 15:38:20.272026 galaxy_importer-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/ansible_test/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/ansible_test/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/builders/local_image_build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/ansible_test/container/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/container/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/container/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/job_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/local_ansible_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/local_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/openshift_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/loaders/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/loaders/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/loaders/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/loaders/runtime_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.272026 galaxy_importer-0.4.9/galaxy_importer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/chksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/requires_ansible_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/galaxy_importer/utils/string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:20.268026 galaxy_importer-0.4.9/galaxy_importer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 15:38:20.000000 galaxy_importer-0.4.9/galaxy_importer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 15:38:20.000000 galaxy_importer-0.4.9/galaxy_importer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:38:20.000000 galaxy_importer-0.4.9/galaxy_importer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 15:38:20.000000 galaxy_importer-0.4.9/galaxy_importer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 15:38:20.000000 galaxy_importer-0.4.9/galaxy_importer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 15:38:20.272026 galaxy_importer-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 15:38:09.000000 galaxy_importer-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.843355 galaxy_importer-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-03 14:21:12.843355 galaxy_importer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer/ansible_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer/ansible_test/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/builders/local_image_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer/ansible_test/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/container/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/container/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/job_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/local_ansible_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/local_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/openshift_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.843355 galaxy_importer-0.5.0/galaxy_importer/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/loaders/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/loaders/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/loaders/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/loaders/runtime_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.843355 galaxy_importer-0.5.0/galaxy_importer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/chksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/requires_ansible_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/galaxy_importer/utils/string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:21:12.839355 galaxy_importer-0.5.0/galaxy_importer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-03 14:21:12.000000 galaxy_importer-0.5.0/galaxy_importer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-03 14:21:12.000000 galaxy_importer-0.5.0/galaxy_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:21:12.000000 galaxy_importer-0.5.0/galaxy_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-03 14:21:12.000000 galaxy_importer-0.5.0/galaxy_importer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 14:21:12.000000 galaxy_importer-0.5.0/galaxy_importer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-03 14:21:12.843355 galaxy_importer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-03 14:21:01.000000 galaxy_importer-0.5.0/setup.py
```

### Comparing `galaxy_importer-0.4.9/LICENSE` & `galaxy_importer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/PKG-INFO` & `galaxy_importer-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy_importer
-Version: 0.4.9
+Version: 0.5.0
 Summary: Galaxy content importer
 Home-page: https://github.com/ansible/galaxy-importer
 Author: Red Hat, Inc.
 Author-email: info@ansible.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `galaxy_importer-0.4.9/README.md` & `galaxy_importer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/__init__.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/builders/__init__.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/builders/local_image_build.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/builders/local_image_build.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/container/Dockerfile` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/container/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/container/entrypoint.sh` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/container/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/job_template.yaml` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/job_template.yaml`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/__init__.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/base.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/base.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/local_ansible_test.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/local_ansible_test.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/local_image.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/local_image.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/ansible_test/runners/openshift_job.py` & `galaxy_importer-0.5.0/galaxy_importer/ansible_test/runners/openshift_job.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/collection.py` & `galaxy_importer-0.5.0/galaxy_importer/collection.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/config.py` & `galaxy_importer-0.5.0/galaxy_importer/config.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/constants.py` & `galaxy_importer-0.5.0/galaxy_importer/constants.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/exceptions.py` & `galaxy_importer-0.5.0/galaxy_importer/exceptions.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/finder.py` & `galaxy_importer-0.5.0/galaxy_importer/finder.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/loaders/collection.py` & `galaxy_importer-0.5.0/galaxy_importer/loaders/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 # You should have received a copy of the Apache License
 # along with Galaxy.  If not, see <http://www.apache.org/licenses/>.
 
 import logging
 import os
 import re
 
-try:
-    from ansible_builder import introspect
-except ImportError:
-    from ansible_builder._target_scripts import introspect
+import ansible_builder.introspect
 
 from galaxy_importer import exceptions as exc
 from galaxy_importer.finder import ContentFinder, FileWalker
 from galaxy_importer import loaders
 from galaxy_importer import schema
 from galaxy_importer.utils import markup as markup_utils
 from galaxy_importer.utils import chksums
@@ -141,15 +138,15 @@
         """Check for python deps file and system deps file if they are listed in
         meta/execution-environment.yml, and log if listed files are not found
 
         Method excluded from pytest coverage, test exist outside repo via iqe.
         """
 
         try:
-            python_deps, system_deps = introspect.process_collection(self.path)
+            python_deps, system_deps = ansible_builder.introspect.process_collection(self.path)
         except FileNotFoundError as e:
             self.log.error(
                 f"Error when checking meta/execution-environment.yml for dependency files: {e}"
             )
 
     def _load_manifest(self):
         manifest_file = os.path.join(self.path, "MANIFEST.json")
```

### Comparing `galaxy_importer-0.4.9/galaxy_importer/loaders/content.py` & `galaxy_importer-0.5.0/galaxy_importer/loaders/content.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import abc
 import logging
 import os
 from pathlib import Path
 import re
 import shutil
-from subprocess import Popen, PIPE, TimeoutExpired
+from subprocess import Popen, PIPE
 import yaml
 
 from galaxy_importer import constants
 from galaxy_importer import exceptions as exc
 from galaxy_importer import schema
 from galaxy_importer.utils import markup as markup_utils
 
@@ -222,28 +222,20 @@
         proc = Popen(
             cmd,
             cwd=self.root,
             encoding="utf-8",
             stdout=PIPE,
             stderr=PIPE,
         )
+        proc.wait()
 
-        try:
-            outs, errs = proc.communicate(timeout=120)
-        except (
-            TimeoutExpired
-        ):  # pragma: no cover - a TimeoutExpired mock would apply to both calls to commnicate()
-            self.log.error("Timeout on call to ansible-lint")
-            proc.kill()
-            outs, errs = proc.communicate()
-
-        for line in outs.splitlines():
+        for line in proc.stdout:
             self.log.warning(line.strip())
 
-        for line in errs.splitlines():
+        for line in proc.stderr:
             if line.startswith(constants.ANSIBLE_LINT_ERROR_PREFIXES):
                 self.log.error(line.rstrip())
 
     def _get_readme(self):
         readme = markup_utils.get_readme_doc_file(os.path.join(self.root, self.rel_path))
         if not readme:
             raise exc.ContentLoadError("No role readme found.")
```

### Comparing `galaxy_importer-0.4.9/galaxy_importer/loaders/doc_string.py` & `galaxy_importer-0.5.0/galaxy_importer/loaders/doc_string.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/loaders/runtime_file.py` & `galaxy_importer-0.5.0/galaxy_importer/loaders/runtime_file.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/main.py` & `galaxy_importer-0.5.0/galaxy_importer/main.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/schema.py` & `galaxy_importer-0.5.0/galaxy_importer/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 _FILENAME_RE = re.compile(
     r"^(?P<namespace>\w+)-(?P<name>\w+)-" r"(?P<version>[0-9a-zA-Z.+-]+)\.tar\.gz$"
 )
 
 
 @attr.s(slots=True)
 class CollectionFilename(object):
+
     namespace = attr.ib()
     name = attr.ib()
     version = attr.ib(converter=semantic_version.Version)
 
     def __str__(self):
         return f"{self.namespace}-{self.name}-{self.version}.tar.gz"
```

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/__init__.py` & `galaxy_importer-0.5.0/galaxy_importer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/chksums.py` & `galaxy_importer-0.5.0/galaxy_importer/utils/chksums.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/markup.py` & `galaxy_importer-0.5.0/galaxy_importer/utils/markup.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/requires_ansible_version.py` & `galaxy_importer-0.5.0/galaxy_importer/utils/requires_ansible_version.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/spdx_licenses.json` & `galaxy_importer-0.5.0/galaxy_importer/utils/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer/utils/spdx_licenses.py` & `galaxy_importer-0.5.0/galaxy_importer/utils/spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/galaxy_importer.egg-info/PKG-INFO` & `galaxy_importer-0.5.0/galaxy_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-importer
-Version: 0.4.9
+Version: 0.5.0
 Summary: Galaxy content importer
 Home-page: https://github.com/ansible/galaxy-importer
 Author: Red Hat, Inc.
 Author-email: info@ansible.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `galaxy_importer-0.4.9/galaxy_importer.egg-info/SOURCES.txt` & `galaxy_importer-0.5.0/galaxy_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_importer-0.4.9/setup.cfg` & `galaxy_importer-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 install_requires = 
 	ansible-core
-	ansible-builder>=1.2.0,<4.0
+	ansible-builder>=1.0.1,<2.0
 	ansible-lint>=6.2.2,<=6.14.3
 	attrs>=21.4.0,<23
 	bleach>=3.3.0,<4
 	bleach-allowlist>=1.0.3,<2
 	flake8>=5.0.0,<7
 	markdown>=3.3.4,<4
 	pyyaml>=5.4.1,<7
@@ -41,14 +41,14 @@
 galaxy_importer = 
 	utils/spdx_licenses.json
 	ansible_test/job_template.yaml
 	ansible_test/container/Dockerfile
 	ansible_test/container/entrypoint.sh
 
 [coverage:report]
-fail_under = 95.50
+fail_under = 95.57
 precision = 2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

