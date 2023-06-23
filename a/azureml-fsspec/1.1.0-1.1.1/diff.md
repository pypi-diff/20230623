# Comparing `tmp/azureml_fsspec-1.1.0-py3-none-any.whl.zip` & `tmp/azureml_fsspec-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10974 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      251 b- defN 23-Jun-06 00:11 azureml/__init__.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-06 00:12 azureml/fsspec/__init__.py
--rw-rw-rw-  2.0 fat    36891 b- defN 23-Jun-06 00:12 azureml/fsspec/spec.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2847 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      763 b- defN 23-Jun-06 00:25 azureml_fsspec-1.1.0.dist-info/RECORD
-9 files, 42331 bytes uncompressed, 9644 bytes compressed:  77.2%
+Zip file size: 10580 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Jun-23 05:56 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-23 05:57 azureml/fsspec/__init__.py
+-rw-rw-rw-  2.0 fat    33551 b- defN 23-Jun-23 05:57 azureml/fsspec/spec.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2847 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      763 b- defN 23-Jun-23 06:07 azureml_fsspec-1.1.1.dist-info/RECORD
+9 files, 38991 bytes uncompressed, 9250 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: azureml/fsspec/__init__.py
 Comment: 
 
 Filename: azureml/fsspec/spec.py
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/LICENSE.txt
+Filename: azureml_fsspec-1.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/METADATA
+Filename: azureml_fsspec-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/WHEEL
+Filename: azureml_fsspec-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/entry_points.txt
+Filename: azureml_fsspec-1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/top_level.txt
+Filename: azureml_fsspec-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_fsspec-1.1.0.dist-info/RECORD
+Filename: azureml_fsspec-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/fsspec/spec.py

```diff
@@ -13,19 +13,17 @@
 from fsspec.implementations.local import make_path_posix
 
 import os
 import pathlib
 import re
 import inspect
 from glob import has_magic
-import azureml.dataprep as _dprep
 from azureml.dataprep.api._loggerfactory import track, _LoggerFactory
 from azureml.dataprep.api._constants import ACTIVITY_INFO_KEY, ERROR_CODE_KEY, \
     COMPLIANT_MESSAGE_KEY, OUTER_ERROR_CODE_KEY
-from azureml.dataprep.api.functions import get_stream_properties
 from azureml.dataprep.rslex import StreamInfo, CachingOptions, BufferingOptions, Downloader, \
     Copier, PyIfDestinationExists, PyLocationInfo, PyDatastoreSource
 from azureml.dataprep.api._rslex_executor import ensure_rslex_environment
 from azureml.dataprep import UserErrorException
 
 
 _PUBLIC_API = 'PublicApi'
@@ -255,61 +253,14 @@
                     just relative path in the format of {datastore}/{relative_path}
         :type path: str
         :return: A list of file paths
         :rtype: list[str]
         """
         return sync(self.loop, self._glob, path)
 
-    async def _glob(self, path=None, **kwargs):
-        """
-        globbing result for the uri
-
-        :param path: path to glob, default to be the uri from __init__
-        :type path: str
-        :return: A list of file paths
-        :rtype: list[str]
-        """
-        custom_dimensions = {'app_name': _APP_NAME}
-        custom_dimensions.update(self._workspace_context)
-
-        with _LoggerFactory.track_activity(_get_logger(), '_glob', _PUBLIC_API,
-                                           custom_dimensions) as activityLogger:
-            try:
-                if not path:
-                    path = self._path
-                path = self._strip_protocol(
-                    path, self._workspace_context).rstrip("/")
-                path = self._get_full_path_from_fs_root(path)
-                dataflow = _dprep.Dataflow(
-                    _dprep.api.engineapi.api.get_engine_api())
-                dataflow = dataflow.add_step(
-                    'Microsoft.DPrep.GetDatastoreFilesBlock',
-                    {'datastores': [self._construct_datastore_source(path)]})
-                stream_properties_expression = get_stream_properties(dataflow['Path'])
-                dataflow = dataflow._add_columns_from_record(stream_properties_expression)
-                records = dataflow._to_pyrecords()
-                if len(records) < 1:
-                    raise ValueError(f'No files found for {path}')
-                else:
-                    files = []
-                    for r in records:
-                        name = r['Path'].resource_identifier[len(self._datastore_source['datastoreName']) + 1:]
-                        files.append(name)
-                return files
-            except Exception as e:
-                if hasattr(activityLogger, ACTIVITY_INFO_KEY):
-                    activityLogger.activity_info['error_code'] = getattr(
-                        e, ERROR_CODE_KEY, '')
-                    activityLogger.activity_info['message'] = getattr(
-                        e, COMPLIANT_MESSAGE_KEY, str(e))
-                    activityLogger.activity_info['outer_error_code'] = getattr(
-                        e, OUTER_ERROR_CODE_KEY, '')
-
-                AzureMachineLearningFileSystem._map_user_error(e)
-
     async def _ls(self, path=None, detail=False, refresh=True, **kwargs):
         """
         List uri, this will return the full list of files iteratively.
 
         :param path: path to list
         :type path: str
         :param detail: whether to return details other than path
@@ -416,34 +367,16 @@
 
                 if not path:
                     path = self._path
                 path = self._strip_protocol(path, self._workspace_context)
                 path = self._get_full_path_from_fs_root(path)
                 self._validate_args_for_open(mode)
 
-                dataflow = _dprep.Dataflow(
-                    _dprep.api.engineapi.api.get_engine_api())
-
-                # construct datastore source on top of the workspace context from __init__
-                dataflow = dataflow.add_step(
-                    'Microsoft.DPrep.GetDatastoreFilesBlock',
-                    {'datastores': [self._construct_datastore_source(path)]})
-                stream_properties_expression = get_stream_properties(
-                    dataflow['Path'])
-                dataflow = dataflow._add_columns_from_record(
-                    stream_properties_expression)
-                records = dataflow._to_pyrecords()
-                if len(records) < 1:
-                    raise ValueError("File not found for the path to open")
-                if len(records) > 1:
-                    raise ValueError("Path is not a single file path")
-
-                r = records[0]
                 si = StreamInfo(
-                    r['Path'].handler, r['Path'].resource_identifier, r['Path'].arguments)
+                    _DATASTORE_HANDLER, path, self._datastore_source)
                 downloader = Downloader(block_size=8 * 1024 * 1024, read_threads=read_threads,
                                         caching_options=CachingOptions(memory_cache_size=memory_cache_size))
 
                 return si.open(buffering_options=BufferingOptions(64, downloader))
             except Exception as e:
                 if hasattr(activityLogger, ACTIVITY_INFO_KEY):
                     activityLogger.activity_info['error_code'] = getattr(
```

## Comparing `azureml_fsspec-1.1.0.dist-info/LICENSE.txt` & `azureml_fsspec-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_fsspec-1.1.0.dist-info/METADATA` & `azureml_fsspec-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-fsspec
-Version: 1.1.0
+Version: 1.1.1
 Summary: Access datastore uri with fsspec
 Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
 Author: Microsoft Corp
 License: Proprietary https://aka.ms/azureml-preview-sdk-license 
 Keywords: file-system,dask,azure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

