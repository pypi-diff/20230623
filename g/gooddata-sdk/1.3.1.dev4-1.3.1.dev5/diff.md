# Comparing `tmp/gooddata-sdk-1.3.1.dev4.tar.gz` & `tmp/gooddata-sdk-1.3.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-sdk-1.3.1.dev4.tar", last modified: Mon Jun  5 07:30:34 2023, max compression
+gzip compressed data, was "gooddata-sdk-1.3.1.dev5.tar", last modified: Fri Jun 23 15:18:33 2023, max compression
```

## Comparing `gooddata-sdk-1.3.1.dev4.tar` & `gooddata-sdk-1.3.1.dev5.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.528478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.532478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/catalog_service_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.532478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.532478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.536478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.536478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/sql_column.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.536478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.536478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.540478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.540478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.540478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/validation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/validation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.540478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.540478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.544478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/entity_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.544478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.544478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.544478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.548478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.548478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/content_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/model_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    42651 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.532478 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-05 07:30:34.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-05 07:30:34.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:30:34.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 07:30:34.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 07:30:34.000000 gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-05 07:30:26.000000 gooddata-sdk-1.3.1.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:34.552478 gooddata-sdk-1.3.1.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-05 07:30:16.000000 gooddata-sdk-1.3.1.dev4/tests/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/catalog_service_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/sql_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.322357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/content_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.326357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42925 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.318357 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:18:33.000000 gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-23 15:18:25.000000 gooddata-sdk-1.3.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:33.330357 gooddata-sdk-1.3.1.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-23 15:18:17.000000 gooddata-sdk-1.3.1.dev5/tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.3.1.dev4/LICENSE.txt` & `gooddata-sdk-1.3.1.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/PKG-INFO` & `gooddata-sdk-1.3.1.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev4
+Version: 1.3.1.dev5
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev4
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev5
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-sdk-1.3.1.dev4/README.md` & `gooddata-sdk-1.3.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/__init__.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/base.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/catalog_service_base.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/catalog_service_base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/data_source.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/entity_model/data_source.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/entity_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/data_source/validation/data_source.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/data_source/validation/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/entity.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/entity.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/request.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/export/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/export/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/identifier.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/identifier.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/entity_model/organization.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/entity_model/organization.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/organization/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/organization/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/declarative_model/permission.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/declarative_model/permission.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/permission/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/permission/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/setting.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/declarative_model/user_group.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/declarative_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/user.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/entity_model/user_group.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/entity_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/user/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/user/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/content_service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/content_service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/entity_model/workspace.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/entity_model/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/model_container.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/model_container.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/catalog/workspace/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/catalog/workspace/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,35 +573,38 @@
             translated = {}
             for x in to_translate:
                 translated[x] = x
             write_layout_to_file(translation_file_path, translated)
         return translated
 
     @staticmethod
-    def add_title_description(to_translate: Set[str], title: str, description: Optional[str]) -> None:
-        to_translate.add(title)
+    def add_title_description(to_translate: Set[str], title: Optional[str], description: Optional[str]) -> None:
+        if title:
+            to_translate.add(title)
         if description:
             to_translate.add(description)
 
     def add_title_description_tags(
-        self, to_translate: Set[str], title: str, description: Optional[str], tags: Optional[List[str]]
+        self, to_translate: Set[str], title: Optional[str], description: Optional[str], tags: Optional[List[str]]
     ) -> None:
         self.add_title_description(to_translate, title, description)
         if tags:
             to_translate.update(set(tags))
 
     @staticmethod
     def set_title_description(workspace_object: Any, translated: Dict[str, str]) -> None:
-        workspace_object.title = translated[workspace_object.title]
+        if workspace_object.title:
+            workspace_object.title = translated[workspace_object.title]
         if workspace_object.description:
             workspace_object.description = translated[workspace_object.description]
 
     def set_title_description_tags(self, workspace_object: Any, translated: Dict[str, str]) -> None:
         self.set_title_description(workspace_object, translated)
