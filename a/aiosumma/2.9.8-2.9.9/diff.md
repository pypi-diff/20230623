# Comparing `tmp/aiosumma-2.9.8-py3-none-any.whl.zip` & `tmp/aiosumma-2.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 155738 bytes, number of entries: 46
+Zip file size: 155786 bytes, number of entries: 46
 -rw-r--r--  2.0 unx      187 b- defN 22-Jun-30 17:44 aiosumma/__init__.py
 -rw-r--r--  2.0 unx      537 b- defN 22-Sep-12 00:31 aiosumma/cli.py
--rw-r--r--  2.0 unx    20643 b- defN 22-Sep-12 15:43 aiosumma/client.py
+-rw-r--r--  2.0 unx    21221 b- defN 22-Sep-12 16:33 aiosumma/client.py
 -rw-r--r--  2.0 unx      741 b- defN 22-Aug-23 18:23 aiosumma/context.py
 -rw-r--r--  2.0 unx   370551 b- defN 22-Jun-30 17:44 aiosumma/data/synsets/drugs.csv
 -rw-r--r--  2.0 unx      126 b- defN 22-Jun-30 17:44 aiosumma/errors.py
 -rw-r--r--  2.0 unx     1322 b- defN 22-Aug-23 17:05 aiosumma/eval_scorer_builder.py
 -rw-r--r--  2.0 unx       65 b- defN 22-Jun-30 17:44 aiosumma/parser/__init__.py
 -rw-r--r--  2.0 unx    10769 b- defN 22-Aug-30 16:49 aiosumma/parser/elements.py
 -rw-r--r--  2.0 unx      147 b- defN 22-Jun-30 17:44 aiosumma/parser/errors.py
@@ -29,20 +29,20 @@
 -rw-r--r--  2.0 unx     2110 b- defN 22-Jun-30 17:44 aiosumma/tree_transformers/synonym.py
 -rw-r--r--  2.0 unx     1944 b- defN 22-Aug-30 20:29 aiosumma/tree_transformers/tantivy.py
 -rw-r--r--  2.0 unx     1609 b- defN 22-Jun-30 17:44 aiosumma/tree_transformers/values.py
 -r-xr-xr-x  2.0 unx     1641 b- defN 22-Sep-11 23:10 summa/proto/beacon_service_pb2.py
 -r-xr-xr-x  2.0 unx     2697 b- defN 22-Sep-09 15:10 summa/proto/beacon_service_pb2_grpc.py
 -r-xr-xr-x  2.0 unx     3431 b- defN 22-Aug-22 12:16 summa/proto/consumer_service_pb2.py
 -r-xr-xr-x  2.0 unx     7986 b- defN 22-Aug-22 12:16 summa/proto/consumer_service_pb2_grpc.py
--r-xr-xr-x  2.0 unx    11339 b- defN 22-Sep-12 15:54 summa/proto/index_service_pb2.py
--r-xr-xr-x  2.0 unx    23390 b- defN 22-Sep-12 15:54 summa/proto/index_service_pb2_grpc.py
+-r-xr-xr-x  2.0 unx    11331 b- defN 22-Sep-12 16:49 summa/proto/index_service_pb2.py
+-r-xr-xr-x  2.0 unx    25093 b- defN 22-Sep-12 16:49 summa/proto/index_service_pb2_grpc.py
 -r-xr-xr-x  2.0 unx     2351 b- defN 22-Aug-22 12:16 summa/proto/reflection_service_pb2.py
 -r-xr-xr-x  2.0 unx     2751 b- defN 22-Aug-22 12:16 summa/proto/reflection_service_pb2_grpc.py
 -r-xr-xr-x  2.0 unx    23421 b- defN 22-Sep-08 00:09 summa/proto/search_service_pb2.py
 -r-xr-xr-x  2.0 unx     2612 b- defN 22-Aug-22 12:16 summa/proto/search_service_pb2_grpc.py
 -r-xr-xr-x  2.0 unx      998 b- defN 22-Aug-22 12:16 summa/proto/utils_pb2.py
 -r-xr-xr-x  2.0 unx      159 b- defN 22-Aug-22 12:16 summa/proto/utils_pb2_grpc.py
-?rw-------  2.0 unx       91 b- defN 22-Sep-12 15:54 aiosumma-2.9.8.dist-info/WHEEL
-?rw-------  2.0 unx      557 b- defN 22-Sep-12 15:54 aiosumma-2.9.8.dist-info/METADATA
--r-xr-xr-x  2.0 unx       47 b- defN 22-Aug-22 12:11 aiosumma-2.9.8.dist-info/entry_points.txt
-?rw-------  2.0 unx     4056 b- defN 22-Sep-12 15:54 aiosumma-2.9.8.dist-info/RECORD
-46 files, 523912 bytes uncompressed, 149210 bytes compressed:  71.5%
+?rw-------  2.0 unx       91 b- defN 22-Sep-12 16:49 aiosumma-2.9.9.dist-info/WHEEL
+?rw-------  2.0 unx      557 b- defN 22-Sep-12 16:49 aiosumma-2.9.9.dist-info/METADATA
+-r-xr-xr-x  2.0 unx       47 b- defN 22-Aug-22 12:11 aiosumma-2.9.9.dist-info/entry_points.txt
+?rw-------  2.0 unx     4056 b- defN 22-Sep-12 16:49 aiosumma-2.9.9.dist-info/RECORD
+46 files, 526185 bytes uncompressed, 149258 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -120,20 +120,20 @@
 
 Filename: summa/proto/utils_pb2.py
 Comment: 
 
 Filename: summa/proto/utils_pb2_grpc.py
 Comment: 
 
