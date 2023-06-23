# Comparing `tmp/deeplake-3.6.4.tar.gz` & `tmp/deeplake-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.4.tar", last modified: Fri Jun 16 18:26:43 2023, max compression
+gzip compressed data, was "deeplake-3.6.5.tar", last modified: Tue Jun 20 17:42:28 2023, max compression
```

## Comparing `deeplake-3.6.4.tar` & `deeplake-3.6.5.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-16 18:24:57.000000 deeplake-3.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-16 18:24:57.000000 deeplake-3.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-16 18:26:43.728096 deeplake-3.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25351 2023-06-16 18:24:57.000000 deeplake-3.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99372 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    85180 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    18863 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    13490 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   113519 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171829 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    15422 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15995 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13705 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50140 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51556 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25170 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    35113 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12673 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10090 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5040 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)    11940 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25897 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22353 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9862 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4015 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16165 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34773 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8435 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25235 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12677 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-16 18:26:43.728096 deeplake-3.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-16 18:24:57.000000 deeplake-3.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.082560 deeplake-3.6.5/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-20 17:40:56.000000 deeplake-3.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 17:40:56.000000 deeplake-3.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-20 17:42:28.082560 deeplake-3.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25351 2023-06-20 17:40:56.000000 deeplake-3.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99372 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    88006 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18863 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    13490 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   117098 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   172516 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15995 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13833 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50495 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51556 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25913 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    35654 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10090 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.062560 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)    11940 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16165 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34773 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.072560 deeplake-3.6.5/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.082560 deeplake-3.6.5/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25235 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.082560 deeplake-3.6.5/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-20 17:40:56.000000 deeplake-3.6.5/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:42:28.052560 deeplake-3.6.5/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-20 17:42:27.000000 deeplake-3.6.5/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-20 17:42:28.082560 deeplake-3.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-20 17:40:56.000000 deeplake-3.6.5/setup.py
```

### Comparing `deeplake-3.6.4/LICENSE` & `deeplake-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/PKG-INFO` & `deeplake-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.4
+Version: 3.6.5
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.4 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.5 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.4/README.md` & `deeplake-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/__init__.py` & `deeplake-3.6.5/deeplake/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.4"
+__version__ = "3.6.5"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.6.4/deeplake/api/dataset.py` & `deeplake-3.6.5/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/info.py` & `deeplake-3.6.5/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/link.py` & `deeplake-3.6.5/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/link_tiled.py` & `deeplake-3.6.5/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/read.py` & `deeplake-3.6.5/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.5/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.5/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_api.py` & `deeplake-3.6.5/deeplake/api/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     InvalidDatasetNameException,
     UnsupportedParameterException,
     DynamicTensorNumpyError,
 )
 from deeplake.util.path import convert_string_to_pathlib_if_needed, verify_dataset_name
 from deeplake.util.testing import assert_array_equal
 from deeplake.util.pretty_print import summary_tensor, summary_dataset
+from deeplake.util.shape_interval import ShapeInterval
 from deeplake.constants import GDRIVE_OPT, MB
 from deeplake.client.config import REPORTING_CONFIG_FILE_PATH
 
 from click.testing import CliRunner
 from deeplake.cli.auth import login, logout
 from deeplake.util.bugout_reporter import feature_report_path
 from rich import print as rich_print
@@ -244,14 +245,37 @@
     )
     assert (
         summary_tensor(ds.images)
         == "\n  htype    shape    dtype  compression\n -------  -------  -------  ------- \n  image    (0,)     int32    jpeg   "
     )
 
 
+def test_view_summary(memory_ds, capsys):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend(np.ones((2500, 10, 5, 3)))
+        ds.abc.extend(np.ones((5000, 5, 5, 3)))
+        ds.abc.extend(np.ones((5000, 5, 10, 3)))
+
+        with pytest.raises(ValueError):
+            ds[2500:].summary()
+
+        ds[2500:].summary(force=True)
+        captured = capsys.readouterr().out
+        assert (
+            captured
+            == f"{str(ds[2500:])}\n\n tensor    htype          shape          dtype  compression\n -------  -------        -------        -------  ------- \n   abc    generic  (10000, 5, 5:10, 3)   None     None   \n"
+        )
+
+        assert (
+            summary_dataset(ds[:7500])
+            == "\n tensor    htype         shape          dtype  compression\n -------  -------       -------        -------  ------- \n   abc    generic  (7500, 5:10, 5, 3)   None     None   "
+        )
+
+
 def test_log(memory_ds, capsys):
     with memory_ds as ds:
         ds.create_tensor("abc")
         ds.abc.extend([1, 2, 3, 4])
 
         header = "---------------\nDeep Lake Version Log\n---------------\n\n"
         current_branch = "Current Branch: main\n"
@@ -2598,25 +2622,73 @@
             np.testing.assert_array_equal(shape, shapes[i])
 
         np.testing.assert_array_equal(ds.abc[0].shapes(), np.array([[[3, 4], [4, 5]]]))
         np.testing.assert_array_equal(
             ds.abc[:3].shapes(),
             np.array([[[3, 4], [4, 5]], [[2, 3], [3, 4]], [[0, 0], [0, 0]]]),
         )