-        workspace_object.tags = [translated[x] for x in workspace_object.tags]
+        if workspace_object.tags:
+            workspace_object.tags = [translated[x] for x in workspace_object.tags]
 
     def get_texts_to_translate(
         self,
         workspace: CatalogWorkspace,
         workspace_content: CatalogDeclarativeWorkspaceModel,
         already_translated: Dict[str, str],
     ) -> Set[str]:
@@ -635,20 +638,20 @@
                             if "alias" in item["measure"]:
                                 to_translate.add(item["measure"]["alias"])
             for dashboard in workspace_content.analytics.analytical_dashboards or []:
                 self.add_title_description(to_translate, dashboard.title, dashboard.description)
                 # Hack: translate titles in free-form, which is not processed intentionally by this SDK
                 for section in dashboard.content["layout"]["sections"]:
                     for item in section["items"]:
-                        title = item["widget"]["title"]
-                        description = item["widget"]["description"]
+                        title = item["widget"].get("title")
+                        description = item["widget"].get("description")
                         self.add_title_description(to_translate, title, description)
                     if "header" in section:
-                        title = section["header"]["title"]
-                        description = section["header"]["description"]
+                        title = section["header"].get("title")
+                        description = section["header"].get("description")
                         self.add_title_description(to_translate, title, description)
 
         # Translate texts, which have not been translated yet
         if already_translated:
             to_translate = to_translate - set(already_translated.keys())
         return to_translate
 
@@ -689,21 +692,23 @@
                             if "alias" in item["measure"]:
                                 item["measure"]["alias"] = translated[item["measure"]["alias"]]
             for dashboard in new_workspace_content.analytics.analytical_dashboards or []:
                 self.set_title_description(dashboard, translated)
                 # Hack: translate titles in free-form, which is not processed intentionally by this SDK
                 for section in dashboard.content["layout"]["sections"]:
                     for item in section["items"]:
-                        item["widget"]["title"] = translated[item["widget"]["title"]]
-                        if item["widget"]["description"]:
-                            item["widget"]["description"] = translated[item["widget"]["description"]]
+                        if "title" in item["widget"]:
+                            item["widget"]["title"] = translated.get(item["widget"]["title"])
+                        if "description" in item["widget"]:
+                            item["widget"]["description"] = translated.get(item["widget"]["description"])
                     if "header" in section:
-                        section["header"]["title"] = translated[section["header"]["title"]]
-                        if section["header"]["description"]:
-                            section["header"]["description"] = translated[section["header"]["description"]]
+                        if "title" in section["header"]:
+                            section["header"]["title"] = translated.get(section["header"]["title"])
+                        if "description" in section["header"]:
+                            section["header"]["description"] = translated.get(section["header"]["description"])
 
     # Declarative methods - workspace data filters
 
     def get_declarative_workspace_data_filters(self) -> CatalogDeclarativeWorkspaceDataFilters:
         """Retrieve a workspace data filers layout.
 
         Args:
```

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/client.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/attribute.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/attribute.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/base.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/execution.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/execution.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/filter.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/model/metric.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/model/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/compute/service.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/compute/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/insight.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/insight.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/sdk.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/support.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/support.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/table.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/type_converter.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/type_converter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk/utils.py` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/PKG-INFO` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev4
+Version: 1.3.1.dev5
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev4
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev5
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-sdk-1.3.1.dev4/gooddata_sdk.egg-info/SOURCES.txt` & `gooddata-sdk-1.3.1.dev5/gooddata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev4/setup.py` & `gooddata-sdk-1.3.1.dev5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-api-client~=1.3.1.dev4",
+    "gooddata-api-client~=1.3.1.dev5",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
     "python-dateutil>=2.5.3",
     "pyyaml>=5.1",
     "attrs==21.4.0",
     "cattrs==22.1.0",
     "brotli==1.0.9",
 ]
 
 
 setup(
     name="gooddata-sdk",
     description="GoodData.CN Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev4",
+    version="1.3.1.dev5",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.7.0",
     project_urls={
-        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3.1.dev4",
+        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3.1.dev5",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

### Comparing `gooddata-sdk-1.3.1.dev4/tests/test_type_converter.py` & `gooddata-sdk-1.3.1.dev5/tests/test_type_converter.py`

 * *Files identical despite different names*

