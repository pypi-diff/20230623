# Comparing `tmp/csvcubed-0.4.3-py3-none-any.whl.zip` & `tmp/csvcubed-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 224704 bytes, number of entries: 190
+Zip file size: 232523 bytes, number of entries: 195
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 csvcubed/README.md
 -rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 csvcubed/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/__init__.py
 -rw-r--r--  2.0 unx     2881 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/build.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/__init__.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/build_code_list.py
@@ -43,15 +43,17 @@
 -rw-r--r--  2.0 unx      380 b- defN 80-Jan-01 00:00 csvcubed/inspect/sparql_handler/sparql_queries/select_metadata_dependencies.sparql
 -rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 csvcubed/inspect/sparql_handler/sparql_queries/select_table_schema_properties.sparql
 -rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 csvcubed/inspect/sparql_handler/sparql_queries/select_units.sparql
 -rw-r--r--  2.0 unx    11705 b- defN 80-Jan-01 00:00 csvcubed/inspect/sparql_handler/sparqlquerymanager.py
 -rw-r--r--  2.0 unx    10276 b- defN 80-Jan-01 00:00 csvcubed/inspect/tableschema.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/__init__.py
--rw-r--r--  2.0 unx     8467 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_config.py
+-rw-r--r--  2.0 unx     3142 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_config_sort.py
+-rw-r--r--  2.0 unx     5103 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_configv1.py
+-rw-r--r--  2.0 unx     5132 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_configv2.py
 -rw-r--r--  2.0 unx    14542 b- defN 80-Jan-01 00:00 csvcubed/models/csvcubedexception.py
 -rw-r--r--  2.0 unx      409 b- defN 80-Jan-01 00:00 csvcubed/models/csvwtype.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/cube/__init__.py
 -rw-r--r--  2.0 unx      676 b- defN 80-Jan-01 00:00 csvcubed/models/cube/catalog.py
 -rw-r--r--  2.0 unx     1367 b- defN 80-Jan-01 00:00 csvcubed/models/cube/columns.py
 -rw-r--r--  2.0 unx     7486 b- defN 80-Jan-01 00:00 csvcubed/models/cube/cube.py
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 csvcubed/models/cube/cube_shape.py
@@ -94,20 +96,20 @@
 -rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 csvcubed/models/uriidentifiable.py
 -rw-r--r--  2.0 unx     3108 b- defN 80-Jan-01 00:00 csvcubed/models/validatedmodel.py
 -rw-r--r--  2.0 unx     3167 b- defN 80-Jan-01 00:00 csvcubed/models/validationerror.py
 -rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 csvcubed/readers/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/__init__.py
 -rw-r--r--  2.0 unx     1637 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py
--rw-r--r--  2.0 unx     6719 b- defN 80-Jan-01 00:00 csvcubed/readers/codelistconfig/codelist_schema_versions.py
+-rw-r--r--  2.0 unx     9002 b- defN 80-Jan-01 00:00 csvcubed/readers/codelistconfig/codelist_schema_versions.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/__init__.py
--rw-r--r--  2.0 unx     4878 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/schema_versions.py
+-rw-r--r--  2.0 unx     5122 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/schema_versions.py
 -rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/__init__.py
--rw-r--r--  2.0 unx    20180 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/columnschema.py
+-rw-r--r--  2.0 unx    21550 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/columnschema.py
 -rw-r--r--  2.0 unx    14157 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/configdeserialiser.py
 -rw-r--r--  2.0 unx      629 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/constants.py
 -rw-r--r--  2.0 unx     4071 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/datatypes.py
 -rw-r--r--  2.0 unx     9137 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1/mapcolumntocomponent.py
 -rw-r--r--  2.0 unx      182 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/readme.md
 -rw-r--r--  2.0 unx      911 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/README.md
 -rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/calendar-day.json
@@ -122,33 +124,36 @@
 -rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/government-half-year.json
 -rw-r--r--  2.0 unx      240 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/government-quarter.json
 -rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/government-week.json
 -rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/government-year.json
 -rw-r--r--  2.0 unx      233 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/gregorian-instant.json
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/gregorian-interval.json
 -rw-r--r--  2.0 unx      345 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/mixed-period.json
+-rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/observation-status-af.json
 -rw-r--r--  2.0 unx      144 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/observation-status.json
--rw-r--r--  2.0 unx      826 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json
+-rw-r--r--  2.0 unx      884 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json
 -rw-r--r--  2.0 unx       95 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/qudt-units.json
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 csvcubed/readers/cubeconfig/v1_0/templates/statistical-geography.json
 -rw-r--r--  2.0 unx     3942 b- defN 80-Jan-01 00:00 csvcubed/readers/preconfiguredtemplates.py
 -rw-r--r--  2.0 unx     1647 b- defN 80-Jan-01 00:00 csvcubed/schema/codelist-config/v1_0/codelistconfig-example.jsonc
 -rw-r--r--  2.0 unx     4941 b- defN 80-Jan-01 00:00 csvcubed/schema/codelist-config/v1_0/schema.json
 -rw-r--r--  2.0 unx     6597 b- defN 80-Jan-01 00:00 csvcubed/schema/codelist-config/v1_1/schema.json
+-rw-r--r--  2.0 unx     6602 b- defN 80-Jan-01 00:00 csvcubed/schema/codelist-config/v2_0/schema.json
 -rw-r--r--  2.0 unx    11497 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_0/qbconfig-example.jsonc
 -rw-r--r--  2.0 unx    23488 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_0/schema.json
 -rw-r--r--  2.0 unx    11153 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_1/qbconfig-example.jsonc
 -rw-r--r--  2.0 unx    25257 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_1/schema.json
 -rw-r--r--  2.0 unx    26394 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_2/schema.json
 -rw-r--r--  2.0 unx    31399 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_3/schema.json
 -rw-r--r--  2.0 unx    32992 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_4/schema.json
