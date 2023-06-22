# Comparing `tmp/palmers_agents_general-0.0.8.tar.gz` & `tmp/palmers_agents_general-0.0.9.tar.gz`

## Comparing `palmers_agents_general-0.0.8.tar` & `palmers_agents_general-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/__init__.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/base_mq_worker.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/blobs_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/base_mq_consumer.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/base_mq_worker.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/db_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.8/palmers_agents_general/base_mq_worker.py` & `palmers_agents_general-0.0.9/palmers_agents_general/base_mq_worker.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.8/palmers_agents_general/blobs_handler.py` & `palmers_agents_general-0.0.9/palmers_agents_general/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.8/palmers_agents_general/models_handler.py` & `palmers_agents_general-0.0.9/palmers_agents_general/models_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.8/LICENSE` & `palmers_agents_general-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.8/pyproject.toml` & `palmers_agents_general-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_agents_general-0.0.8/PKG-INFO` & `palmers_agents_general-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_agents_general
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Assaf <assafm@sdatta.ai>, Roy  <roy@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