+        np.testing.assert_array_equal(
+            ds.abc[1:3].shapes(),
+            np.array([[[2, 3], [3, 4]], [[0, 0], [0, 0]]]),
+        )
 
 
 def test_shape_squeeze(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc")
         ds.abc.extend(np.ones((5, 10, 10, 10)))
         ds.abc.extend(np.ones((5, 10, 12, 20)))
 
     assert ds.abc[5:, :, 9].shape == (5, 10, 20)
 
 
+def test_slice_shape_interval(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend(np.ones((2, 1, 2, 3)))
+        ds.abc.extend(np.ones((2, 3, 4, 5)))
+        ds.abc.extend(np.ones((2, 5, 6, 2)))
+
+    assert ds.abc.shape_interval == ShapeInterval((6, 1, 2, 2), (6, 5, 6, 5))
+    assert ds[:4].abc.shape_interval == ShapeInterval((4, 1, 2, 3), (4, 3, 4, 5))
+    assert ds[2:].abc.shape_interval == ShapeInterval((4, 3, 4, 2), (4, 5, 6, 5))
+
+    with memory_ds as ds:
+        ds.create_tensor("regular_seq", htype="sequence")
+        ds.regular_seq.extend(np.ones((2, 2, 1, 2, 3)))
+        ds.regular_seq.extend(np.ones((2, 2, 3, 4, 5)))
+        ds.regular_seq.extend(np.ones((2, 2, 5, 6, 2)))
+
+    assert ds.regular_seq.shape_interval == ShapeInterval(
+        (6, 2, 1, 2, 2), (6, 2, 5, 6, 5)
+    )
+    assert ds.regular_seq[:4].shape_interval == ShapeInterval(
+        (4, 2, 1, 2, 3), (4, 2, 3, 4, 5)
+    )
+    assert ds.regular_seq[2:].shape_interval == ShapeInterval(
+        (4, 2, 3, 4, 2), (4, 2, 5, 6, 5)
+    )
+
+    with memory_ds as ds:
+        ds.create_tensor("irregular_seq", htype="sequence")
+        ds.irregular_seq.extend([np.ones((2, 1, 2, 3)), np.ones((3, 3, 4, 5))])
+        ds.irregular_seq.extend([np.ones((3, 5, 6, 2)), np.ones((4, 7, 8, 9))])
+        ds.irregular_seq.extend(np.ones((2, 1, 5, 5, 3)))
+
+    assert ds.irregular_seq.shape_interval == ShapeInterval(
+        (6, 1, 1, 2, 2), (6, 4, 7, 8, 9)
+    )
+    assert ds.irregular_seq[:4].shape_interval == ShapeInterval(
+        (4, 2, 1, 2, 2), (4, 4, 7, 8, 9)
+    )
+    assert ds.irregular_seq[2:].shape_interval == ShapeInterval(
+        (4, 1, 5, 5, 2), (4, 4, 7, 8, 9)
+    )
+
+
 def test_non_local_org_id():
     with pytest.raises(ValueError):
         ds = deeplake.dataset("hub://test/test_dataset", org_id="test")
 
     with pytest.raises(ValueError):
         ds = deeplake.empty("hub://test/test_dataset", org_id="test")
```

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.5/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.5/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.5/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.5/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.5/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.5/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.5/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_events.py` & `deeplake-3.6.5/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.5/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_info.py` & `deeplake-3.6.5/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.5/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_json.py` & `deeplake-3.6.5/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_link.py` & `deeplake-3.6.5/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.5/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_linking.py` & `deeplake-3.6.5/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.5/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_meta.py` & `deeplake-3.6.5/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.5/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_none.py` & `deeplake-3.6.5/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.5/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.5/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.5/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.5/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_pop.py` & `deeplake-3.6.5/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.5/deeplake/api/tests/test_readonly.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,7 +41,20 @@
     with pytest.raises(ReadOnlyModeError):
         ds.tensor.info.update(key=0)
 
 
 @pytest.mark.xfail(raises=CouldNotCreateNewDatasetException, strict=True)
 def test_readonly_doesnt_exist(local_path):
     deeplake.dataset(local_path, read_only=True)
+
+
+def test_readonly_viewer(capsys, hub_cloud_dev_token):
+    # testingacc2 is viewer on notify org
+    ds = deeplake.load("hub://notify/p-8M-trp", token=hub_cloud_dev_token)
+
+    out = capsys.readouterr()
+    assert (
+        "Opening dataset in read-only mode as you don't have write permissions."
+        in out.out
+    )
+
+    assert ds.read_only
```

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.5/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_reset.py` & `deeplake-3.6.5/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.5/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_text.py` & `deeplake-3.6.5/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.5/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_video.py` & `deeplake-3.6.5/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tests/test_views.py` & `deeplake-3.6.5/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/api/tiled.py` & `deeplake-3.6.5/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/structured/base.py` & `deeplake-3.6.5/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.5/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.5/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.5/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.5/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.5/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/base.py` & `deeplake-3.6.5/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.5/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.5/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.5/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.5/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.5/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.5/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/util.py` & `deeplake-3.6.5/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.5/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.5/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/cli/auth.py` & `deeplake-3.6.5/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/cli/test_cli.py` & `deeplake-3.6.5/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/client/client.py` & `deeplake-3.6.5/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/client/config.py` & `deeplake-3.6.5/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/client/log.py` & `deeplake-3.6.5/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/client/test_client.py` & `deeplake-3.6.5/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/client/utils.py` & `deeplake-3.6.5/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/compression.py` & `deeplake-3.6.5/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/constants.py` & `deeplake-3.6.5/deeplake/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,7 +239,9 @@
         "name": "id",
         "htype": "text",
         "create_id_tensor": False,
         "create_sample_info_tensor": False,
         "create_shape_tensor": False,
     },
 ]
+
+VIEW_SUMMARY_SAFE_LIMIT = 10000
```

### Comparing `deeplake-3.6.4/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.5/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.5/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.5/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.5/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.5/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.5/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.5/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/chunk_engine.py` & `deeplake-3.6.5/deeplake/core/chunk_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2486,15 +2486,16 @@
     def _sequence_item_length_range(self):
         """Returns minimum and maximum length of items in a sequence"""
         enc = self.sequence_encoder
         nrows = len(enc._encoded)
         if nrows == 0:
             return 0, 0
         min_ = max_ = enc[0][1] - enc[0][0]
-        for i in range(1, nrows):
+        # sequence length is number of samples in tensor
+        for i in range(1, self._sequence_length):
             length = enc[i][1] - enc[i][0]
             if length < min_:
                 min_ = length
             elif length > max_:
                 max_ = length
         return min_, max_
 
@@ -2545,14 +2546,16 @@
         sample_indices = list(
             index_0.indices(self._sequence_length or self.num_samples)
         )
         num_samples = len(sample_indices)
 
         sample_ndim = self.ndim() - 1
 
+        bad_shapes = []
+        offset = 0
         for i, idx in enumerate(sample_indices):
             if self.tensor_meta.htype in ("text", "json"):
                 shape = (1,)
             elif sample_shape_provider:
                 shape = self._get_sample_shape_from_provider(
                     sample_shape_provider, idx, sample_index, flatten
                 )
@@ -2561,19 +2564,29 @@
                 shape = self.read_shape_for_sample(idx)  # type: ignore
                 # if link verification was not done
                 if len(shape) > sample_ndim:
                     sample_ndim = len(shape)
                     sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
 
             if flatten:
-                start, end = self.sequence_encoder[i]
-                sample_shapes[start:end] = shape
+                # fill sample shapes with sequence item shapes, no nesting
+                start, end = self.sequence_encoder[idx]
+                length = end - start
+                sample_shapes[offset : offset + length] = shape
+                offset += length
             else:
-                sample_shapes[i] = shape
-        return sample_shapes
+                try:
+                    sample_shapes[i] = shape
+                except ValueError:
+                    # Backwards compatibility for old datasets with
+                    # grayscale images stored as (H, W) instead of (H, W, 1)
+                    if len(shape) == 2 and sample_shapes.shape[1] == 3:
+                        sample_shapes[i] = shape + (1,)
+                        bad_shapes.append(i)
+        return sample_shapes, bad_shapes
 
     def _get_total_samples_and_sample_ndim(self, index_0):
         """Returns total number of samples (including sequence items) and sample ndim using first index"""
         tensor_ndim = self.ndim()
         if self.is_sequence:
             sample_indices = list(index_0.indices(self._sequence_length))
             num_samples = sum(
@@ -2588,56 +2601,77 @@
             sample_ndim = tensor_ndim - 1
         return num_samples, sample_ndim
 
     def _group_flat_shapes(self, sample_shapes, index_0, sample_ndim):
         """Groups shapes of flattened sequence items"""
         sample_indices = list(index_0.indices(self._sequence_length))
         num_samples = len(sample_indices)
+        seq_item_length = self.sequence_encoder[sample_indices[0]]
+        seq_item_length = seq_item_length[1] - seq_item_length[0]
+        # try reshape to (num_samples, seq_item_length, sample_ndim)
         try:
+            if isinstance(sample_shapes, list):
+                raise ValueError
             sample_shapes = sample_shapes[np.newaxis, :].reshape(
-                num_samples, -1, sample_ndim
+                num_samples, seq_item_length, sample_ndim
             )
             return sample_shapes
         except ValueError:
             sample_shapes_list = []
-            for i in sample_indices:
-                start, end = self.sequence_encoder[i]
-                sample_shapes_list.append(sample_shapes[start:end])
+            offset = 0
+            for i, idx in enumerate(sample_indices):
+                start, end = self.sequence_encoder[idx]
+                length = end - start
+                sample_shapes_list.append(sample_shapes[offset : offset + length])
+                offset += length
             return sample_shapes_list
 
     def shapes(
         self,
         index: Index,
         sample_shape_provider: Optional[Callable] = None,
         pad_tensor: bool = False,
+        convert_bad_to_list: bool = True,
     ):
         if len(index) > 1:
             raise IndexError(f"`.shapes` only accepts indexing on the primary axis.")
 
         index_0 = index.values[0]
         num_samples, sample_ndim = self._get_total_samples_and_sample_ndim(index_0)
 
         sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
 
-        shape = self.shape_interval(index).astuple()[1:]
+        if (
+            index.is_trivial()
+            or self.tensor_meta.min_shape == self.tensor_meta.max_shape
+            or num_samples == 0
+        ):
+            shape = self.shape_interval(index).astuple()[1:]
+        else:
+            shape = None
 
         if (
             not index_0.subscriptable()
             and pad_tensor
             and index_0.value >= self.tensor_length  # type: ignore
         ):
             shape = self.get_empty_sample().shape
 
-        if num_samples > 0 and None in shape or self.tensor_meta.is_link:
-            sample_shapes = self._populate_sample_shapes(
+        if shape is None or None in shape or self.tensor_meta.is_link:
+            sample_shapes, bad_shapes = self._populate_sample_shapes(
                 sample_shapes,
                 index,
                 sample_shape_provider,
                 flatten=True if self.is_sequence else False,
             )
+            # convert to list if grayscale images were stored as (H, W) instead of (H, W, 1)
+            if bad_shapes and convert_bad_to_list:
+                sample_shapes = sample_shapes.tolist()
+                for i in bad_shapes:
+                    sample_shapes[i] = sample_shapes[i][:-1]
             if self.is_sequence:
                 sample_shapes = self._group_flat_shapes(
                     sample_shapes, index_0, sample_ndim
                 )
         else:
             sample_shapes[:] = shape
 
@@ -2685,59 +2719,62 @@
         if (
             not index_0.subscriptable()
             and pad_tensor
             and index_0.value >= self.tensor_length  # type: ignore
         ):
             return self.get_empty_sample().shape
 
-        shape = self.shape_interval(index).astuple()
-        if index_0.is_trivial():
-            return shape
-
         num_samples = index_0.length(self._sequence_length or self.num_samples)
-        if num_samples == 0:
+        if index_0.is_trivial() or num_samples == 0:
+            shape = self.shape_interval(index).astuple()
             return shape
+        elif self.tensor_meta.min_shape == self.tensor_meta.max_shape:
+            shape = self.shape_interval(index).astuple()[1:]
+        else:
+            shape = None
 
-        shape = shape[1:]
         sample_ndim = tensor_ndim - 1
         sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
 
-        if None in shape or self.tensor_meta.is_link:
-            sample_shapes = self._populate_sample_shapes(
+        if shape is None or None in shape or self.tensor_meta.is_link:
+            sample_shapes, bad_shapes = self._populate_sample_shapes(
                 sample_shapes, index, sample_shape_provider, flatten=False
             )
             sample_ndim = sample_shapes.shape[1]
         else:
             sample_shapes[:] = shape
 
         squeeze_dims = self._apply_deeper_indexing(
             sample_shapes, num_samples, sample_index
         )
         shape = self._sample_shapes_to_shape(sample_shapes, squeeze_dims, sample_ndim)
 
         if index_0.subscriptable():
             shape = (num_samples, *shape)  # type: ignore
 
-        return shape
+        return shape  # type: ignore
 
     def ndim(self, index: Optional[Index] = None) -> int:
         ndim = len(self.tensor_meta.min_shape) + 1
         if self.is_sequence:
             ndim += 1
         if index:
             for idx in index.values:
                 if not idx.subscriptable():
                     ndim -= 1
         return ndim
 
-    def shape_interval(self, index: Index) -> ShapeInterval:
+    def shape_interval(
+        self, index: Index, sample_shape_provider: Optional[Callable] = None
+    ) -> ShapeInterval:
         """Returns a `ShapeInterval` object that describes this tensor's shape more accurately. Length is included.
 
         Args:
             index (Index): Index to use for shape calculation.
+            sample_shape_provider (Optional, Callable): Function that returns a sample shape for a given index.
 
         Note:
             If you are expecting a `tuple`, use `tensor.shape` instead.
 
         Example:
             >>> tensor.append(np.zeros((10, 10)))
             >>> tensor.append(np.zeros((10, 15)))
@@ -2747,22 +2784,54 @@
             (2, 10, 10:15)
 
         Returns:
             ShapeInterval: Object containing `lower` and `upper` properties.
         """
         meta = self.tensor_meta
         if self.is_sequence:
-            seq_length = index.length(self._sequence_length)
-            min_item_length, max_item_length = self._sequence_item_length_range
-            min_length = [seq_length, min_item_length]
-            max_length = [seq_length, max_item_length]
+            tensor_length = index.length(self._sequence_length)
         else:
-            min_length = max_length = [index.length(meta.length)]
-        min_shape = min_length + list(meta.min_shape)
-        max_shape = max_length + list(meta.max_shape)
+            tensor_length = index.length(meta.length)
+
+        if index.is_trivial() or meta.min_shape == meta.max_shape or tensor_length == 0:
+            if self.is_sequence:
+                min_item_length, max_item_length = self._sequence_item_length_range
+                min_length = [tensor_length, min_item_length]
+                max_length = [tensor_length, max_item_length]
+            else:
+                min_length = max_length = [tensor_length]
+            min_shape = min_length + list(meta.min_shape)
+            max_shape = max_length + list(meta.max_shape)
+        else:
+            # need to fetch all shapes for the index
+            shapes = self.shapes(
+                index, sample_shape_provider, convert_bad_to_list=False
+            )
+            if self.is_sequence:
+                if isinstance(shapes, np.ndarray):
+                    # uniform sequence of shape (num_samples, num_items, ...)
+                    min_shape = [*shapes.shape[:-1], *np.amin(shapes, axis=(0, 1))]
+                    max_shape = [*shapes.shape[:-1], *np.amax(shapes, axis=(0, 1))]
+                else:
+                    # non-uniform sequence
+                    item_lengths = list(map(len, shapes))
+                    min_item_length, max_item_length = min(item_lengths), max(
+                        item_lengths
+                    )
+                    min_item_shape = np.amin(
+                        list(map(lambda x: np.amin(x, axis=0), shapes)), axis=0
+                    )
+                    max_item_shape = np.amax(
+                        list(map(lambda x: np.amax(x, axis=0), shapes)), axis=0
+                    )
+                    min_shape = [len(shapes), min_item_length, *min_item_shape]
+                    max_shape = [len(shapes), max_item_length, *max_item_shape]
+            else:
+                min_shape = [len(shapes), *np.amin(shapes, axis=0)]
+                max_shape = [len(shapes), *np.amax(shapes, axis=0)]
 
         return ShapeInterval(min_shape, max_shape)
 
     def _transform_callback(
         self, samples, flat: Optional[bool], progressbar: bool = False
     ):
         """Used in transforms to handle linked tensors."""
```

### Comparing `deeplake-3.6.4/deeplake/core/compression.py` & `deeplake-3.6.5/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/compute/process.py` & `deeplake-3.6.5/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/compute/provider.py` & `deeplake-3.6.5/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/compute/ray.py` & `deeplake-3.6.5/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/compute/serial.py` & `deeplake-3.6.5/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/compute/thread.py` & `deeplake-3.6.5/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/dataset/__init__.py` & `deeplake-3.6.5/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/dataset/dataset.py` & `deeplake-3.6.5/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
         d["_client"] = d["ds_name"] = None
         # uniquely identifies dataset
         d["path"] = convert_pathlib_to_string_if_needed(path) or get_path_from_storage(
             storage
         )
         d["storage"] = storage
         d["_read_only_error"] = read_only is False
-        d["_read_only"] = DEFAULT_READONLY if read_only is None else read_only
         d["base_storage"] = get_base_storage(storage)
+        d["_read_only"] = d["base_storage"].read_only
         d["_locked_out"] = False  # User requested write access but was denied
         d["is_iteration"] = is_iteration
         d["is_first_load"] = version_state is None
         d["_is_filtered_view"] = False
         d["index"] = index or Index()
         d["group_index"] = group_index
         d["_token"] = token
@@ -2398,19 +2398,36 @@
             size = self.size_approx()
             if size > deeplake.constants.DELETE_SAFETY_SIZE:
                 raise DatasetTooLargeToDelete(self.path)
 
         self._unlock()
         self.storage.clear()
 
-    def summary(self):
-        """Prints a summary of the dataset."""
+    def summary(self, force: bool = False):
+        """Prints a summary of the dataset.
+
+        Args:
+            force (bool): Dataset views with more than 10000 samples might take a long time to summarize. If `force=True`,
+                the summary will be printed regardless. An error will be raised otherwise.
+
+        Raises:
+            ValueError: If the dataset view might take a long time to summarize and `force=False`
+        """
 
         deeplake_reporter.feature_report(feature_name="summary", parameters={})
 
+        if (
+            not self.index.is_trivial()
+            and self.max_len >= deeplake.constants.VIEW_SUMMARY_SAFE_LIMIT
+            and not force
+        ):
+            raise ValueError(
+                "Dataset views with more than 10000 samples might take a long time to summarize. Use `force=True` to override."
+            )
+
         pretty_print = summary_dataset(self)
 
         print(self)
         print(pretty_print)
 
     def __str__(self):
         path_str = ""
```

### Comparing `deeplake-3.6.4/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.5/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     RenameError,
     ReadOnlyModeError,
 )
 from deeplake.util.link import save_link_creds
 from deeplake.util.path import is_hub_cloud_path
 from deeplake.util.tag import process_hub_path
 from deeplake.util.logging import log_visualizer_link
-from deeplake.util.storage import storage_provider_from_hub_path
+from deeplake.util.storage import (
+    storage_provider_from_hub_path,
+    get_dataset_credentials,
+)
 from warnings import warn
 import time
 import deeplake
 
 
 class DeepLakeCloudDataset(Dataset):
     """Subclass of :class:`Dataset`. Deep Lake cloud datasets are those datasets which are stored on Activeloop servers, their paths look like:
@@ -373,21 +376,29 @@
     def _temp_write_access(self):
         if not self.read_only or self._locked_out:
             return memoryview(b"")  # No-op context manager
 
         class _TmpWriteAccess:
             def __enter__(self2):
                 self2.orig_storage = self.base_storage
-                storage = storage_provider_from_hub_path(
-                    self.path, read_only=False, token=self._token
+
+                # check for write access
+                client = DeepLakeBackendClient(self._token)
+                _, org_id, ds_name, _ = process_hub_path(self.path)
+                _, _, mode, _, _ = get_dataset_credentials(
+                    client, org_id, ds_name, mode=None, db_engine=False
                 )
-                if storage.read_only:
+                if mode == "r":
                     raise ReadOnlyModeError(
                         f"You do not have permission to write to this dataset ({self.path})."
                     )
+
+                storage = storage_provider_from_hub_path(
+                    self.path, read_only=False, token=self._token
+                )
                 self.base_storage = storage
 
             def __exit__(self2, *_, **__):
                 self.base_storage = self2.orig_storage
 
         return _TmpWriteAccess()
```

### Comparing `deeplake-3.6.4/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.5/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.5/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.5/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.5/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/fast_forwarding.py` & `deeplake-3.6.5/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/index/index.py` & `deeplake-3.6.5/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/io.py` & `deeplake-3.6.5/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/ipc.py` & `deeplake-3.6.5/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/link_creds.py` & `deeplake-3.6.5/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.5/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/linked_sample.py` & `deeplake-3.6.5/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.5/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/lock.py` & `deeplake-3.6.5/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.5/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.5/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.5/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.5/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.5/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.5/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.5/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.5/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.5/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.5/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/partial_reader.py` & `deeplake-3.6.5/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/partial_sample.py` & `deeplake-3.6.5/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/polygon.py` & `deeplake-3.6.5/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/query/autocomplete.py` & `deeplake-3.6.5/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/query/filter.py` & `deeplake-3.6.5/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/query/query.py` & `deeplake-3.6.5/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/sample.py` & `deeplake-3.6.5/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/serialize.py` & `deeplake-3.6.5/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/azure.py` & `deeplake-3.6.5/deeplake/core/storage/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import posixpath
 import time
+import logging
 from typing import Dict, Optional, Tuple
 from datetime import datetime, timedelta, timezone
 
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.util.exceptions import PathNotEmptyException
 
@@ -11,18 +12,20 @@
     from azure.identity import DefaultAzureCredential
     from azure.storage.blob import (
         BlobServiceClient,
         BlobSasPermissions,
         ContainerSasPermissions,
         generate_blob_sas,
         generate_container_sas,
-        generate_account_sas,
     )
     from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
 
+    logger = logging.getLogger("azure.identity")
+    logger.setLevel(logging.ERROR)
+
     _AZURE_PACKAGES_INSTALLED = True
 except ImportError:
     _AZURE_PACKAGES_INSTALLED = False
 
 
 class AzureProvider(StorageProvider):
     def __init__(self, root: str, creds: Dict = {}, token: Optional[str] = None):
@@ -223,15 +226,17 @@
         self.hub_path = hub_path
         self.tag = hub_path[6:]  # removing the hub:// part from the path
         self.expiration = expiration
         self.db_engine = db_engine
         self.repository = repository
 
     def subdir(self, path: str, read_only: bool = False):
-        sd = self.__class__(root=posixpath.join(self.root, path))
+        sd = self.__class__(
+            root=posixpath.join(self.root, path), creds=self.creds, token=self.token
+        )
         if self.expiration:
             sd._set_hub_creds_info(
                 self.hub_path, self.expiration, self.db_engine, self.repository
             )
         sd.read_only = read_only
         return sd
```

### Comparing `deeplake-3.6.4/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.5/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/gcs.py` & `deeplake-3.6.5/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/google_drive.py` & `deeplake-3.6.5/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/local.py` & `deeplake-3.6.5/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.5/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/memory.py` & `deeplake-3.6.5/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/provider.py` & `deeplake-3.6.5/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/storage/s3.py` & `deeplake-3.6.5/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tensor.py` & `deeplake-3.6.5/deeplake/core/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,15 +586,21 @@
 
         Returns:
             ShapeInterval: Object containing ``lower`` and ``upper`` properties.
 
         Note:
             If you are expecting a tuple, use :attr:`shape` instead.
         """
-        return self.chunk_engine.shape_interval(self.index)
+        sample_shape_tensor = self._sample_shape_tensor
+        sample_shape_provider = (
+            self._sample_shape_provider(sample_shape_tensor)
+            if sample_shape_tensor
+            else None
+        )
+        return self.chunk_engine.shape_interval(self.index, sample_shape_provider)
 
     @property
     def is_dynamic(self) -> bool:
         """Will return ``True`` if samples in this tensor have shapes that are unequal."""
         return self.shape_interval.is_dynamic
 
     @property
@@ -1139,21 +1145,25 @@
         if self.is_sequence:
 
             def get_sample_shape(global_sample_index: int):
                 seq_pos = slice(
                     *self.chunk_engine.sequence_encoder[global_sample_index]
                 )
                 idx = Index([IndexEntry(seq_pos)])
-                shapes = sample_shape_tensor[idx].numpy()
+                shapes = sample_shape_tensor[idx].numpy(fetch_chunks=True)
                 return shapes
 
         else:
 
             def get_sample_shape(global_sample_index: int):
-                return tuple(sample_shape_tensor[global_sample_index].numpy().tolist())
+                return tuple(
+                    sample_shape_tensor[global_sample_index]
+                    .numpy(fetch_chunks=True)
+                    .tolist()
+                )
 
         return get_sample_shape
 
     def _get_sample_info_at_index(self, global_sample_index: int, sample_info_tensor):
         if self.is_sequence:
             return [
                 sample_info_tensor[i].data()
```

### Comparing `deeplake-3.6.4/deeplake/core/tensor_link.py` & `deeplake-3.6.5/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/test_serialize.py` & `deeplake-3.6.5/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_compression.py` & `deeplake-3.6.5/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_compute.py` & `deeplake-3.6.5/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.5/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_io.py` & `deeplake-3.6.5/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_locking.py` & `deeplake-3.6.5/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.5/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.5/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.5/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.5/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.5/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/serialize.py` & `deeplake-3.6.5/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.5/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.5/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/transform/test_transform.py` & `deeplake-3.6.5/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/transform/transform.py` & `deeplake-3.6.5/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.5/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.5/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.5/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.5/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from deeplake.util.bugout_reporter import feature_report_path, deeplake_reporter
 
 logger = logging.getLogger(__name__)
 
 
 class VectorStore:
-    """Base class for DeepLakeVectorStore"""
+    """Base class for VectorStore"""
 
     def __init__(
         self,
         path: Union[str, pathlib.Path],
         tensor_params: List[Dict[str, object]] = DEFAULT_VECTORSTORE_TENSORS,
         embedding_function: Optional[Callable] = None,
         read_only: Optional[bool] = False,
@@ -38,31 +38,31 @@
         num_workers: int = 0,
         exec_option: str = "python",
         token: Optional[str] = None,
         overwrite: bool = False,
         verbose=True,
         **kwargs: Any,
     ) -> None:
-        """Creates an empty DeepLakeVectorStore or loads an existing one if it exists at the specified ``path``.
+        """Creates an empty VectorStore or loads an existing one if it exists at the specified ``path``.
 
         Examples:
             >>> # Create a vector store with default tensors
-            >>> data = DeepLakeVectorStore(
-            ...        path = <path_for_storing_Data>,
+            >>> data = VectorStore(
+            ...        path = "./my_vector_store",
             ... )
-            >>>
+
             >>> # Create a vector store in the Deep Lake Managed Tensor Database
-            >>> data = DeepLakeVectorStore(
+            >>> data = VectorStore(
             ...        path = "hub://org_id/dataset_name",
             ...        runtime = {"tensor_db": True},
             ... )
-            >>>
+
             >>> # Create a vector store with custom tensors
-            >>> data = DeepLakeVectorStore(
-            ...        path = <path_for_storing_data>,
+            >>> data = VectorStore(
+            ...        path = "./my_vector_store",
             ...        tensor_params = [{"name": "text", "htype": "text"},
             ...                         {"name": "embedding_1", "htype": "embedding"},
             ...                         {"name": "embedding_2", "htype": "embedding"},
             ...                         {"name": "source", "htype": "text"},
             ...                         {"name": "metadata", "htype": "json"}
             ...                        ]
             ... )
@@ -74,23 +74,27 @@
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             tensor_params (List[Dict[str, dict]], optional): List of dictionaries that contains information about tensors that user wants to create. See ``create_tensor`` in Deep Lake API docs for more information. Defaults to ``DEFAULT_VECTORSTORE_TENSORS``.
             embedding_function (Optional[callable], optional): Function that converts the embeddable data into embeddings. Defaults to None.
             read_only (bool, optional):  Opens dataset in read-only mode if True. Defaults to False.
             num_workers (int): Number of workers to use for parallel ingestion.
             ingestion_batch_size (int): Batch size to use for parallel ingestion.
-            exec_option (str): Default method for search execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
+            exec_option (str): Default method for search execution. It could be either It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``"python"``.
+
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"db_engine": True} during dataset creation.
             token (str, optional): Activeloop token, used for fetching user credentials. This is Optional, tokens are normally autogenerated. Defaults to None.
             overwrite (bool): If set to True this overwrites the Vector Store if it already exists. Defaults to False.
             verbose (bool): Whether to print summary of the dataset created. Defaults to True.
             **kwargs (Any): Additional keyword arguments.
 
+        ..
+            # noqa: DAR101
+
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if the Vector Store exists! Be very careful when setting this parameter.
         """
         feature_report_path(
             path,
             "vs.initialize",
             {
@@ -141,51 +145,74 @@
         **tensors,
     ) -> Optional[List[str]]:
         """Adding elements to deeplake vector store.
 
         Tensor names are specified as parameters, and data for each tensor is specified as parameter values. All data must of equal length.
 
         Examples:
+            >>> # Dummy data
+            >>> texts = ["Hello", "World"]
+            >>> embeddings = [[1, 2, 3], [4, 5, 6]]
+            >>> metadatas = [{"timestamp": "01:20"}, {"timestamp": "01:22"}]
+            >>> emebdding_fn = lambda x: [[1, 2, 3]] * len(x)
+            >>> embedding_fn_2 = lambda x: [[4, 5]] * len(x)
+
             >>> # Directly upload embeddings
             >>> deeplake_vector_store.add(
-            ...     text = <list_of_texts>,
-            ...     embedding = [list_of_embeddings]
-            ...     metadata = <list_of_metadata_jsons>,
+            ...     text = texts,
+            ...     embedding = embeddings,
+            ...     metadata = metadatas,
             ... )
-            >>>
+
             >>> # Upload embedding via embedding function
             >>> deeplake_vector_store.add(
-            ...     text = <list_of_texts>,
-            ...     metadata = <list_of_metadata_jsons>,
-            ...     embedding_function = <embedding_function>,
-            ...     embedding_data = <list_of_data_for_embedding>,
+            ...     text = texts,
+            ...     metadata = metadatas,
+            ...     embedding_function = embedding_fn,
+            ...     embedding_data = texts,
             ... )
-            >>>
+
             >>> # Upload embedding via embedding function to a user-defined embedding tensor
             >>> deeplake_vector_store.add(
-            ...     text = <list_of_texts>,
-            ...     metadata = <list_of_metadata_jsons>,
-            ...     embedding_function = <embedding_function>,
-            ...     embedding_data = <list_of_data_for_embedding>,
-            ...     embedding_tensor = <user_defined_embedding_tensor_name>,
+            ...     text = texts,
+            ...     metadata = metadatas,
+            ...     embedding_function = embedding_fn,
+            ...     embedding_data = texts,
+            ...     embedding_tensor = "embedding_1",
             ... )
+
+            >>> # Multiple embedding functions (user defined embedding tensors must be specified)
+            >>> deeplake_vector_store.add(
+            ...     embedding_tensor = ["embedding_1", "embedding_2"]
+            ...     embedding_function = [embedding_fn, embedding_fn_2],
+            ...     embedding_data = [texts, texts],
+            ... )
+
+            >>> # Alternative syntax for multiple embedding functions
+            >>> deeplake_vector_store.add(
+            ...     text = texts,
+            ...     metadata = metadatas,
+            ...     embedding_tensor_1 = (embedding_fn, texts),
+            ...     embedding_tensor_2 = (embedding_fn_2, texts),
+            ... )
+
             >>> # Add data to fully custom tensors
             >>> deeplake_vector_store.add(
-            ...     tensor_A = <list_of_data_for_tensor_A>,
-            ...     tensor_B = <list_of_data_for_tensor_B>
-            ...     tensor_C = <list_of_data_for_tensor_C>,
-            ...     embedding_function = <embedding_function>,
-            ...     embedding_data = <list_of_data_for_embedding>,
-            ...     embedding_tensor = <user_defined_embedding_tensor_name>,
+            ...     tensor_A = [1, 2],
+            ...     tensor_B = ["a", "b"],
+            ...     tensor_C = ["some", "data"],
+            ...     embedding_function = embedding_fn,
+            ...     embedding_data = texts,
+            ...     embedding_tensor = "embedding_1",
             ... )
 
         Args:
             embedding_function (Optional[Callable]): embedding function used to convert ``embedding_data`` into embeddings. Overrides the ``embedding_function`` specified when initializing the Vector Store.
             embedding_data (Optional[List]): Data to be converted into embeddings using the provided ``embedding_function``. Defaults to None.
-            embedding_tensor (Optional[str]): Tensor where results from the embedding function will be stored. If None, the embedding tensors is automatically inferred (when possible). Defaults to None.
+            embedding_tensor (Optional[str]): Tensor where results from the embedding function will be stored. If None, the embedding tensor is automatically inferred (when possible). Defaults to None.
             total_samples_processed (int): Total number of samples processed before ingestion stopped. When specified.
             return_ids (bool): Whether to return added ids as an ouput of the method. Defaults to False.
             num_workers (int): Number of workers to use for parallel ingestion. Overrides the ``num_workers`` specified when initializing the Vector Store.
             ingestion_batch_size (int): Batch size to use for parallel ingestion. Defaults to 1000. Overrides the ``ingestion_batch_size`` specified when initializing the Vector Store.
             **tensors: Keyword arguments where the key is the tensor name, and the value is a list of samples that should be uploaded to that tensor.
 
         Returns:
@@ -264,60 +291,67 @@
         query: Optional[str] = None,
         filter: Optional[Union[Dict, Callable]] = None,
         exec_option: Optional[str] = "python",
         embedding_tensor: str = "embedding",
         return_tensors: Optional[List[str]] = None,
         return_view: bool = False,
     ) -> Union[Dict, deeplake.core.dataset.Dataset]:
-        """DeepLakeVectorStore search method that combines embedding search, metadata search, and custom TQL search.
+        """VectorStore search method that combines embedding search, metadata search, and custom TQL search.
 
         Examples:
             >>> # Search using an embedding
             >>> data = vector_store.search(
-            ...        embedding = <your_embedding>,
-            ...        exec_option = <preferred_exec_option>,
+            ...        embedding = [1, 2, 3],
+            ...        exec_option = "python",
             ... )
+
             >>> # Search using an embedding function and data for embedding
             >>> data = vector_store.search(
             ...        embedding_data = "What does this chatbot do?",
-            ...        embedding_function = <your_embedding_function>,
-            ...        exec_option = <preferred_exec_option>,
+            ...        embedding_function = query_embedding_fn,
+            ...        exec_option = "compute_engine",
             ... )
-            >>>
+
             >>> # Add a filter to your search
             >>> data = vector_store.search(
-            ...        embedding = <your_embedding>,
-            ...        exec_option = <preferred_exec_option>,
+            ...        embedding = np.ones(3),
+            ...        exec_option = "python",
             ...        filter = {"json_tensor_name": {"key: value"}, "json_tensor_name_2": {"key_2: value_2"},...}, # Only valid for exec_option = "python"
             ... )
-            >>>
+
             >>> # Search using TQL
             >>> data = vector_store.search(
             ...        query = "select * where ..... <add TQL syntax>",
-            ...        exec_option = <preferred_exec_option>, # Only valid for exec_option = "compute_engine" or "tensor_db"
+            ...        exec_option = "tensor_db", # Only valid for exec_option = "compute_engine" or "tensor_db"
             ... )
 
         Args:
             embedding (Union[np.ndarray, List[float]], optional): Embedding representation for performing the search. Defaults to None. The ``embedding_data`` and ``embedding`` cannot both be specified.
             embedding_data: Data against which the search will be performed by embedding it using the `embedding_function`. Defaults to None. The `embedding_data` and `embedding` cannot both be specified.
             embedding_function (callable, optional): function for converting `embedding_data` into embedding. Only valid if `embedding_data` is specified
             k (int): Number of elements to return after running query. Defaults to 4.
-            distance_metric (str): Type of distance metric to use for sorting the data. Avaliable options are: "L1", "L2", "COS", "MAX". Defaults to "COS".
+            distance_metric (str): Type of distance metric to use for sorting the data. Avaliable options are: ``"L1", "L2", "COS", "MAX"``. Defaults to ``"COS"``.
             query (Optional[str]):  TQL Query string for direct evaluation, without application of additional filters or vector search.
             filter (Union[Dict, Callable], optional): Additional filter evaluated prior to the embedding search.
+
                 - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
-                - ``Function`` - Any function that is compatible with `deeplake.filter`.
-            exec_option (Optional[str]): Method for search execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
+                - ``Function`` - Any function that is compatible with :meth:`Dataset.filter <deeplake.core.dataset.Dataset.filter>`.
+
+            exec_option (Optional[str]): Method for search execution. It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``"python"``.
+
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"db_engine": True} during dataset creation.
             embedding_tensor (str): Name of tensor with embeddings. Defaults to "embedding".
             return_tensors (Optional[List[str]]): List of tensors to return data for. Defaults to None. If None, all tensors are returned.
             return_view (bool): Return a Deep Lake dataset view that satisfied the search parameters, instead of a dictinary with data. Defaults to False.
 
+        ..
+            # noqa: DAR101
+
         Raises:
             ValueError: When invalid parameters are specified.
 
         Returns:
             Dict: Dictionary where keys are tensor names and values are the results of the search
         """
 
@@ -390,48 +424,53 @@
         row_ids: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         filter: Optional[Union[Dict, Callable]] = None,
         query: Optional[str] = None,
         exec_option: Optional[str] = "python",
         delete_all: Optional[bool] = None,
     ) -> bool:
-        """Delete the data in the Vector Store. Does not delete the tensor definitions. To delete the vector store completely, first run ``DeepLakeVectorStore.delete_by_path()``.
+        """Delete the data in the Vector Store. Does not delete the tensor definitions. To delete the vector store completely, first run :meth:`VectorStore.delete_by_path()`.
 
         Examples:
             >>> # Delete using ids:
             >>> data = vector_store.delete(ids)
-            >>>
+
             >>> # Delete data using filter
             >>> data = vector_store.delete(
             ...        filter = {"json_tensor_name": {"key: value"}, "json_tensor_name_2": {"key_2: value_2"}},
             ... )
-            >>>
+
             >>> # Delete data using TQL
             >>> data = vector_store.delete(
             ...        query = "select * where ..... <add TQL syntax>",
-            ...        exec_option = <preferred_exec_option>,
+            ...        exec_option = "compute_engine",
             ... )
 
         Args:
             ids (Optional[List[str]]): List of unique ids. Defaults to None.
             row_ids (Optional[List[str]]): List of absolute row indices from the dataset. Defaults to None.
             filter (Union[Dict, Callable], optional): Filter for finding samples for deletion.
+
                 - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
                 - ``Function`` - Any function that is compatible with `deeplake.filter`.
             query (Optional[str]):  TQL Query string for direct evaluation for finding samples for deletion, without application of additional filters.
-            exec_option (str, optional): Method for search execution for finding samples for deletion. It could be either "python", "compute_engine". Defaults to "python".
+            exec_option (str, optional): Method for search execution for finding samples for deletion. It could be either ``"python"`` or ``"compute_engine"``. Defaults to ``"python"``.
+
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
             delete_all (Optional[bool]): Whether to delete all the samples and version history of the dataset. Defaults to None.
 
+        ..
+            # noqa: DAR101
+
         Returns:
             bool: Returns True if deletion was successful, otherwise it raises a ValueError.
 
         Raises:
-            ValueError: If neither `ids`, `filter`, `query`, nor `delete_all` are specified, or if an invalid `exec_option` is provided.
+            ValueError: If neither ``ids``, ``filter``, ``query``, nor ``delete_all`` are specified, or if an invalid ``exec_option`` is provided.
         """
 
         deeplake_reporter.feature_report(
             feature_name="vs.delete",
             parameters={
                 "ids": True if ids is not None else False,
                 "query": query[0:100] if query is not None else False,
```

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.5/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1141,7 +1141,26 @@
     )
 
     vector_store.add(text=texts, embedding=embeddings)
     with pytest.raises(AssertionError):
         vector_store.search([texts[0], texts[0]], embedding_fn3, k=1)
 
     vector_store.search([texts[0]], embedding_fn4, k=1)
+
+
+def test_embeddings_only(local_path):
+    vector_store = VectorStore(
+        path=local_path,
+        overwrite=True,
+        tensor_params=[
+            {"name": "embedding_1", "htype": "embedding"},
+            {"name": "embedding_2", "htype": "embedding"},
+        ],
+    )
+
+    vector_store.add(
+        embedding_1=(embedding_fn, texts), embedding_2=(embedding_fn3, texts)
+    )
+
+    assert len(vector_store.dataset) == 10
+    assert len(vector_store.dataset.embedding_1) == 10
+    assert len(vector_store.dataset.embedding_2) == 10
```

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,18 +234,24 @@
 
 def preprocess_tensors(
     embedding_data=None, embedding_tensor=None, dataset=None, **tensors
 ):
     # generate id list equal to the length of the tensors
     # dont use None tensors to get length of tensor
     _tensors = {k: v for k, v in tensors.items() if v is not None}
-    first_item = next(iter(_tensors))
+    try:
+        num_items = len(next(iter(_tensors.values())))
+    except StopIteration:
+        if embedding_data:
+            num_items = len(embedding_data[0])
+        else:
+            num_items = 0
     ids_tensor = "ids" if "ids" in _tensors else "id"
     if ids_tensor not in _tensors or ids_tensor is None:
-        id = [str(uuid.uuid1()) for _ in _tensors[first_item]]
+        id = [str(uuid.uuid1()) for _ in range(num_items)]
         tensors[ids_tensor] = id
 
     processed_tensors = {ids_tensor: tensors[ids_tensor]}
 
     for tensor_name, tensor_data in tensors.items():
         if tensor_data is None:
             tensor_data = [None] * len(tensors[ids_tensor])
```

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.5/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.5/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.5/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.5/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.5/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.5/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.5/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.5/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/dataloader.py` & `deeplake-3.6.5/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.5/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.5/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.5/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/test_query.py` & `deeplake-3.6.5/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.5/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/enterprise/util.py` & `deeplake-3.6.5/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/hooks.py` & `deeplake-3.6.5/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/htype.py` & `deeplake-3.6.5/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.5/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.5/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.5/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.5/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.5/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.5/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/tf/common.py` & `deeplake-3.6.5/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.5/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.5/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.5/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.5/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/client_fixtures.py` & `deeplake-3.6.5/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/common.py` & `deeplake-3.6.5/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.5/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/path_fixtures.py` & `deeplake-3.6.5/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.5/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/access_method.py` & `deeplake-3.6.5/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/agreement.py` & `deeplake-3.6.5/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/array_list.py` & `deeplake-3.6.5/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.5/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/auto.py` & `deeplake-3.6.5/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/bugout_reporter.py` & `deeplake-3.6.5/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/cache_chain.py` & `deeplake-3.6.5/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/casting.py` & `deeplake-3.6.5/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/check_latest_version.py` & `deeplake-3.6.5/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/chunk_engine.py` & `deeplake-3.6.5/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/class_label.py` & `deeplake-3.6.5/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/compute.py` & `deeplake-3.6.5/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/connect_dataset.py` & `deeplake-3.6.5/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/dataset.py` & `deeplake-3.6.5/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/diff.py` & `deeplake-3.6.5/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/downsample.py` & `deeplake-3.6.5/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/encoder.py` & `deeplake-3.6.5/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/exceptions.py` & `deeplake-3.6.5/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/exif.py` & `deeplake-3.6.5/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/from_tfds.py` & `deeplake-3.6.5/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/htype.py` & `deeplake-3.6.5/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/image.py` & `deeplake-3.6.5/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/invalid_view_op.py` & `deeplake-3.6.5/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/iteration_warning.py` & `deeplake-3.6.5/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/json.py` & `deeplake-3.6.5/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/keys.py` & `deeplake-3.6.5/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/link.py` & `deeplake-3.6.5/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/logging.py` & `deeplake-3.6.5/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/merge.py` & `deeplake-3.6.5/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/modified.py` & `deeplake-3.6.5/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/notebook.py` & `deeplake-3.6.5/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.5/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.5/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.5/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.5/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.5/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/path.py` & `deeplake-3.6.5/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/pretty_print.py` & `deeplake-3.6.5/deeplake/util/pretty_print.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     divider = ["-------"] * 4
     max_column_length = [7, 7, 7, 7]
 
     tensor_htype = tensor.htype
     if tensor_htype == None:
         tensor_htype = "None"
 
-    shape = tensor.shape
-    tensor_shape = str(tensor.shape_interval if None in shape else shape)
+    tensor_shape = str(tensor.shape_interval)
 
     tensor_compression = tensor.meta.sample_compression
     if tensor_compression == None:
         tensor_compression = "None"
 
     if tensor.dtype == None:
         tensor_dtype = "None"
@@ -84,16 +83,15 @@
     for tensor_name in tensor_dict:
         tensor_object = tensor_dict[tensor_name]
 
         tensor_htype = tensor_object.htype
         if tensor_htype == None:
             tensor_htype = "None"
 
-        shape = tensor_object.shape
-        tensor_shape = str(tensor_object.shape_interval if None in shape else shape)
+        tensor_shape = str(tensor_object.shape_interval)
 
         tensor_compression = tensor_object.meta.sample_compression
         if tensor_compression == None:
             tensor_compression = "None"
 
         if tensor_object.dtype == None:
             tensor_dtype = "None"
```

### Comparing `deeplake-3.6.4/deeplake/util/remove_cache.py` & `deeplake-3.6.5/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/scheduling.py` & `deeplake-3.6.5/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/shape_interval.py` & `deeplake-3.6.5/deeplake/util/shape_interval.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,11 +74,19 @@
 
         for l, u in zip(self.lower, self.upper):
             if l == u:
                 intervals.append(str(l))
             else:
                 intervals.append(f"{l}:{u}")
 
+        if len(intervals) == 1:
+            return f"({intervals[0]},)"
         return f"({', '.join(intervals)})"
 
     def __repr__(self):
         return str(self)
+
+    def __eq__(self, other):
+        if not isinstance(other, ShapeInterval):
+            return False
+
+        return self.lower == other.lower and self.upper == other.upper
```

### Comparing `deeplake-3.6.4/deeplake/util/spinner.py` & `deeplake-3.6.5/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/split.py` & `deeplake-3.6.5/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/storage.py` & `deeplake-3.6.5/deeplake/util/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from deeplake.util.agreement import handle_dataset_agreements
 from deeplake.util.cache_chain import generate_chain
 from deeplake.constants import LOCAL_CACHE_PREFIX, MB
 from deeplake.util.exceptions import AgreementNotAcceptedError
 from deeplake.util.tag import process_hub_path
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 from deeplake.core.storage.provider import StorageProvider
 import os
 from deeplake.core.storage import (
     LocalProvider,
     S3Provider,
     GCSProvider,
     AzureProvider,
@@ -98,43 +98,53 @@
         storage._is_hub_path = is_hub_path
 
     if read_only:
         storage.enable_readonly()
     return storage
 
 
-def storage_provider_from_hub_path(
-    path: str,
-    read_only: bool = False,
-    db_engine: bool = False,
-    token: Optional[str] = None,
-    creds: Optional[Union[dict, str]] = None,
+def get_dataset_credentials(
+    client: DeepLakeBackendClient,
+    org_id: str,
+    ds_name: str,
+    mode: Optional[str],
+    db_engine: bool,
 ):
-    path, org_id, ds_name, subdir = process_hub_path(path)
-    client = DeepLakeBackendClient(token=token)
-
-    mode = "r" if read_only else None
     # this will give the proper url (s3, gcs, etc) and corresponding creds, depending on where the dataset is stored.
     try:
         url, final_creds, mode, expiration, repo = client.get_dataset_credentials(
             org_id, ds_name, mode=mode, db_engine={"enabled": db_engine}
         )
     except AgreementNotAcceptedError as e:
         handle_dataset_agreements(client, e.agreements, org_id, ds_name)
         url, final_creds, mode, expiration, repo = client.get_dataset_credentials(
             org_id, ds_name, mode=mode, db_engine={"enabled": db_engine}
         )
+    return url, final_creds, mode, expiration, repo
+
 
-    if mode == "r":
+def storage_provider_from_hub_path(
+    path: str,
+    read_only: Optional[bool] = None,
+    db_engine: bool = False,
+    token: Optional[str] = None,
+    creds: Optional[Union[dict, str]] = None,
+):
+    path, org_id, ds_name, subdir = process_hub_path(path)
+    client = DeepLakeBackendClient(token=token)
+
+    mode = None if (read_only is None) else ("r" if read_only else "w")
+    url, final_creds, mode, expiration, repo = get_dataset_credentials(
+        client, org_id, ds_name, mode, db_engine
+    )
+
+    if mode == "r" and read_only is None and not DEFAULT_READONLY:
+        # warns user about automatic mode change
+        print("Opening dataset in read-only mode as you don't have write permissions.")
         read_only = True
-        if read_only is None and not DEFAULT_READONLY:
-            # warns user about automatic mode change
-            print(
-                "Opening dataset in read-only mode as you don't have write permissions."
-            )
 
     if read_only is None:
         read_only = DEFAULT_READONLY
 
     url = posixpath.join(url, subdir)
 
     creds_used = "PLATFORM"
```

### Comparing `deeplake-3.6.4/deeplake/util/tag.py` & `deeplake-3.6.5/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tensor_db.py` & `deeplake-3.6.5/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/testing.py` & `deeplake-3.6.5/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_auto.py` & `deeplake-3.6.5/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.5/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.5/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_read.py` & `deeplake-3.6.5/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.5/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_split.py` & `deeplake-3.6.5/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.5/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.5/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/transform.py` & `deeplake-3.6.5/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/version_control.py` & `deeplake-3.6.5/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/util/video.py` & `deeplake-3.6.5/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.5/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake/visualizer/visualizer.py` & `deeplake-3.6.5/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.5/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.4
+Version: 3.6.5
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.4 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.5 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.4/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.5/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.4/deeplake.egg-info/requires.txt` & `deeplake-3.6.5/deeplake.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 azure-storage-blob
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
-libdeeplake==0.0.59
+libdeeplake==0.0.60
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -47,15 +47,15 @@
 azure-storage-blob
 
 [dicom]
 nibabel
 pydicom
 
 [enterprise]
-libdeeplake==0.0.59
+libdeeplake==0.0.60
 pyjwt
 
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
```

### Comparing `deeplake-3.6.4/setup.py` & `deeplake-3.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.59"
+    libdeeplake = "libdeeplake==0.0.60"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