+-rw-r--r--  2.0 unx    32872 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_5/schema.json
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 csvcubed/utils/__init__.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 csvcubed/utils/cache.py
 -rw-r--r--  2.0 unx     2979 b- defN 80-Jan-01 00:00 csvcubed/utils/cli.py
--rw-r--r--  2.0 unx     6536 b- defN 80-Jan-01 00:00 csvcubed/utils/createlocalcopyresponse.py
+-rw-r--r--  2.0 unx     6998 b- defN 80-Jan-01 00:00 csvcubed/utils/createlocalcopyresponse.py
 -rw-r--r--  2.0 unx    13809 b- defN 80-Jan-01 00:00 csvcubed/utils/csvdataset.py
 -rw-r--r--  2.0 unx     3406 b- defN 80-Jan-01 00:00 csvcubed/utils/csvw.py
 -rw-r--r--  2.0 unx      453 b- defN 80-Jan-01 00:00 csvcubed/utils/datetime.py
 -rw-r--r--  2.0 unx     1488 b- defN 80-Jan-01 00:00 csvcubed/utils/dict.py
 -rw-r--r--  2.0 unx     1682 b- defN 80-Jan-01 00:00 csvcubed/utils/file.py
 -rw-r--r--  2.0 unx     1582 b- defN 80-Jan-01 00:00 csvcubed/utils/iterables.py
 -rw-r--r--  2.0 unx     4253 b- defN 80-Jan-01 00:00 csvcubed/utils/json.py
@@ -178,15 +183,15 @@
 -rw-r--r--  2.0 unx    22952 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/dsdtordfmodelshelper.py
 -rw-r--r--  2.0 unx     3597 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/newresourceurigenerator.py
 -rw-r--r--  2.0 unx    27378 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/urihelper.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/__init__.py
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/constants.py
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py
 -rw-r--r--  2.0 unx    20804 b- defN 80-Jan-01 00:00 csvcubed/writers/qbwriter.py
--rw-r--r--  2.0 unx     9470 b- defN 80-Jan-01 00:00 csvcubed/writers/skoscodelistwriter.py
+-rw-r--r--  2.0 unx     9528 b- defN 80-Jan-01 00:00 csvcubed/writers/skoscodelistwriter.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 csvcubed/writers/writerbase.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3970 b- defN 80-Jan-01 00:00 csvcubed-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    19080 b- defN 16-Jan-01 00:00 csvcubed-0.4.3.dist-info/RECORD
-190 files, 811767 bytes uncompressed, 193416 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3970 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    19635 b- defN 16-Jan-01 00:00 csvcubed-0.4.4.dist-info/RECORD
+195 files, 861439 bytes uncompressed, 200315 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -138,15 +138,21 @@
 
 Filename: csvcubed/models/__init__.py
 Comment: 
 
 Filename: csvcubed/models/codelistconfig/__init__.py
 Comment: 
 
-Filename: csvcubed/models/codelistconfig/code_list_config.py
+Filename: csvcubed/models/codelistconfig/code_list_config_sort.py
+Comment: 
+
+Filename: csvcubed/models/codelistconfig/code_list_configv1.py
+Comment: 
+
+Filename: csvcubed/models/codelistconfig/code_list_configv2.py
 Comment: 
 
 Filename: csvcubed/models/csvcubedexception.py
 Comment: 
 
 Filename: csvcubed/models/csvwtype.py
 Comment: 
@@ -375,14 +381,17 @@
 
 Filename: csvcubed/readers/cubeconfig/v1_0/templates/gregorian-interval.json
 Comment: 
 
 Filename: csvcubed/readers/cubeconfig/v1_0/templates/mixed-period.json
 Comment: 
 
+Filename: csvcubed/readers/cubeconfig/v1_0/templates/observation-status-af.json
+Comment: 
+
 Filename: csvcubed/readers/cubeconfig/v1_0/templates/observation-status.json
 Comment: 
 
 Filename: csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json
 Comment: 
 
 Filename: csvcubed/readers/cubeconfig/v1_0/templates/qudt-units.json
@@ -399,14 +408,17 @@
 
 Filename: csvcubed/schema/codelist-config/v1_0/schema.json
 Comment: 
 
 Filename: csvcubed/schema/codelist-config/v1_1/schema.json
 Comment: 
 
+Filename: csvcubed/schema/codelist-config/v2_0/schema.json
+Comment: 
+
 Filename: csvcubed/schema/cube-config/v1_0/qbconfig-example.jsonc
 Comment: 
 
 Filename: csvcubed/schema/cube-config/v1_0/schema.json
 Comment: 
 
 Filename: csvcubed/schema/cube-config/v1_1/qbconfig-example.jsonc
@@ -420,14 +432,17 @@
 
 Filename: csvcubed/schema/cube-config/v1_3/schema.json
 Comment: 
 
 Filename: csvcubed/schema/cube-config/v1_4/schema.json
 Comment: 
 
+Filename: csvcubed/schema/cube-config/v1_5/schema.json
+Comment: 
+
 Filename: csvcubed/utils/__init__.py
 Comment: 
 
 Filename: csvcubed/utils/cache.py
 Comment: 
 
 Filename: csvcubed/utils/cli.py
@@ -549,23 +564,23 @@
 
 Filename: csvcubed/writers/skoscodelistwriter.py
 Comment: 
 
 Filename: csvcubed/writers/writerbase.py
 Comment: 
 
