# Comparing `tmp/aserto-directory-0.0.1rc1.tar.gz` & `tmp/aserto-directory-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aserto-directory-0.0.1rc1.tar", max compression
+gzip compressed data, was "aserto-directory-0.21.0.tar", max compression
```

## Comparing `aserto-directory-0.0.1rc1.tar` & `aserto-directory-0.21.0.tar`

### file list

```diff
@@ -1,30 +1,43 @@
--rw-r--r--   0        0        0    11357 2022-10-22 23:48:08.925669 aserto-directory-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0      936 2022-10-23 17:05:38.091144 aserto-directory-0.0.1rc1/README.md
--rw-r--r--   0        0        0     1809 2022-10-23 17:27:00.170877 aserto-directory-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0      713 2022-10-23 17:31:22.425738 aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/__init__.py
--rw-r--r--   0        0        0     8252 2022-10-23 17:31:22.345683 aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2.py
--rw-r--r--   0        0        0    23803 2022-10-23 17:31:22.349492 aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2.pyi
--rw-r--r--   0        0        0      159 2022-10-23 17:31:22.347054 aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-10-23 17:31:22.347668 aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2_grpc.pyi
--rw-r--r--   0        0        0      383 2022-10-23 17:31:22.425902 aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/__init__.py
--rw-r--r--   0        0        0     3579 2022-10-23 17:31:22.345880 aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2.py
--rw-r--r--   0        0        0     6380 2022-10-23 17:31:22.349318 aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2.pyi
--rw-r--r--   0        0        0     2796 2022-10-23 17:31:22.346206 aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py
--rw-r--r--   0        0        0      841 2022-10-23 17:31:22.349399 aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi
--rw-r--r--   0        0        0      423 2022-10-23 17:31:22.425649 aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/__init__.py
--rw-r--r--   0        0        0     3813 2022-10-23 17:31:22.349398 aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2.py
--rw-r--r--   0        0        0     6067 2022-10-23 17:31:22.346389 aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2.pyi
--rw-r--r--   0        0        0     2826 2022-10-23 17:31:22.346150 aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2_grpc.py
--rw-r--r--   0        0        0      877 2022-10-23 17:31:22.348857 aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi
--rw-r--r--   0        0        0     1815 2022-10-23 17:31:22.425529 aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/__init__.py
--rw-r--r--   0        0        0    11711 2022-10-23 17:31:22.347376 aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2.py
--rw-r--r--   0        0        0    26106 2022-10-23 17:31:22.347351 aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2.pyi
--rw-r--r--   0        0        0    26460 2022-10-23 17:31:22.347625 aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2_grpc.py
--rw-r--r--   0        0        0     6964 2022-10-23 17:31:22.347892 aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi
--rw-r--r--   0        0        0     1387 2022-10-23 17:31:22.425826 aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/__init__.py
--rw-r--r--   0        0        0     7774 2022-10-23 17:31:22.348229 aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2.py
--rw-r--r--   0        0        0    14250 2022-10-23 17:31:22.349331 aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2.pyi
--rw-r--r--   0        0        0    19345 2022-10-23 17:31:22.348459 aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2_grpc.py
--rw-r--r--   0        0        0     5174 2022-10-23 17:31:22.348768 aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi
--rw-r--r--   0        0        0     1885 2022-10-23 17:33:56.599305 aserto-directory-0.0.1rc1/setup.py
--rw-r--r--   0        0        0     2041 2022-10-23 17:33:56.599684 aserto-directory-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-22 23:48:08.925669 aserto-directory-0.21.0/LICENSE
+-rw-r--r--   0        0        0      952 2022-10-23 18:46:33.575812 aserto-directory-0.21.0/README.md
+-rw-r--r--   0        0        0     1806 2023-06-23 18:31:11.729512 aserto-directory-0.21.0/pyproject.toml
+-rw-r--r--   0        0        0      713 2022-10-23 17:31:22.425738 aserto-directory-0.21.0/src/aserto/directory/common/v2/__init__.py
+-rw-r--r--   0        0        0     7730 2023-05-01 21:57:11.999226 aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2.py
+-rw-r--r--   0        0        0    20055 2023-05-01 21:57:11.999459 aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2022-10-23 17:31:22.347054 aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2022-10-23 17:31:22.347668 aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2_grpc.pyi
+-rw-r--r--   0        0        0      383 2022-10-23 17:31:22.425902 aserto-directory-0.21.0/src/aserto/directory/exporter/v2/__init__.py
+-rw-r--r--   0        0        0     3579 2022-10-23 17:31:22.345880 aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2.py
+-rw-r--r--   0        0        0     6380 2022-10-23 17:31:22.349318 aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2.pyi
+-rw-r--r--   0        0        0     2796 2022-10-23 17:31:22.346206 aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py
+-rw-r--r--   0        0        0      841 2022-10-23 17:31:22.349399 aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi
+-rw-r--r--   0        0        0      423 2022-10-23 17:31:22.425649 aserto-directory-0.21.0/src/aserto/directory/importer/v2/__init__.py
+-rw-r--r--   0        0        0     3813 2022-10-23 17:31:22.349398 aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2.py
+-rw-r--r--   0        0        0     6067 2022-10-23 17:31:22.346389 aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2.pyi
+-rw-r--r--   0        0        0     2826 2022-10-23 17:31:22.346150 aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2_grpc.py
+-rw-r--r--   0        0        0      877 2022-10-23 17:31:22.348857 aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1815 2023-04-21 20:20:24.666352 aserto-directory-0.21.0/src/aserto/directory/reader/v2/__init__.py
+-rw-r--r--   0        0        0    12336 2023-04-21 20:20:24.666544 aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2.py
+-rw-r--r--   0        0        0    27701 2023-04-21 20:20:24.666746 aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2.pyi
+-rw-r--r--   0        0        0    26460 2022-10-23 17:31:22.347625 aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2_grpc.py
+-rw-r--r--   0        0        0     6964 2022-10-23 17:31:22.347892 aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi
+-rw-r--r--   0        0        0      440 2023-05-01 21:57:11.999787 aserto-directory-0.21.0/src/aserto/directory/schema/v2/__init__.py
+-rw-r--r--   0        0        0     1774 2023-04-21 20:20:24.667050 aserto-directory-0.21.0/src/aserto/directory/schema/v2/group_pb2.py
+-rw-r--r--   0        0        0      911 2023-04-21 20:20:24.667140 aserto-directory-0.21.0/src/aserto/directory/schema/v2/group_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 20:20:24.667281 aserto-directory-0.21.0/src/aserto/directory/schema/v2/group_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-21 20:20:24.667441 aserto-directory-0.21.0/src/aserto/directory/schema/v2/group_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2432 2023-04-21 20:20:24.667584 aserto-directory-0.21.0/src/aserto/directory/schema/v2/identity_pb2.py
+-rw-r--r--   0        0        0     3618 2023-04-21 20:20:24.667694 aserto-directory-0.21.0/src/aserto/directory/schema/v2/identity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 20:20:24.667797 aserto-directory-0.21.0/src/aserto/directory/schema/v2/identity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-21 20:20:24.667892 aserto-directory-0.21.0/src/aserto/directory/schema/v2/identity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2504 2023-04-21 20:20:24.668022 aserto-directory-0.21.0/src/aserto/directory/schema/v2/user_pb2.py
+-rw-r--r--   0        0        0     5621 2023-04-21 20:20:24.668136 aserto-directory-0.21.0/src/aserto/directory/schema/v2/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-21 20:20:24.668212 aserto-directory-0.21.0/src/aserto/directory/schema/v2/user_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-21 20:20:24.668289 aserto-directory-0.21.0/src/aserto/directory/schema/v2/user_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1387 2023-05-01 21:57:12.000162 aserto-directory-0.21.0/src/aserto/directory/writer/v2/__init__.py
+-rw-r--r--   0        0        0     7774 2022-10-23 17:31:22.348229 aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2.py
+-rw-r--r--   0        0        0    14250 2022-10-23 17:31:22.349331 aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2.pyi
+-rw-r--r--   0        0        0    19345 2022-10-23 17:31:22.348459 aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2_grpc.py
+-rw-r--r--   0        0        0     5174 2022-10-23 17:31:22.348768 aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1931 2023-06-23 18:42:47.525653 aserto-directory-0.21.0/setup.py
+-rw-r--r--   0        0        0     2055 2023-06-23 18:42:47.526195 aserto-directory-0.21.0/PKG-INFO
```

### Comparing `aserto-directory-0.0.1rc1/LICENSE` & `aserto-directory-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/README.md` & `aserto-directory-0.21.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 ### Using Poetry
 ```sh
 poetry add aserto-directory
 ```
 ## Usage
 ```py
 import grpc
-from aserto.directory.common.v2 import ObjectTypeRequest
-from aserto.directory.reader.v2 import ReaderStub
+from aserto.directory.reader.v2 import ReaderStub, GetObjectTypesRequest
 
-with grpc.secure_channel(target=f"directory.prod.aserto.com:8443") as channel:
+with grpc.secure_channel(
+    target="directory.prod.aserto.com:8443",
+    credentials=grpc.ssl_channel_credentials(),
+) as channel:
     reader = ReaderStub(channel)
 
     # List all object types in the directory
-    response = client.GetObjectTypes(
+    response = reader.GetObjectTypes(
         GetObjectTypesRequest(),
         metadata=(
             ("authorization", f"basic {ASERTO_DIRECTORY_API_KEY}"),
             ("aserto-tenant-id", ASERTO_TENANT_ID),
         ),
     )
 
     for object_type in response.results:
         print("Object Type:", object_type.name)
-```
```

### Comparing `aserto-directory-0.0.1rc1/pyproject.toml` & `aserto-directory-0.21.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aserto-directory"
-version = "0.0.1.rc1"
+version = "0.21.0"
 description = "gRPC client for Aserto Directory service instances"
 readme = "README.md"
 authors = ["Aserto, Inc. <pypi@aserto.com>"]
 homepage = "https://github.com/aserto-dev/python-directory"
 repository = "https://github.com/aserto-dev/python-directory"
 documentation = "https://github.com/aserto-dev/python-directory"
 license = "Apache-2.0"
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/__init__.py` & `aserto-directory-0.21.0/src/aserto/directory/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2.py` & `aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/common/v2/common.proto\x12\x1a\x61serto.directory.common.v2\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x9a\x03\n\nObjectType\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x1d\n\nis_subject\x18\x04 \x01(\x08R\tisSubject\x12\x18\n\x07ordinal\x18\x05 \x01(\x05R\x07ordinal\x12\x16\n\x06status\x18\x06 \x01(\rR\x06status\x12/\n\x06schema\x18\n \x01(\x0b\x32\x17.google.protobuf.StructR\x06schema\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x39\n\ndeleted_at\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tdeletedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hash\"\x98\x02\n\nPermission\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x39\n\ndeleted_at\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tdeletedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hash\"\xa7\x03\n\x0cRelationType\x12\x0e\n\x02id\x18\x01 \x01(\x05R\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1f\n\x0bobject_type\x18\x03 \x01(\tR\nobjectType\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName\x12\x18\n\x07ordinal\x18\x05 \x01(\x05R\x07ordinal\x12\x16\n\x06status\x18\x06 \x01(\rR\x06status\x12\x16\n\x06unions\x18\x07 \x03(\tR\x06unions\x12 \n\x0bpermissions\x18\x08 \x03(\tR\x0bpermissions\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x39\n\ndeleted_at\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tdeletedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hash\"\xdf\x02\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03key\x18\x02 \x01(\tR\x03key\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName\x12\x37\n\nproperties\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructR\nproperties\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x39\n\ndeleted_at\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tdeletedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hash\"\xf9\x02\n\x08Relation\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12\x1a\n\x08relation\x18\x02 \x01(\tR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x39\n\ndeleted_at\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tdeletedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hash\"\xb3\x02\n\x10ObjectDependency\x12\x1f\n\x0bobject_type\x18\x01 \x01(\tR\nobjectType\x12\x1b\n\tobject_id\x18\x03 \x01(\tR\x08objectId\x12\x1d\n\nobject_key\x18\x04 \x01(\tR\tobjectKey\x12\x1a\n\x08relation\x18\x05 \x01(\tR\x08relation\x12!\n\x0csubject_type\x18\x07 \x01(\tR\x0bsubjectType\x12\x1d\n\nsubject_id\x18\t \x01(\tR\tsubjectId\x12\x1f\n\x0bsubject_key\x18\n \x01(\tR\nsubjectKey\x12\x14\n\x05\x64\x65pth\x18\x0b \x01(\x05R\x05\x64\x65pth\x12\x19\n\x08is_cycle\x18\x0c \x01(\x08R\x07isCycle\x12\x12\n\x04path\x18\r \x03(\tR\x04path\"T\n\x14ObjectTypeIdentifier\x12\x13\n\x02id\x18\x01 \x01(\x05H\x00R\x02id\x88\x01\x01\x12\x17\n\x04name\x18\x02 \x01(\tH\x01R\x04name\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_name\"T\n\x14PermissionIdentifier\x12\x13\n\x02id\x18\x01 \x01(\tH\x00R\x02id\x88\x01\x01\x12\x17\n\x04name\x18\x02 \x01(\tH\x01R\x04name\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_name\"\x8c\x01\n\x16RelationTypeIdentifier\x12\x13\n\x02id\x18\x01 \x01(\x05H\x00R\x02id\x88\x01\x01\x12\x17\n\x04name\x18\x02 \x01(\tH\x01R\x04name\x88\x01\x01\x12$\n\x0bobject_type\x18\x03 \x01(\tH\x02R\nobjectType\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_nameB\x0e\n\x0c_object_type\"o\n\x10ObjectIdentifier\x12\x17\n\x04type\x18\x01 \x01(\tH\x00R\x04type\x88\x01\x01\x12\x13\n\x02id\x18\x02 \x01(\tH\x01R\x02id\x88\x01\x01\x12\x15\n\x03key\x18\x03 \x01(\tH\x02R\x03key\x88\x01\x01\x42\x07\n\x05_typeB\x05\n\x03_idB\x06\n\x04_key\"\xf2\x01\n\x12RelationIdentifier\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x02 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\"=\n\x11PaginationRequest\x12\x12\n\x04size\x18\x01 \x01(\x05R\x04size\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"T\n\x12PaginationResponse\x12\x1d\n\nnext_token\x18\x01 \x01(\tR\tnextToken\x12\x1f\n\x0bresult_size\x18\x02 \x01(\x05R\nresultSize*^\n\x04\x46lag\x12\x10\n\x0c\x46LAG_UNKNOWN\x10\x00\x12\x0f\n\x0b\x46LAG_HIDDEN\x10\x01\x12\x11\n\rFLAG_READONLY\x10\x02\x12\x0f\n\x0b\x46LAG_SYSTEM\x10\x04\x12\x0f\n\x0b\x46LAG_SHADOW\x10\x08\x42\x80\x02\n\x1e\x63om.aserto.directory.common.v2B\x0b\x43ommonProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/common/v2;common\xa2\x02\x03\x41\x44\x43\xaa\x02\x1a\x41serto.Directory.Common.V2\xca\x02\x1b\x41serto\\Directory_\\Common\\V2\xe2\x02\'Aserto\\Directory_\\Common\\V2\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Common::V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/common/v2/common.proto\x12\x1a\x61serto.directory.common.v2\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xeb\x02\n\nObjectType\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x1d\n\nis_subject\x18\x04 \x01(\x08R\tisSubject\x12\x18\n\x07ordinal\x18\x05 \x01(\x05R\x07ordinal\x12\x16\n\x06status\x18\x06 \x01(\rR\x06status\x12/\n\x06schema\x18\n \x01(\x0b\x32\x17.google.protobuf.StructR\x06schema\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hashJ\x04\x08\x01\x10\x02J\x04\x08\x16\x10\x17R\x02idR\ndeleted_at\"\xe9\x01\n\nPermission\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hashJ\x04\x08\x01\x10\x02J\x04\x08\x16\x10\x17R\x02idR\ndeleted_at\"\xf8\x02\n\x0cRelationType\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1f\n\x0bobject_type\x18\x03 \x01(\tR\nobjectType\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName\x12\x18\n\x07ordinal\x18\x05 \x01(\x05R\x07ordinal\x12\x16\n\x06status\x18\x06 \x01(\rR\x06status\x12\x16\n\x06unions\x18\x07 \x03(\tR\x06unions\x12 \n\x0bpermissions\x18\x08 \x03(\tR\x0bpermissions\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hashJ\x04\x08\x01\x10\x02J\x04\x08\x16\x10\x17R\x02idR\ndeleted_at\"\xb0\x02\n\x06Object\x12\x10\n\x03key\x18\x02 \x01(\tR\x03key\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName\x12\x37\n\nproperties\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructR\nproperties\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hashJ\x04\x08\x01\x10\x02J\x04\x08\x16\x10\x17R\x02idR\ndeleted_at\"\xd0\x02\n\x08Relation\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12\x1a\n\x08relation\x18\x02 \x01(\tR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x39\n\ncreated_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x12\n\x04hash\x18\x17 \x01(\tR\x04hashJ\x04\x08\x16\x10\x17R\ndeleted_at\"\x9a\x02\n\x10ObjectDependency\x12\x1f\n\x0bobject_type\x18\x01 \x01(\tR\nobjectType\x12\x1d\n\nobject_key\x18\x04 \x01(\tR\tobjectKey\x12\x1a\n\x08relation\x18\x05 \x01(\tR\x08relation\x12!\n\x0csubject_type\x18\x07 \x01(\tR\x0bsubjectType\x12\x1f\n\x0bsubject_key\x18\n \x01(\tR\nsubjectKey\x12\x14\n\x05\x64\x65pth\x18\x0b \x01(\x05R\x05\x64\x65pth\x12\x19\n\x08is_cycle\x18\x0c \x01(\x08R\x07isCycle\x12\x12\n\x04path\x18\r \x03(\tR\x04pathJ\x04\x08\x03\x10\x04J\x04\x08\t\x10\nR\tobject_idR\nsubject_id\"B\n\x14ObjectTypeIdentifier\x12\x17\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x88\x01\x01\x42\x07\n\x05_nameJ\x04\x08\x01\x10\x02R\x02id\"B\n\x14PermissionIdentifier\x12\x17\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x88\x01\x01\x42\x07\n\x05_nameJ\x04\x08\x01\x10\x02R\x02id\"z\n\x16RelationTypeIdentifier\x12\x17\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x88\x01\x01\x12$\n\x0bobject_type\x18\x03 \x01(\tH\x01R\nobjectType\x88\x01\x01\x42\x07\n\x05_nameB\x0e\n\x0c_object_typeJ\x04\x08\x01\x10\x02R\x02id\"]\n\x10ObjectIdentifier\x12\x17\n\x04type\x18\x01 \x01(\tH\x00R\x04type\x88\x01\x01\x12\x15\n\x03key\x18\x03 \x01(\tH\x01R\x03key\x88\x01\x01\x42\x07\n\x05_typeB\x06\n\x04_keyJ\x04\x08\x02\x10\x03R\x02id\"\xf2\x01\n\x12RelationIdentifier\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x02 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\"=\n\x11PaginationRequest\x12\x12\n\x04size\x18\x01 \x01(\x05R\x04size\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"T\n\x12PaginationResponse\x12\x1d\n\nnext_token\x18\x01 \x01(\tR\tnextToken\x12\x1f\n\x0bresult_size\x18\x02 \x01(\x05R\nresultSize*^\n\x04\x46lag\x12\x10\n\x0c\x46LAG_UNKNOWN\x10\x00\x12\x0f\n\x0b\x46LAG_HIDDEN\x10\x01\x12\x11\n\rFLAG_READONLY\x10\x02\x12\x0f\n\x0b\x46LAG_SYSTEM\x10\x04\x12\x0f\n\x0b\x46LAG_SHADOW\x10\x08\x42\x80\x02\n\x1e\x63om.aserto.directory.common.v2B\x0b\x43ommonProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/common/v2;common\xa2\x02\x03\x41\x44\x43\xaa\x02\x1a\x41serto.Directory.Common.V2\xca\x02\x1b\x41serto\\Directory_\\Common\\V2\xe2\x02\'Aserto\\Directory_\\Common\\V2\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Common::V2b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aserto.directory.common.v2.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.aserto.directory.common.v2B\013CommonProtoP\001ZDgithub.com/aserto-dev/go-directory/aserto/directory/common/v2;common\242\002\003ADC\252\002\032Aserto.Directory.Common.V2\312\002\033Aserto\\Directory_\\Common\\V2\342\002\'Aserto\\Directory_\\Common\\V2\\GPBMetadata\352\002\035Aserto::Directory::Common::V2'
-  _FLAG._serialized_start=3122
-  _FLAG._serialized_end=3216
+  _FLAG._serialized_start=2795
+  _FLAG._serialized_end=2889
   _OBJECTTYPE._serialized_start=135
-  _OBJECTTYPE._serialized_end=545
-  _PERMISSION._serialized_start=548
-  _PERMISSION._serialized_end=828
-  _RELATIONTYPE._serialized_start=831
-  _RELATIONTYPE._serialized_end=1254
-  _OBJECT._serialized_start=1257
-  _OBJECT._serialized_end=1608
-  _RELATION._serialized_start=1611
-  _RELATION._serialized_end=1988
-  _OBJECTDEPENDENCY._serialized_start=1991
-  _OBJECTDEPENDENCY._serialized_end=2298
-  _OBJECTTYPEIDENTIFIER._serialized_start=2300
-  _OBJECTTYPEIDENTIFIER._serialized_end=2384
-  _PERMISSIONIDENTIFIER._serialized_start=2386
-  _PERMISSIONIDENTIFIER._serialized_end=2470
-  _RELATIONTYPEIDENTIFIER._serialized_start=2473
-  _RELATIONTYPEIDENTIFIER._serialized_end=2613
-  _OBJECTIDENTIFIER._serialized_start=2615
-  _OBJECTIDENTIFIER._serialized_end=2726
-  _RELATIONIDENTIFIER._serialized_start=2729
-  _RELATIONIDENTIFIER._serialized_end=2971
-  _PAGINATIONREQUEST._serialized_start=2973
-  _PAGINATIONREQUEST._serialized_end=3034
-  _PAGINATIONRESPONSE._serialized_start=3036
-  _PAGINATIONRESPONSE._serialized_end=3120
+  _OBJECTTYPE._serialized_end=498
+  _PERMISSION._serialized_start=501
+  _PERMISSION._serialized_end=734
+  _RELATIONTYPE._serialized_start=737
+  _RELATIONTYPE._serialized_end=1113
+  _OBJECT._serialized_start=1116
+  _OBJECT._serialized_end=1420
+  _RELATION._serialized_start=1423
+  _RELATION._serialized_end=1759
+  _OBJECTDEPENDENCY._serialized_start=1762
+  _OBJECTDEPENDENCY._serialized_end=2044
+  _OBJECTTYPEIDENTIFIER._serialized_start=2046
+  _OBJECTTYPEIDENTIFIER._serialized_end=2112
+  _PERMISSIONIDENTIFIER._serialized_start=2114
+  _PERMISSIONIDENTIFIER._serialized_end=2180
+  _RELATIONTYPEIDENTIFIER._serialized_start=2182
+  _RELATIONTYPEIDENTIFIER._serialized_end=2304
+  _OBJECTIDENTIFIER._serialized_start=2306
+  _OBJECTIDENTIFIER._serialized_end=2399
+  _RELATIONIDENTIFIER._serialized_start=2402
+  _RELATIONIDENTIFIER._serialized_end=2644
+  _PAGINATIONREQUEST._serialized_start=2646
+  _PAGINATIONREQUEST._serialized_end=2707
+  _PAGINATIONRESPONSE._serialized_start=2709
+  _PAGINATIONRESPONSE._serialized_end=2793
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/common/v2/common_pb2.pyi` & `aserto-directory-0.21.0/src/aserto/directory/common/v2/common_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -51,27 +51,23 @@
 """shadow object by type+key associated to parent object"""
 global___Flag = Flag
 
 @typing_extensions.final
 class ObjectType(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     IS_SUBJECT_FIELD_NUMBER: builtins.int
     ORDINAL_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     SCHEMA_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
-    DELETED_AT_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
-    id: builtins.int
-    """internal object type id"""
     name: builtins.str
     """object type name (unique, lc-string)"""
     display_name: builtins.str
     """object type display name"""
     is_subject: builtins.bool
     """object type is a subject (user|group) (default false)"""
     ordinal: builtins.int
@@ -83,101 +79,83 @@
         """object type schema definition (JSON)"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """created at timestamp (UTC)"""
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """last updated timestamp (UTC)"""
-    @property
-    def deleted_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """deleted timestamp (UTC)"""
     hash: builtins.str
     """object instance hash"""
     def __init__(
         self,
         *,
-        id: builtins.int = ...,
         name: builtins.str = ...,
         display_name: builtins.str = ...,
         is_subject: builtins.bool = ...,
         ordinal: builtins.int = ...,
         status: builtins.int = ...,
         schema: google.protobuf.struct_pb2.Struct | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        deleted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         hash: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "schema", b"schema", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "display_name", b"display_name", "hash", b"hash", "id", b"id", "is_subject", b"is_subject", "name", b"name", "ordinal", b"ordinal", "schema", b"schema", "status", b"status", "updated_at", b"updated_at"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "schema", b"schema", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "display_name", b"display_name", "hash", b"hash", "is_subject", b"is_subject", "name", b"name", "ordinal", b"ordinal", "schema", b"schema", "status", b"status", "updated_at", b"updated_at"]) -> None: ...
 
 global___ObjectType = ObjectType
 
 @typing_extensions.final
 class Permission(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
-    DELETED_AT_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
-    id: builtins.str
-    """internal permission id"""
     name: builtins.str
     """permission name (unique, cs-string)"""
     display_name: builtins.str
     """permission display name"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """created at timestamp (UTC)"""
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """last updated timestamp (UTC)"""
-    @property
-    def deleted_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """deleted timestamp (UTC)"""
     hash: builtins.str
     """object instance hash"""
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
         name: builtins.str = ...,
         display_name: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        deleted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         hash: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "display_name", b"display_name", "hash", b"hash", "id", b"id", "name", b"name", "updated_at", b"updated_at"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "display_name", b"display_name", "hash", b"hash", "name", b"name", "updated_at", b"updated_at"]) -> None: ...
 
 global___Permission = Permission
 
 @typing_extensions.final
 class RelationType(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     OBJECT_TYPE_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     ORDINAL_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     UNIONS_FIELD_NUMBER: builtins.int
     PERMISSIONS_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
-    DELETED_AT_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
-    id: builtins.int
-    """relation type id selector"""
     name: builtins.str
     """relation type name selector"""
     object_type: builtins.str
     """object type referenced by relation"""
     display_name: builtins.str
     """relation display name"""
     ordinal: builtins.int
@@ -192,55 +170,46 @@
         """permissions associated to relation type instance"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """created at timestamp (UTC)"""
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """last updated timestamp (UTC)"""
-    @property
-    def deleted_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """deleted timestamp (UTC)"""
     hash: builtins.str
     """object instance hash"""
     def __init__(
         self,
         *,
-        id: builtins.int = ...,
         name: builtins.str = ...,
         object_type: builtins.str = ...,
         display_name: builtins.str = ...,
         ordinal: builtins.int = ...,
         status: builtins.int = ...,
         unions: collections.abc.Iterable[builtins.str] | None = ...,
         permissions: collections.abc.Iterable[builtins.str] | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        deleted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         hash: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "display_name", b"display_name", "hash", b"hash", "id", b"id", "name", b"name", "object_type", b"object_type", "ordinal", b"ordinal", "permissions", b"permissions", "status", b"status", "unions", b"unions", "updated_at", b"updated_at"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "display_name", b"display_name", "hash", b"hash", "name", b"name", "object_type", b"object_type", "ordinal", b"ordinal", "permissions", b"permissions", "status", b"status", "unions", b"unions", "updated_at", b"updated_at"]) -> None: ...
 
 global___RelationType = RelationType
 
 @typing_extensions.final
 class Object(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     KEY_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
-    DELETED_AT_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
-    id: builtins.str
-    """internal object id (uuid)"""
     key: builtins.str
     """external object key (cs-string)"""
     type: builtins.str
     """object type name"""
     display_name: builtins.str
     """display name object"""
     @property
@@ -248,249 +217,205 @@
         """property bag"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """created at timestamp (UTC)"""
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """last updated timestamp (UTC)"""
-    @property
-    def deleted_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """deleted timestamp (UTC)"""
     hash: builtins.str
     """object instance hash"""
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
         key: builtins.str = ...,
         type: builtins.str = ...,
         display_name: builtins.str = ...,
         properties: google.protobuf.struct_pb2.Struct | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        deleted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         hash: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "properties", b"properties", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "display_name", b"display_name", "hash", b"hash", "id", b"id", "key", b"key", "properties", b"properties", "type", b"type", "updated_at", b"updated_at"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "properties", b"properties", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "display_name", b"display_name", "hash", b"hash", "key", b"key", "properties", b"properties", "type", b"type", "updated_at", b"updated_at"]) -> None: ...
 
 global___Object = Object
 
 @typing_extensions.final
 class Relation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBJECT_FIELD_NUMBER: builtins.int
     RELATION_FIELD_NUMBER: builtins.int
     OBJECT_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
-    DELETED_AT_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
     @property
     def subject(self) -> global___ObjectIdentifier:
         """subject identifier"""
     relation: builtins.str
-    """relation type ID"""
+    """relation type name"""
     @property
     def object(self) -> global___ObjectIdentifier:
         """object identifier"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """created at timestamp (UTC)"""
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """last updated timestamp (UTC)"""
-    @property
-    def deleted_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """deleted timestamp (UTC)"""
     hash: builtins.str
     """object instance hash"""
     def __init__(
         self,
         *,
         subject: global___ObjectIdentifier | None = ...,
         relation: builtins.str = ...,
         object: global___ObjectIdentifier | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        deleted_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         hash: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "object", b"object", "subject", b"subject", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "deleted_at", b"deleted_at", "hash", b"hash", "object", b"object", "relation", b"relation", "subject", b"subject", "updated_at", b"updated_at"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "object", b"object", "subject", b"subject", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "hash", b"hash", "object", b"object", "relation", b"relation", "subject", b"subject", "updated_at", b"updated_at"]) -> None: ...
 
 global___Relation = Relation
 
 @typing_extensions.final
 class ObjectDependency(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OBJECT_TYPE_FIELD_NUMBER: builtins.int
-    OBJECT_ID_FIELD_NUMBER: builtins.int
     OBJECT_KEY_FIELD_NUMBER: builtins.int
     RELATION_FIELD_NUMBER: builtins.int
     SUBJECT_TYPE_FIELD_NUMBER: builtins.int
-    SUBJECT_ID_FIELD_NUMBER: builtins.int
     SUBJECT_KEY_FIELD_NUMBER: builtins.int
     DEPTH_FIELD_NUMBER: builtins.int
     IS_CYCLE_FIELD_NUMBER: builtins.int
     PATH_FIELD_NUMBER: builtins.int
     object_type: builtins.str
     """object type name of source object"""
-    object_id: builtins.str
-    """object id (uuid) of source object"""
     object_key: builtins.str
     """object search key of source object"""
     relation: builtins.str
     """relation identifier"""
     subject_type: builtins.str
     """object type id of target object"""
-    subject_id: builtins.str
-    """object id (uuid) of target object"""
     subject_key: builtins.str
     """object search key of target object"""
     depth: builtins.int
     """dependency depth"""
     is_cycle: builtins.bool
     """dependency cycle"""
     @property
     def path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """dependency path"""
     def __init__(
         self,
         *,
         object_type: builtins.str = ...,
-        object_id: builtins.str = ...,
         object_key: builtins.str = ...,
         relation: builtins.str = ...,
         subject_type: builtins.str = ...,
-        subject_id: builtins.str = ...,
         subject_key: builtins.str = ...,
         depth: builtins.int = ...,
         is_cycle: builtins.bool = ...,
         path: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["depth", b"depth", "is_cycle", b"is_cycle", "object_id", b"object_id", "object_key", b"object_key", "object_type", b"object_type", "path", b"path", "relation", b"relation", "subject_id", b"subject_id", "subject_key", b"subject_key", "subject_type", b"subject_type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["depth", b"depth", "is_cycle", b"is_cycle", "object_key", b"object_key", "object_type", b"object_type", "path", b"path", "relation", b"relation", "subject_key", b"subject_key", "subject_type", b"subject_type"]) -> None: ...
 
 global___ObjectDependency = ObjectDependency
 
 @typing_extensions.final
 class ObjectTypeIdentifier(google.protobuf.message.Message):
     """ObjectType identifier"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    id: builtins.int
-    """internal object type id"""
     name: builtins.str
     """object type name (unique, lc-string)"""
     def __init__(
         self,
         *,
-        id: builtins.int | None = ...,
         name: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "id", b"id", "name", b"name"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "id", b"id", "name", b"name"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_id", b"_id"]) -> typing_extensions.Literal["id"] | None: ...
-    @typing.overload
+    def HasField(self, field_name: typing_extensions.Literal["_name", b"_name", "name", b"name"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_name", b"_name", "name", b"name"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_name", b"_name"]) -> typing_extensions.Literal["name"] | None: ...
 
 global___ObjectTypeIdentifier = ObjectTypeIdentifier
 
 @typing_extensions.final
 class PermissionIdentifier(google.protobuf.message.Message):
     """Permission identifier"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    id: builtins.str
-    """internal permission id"""
     name: builtins.str
     """permission name (unique, cs-string)"""
     def __init__(
         self,
         *,
-        id: builtins.str | None = ...,
         name: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "id", b"id", "name", b"name"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "id", b"id", "name", b"name"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_id", b"_id"]) -> typing_extensions.Literal["id"] | None: ...
-    @typing.overload
+    def HasField(self, field_name: typing_extensions.Literal["_name", b"_name", "name", b"name"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_name", b"_name", "name", b"name"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_name", b"_name"]) -> typing_extensions.Literal["name"] | None: ...
 
 global___PermissionIdentifier = PermissionIdentifier
 
 @typing_extensions.final
 class RelationTypeIdentifier(google.protobuf.message.Message):
     """RelationType identifier"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     OBJECT_TYPE_FIELD_NUMBER: builtins.int
-    id: builtins.int
-    """relation type id selector"""
     name: builtins.str
     """relation type name selector"""
     object_type: builtins.str
     """object type referenced by relation"""
     def __init__(
         self,
         *,
-        id: builtins.int | None = ...,
         name: builtins.str | None = ...,
         object_type: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "_object_type", b"_object_type", "id", b"id", "name", b"name", "object_type", b"object_type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_id", b"_id", "_name", b"_name", "_object_type", b"_object_type", "id", b"id", "name", b"name", "object_type", b"object_type"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_id", b"_id"]) -> typing_extensions.Literal["id"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_name", b"_name", "_object_type", b"_object_type", "name", b"name", "object_type", b"object_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_name", b"_name", "_object_type", b"_object_type", "name", b"name", "object_type", b"object_type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_name", b"_name"]) -> typing_extensions.Literal["name"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_object_type", b"_object_type"]) -> typing_extensions.Literal["object_type"] | None: ...
 
 global___RelationTypeIdentifier = RelationTypeIdentifier
 
 @typing_extensions.final
 class ObjectIdentifier(google.protobuf.message.Message):
     """Object identifier"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_FIELD_NUMBER: builtins.int
-    ID_FIELD_NUMBER: builtins.int
     KEY_FIELD_NUMBER: builtins.int
     type: builtins.str
     """object type"""
-    id: builtins.str
-    """internal object id (uuid)"""
     key: builtins.str
     """external object key (cs-string)"""
     def __init__(
         self,
         *,
         type: builtins.str | None = ...,
-        id: builtins.str | None = ...,
         key: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_id", b"_id", "_key", b"_key", "_type", b"_type", "id", b"id", "key", b"key", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_id", b"_id", "_key", b"_key", "_type", b"_type", "id", b"id", "key", b"key", "type", b"type"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_id", b"_id"]) -> typing_extensions.Literal["id"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_key", b"_key", "_type", b"_type", "key", b"key", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_key", b"_key", "_type", b"_type", "key", b"key", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_key", b"_key"]) -> typing_extensions.Literal["key"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_type", b"_type"]) -> typing_extensions.Literal["type"] | None: ...
 
 global___ObjectIdentifier = ObjectIdentifier
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2.py` & `aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2.pyi` & `aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py` & `aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi` & `aserto-directory-0.21.0/src/aserto/directory/exporter/v2/exporter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2.py` & `aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2.pyi` & `aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2_grpc.py` & `aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi` & `aserto-directory-0.21.0/src/aserto/directory/importer/v2/importer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/__init__.py` & `aserto-directory-0.21.0/src/aserto/directory/reader/v2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 # This file is generated by init_gen.py. Do not edit.
 
-from aserto.directory.reader.v2.reader_pb2_grpc import (
-    ReaderStub,
-    ReaderServicer,
-)
-
 from aserto.directory.reader.v2.reader_pb2 import (
     GetObjectTypeRequest,
     GetObjectTypeResponse,
     GetObjectTypesRequest,
     GetObjectTypesResponse,
     GetRelationTypeRequest,
     GetRelationTypeResponse,
@@ -33,17 +28,20 @@
     CheckRelationRequest,
     CheckRelationResponse,
     CheckResponse,
     GetGraphRequest,
     GetGraphResponse,
 )
 
+from aserto.directory.reader.v2.reader_pb2_grpc import (
+    ReaderStub,
+    ReaderServicer,
+)
+
 __all__ = [
-    "ReaderStub",
-    "ReaderServicer",
     "GetObjectTypeRequest",
     "GetObjectTypeResponse",
     "GetObjectTypesRequest",
     "GetObjectTypesResponse",
     "GetRelationTypeRequest",
     "GetRelationTypeResponse",
     "GetRelationTypesRequest",
@@ -65,8 +63,10 @@
     "CheckPermissionRequest",
     "CheckPermissionResponse",
     "CheckRelationRequest",
     "CheckRelationResponse",
     "CheckResponse",
     "GetGraphRequest",
     "GetGraphResponse",
+    "ReaderStub",
+    "ReaderServicer",
 ]
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2.py` & `aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from aserto.directory.common.v2 import common_pb2 as aserto_dot_directory_dot_common_dot_v2_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/reader/v2/reader.proto\x12\x1a\x61serto.directory.reader.v2\x1a\'aserto/directory/common/v2/common.proto\"^\n\x14GetObjectTypeRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\"W\n\x15GetObjectTypeResponse\x12>\n\x06result\x18\x01 \x01(\x0b\x32&.aserto.directory.common.v2.ObjectTypeR\x06result\"Z\n\x15GetObjectTypesRequest\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9e\x01\n\x16GetObjectTypesResponse\x12@\n\x07results\x18\x01 \x03(\x0b\x32&.aserto.directory.common.v2.ObjectTypeR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"b\n\x16GetRelationTypeRequest\x12H\n\x05param\x18\x01 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x05param\"[\n\x17GetRelationTypeResponse\x12@\n\x06result\x18\x01 \x01(\x0b\x32(.aserto.directory.common.v2.RelationTypeR\x06result\"\xa4\x01\n\x17GetRelationTypesRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\xa2\x01\n\x18GetRelationTypesResponse\x12\x42\n\x07results\x18\x01 \x03(\x0b\x32(.aserto.directory.common.v2.RelationTypeR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"V\n\x10GetObjectRequest\x12\x42\n\x05param\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x05param\"O\n\x11GetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v2.ObjectR\x06result\"Z\n\x14GetObjectManyRequest\x12\x42\n\x05param\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x05param\"U\n\x15GetObjectManyResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v2.ObjectR\x07results\"\x9e\x01\n\x11GetObjectsRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x96\x01\n\x12GetObjectsResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v2.ObjectR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"Z\n\x12GetRelationRequest\x12\x44\n\x05param\x18\x01 \x01(\x0b\x32..aserto.directory.common.v2.RelationIdentifierR\x05param\"U\n\x13GetRelationResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v2.RelationR\x07results\"\x9e\x01\n\x13GetRelationsRequest\x12\x44\n\x05param\x18\x01 \x01(\x0b\x32..aserto.directory.common.v2.RelationIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9a\x01\n\x14GetRelationsResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v2.RelationR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"^\n\x14GetPermissionRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.PermissionIdentifierR\x05param\"W\n\x15GetPermissionResponse\x12>\n\x06result\x18\x01 \x01(\x0b\x32&.aserto.directory.common.v2.PermissionR\x06result\"Z\n\x15GetPermissionsRequest\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9e\x01\n\x16GetPermissionsResponse\x12@\n\x07results\x18\x01 \x03(\x0b\x32&.aserto.directory.common.v2.PermissionR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"\x8e\x02\n\x16\x43heckPermissionRequest\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12P\n\npermission\x18\x02 \x01(\x0b\x32\x30.aserto.directory.common.v2.PermissionIdentifierR\npermission\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x14\n\x05trace\x18\x07 \x01(\x08R\x05trace\"E\n\x17\x43heckPermissionResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\x8a\x02\n\x14\x43heckRelationRequest\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x02 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x14\n\x05trace\x18\x07 \x01(\x08R\x05trace\"C\n\x15\x43heckRelationResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\";\n\rCheckResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xb5\x02\n\x0fGetGraphRequest\x12\x44\n\x06\x61nchor\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06\x61nchor\x12\x46\n\x07subject\x18\x02 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x03 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x04 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\"Z\n\x10GetGraphResponse\x12\x46\n\x07results\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v2.ObjectDependencyR\x07results2\x86\r\n\x06Reader\x12v\n\rGetObjectType\x12\x30.aserto.directory.reader.v2.GetObjectTypeRequest\x1a\x31.aserto.directory.reader.v2.GetObjectTypeResponse\"\x00\x12y\n\x0eGetObjectTypes\x12\x31.aserto.directory.reader.v2.GetObjectTypesRequest\x1a\x32.aserto.directory.reader.v2.GetObjectTypesResponse\"\x00\x12|\n\x0fGetRelationType\x12\x32.aserto.directory.reader.v2.GetRelationTypeRequest\x1a\x33.aserto.directory.reader.v2.GetRelationTypeResponse\"\x00\x12\x7f\n\x10GetRelationTypes\x12\x33.aserto.directory.reader.v2.GetRelationTypesRequest\x1a\x34.aserto.directory.reader.v2.GetRelationTypesResponse\"\x00\x12v\n\rGetPermission\x12\x30.aserto.directory.reader.v2.GetPermissionRequest\x1a\x31.aserto.directory.reader.v2.GetPermissionResponse\"\x00\x12y\n\x0eGetPermissions\x12\x31.aserto.directory.reader.v2.GetPermissionsRequest\x1a\x32.aserto.directory.reader.v2.GetPermissionsResponse\"\x00\x12j\n\tGetObject\x12,.aserto.directory.reader.v2.GetObjectRequest\x1a-.aserto.directory.reader.v2.GetObjectResponse\"\x00\x12v\n\rGetObjectMany\x12\x30.aserto.directory.reader.v2.GetObjectManyRequest\x1a\x31.aserto.directory.reader.v2.GetObjectManyResponse\"\x00\x12m\n\nGetObjects\x12-.aserto.directory.reader.v2.GetObjectsRequest\x1a..aserto.directory.reader.v2.GetObjectsResponse\"\x00\x12p\n\x0bGetRelation\x12..aserto.directory.reader.v2.GetRelationRequest\x1a/.aserto.directory.reader.v2.GetRelationResponse\"\x00\x12s\n\x0cGetRelations\x12/.aserto.directory.reader.v2.GetRelationsRequest\x1a\x30.aserto.directory.reader.v2.GetRelationsResponse\"\x00\x12|\n\x0f\x43heckPermission\x12\x32.aserto.directory.reader.v2.CheckPermissionRequest\x1a\x33.aserto.directory.reader.v2.CheckPermissionResponse\"\x00\x12v\n\rCheckRelation\x12\x30.aserto.directory.reader.v2.CheckRelationRequest\x1a\x31.aserto.directory.reader.v2.CheckRelationResponse\"\x00\x12g\n\x08GetGraph\x12+.aserto.directory.reader.v2.GetGraphRequest\x1a,.aserto.directory.reader.v2.GetGraphResponse\"\x00\x42\x80\x02\n\x1e\x63om.aserto.directory.reader.v2B\x0bReaderProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v2;reader\xa2\x02\x03\x41\x44R\xaa\x02\x1a\x41serto.Directory.Reader.V2\xca\x02\x1b\x41serto\\Directory_\\Reader\\V2\xe2\x02\'Aserto\\Directory_\\Reader\\V2\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Reader::V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'aserto/directory/reader/v2/reader.proto\x12\x1a\x61serto.directory.reader.v2\x1a\'aserto/directory/common/v2/common.proto\"^\n\x14GetObjectTypeRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\"W\n\x15GetObjectTypeResponse\x12>\n\x06result\x18\x01 \x01(\x0b\x32&.aserto.directory.common.v2.ObjectTypeR\x06result\"Z\n\x15GetObjectTypesRequest\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9e\x01\n\x16GetObjectTypesResponse\x12@\n\x07results\x18\x01 \x03(\x0b\x32&.aserto.directory.common.v2.ObjectTypeR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"b\n\x16GetRelationTypeRequest\x12H\n\x05param\x18\x01 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x05param\"[\n\x17GetRelationTypeResponse\x12@\n\x06result\x18\x01 \x01(\x0b\x32(.aserto.directory.common.v2.RelationTypeR\x06result\"\xa4\x01\n\x17GetRelationTypesRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\xa2\x01\n\x18GetRelationTypesResponse\x12\x42\n\x07results\x18\x01 \x03(\x0b\x32(.aserto.directory.common.v2.RelationTypeR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"V\n\x10GetObjectRequest\x12\x42\n\x05param\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x05param\"O\n\x11GetObjectResponse\x12:\n\x06result\x18\x01 \x01(\x0b\x32\".aserto.directory.common.v2.ObjectR\x06result\"Z\n\x14GetObjectManyRequest\x12\x42\n\x05param\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x05param\"U\n\x15GetObjectManyResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v2.ObjectR\x07results\"\x9e\x01\n\x11GetObjectsRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.ObjectTypeIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x96\x01\n\x12GetObjectsResponse\x12<\n\x07results\x18\x01 \x03(\x0b\x32\".aserto.directory.common.v2.ObjectR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"\x93\x01\n\x12GetRelationRequest\x12\x44\n\x05param\x18\x01 \x01(\x0b\x32..aserto.directory.common.v2.RelationIdentifierR\x05param\x12&\n\x0cwith_objects\x18\x02 \x01(\x08H\x00R\x0bwithObjects\x88\x01\x01\x42\x0f\n\r_with_objects\"\x8d\x02\n\x13GetRelationResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v2.RelationR\x07results\x12V\n\x07objects\x18\x02 \x03(\x0b\x32<.aserto.directory.reader.v2.GetRelationResponse.ObjectsEntryR\x07objects\x1a^\n\x0cObjectsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32\".aserto.directory.common.v2.ObjectR\x05value:\x02\x38\x01\"\x9e\x01\n\x13GetRelationsRequest\x12\x44\n\x05param\x18\x01 \x01(\x0b\x32..aserto.directory.common.v2.RelationIdentifierR\x05param\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9a\x01\n\x14GetRelationsResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.aserto.directory.common.v2.RelationR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"^\n\x14GetPermissionRequest\x12\x46\n\x05param\x18\x01 \x01(\x0b\x32\x30.aserto.directory.common.v2.PermissionIdentifierR\x05param\"W\n\x15GetPermissionResponse\x12>\n\x06result\x18\x01 \x01(\x0b\x32&.aserto.directory.common.v2.PermissionR\x06result\"Z\n\x15GetPermissionsRequest\x12\x41\n\x04page\x18\t \x01(\x0b\x32-.aserto.directory.common.v2.PaginationRequestR\x04page\"\x9e\x01\n\x16GetPermissionsResponse\x12@\n\x07results\x18\x01 \x03(\x0b\x32&.aserto.directory.common.v2.PermissionR\x07results\x12\x42\n\x04page\x18\t \x01(\x0b\x32..aserto.directory.common.v2.PaginationResponseR\x04page\"\x8e\x02\n\x16\x43heckPermissionRequest\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12P\n\npermission\x18\x02 \x01(\x0b\x32\x30.aserto.directory.common.v2.PermissionIdentifierR\npermission\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x14\n\x05trace\x18\x07 \x01(\x08R\x05trace\"E\n\x17\x43heckPermissionResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\x8a\x02\n\x14\x43heckRelationRequest\x12\x46\n\x07subject\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x02 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x03 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\x12\x14\n\x05trace\x18\x07 \x01(\x08R\x05trace\"C\n\x15\x43heckRelationResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\";\n\rCheckResponse\x12\x14\n\x05\x63heck\x18\x01 \x01(\x08R\x05\x63heck\x12\x14\n\x05trace\x18\x02 \x03(\tR\x05trace\"\xb5\x02\n\x0fGetGraphRequest\x12\x44\n\x06\x61nchor\x18\x01 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06\x61nchor\x12\x46\n\x07subject\x18\x02 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x07subject\x12N\n\x08relation\x18\x03 \x01(\x0b\x32\x32.aserto.directory.common.v2.RelationTypeIdentifierR\x08relation\x12\x44\n\x06object\x18\x04 \x01(\x0b\x32,.aserto.directory.common.v2.ObjectIdentifierR\x06object\"Z\n\x10GetGraphResponse\x12\x46\n\x07results\x18\x01 \x03(\x0b\x32,.aserto.directory.common.v2.ObjectDependencyR\x07results2\x86\r\n\x06Reader\x12v\n\rGetObjectType\x12\x30.aserto.directory.reader.v2.GetObjectTypeRequest\x1a\x31.aserto.directory.reader.v2.GetObjectTypeResponse\"\x00\x12y\n\x0eGetObjectTypes\x12\x31.aserto.directory.reader.v2.GetObjectTypesRequest\x1a\x32.aserto.directory.reader.v2.GetObjectTypesResponse\"\x00\x12|\n\x0fGetRelationType\x12\x32.aserto.directory.reader.v2.GetRelationTypeRequest\x1a\x33.aserto.directory.reader.v2.GetRelationTypeResponse\"\x00\x12\x7f\n\x10GetRelationTypes\x12\x33.aserto.directory.reader.v2.GetRelationTypesRequest\x1a\x34.aserto.directory.reader.v2.GetRelationTypesResponse\"\x00\x12v\n\rGetPermission\x12\x30.aserto.directory.reader.v2.GetPermissionRequest\x1a\x31.aserto.directory.reader.v2.GetPermissionResponse\"\x00\x12y\n\x0eGetPermissions\x12\x31.aserto.directory.reader.v2.GetPermissionsRequest\x1a\x32.aserto.directory.reader.v2.GetPermissionsResponse\"\x00\x12j\n\tGetObject\x12,.aserto.directory.reader.v2.GetObjectRequest\x1a-.aserto.directory.reader.v2.GetObjectResponse\"\x00\x12v\n\rGetObjectMany\x12\x30.aserto.directory.reader.v2.GetObjectManyRequest\x1a\x31.aserto.directory.reader.v2.GetObjectManyResponse\"\x00\x12m\n\nGetObjects\x12-.aserto.directory.reader.v2.GetObjectsRequest\x1a..aserto.directory.reader.v2.GetObjectsResponse\"\x00\x12p\n\x0bGetRelation\x12..aserto.directory.reader.v2.GetRelationRequest\x1a/.aserto.directory.reader.v2.GetRelationResponse\"\x00\x12s\n\x0cGetRelations\x12/.aserto.directory.reader.v2.GetRelationsRequest\x1a\x30.aserto.directory.reader.v2.GetRelationsResponse\"\x00\x12|\n\x0f\x43heckPermission\x12\x32.aserto.directory.reader.v2.CheckPermissionRequest\x1a\x33.aserto.directory.reader.v2.CheckPermissionResponse\"\x00\x12v\n\rCheckRelation\x12\x30.aserto.directory.reader.v2.CheckRelationRequest\x1a\x31.aserto.directory.reader.v2.CheckRelationResponse\"\x00\x12g\n\x08GetGraph\x12+.aserto.directory.reader.v2.GetGraphRequest\x1a,.aserto.directory.reader.v2.GetGraphResponse\"\x00\x42\x80\x02\n\x1e\x63om.aserto.directory.reader.v2B\x0bReaderProtoP\x01ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v2;reader\xa2\x02\x03\x41\x44R\xaa\x02\x1a\x41serto.Directory.Reader.V2\xca\x02\x1b\x41serto\\Directory_\\Reader\\V2\xe2\x02\'Aserto\\Directory_\\Reader\\V2\\GPBMetadata\xea\x02\x1d\x41serto::Directory::Reader::V2b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aserto.directory.reader.v2.reader_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.aserto.directory.reader.v2B\013ReaderProtoP\001ZDgithub.com/aserto-dev/go-directory/aserto/directory/reader/v2;reader\242\002\003ADR\252\002\032Aserto.Directory.Reader.V2\312\002\033Aserto\\Directory_\\Reader\\V2\342\002\'Aserto\\Directory_\\Reader\\V2\\GPBMetadata\352\002\035Aserto::Directory::Reader::V2'
+  _GETRELATIONRESPONSE_OBJECTSENTRY._options = None
+  _GETRELATIONRESPONSE_OBJECTSENTRY._serialized_options = b'8\001'
   _GETOBJECTTYPEREQUEST._serialized_start=112
   _GETOBJECTTYPEREQUEST._serialized_end=206
   _GETOBJECTTYPERESPONSE._serialized_start=208
   _GETOBJECTTYPERESPONSE._serialized_end=295
   _GETOBJECTTYPESREQUEST._serialized_start=297
   _GETOBJECTTYPESREQUEST._serialized_end=387
   _GETOBJECTTYPESRESPONSE._serialized_start=390
@@ -46,40 +48,42 @@
   _GETOBJECTMANYREQUEST._serialized_end=1334
   _GETOBJECTMANYRESPONSE._serialized_start=1336
   _GETOBJECTMANYRESPONSE._serialized_end=1421
   _GETOBJECTSREQUEST._serialized_start=1424
   _GETOBJECTSREQUEST._serialized_end=1582
   _GETOBJECTSRESPONSE._serialized_start=1585
   _GETOBJECTSRESPONSE._serialized_end=1735
-  _GETRELATIONREQUEST._serialized_start=1737
-  _GETRELATIONREQUEST._serialized_end=1827
-  _GETRELATIONRESPONSE._serialized_start=1829
-  _GETRELATIONRESPONSE._serialized_end=1914
-  _GETRELATIONSREQUEST._serialized_start=1917
-  _GETRELATIONSREQUEST._serialized_end=2075
-  _GETRELATIONSRESPONSE._serialized_start=2078
-  _GETRELATIONSRESPONSE._serialized_end=2232
-  _GETPERMISSIONREQUEST._serialized_start=2234
-  _GETPERMISSIONREQUEST._serialized_end=2328
-  _GETPERMISSIONRESPONSE._serialized_start=2330
-  _GETPERMISSIONRESPONSE._serialized_end=2417
-  _GETPERMISSIONSREQUEST._serialized_start=2419
-  _GETPERMISSIONSREQUEST._serialized_end=2509
-  _GETPERMISSIONSRESPONSE._serialized_start=2512
-  _GETPERMISSIONSRESPONSE._serialized_end=2670
-  _CHECKPERMISSIONREQUEST._serialized_start=2673
-  _CHECKPERMISSIONREQUEST._serialized_end=2943
-  _CHECKPERMISSIONRESPONSE._serialized_start=2945
-  _CHECKPERMISSIONRESPONSE._serialized_end=3014
-  _CHECKRELATIONREQUEST._serialized_start=3017
-  _CHECKRELATIONREQUEST._serialized_end=3283
-  _CHECKRELATIONRESPONSE._serialized_start=3285
-  _CHECKRELATIONRESPONSE._serialized_end=3352
-  _CHECKRESPONSE._serialized_start=3354
-  _CHECKRESPONSE._serialized_end=3413
-  _GETGRAPHREQUEST._serialized_start=3416
-  _GETGRAPHREQUEST._serialized_end=3725
-  _GETGRAPHRESPONSE._serialized_start=3727
-  _GETGRAPHRESPONSE._serialized_end=3817
-  _READER._serialized_start=3820
-  _READER._serialized_end=5490
+  _GETRELATIONREQUEST._serialized_start=1738
+  _GETRELATIONREQUEST._serialized_end=1885
+  _GETRELATIONRESPONSE._serialized_start=1888
+  _GETRELATIONRESPONSE._serialized_end=2157
+  _GETRELATIONRESPONSE_OBJECTSENTRY._serialized_start=2063
+  _GETRELATIONRESPONSE_OBJECTSENTRY._serialized_end=2157
+  _GETRELATIONSREQUEST._serialized_start=2160
+  _GETRELATIONSREQUEST._serialized_end=2318
+  _GETRELATIONSRESPONSE._serialized_start=2321
+  _GETRELATIONSRESPONSE._serialized_end=2475
+  _GETPERMISSIONREQUEST._serialized_start=2477
+  _GETPERMISSIONREQUEST._serialized_end=2571
+  _GETPERMISSIONRESPONSE._serialized_start=2573
+  _GETPERMISSIONRESPONSE._serialized_end=2660
+  _GETPERMISSIONSREQUEST._serialized_start=2662
+  _GETPERMISSIONSREQUEST._serialized_end=2752
+  _GETPERMISSIONSRESPONSE._serialized_start=2755
+  _GETPERMISSIONSRESPONSE._serialized_end=2913
+  _CHECKPERMISSIONREQUEST._serialized_start=2916
+  _CHECKPERMISSIONREQUEST._serialized_end=3186
+  _CHECKPERMISSIONRESPONSE._serialized_start=3188
+  _CHECKPERMISSIONRESPONSE._serialized_end=3257
+  _CHECKRELATIONREQUEST._serialized_start=3260
+  _CHECKRELATIONREQUEST._serialized_end=3526
+  _CHECKRELATIONRESPONSE._serialized_start=3528
+  _CHECKRELATIONRESPONSE._serialized_end=3595
+  _CHECKRESPONSE._serialized_start=3597
+  _CHECKRESPONSE._serialized_end=3656
+  _GETGRAPHREQUEST._serialized_start=3659
+  _GETGRAPHREQUEST._serialized_end=3968
+  _GETGRAPHRESPONSE._serialized_start=3970
+  _GETGRAPHRESPONSE._serialized_end=4060
+  _READER._serialized_start=4063
+  _READER._serialized_end=5733
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2.pyi` & `aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -293,41 +293,69 @@
 global___GetObjectsResponse = GetObjectsResponse
 
 @typing_extensions.final
 class GetRelationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAM_FIELD_NUMBER: builtins.int
+    WITH_OBJECTS_FIELD_NUMBER: builtins.int
     @property
     def param(self) -> aserto.directory.common.v2.common_pb2.RelationIdentifier:
         """relation selector"""
+    with_objects: builtins.bool
+    """materialize relation objects"""
     def __init__(
         self,
         *,
         param: aserto.directory.common.v2.common_pb2.RelationIdentifier | None = ...,
+        with_objects: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["param", b"param"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["param", b"param"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_with_objects", b"_with_objects", "param", b"param", "with_objects", b"with_objects"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_with_objects", b"_with_objects", "param", b"param", "with_objects", b"with_objects"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_with_objects", b"_with_objects"]) -> typing_extensions.Literal["with_objects"] | None: ...
 
 global___GetRelationRequest = GetRelationRequest
 
 @typing_extensions.final
 class GetRelationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
+    class ObjectsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> aserto.directory.common.v2.common_pb2.Object: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: aserto.directory.common.v2.common_pb2.Object | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     RESULTS_FIELD_NUMBER: builtins.int
+    OBJECTS_FIELD_NUMBER: builtins.int
     @property
     def results(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[aserto.directory.common.v2.common_pb2.Relation]:
         """array of relation instances"""
+    @property
+    def objects(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, aserto.directory.common.v2.common_pb2.Object]:
+        """map of materialized relation objects"""
     def __init__(
         self,
         *,
         results: collections.abc.Iterable[aserto.directory.common.v2.common_pb2.Relation] | None = ...,
+        objects: collections.abc.Mapping[builtins.str, aserto.directory.common.v2.common_pb2.Object] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["results", b"results"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["objects", b"objects", "results", b"results"]) -> None: ...
 
 global___GetRelationResponse = GetRelationResponse
 
 @typing_extensions.final
 class GetRelationsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2_grpc.py` & `aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi` & `aserto-directory-0.21.0/src/aserto/directory/reader/v2/reader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/__init__.py` & `aserto-directory-0.21.0/src/aserto/directory/writer/v2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 # This file is generated by init_gen.py. Do not edit.
 
-from aserto.directory.writer.v2.writer_pb2_grpc import (
-    WriterStub,
-    WriterServicer,
-)
-
 from aserto.directory.writer.v2.writer_pb2 import (
     SetObjectTypeRequest,
     SetObjectTypeResponse,
     DeleteObjectTypeRequest,
     DeleteObjectTypeResponse,
     SetRelationTypeRequest,
     SetRelationTypeResponse,
@@ -24,17 +19,20 @@
     DeleteObjectResponse,
     SetRelationRequest,
     SetRelationResponse,
     DeleteRelationRequest,
     DeleteRelationResponse,
 )
 
+from aserto.directory.writer.v2.writer_pb2_grpc import (
+    WriterStub,
+    WriterServicer,
+)
+
 __all__ = [
-    "WriterStub",
-    "WriterServicer",
     "SetObjectTypeRequest",
     "SetObjectTypeResponse",
     "DeleteObjectTypeRequest",
     "DeleteObjectTypeResponse",
     "SetRelationTypeRequest",
     "SetRelationTypeResponse",
     "DeleteRelationTypeRequest",
@@ -47,8 +45,10 @@
     "SetObjectResponse",
     "DeleteObjectRequest",
     "DeleteObjectResponse",
     "SetRelationRequest",
     "SetRelationResponse",
     "DeleteRelationRequest",
     "DeleteRelationResponse",
+    "WriterStub",
+    "WriterServicer",
 ]
```

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2.py` & `aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2.pyi` & `aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2_grpc.py` & `aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi` & `aserto-directory-0.21.0/src/aserto/directory/writer/v2/writer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aserto-directory-0.0.1rc1/setup.py` & `aserto-directory-0.21.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 packages = \
 ['aserto',
  'aserto.directory.common.v2',
  'aserto.directory.exporter.v2',
  'aserto.directory.importer.v2',
  'aserto.directory.reader.v2',
+ 'aserto.directory.schema.v2',
  'aserto.directory.writer.v2']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'aserto-directory',
-    'version': '0.0.1rc1',
+    'version': '0.21.0',
     'description': 'gRPC client for Aserto Directory service instances',
-    'long_description': '# Aserto Directory gRPC client\nThis is an automatically generated client for interacting with Aserto\'s\n[Directory service](https://docs.aserto.com/docs/overview/directory) using the gRPC protocol.\n\n## Installation\n### Using Pip\n```sh\npip install aserto-directory\n```\n### Using Poetry\n```sh\npoetry add aserto-directory\n```\n## Usage\n```py\nimport grpc\nfrom aserto.directory.common.v2 import ObjectTypeRequest\nfrom aserto.directory.reader.v2 import ReaderStub\n\nwith grpc.secure_channel(target=f"directory.prod.aserto.com:8443") as channel:\n    reader = ReaderStub(channel)\n\n    # List all object types in the directory\n    response = client.GetObjectTypes(\n        GetObjectTypesRequest(),\n        metadata=(\n            ("authorization", f"basic {ASERTO_DIRECTORY_API_KEY}"),\n            ("aserto-tenant-id", ASERTO_TENANT_ID),\n        ),\n    )\n\n    for object_type in response.results:\n        print("Object Type:", object_type.name)\n```\n',
+    'long_description': '# Aserto Directory gRPC client\nThis is an automatically generated client for interacting with Aserto\'s\n[Directory service](https://docs.aserto.com/docs/overview/directory) using the gRPC protocol.\n\n## Installation\n### Using Pip\n```sh\npip install aserto-directory\n```\n### Using Poetry\n```sh\npoetry add aserto-directory\n```\n## Usage\n```py\nimport grpc\nfrom aserto.directory.reader.v2 import ReaderStub, GetObjectTypesRequest\n\nwith grpc.secure_channel(\n    target="directory.prod.aserto.com:8443",\n    credentials=grpc.ssl_channel_credentials(),\n) as channel:\n    reader = ReaderStub(channel)\n\n    # List all object types in the directory\n    response = reader.GetObjectTypes(\n        GetObjectTypesRequest(),\n        metadata=(\n            ("authorization", f"basic {ASERTO_DIRECTORY_API_KEY}"),\n            ("aserto-tenant-id", ASERTO_TENANT_ID),\n        ),\n    )\n\n    for object_type in response.results:\n        print("Object Type:", object_type.name)\n',
     'author': 'Aserto, Inc.',
     'author_email': 'pypi@aserto.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/aserto-dev/python-directory',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `aserto-directory-0.0.1rc1/PKG-INFO` & `aserto-directory-0.21.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aserto-directory
-Version: 0.0.1rc1
+Version: 0.21.0
 Summary: gRPC client for Aserto Directory service instances
 Home-page: https://github.com/aserto-dev/python-directory
 License: Apache-2.0
 Author: Aserto, Inc.
 Author-email: pypi@aserto.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -36,26 +36,27 @@
 ### Using Poetry
 ```sh
 poetry add aserto-directory
 ```
 ## Usage
 ```py
 import grpc
-from aserto.directory.common.v2 import ObjectTypeRequest
-from aserto.directory.reader.v2 import ReaderStub
+from aserto.directory.reader.v2 import ReaderStub, GetObjectTypesRequest
 
-with grpc.secure_channel(target=f"directory.prod.aserto.com:8443") as channel:
+with grpc.secure_channel(
+    target="directory.prod.aserto.com:8443",
+    credentials=grpc.ssl_channel_credentials(),
+) as channel:
     reader = ReaderStub(channel)
 
     # List all object types in the directory
-    response = client.GetObjectTypes(
+    response = reader.GetObjectTypes(
         GetObjectTypesRequest(),
         metadata=(
             ("authorization", f"basic {ASERTO_DIRECTORY_API_KEY}"),
             ("aserto-tenant-id", ASERTO_TENANT_ID),
         ),
     )
 
     for object_type in response.results:
         print("Object Type:", object_type.name)
-```
```