-Filename: aiosumma-2.9.8.dist-info/WHEEL
+Filename: aiosumma-2.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: aiosumma-2.9.8.dist-info/METADATA
+Filename: aiosumma-2.9.9.dist-info/METADATA
 Comment: 
 
-Filename: aiosumma-2.9.8.dist-info/entry_points.txt
+Filename: aiosumma-2.9.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: aiosumma-2.9.8.dist-info/RECORD
+Filename: aiosumma-2.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiosumma/client.py

```diff
@@ -135,28 +135,52 @@
                     field=sort_by_field[0],
                     order=sort_by_field[1],
                 ) if sort_by_field else None
             ),
             metadata=(('request-id', request_id), ('session-id', session_id)),
         )
 
+    @expose
+    async def attach_index(
+        self,
+        index_name: str,
+        index_path: str,
+        request_id: Optional[str] = None,
+        session_id: Optional[str] = None,
+    ) -> index_service_pb.AttachIndexResponse:
+        """
+        Alter index options like compression and ordering
+
+        Args:
+            index_name: index name
+            index_path: index path
+            request_id: request id
+            session_id: session id
+        """
+        return await self.stubs['index_api'].attach_index(
+            index_service_pb.AttachIndexRequest(
+                index_name=index_name,
+                index_path=index_path,
+            ),
+            metadata=(('request-id', request_id), ('session-id', session_id)),
+        )
+
     @expose(with_from_file=True)
     async def create_index(
         self,
         index_name: str,
         schema: str,
         primary_key: Optional[str] = None,
         default_fields: Optional[List[str]] = None,
         multi_fields: Optional[List[str]] = None,
         compression: Optional[Union[str, int]] = None,
         writer_heap_size_bytes: Optional[int] = None,
         writer_threads: Optional[int] = None,
         autocommit_interval_ms: Optional[int] = None,
         sort_by_field: Optional[Tuple] = None,
-        is_index_existing: bool = False,
         request_id: Optional[str] = None,
         session_id: Optional[str] = None,
     ) -> index_service_pb.CreateIndexResponse:
         """
         Create index
 
         Args:
@@ -169,15 +193,14 @@
             writer_heap_size_bytes: Tantivy writer heap size in bytes, shared between all threads
             writer_threads: Tantivy writer threads
             autocommit_interval_ms: if true then there will be a separate thread committing index every nth milliseconds
                 set by this parameter
             request_id: request id
             session_id: session id
             sort_by_field: (field_name, order)
-            is_index_existing: if true then try to open and import existing Tantivy files
         """
         if isinstance(compression, str):
             compression = index_service_pb.Compression.Value(compression)
         elif isinstance(compression, int):
             compression = index_service_pb.Compression.Name(compression)
         return await self.stubs['index_api'].create_index(
             index_service_pb.CreateIndexRequest(
@@ -189,16 +212,15 @@
                 compression=compression,
                 writer_heap_size_bytes=writer_heap_size_bytes,
                 writer_threads=writer_threads,
                 autocommit_interval_ms=autocommit_interval_ms,
                 sort_by_field=index_service_pb.SortByField(
                     field=sort_by_field[0],
                     order=sort_by_field[1],
-                ) if sort_by_field else None,
-                is_index_existing=is_index_existing,
+                ) if sort_by_field else None
             ),
             metadata=(('request-id', request_id), ('session-id', session_id)),
         )
 
     @expose
     async def delete_consumer(
         self,
```

## summa/proto/index_service_pb2.py

