# Comparing `tmp/qdrant_client-1.2.0.tar.gz` & `tmp/qdrant_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.2.0.tar", max compression
+gzip compressed data, was "qdrant_client-1.3.0.tar", max compression
```

## Comparing `qdrant_client-1.2.0.tar` & `qdrant_client-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    11357 2023-05-24 09:08:26.469326 qdrant_client-1.2.0/LICENSE
--rw-r--r--   0        0        0     6250 2023-05-24 09:08:26.469326 qdrant_client-1.2.0/README.md
--rw-r--r--   0        0        0     1391 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/__init__.py
--rw-r--r--   0        0        0     9904 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/client_base.py
--rw-r--r--   0        0        0     9742 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3364 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    68611 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    36463 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     2063 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    16916 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    53062 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2907 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    30011 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-05-24 09:08:26.473326 qdrant_client-1.2.0/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    38894 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    66445 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2979 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    28665 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     6371 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     4388 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    23078 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/tests/__init__.py
--rw-r--r--   0        0        0     4210 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/local/tests/test_payload_filters.py
--rw-r--r--   0        0        0       40 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    13716 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1496 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    18788 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2873 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/py.typed
--rw-r--r--   0        0        0    67758 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    70630 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2919 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2567 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-05-24 09:08:26.477326 qdrant_client-1.2.0/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 13:38:56.175043 qdrant_client-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6250 2023-06-23 13:38:56.175043 qdrant_client-1.3.0/README.md
+-rw-r--r--   0        0        0     1417 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    10034 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9742 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3447 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    72811 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    36463 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     2063 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    16916 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    54119 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    30011 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    38894 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    67870 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2979 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    29728 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     6371 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     4388 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    23964 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/tests/__init__.py
+-rw-r--r--   0        0        0     4210 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/tests/test_payload_filters.py
+-rw-r--r--   0        0        0       40 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    13786 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1496 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    19848 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2873 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/py.typed
+-rw-r--r--   0        0        0    72285 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    81209 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2160 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.3.0/PKG-INFO
```

### Comparing `qdrant_client-1.2.0/LICENSE` & `qdrant_client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/README.md` & `qdrant_client-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Client library and SDK for the [Qdrant](https://github.com/qdrant/qdrant) vector search engine.
 
 Library contains type definitions for all Qdrant API and allows to make both Sync and Async requests.
 
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/qdrant/redoc/index.html) directly.
 It also provides some additional helper methods for frequently required operations, e.g. initial collection uploading.
 
