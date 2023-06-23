# Comparing `tmp/kafka-schema-registry-admin-0.2.4.tar.gz` & `tmp/kafka_schema_registry_admin-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-schema-registry-admin-0.2.4.tar", max compression
+gzip compressed data, was "kafka_schema_registry_admin-0.2.5.tar", max compression
```

## Comparing `kafka-schema-registry-admin-0.2.4.tar` & `kafka_schema_registry_admin-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     7652 2022-06-27 09:02:38.500773 kafka-schema-registry-admin-0.2.4/LICENSE
--rw-r--r--   0        0        0      586 2022-06-27 09:02:38.501772 kafka-schema-registry-admin-0.2.4/README.rst
--rw-r--r--   0        0        0      239 2022-07-15 10:03:43.303831 kafka-schema-registry-admin-0.2.4/kafka_schema_registry_admin/__init__.py
--rw-r--r--   0        0        0    14933 2022-07-15 10:03:03.368239 kafka-schema-registry-admin-0.2.4/kafka_schema_registry_admin/kafka_schema_registry_admin.py
--rw-r--r--   0        0        0     1569 2022-07-15 10:03:43.303831 kafka-schema-registry-admin-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1306 2022-07-15 10:03:48.852516 kafka-schema-registry-admin-0.2.4/setup.py
--rw-r--r--   0        0        0     1415 2022-07-15 10:03:48.852733 kafka-schema-registry-admin-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2022-06-27 09:02:38.500773 kafka_schema_registry_admin-0.2.5/LICENSE
+-rw-r--r--   0        0        0      586 2022-06-27 09:02:38.501772 kafka_schema_registry_admin-0.2.5/README.rst
+-rw-r--r--   0        0        0      239 2023-06-23 11:22:38.507808 kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/__init__.py
+-rw-r--r--   0        0        0    14932 2023-06-23 11:22:39.091815 kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/kafka_schema_registry_admin.py
+-rw-r--r--   0        0        0     1560 2023-06-23 11:22:38.507808 kafka_schema_registry_admin-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.2.5/PKG-INFO
```

### Comparing `kafka-schema-registry-admin-0.2.4/LICENSE` & `kafka_schema_registry_admin-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-schema-registry-admin-0.2.4/README.rst` & `kafka_schema_registry_admin-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `kafka-schema-registry-admin-0.2.4/kafka_schema_registry_admin/kafka_schema_registry_admin.py` & `kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/kafka_schema_registry_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         :param bool permanent:
         """
         url = f"{self.SchemaRegistryUrl}/subjects/{subject_name}"
         if version_id:
             url = f"{url}/versions/{version_id}"
         LOG.debug(url)
         if self.Username:
-
             req = requests.delete(url, auth=(self.Username, self.Password))
             if permanent:
                 permanent_url = f"{url}?permanent=true"
                 req = requests.delete(
                     permanent_url, auth=(self.Username, self.Password)
                 )
         else:
```

### Comparing `kafka-schema-registry-admin-0.2.4/pyproject.toml` & `kafka_schema_registry_admin-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "kafka-schema-registry-admin"
-version = "0.2.4"
+version = "0.2.5"
 description = "Pure HTTP client to manage schemas in Schema Registry"
 authors = ["John Preston <john@ews-network.net>"]
 license = "LGPL-3.0-only"
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -15,36 +15,36 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.28.0"
 pydantic = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
+black = "^23.0"
 isort = "^5.10.1"
 coverage = "^6.4.1"
 Sphinx = "^5.0.2"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 tbump = "^6.9.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_schema_registry_admin"
 
 [tool.tbump.version]
-current = "0.2.4"
+current = "0.2.5"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka-schema-registry-admin-0.2.4/PKG-INFO` & `kafka_schema_registry_admin-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kafka-schema-registry-admin
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pure HTTP client to manage schemas in Schema Registry
 License: LGPL-3.0-only
 Author: John Preston
 Author-email: john@ews-network.net
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/x-rst
 
 ===========================
 Kafka schema registry admin
 ===========================
```