```diff
@@ -10,91 +10,91 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from summa.proto import utils_pb2 as summa_dot_proto_dot_utils__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fsumma/proto/index_service.proto\x12\x0bsumma.proto\x1a\x17summa/proto/utils.proto\"\xd8\x01\n\x11\x41lterIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12?\n\x0b\x63ompression\x18\x02 \x01(\x0e\x32\x18.summa.proto.CompressionH\x00R\x0b\x63ompression\x88\x01\x01\x12\x41\n\rsort_by_field\x18\x03 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x01R\x0bsortByField\x88\x01\x01\x42\x0e\n\x0c_compressionB\x10\n\x0e_sort_by_field\">\n\x12\x41lterIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"R\n\x12\x41ttachIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12\x1d\n\nindex_path\x18\x02 \x01(\tR\tindexPath\"?\n\x13\x41ttachIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"o\n\x12\x43ommitIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x38\n\x0b\x63ommit_mode\x18\x02 \x01(\x0e\x32\x17.summa.proto.CommitModeR\ncommitMode\"y\n\x13\x43ommitIndexResponse\x12\x1d\n\x07opstamp\x18\x01 \x01(\x04H\x00R\x07opstamp\x88\x01\x01\x12&\n\x0c\x65lapsed_secs\x18\x02 \x01(\x01H\x01R\x0b\x65lapsedSecs\x88\x01\x01\x42\n\n\x08_opstampB\x0f\n\r_elapsed_secs\"M\n\x0bSortByField\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12(\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.OrderR\x05order\"\xaf\x05\n\x12\x43reateIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12\x16\n\x06schema\x18\x02 \x01(\tR\x06schema\x12;\n\x0cindex_engine\x18\n \x01(\x0e\x32\x18.summa.proto.IndexEngineR\x0bindexEngine\x12$\n\x0bprimary_key\x18\x03 \x01(\tH\x00R\nprimaryKey\x88\x01\x01\x12%\n\x0e\x64\x65\x66\x61ult_fields\x18\x04 \x03(\tR\rdefaultFields\x12:\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.CompressionR\x0b\x63ompression\x12\x38\n\x16writer_heap_size_bytes\x18\x06 \x01(\x04H\x01R\x13writerHeapSizeBytes\x88\x01\x01\x12*\n\x0ewriter_threads\x18\x07 \x01(\x04H\x02R\rwriterThreads\x88\x01\x01\x12\x39\n\x16\x61utocommit_interval_ms\x18\x08 \x01(\x04H\x03R\x14\x61utocommitIntervalMs\x88\x01\x01\x12\x41\n\rsort_by_field\x18\t \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x04R\x0bsortByField\x88\x01\x01\x12!\n\x0cmulti_fields\x18\x0b \x03(\tR\x0bmultiFields\x12*\n\x11is_index_existing\x18\x0c \x01(\x08R\x0fisIndexExistingB\x0e\n\x0c_primary_keyB\x19\n\x17_writer_heap_size_bytesB\x11\n\x0f_writer_threadsB\x19\n\x17_autocommit_interval_msB\x10\n\x0e_sort_by_field\"?\n\x13\x43reateIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"Y\n\x15\x44\x65leteDocumentRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1f\n\x0bprimary_key\x18\x02 \x01(\x03R\nprimaryKey\"C\n\x16\x44\x65leteDocumentResponse\x12\x1d\n\x07opstamp\x18\x01 \x01(\x04H\x00R\x07opstamp\x88\x01\x01\x42\n\n\x08_opstamp\"3\n\x12\x44\x65leteIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\"\x15\n\x13\x44\x65leteIndexResponse\"\x1a\n\x18GetIndicesAliasesRequest\"\xc3\x01\n\x19GetIndicesAliasesResponse\x12\x63\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntryR\x0eindicesAliases\x1a\x41\n\x13IndicesAliasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"2\n\x0fGetIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\"<\n\x10GetIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"\x13\n\x11GetIndicesRequest\"B\n\x12GetIndicesResponse\x12,\n\x07indices\x18\x01 \x03(\x0b\x32\x12.summa.proto.IndexR\x07indices\"[\n\x1aIndexDocumentStreamRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1c\n\tdocuments\x18\x02 \x03(\x0cR\tdocuments\"\x84\x01\n\x1bIndexDocumentStreamResponse\x12!\n\x0csuccess_docs\x18\x01 \x01(\x04R\x0bsuccessDocs\x12\x1f\n\x0b\x66\x61iled_docs\x18\x02 \x01(\x04R\nfailedDocs\x12!\n\x0c\x65lapsed_secs\x18\x03 \x01(\x01R\x0b\x65lapsedSecs\"S\n\x14IndexDocumentRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1a\n\x08\x64ocument\x18\x02 \x01(\x0cR\x08\x64ocument\"1\n\x15IndexDocumentResponse\x12\x18\n\x07opstamp\x18\x01 \x01(\x04R\x07opstamp\"X\n\x14MergeSegmentsRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1f\n\x0bsegment_ids\x18\x02 \x03(\tR\nsegmentIds\"\x17\n\x15MergeSegmentsResponse\"V\n\x14SetIndexAliasRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1d\n\nindex_name\x18\x02 \x01(\tR\tindexName\"U\n\x15SetIndexAliasResponse\x12)\n\x0eold_index_name\x18\x01 \x01(\tH\x00R\x0coldIndexName\x88\x01\x01\x42\x11\n\x0f_old_index_name\"5\n\x12VacuumIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\"\x15\n\x13VacuumIndexResponse\"\xc5\x01\n\x05Index\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12#\n\rindex_aliases\x18\x02 \x03(\tR\x0cindexAliases\x12!\n\x0cindex_engine\x18\x03 \x01(\tR\x0bindexEngine\x12\x19\n\x08num_docs\x18\x04 \x01(\x04R\x07numDocs\x12:\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.CompressionR\x0b\x63ompression\"4\n\x16IndexDocumentOperation\x12\x1a\n\x08\x64ocument\x18\x01 \x01(\x0cR\x08\x64ocument\"k\n\x0eIndexOperation\x12L\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00R\rindexDocumentB\x0b\n\toperation*B\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04*#\n\x0bIndexEngine\x12\x08\n\x04\x46ile\x10\x00\x12\n\n\x06Memory\x10\x01*!\n\nCommitMode\x12\t\n\x05\x41sync\x10\x00\x12\x08\n\x04Sync\x10\x01\x32\x96\t\n\x08IndexApi\x12P\n\x0b\x61lter_index\x12\x1e.summa.proto.AlterIndexRequest\x1a\x1f.summa.proto.AlterIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12\\\n\x0f\x64\x65lete_document\x12\".summa.proto.DeleteDocumentRequest\x1a#.summa.proto.DeleteDocumentResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fsumma/proto/index_service.proto\x12\x0bsumma.proto\x1a\x17summa/proto/utils.proto\"\xd8\x01\n\x11\x41lterIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12?\n\x0b\x63ompression\x18\x02 \x01(\x0e\x32\x18.summa.proto.CompressionH\x00R\x0b\x63ompression\x88\x01\x01\x12\x41\n\rsort_by_field\x18\x03 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x01R\x0bsortByField\x88\x01\x01\x42\x0e\n\x0c_compressionB\x10\n\x0e_sort_by_field\">\n\x12\x41lterIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"3\n\x12\x41ttachIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\"?\n\x13\x41ttachIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"o\n\x12\x43ommitIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x38\n\x0b\x63ommit_mode\x18\x02 \x01(\x0e\x32\x17.summa.proto.CommitModeR\ncommitMode\"y\n\x13\x43ommitIndexResponse\x12\x1d\n\x07opstamp\x18\x01 \x01(\x04H\x00R\x07opstamp\x88\x01\x01\x12&\n\x0c\x65lapsed_secs\x18\x02 \x01(\x01H\x01R\x0b\x65lapsedSecs\x88\x01\x01\x42\n\n\x08_opstampB\x0f\n\r_elapsed_secs\"M\n\x0bSortByField\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12(\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.OrderR\x05order\"\x83\x05\n\x12\x43reateIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12\x16\n\x06schema\x18\x02 \x01(\tR\x06schema\x12;\n\x0cindex_engine\x18\n \x01(\x0e\x32\x18.summa.proto.IndexEngineR\x0bindexEngine\x12$\n\x0bprimary_key\x18\x03 \x01(\tH\x00R\nprimaryKey\x88\x01\x01\x12%\n\x0e\x64\x65\x66\x61ult_fields\x18\x04 \x03(\tR\rdefaultFields\x12:\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.CompressionR\x0b\x63ompression\x12\x38\n\x16writer_heap_size_bytes\x18\x06 \x01(\x04H\x01R\x13writerHeapSizeBytes\x88\x01\x01\x12*\n\x0ewriter_threads\x18\x07 \x01(\x04H\x02R\rwriterThreads\x88\x01\x01\x12\x39\n\x16\x61utocommit_interval_ms\x18\x08 \x01(\x04H\x03R\x14\x61utocommitIntervalMs\x88\x01\x01\x12\x41\n\rsort_by_field\x18\t \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x04R\x0bsortByField\x88\x01\x01\x12!\n\x0cmulti_fields\x18\x0b \x03(\tR\x0bmultiFieldsB\x0e\n\x0c_primary_keyB\x19\n\x17_writer_heap_size_bytesB\x11\n\x0f_writer_threadsB\x19\n\x17_autocommit_interval_msB\x10\n\x0e_sort_by_field\"?\n\x13\x43reateIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"Y\n\x15\x44\x65leteDocumentRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1f\n\x0bprimary_key\x18\x02 \x01(\x03R\nprimaryKey\"C\n\x16\x44\x65leteDocumentResponse\x12\x1d\n\x07opstamp\x18\x01 \x01(\x04H\x00R\x07opstamp\x88\x01\x01\x42\n\n\x08_opstamp\"3\n\x12\x44\x65leteIndexRequest\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\"\x15\n\x13\x44\x65leteIndexResponse\"\x1a\n\x18GetIndicesAliasesRequest\"\xc3\x01\n\x19GetIndicesAliasesResponse\x12\x63\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntryR\x0eindicesAliases\x1a\x41\n\x13IndicesAliasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"2\n\x0fGetIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\"<\n\x10GetIndexResponse\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x12.summa.proto.IndexR\x05index\"\x13\n\x11GetIndicesRequest\"B\n\x12GetIndicesResponse\x12,\n\x07indices\x18\x01 \x03(\x0b\x32\x12.summa.proto.IndexR\x07indices\"[\n\x1aIndexDocumentStreamRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1c\n\tdocuments\x18\x02 \x03(\x0cR\tdocuments\"\x84\x01\n\x1bIndexDocumentStreamResponse\x12!\n\x0csuccess_docs\x18\x01 \x01(\x04R\x0bsuccessDocs\x12\x1f\n\x0b\x66\x61iled_docs\x18\x02 \x01(\x04R\nfailedDocs\x12!\n\x0c\x65lapsed_secs\x18\x03 \x01(\x01R\x0b\x65lapsedSecs\"S\n\x14IndexDocumentRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1a\n\x08\x64ocument\x18\x02 \x01(\x0cR\x08\x64ocument\"1\n\x15IndexDocumentResponse\x12\x18\n\x07opstamp\x18\x01 \x01(\x04R\x07opstamp\"X\n\x14MergeSegmentsRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1f\n\x0bsegment_ids\x18\x02 \x03(\tR\nsegmentIds\"\x17\n\x15MergeSegmentsResponse\"V\n\x14SetIndexAliasRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\x12\x1d\n\nindex_name\x18\x02 \x01(\tR\tindexName\"U\n\x15SetIndexAliasResponse\x12)\n\x0eold_index_name\x18\x01 \x01(\tH\x00R\x0coldIndexName\x88\x01\x01\x42\x11\n\x0f_old_index_name\"5\n\x12VacuumIndexRequest\x12\x1f\n\x0bindex_alias\x18\x01 \x01(\tR\nindexAlias\"\x15\n\x13VacuumIndexResponse\"\xc5\x01\n\x05Index\x12\x1d\n\nindex_name\x18\x01 \x01(\tR\tindexName\x12#\n\rindex_aliases\x18\x02 \x03(\tR\x0cindexAliases\x12!\n\x0cindex_engine\x18\x03 \x01(\tR\x0bindexEngine\x12\x19\n\x08num_docs\x18\x04 \x01(\x04R\x07numDocs\x12:\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.CompressionR\x0b\x63ompression\"4\n\x16IndexDocumentOperation\x12\x1a\n\x08\x64ocument\x18\x01 \x01(\x0cR\x08\x64ocument\"k\n\x0eIndexOperation\x12L\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00R\rindexDocumentB\x0b\n\toperation*B\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04*#\n\x0bIndexEngine\x12\x08\n\x04\x46ile\x10\x00\x12\n\n\x06Memory\x10\x01*!\n\nCommitMode\x12\t\n\x05\x41sync\x10\x00\x12\x08\n\x04Sync\x10\x01\x32\xeb\t\n\x08IndexApi\x12P\n\x0b\x61lter_index\x12\x1e.summa.proto.AlterIndexRequest\x1a\x1f.summa.proto.AlterIndexResponse\"\x00\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12\\\n\x0f\x64\x65lete_document\x12\".summa.proto.DeleteDocumentRequest\x1a#.summa.proto.DeleteDocumentResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'summa.proto.index_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_options = b'8\001'
-  _COMPRESSION._serialized_start=3335
-  _COMPRESSION._serialized_end=3401
-  _INDEXENGINE._serialized_start=3403
-  _INDEXENGINE._serialized_end=3438
-  _COMMITMODE._serialized_start=3440
-  _COMMITMODE._serialized_end=3473
+  _COMPRESSION._serialized_start=3260
+  _COMPRESSION._serialized_end=3326
+  _INDEXENGINE._serialized_start=3328
+  _INDEXENGINE._serialized_end=3363
+  _COMMITMODE._serialized_start=3365
+  _COMMITMODE._serialized_end=3398
   _ALTERINDEXREQUEST._serialized_start=74
   _ALTERINDEXREQUEST._serialized_end=290
   _ALTERINDEXRESPONSE._serialized_start=292
   _ALTERINDEXRESPONSE._serialized_end=354
   _ATTACHINDEXREQUEST._serialized_start=356
-  _ATTACHINDEXREQUEST._serialized_end=438
-  _ATTACHINDEXRESPONSE._serialized_start=440
-  _ATTACHINDEXRESPONSE._serialized_end=503
-  _COMMITINDEXREQUEST._serialized_start=505
-  _COMMITINDEXREQUEST._serialized_end=616
-  _COMMITINDEXRESPONSE._serialized_start=618
-  _COMMITINDEXRESPONSE._serialized_end=739
-  _SORTBYFIELD._serialized_start=741
-  _SORTBYFIELD._serialized_end=818
-  _CREATEINDEXREQUEST._serialized_start=821
-  _CREATEINDEXREQUEST._serialized_end=1508
-  _CREATEINDEXRESPONSE._serialized_start=1510
-  _CREATEINDEXRESPONSE._serialized_end=1573
-  _DELETEDOCUMENTREQUEST._serialized_start=1575
-  _DELETEDOCUMENTREQUEST._serialized_end=1664
-  _DELETEDOCUMENTRESPONSE._serialized_start=1666
-  _DELETEDOCUMENTRESPONSE._serialized_end=1733
-  _DELETEINDEXREQUEST._serialized_start=1735
-  _DELETEINDEXREQUEST._serialized_end=1786
-  _DELETEINDEXRESPONSE._serialized_start=1788
-  _DELETEINDEXRESPONSE._serialized_end=1809
-  _GETINDICESALIASESREQUEST._serialized_start=1811
-  _GETINDICESALIASESREQUEST._serialized_end=1837
-  _GETINDICESALIASESRESPONSE._serialized_start=1840
-  _GETINDICESALIASESRESPONSE._serialized_end=2035
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=1970
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=2035
-  _GETINDEXREQUEST._serialized_start=2037
-  _GETINDEXREQUEST._serialized_end=2087
-  _GETINDEXRESPONSE._serialized_start=2089
-  _GETINDEXRESPONSE._serialized_end=2149
-  _GETINDICESREQUEST._serialized_start=2151
-  _GETINDICESREQUEST._serialized_end=2170
-  _GETINDICESRESPONSE._serialized_start=2172
-  _GETINDICESRESPONSE._serialized_end=2238
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2240
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2331
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2334
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2466
-  _INDEXDOCUMENTREQUEST._serialized_start=2468
-  _INDEXDOCUMENTREQUEST._serialized_end=2551
-  _INDEXDOCUMENTRESPONSE._serialized_start=2553
-  _INDEXDOCUMENTRESPONSE._serialized_end=2602
-  _MERGESEGMENTSREQUEST._serialized_start=2604
-  _MERGESEGMENTSREQUEST._serialized_end=2692
-  _MERGESEGMENTSRESPONSE._serialized_start=2694
-  _MERGESEGMENTSRESPONSE._serialized_end=2717
-  _SETINDEXALIASREQUEST._serialized_start=2719
-  _SETINDEXALIASREQUEST._serialized_end=2805
-  _SETINDEXALIASRESPONSE._serialized_start=2807
-  _SETINDEXALIASRESPONSE._serialized_end=2892
-  _VACUUMINDEXREQUEST._serialized_start=2894
-  _VACUUMINDEXREQUEST._serialized_end=2947
-  _VACUUMINDEXRESPONSE._serialized_start=2949
-  _VACUUMINDEXRESPONSE._serialized_end=2970
-  _INDEX._serialized_start=2973
-  _INDEX._serialized_end=3170
-  _INDEXDOCUMENTOPERATION._serialized_start=3172
-  _INDEXDOCUMENTOPERATION._serialized_end=3224
-  _INDEXOPERATION._serialized_start=3226
-  _INDEXOPERATION._serialized_end=3333
-  _INDEXAPI._serialized_start=3476
-  _INDEXAPI._serialized_end=4650
+  _ATTACHINDEXREQUEST._serialized_end=407
+  _ATTACHINDEXRESPONSE._serialized_start=409
+  _ATTACHINDEXRESPONSE._serialized_end=472
+  _COMMITINDEXREQUEST._serialized_start=474
+  _COMMITINDEXREQUEST._serialized_end=585
+  _COMMITINDEXRESPONSE._serialized_start=587
+  _COMMITINDEXRESPONSE._serialized_end=708
+  _SORTBYFIELD._serialized_start=710
+  _SORTBYFIELD._serialized_end=787
+  _CREATEINDEXREQUEST._serialized_start=790
+  _CREATEINDEXREQUEST._serialized_end=1433
+  _CREATEINDEXRESPONSE._serialized_start=1435
+  _CREATEINDEXRESPONSE._serialized_end=1498
+  _DELETEDOCUMENTREQUEST._serialized_start=1500
+  _DELETEDOCUMENTREQUEST._serialized_end=1589
+  _DELETEDOCUMENTRESPONSE._serialized_start=1591
+  _DELETEDOCUMENTRESPONSE._serialized_end=1658
+  _DELETEINDEXREQUEST._serialized_start=1660
+  _DELETEINDEXREQUEST._serialized_end=1711
+  _DELETEINDEXRESPONSE._serialized_start=1713
+  _DELETEINDEXRESPONSE._serialized_end=1734
+  _GETINDICESALIASESREQUEST._serialized_start=1736
+  _GETINDICESALIASESREQUEST._serialized_end=1762
+  _GETINDICESALIASESRESPONSE._serialized_start=1765
+  _GETINDICESALIASESRESPONSE._serialized_end=1960
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=1895
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=1960
+  _GETINDEXREQUEST._serialized_start=1962
+  _GETINDEXREQUEST._serialized_end=2012
+  _GETINDEXRESPONSE._serialized_start=2014
+  _GETINDEXRESPONSE._serialized_end=2074
+  _GETINDICESREQUEST._serialized_start=2076
+  _GETINDICESREQUEST._serialized_end=2095
+  _GETINDICESRESPONSE._serialized_start=2097
+  _GETINDICESRESPONSE._serialized_end=2163
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2165
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2256
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2259
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2391
+  _INDEXDOCUMENTREQUEST._serialized_start=2393
+  _INDEXDOCUMENTREQUEST._serialized_end=2476
+  _INDEXDOCUMENTRESPONSE._serialized_start=2478
+  _INDEXDOCUMENTRESPONSE._serialized_end=2527
+  _MERGESEGMENTSREQUEST._serialized_start=2529
+  _MERGESEGMENTSREQUEST._serialized_end=2617
+  _MERGESEGMENTSRESPONSE._serialized_start=2619
+  _MERGESEGMENTSRESPONSE._serialized_end=2642
+  _SETINDEXALIASREQUEST._serialized_start=2644
+  _SETINDEXALIASREQUEST._serialized_end=2730
+  _SETINDEXALIASRESPONSE._serialized_start=2732
+  _SETINDEXALIASRESPONSE._serialized_end=2817
+  _VACUUMINDEXREQUEST._serialized_start=2819
+  _VACUUMINDEXREQUEST._serialized_end=2872
+  _VACUUMINDEXRESPONSE._serialized_start=2874
+  _VACUUMINDEXRESPONSE._serialized_end=2895
+  _INDEX._serialized_start=2898
+  _INDEX._serialized_end=3095
+  _INDEXDOCUMENTOPERATION._serialized_start=3097
+  _INDEXDOCUMENTOPERATION._serialized_end=3149
+  _INDEXOPERATION._serialized_start=3151
+  _INDEXOPERATION._serialized_end=3258
+  _INDEXAPI._serialized_start=3401
+  _INDEXAPI._serialized_end=4660
 # @@protoc_insertion_point(module_scope)
```