-Filename: csvcubed-0.4.3.dist-info/LICENSE
+Filename: csvcubed-0.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: csvcubed-0.4.3.dist-info/METADATA
+Filename: csvcubed-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: csvcubed-0.4.3.dist-info/WHEEL
+Filename: csvcubed-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: csvcubed-0.4.3.dist-info/entry_points.txt
+Filename: csvcubed-0.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: csvcubed-0.4.3.dist-info/RECORD
+Filename: csvcubed-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## csvcubed/readers/codelistconfig/codelist_schema_versions.py

```diff
@@ -6,15 +6,16 @@
 """
 
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import Callable, List, Optional, Tuple, Union
 
-from csvcubed.models.codelistconfig.code_list_config import CodeListConfig
+from csvcubed.models.codelistconfig.code_list_configv1 import CodeListConfigV1
+from csvcubed.models.codelistconfig.code_list_configv2 import CodeListConfigV2
 from csvcubed.models.cube.qb.components.codelist import NewQbCodeList
 from csvcubed.models.jsonvalidationerrors import JsonSchemaValidationError
 from csvcubed.models.validationerror import ValidationError
 from csvcubed.readers.cubeconfig.utils import load_resource
 from csvcubed.utils.validators.schema import (
     map_to_internal_validation_errors,
     validate_dict_against_schema,
@@ -41,36 +42,47 @@
 """
 
 _v1_0_CODELIST_SCHEMA_URL = "https://purl.org/csv-cubed/code-list-config/v1.0"
 _v1_1_CODELIST_SCHEMA_URL = "https://purl.org/csv-cubed/code-list-config/v1.1"
 
 V1_CODELIST_SCHEMA_URL = "https://purl.org/csv-cubed/code-list-config/v1"  # v1 defaults to the latest minor version of v1.*.
 
+_v2_0_CODELIST_SCHEMA_URL = "https://purl.org/csv-cubed/code-list-config/v2.0"
+
+V2_CODELIST_SCHEMA_URL = "https://purl.org/csv-cubed/code-list-config/v2"  # v2 defaults to the latest minor version of v2.*.
 
 LATEST_V1_CODELIST_SCHEMA_URL = _v1_1_CODELIST_SCHEMA_URL
 """
     This holds the URL identifying the latest minor version of the V1 schema.
 
     When adding a new minor version to the V1 schema, you must update this variable.
 """
 
-LATEST_CODELIST_SCHEMA_URL = LATEST_V1_CODELIST_SCHEMA_URL
+LATEST_V2_CODELIST_SCHEMA_URL = _v2_0_CODELIST_SCHEMA_URL
+"""
+    This holds the URL identifying the latest minor version of the V2 schema.
+
+    When adding a new minor version to the V2 schema, you must update this variable.
+"""
+
+LATEST_CODELIST_SCHEMA_URL = LATEST_V2_CODELIST_SCHEMA_URL
 """
     This holds the URL identifying the latest version of the schema.
 
     When adding a new schema version, you must update this variable.
 """
 
 
 class CodeListConfigJsonSchemaMajorVersion(Enum):
     """
     Major versions of the code list config schema.
     """
 
     v1 = 1
+    v2 = 2
 
 
 class CodeListConfigJsonSchemaMinorVersion(Enum):
     """
     Minor versions of the code list config schema.
     """
 
@@ -83,19 +95,56 @@
     schema_version_minor: int,
 ) -> Tuple[NewQbCodeList, List[JsonSchemaValidationError], List[ValidationError]]:
     """Extract a code list form a JSON file and validate"""
 
     _logger.debug("Using schema minor version %s", schema_version_minor)
 
     if isinstance(code_list_config_path_or_dict, Path):
-        code_list_config, code_list_config_dict = CodeListConfig.from_json_file(
+        code_list_config, code_list_config_dict = CodeListConfigV1.from_json_file(
             code_list_config_path_or_dict
         )
     else:
-        code_list_config = CodeListConfig.from_dict(code_list_config_path_or_dict)
+        code_list_config = CodeListConfigV1.from_dict(code_list_config_path_or_dict)
+        code_list_config_dict = code_list_config_path_or_dict
+
+    schema = load_resource(code_list_config.schema)
+
+    unmapped_schema_validation_errors = validate_dict_against_schema(
+        value=code_list_config_dict, schema=schema
+    )
+
+    code_list_schema_validation_errors = map_to_internal_validation_errors(
+        schema, unmapped_schema_validation_errors
+    )
+
+    code_list = NewQbCodeList(
+        code_list_config.metadata, code_list_config.new_qb_concepts
+    )
+
+    return (
+        code_list,
+        code_list_schema_validation_errors,
+        code_list.validate(),  # type: ignore
+    )
+
+
+def _extract_and_validate_code_list_v2(
+    code_list_config_path_or_dict: Union[Path, dict],
+    schema_version_minor: int,
+) -> Tuple[NewQbCodeList, List[JsonSchemaValidationError], List[ValidationError]]:
+    """Extract a code list form a JSON file and validate"""
+
+    _logger.debug("Using schema minor version %s", schema_version_minor)
+
+    if isinstance(code_list_config_path_or_dict, Path):
+        code_list_config, code_list_config_dict = CodeListConfigV2.from_json_file(
+            code_list_config_path_or_dict
+        )
+    else:
+        code_list_config = CodeListConfigV2.from_dict(code_list_config_path_or_dict)
         code_list_config_dict = code_list_config_path_or_dict
 
     schema = load_resource(code_list_config.schema)
 
     unmapped_schema_validation_errors = validate_dict_against_schema(
         value=code_list_config_dict, schema=schema
     )
@@ -133,34 +182,46 @@
         schema_version_minor.value,
     )
 
     if schema_version_major == CodeListConfigJsonSchemaMajorVersion.v1:
         return lambda config_path_or_dict: _extract_and_validate_code_list_v1(
             config_path_or_dict, schema_version_minor.value
         )
+    elif schema_version_major == CodeListConfigJsonSchemaMajorVersion.v2:
+        return lambda config_path_or_dict: _extract_and_validate_code_list_v2(
+            config_path_or_dict, schema_version_minor.value
+        )
     else:
         raise ValueError(f"Unhandled major schema version {schema_version_major}")
 
 
 def _get_code_list_schema_version(
     schema_path: str,
 ) -> Tuple[CodeListConfigJsonSchemaMajorVersion, CodeListConfigJsonSchemaMinorVersion]:
     if schema_path == V1_CODELIST_SCHEMA_URL:
         schema_path = LATEST_V1_CODELIST_SCHEMA_URL
 
+    if schema_path == V2_CODELIST_SCHEMA_URL:
+        schema_path = LATEST_V2_CODELIST_SCHEMA_URL
+
     if schema_path == _v1_0_CODELIST_SCHEMA_URL:
         return (
             CodeListConfigJsonSchemaMajorVersion.v1,
             CodeListConfigJsonSchemaMinorVersion.v0,
         )
     elif schema_path == _v1_1_CODELIST_SCHEMA_URL:
         return (
             CodeListConfigJsonSchemaMajorVersion.v1,
             CodeListConfigJsonSchemaMinorVersion.v1,
         )
+    elif schema_path == _v2_0_CODELIST_SCHEMA_URL:
+        return (
+            CodeListConfigJsonSchemaMajorVersion.v2,
+            CodeListConfigJsonSchemaMinorVersion.v0,
+        )
     else:
         raise ValueError(
             f"The $schema '{schema_path}' referenced in the code list config file is not recognised. Please check for any updates to your csvcubed installation."
         )
 
 
 def get_code_list_versioned_deserialiser(
```