-See [QuickStart](https://qdrant.tech/documentation/quick_start/#create-collection) for more details!
+See [QuickStart](https://qdrant.tech/documentation/quick-start/#create-collection) for more details!
 
 ## Installation
 
 ```
 pip install qdrant-client
 ```
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
 definitions for all Qdrant API and allows to make both Sync and Async requests.
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/
 qdrant/redoc/index.html) directly. It also provides some additional helper
 methods for frequently required operations, e.g. initial collection uploading.
-See [QuickStart](https://qdrant.tech/documentation/quick_start/#create-
+See [QuickStart](https://qdrant.tech/documentation/quick-start/#create-
 collection) for more details! ## Installation ``` pip install qdrant-client ```
 ## Features - Type hints for all API methods - Local mode - use same API
 without running server - REST and gRPC support - Minimal dependencies ## Local
 mode
                                     [Qdrant]
 Python client allows you to run same code in local mode without running Qdrant
 server. Simply initialize client like this: ```python from qdrant_client import
```

### Comparing `qdrant_client-1.2.0/pyproject.toml` & `qdrant_client-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.2.0"
+version = "1.3.0"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
@@ -29,14 +29,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
 grpcio-tools = "^1.46.0"
 sphinx = "^4.4.0"
 qdrant-sphinx-theme = { git = "https://github.com/qdrant/qdrant_sphinx_theme.git", branch = "master" }
 coverage = "^6.3.3"
 pytest-asyncio = "^0.21.0"
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.types.dependencies]
 pyright = "^1.1.293"
 mypy = "^1.0.0"
 types-protobuf = "^4.21.0.5"
```

### Comparing `qdrant_client-1.2.0/qdrant_client/client_base.py` & `qdrant_client-1.3.0/qdrant_client/client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         query_filter: Optional[models.Filter] = None,
         search_params: Optional[models.SearchParams] = None,
         limit: int = 10,
         group_size: int = 1,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         raise NotImplementedError()
 
     def recommend_batch(
         self,
         collection_name: str,
@@ -91,14 +92,15 @@
         limit: int = 10,
         group_size: int = 1,
         score_threshold: Optional[float] = None,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         using: Optional[str] = None,
         lookup_from: Optional[models.LookupLocation] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         raise NotImplementedError()
 
     def scroll(
         self,
         collection_name: str,
```

### Comparing `qdrant_client-1.2.0/qdrant_client/connection.py` & `qdrant_client-1.3.0/qdrant_client/connection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/conversions/common_types.py` & `qdrant_client-1.3.0/qdrant_client/conversions/common_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 HnswConfigDiff = Union[rest.HnswConfigDiff, grpc.HnswConfigDiff]
 OptimizersConfigDiff = Union[rest.OptimizersConfigDiff, grpc.OptimizersConfigDiff]
 CollectionParamsDiff = Union[rest.CollectionParamsDiff, grpc.CollectionParamsDiff]
 WalConfigDiff = Union[rest.WalConfigDiff, grpc.WalConfigDiff]
 QuantizationConfig = Union[rest.QuantizationConfig, grpc.QuantizationConfig]
 PointId = Union[int, str, grpc.PointId]
 PayloadSchemaType = Union[
-    rest.PayloadSchemaType, rest.PayloadSchemaParams, int
+    rest.PayloadSchemaType, rest.PayloadSchemaParams, int, grpc.PayloadIndexParams
 ]  # type(grpc.PayloadSchemaType) == int
 Points = Union[rest.Batch, List[Union[rest.PointStruct, grpc.PointStruct]]]
 PointsSelector = Union[
     List[PointId], rest.Filter, grpc.Filter, rest.PointsSelector, grpc.PointsSelector
 ]
 LookupLocation = Union[rest.LookupLocation, grpc.LookupLocation]
 
@@ -56,14 +56,15 @@
 InitFrom: TypeAlias = rest.InitFrom
 
 SearchRequest = Union[rest.SearchRequest, grpc.SearchPoints]
 RecommendRequest = Union[rest.RecommendRequest, grpc.RecommendPoints]
 
 ReadConsistency: TypeAlias = rest.ReadConsistency
 WriteOrdering: TypeAlias = rest.WriteOrdering
+WithLookupInterface: TypeAlias = rest.WithLookupInterface
 
 GroupsResult: TypeAlias = rest.GroupsResult
 
 # we can't use `nptyping` package due to numpy/python-version incompatibilities
 # thus we need to define precise type annotations while we support python3.7
 _np_numeric = Union[
     np.bool_,  # pylance can't handle np.bool8 alias
```

### Comparing `qdrant_client-1.2.0/qdrant_client/conversions/conversion.py` & `qdrant_client-1.3.0/qdrant_client/conversions/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,44 @@
     return dict((key, json_to_value(val)) for key, val in payload.items())
 
 
 def grpc_to_payload(grpc: Dict[str, Value]) -> Dict[str, Any]:
     return dict((key, value_to_json(val)) for key, val in grpc.items())
 
 
+def grpc_payload_schema_to_field_type(model: grpc.PayloadSchemaType) -> grpc.FieldType:
+    if model == grpc.PayloadSchemaType.Keyword:
+        return grpc.FieldType.FieldTypeKeyword
+    if model == grpc.PayloadSchemaType.Integer:
+        return grpc.FieldType.FieldTypeInteger
+    if model == grpc.PayloadSchemaType.Float:
+        return grpc.FieldType.FieldTypeFloat
+    if model == grpc.PayloadSchemaType.Geo:
+        return grpc.FieldType.FieldTypeGeo
+    if model == grpc.PayloadSchemaType.Text:
+        return grpc.FieldType.FieldTypeText
+
+    raise ValueError(f"invalid PayloadSchemaType model: {model}")  # pragma: no cover
+
+
+def grpc_field_type_to_payload_schema(model: grpc.FieldType) -> grpc.PayloadSchemaType:
+    if model == grpc.FieldType.FieldTypeKeyword:
+        return grpc.PayloadSchemaType.Keyword
+    if model == grpc.FieldType.FieldTypeInteger:
+        return grpc.PayloadSchemaType.Integer
+    if model == grpc.FieldType.FieldTypeFloat:
+        return grpc.PayloadSchemaType.Float
+    if model == grpc.FieldType.FieldTypeGeo:
+        return grpc.PayloadSchemaType.Geo
+    if model == grpc.FieldType.FieldTypeText:
+        return grpc.PayloadSchemaType.Text
+
+    raise ValueError(f"invalid FieldType model: {model}")  # pragma: no cover
+
+
 class GrpcToRest:
     @classmethod
     def convert_condition(cls, model: grpc.Condition) -> rest.Condition:
         name = model.WhichOneof("condition_one_of")
         val = getattr(model, name)
 
         if name == "field":
@@ -239,18 +269,31 @@
     ) -> Dict[str, rest.PayloadIndexInfo]:
         return {key: cls.convert_payload_schema_info(info) for key, info in model.items()}
 
     @classmethod
     def convert_payload_schema_info(cls, model: grpc.PayloadSchemaInfo) -> rest.PayloadIndexInfo:
         return rest.PayloadIndexInfo(
             data_type=cls.convert_payload_schema_type(model.data_type),
+            params=cls.convert_payload_schema_params(model.params)
+            if model.HasField("params")
+            else None,
             points=model.points,
         )
 
     @classmethod
+    def convert_payload_schema_params(
+        cls, model: grpc.PayloadIndexParams
+    ) -> rest.PayloadSchemaParams:
+        if model.HasField("text_index_params"):
+            text_index_params = model.text_index_params
+            return cls.convert_text_index_params(text_index_params)
+
+        raise ValueError(f"invalid PayloadIndexParams model: {model}")
+
+    @classmethod
     def convert_payload_schema_type(cls, model: grpc.PayloadSchemaType) -> rest.PayloadSchemaType:
         if model == grpc.PayloadSchemaType.Float:
             return rest.PayloadSchemaType.FLOAT
         elif model == grpc.PayloadSchemaType.Geo:
             return rest.PayloadSchemaType.GEO
         elif model == grpc.PayloadSchemaType.Integer:
             return rest.PayloadSchemaType.INTEGER
@@ -528,14 +571,21 @@
             return rest.CreateAliasOperation(create_alias=cls.convert_create_alias(val))
         if name == "delete_alias":
             return rest.DeleteAliasOperation(delete_alias=cls.convert_delete_alias(val))
 
         raise ValueError(f"invalid AliasOperations model: {model}")  # pragma: no cover
 
     @classmethod
+    def convert_alias_description(cls, model: grpc.AliasDescription) -> rest.AliasDescription:
+        return rest.AliasDescription(
+            alias_name=model.alias_name,
+            collection_name=model.collection_name,
+        )
+
+    @classmethod
     def convert_points_selector(cls, model: grpc.PointsSelector) -> rest.PointsSelector:
         name = model.WhichOneof("points_selector_one_of")
         val = getattr(model, name)
 
         if name == "points":
             return rest.PointIdsList(points=[cls.convert_point_id(point) for point in val.ids])
         if name == "filter":
@@ -810,42 +860,56 @@
     @classmethod
     def convert_quantization_search_params(
         cls, model: grpc.QuantizationSearchParams
     ) -> rest.QuantizationSearchParams:
         return rest.QuantizationSearchParams(
             ignore=model.ignore if model.HasField("ignore") else None,
             rescore=model.rescore if model.HasField("rescore") else None,
+            oversampling=model.oversampling if model.HasField("oversampling") else None,
         )
 
     @classmethod
     def convert_point_vectors(cls, model: grpc.PointVectors) -> rest.PointVectors:
         return rest.PointVectors(
             id=cls.convert_point_id(model.id),
             vector=cls.convert_vectors(model.vectors),
         )
 
     @classmethod
     def convert_groups_result(cls, model: grpc.GroupsResult) -> rest.GroupsResult:
         return rest.GroupsResult(
-            groups=[cls.convert_group(group) for group in model.groups],
+            groups=[cls.convert_point_group(group) for group in model.groups],
         )
 
     @classmethod
-    def convert_group(cls, model: grpc.PointGroup) -> rest.PointGroup:
+    def convert_point_group(cls, model: grpc.PointGroup) -> rest.PointGroup:
         return rest.PointGroup(
             id=cls.convert_group_id(model.id),
             hits=[cls.convert_scored_point(hit) for hit in model.hits],
+            lookup=cls.convert_record(model.lookup) if model.HasField("lookup") else None,
         )
 
     @classmethod
     def convert_group_id(cls, model: grpc.GroupId) -> rest.GroupId:
         name = model.WhichOneof("kind")
         val = getattr(model, name)
         return val
 
+    @classmethod
+    def convert_with_lookup(cls, model: grpc.WithLookup) -> rest.WithLookup:
+        return rest.WithLookup(
+            collection=model.collection,
+            with_payload=cls.convert_with_payload_selector(model.with_payload)
+            if model.HasField("with_payload")
+            else None,
+            with_vectors=cls.convert_with_vectors_selector(model.with_vectors)
+            if model.HasField("with_vectors")
+            else None,
+        )
+
 
 # ----------------------------------------
 #
 # ----------- REST TO gRPC ---------------
 #
 # ----------------------------------------
 
@@ -923,26 +987,42 @@
     def convert_payload_schema(
         cls, model: Dict[str, rest.PayloadIndexInfo]
     ) -> Dict[str, grpc.PayloadSchemaInfo]:
         return dict((key, cls.convert_payload_index_info(val)) for key, val in model.items())
 
     @classmethod
     def convert_payload_index_info(cls, model: rest.PayloadIndexInfo) -> grpc.PayloadSchemaInfo:
-        return grpc.PayloadSchemaInfo(data_type=cls.convert_payload_schema_type(model.data_type))
+        params = model.params
+        return grpc.PayloadSchemaInfo(
+            data_type=cls.convert_payload_schema_type(model.data_type),
+            params=cls.convert_payload_schema_params(params) if params is not None else None,
+            points=model.points,
+        )
+
+    @classmethod
+    def convert_payload_schema_params(
+        cls, model: rest.PayloadSchemaParams
+    ) -> grpc.PayloadIndexParams:
+        if isinstance(model, rest.TextIndexParams):
+            return grpc.PayloadIndexParams(text_index_params=cls.convert_text_index_params(model))
+
+        raise ValueError(f"invalid PayloadSchemaParams model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_payload_schema_type(cls, model: rest.PayloadSchemaType) -> grpc.PayloadSchemaType:
         if model == rest.PayloadSchemaType.KEYWORD:
             return grpc.PayloadSchemaType.Keyword
         if model == rest.PayloadSchemaType.INTEGER:
             return grpc.PayloadSchemaType.Integer
         if model == rest.PayloadSchemaType.FLOAT:
             return grpc.PayloadSchemaType.Float
         if model == rest.PayloadSchemaType.GEO:
             return grpc.PayloadSchemaType.Geo
+        if model == rest.PayloadSchemaType.TEXT:
+            return grpc.PayloadSchemaType.Text
 
         raise ValueError(f"invalid PayloadSchemaType model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_update_result(cls, model: rest.UpdateResult) -> grpc.UpdateResult:
         return grpc.UpdateResult(
             operation_id=model.operation_id,
@@ -1238,14 +1318,21 @@
             return grpc.AliasOperations(delete_alias=cls.convert_delete_alias(model.delete_alias))
         if isinstance(model, rest.RenameAliasOperation):
             return grpc.AliasOperations(rename_alias=cls.convert_rename_alias(model.rename_alias))
 
         raise ValueError(f"invalid AliasOperations model: {model}")  # pragma: no cover
 
     @classmethod
+    def convert_alias_description(cls, model: rest.AliasDescription) -> grpc.AliasDescription:
+        return grpc.AliasDescription(
+            alias_name=model.alias_name,
+            collection_name=model.collection_name,
+        )
+
+    @classmethod
     def convert_extended_point_id(cls, model: rest.ExtendedPointId) -> grpc.PointId:
         if isinstance(model, int):
             return grpc.PointId(num=model)
         if isinstance(model, str):
             return grpc.PointId(uuid=model)
         raise ValueError(f"invalid ExtendedPointId model: {model}")  # pragma: no cover
 
@@ -1605,14 +1692,15 @@
     @classmethod
     def convert_quantization_search_params(
         cls, model: rest.QuantizationSearchParams
     ) -> grpc.QuantizationSearchParams:
         return grpc.QuantizationSearchParams(
             ignore=model.ignore,
             rescore=model.rescore,
+            oversampling=model.oversampling,
         )
 
     @classmethod
     def convert_point_vectors(cls, model: rest.PointVectors) -> grpc.PointVectors:
         return grpc.PointVectors(
             id=cls.convert_extended_point_id(model.id),
             vectors=cls.convert_vector_struct(model.vector),
@@ -1625,14 +1713,15 @@
         )
 
     @classmethod
     def convert_point_group(cls, model: rest.PointGroup) -> grpc.PointGroup:
         return grpc.PointGroup(
             id=cls.convert_group_id(model.id),
             hits=[cls.convert_scored_point(point) for point in model.hits],
+            lookup=cls.convert_record(model.lookup) if model.lookup is not None else None,
         )
 
     @classmethod
     def convert_group_id(cls, model: rest.GroupId) -> grpc.GroupId:
         if isinstance(model, str):
             return grpc.GroupId(
                 string_value=model,
@@ -1644,7 +1733,19 @@
                 )
             else:
                 return grpc.GroupId(
                     integer_value=model,
                 )
         else:
             raise ValueError(f"invalid GroupId model: {model}")
+
+    @classmethod
+    def convert_with_lookup(cls, model: rest.WithLookup) -> grpc.WithLookup:
+        return grpc.WithLookup(
+            collection=model.collection,
+            with_vectors=cls.convert_with_vectors(model.with_vectors)
+            if model.with_vectors is not None
+            else None,
+            with_payload=cls.convert_with_payload_interface(model.with_payload)
+            if model.with_payload is not None
+            else None,
+        )
```

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/points_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import json_with_int_pb2 as json__with__int__pb2
 from . import collections_pb2 as collections__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xaa\x01\n\x12UpdatePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12$\n\x06points\x18\x03 \x03(\x0b\x32\x14.qdrant.PointVectors\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"M\n\x0cPointVectors\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12 \n\x07vectors\x18\x02 \x01(\x0b\x32\x0f.qdrant.Vectors\"\xdf\x01\n\x12\x44\x65letePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12/\n\x0fpoints_selector\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12(\n\x07vectors\x18\x04 \x01(\x0b\x32\x17.qdrant.VectorsSelector\x12,\n\x08ordering\x18\x05 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\\\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescore\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xdc\x03\n\x11SearchPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\r\x12\x31\n\x0cwith_payload\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x06 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x07 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0bvector_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\t \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x10\n\x08group_by\x18\n \x01(\t\x12\x12\n\ngroup_size\x18\x0b \x01(\r\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistency\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xcb\x04\n\x14RecommendPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\r\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x12\n\x05using\x18\t \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\n \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x30\n\x0blookup_from\x18\x0b \x01(\x0b\x32\x16.qdrant.LookupLocationH\x03\x88\x01\x01\x12\x10\n\x08group_by\x18\x0c \x01(\t\x12\x12\n\ngroup_size\x18\r \x01(\r\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistency\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"\\\n\x07GroupId\x12\x18\n\x0eunsigned_value\x18\x01 \x01(\x04H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x03H\x00\x12\x16\n\x0cstring_value\x18\x03 \x01(\tH\x00\x42\x06\n\x04kind\"L\n\nPointGroup\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.GroupId\x12!\n\x04hits\x18\x02 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"2\n\x0cGroupsResult\x12\"\n\x06groups\x18\x01 \x03(\x0b\x32\x12.qdrant.PointGroup\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x14SearchGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"M\n\x17RecommendGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\x99\x02\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x12*\n\x07is_null\x18\x05 \x01(\x0b\x32\x17.qdrant.IsNullConditionH\x00\x12)\n\x06nested\x18\x06 \x01(\x0b\x32\x17.qdrant.NestedConditionH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x1e\n\x0fIsNullCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\">\n\x0fNestedCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xa3\x02\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x33\n\x0f\x65xcept_integers\x18\x07 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x32\n\x0f\x65xcept_keywords\x18\x08 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xaa\x01\n\x12UpdatePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12$\n\x06points\x18\x03 \x03(\x0b\x32\x14.qdrant.PointVectors\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"M\n\x0cPointVectors\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12 \n\x07vectors\x18\x02 \x01(\x0b\x32\x0f.qdrant.Vectors\"\xdf\x01\n\x12\x44\x65letePointVectors\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12/\n\x0fpoints_selector\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12(\n\x07vectors\x18\x04 \x01(\x0b\x32\x17.qdrant.VectorsSelector\x12,\n\x08ordering\x18\x05 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\x88\x01\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12\x19\n\x0coversampling\x18\x03 \x01(\x01H\x02\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescoreB\x0f\n\r_oversampling\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xb2\x01\n\nWithLookup\x12\x12\n\ncollection\x18\x01 \x01(\t\x12\x36\n\x0cwith_payload\x18\x02 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelectorH\x00\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x03 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x01\x88\x01\x01\x42\x0f\n\r_with_payloadB\x0f\n\r_with_vectors\"\x9a\x04\n\x11SearchPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\r\x12\x31\n\x0cwith_payload\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x06 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x07 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0bvector_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\t \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x10\n\x08group_by\x18\n \x01(\t\x12\x12\n\ngroup_size\x18\x0b \x01(\r\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x12,\n\x0bwith_lookup\x18\r \x01(\x0b\x32\x12.qdrant.WithLookupH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyB\x0e\n\x0c_with_lookup\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\x89\x05\n\x14RecommendPointGroups\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\r\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x12\n\x05using\x18\t \x01(\tH\x01\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\n \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x30\n\x0blookup_from\x18\x0b \x01(\x0b\x32\x16.qdrant.LookupLocationH\x03\x88\x01\x01\x12\x10\n\x08group_by\x18\x0c \x01(\t\x12\x12\n\ngroup_size\x18\r \x01(\r\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x12,\n\x0bwith_lookup\x18\x0f \x01(\x0b\x32\x12.qdrant.WithLookupH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyB\x0e\n\x0c_with_lookup\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"\\\n\x07GroupId\x12\x18\n\x0eunsigned_value\x18\x01 \x01(\x04H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x03H\x00\x12\x16\n\x0cstring_value\x18\x03 \x01(\tH\x00\x42\x06\n\x04kind\"t\n\nPointGroup\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.GroupId\x12!\n\x04hits\x18\x02 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12&\n\x06lookup\x18\x03 \x01(\x0b\x32\x16.qdrant.RetrievedPoint\"2\n\x0cGroupsResult\x12\"\n\x06groups\x18\x01 \x03(\x0b\x32\x12.qdrant.PointGroup\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x14SearchGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"M\n\x17RecommendGroupsResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.GroupsResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\x99\x02\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x12*\n\x07is_null\x18\x05 \x01(\x0b\x32\x17.qdrant.IsNullConditionH\x00\x12)\n\x06nested\x18\x06 \x01(\x0b\x32\x17.qdrant.NestedConditionH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x1e\n\x0fIsNullCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\">\n\x0fNestedCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xa3\x02\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x33\n\x0f\x65xcept_integers\x18\x07 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x12\x32\n\x0f\x65xcept_keywords\x18\x08 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
 
 _WRITEORDERINGTYPE = DESCRIPTOR.enum_types_by_name['WriteOrderingType']
 WriteOrderingType = enum_type_wrapper.EnumTypeWrapper(_WRITEORDERINGTYPE)
 _READCONSISTENCYTYPE = DESCRIPTOR.enum_types_by_name['ReadConsistencyType']
 ReadConsistencyType = enum_type_wrapper.EnumTypeWrapper(_READCONSISTENCYTYPE)
 _FIELDTYPE = DESCRIPTOR.enum_types_by_name['FieldType']
 FieldType = enum_type_wrapper.EnumTypeWrapper(_FIELDTYPE)
@@ -67,14 +67,15 @@
 _VECTORS = DESCRIPTOR.message_types_by_name['Vectors']
 _VECTORSSELECTOR = DESCRIPTOR.message_types_by_name['VectorsSelector']
 _WITHVECTORSSELECTOR = DESCRIPTOR.message_types_by_name['WithVectorsSelector']
 _QUANTIZATIONSEARCHPARAMS = DESCRIPTOR.message_types_by_name['QuantizationSearchParams']
 _SEARCHPARAMS = DESCRIPTOR.message_types_by_name['SearchParams']
 _SEARCHPOINTS = DESCRIPTOR.message_types_by_name['SearchPoints']
 _SEARCHBATCHPOINTS = DESCRIPTOR.message_types_by_name['SearchBatchPoints']
+_WITHLOOKUP = DESCRIPTOR.message_types_by_name['WithLookup']
 _SEARCHPOINTGROUPS = DESCRIPTOR.message_types_by_name['SearchPointGroups']
 _SCROLLPOINTS = DESCRIPTOR.message_types_by_name['ScrollPoints']
 _LOOKUPLOCATION = DESCRIPTOR.message_types_by_name['LookupLocation']
 _RECOMMENDPOINTS = DESCRIPTOR.message_types_by_name['RecommendPoints']
 _RECOMMENDBATCHPOINTS = DESCRIPTOR.message_types_by_name['RecommendBatchPoints']
 _RECOMMENDPOINTGROUPS = DESCRIPTOR.message_types_by_name['RecommendPointGroups']
 _COUNTPOINTS = DESCRIPTOR.message_types_by_name['CountPoints']
@@ -311,14 +312,21 @@
 SearchBatchPoints = _reflection.GeneratedProtocolMessageType('SearchBatchPoints', (_message.Message,), {
   'DESCRIPTOR' : _SEARCHBATCHPOINTS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.SearchBatchPoints)
   })
 _sym_db.RegisterMessage(SearchBatchPoints)
 
+WithLookup = _reflection.GeneratedProtocolMessageType('WithLookup', (_message.Message,), {
+  'DESCRIPTOR' : _WITHLOOKUP,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.WithLookup)
+  })
+_sym_db.RegisterMessage(WithLookup)
+
 SearchPointGroups = _reflection.GeneratedProtocolMessageType('SearchPointGroups', (_message.Message,), {
   'DESCRIPTOR' : _SEARCHPOINTGROUPS,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.SearchPointGroups)
   })
 _sym_db.RegisterMessage(SearchPointGroups)
 
@@ -649,22 +657,22 @@
   _NAMEDVECTORS_VECTORSENTRY._serialized_options = b'8\001'
   _SCOREDPOINT_PAYLOADENTRY._options = None
   _SCOREDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _RETRIEVEDPOINT_PAYLOADENTRY._options = None
   _RETRIEVEDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _POINTSTRUCT_PAYLOADENTRY._options = None
   _POINTSTRUCT_PAYLOADENTRY._serialized_options = b'8\001'
-  _WRITEORDERINGTYPE._serialized_start=10123
-  _WRITEORDERINGTYPE._serialized_end=10176
-  _READCONSISTENCYTYPE._serialized_start=10178
-  _READCONSISTENCYTYPE._serialized_end=10234
-  _FIELDTYPE._serialized_start=10236
-  _FIELDTYPE._serialized_end=10348
-  _UPDATESTATUS._serialized_start=10350
-  _UPDATESTATUS._serialized_end=10422
+  _WRITEORDERINGTYPE._serialized_start=10513
+  _WRITEORDERINGTYPE._serialized_end=10566
+  _READCONSISTENCYTYPE._serialized_start=10568
+  _READCONSISTENCYTYPE._serialized_end=10624
+  _FIELDTYPE._serialized_start=10626
+  _FIELDTYPE._serialized_end=10738
+  _UPDATESTATUS._serialized_start=10740
+  _UPDATESTATUS._serialized_end=10812
   _WRITEORDERING._serialized_start=64
   _WRITEORDERING._serialized_end=120
   _READCONSISTENCY._serialized_start=122
   _READCONSISTENCY._serialized_end=211
   _POINTID._serialized_start=213
   _POINTID._serialized_end=273
   _VECTOR._serialized_start=275
@@ -705,108 +713,110 @@
   _NAMEDVECTORS_VECTORSENTRY._serialized_end=2973
   _VECTORS._serialized_start=2975
   _VECTORS._serialized_end=3078
   _VECTORSSELECTOR._serialized_start=3080
   _VECTORSSELECTOR._serialized_end=3112
   _WITHVECTORSSELECTOR._serialized_start=3114
   _WITHVECTORSSELECTOR._serialized_end=3217
-  _QUANTIZATIONSEARCHPARAMS._serialized_start=3219
-  _QUANTIZATIONSEARCHPARAMS._serialized_end=3311
-  _SEARCHPARAMS._serialized_start=3314
-  _SEARCHPARAMS._serialized_end=3470
-  _SEARCHPOINTS._serialized_start=3473
-  _SEARCHPOINTS._serialized_end=3944
-  _SEARCHBATCHPOINTS._serialized_start=3947
-  _SEARCHBATCHPOINTS._serialized_end=4113
-  _SEARCHPOINTGROUPS._serialized_start=4116
-  _SEARCHPOINTGROUPS._serialized_end=4592
-  _SCROLLPOINTS._serialized_start=4595
-  _SCROLLPOINTS._serialized_end=4952
-  _LOOKUPLOCATION._serialized_start=4954
-  _LOOKUPLOCATION._serialized_end=5037
-  _RECOMMENDPOINTS._serialized_start=5040
-  _RECOMMENDPOINTS._serialized_end=5622
-  _RECOMMENDBATCHPOINTS._serialized_start=5625
-  _RECOMMENDBATCHPOINTS._serialized_end=5800
-  _RECOMMENDPOINTGROUPS._serialized_start=5803
-  _RECOMMENDPOINTGROUPS._serialized_end=6390
-  _COUNTPOINTS._serialized_start=6392
-  _COUNTPOINTS._serialized_end=6492
-  _POINTSOPERATIONRESPONSE._serialized_start=6494
-  _POINTSOPERATIONRESPONSE._serialized_end=6571
-  _UPDATERESULT._serialized_start=6573
-  _UPDATERESULT._serialized_end=6647
-  _SCOREDPOINT._serialized_start=6650
-  _SCOREDPOINT._serialized_end=6895
+  _QUANTIZATIONSEARCHPARAMS._serialized_start=3220
+  _QUANTIZATIONSEARCHPARAMS._serialized_end=3356
+  _SEARCHPARAMS._serialized_start=3359
+  _SEARCHPARAMS._serialized_end=3515
+  _SEARCHPOINTS._serialized_start=3518
+  _SEARCHPOINTS._serialized_end=3989
+  _SEARCHBATCHPOINTS._serialized_start=3992
+  _SEARCHBATCHPOINTS._serialized_end=4158
+  _WITHLOOKUP._serialized_start=4161
+  _WITHLOOKUP._serialized_end=4339
+  _SEARCHPOINTGROUPS._serialized_start=4342
+  _SEARCHPOINTGROUPS._serialized_end=4880
+  _SCROLLPOINTS._serialized_start=4883
+  _SCROLLPOINTS._serialized_end=5240
+  _LOOKUPLOCATION._serialized_start=5242
+  _LOOKUPLOCATION._serialized_end=5325
+  _RECOMMENDPOINTS._serialized_start=5328
+  _RECOMMENDPOINTS._serialized_end=5910
+  _RECOMMENDBATCHPOINTS._serialized_start=5913
+  _RECOMMENDBATCHPOINTS._serialized_end=6088
+  _RECOMMENDPOINTGROUPS._serialized_start=6091
+  _RECOMMENDPOINTGROUPS._serialized_end=6740
+  _COUNTPOINTS._serialized_start=6742
+  _COUNTPOINTS._serialized_end=6842
+  _POINTSOPERATIONRESPONSE._serialized_start=6844
+  _POINTSOPERATIONRESPONSE._serialized_end=6921
+  _UPDATERESULT._serialized_start=6923
+  _UPDATERESULT._serialized_end=6997
+  _SCOREDPOINT._serialized_start=7000
+  _SCOREDPOINT._serialized_end=7245
   _SCOREDPOINT_PAYLOADENTRY._serialized_start=1609
   _SCOREDPOINT_PAYLOADENTRY._serialized_end=1670
-  _GROUPID._serialized_start=6897
-  _GROUPID._serialized_end=6989
-  _POINTGROUP._serialized_start=6991
-  _POINTGROUP._serialized_end=7067
-  _GROUPSRESULT._serialized_start=7069
-  _GROUPSRESULT._serialized_end=7119
-  _SEARCHRESPONSE._serialized_start=7121
-  _SEARCHRESPONSE._serialized_end=7188
-  _BATCHRESULT._serialized_start=7190
-  _BATCHRESULT._serialized_end=7240
-  _SEARCHBATCHRESPONSE._serialized_start=7242
-  _SEARCHBATCHRESPONSE._serialized_end=7314
-  _SEARCHGROUPSRESPONSE._serialized_start=7316
-  _SEARCHGROUPSRESPONSE._serialized_end=7390
-  _COUNTRESPONSE._serialized_start=7392
-  _COUNTRESPONSE._serialized_end=7458
-  _SCROLLRESPONSE._serialized_start=7461
-  _SCROLLRESPONSE._serialized_end=7600
-  _COUNTRESULT._serialized_start=7602
-  _COUNTRESULT._serialized_end=7630
-  _RETRIEVEDPOINT._serialized_start=7633
-  _RETRIEVEDPOINT._serialized_end=7852
+  _GROUPID._serialized_start=7247
+  _GROUPID._serialized_end=7339
+  _POINTGROUP._serialized_start=7341
+  _POINTGROUP._serialized_end=7457
+  _GROUPSRESULT._serialized_start=7459
+  _GROUPSRESULT._serialized_end=7509
+  _SEARCHRESPONSE._serialized_start=7511
+  _SEARCHRESPONSE._serialized_end=7578
+  _BATCHRESULT._serialized_start=7580
+  _BATCHRESULT._serialized_end=7630
+  _SEARCHBATCHRESPONSE._serialized_start=7632
+  _SEARCHBATCHRESPONSE._serialized_end=7704
+  _SEARCHGROUPSRESPONSE._serialized_start=7706
+  _SEARCHGROUPSRESPONSE._serialized_end=7780
+  _COUNTRESPONSE._serialized_start=7782
+  _COUNTRESPONSE._serialized_end=7848
+  _SCROLLRESPONSE._serialized_start=7851
+  _SCROLLRESPONSE._serialized_end=7990
+  _COUNTRESULT._serialized_start=7992
+  _COUNTRESULT._serialized_end=8020
+  _RETRIEVEDPOINT._serialized_start=8023
+  _RETRIEVEDPOINT._serialized_end=8242
   _RETRIEVEDPOINT_PAYLOADENTRY._serialized_start=1609
   _RETRIEVEDPOINT_PAYLOADENTRY._serialized_end=1670
-  _GETRESPONSE._serialized_start=7854
-  _GETRESPONSE._serialized_end=7921
-  _RECOMMENDRESPONSE._serialized_start=7923
-  _RECOMMENDRESPONSE._serialized_end=7993
-  _RECOMMENDBATCHRESPONSE._serialized_start=7995
-  _RECOMMENDBATCHRESPONSE._serialized_end=8070
-  _RECOMMENDGROUPSRESPONSE._serialized_start=8072
-  _RECOMMENDGROUPSRESPONSE._serialized_end=8149
-  _FILTER._serialized_start=8151
-  _FILTER._serialized_end=8264
-  _CONDITION._serialized_start=8267
-  _CONDITION._serialized_end=8548
-  _ISEMPTYCONDITION._serialized_start=8550
-  _ISEMPTYCONDITION._serialized_end=8581
-  _ISNULLCONDITION._serialized_start=8583
-  _ISNULLCONDITION._serialized_end=8613
-  _HASIDCONDITION._serialized_start=8615
-  _HASIDCONDITION._serialized_end=8664
-  _NESTEDCONDITION._serialized_start=8666
-  _NESTEDCONDITION._serialized_end=8728
-  _FIELDCONDITION._serialized_start=8731
-  _FIELDCONDITION._serialized_end=8952
-  _MATCH._serialized_start=8955
-  _MATCH._serialized_end=9246
-  _REPEATEDSTRINGS._serialized_start=9248
-  _REPEATEDSTRINGS._serialized_end=9282
-  _REPEATEDINTEGERS._serialized_start=9284
-  _REPEATEDINTEGERS._serialized_end=9320
-  _RANGE._serialized_start=9322
-  _RANGE._serialized_end=9429
-  _GEOBOUNDINGBOX._serialized_start=9431
-  _GEOBOUNDINGBOX._serialized_end=9523
-  _GEORADIUS._serialized_start=9525
-  _GEORADIUS._serialized_end=9586
-  _VALUESCOUNT._serialized_start=9588
-  _VALUESCOUNT._serialized_end=9701
-  _POINTSSELECTOR._serialized_start=9703
-  _POINTSSELECTOR._serialized_end=9820
-  _POINTSIDSLIST._serialized_start=9822
-  _POINTSIDSLIST._serialized_end=9867
-  _POINTSTRUCT._serialized_start=9870
-  _POINTSTRUCT._serialized_end=10083
+  _GETRESPONSE._serialized_start=8244
+  _GETRESPONSE._serialized_end=8311
+  _RECOMMENDRESPONSE._serialized_start=8313
+  _RECOMMENDRESPONSE._serialized_end=8383
+  _RECOMMENDBATCHRESPONSE._serialized_start=8385
+  _RECOMMENDBATCHRESPONSE._serialized_end=8460
+  _RECOMMENDGROUPSRESPONSE._serialized_start=8462
+  _RECOMMENDGROUPSRESPONSE._serialized_end=8539
+  _FILTER._serialized_start=8541
+  _FILTER._serialized_end=8654
+  _CONDITION._serialized_start=8657
+  _CONDITION._serialized_end=8938
+  _ISEMPTYCONDITION._serialized_start=8940
+  _ISEMPTYCONDITION._serialized_end=8971
+  _ISNULLCONDITION._serialized_start=8973
+  _ISNULLCONDITION._serialized_end=9003
+  _HASIDCONDITION._serialized_start=9005
+  _HASIDCONDITION._serialized_end=9054
+  _NESTEDCONDITION._serialized_start=9056
+  _NESTEDCONDITION._serialized_end=9118
+  _FIELDCONDITION._serialized_start=9121
+  _FIELDCONDITION._serialized_end=9342
+  _MATCH._serialized_start=9345
+  _MATCH._serialized_end=9636
+  _REPEATEDSTRINGS._serialized_start=9638
+  _REPEATEDSTRINGS._serialized_end=9672
+  _REPEATEDINTEGERS._serialized_start=9674
+  _REPEATEDINTEGERS._serialized_end=9710
+  _RANGE._serialized_start=9712
+  _RANGE._serialized_end=9819
+  _GEOBOUNDINGBOX._serialized_start=9821
+  _GEOBOUNDINGBOX._serialized_end=9913
+  _GEORADIUS._serialized_start=9915
+  _GEORADIUS._serialized_end=9976
+  _VALUESCOUNT._serialized_start=9978
+  _VALUESCOUNT._serialized_end=10091
+  _POINTSSELECTOR._serialized_start=10093
+  _POINTSSELECTOR._serialized_end=10210
+  _POINTSIDSLIST._serialized_start=10212
+  _POINTSIDSLIST._serialized_end=10257
+  _POINTSTRUCT._serialized_start=10260
+  _POINTSTRUCT._serialized_end=10473
   _POINTSTRUCT_PAYLOADENTRY._serialized_start=1609
   _POINTSTRUCT_PAYLOADENTRY._serialized_end=1670
-  _GEOPOINT._serialized_start=10085
-  _GEOPOINT._serialized_end=10121
+  _GEOPOINT._serialized_start=10475
+  _GEOPOINT._serialized_end=10511
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.3.0/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.3.0/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api/points_api.py` & `qdrant_client-1.3.0/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api/service_api.py` & `qdrant_client-1.3.0/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.3.0/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/api_client.py` & `qdrant_client-1.3.0/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/exceptions.py` & `qdrant_client-1.3.0/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/http/models/models.py` & `qdrant_client-1.3.0/qdrant_client/http/models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     startup: datetime = Field(..., description="")
 
 
 class AppFeaturesTelemetry(BaseModel):
     debug: bool = Field(..., description="")
     web_feature: bool = Field(..., description="")
     service_debug_feature: bool = Field(..., description="")
+    recovery_mode: bool = Field(..., description="")
 
 
 class Batch(BaseModel):
     ids: List["ExtendedPointId"] = Field(..., description="")
     vectors: "BatchVectorStruct" = Field(..., description="")
     payloads: Optional[List["Payload"]] = Field(default=None, description="")
 
@@ -973,14 +974,15 @@
 
     uri: str = Field(..., description="Information of a peer in the cluster")
 
 
 class PointGroup(BaseModel):
     hits: List["ScoredPoint"] = Field(..., description="Scored points that have the same value of the group_by key")
     id: "GroupId" = Field(..., description="")
+    lookup: Optional["Record"] = Field(default=None, description="Record that has been looked up using the group id")
 
 
 class PointIdsList(BaseModel):
     points: List["ExtendedPointId"] = Field(..., description="")
 
 
 class PointRequest(BaseModel):
@@ -1027,14 +1029,18 @@
     ignore: Optional[bool] = Field(
         default=False, description="If true, quantized vectors are ignored. Default is false."
     )
     rescore: Optional[bool] = Field(
         default=False,
         description="If true, use original vectors to re-score top-k results. Might require more time in case if original vectors are stored on disk. Default is false.",
     )
+    oversampling: Optional[float] = Field(
+        default=None,
+        description="Oversampling factor for quantization. Default is 1.0.  Defines how many extra vectors should be pre-selected using quantized index, and then re-scored using original vectors.  For example, if `oversampling` is 2.4 and `limit` is 100, then 240 vectors will be pre-selected using quantized index, and then top-100 will be returned after re-scoring.",
+    )
 
 
 class RaftInfo(BaseModel):
     """
     Summary information about the current raft state
     """
 
@@ -1095,14 +1101,17 @@
     )
     group_by: str = Field(
         ...,
         description="Payload field to group by, must be a string or number field. If the field contains more than 1 value, all values will be used for grouping. One point can be in multiple groups.",
     )
     group_size: int = Field(..., description="Maximum amount of points to return per group")
     limit: int = Field(..., description="Maximum amount of groups to return")
+    with_lookup: Optional["WithLookupInterface"] = Field(
+        default=None, description="Look for points in another collection using the group ids"
+    )
 
 
 class RecommendRequest(BaseModel):
     """
     Recommendation request. Provides positive and negative examples of the vectors, which are already stored in the collection.  Service should look for the points which are closer to positive examples and at the same time further to negative examples. The concrete way of how to compare negative and positive distances is up to implementation in `segment` crate.
     """
 
@@ -1295,14 +1304,17 @@
     )
     group_by: str = Field(
         ...,
         description="Payload field to group by, must be a string or number field. If the field contains more than 1 value, all values will be used for grouping. One point can be in multiple groups.",
     )
     group_size: int = Field(..., description="Maximum amount of points to return per group")
     limit: int = Field(..., description="Maximum amount of groups to return")
+    with_lookup: Optional["WithLookupInterface"] = Field(
+        default=None, description="Look for points in another collection using the group ids"
+    )
 
 
 class SearchParams(BaseModel):
     """
     Additional parameters of the search
     """
 
@@ -1566,14 +1578,24 @@
     )
 
 
 class WebApiTelemetry(BaseModel):
     responses: Dict[str, Dict[str, "OperationDurationStatistics"]] = Field(..., description="")
 
 
+class WithLookup(BaseModel):
+    collection: str = Field(..., description="Name of the collection to use for points lookup")
+    with_payload: Optional["WithPayloadInterface"] = Field(
+        default=None, description="Options for specifying which payload to include (or not)"
+    )
+    with_vectors: Optional["WithVector"] = Field(
+        default=None, description="Options for specifying which vectors to include (or not)"
+    )
+
+
 class WriteOrdering(str, Enum):
     WEAK = "weak"
     MEDIUM = "medium"
     STRONG = "strong"
 
 
 AliasOperations = Union[
@@ -1686,14 +1708,18 @@
     List[StrictFloat],
     Dict[StrictStr, List[StrictFloat]],
 ]
 VectorsConfig = Union[
     VectorParams,
     Dict[StrictStr, VectorParams],
 ]
+WithLookupInterface = Union[
+    WithLookup,
+    StrictStr,
+]
 WithVector = Union[
     List[StrictStr],
     StrictBool,
 ]
 PayloadFieldSchema = Union[
     PayloadSchemaType,
     PayloadSchemaParams,
```

### Comparing `qdrant_client-1.2.0/qdrant_client/local/distances.py` & `qdrant_client-1.3.0/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/local/geo.py` & `qdrant_client-1.3.0/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/local/local_collection.py` & `qdrant_client-1.3.0/qdrant_client/local/local_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                         vectors[name].append(v)
                     else:
                         vectors[name].append(
                             np.ones(self.config.vectors[name].size, dtype=np.float32)
                         )
                         deleted_ids.append((idx, name))
 
-                self.payload.append(point.payload)
+                self.payload.append(point.payload or {})
 
             for name, named_vectors in vectors.items():
                 self.vectors[name] = np.array(named_vectors)
                 self.deleted_per_vector[name] = np.zeros(len(self.payload), dtype=bool)
 
             for idx, name in deleted_ids:
                 self.deleted_per_vector[name][idx] = 1
@@ -259,14 +259,16 @@
         group_by: str,
         query_filter: Optional[models.Filter] = None,
         limit: int = 10,
         group_size: int = 1,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
+        with_lookup_collection: Optional["LocalCollection"] = None,
     ) -> models.GroupsResult:
         points = self.search(
             query_vector=query_vector,
             query_filter=query_filter,
             limit=len(self.ids_inv),
             with_payload=True,
             with_vectors=with_vectors,
@@ -292,15 +294,33 @@
                     groups[group_value] = models.PointGroup(id=group_value, hits=[])
 
                 if len(groups[group_value].hits) >= group_size:
                     continue
 
                 groups[group_value].hits.append(point)
 
-        return models.GroupsResult(groups=list(groups.values())[:limit])
+        groups_result: List[models.PointGroup] = list(groups.values())[:limit]
+
+        if isinstance(with_lookup, str):
+            with_lookup = models.WithLookup(
+                collection=with_lookup,
+                with_payload=None,
+                with_vectors=None,
+            )
+
+        if with_lookup is not None and with_lookup_collection is not None:
+            for group in groups_result:
+                lookup = with_lookup_collection.retrieve(
+                    ids=[group.id],
+                    with_payload=with_lookup.with_payload,
+                    with_vectors=with_lookup.with_vectors,
+                )
+                group.lookup = next(iter(lookup), None)
+
+        return models.GroupsResult(groups=groups_result)
 
     def retrieve(
         self,
         ids: Sequence[types.PointId],
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
     ) -> List[models.Record]:
@@ -429,14 +449,16 @@
         group_size: int = 1,
         score_threshold: Optional[float] = None,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         using: Optional[str] = None,
         lookup_from_collection: Optional["LocalCollection"] = None,
         lookup_from_vector_name: Optional[str] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
+        with_lookup_collection: Optional["LocalCollection"] = None,
     ) -> types.GroupsResult:
         search_in_vector_name, vector, query_filter = self._recommend(
             positive,
             negative,
             query_filter,
             using,
             lookup_from_collection,
@@ -447,14 +469,16 @@
             query_filter=query_filter,
             group_by=group_by,
             group_size=group_size,
             limit=limit,
             with_payload=with_payload,
             with_vectors=with_vectors,
             score_threshold=score_threshold,
+            with_lookup=with_lookup,
+            with_lookup_collection=with_lookup_collection,
         )
 
     @classmethod
     def _universal_id(cls, point_id: models.ExtendedPointId) -> Tuple[str, int]:
         if isinstance(point_id, str):
             return point_id, 0
         elif isinstance(point_id, int):
@@ -514,15 +538,15 @@
             ids_inv=self.ids_inv,
         )
         mask = payload_mask & ~self.deleted
         return models.CountResult(count=np.count_nonzero(mask))
 
     def _update_point(self, point: models.PointStruct) -> None:
         idx = self.ids[point.id]
-        self.payload[idx] = point.payload
+        self.payload[idx] = point.payload or {}
 
         if isinstance(point.vector, list):
             vectors = {DEFAULT_VECTOR_NAME: point.vector}
         else:
             vectors = point.vector
 
         for vector_name, named_vectors in self.vectors.items():
@@ -535,15 +559,15 @@
 
         self.deleted[idx] = 0
 
     def _add_point(self, point: models.PointStruct) -> None:
         idx = len(self.ids)
         self.ids[point.id] = idx
         self.ids_inv.append(point.id)
-        self.payload.append(point.payload)
+        self.payload.append(point.payload or {})
         self.deleted = np.append(self.deleted, 0)
 
         if isinstance(point.vector, list):
             vectors = {DEFAULT_VECTOR_NAME: point.vector}
         else:
             vectors = point.vector
 
@@ -733,15 +757,15 @@
             models.FilterSelector,
             models.PointIdsList,
         ],
     ) -> None:
         ids = self._selector_to_ids(selector)
         for point_id in ids:
             idx = self.ids[point_id]
-            self.payload[idx] = payload
+            self.payload[idx] = payload or {}
             self._persist_by_id(point_id)
 
     def delete_payload(
         self,
         keys: Sequence[str],
         selector: Union[
             models.Filter,
```

### Comparing `qdrant_client-1.2.0/qdrant_client/local/payload_filters.py` & `qdrant_client-1.3.0/qdrant_client/local/payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.3.0/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/local/persistence.py` & `qdrant_client-1.3.0/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.3.0/qdrant_client/local/qdrant_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import itertools
 import json
 import logging
 import os
 import shutil
 from io import TextIOWrapper
-from itertools import zip_longest
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import portalocker
 
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.conversions import common_types as types
@@ -164,26 +164,36 @@
         query_filter: Optional[rest_models.Filter] = None,
         search_params: Optional[rest_models.SearchParams] = None,
         limit: int = 10,
         group_size: int = 1,
         with_payload: Union[bool, Sequence[str], rest_models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         collection = self._get_collection(collection_name)
+        with_lookup_collection = None
+        if with_lookup is not None:
+            if isinstance(with_lookup, str):
+                with_lookup_collection = self._get_collection(with_lookup)
+            else:
+                with_lookup_collection = self._get_collection(with_lookup.collection)
+
         return collection.search_groups(
             query_vector=query_vector,
             query_filter=query_filter,
             limit=limit,
             group_by=group_by,
             group_size=group_size,
             with_payload=with_payload,
             with_vectors=with_vectors,
             score_threshold=score_threshold,
+            with_lookup=with_lookup,
+            with_lookup_collection=with_lookup_collection,
         )
 
     def recommend_batch(
         self,
         collection_name: str,
         requests: Sequence[types.RecommendRequest],
         **kwargs: Any,
@@ -248,18 +258,25 @@
         limit: int = 10,
         group_size: int = 1,
         score_threshold: Optional[float] = None,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         using: Optional[str] = None,
         lookup_from: Optional[types.LookupLocation] = None,
-        consistency: Optional[types.ReadConsistency] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         collection = self._get_collection(collection_name)
+        with_lookup_collection = None
+        if with_lookup is not None:
+            if isinstance(with_lookup, str):
+                with_lookup_collection = self._get_collection(with_lookup)
+            else:
+                with_lookup_collection = self._get_collection(with_lookup.collection)
+
         return collection.recommend_groups(
             positive=positive,
             negative=negative,
             group_by=group_by,
             group_size=group_size,
             query_filter=query_filter,
             limit=limit,
@@ -267,14 +284,16 @@
             with_vectors=with_vectors,
             score_threshold=score_threshold,
             using=using,
             lookup_from_collection=self._get_collection(lookup_from.collection)
             if lookup_from
             else None,
             lookup_from_vector_name=lookup_from.vector if lookup_from else None,
+            with_lookup=with_lookup,
+            with_lookup_collection=with_lookup_collection,
         )
 
     def scroll(
         self,
         collection_name: str,
         scroll_filter: Optional[types.Filter] = None,
         limit: int = 10,
@@ -533,20 +552,22 @@
         ids: Optional[Iterable[types.PointId]] = None,
         **kwargs: Any,
     ) -> None:
         collection = self._get_collection(collection_name)
         collection.upsert(
             [
                 rest_models.PointStruct(
-                    id=point_id or idx,
+                    id=point_id,
                     vector=(vector.tolist() if isinstance(vector, np.ndarray) else vector) or {},
                     payload=payload or {},
                 )
-                for idx, (point_id, vector, payload) in enumerate(
-                    zip_longest(ids or [], iter(vectors), payload or [])
+                for (point_id, vector, payload) in zip(
+                    ids or itertools.count(),
+                    iter(vectors),
+                    payload or itertools.cycle([{}]),
                 )
             ]
         )
 
     def create_payload_index(
         self,
         collection_name: str,
```

### Comparing `qdrant_client-1.2.0/qdrant_client/local/tests/test_payload_filters.py` & `qdrant_client-1.3.0/qdrant_client/local/tests/test_payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/parallel_processor.py` & `qdrant_client-1.3.0/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/collections.proto` & `qdrant_client-1.3.0/qdrant_client/proto/collections.proto`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 message CreateCollection {
   string collection_name = 1; // Name of the collection
   reserved 2; // Deprecated
   reserved 3; // Deprecated
   optional HnswConfigDiff hnsw_config = 4; // Configuration of vector index
   optional WalConfigDiff wal_config = 5; // Configuration of the Write-Ahead-Log
   optional OptimizersConfigDiff optimizers_config = 6; // Configuration of the optimizers
-  optional uint32 shard_number = 7; // Number of shards in the collection, default = 1
+  optional uint32 shard_number = 7; // Number of shards in the collection, default is 1 for standalone, otherwise equal to the number of nodes. Minimum is 1
   optional bool on_disk_payload = 8; // If true - point's payload will not be stored in memory
   optional uint64 timeout = 9; // Wait timeout for operation commit in seconds, if not specified - default value will be supplied
   optional VectorsConfig vectors_config = 10; // Configuration for vectors
   optional uint32 replication_factor = 11; // Number of replicas of each shard that network tries to maintain, default = 1
   optional uint32 write_consistency_factor = 12; // How many replicas should apply the operation for us to consider it successful, default = 1
   optional string init_from_collection = 13; // Specify name of the other collection to copy data from
   optional QuantizationConfig quantization_config = 14; // Quantization configuration of vector
```

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.3.0/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.3.0/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/points.proto` & `qdrant_client-1.3.0/qdrant_client/proto/points.proto`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,25 @@
    */
   optional bool ignore = 1;
 
   /*
   If true, use original vectors to re-score top-k results. Default is true.
    */
   optional bool rescore = 2;
+
+  /*
+  Oversampling factor for quantization.
+
+  Defines how many extra vectors should be pre-selected using quantized index,
+  and then re-scored using original vectors.
+
+  For example, if `oversampling` is 2.4 and `limit` is 100, then 240 vectors will be pre-selected using quantized index,
+  and then top-100 will be returned after re-scoring.
+   */
+  optional double oversampling = 3;
 }
 
 message SearchParams {
   /*
   Params relevant to HNSW index. Size of the beam in a beam-search.
   Larger the value - more accurate the result, more time required for search.
    */
@@ -225,27 +236,35 @@
 
 message SearchBatchPoints {
   string collection_name = 1; // Name of the collection
   repeated SearchPoints search_points = 2;
   optional ReadConsistency read_consistency = 3; // Options for specifying read consistency guarantees
 }
 
+message WithLookup {
+  string collection = 1; // Name of the collection to use for points lookup
+  optional WithPayloadSelector with_payload = 2; // Options for specifying which payload to include (or not)
+  optional WithVectorsSelector with_vectors = 3; // Options for specifying which vectors to include (or not)
+}
+
+
 message SearchPointGroups {
   string collection_name = 1; // Name of the collection
   repeated float vector = 2; // Vector to compare against
   Filter filter = 3; // Filter conditions - return only those points that satisfy the specified conditions
   uint32 limit = 4; // Max number of result
   WithPayloadSelector with_payload = 5; // Options for specifying which payload to include or not
   SearchParams params = 6; // Search config
   optional float score_threshold = 7; // If provided - cut off results with worse scores
   optional string vector_name = 8; // Which vector to use for search, if not specified - use default vector
   optional WithVectorsSelector with_vectors = 9; // Options for specifying which vectors to include into response
   string group_by = 10; // Payload field to group by, must be a string or number field. If there are multiple values for the field, all of them will be used. One point can be in multiple groups.
   uint32 group_size = 11; // Maximum amount of points to return per group
   optional ReadConsistency read_consistency = 12; // Options for specifying read consistency guarantees
+  optional WithLookup with_lookup = 13; // Options for specifying how to use the group id to lookup points in another collection
 }
 
 message ScrollPoints {
   string collection_name = 1;
   Filter filter = 2; // Filter conditions - return only those points that satisfy the specified conditions
   optional PointId offset = 3; // Start with this ID
   optional uint32 limit = 4; // Max number of result
@@ -294,14 +313,15 @@
   optional float score_threshold = 8; // If provided - cut off results with worse scores
   optional string using = 9; // Define which vector to use for recommendation, if not specified - default vector
   optional WithVectorsSelector with_vectors = 10; // Options for specifying which vectors to include into response
   optional LookupLocation lookup_from = 11; // Name of the collection to use for points lookup, if not specified - use current collection
   string group_by = 12; // Payload field to group by, must be a string or number field. If there are multiple values for the field, all of them will be used. One point can be in multiple groups.
   uint32 group_size = 13; // Maximum amount of points to return per group
   optional ReadConsistency read_consistency = 14; // Options for specifying read consistency guarantees
+  optional WithLookup with_lookup = 15; // Options for specifying how to use the group id to lookup points in another collection
 }
 
 message CountPoints {
   string collection_name = 1; // name of the collection
   Filter filter = 2; // Filter conditions - return only those points that satisfy the specified conditions
   optional bool exact = 3; // If `true` - return exact count, if `false` - return approximate count
 }
@@ -345,14 +365,15 @@
     string string_value = 3;
   }
 }
 
 message PointGroup {
   GroupId id = 1; // Group id
   repeated ScoredPoint hits = 2; // Points in the group
+  RetrievedPoint lookup = 3; // Point(s) from the lookup collection that matches the group id
 }
 
 message GroupsResult {
   repeated PointGroup groups = 1; // Groups
 }
 
 message SearchResponse {
```

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/points_service.proto` & `qdrant_client-1.3.0/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.3.0/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/qdrant_client/qdrant_client.py` & `qdrant_client-1.3.0/qdrant_client/qdrant_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 from qdrant_client import grpc as grpc
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import ApiClient, SyncApis
 from qdrant_client.local.qdrant_local import QdrantLocal
@@ -48,14 +49,15 @@
             Example: `service/v1` will result in `http://localhost:6333/service/v1/{qdrant-endpoint}` for REST API.
             Default: `None`
         timeout:
             Timeout for REST and gRPC API requests.
             Default: 5.0 seconds for REST and unlimited for gRPC
         host: Host name of Qdrant service. If url and host are None, set to 'localhost'.
             Default: `None`
+        path: Persistence path for QdrantLocal. Default: `None`
         **kwargs: Additional arguments passed directly into REST client initialization
 
     """
 
     def __init__(
         self,
         location: Optional[str] = None,
@@ -185,14 +187,16 @@
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of search responses
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.search_batch(
             collection_name=collection_name,
             requests=requests,
             consistency=consistency,
             **kwargs,
         )
 
@@ -276,14 +280,16 @@
                     ]
                 )
             )
 
         Returns:
             List of found close points with similarity scores.
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.search(
             collection_name=collection_name,
             query_vector=query_vector,
             query_filter=query_filter,
             search_params=search_params,
             limit=limit,
             offset=offset,
@@ -308,14 +314,15 @@
         query_filter: Optional[types.Filter] = None,
         search_params: Optional[types.SearchParams] = None,
         limit: int = 10,
         group_size: int = 1,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         consistency: Optional[types.ReadConsistency] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         """Search for closest vectors grouped by payload field.
 
         Searches best matches for query vector grouped by the value of payload field.
         Useful to obtain most relevant results for each category, deduplicate results,
@@ -347,38 +354,46 @@
                 - If List of string - include only specified fields
                 - Default: `False`
             score_threshold: Minimal score threshold for the result.
                 If defined, less similar results will not be returned.
                 Score of the returned result might be higher or smaller than the threshold depending
                 on the Distance function used.
                 E.g. for cosine similarity only higher scores will be returned.
+            with_lookup:
+                Look for points in another collection using the group ids.
+                If specified, each group will contain a record from the specified collection
+                with the same id as the group id. In addition, the parameter allows to specify
+                which parts of the record should be returned, like in `with_payload` and `with_vectors` parameters.
             consistency:
                 Read consistency of the search. Defines how many replicas should be queried before returning the result.
                 Values:
                 - int - number of replicas to query, values should present in all queried replicas
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of groups with not more than `group_size` hits in each group.
             Each group also contains an id of the group, which is the value of the payload field.
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.search_groups(
             collection_name=collection_name,
             query_vector=query_vector,
             group_by=group_by,
             query_filter=query_filter,
             search_params=search_params,
             limit=limit,
             group_size=group_size,
             with_payload=with_payload,
             with_vectors=with_vectors,
             score_threshold=score_threshold,
             consistency=consistency,
+            with_lookup=with_lookup,
             **kwargs,
         )
 
     def recommend_batch(
         self,
         collection_name: str,
         requests: Sequence[types.RecommendRequest],
@@ -397,14 +412,16 @@
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of recommend responses
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.recommend_batch(
             collection_name=collection_name,
             requests=requests,
             consistency=consistency,
             **kwargs,
         )
 
@@ -479,14 +496,15 @@
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of recommended points with similarity scores.
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
 
         return self._client.recommend(
             collection_name=collection_name,
             positive=positive,
             negative=negative,
             query_filter=query_filter,
             search_params=search_params,
@@ -512,14 +530,15 @@
         limit: int = 10,
         group_size: int = 1,
         score_threshold: Optional[float] = None,
         with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         using: Optional[str] = None,
         lookup_from: Optional[types.LookupLocation] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         consistency: Optional[types.ReadConsistency] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         """Recommend point groups: search for similar points based on already stored in Qdrant examples
         and groups by payload field.
 
         Recommend best matches for given stored examples grouped by the value of payload field.
@@ -564,27 +583,34 @@
                 E.g. for cosine similarity only higher scores will be returned.
             using:
                 Name of the vectors to use for recommendations.
                 If `None` - use default vectors.
             lookup_from:
                 Defines a location (collection and vector field name), used to lookup vectors for recommendations.
                 If `None` - use current collection will be used.
+            with_lookup:
+                Look for points in another collection using the group ids.
+                If specified, each group will contain a record from the specified collection
+                with the same id as the group id. In addition, the parameter allows to specify
+                which parts of the record should be returned, like in `with_payload` and `with_vectors` parameters.
             consistency:
                 Read consistency of the search. Defines how many replicas should be queried before returning the result.
                 Values:
                 - int - number of replicas to query, values should present in all queried replicas
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of groups with not more than `group_size` hits in each group.
             Each group also contains an id of the group, which is the value of the payload field.
 
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.recommend_groups(
             collection_name=collection_name,
             group_by=group_by,
             positive=positive,
             negative=negative,
             query_filter=query_filter,
             search_params=search_params,
@@ -592,14 +618,15 @@
             group_size=group_size,
             score_threshold=score_threshold,
             with_payload=with_payload,
             with_vectors=with_vectors,
             using=using,
             lookup_from=lookup_from,
             consistency=consistency,
+            with_lookup=with_lookup,
             **kwargs,
         )
 
     def scroll(
         self,
         collection_name: str,
         scroll_filter: Optional[types.Filter] = None,
@@ -639,14 +666,16 @@
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             A pair of (List of points) and (optional offset for the next scroll request).
             If next page offset is `None` - there is no more points in the collection to scroll.
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.scroll(
             collection_name=collection_name,
             scroll_filter=scroll_filter,
             limit=limit,
             offset=offset,
             with_payload=with_payload,
             with_vectors=with_vectors,
@@ -671,14 +700,16 @@
             exact:
                 If `True` - provide the exact count of points matching the filter.
                 If `False` - provide the approximate count of points matching the filter. Works faster.
 
         Returns:
             Amount of points in the collection matching the filter.
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.count(
             collection_name=collection_name,
             count_filter=count_filter,
             exact=exact,
             **kwargs,
         )
 
@@ -708,14 +739,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.upsert(
             collection_name=collection_name,
             points=points,
             wait=wait,
             ordering=ordering,
             **kwargs,
         )
@@ -743,14 +776,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.update_vectors(
             collection_name=collection_name,
             vectors=vectors,
             wait=wait,
             ordering=ordering,
         )
 
@@ -782,14 +817,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_vectors(
             collection_name=collection_name,
             vectors=vectors,
             points=points,
             wait=wait,
             ordering=ordering,
         )
@@ -826,14 +863,16 @@
                 - 'majority' - query all replicas, but return values present in the majority of replicas
                 - 'quorum' - query the majority of replicas, return values present in all of them
                 - 'all' - query all replicas, and return values present in all replicas
 
         Returns:
             List of points
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.retrieve(
             collection_name=collection_name,
             ids=ids,
             with_payload=with_payload,
             with_vectors=with_vectors,
             consistency=consistency,
             **kwargs,
@@ -866,14 +905,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete(
             collection_name=collection_name,
             points_selector=points_selector,
             wait=wait,
             ordering=ordering,
             **kwargs,
         )
@@ -922,14 +963,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.set_payload(
             collection_name=collection_name,
             payload=payload,
             points=points,
             wait=wait,
             ordering=ordering,
             **kwargs,
@@ -981,14 +1024,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.overwrite_payload(
             collection_name=collection_name,
             payload=payload,
             points=points,
             wait=wait,
             ordering=ordering,
             **kwargs,
@@ -1023,14 +1068,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_payload(
             collection_name=collection_name,
             keys=keys,
             points=points,
             wait=wait,
             ordering=ordering,
             **kwargs,
@@ -1063,14 +1110,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.clear_payload(
             collection_name=collection_name,
             points_selector=points_selector,
             wait=wait,
             ordering=ordering,
             **kwargs,
         )
@@ -1090,14 +1139,16 @@
             timeout:
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.update_collection_aliases(
             change_aliases_operations=change_aliases_operations,
             timeout=timeout,
             **kwargs,
         )
 
     def get_collection_aliases(
@@ -1107,67 +1158,84 @@
 
         Args:
             collection_name: Name of the collection
 
         Returns:
             Collection aliases
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.get_collection_aliases(collection_name=collection_name, **kwargs)
 
     def get_aliases(self, **kwargs: Any) -> types.CollectionsAliasesResponse:
         """Get all aliases
 
         Returns:
             All aliases of all collections
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.get_aliases(**kwargs)
 
     def get_collections(self, **kwargs: Any) -> types.CollectionsResponse:
         """Get list name of all existing collections
 
         Returns:
             List of the collections
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.get_collections(**kwargs)
 
     def get_collection(self, collection_name: str, **kwargs: Any) -> types.CollectionInfo:
         """Get detailed information about specified existing collection
 
         Args:
             collection_name: Name of the collection
 
         Returns:
             Detailed information about the collection
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.get_collection(collection_name=collection_name, **kwargs)
 
     def update_collection(
         self,
         collection_name: str,
-        optimizer_config: Optional[types.OptimizersConfigDiff] = None,
+        optimizers_config: Optional[types.OptimizersConfigDiff] = None,
         collection_params: Optional[types.CollectionParamsDiff] = None,
         timeout: Optional[int] = None,
         **kwargs: Any,
     ) -> bool:
         """Update parameters of the collection
 
         Args:
             collection_name: Name of the collection
-            optimizer_config: Override for optimizer configuration
+            optimizers_config: Override for optimizer configuration
             collection_params: Override for collection parameters
             timeout:
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
-
         Returns:
             Operation result
         """
+        if "optimizer_config" in kwargs and optimizers_config is not None:
+            raise ValueError(
+                "Only one of optimizer_config and optimizers_config should be specified"
+            )
+
+        if "optimizer_config" in kwargs:
+            optimizers_config = kwargs.pop("optimizer_config")
+
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.update_collection(
             collection_name=collection_name,
-            optimizer_config=optimizer_config,
+            optimizers_config=optimizers_config,
             collection_params=collection_params,
             timeout=timeout,
             **kwargs,
         )
 
     def delete_collection(
         self, collection_name: str, timeout: Optional[int] = None, **kwargs: Any
@@ -1179,14 +1247,16 @@
             timeout:
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_collection(
             collection_name=collection_name, timeout=timeout, **kwargs
         )
 
     def create_collection(
         self,
         collection_name: str,
@@ -1236,14 +1306,16 @@
             timeout:
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.create_collection(
             collection_name=collection_name,
             vectors_config=vectors_config,
             shard_number=shard_number,
             replication_factor=replication_factor,
             write_consistency_factor=write_consistency_factor,
             on_disk_payload=on_disk_payload,
@@ -1305,14 +1377,15 @@
             timeout:
                 Wait for operation commit timeout in seconds.
                 If timeout is reached - request will return with service error.
 
         Returns:
             Operation result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
 
         return self._client.recreate_collection(
             collection_name=collection_name,
             vectors_config=vectors_config,
             shard_number=shard_number,
             replication_factor=replication_factor,
             write_consistency_factor=write_consistency_factor,
@@ -1346,14 +1419,16 @@
             batch_size: How many vectors upload per-request, Default: 64
             parallel: Number of parallel processes of upload
             method: Start method for parallel processes, Default: forkserver
             max_retries: maximum number of retries in case of a failure
                 during the upload of a batch
 
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.upload_records(
             collection_name=collection_name,
             records=records,
             batch_size=batch_size,
             parallel=parallel,
             method=method,
             max_retries=max_retries,
@@ -1384,14 +1459,16 @@
             ids: Iterable of custom vectors ids, Optional, Default: None
             batch_size: How many vectors upload per-request, Default: 64
             parallel: Number of parallel processes of upload
             method: Start method for parallel processes, Default: forkserver
             max_retries: maximum number of retries in case of a failure
                 during the upload of a batch
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.upload_collection(
             collection_name=collection_name,
             vectors=vectors,
             payload=payload,
             ids=ids,
             batch_size=batch_size,
             parallel=parallel,
@@ -1429,14 +1506,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation Result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.create_payload_index(
             collection_name=collection_name,
             field_name=field_name,
             field_schema=field_schema,
             field_type=field_type,
             wait=wait,
             ordering=ordering,
@@ -1467,14 +1546,16 @@
                     may be inconsistent for a short period of time in case of leader change
                 - 'strong' - Write operations go through the permanent leader,
                     consistent, but may be unavailable if leader is down
 
         Returns:
             Operation Result
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_payload_index(
             collection_name=collection_name,
             field_name=field_name,
             wait=wait,
             ordering=ordering,
             **kwargs,
         )
@@ -1486,68 +1567,80 @@
 
         Args:
             collection_name: Name of the collection
 
         Returns:
             List of snapshots
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.list_snapshots(collection_name=collection_name, **kwargs)
 
     def create_snapshot(
         self, collection_name: str, **kwargs: Any
     ) -> Optional[types.SnapshotDescription]:
         """Create snapshot for a given collection.
 
         Args:
             collection_name: Name of the collection
 
         Returns:
             Snapshot description
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.create_snapshot(collection_name=collection_name, **kwargs)
 
     def delete_snapshot(self, collection_name: str, snapshot_name: str, **kwargs: Any) -> bool:
         """Delete snapshot for a given collection.
 
         Args:
             collection_name: Name of the collection
             snapshot_name: Snapshot id
 
         Returns:
             True if snapshot was deleted
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_snapshot(
             collection_name=collection_name, snapshot_name=snapshot_name, **kwargs
         )
 
     def list_full_snapshots(self, **kwargs: Any) -> List[types.SnapshotDescription]:
         """List all snapshots for a whole storage
 
         Returns:
             List of snapshots
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.list_full_snapshots(**kwargs)
 
     def create_full_snapshot(self, **kwargs: Any) -> types.SnapshotDescription:
         """Create snapshot for a whole storage.
 
         Returns:
             Snapshot description
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.create_full_snapshot(**kwargs)
 
     def delete_full_snapshot(self, snapshot_name: str, **kwargs: Any) -> bool:
         """Delete snapshot for a whole storage.
 
         Args:
             snapshot_name: Snapshot name
 
         Returns:
             True if snapshot was deleted
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.delete_full_snapshot(snapshot_name=snapshot_name, **kwargs)
 
     def recover_snapshot(
         self,
         collection_name: str,
         location: str,
         priority: Optional[types.SnapshotPriority] = None,
@@ -1565,25 +1658,33 @@
             priority:
                 Defines source of truth for snapshot recovery
                     - `snapshot` means - prefer snapshot data over the current state
                     - `replica` means - prefer existing data over the snapshot
                 Default: `replica`
 
         """
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.recover_snapshot(
             collection_name=collection_name,
             location=location,
             priority=priority,
             **kwargs,
         )
 
     def lock_storage(self, reason: str, **kwargs: Any) -> types.LocksOption:
         """Lock storage for writing."""
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.lock_storage(reason=reason, **kwargs)
 
     def unlock_storage(self, **kwargs: Any) -> types.LocksOption:
         """Unlock storage for writing."""
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.unlock_storage(**kwargs)
 
     def get_locks(self, **kwargs: Any) -> types.LocksOption:
         """Get current locks state."""
+        assert len(kwargs) == 0, f"Unknown arguments: {list(kwargs.keys())}"
+
         return self._client.get_locks(**kwargs)
```

### Comparing `qdrant_client-1.2.0/qdrant_client/qdrant_remote.py` & `qdrant_client-1.3.0/qdrant_client/qdrant_remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 import numpy as np
 from urllib3.util import Url, parse_url
 
 from qdrant_client import grpc as grpc
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.connection import get_async_channel, get_channel
 from qdrant_client.conversions import common_types as types
-from qdrant_client.conversions.conversion import GrpcToRest, RestToGrpc
+from qdrant_client.conversions.conversion import (
+    GrpcToRest,
+    RestToGrpc,
+    grpc_payload_schema_to_field_type,
+)
 from qdrant_client.http import ApiClient, SyncApis
 from qdrant_client.http import models
 from qdrant_client.http import models as rest_models
 from qdrant_client.parallel_processor import ParallelWorkerPool
 from qdrant_client.uploader.grpc_uploader import GrpcBatchUploader
 from qdrant_client.uploader.rest_uploader import RestBatchUploader
 from qdrant_client.uploader.uploader import BaseUploader
@@ -61,14 +65,19 @@
         if host is not None and (host.startswith("http://") or host.startswith("https://")):
             raise ValueError(
                 f"`host` param is not expected to contain protocol (http:// or https://). "
                 f"Try to use `url` parameter instead."
             )
 
         elif url:
+            if url.startswith("localhost"):
+                # Handle for a special case when url is localhost:port
+                # Which is not parsed correctly by urllib
+                url = f"//{url}"
+
             parsed_url: Url = parse_url(url)
             self._host, self._port = parsed_url.host, parsed_url.port
 
             if parsed_url.scheme:
                 self._https = parsed_url.scheme == "https"
                 self._scheme = parsed_url.scheme
 
@@ -120,74 +129,81 @@
             self._rest_args["timeout"] = self._timeout
 
         self.openapi_client: SyncApis[ApiClient] = SyncApis(host=self.rest_uri, **self._rest_args)
 
         self._grpc_channel = None
         self._grpc_points_client: Optional[grpc.PointsStub] = None
         self._grpc_collections_client: Optional[grpc.CollectionsStub] = None
+        self._grpc_snapshots_client: Optional[grpc.SnapshotsStub] = None
 
         self._aio_grpc_channel = None
         self._aio_grpc_points_client: Optional[grpc.PointsStub] = None
         self._aio_grpc_collections_client: Optional[grpc.CollectionsStub] = None
+        self._aio_grpc_snapshots_client: Optional[grpc.SnapshotsStub] = None
 
     def __del__(self) -> None:
         if hasattr(self, "_grpc_channel") and self._grpc_channel is not None:
-            self._grpc_channel.close()
+            try:
+                self._grpc_channel.close()
+            except AttributeError:
+                logging.warning("Connection was interrupted on server side")
 
     @staticmethod
     def _parse_url(url: str) -> Tuple[Optional[str], str, Optional[int], Optional[str]]:
         parse_result: Url = parse_url(url)
         scheme, host, port, prefix = (
             parse_result.scheme,
             parse_result.host,
             parse_result.port,
             parse_result.path,
         )
         return scheme, host, port, prefix
 
-    def _init_grpc_points_client(self) -> None:
+    def _init_grpc_channel(self) -> None:
         if self._grpc_channel is None:
             self._grpc_channel = get_channel(
                 host=self._host,
                 port=self._grpc_port,
                 ssl=self._https,
                 metadata=self._grpc_headers,
             )
-        self._grpc_points_client = grpc.PointsStub(self._grpc_channel)
 
-    def _init_grpc_collections_client(self) -> None:
-        if self._grpc_channel is None:
-            self._grpc_channel = get_channel(
+    def _init_async_grpc_channel(self) -> None:
+        if self._aio_grpc_channel is None:
+            self._aio_grpc_channel = get_async_channel(
                 host=self._host,
                 port=self._grpc_port,
                 ssl=self._https,
                 metadata=self._grpc_headers,
             )
+
+    def _init_grpc_points_client(self) -> None:
+        self._init_grpc_channel()
+        self._grpc_points_client = grpc.PointsStub(self._grpc_channel)
+
+    def _init_grpc_collections_client(self) -> None:
+        self._init_grpc_channel()
         self._grpc_collections_client = grpc.CollectionsStub(self._grpc_channel)
 
+    def _init_grpc_snapshots_client(self) -> None:
+        self._init_grpc_channel()
+        self._grpc_snapshots_client = grpc.SnapshotsStub(self._grpc_channel)
+
     def _init_async_grpc_points_client(self) -> None:
-        if self._aio_grpc_channel is None:
-            self._aio_grpc_channel = get_async_channel(
-                host=self._host,
-                port=self._grpc_port,
-                ssl=self._https,
-                metadata=self._grpc_headers,
-            )
+        self._init_async_grpc_channel()
         self._aio_grpc_points_client = grpc.PointsStub(self._aio_grpc_channel)
 
     def _init_async_grpc_collections_client(self) -> None:
-        if self._aio_grpc_channel is None:
-            self._aio_grpc_channel = get_async_channel(
-                host=self._host,
-                port=self._grpc_port,
-                ssl=self._https,
-                metadata=self._grpc_headers,
-            )
+        self._init_async_grpc_channel()
         self._aio_grpc_collections_client = grpc.CollectionsStub(self._aio_grpc_channel)
 
+    def _init_async_grpc_snapshots_client(self) -> None:
+        self._init_async_grpc_channel()
+        self._aio_grpc_snapshots_client = grpc.SnapshotsStub(self._aio_grpc_channel)
+
     @property
     def async_grpc_collections(self) -> grpc.CollectionsStub:
         """gRPC client for collections methods
 
         Returns:
             An instance of raw gRPC client, generated from Protobuf
         """
@@ -203,14 +219,25 @@
             An instance of raw gRPC client, generated from Protobuf
         """
         if self._aio_grpc_points_client is None:
             self._init_async_grpc_points_client()
         return self._aio_grpc_points_client
 
     @property
+    def async_grpc_snapshots(self) -> grpc.SnapshotsStub:
+        """gRPC client for snapshots methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if self._aio_grpc_snapshots_client is None:
+            self._init_async_grpc_snapshots_client()
+        return self._aio_grpc_snapshots_client
+
+    @property
     def grpc_collections(self) -> grpc.CollectionsStub:
         """gRPC client for collections methods
 
         Returns:
             An instance of raw gRPC client, generated from Protobuf
         """
         if self._grpc_collections_client is None:
@@ -225,14 +252,25 @@
             An instance of raw gRPC client, generated from Protobuf
         """
         if self._grpc_points_client is None:
             self._init_grpc_points_client()
         return self._grpc_points_client
 
     @property
+    def grpc_snapshots(self) -> grpc.SnapshotsStub:
+        """gRPC client for snapshots methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if self._grpc_snapshots_client is None:
+            self._init_grpc_snapshots_client()
+        return self._grpc_snapshots_client
+
+    @property
     def rest(self) -> SyncApis[ApiClient]:
         """REST Client
 
         Returns:
             An instance of raw REST API client, generated from OpenAPI schema
         """
         return self.openapi_client
@@ -423,20 +461,27 @@
         query_filter: Optional[models.Filter] = None,
         search_params: Optional[models.SearchParams] = None,
         limit: int = 10,
         group_size: int = 1,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         consistency: Optional[types.ReadConsistency] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         if self._prefer_grpc:
             vector_name = None
 
+            if isinstance(with_lookup, rest_models.WithLookup):
+                with_lookup = RestToGrpc.convert_with_lookup(with_lookup)
+
+            if isinstance(with_lookup, str):
+                with_lookup = grpc.WithLookup(lookup=with_lookup)
+
             if isinstance(query_vector, types.NamedVector):
                 vector = query_vector.vector
                 vector_name = query_vector.name
 
             elif isinstance(query_vector, tuple):
                 vector_name = query_vector[0]
                 vector = query_vector[1]
@@ -482,25 +527,32 @@
                     group_size=group_size,
                     with_vectors=with_vectors,
                     with_payload=with_payload,
                     params=search_params,
                     score_threshold=score_threshold,
                     group_by=group_by,
                     read_consistency=consistency,
+                    with_lookup=with_lookup,
                 ),
                 timeout=self._timeout,
             ).result
 
             return GrpcToRest.convert_groups_result(result)
         else:
+            if isinstance(with_lookup, grpc.WithLookup):
+                with_lookup = GrpcToRest.convert_with_lookup(with_lookup)
+
             if isinstance(query_vector, tuple):
                 query_vector = rest_models.NamedVector.construct(
                     name=query_vector[0], vector=query_vector[1]
                 )
 
+            if isinstance(query_vector, np.ndarray):
+                query_vector = query_vector.tolist()
+
             if isinstance(query_filter, grpc.Filter):
                 query_filter = GrpcToRest.convert_filter(model=query_filter)
 
             if isinstance(search_params, grpc.SearchParams):
                 search_params = GrpcToRest.convert_search_params(search_params)
 
             if isinstance(with_payload, grpc.WithPayloadSelector):
@@ -512,14 +564,15 @@
                 params=search_params,
                 with_payload=with_payload,
                 with_vector=with_vectors,
                 score_threshold=score_threshold,
                 group_by=group_by,
                 group_size=group_size,
                 limit=limit,
+                with_lookup=with_lookup,
             )
 
             return self.openapi_client.points_api.search_point_groups(
                 search_groups_request=search_groups_request,
                 collection_name=collection_name,
                 consistency=consistency,
             ).result
@@ -715,21 +768,28 @@
         limit: int = 10,
         group_size: int = 1,
         score_threshold: Optional[float] = None,
         with_payload: Union[bool, Sequence[str], models.PayloadSelector] = True,
         with_vectors: Union[bool, Sequence[str]] = False,
         using: Optional[str] = None,
         lookup_from: Optional[models.LookupLocation] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
         consistency: Optional[models.ReadConsistencyType] = None,
         **kwargs: Any,
     ) -> types.GroupsResult:
         if negative is None:
             negative = []
 
         if self._prefer_grpc:
+            if isinstance(with_lookup, rest_models.WithLookup):
+                with_lookup = RestToGrpc.convert_with_lookup(with_lookup)
+
+            if isinstance(with_lookup, str):
+                with_lookup = grpc.WithLookup(lookup_index=with_lookup)
+
             positive = [
                 RestToGrpc.convert_extended_point_id(point_id)
                 if isinstance(point_id, (str, int))
                 else point_id
                 for point_id in positive
             ]
 
@@ -784,21 +844,25 @@
                     with_vectors=with_vectors,
                     with_payload=with_payload,
                     params=search_params,
                     score_threshold=score_threshold,
                     using=using,
                     lookup_from=lookup_from,
                     read_consistency=consistency,
+                    with_lookup=with_lookup,
                 ),
                 timeout=self._timeout,
             ).result
 
             assert res is not None, "Recommend groups API returned None"
             return GrpcToRest.convert_groups_result(res)
         else:
+            if isinstance(with_lookup, grpc.WithLookup):
+                with_lookup = GrpcToRest.convert_with_lookup(with_lookup)
+
             positive = [
                 GrpcToRest.convert_point_id(point_id)
                 if isinstance(point_id, grpc.PointId)
                 else point_id
                 for point_id in positive
             ]
 
@@ -833,14 +897,15 @@
                     group_size=group_size,
                     params=search_params,
                     with_payload=with_payload,
                     with_vector=with_vectors,
                     score_threshold=score_threshold,
                     lookup_from=lookup_from,
                     using=using,
+                    with_lookup=with_lookup,
                 ),
             ).result
 
             assert result is not None, "Recommend points API returned None"
             return result
 
     def scroll(
@@ -932,14 +997,25 @@
     def count(
         self,
         collection_name: str,
         count_filter: Optional[types.Filter] = None,
         exact: bool = True,
         **kwargs: Any,
     ) -> types.CountResult:
+        if self._prefer_grpc:
+            if isinstance(count_filter, rest_models.Filter):
+                count_filter = RestToGrpc.convert_filter(model=count_filter)
+            response = self.grpc_points.Count(
+                grpc.CountPoints(
+                    collection_name=collection_name, filter=count_filter, exact=exact
+                ),
+                timeout=self._timeout,
+            ).result
+            return GrpcToRest.convert_count_result(response)
+
         if isinstance(count_filter, grpc.Filter):
             count_filter = GrpcToRest.convert_filter(model=count_filter)
 
         count_result = self.openapi_client.points_api.count_points(
             collection_name=collection_name,
             count_request=rest_models.CountRequest(filter=count_filter, exact=exact),
         ).result
@@ -1447,14 +1523,29 @@
 
     def update_collection_aliases(
         self,
         change_aliases_operations: Sequence[types.AliasOperations],
         timeout: Optional[int] = None,
         **kwargs: Any,
     ) -> bool:
+        if self._prefer_grpc:
+            change_aliases_operation = [
+                RestToGrpc.convert_alias_operations(operation)
+                if not isinstance(operation, grpc.AliasOperations)
+                else operation
+                for operation in change_aliases_operations
+            ]
+            return self.grpc_collections.UpdateAliases(
+                grpc.ChangeAliases(
+                    timeout=timeout,
+                    actions=change_aliases_operation,
+                ),
+                timeout=self._timeout,
+            ).result
+
         change_aliases_operation = [
             GrpcToRest.convert_alias_operations(operation)
             if isinstance(operation, grpc.AliasOperations)
             else operation
             for operation in change_aliases_operations
         ]
         result: Optional[bool] = self.http.collections_api.update_aliases(
@@ -1465,23 +1556,43 @@
         ).result
         assert result is not None, "Update aliases returned None"
         return result
 
     def get_collection_aliases(
         self, collection_name: str, **kwargs: Any
     ) -> types.CollectionsAliasesResponse:
+        if self._prefer_grpc:
+            response = self.grpc_collections.ListCollectionAliases(
+                grpc.ListCollectionAliasesRequest(collection_name=collection_name),
+                timeout=self._timeout,
+            ).aliases
+            return types.CollectionsAliasesResponse(
+                aliases=[
+                    GrpcToRest.convert_alias_description(description) for description in response
+                ]
+            )
+
         result: Optional[
             types.CollectionsAliasesResponse
         ] = self.http.collections_api.get_collection_aliases(
             collection_name=collection_name
         ).result
         assert result is not None, "Get collection aliases returned None"
         return result
 
     def get_aliases(self, **kwargs: Any) -> types.CollectionsAliasesResponse:
+        if self._prefer_grpc:
+            response = self.grpc_collections.ListAliases(
+                grpc.ListAliasesRequest(), timeout=self._timeout
+            ).aliases
+            return types.CollectionsAliasesResponse(
+                aliases=[
+                    GrpcToRest.convert_alias_description(description) for description in response
+                ]
+            )
         result: Optional[
             types.CollectionsAliasesResponse
         ] = self.http.collections_api.get_collections_aliases().result
         assert result is not None, "Get aliases returned None"
         return result
 
     def get_collections(self, **kwargs: Any) -> types.CollectionsResponse:
@@ -1515,38 +1626,60 @@
         ).result
         assert result is not None, "Get collection returned None"
         return result
 
     def update_collection(
         self,
         collection_name: str,
-        optimizer_config: Optional[types.OptimizersConfigDiff] = None,
+        optimizers_config: Optional[types.OptimizersConfigDiff] = None,
         collection_params: Optional[types.CollectionParamsDiff] = None,
         timeout: Optional[int] = None,
         **kwargs: Any,
     ) -> bool:
-        if isinstance(optimizer_config, grpc.OptimizersConfigDiff):
-            optimizer_config = GrpcToRest.convert_optimizers_config_diff(optimizer_config)
+        if self._prefer_grpc:
+            if isinstance(optimizers_config, rest_models.OptimizersConfigDiff):
+                optimizers_config = RestToGrpc.convert_optimizers_config_diff(optimizers_config)
+
+            if isinstance(collection_params, rest_models.CollectionParamsDiff):
+                collection_params = RestToGrpc.convert_collection_params_diff(collection_params)
+
+            return self.grpc_collections.Update(
+                grpc.UpdateCollection(
+                    collection_name=collection_name,
+                    optimizers_config=optimizers_config,
+                    params=collection_params,
+                ),
+                timeout=self._timeout,
+            ).result
+
+        if isinstance(optimizers_config, grpc.OptimizersConfigDiff):
+            optimizers_config = GrpcToRest.convert_optimizers_config_diff(optimizers_config)
 
         if isinstance(collection_params, grpc.CollectionParamsDiff):
             collection_params = GrpcToRest.convert_collection_params_diff(collection_params)
 
         result: Optional[bool] = self.http.collections_api.update_collection(
             collection_name,
             update_collection=rest_models.UpdateCollection(
-                optimizers_config=optimizer_config, params=collection_params
+                optimizers_config=optimizers_config, params=collection_params
             ),
             timeout=timeout,
         ).result
         assert result is not None, "Update collection returned None"
         return result
 
     def delete_collection(
         self, collection_name: str, timeout: Optional[int] = None, **kwargs: Any
     ) -> bool:
+        if self._prefer_grpc:
+            return self.grpc_collections.Delete(
+                grpc.DeleteCollection(collection_name=collection_name),
+                timeout=self._timeout,
+            ).result
+
         result: Optional[bool] = self.http.collections_api.delete_collection(
             collection_name, timeout=timeout
         ).result
         assert result is not None, "Delete collection returned None"
         return result
 
     def create_collection(
@@ -1561,14 +1694,49 @@
         optimizers_config: Optional[types.OptimizersConfigDiff] = None,
         wal_config: Optional[types.WalConfigDiff] = None,
         quantization_config: Optional[types.QuantizationConfig] = None,
         init_from: Optional[types.InitFrom] = None,
         timeout: Optional[int] = None,
         **kwargs: Any,
     ) -> bool:
+        if self._prefer_grpc:
+            if isinstance(vectors_config, (rest_models.VectorParams, dict)):
+                vectors_config = RestToGrpc.convert_vectors_config(vectors_config)
+
+            if isinstance(hnsw_config, rest_models.HnswConfigDiff):
+                hnsw_config = RestToGrpc.convert_hnsw_config_diff(hnsw_config)
+
+            if isinstance(optimizers_config, rest_models.OptimizersConfigDiff):
+                optimizers_config = RestToGrpc.convert_optimizers_config_diff(optimizers_config)
+
+            if isinstance(wal_config, rest_models.WalConfigDiff):
+                wal_config = RestToGrpc.convert_wal_config_diff(wal_config)
+
+            if isinstance(
+                quantization_config,
+                (rest_models.ScalarQuantization, rest_models.ProductQuantization),
+            ):
+                quantization_config = RestToGrpc.convert_quantization_config(quantization_config)
+
+            create_collection = grpc.CreateCollection(
+                collection_name=collection_name,
+                hnsw_config=hnsw_config,
+                wal_config=wal_config,
+                optimizers_config=optimizers_config,
+                shard_number=shard_number,
+                on_disk_payload=on_disk_payload,
+                timeout=timeout,
+                vectors_config=vectors_config,
+                replication_factor=replication_factor,
+                write_consistency_factor=write_consistency_factor,
+                init_from_collection=init_from,
+                quantization_config=quantization_config,
+            )
+            return self.grpc_collections.Create(create_collection).result
+
         if isinstance(hnsw_config, grpc.HnswConfigDiff):
             hnsw_config = GrpcToRest.convert_hnsw_config_diff(hnsw_config)
 
         if isinstance(optimizers_config, grpc.OptimizersConfigDiff):
             optimizers_config = GrpcToRest.convert_optimizers_config_diff(optimizers_config)
 
         if isinstance(wal_config, grpc.WalConfigDiff):
@@ -1724,17 +1892,54 @@
         ordering: Optional[types.WriteOrdering] = None,
         **kwargs: Any,
     ) -> types.UpdateResult:
         if field_type is not None:
             warnings.warn("field_type is deprecated, use field_schema instead", DeprecationWarning)
             field_schema = field_type
 
+        if self._prefer_grpc:
+            field_index_params = None
+            if isinstance(field_schema, rest_models.PayloadSchemaType):
+                field_schema = RestToGrpc.convert_payload_schema_type(field_schema)
+
+            if isinstance(field_schema, int):
+                # There are no means to distinguish grpc.PayloadSchemaType and grpc.FieldType,
+                # as both of them are just ints
+                # method signature assumes that grpc.PayloadSchemaType is passed,
+                # otherwise the value will be corrupted
+                field_schema = grpc_payload_schema_to_field_type(field_schema)
+
+            if isinstance(field_schema, rest_models.TextIndexParams):
+                field_index_params = grpc.PayloadIndexParams(
+                    text_index_params=RestToGrpc.convert_text_index_params(field_schema)
+                )
+                field_schema = grpc.FieldType.FieldTypeText
+
+            if isinstance(field_schema, grpc.PayloadIndexParams):
+                field_index_params = field_schema
+                field_schema = grpc.FieldType.FieldTypeText
+
+            request = grpc.CreateFieldIndexCollection(
+                collection_name=collection_name,
+                field_name=field_name,
+                field_type=field_schema,
+                field_index_params=field_index_params,
+                wait=wait,
+                ordering=ordering,
+            )
+            return GrpcToRest.convert_update_result(
+                self.grpc_points.CreateFieldIndex(request).result
+            )
+
         if isinstance(field_schema, int):  # type(grpc.PayloadSchemaType) == int
             field_schema = GrpcToRest.convert_payload_schema_type(field_schema)
 
+        if isinstance(field_schema, grpc.PayloadIndexParams):
+            field_schema = GrpcToRest.convert_payload_schema_params(field_schema)
+
         result: Optional[
             types.UpdateResult
         ] = self.openapi_client.collections_api.create_field_index(
             collection_name=collection_name,
             create_field_index=rest_models.CreateFieldIndex(
                 field_name=field_name, field_schema=field_schema
             ),
@@ -1748,60 +1953,108 @@
         self,
         collection_name: str,
         field_name: str,
         wait: bool = True,
         ordering: Optional[types.WriteOrdering] = None,
         **kwargs: Any,
     ) -> types.UpdateResult:
+        if self._prefer_grpc:
+            request = grpc.DeleteFieldIndexCollection(
+                collection_name=collection_name,
+                field_name=field_name,
+                wait=wait,
+                ordering=ordering,
+            )
+            return GrpcToRest.convert_update_result(
+                self.grpc_points.DeleteFieldIndex(request).result
+            )
+
         result: Optional[
             types.UpdateResult
         ] = self.openapi_client.collections_api.delete_field_index(
             collection_name=collection_name,
             field_name=field_name,
             wait=wait,
             ordering=ordering,
         ).result
         assert result is not None, "Delete field index returned None"
         return result
 
     def list_snapshots(
         self, collection_name: str, **kwargs: Any
     ) -> List[types.SnapshotDescription]:
+        if self._prefer_grpc:
+            snapshots = self.grpc_snapshots.List(
+                grpc.ListSnapshotsRequest(collection_name=collection_name)
+            ).snapshot_descriptions
+            return [GrpcToRest.convert_snapshot_description(snapshot) for snapshot in snapshots]
+
         snapshots = self.openapi_client.collections_api.list_snapshots(
             collection_name=collection_name
         ).result
         assert snapshots is not None, "List snapshots API returned None result"
         return snapshots
 
     def create_snapshot(
         self, collection_name: str, **kwargs: Any
     ) -> Optional[types.SnapshotDescription]:
+        if self._prefer_grpc:
+            snapshot = self.grpc_snapshots.Create(
+                grpc.CreateSnapshotRequest(collection_name=collection_name)
+            ).snapshot_description
+            return GrpcToRest.convert_snapshot_description(snapshot)
+
         return self.openapi_client.collections_api.create_snapshot(
             collection_name=collection_name
         ).result
 
     def delete_snapshot(self, collection_name: str, snapshot_name: str, **kwargs: Any) -> bool:
+        if self._prefer_grpc:
+            self.grpc_snapshots.Delete(
+                grpc.DeleteSnapshotRequest(
+                    collection_name=collection_name, snapshot_name=snapshot_name
+                )
+            )
+            return True
+
         result: Optional[bool] = self.openapi_client.collections_api.delete_snapshot(
             collection_name=collection_name,
             snapshot_name=snapshot_name,
         ).result
         assert result is not None, "Delete snapshot API returned None"
         return result
 
     def list_full_snapshots(self, **kwargs: Any) -> List[types.SnapshotDescription]:
+        if self._prefer_grpc:
+            snapshots = self.grpc_snapshots.ListFull(
+                grpc.ListFullSnapshotsRequest()
+            ).snapshot_descriptions
+            return [GrpcToRest.convert_snapshot_description(snapshot) for snapshot in snapshots]
+
         snapshots = self.openapi_client.snapshots_api.list_full_snapshots().result
         assert snapshots is not None, "List full snapshots API returned None result"
         return snapshots
 
     def create_full_snapshot(self, **kwargs: Any) -> types.SnapshotDescription:
+        if self._prefer_grpc:
+            snapshot_description = self.grpc_snapshots.CreateFull(
+                grpc.CreateFullSnapshotRequest()
+            ).snapshot_description
+            return GrpcToRest.convert_snapshot_description(snapshot_description)
+
         snapshot_description = self.openapi_client.snapshots_api.create_full_snapshot().result
         assert snapshot_description is not None, "Create full snapshot API returned None result"
         return snapshot_description
 
     def delete_full_snapshot(self, snapshot_name: str, **kwargs: Any) -> bool:
+        if self._prefer_grpc:
+            self.grpc_snapshots.DeleteFull(
+                grpc.DeleteFullSnapshotRequest(snapshot_name=snapshot_name)
+            )
+            return True
         result: Optional[bool] = self.openapi_client.snapshots_api.delete_full_snapshot(
             snapshot_name=snapshot_name,
         ).result
         assert result is not None, "Delete full snapshot API returned None"
         return result
 
     def recover_snapshot(
```

### Comparing `qdrant_client-1.2.0/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.3.0/qdrant_client/uploader/grpc_uploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,24 +28,20 @@
         )
         for idx, vector, payload in zip(ids_batch, vectors_batch, payload_batch)
     ]
 
     for attempt in range(max_retries):
         try:
             points_client.Upsert(grpc.UpsertPoints(collection_name=collection_name, points=points))
-            return True
-        except Exception as e:  # pylint: disable=broad-except
-            if attempt == (max_retries - 1):
-                logging.exception(e)
-                return False
-        else:
-            logging.warn(f"Batch upload failed {attempt + 1} times. Retrying...")
-            continue
+        except Exception as e:
+            logging.warning(f"Batch upload failed {attempt + 1} times. Retrying...")
 
-    return False  # suppress mypy complaints
+            if attempt == max_retries - 1:
+                raise e
+    return True
 
 
 class GrpcBatchUploader(BaseUploader):
     def __init__(
         self,
         host: str,
         port: int,
```

### Comparing `qdrant_client-1.2.0/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.3.0/qdrant_client/uploader/rest_uploader.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,14 @@
     openapi_client: SyncApis,
     collection_name: str,
     batch: Union[Tuple, Batch],
     max_retries: int,
 ) -> bool:
     ids_batch, vectors_batch, payload_batch = batch
 
-    # Make sure we do not send too many ids in case there is an iterable over vectors,
-    # and we do not know how many ids are required in advance
-    if len(ids_batch) > len(vectors_batch):
-        ids_batch = ids_batch[: len(vectors_batch)]
-
     if payload_batch is not None:
         payload_batch = list(payload_batch)
     else:
         payload_batch = (None for _ in count())
 
     points = [
         PointStruct(
@@ -36,24 +31,20 @@
 
     for attempt in range(max_retries):
         try:
             openapi_client.points_api.upsert_points(
                 collection_name=collection_name,
                 point_insert_operations=PointsList(points=points),
             )
-            return True
         except Exception as e:
-            if attempt == (max_retries - 1):  # pylint: disable=broad-except
-                logging.exception(e)
-                return False
-        else:
-            logging.warn(f"Batch upload failed {attempt + 1} times. Retrying...")
-            continue
+            logging.warning(f"Batch upload failed {attempt + 1} times. Retrying...")
 
-    return False  # suppress mypy complaints
+            if attempt == max_retries - 1:
+                raise e
+    return True
 
 
 class RestBatchUploader(BaseUploader):
     def __init__(self, uri: str, collection_name: str, max_retries: int, **kwargs: Any):
         self.collection_name = collection_name
         self.openapi_client: SyncApis = SyncApis(host=uri, **kwargs)
         self.max_retries = max_retries
```

### Comparing `qdrant_client-1.2.0/qdrant_client/uploader/uploader.py` & `qdrant_client-1.3.0/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.2.0/PKG-INFO` & `qdrant_client-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,15 @@
 Client library and SDK for the [Qdrant](https://github.com/qdrant/qdrant) vector search engine.
 
 Library contains type definitions for all Qdrant API and allows to make both Sync and Async requests.
 
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/qdrant/redoc/index.html) directly.
 It also provides some additional helper methods for frequently required operations, e.g. initial collection uploading.
 
-See [QuickStart](https://qdrant.tech/documentation/quick_start/#create-collection) for more details!
+See [QuickStart](https://qdrant.tech/documentation/quick-start/#create-collection) for more details!
 
 ## Installation
 
 ```
 pip install qdrant-client
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.2.0 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.3.0 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -18,15 +18,15 @@
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
 definitions for all Qdrant API and allows to make both Sync and Async requests.
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/
 qdrant/redoc/index.html) directly. It also provides some additional helper
 methods for frequently required operations, e.g. initial collection uploading.
-See [QuickStart](https://qdrant.tech/documentation/quick_start/#create-
+See [QuickStart](https://qdrant.tech/documentation/quick-start/#create-
 collection) for more details! ## Installation ``` pip install qdrant-client ```
 ## Features - Type hints for all API methods - Local mode - use same API
 without running server - REST and gRPC support - Minimal dependencies ## Local
 mode
                                     [Qdrant]
 Python client allows you to run same code in local mode without running Qdrant
 server. Simply initialize client like this: ```python from qdrant_client import
```