## summa/proto/index_service_pb2_grpc.py

```diff
@@ -15,14 +15,19 @@
             channel: A grpc.Channel.
         """
         self.alter_index = channel.unary_unary(
                 '/summa.proto.IndexApi/alter_index',
                 request_serializer=summa_dot_proto_dot_index__service__pb2.AlterIndexRequest.SerializeToString,
                 response_deserializer=summa_dot_proto_dot_index__service__pb2.AlterIndexResponse.FromString,
                 )
+        self.attach_index = channel.unary_unary(
+                '/summa.proto.IndexApi/attach_index',
+                request_serializer=summa_dot_proto_dot_index__service__pb2.AttachIndexRequest.SerializeToString,
+                response_deserializer=summa_dot_proto_dot_index__service__pb2.AttachIndexResponse.FromString,
+                )
         self.commit_index = channel.unary_unary(
                 '/summa.proto.IndexApi/commit_index',
                 request_serializer=summa_dot_proto_dot_index__service__pb2.CommitIndexRequest.SerializeToString,
                 response_deserializer=summa_dot_proto_dot_index__service__pb2.CommitIndexResponse.FromString,
                 )
         self.create_index = channel.unary_unary(
                 '/summa.proto.IndexApi/create_index',
@@ -86,14 +91,20 @@
 
     def alter_index(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def attach_index(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def commit_index(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def create_index(self, request, context):
@@ -166,14 +177,19 @@
 def add_IndexApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'alter_index': grpc.unary_unary_rpc_method_handler(
                     servicer.alter_index,
                     request_deserializer=summa_dot_proto_dot_index__service__pb2.AlterIndexRequest.FromString,
                     response_serializer=summa_dot_proto_dot_index__service__pb2.AlterIndexResponse.SerializeToString,
             ),
+            'attach_index': grpc.unary_unary_rpc_method_handler(
+                    servicer.attach_index,
+                    request_deserializer=summa_dot_proto_dot_index__service__pb2.AttachIndexRequest.FromString,
+                    response_serializer=summa_dot_proto_dot_index__service__pb2.AttachIndexResponse.SerializeToString,
+            ),
             'commit_index': grpc.unary_unary_rpc_method_handler(
                     servicer.commit_index,
                     request_deserializer=summa_dot_proto_dot_index__service__pb2.CommitIndexRequest.FromString,
                     response_serializer=summa_dot_proto_dot_index__service__pb2.CommitIndexResponse.SerializeToString,
             ),
             'create_index': grpc.unary_unary_rpc_method_handler(
                     servicer.create_index,
@@ -254,14 +270,31 @@
         return grpc.experimental.unary_unary(request, target, '/summa.proto.IndexApi/alter_index',
             summa_dot_proto_dot_index__service__pb2.AlterIndexRequest.SerializeToString,
             summa_dot_proto_dot_index__service__pb2.AlterIndexResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def attach_index(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/summa.proto.IndexApi/attach_index',
+            summa_dot_proto_dot_index__service__pb2.AttachIndexRequest.SerializeToString,
+            summa_dot_proto_dot_index__service__pb2.AttachIndexResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def commit_index(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

## Comparing `aiosumma-2.9.8.dist-info/METADATA` & `aiosumma-2.9.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosumma
-Version: 2.9.8
+Version: 2.9.9
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Home-page: https://github.com/izihawa/aiosumma
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Requires-Python: >=3.9
```

## Comparing `aiosumma-2.9.8.dist-info/RECORD` & `aiosumma-2.9.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-aiosumma-2.9.8.dist-info/METADATA,sha256=jzRy4O8YWYQgQU9aOptAmrGzE7aIKmRcX9anAfMXU-I,557
-aiosumma-2.9.8.dist-info/RECORD,,
-aiosumma-2.9.8.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
-aiosumma-2.9.8.dist-info/entry_points.txt,sha256=zvEtXfXN8m8MrrWuU0Kw_BwFqLnLrWYuB5tpu7TH4DU,47
+aiosumma-2.9.9.dist-info/METADATA,sha256=xHSDoahwZV6glb5PwSP5nhUavW3YLkWATxSBk6PiwTA,557
+aiosumma-2.9.9.dist-info/RECORD,,
+aiosumma-2.9.9.dist-info/WHEEL,sha256=sobxWSyDDkdg_rinUth-jxhXHqoNqlmNMJY3aTZn2Us,91
+aiosumma-2.9.9.dist-info/entry_points.txt,sha256=zvEtXfXN8m8MrrWuU0Kw_BwFqLnLrWYuB5tpu7TH4DU,47
 aiosumma/__init__.py,sha256=PX__okY1060Mk0-u6gzRZhfgJpA1mcxH-qyfCNvj-Vk,187
 aiosumma/cli.py,sha256=_3yfc76H01KWHa8cCEzAGiGiE1lbWsdo0VvEEjx8TNg,537