## csvcubed/readers/cubeconfig/schema_versions.py

```diff
@@ -34,25 +34,27 @@
 """
 
 _v1_0_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.0"
 _v1_1_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.1"
 _v1_2_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.2"
 _v1_3_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.3"
 _v1_4_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.4"
+_v1_5_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1.5"
+
 V1_SCHEMA_URL = "https://purl.org/csv-cubed/qube-config/v1"  # v1 defaults to the latest minor version of v1.*.
 
 
-_LATEST_V1_SCHEMA_URL = _v1_4_SCHEMA_URL
+_LATEST_V1_SCHEMA_URL = _v1_5_SCHEMA_URL
 """
     This holds the URL identifying the latest minor version of the V1 schema.
 
     When adding a new minor version to the V1 schema, you must update this variable.
 """
 
-_LATEST_SCHEMA_URL = _v1_4_SCHEMA_URL
+_LATEST_SCHEMA_URL = _v1_5_SCHEMA_URL
 """
     This holds the URL identifying the latest version of the schema.
 
     When adding a new schema version, you must update this variable.
 """
 
 
@@ -70,14 +72,15 @@
     """
 
     v0 = 0
     v1 = 1
     v2 = 2
     v3 = 3
     v4 = 4
+    v5 = 5
 
 
 def get_deserialiser_for_schema(
     maybe_schema_path: Optional[str],
 ) -> QubeConfigDeserialiser:
     """
     Provides a versioned deserialiser function appropriate to the referenced schema.
@@ -126,11 +129,16 @@
             QubeConfigJsonSchemaMinorVersion.v3,
         )
     elif schema_path == _v1_4_SCHEMA_URL:
         return (
             QubeConfigJsonSchemaMajorVersion.v1,
             QubeConfigJsonSchemaMinorVersion.v4,
         )
+    elif schema_path == _v1_5_SCHEMA_URL:
+        return (
+            QubeConfigJsonSchemaMajorVersion.v1,
+            QubeConfigJsonSchemaMinorVersion.v5,
+        )
     else:
         raise ValueError(
             f"The $schema '{schema_path}' referenced in the cube config file is not recognised. Please check for any updates to your csvcubed installation."
         )
```

## csvcubed/readers/cubeconfig/v1/columnschema.py

