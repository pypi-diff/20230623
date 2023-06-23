# Comparing `tmp/schematicpy-23.6.1.tar.gz` & `tmp/schematicpy-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-23.6.1.tar", max compression
+gzip compressed data, was "schematicpy-23.6.2.tar", max compression
```

## Comparing `schematicpy-23.6.1.tar` & `schematicpy-23.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1073 2023-06-15 23:22:47.239571 schematicpy-23.6.1/LICENSE
--rw-r--r--   0        0        0    16389 2023-06-15 23:22:47.239571 schematicpy-23.6.1/README.md
--rw-r--r--   0        0        0     3356 2023-06-15 23:23:20.580086 schematicpy-23.6.1/pyproject.toml
--rw-r--r--   0        0        0     1411 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/__main__.py
--rw-r--r--   0        0        0     4843 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/configuration.py
--rw-r--r--   0        0        0      663 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2023-06-15 23:22:47.239571 schematicpy-23.6.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3129 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/exceptions.py
--rw-r--r--   0        0        0    10598 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/help.py
--rw-r--r--   0        0        0     3415 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0     9375 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    74507 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    22894 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     6912 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/commands.py
--rw-r--r--   0        0        0    16680 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    44816 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    11604 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      166 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     2470 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/curie.py
--rw-r--r--   0        0        0    34388 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/df_parser.py
--rw-r--r--   0        0        0    46753 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/explorer.py
--rw-r--r--   0        0        0    30347 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/generator.py
--rw-r--r--   0        0        0     7100 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/schemas/validator.py
--rw-r--r--   0        0        0       96 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2023-06-15 23:22:47.247571 schematicpy-23.6.1/schematic/store/base.py
--rw-r--r--   0        0        0   113572 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/store/synapse.py
--rw-r--r--   0        0        0      787 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     4765 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2785 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     8086 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0     6338 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/general.py
--rw-r--r--   0        0        0     8197 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1148 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0     9804 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0     9565 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     2629 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      236 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/version.py
--rw-r--r--   0        0        0      135 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    10207 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     3480 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    37113 2023-06-15 23:22:47.251571 schematicpy-23.6.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    18820 1970-01-01 00:00:00.000000 schematicpy-23.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-23 14:49:46.042848 schematicpy-23.6.2/LICENSE
+-rw-r--r--   0        0        0    16389 2023-06-23 14:49:46.042848 schematicpy-23.6.2/README.md
+-rw-r--r--   0        0        0     3356 2023-06-23 14:50:32.786913 schematicpy-23.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1411 2023-06-23 14:49:46.042848 schematicpy-23.6.2/schematic/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-23 14:49:46.042848 schematicpy-23.6.2/schematic/__main__.py
+-rw-r--r--   0        0        0     4843 2023-06-23 14:49:46.042848 schematicpy-23.6.2/schematic/configuration.py
+-rw-r--r--   0        0        0      663 2023-06-23 14:49:46.042848 schematicpy-23.6.2/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2023-06-23 14:49:46.042848 schematicpy-23.6.2/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3129 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/exceptions.py
+-rw-r--r--   0        0        0    10598 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/help.py
+-rw-r--r--   0        0        0     3415 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/loader.py
+-rw-r--r--   0        0        0       59 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0     9375 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    74507 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    22894 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/models/__init__.py
+-rw-r--r--   0        0        0     6912 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/models/commands.py
+-rw-r--r--   0        0        0    16680 2023-06-23 14:49:46.050848 schematicpy-23.6.2/schematic/models/metadata.py
+-rw-r--r--   0        0        0    44816 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    11604 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      166 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     2470 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     4291 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/curie.py
+-rw-r--r--   0        0        0    34388 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/df_parser.py
+-rw-r--r--   0        0        0    46753 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/explorer.py
+-rw-r--r--   0        0        0    30347 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/generator.py
+-rw-r--r--   0        0        0     7100 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/schemas/validator.py
+-rw-r--r--   0        0        0       96 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/store/base.py
+-rw-r--r--   0        0        0   113572 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/store/synapse.py
+-rw-r--r--   0        0        0      787 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     4765 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     2785 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0     8086 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0     6338 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/general.py
+-rw-r--r--   0        0        0     8197 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1148 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0     9804 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0     9565 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     2629 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      236 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/version.py
+-rw-r--r--   0        0        0      135 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    10207 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     3480 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    37113 2023-06-23 14:49:46.054848 schematicpy-23.6.2/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    18820 1970-01-01 00:00:00.000000 schematicpy-23.6.2/PKG-INFO
```

### Comparing `schematicpy-23.6.1/LICENSE` & `schematicpy-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/README.md` & `schematicpy-23.6.2/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/pyproject.toml` & `schematicpy-23.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v23.6.1"
+version = "v23.6.2"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
```

### Comparing `schematicpy-23.6.1/schematic/__init__.py` & `schematicpy-23.6.2/schematic/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/__main__.py` & `schematicpy-23.6.2/schematic/__main__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/configuration.py` & `schematicpy-23.6.2/schematic/configuration.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/README.md` & `schematicpy-23.6.2/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-23.6.2/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-23.6.2/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-23.6.2/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-23.6.2/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-23.6.2/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/exceptions.py` & `schematicpy-23.6.2/schematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/help.py` & `schematicpy-23.6.2/schematic/help.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/loader.py` & `schematicpy-23.6.2/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/manifest/commands.py` & `schematicpy-23.6.2/schematic/manifest/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/manifest/generator.py` & `schematicpy-23.6.2/schematic/manifest/generator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/models/GE_Helpers.py` & `schematicpy-23.6.2/schematic/models/GE_Helpers.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/models/commands.py` & `schematicpy-23.6.2/schematic/models/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/models/metadata.py` & `schematicpy-23.6.2/schematic/models/metadata.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/models/validate_attribute.py` & `schematicpy-23.6.2/schematic/models/validate_attribute.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/models/validate_manifest.py` & `schematicpy-23.6.2/schematic/models/validate_manifest.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/commands.py` & `schematicpy-23.6.2/schematic/schemas/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/curie.py` & `schematicpy-23.6.2/schematic/schemas/curie.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/df_parser.py` & `schematicpy-23.6.2/schematic/schemas/df_parser.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/explorer.py` & `schematicpy-23.6.2/schematic/schemas/explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/generator.py` & `schematicpy-23.6.2/schematic/schemas/generator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/schemas/validator.py` & `schematicpy-23.6.2/schematic/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/store/synapse.py` & `schematicpy-23.6.2/schematic/store/synapse.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/__init__.py` & `schematicpy-23.6.2/schematic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/cli_utils.py` & `schematicpy-23.6.2/schematic/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/curie_utils.py` & `schematicpy-23.6.2/schematic/utils/curie_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/df_utils.py` & `schematicpy-23.6.2/schematic/utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/general.py` & `schematicpy-23.6.2/schematic/utils/general.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/google_api_utils.py` & `schematicpy-23.6.2/schematic/utils/google_api_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/io_utils.py` & `schematicpy-23.6.2/schematic/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/schema_utils.py` & `schematicpy-23.6.2/schematic/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/validate_rules_utils.py` & `schematicpy-23.6.2/schematic/utils/validate_rules_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/utils/validate_utils.py` & `schematicpy-23.6.2/schematic/utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/visualization/attributes_explorer.py` & `schematicpy-23.6.2/schematic/visualization/attributes_explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/visualization/commands.py` & `schematicpy-23.6.2/schematic/visualization/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/schematic/visualization/tangled_tree.py` & `schematicpy-23.6.2/schematic/visualization/tangled_tree.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.1/PKG-INFO` & `schematicpy-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 23.6.1
+Version: 23.6.2
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
```