-aiosumma/client.py,sha256=864wnQJBukXJBeR0Hqc1qk4P6sJNo4EU2EDJzU-Dck0,20643
+aiosumma/client.py,sha256=ZUTAp6HrVxkzGVooMz_5AujWplkxmvW39EIN5CWYmkE,21221
 aiosumma/context.py,sha256=TQKZ26VJ9ALqEqu3NbkYQpdFaSx5Y-gpdUSlgfDH0ec,741
 aiosumma/data/synsets/drugs.csv,sha256=SsiCoVHJIcCY_oI4enTugr1pODv7-IFP0Q3SInAcsuU,370551
 aiosumma/errors.py,sha256=bikz5E2RduZXxbG6jCsl--3ix95mAHJdCujG_ZPxacw,126
 aiosumma/eval_scorer_builder.py,sha256=Uqchil_MMjysUBI1SORidtE1PkG6cRIpM95U9PrG44k,1322
 aiosumma/parser/__init__.py,sha256=gA8deo6hXe-JqyWU96ByOZGeiJ6jr46-IR10mE25fy4,65
 aiosumma/parser/elements.py,sha256=Tk20QxdT8px3ECwIXH_0P0zMm9QQS8yuh8n-sunDvSM,10769
 aiosumma/parser/errors.py,sha256=mSa6Cyosa8YpCjB-puHuV4CMJQkQvO1RM3koBY0G73A,147