```diff
@@ -42,14 +42,15 @@
 from csvcubed.models.cube.qb.components.measuresdimension import QbMultiMeasureDimension
 from csvcubed.models.cube.qb.components.observedvalue import QbObservationValue
 from csvcubed.models.cube.qb.components.unit import ExistingQbUnit, NewQbUnit
 from csvcubed.models.cube.qb.components.unitscolumn import QbMultiUnits
 from csvcubed.models.jsonvalidationerrors import JsonSchemaValidationError
 from csvcubed.readers.codelistconfig.codelist_schema_versions import (
     LATEST_V1_CODELIST_SCHEMA_URL,
+    LATEST_V2_CODELIST_SCHEMA_URL,
 )
 from csvcubed.utils.file import code_list_config_json_exists
 from csvcubed.utils.uri import csvw_column_name_safe, looks_like_uri
 
 _logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=object)
@@ -113,14 +114,15 @@
         if isinstance(self.code_list, str):
             if looks_like_uri(self.code_list):
                 return (ExistingQbCodeList(self.code_list), [])
             # The following elif is for cube config v1.1. This also requires the user to define the configuration in the build command, and therefore cube_config_path.
             elif (
                 cube_config_minor_version
                 and cube_config_minor_version >= 1
+                and cube_config_minor_version < 5
                 and cube_config_path
                 and code_list_config_json_exists(
                     Path(self.code_list), cube_config_path.parent
                 )
             ):
                 code_list_path = Path(self.code_list)
                 code_list_config_path = (
@@ -140,14 +142,44 @@
                 (
                     new_code_list,
                     json_schema_validation_errors,
                     _,
                 ) = deserialiser(code_list_config_path)
 
                 return (new_code_list, json_schema_validation_errors)
+            elif (
+                cube_config_minor_version
+                and cube_config_minor_version >= 5
+                and cube_config_path
+                and code_list_config_json_exists(
+                    Path(self.code_list), cube_config_path.parent
+                )
+            ):
+                code_list_path = Path(self.code_list)
+                code_list_config_path = (
+                    code_list_path
+                    if code_list_path.is_absolute()
+                    else (cube_config_path.parent / code_list_path).resolve()
+                )
+                _logger.info(
+                    f"Loading code list from local file path: {code_list_config_path}"
+                )
+
+                deserialiser = get_code_list_versioned_deserialiser(
+                    code_list_config_path,
+                    default_schema_uri=LATEST_V2_CODELIST_SCHEMA_URL,
+                )
+
+                (
+                    new_code_list,
+                    json_schema_validation_errors,
+                    _,
+                ) = deserialiser(code_list_config_path)
+
+                return (new_code_list, json_schema_validation_errors)
             else:
                 raise ValueError(
                     "Code List contains a string that cannot be recognised as a URI or a valid File Path"
                 )
 
         elif isinstance(self.code_list, bool):
             if self.code_list is False:
@@ -173,15 +205,18 @@
         # The following elif is for cube config v1.1 and when the code list is defined inline.
         elif (
             cube_config_minor_version
             and cube_config_minor_version >= 1
             and isinstance(self.code_list, dict)
         ):
             deserialiser = get_code_list_versioned_deserialiser(
-                self.code_list, default_schema_uri=LATEST_V1_CODELIST_SCHEMA_URL
+                self.code_list,
+                default_schema_uri=LATEST_V1_CODELIST_SCHEMA_URL
+                if cube_config_minor_version < 5
+                else LATEST_V2_CODELIST_SCHEMA_URL,
             )
 
             (
                 new_code_list,
                 json_schema_validation_errors,
                 _,
             ) = deserialiser(self.code_list)
```

## csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json

### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'obseration-status-af'": "'observation-status-af.json'"}*

```diff
@@ -7,14 +7,15 @@
     "gregorian-instant": "gregorian-instant.json",
     "gregorian-interval": "gregorian-interval.json",
     "half-year": "calendar-half-year.json",
     "hour": "calendar-hour.json",
     "minute": "calendar-minute.json",
     "mixed-period": "mixed-period.json",
     "month": "calendar-month.json",
+    "obseration-status-af": "observation-status-af.json",
     "observation-status": "observation-status.json",
     "quarter": "calendar-quarter.json",
     "qudt": "qudt-units.json",
     "second": "calendar-seconds.json",
     "statistical-geography": "statistical-geography.json",
     "week": "calendar-week.json",
     "year": "calendar-year.json"
```

## csvcubed/utils/createlocalcopyresponse.py

```diff
@@ -34,34 +34,49 @@
     / "v1_3"
     / "schema.json",
     "//purl.org/csv-cubed/qube-config/v1.4": APP_ROOT_DIR_PATH
     / "schema"
     / "cube-config"
     / "v1_4"
     / "schema.json",
+    "//purl.org/csv-cubed/qube-config/v1.5": APP_ROOT_DIR_PATH
+    / "schema"
+    / "cube-config"
+    / "v1_5"
+    / "schema.json",
     "//purl.org/csv-cubed/qube-config/v1": APP_ROOT_DIR_PATH
     / "schema"
     / "cube-config"
-    / "v1_4"
+    / "v1_5"
     / "schema.json",  # v1 defaults to latest minor version of v1.*.
-    "//purl.org/csv-cubed/codelist-config/v1.0": APP_ROOT_DIR_PATH
+    "//purl.org/csv-cubed/code-list-config/v1.0": APP_ROOT_DIR_PATH
     / "schema"
     / "codelist-config"
     / "v1_0"
     / "schema.json",
-    "//purl.org/csv-cubed/codelist-config/v1.1": APP_ROOT_DIR_PATH
+    "//purl.org/csv-cubed/code-list-config/v1.1": APP_ROOT_DIR_PATH
     / "schema"
     / "codelist-config"
     / "v1_1"
     / "schema.json",
+    "//purl.org/csv-cubed/code-list-config/v2.0": APP_ROOT_DIR_PATH
+    / "schema"
+    / "codelist-config"
+    / "v2_0"
+    / "schema.json",
     "//purl.org/csv-cubed/code-list-config/v1": APP_ROOT_DIR_PATH
     / "schema"
     / "codelist-config"
     / "v1_1"
     / "schema.json",  # v1 defaults to latest minor version of v1.*.
+    "//purl.org/csv-cubed/code-list-config/v2": APP_ROOT_DIR_PATH
+    / "schema"
+    / "codelist-config"
+    / "v2_0"
+    / "schema.json",  # v2 defaults to latest minor version of v2.*.
 }
 
 
 def _get_url_to_file_path_map() -> Dict[str, Path]:
     """
     Dynamically adds template URLs + corresponding files to the hardcoded map:
     _hard_coded_map_url_to_file_path for use in schema mocking and when a local
```

## csvcubed/writers/skoscodelistwriter.py

```diff
@@ -146,15 +146,15 @@
             )
 
             csvw_columns.append(
                 {
                     "titles": "Original Concept URI",
                     "name": "uri",
                     "required": True,
-                    "propertyUrl": "owl:sameAs",
+                    "propertyUrl": "skos:exactMatch",
                     "valueUrl": "{+uri}",
                 }
             )
 
         csvw_columns.append(
             {
                 "virtual": True,
@@ -171,14 +171,15 @@
                 "name": "virt_type",
                 "required": True,
                 "propertyUrl": "rdf:type",
                 "valueUrl": "skos:Concept",
             }
         )
         return {
+            "@context": "http://www.w3.org/ns/csvw",
             "columns": csvw_columns,
             "aboutUrl": self.uri_helper.get_concept_uri("{+uri_identifier}"),
             "primaryKey": "uri_identifier",
         }
 
     def _get_csvw_metadata(self) -> dict:
         scheme_uri = self.uri_helper.get_scheme_uri()
```

## Comparing `csvcubed-0.4.3.dist-info/LICENSE` & `csvcubed-0.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csvcubed-0.4.3.dist-info/METADATA` & `csvcubed-0.4.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvcubed
-Version: 0.4.3
+Version: 0.4.4
 Summary: A tool to generate RDF Data Cube style CSV-W cubes from tidy CSV files. Part of the csvcubed family.
 License: Apache-2.0
 Author: Integrated Data Service - Dissemination
 Author-email: csvcubed@gsscogs.uk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `csvcubed-0.4.3.dist-info/RECORD` & `csvcubed-0.4.4.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 csvcubed/inspect/sparql_handler/sparql_queries/select_metadata_dependencies.sparql,sha256=548FykAbWj7DcD5Z3uipo289LcmKJoIhxcUMx-ODztI,380
 csvcubed/inspect/sparql_handler/sparql_queries/select_table_schema_properties.sparql,sha256=2al7ZhCLHtPEVkvubzigAlmrTuT5AHup5B6WtoQxzBw,466
 csvcubed/inspect/sparql_handler/sparql_queries/select_units.sparql,sha256=yGmTqCiseRgr8rSTuvoQlhEZWZruzdyP-iiFQFdCMhc,361
 csvcubed/inspect/sparql_handler/sparqlquerymanager.py,sha256=r-HncGkcL24sKjMTIJ9sDaDVs7ndghDyKmHP5DfBKE0,11705
 csvcubed/inspect/tableschema.py,sha256=dcK4aelSwY43zKpg4GZLkr-KCahEMWX9UBfYI93CRPg,10276
 csvcubed/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/codelistconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/models/codelistconfig/code_list_config.py,sha256=dkPPoTyazqpYPuOJ2jUzCOL1DIDu16EveiqOEstLUSQ,8467
+csvcubed/models/codelistconfig/code_list_config_sort.py,sha256=0i9-NPwSVqNBjatLwxbAzrH50xgnUB9A5KSRFm-YaEk,3142
+csvcubed/models/codelistconfig/code_list_configv1.py,sha256=_NS2RtPQKt4lrxckDW4laT_SynRrt6WdHEekANHoJpc,5103
+csvcubed/models/codelistconfig/code_list_configv2.py,sha256=Y-ONWbYIems9IlPNuJhRUUisPdAsxQaxTGsF8FVB56U,5132
 csvcubed/models/csvcubedexception.py,sha256=cfE3N-06CZ_bjMJV5gZ4KK6JLuFdq7Jcbe4uZiA-Krc,14542
 csvcubed/models/csvwtype.py,sha256=7WXT5EcWT48YNFn3oyPJkgPKRDPoyJZZrXHvaeWC6Jk,409
 csvcubed/models/cube/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/cube/catalog.py,sha256=9AX4wIIglrjSTkhUI2YmzbLv_D9Z4rmz11bTMN74occ,676
 csvcubed/models/cube/columns.py,sha256=Abm4LtHqIy1Xa1HWiZfSXluCpETcVIYkwhdkLORUVe8,1367
 csvcubed/models/cube/cube.py,sha256=yf8MhAfUzCgF1aUIwL83cJO69QbGyyR8Z8D0gaD8R28,7486
 csvcubed/models/cube/cube_shape.py,sha256=rKamnT0oyVesazKlQnCt2jYMHVeCIoG6kc3H34bTlms,234
@@ -93,20 +95,20 @@
 csvcubed/models/uriidentifiable.py,sha256=tP9hBDJj7LIUMjdvO7mc2PYNKOCmu8NjSt_2XFtpIFw,1814
 csvcubed/models/validatedmodel.py,sha256=IcRFWUvmXO839gU1HCLQ8h41_CGqkdSe8mfBD2uvD9Q,3108
 csvcubed/models/validationerror.py,sha256=uDx5TPS_VcZZT790HM_V_hlkKnRj19-YIJrBIJnfrEY,3167
 csvcubed/readers/__init__.py,sha256=j-b06j5EDS5IAqkd7FkyGb9TV-KLDyGB0_g65LnaoEA,110
 csvcubed/readers/catalogmetadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/catalogmetadata/v1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py,sha256=BqmMn8wEc5KCcAhtCkXfNr78BZe6bRvKAywQ5m_gMgY,1637
-csvcubed/readers/codelistconfig/codelist_schema_versions.py,sha256=tbCSAiFKIHPdgOQeAL2DxCnETllJZ2RYXAO0YAznVbg,6719
+csvcubed/readers/codelistconfig/codelist_schema_versions.py,sha256=fumfdasXOzB-u_kLd3AH_V5-JxSBShcbxI8GviM4ir4,9002
 csvcubed/readers/cubeconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/readers/cubeconfig/schema_versions.py,sha256=DRtWlYhy6QbBJyrmfdtIVhvDuvceujjLC5-F85wG9aY,4878
+csvcubed/readers/cubeconfig/schema_versions.py,sha256=mdwlHafjhOhXlnyOCzTB4cBYBce8vcTlXcNJ8Ez9lvE,5122
 csvcubed/readers/cubeconfig/utils.py,sha256=CCq1Fu5SbGPSi02MPLsR-08tje0ByK5wc3xw5_esRGc,1814
 csvcubed/readers/cubeconfig/v1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/readers/cubeconfig/v1/columnschema.py,sha256=Jvs-dINoRDfGOffaUxGHM-VI9Rf1NwSbYJOvV9attyc,20180
+csvcubed/readers/cubeconfig/v1/columnschema.py,sha256=o4-wcPpC6PQlZeg1URb3QRe-FW0MVaMNEwVVLISkY0Y,21550
 csvcubed/readers/cubeconfig/v1/configdeserialiser.py,sha256=QstbhGGcOrbSHnC8YJe4ZzUdK9rDx8xzla4mZGTedfQ,14157
 csvcubed/readers/cubeconfig/v1/constants.py,sha256=gUVnAVgrNF3HLlBn4MuEYPsIcDsD_Tjt5-GOSHyPtpE,629
 csvcubed/readers/cubeconfig/v1/datatypes.py,sha256=ORpESm5zGMUjLa78MZzxNUeSqj75DxPz5jeeoiGkeLo,4071
 csvcubed/readers/cubeconfig/v1/mapcolumntocomponent.py,sha256=Pkx0sPoNg7o4WOELVPBNkwd5y-b26Idyjjzc0VloQks,9137
 csvcubed/readers/cubeconfig/v1_0/readme.md,sha256=PlZMtxW93oA89UzwpvukvgpdB9bKoTz-EzDf4bk6I3M,182
 csvcubed/readers/cubeconfig/v1_0/templates/README.md,sha256=7o-Osoki8FBzRiU9sdTAfBlf5S1GUsbInHubMZKpaaI,911
 csvcubed/readers/cubeconfig/v1_0/templates/calendar-day.json,sha256=oXr64AxuPOMSOMYTGDTY432C8t3vCEq8mBUpFPYeoSM,210
@@ -121,33 +123,36 @@
 csvcubed/readers/cubeconfig/v1_0/templates/government-half-year.json,sha256=rv98YUJONBkj3H2pBZoZJ_mJHKWRiYOSDeYXk0Yf83c,239
 csvcubed/readers/cubeconfig/v1_0/templates/government-quarter.json,sha256=v4abW1zLWfAOUIEr7NeJwWxwC-FjiA1csW0VnPHn4A0,240
 csvcubed/readers/cubeconfig/v1_0/templates/government-week.json,sha256=t8-oIAHCx4eEtuDzwQdMbqg8G7_mblU-1wPFkTvhmKI,235
 csvcubed/readers/cubeconfig/v1_0/templates/government-year.json,sha256=lV7usWk3L8dfqG8kd9nPgBzAjCPZcnjieq8wkLRoiwg,235
 csvcubed/readers/cubeconfig/v1_0/templates/gregorian-instant.json,sha256=IM--tPQUyAN7Ai1b6rN5p1WvWTZDSrJ8JJwFeFR6rGs,233
 csvcubed/readers/cubeconfig/v1_0/templates/gregorian-interval.json,sha256=ihhKRmq_E6Gi0W2vXeJWMiMujKaU_QRPjvbhEbMrpyE,246
 csvcubed/readers/cubeconfig/v1_0/templates/mixed-period.json,sha256=dqpS-QJssrush8vyteqG7ciQUnaXNymn4E-zQkKFuZ8,345
+csvcubed/readers/cubeconfig/v1_0/templates/observation-status-af.json,sha256=F-XmCTfFUCWmI5vzdO3S87h__VlG18XmvXnOWQoZgmg,258
 csvcubed/readers/cubeconfig/v1_0/templates/observation-status.json,sha256=Xfv63Q9Ssxjs8mrkCr8XXVd-XEXowXodEMx4IQu29yQ,144
-csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json,sha256=eCm3uwehDw-TFKI2D_ugpWoZ97vWU0oVOBrVjO-F2BM,826
+csvcubed/readers/cubeconfig/v1_0/templates/preset_column_config.json,sha256=3Ky3jzrUNNYu8JyR8-imACJ3j4QI_aqbuvyOEnD_5JI,884
 csvcubed/readers/cubeconfig/v1_0/templates/qudt-units.json,sha256=-lQlgBb_UyivCva9E1kSZMq8TqBRmgTMlbFXu_25k3s,95
 csvcubed/readers/cubeconfig/v1_0/templates/statistical-geography.json,sha256=wRReh4FU_28Bl09JJ-VIKOUcZgfRYGXL3k_RetblVIw,270
 csvcubed/readers/preconfiguredtemplates.py,sha256=CL8wTOdSmf375Dm-nhvxEqokNmRX8-CE4tqko779TXU,3942
 csvcubed/schema/codelist-config/v1_0/codelistconfig-example.jsonc,sha256=zZUZAVxewdxpRt5e_jF6UzrGsIZ7cxzxqPctuAMCRyU,1647
 csvcubed/schema/codelist-config/v1_0/schema.json,sha256=SoCAdfcZO9439MAFjF_BYp2P96eF8n1K03I7BYj9dpg,4941
 csvcubed/schema/codelist-config/v1_1/schema.json,sha256=YvxsuNZjk8SWokh6aUpifABYFiDi6TmbNiqrl8S6mrM,6597
+csvcubed/schema/codelist-config/v2_0/schema.json,sha256=OfV_bUYYrFYhKZbdpeYLHl1qbMtMjj7YUWFhaeZyPRw,6602
 csvcubed/schema/cube-config/v1_0/qbconfig-example.jsonc,sha256=UgF3Yn7oybxWF4pYnNr-o78uBRMIqbwQG1yfRCsm6Nc,11497
 csvcubed/schema/cube-config/v1_0/schema.json,sha256=j6WWPxsgLsm8MriX61-KfZmxakji91HsilAi5SQQwKE,23488
 csvcubed/schema/cube-config/v1_1/qbconfig-example.jsonc,sha256=dpmKT0QeJOs-QntgUGHGr23lgqIEj93gpWa8NkUNlfo,11153
 csvcubed/schema/cube-config/v1_1/schema.json,sha256=SfM5ceL8lxeouVyko03CB09sIfydh9qqH0DMqKT7J28,25257
 csvcubed/schema/cube-config/v1_2/schema.json,sha256=1zuVO6WXBXRL-TZtMWgAWbhHrfjwcCwXNUO0z2jIDyk,26394
 csvcubed/schema/cube-config/v1_3/schema.json,sha256=vNobTvct1s70-XmovUf2kHhJ5v7t_A0ZKiLJo6Psck4,31399
 csvcubed/schema/cube-config/v1_4/schema.json,sha256=6CaymYv-yIMNpNAlPMpHZXPUUM7qOxKx22PRvBfi-IM,32992
+csvcubed/schema/cube-config/v1_5/schema.json,sha256=1PoaqMnE1SWKCvQHUxw-eqyeqo5DdjiZg8kEyEklPzQ,32872
 csvcubed/utils/__init__.py,sha256=GEljQsipGps0CgGfOBUMnoAeFqnQbZkZzfb86R96ZpQ,67
 csvcubed/utils/cache.py,sha256=FJtD-pWfWE7AVFYW36V1lpm5iw377cX4Z5H3YUIU07M,356
 csvcubed/utils/cli.py,sha256=az8WpfljZdlffBMpuYZ8FtCXhl8u_uGlCXMsma01WnQ,2979
-csvcubed/utils/createlocalcopyresponse.py,sha256=w2vD5f9DnW_D_9VwWP_MfEMro5bpmX77qXkJzmhAsgs,6536
+csvcubed/utils/createlocalcopyresponse.py,sha256=fnn2uS6Geiye_OdL5gSRZStl3x2ThYvTii6HCkfo83A,6998
 csvcubed/utils/csvdataset.py,sha256=cyeWql85rJnNlHGF62SxYk78FIeRSduSaS1hIBrN-a4,13809
 csvcubed/utils/csvw.py,sha256=iVexgf1UFgEFFoNHMkc5mlb9b3eAODzz59qfIUyT0m4,3406
 csvcubed/utils/datetime.py,sha256=VaammJPt10PUuN4qGgsntobgbCKUOIoqNNEwpDHWtRA,453
 csvcubed/utils/dict.py,sha256=YlhEoyBELSrKcS0dd42b7SMBSHX7Eh0R1uV4cabXU8M,1488
 csvcubed/utils/file.py,sha256=9q_7i8MPriBdggvHCFIY2VYgeoiFru4kGyWWJ2Nb9F0,1682
 csvcubed/utils/iterables.py,sha256=cP-wcLYUj-M1QNc9ysnt7l_ILYPd-nMY9IzXPqG4WDA,1582
 csvcubed/utils/json.py,sha256=qg29-TkmSa9myqz1SHi6mUTsKCNCsmCx4Z4hmHLw9gs,4253
@@ -177,14 +182,14 @@
 csvcubed/writers/helpers/qbwriter/dsdtordfmodelshelper.py,sha256=3hVEeqJ_txmCO7yOnLkOqCWtQB5tRRP1no80p3zAyv4,22952
 csvcubed/writers/helpers/qbwriter/newresourceurigenerator.py,sha256=yuwI8enmByK3xNFQ6c8v7q2kxJ5Bv4hPA3uiTja2Jw0,3597
 csvcubed/writers/helpers/qbwriter/urihelper.py,sha256=BzVnUueyoE1DBncTByKnigeLozePdfFRfxzaguwCtxY,27378
 csvcubed/writers/helpers/skoscodelistwriter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/writers/helpers/skoscodelistwriter/constants.py,sha256=FjVa2JsAc7uIxzQOJgNg3zf8Ha-YZvMzF75sqq_e93g,157
 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py,sha256=DWkL2zO4QsLV8Oo-nVXxS4cxA1ic4stSBp7NZpClbps,2437
 csvcubed/writers/qbwriter.py,sha256=fDesUmhWU1211z_wDQi8xFdfpB0CqdSHG7pM-YlsJQc,20804
-csvcubed/writers/skoscodelistwriter.py,sha256=dCK3RaOrv4jeD6l4SZ2PT9tr8zqZwR2x8kbRTsASIMc,9470
+csvcubed/writers/skoscodelistwriter.py,sha256=-ROyhtzqbZjss4XjQkzhQvdjG51oIlkDgOclA3e28uU,9528
 csvcubed/writers/writerbase.py,sha256=lzEHMgqdWBIFbxthYjf5JuE3i5gp5Vbb1Xw359TY3to,283
-csvcubed-0.4.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-csvcubed-0.4.3.dist-info/METADATA,sha256=kot3vebo4vqkz5cCYbWBcj2mMxo3tNzEeF-2LO3_5Co,3970
-csvcubed-0.4.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-csvcubed-0.4.3.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
-csvcubed-0.4.3.dist-info/RECORD,,
+csvcubed-0.4.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+csvcubed-0.4.4.dist-info/METADATA,sha256=sVZSsopkHs7Vq6NNT9UyP0LwCPubjnhaoaKp21YNVAY,3970
+csvcubed-0.4.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+csvcubed-0.4.4.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
+csvcubed-0.4.4.dist-info/RECORD,,
```