@@ -32,15 +32,15 @@
 aiosumma/tree_transformers/synonym.py,sha256=sSpRhvftiEJSDWITdBArMRe40WYaiN2c-vTUf0coT_k,2110
 aiosumma/tree_transformers/tantivy.py,sha256=JEHsqtBChvFiS7uDrAWW_dx42-YJowBvDvkPMXQN3d8,1944
 aiosumma/tree_transformers/values.py,sha256=5ecrMKWnv7jrM8ZkDTDd6gUobjkw1I6jPhDkBBp4lAk,1609
 summa/proto/beacon_service_pb2.py,sha256=vEzkdz_oMHDxwHBmRGU1rqKTPf0-nkix6iUljPtWzuI,1641
 summa/proto/beacon_service_pb2_grpc.py,sha256=ifGr7-qwR-3KyQBwG3jWcffTDsUL4d70ubmmeDzXrQg,2697
 summa/proto/consumer_service_pb2.py,sha256=LSZeClttCY_Qccy4iS1hBsNter9UBoA1xJCax-PZ8I0,3431
 summa/proto/consumer_service_pb2_grpc.py,sha256=adsTZ3FKk9hUap02gcSkLk1V-SKm5ROPPaN3Qgm2mJE,7986
-summa/proto/index_service_pb2.py,sha256=nTb783ynk4XpRZXsxg3GSmoXqbowIdH-ifxKe8j0yUg,11339
-summa/proto/index_service_pb2_grpc.py,sha256=f4ciXFY96GlQ4Dcwq9qir27PF5QRLfBkO0UpZUJWmvw,23390
+summa/proto/index_service_pb2.py,sha256=xpEaX_LFnVQZOwKp39xor5eXcyiFEGvxGoTcAfFWewE,11331
+summa/proto/index_service_pb2_grpc.py,sha256=ou-Mf9lsY9sxh6WvABe5o4FWgECCJnX98rnPgQf8fV0,25093
 summa/proto/reflection_service_pb2.py,sha256=Li-m3kqZa-ZlcJit5Ng0cCPZb3wmyc_UbIvoK9pTUOE,2351
 summa/proto/reflection_service_pb2_grpc.py,sha256=O0VVpRqTDUt320-BIn3iG_L5QUt22zMhDW_NX1t_jzc,2751
 summa/proto/search_service_pb2.py,sha256=RMAem6wYufqtYlWMy5WbWfj4XXQ5-fnV16-psItzUhQ,23421
 summa/proto/search_service_pb2_grpc.py,sha256=uoJsDtL0FnivhGCWASySxItz0BHX8EdZJC_TnwfU03Q,2612
 summa/proto/utils_pb2.py,sha256=7rj2rrf_Y-ZCt7xTTBnxDn3CH3RgJAtZcel7VtoSwn8,998
 summa/proto/utils_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
```

