# Comparing `tmp/coretex-1.0.6.tar.gz` & `tmp/coretex-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.6.tar", last modified: Wed Jun 14 11:57:14 2023, max compression
+gzip compressed data, was "coretex-1.0.7.tar", last modified: Fri Jun 23 09:30:00 2023, max compression
```

## Comparing `coretex-1.0.6.tar` & `coretex-1.0.7.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.004337 coretex-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-14 11:57:02.000000 coretex-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-14 11:57:14.004337 coretex-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-14 11:57:02.000000 coretex-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.976337 coretex-1.0.6/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.980337 coretex-1.0.6/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.984337 coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/network_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.988337 coretex-1.0.6/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/experiment_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.988337 coretex-1.0.6/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.988337 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/experiment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.992337 coretex-1.0.6/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.992337 coretex-1.0.6/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.992337 coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.992337 coretex-1.0.6/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.992337 coretex-1.0.6/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.996337 coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.996337 coretex-1.0.6/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.996337 coretex-1.0.6/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.996337 coretex-1.0.6/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.000337 coretex-1.0.6/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.000337 coretex-1.0.6/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.000337 coretex-1.0.6/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.000337 coretex-1.0.6/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.000337 coretex-1.0.6/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:14.004337 coretex-1.0.6/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-14 11:57:02.000000 coretex-1.0.6/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:57:13.976337 coretex-1.0.6/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-14 11:57:13.000000 coretex-1.0.6/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-14 11:57:13.000000 coretex-1.0.6/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:57:13.000000 coretex-1.0.6/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-14 11:57:13.000000 coretex-1.0.6/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:57:13.000000 coretex-1.0.6/coretex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-14 11:57:02.000000 coretex-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:57:14.004337 coretex-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-23 09:29:47.000000 coretex-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-23 09:30:00.421241 coretex-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-23 09:29:47.000000 coretex-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/network_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/experiment_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-23 09:29:47.000000 coretex-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:30:00.421241 coretex-1.0.7/setup.cfg
```

### Comparing `coretex-1.0.6/LICENSE` & `coretex-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/PKG-INFO` & `coretex-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.6/README.md` & `coretex-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/__init__.py` & `coretex-1.0.7/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/_configuration.py` & `coretex-1.0.7/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/_logger.py` & `coretex-1.0.7/coretex/_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
 from .folder_management import FolderManager
 from .logging import LogSeverity, initializeLogger
 from .utils import DATE_FORMAT
 
 
 def _initializeDefaultLogger() -> None:
-    logPath = FolderManager.instance().logs / f"{datetime.now().strftime(DATE_FORMAT)}.log"
+    logPath = FolderManager.instance().logs / f"coretexpylib_{datetime.now().strftime(DATE_FORMAT)}.log"
     initializeLogger(LogSeverity.info, logPath)
```

### Comparing `coretex-1.0.6/coretex/cache/__init__.py` & `coretex-1.0.7/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/cache/cache_module.py` & `coretex-1.0.7/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/codable/__init__.py` & `coretex-1.0.7/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/codable/codable.py` & `coretex-1.0.7/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/codable/descriptor.py` & `coretex-1.0.7/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/__init__.py` & `coretex-1.0.7/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/annotation/__init__.py` & `coretex-1.0.7/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.7/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.7/coretex/coretex/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.7/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.7/coretex/coretex/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/__init__.py` & `coretex-1.0.7/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.7/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.7/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/__init__.py` & `coretex-1.0.7/coretex/coretex/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.7/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.7/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.7/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.7/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/dataset/utils.py` & `coretex-1.0.7/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/__init__.py` & `coretex-1.0.7/coretex/coretex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/artifact.py` & `coretex-1.0.7/coretex/coretex/experiment/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/experiment.py` & `coretex-1.0.7/coretex/coretex/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/experiment_builder.py` & `coretex-1.0.7/coretex/coretex/experiment/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/metric.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.7/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/parameters.py` & `coretex-1.0.7/coretex/coretex/experiment/parameters.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/status.py` & `coretex-1.0.7/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/experiment/utils.py` & `coretex-1.0.7/coretex/coretex/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/model/__init__.py` & `coretex-1.0.7/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/model/model.py` & `coretex-1.0.7/coretex/coretex/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/__init__.py` & `coretex-1.0.7/coretex/coretex/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.7/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.7/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.7/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.7/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.7/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.7/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/local_sample.py` & `coretex-1.0.7/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/network_sample.py` & `coretex-1.0.7/coretex/coretex/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/sample/sample.py` & `coretex-1.0.7/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/space/__init__.py` & `coretex-1.0.7/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/space/base.py` & `coretex-1.0.7/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/space/project.py` & `coretex-1.0.7/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/space/space.py` & `coretex-1.0.7/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/coretex/space/space_task.py` & `coretex-1.0.7/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/folder_management/__init__.py` & `coretex-1.0.7/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/folder_management/folder_manager.py` & `coretex-1.0.7/coretex/folder_management/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/logging/__init__.py` & `coretex-1.0.7/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/logging/log.py` & `coretex-1.0.7/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/logging/log_severity.py` & `coretex-1.0.7/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/logging/logger.py` & `coretex-1.0.7/coretex/logging/logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/__init__.py` & `coretex-1.0.7/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/chunk_upload_session.py` & `coretex-1.0.7/coretex/networking/chunk_upload_session.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/file_data.py` & `coretex-1.0.7/coretex/networking/file_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/network_manager.py` & `coretex-1.0.7/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/network_manager_base.py` & `coretex-1.0.7/coretex/networking/network_manager_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,14 @@
         return self._requestManager.genericRequest(RequestType.delete, endpoint, self._requestHeader())
 
     def genericJSONRequest(
         self,
         endpoint: str,
         requestType: RequestType,
         parameters: Optional[Dict[str, Any]] = None,
-        headers: Optional[Dict[str, str]] = None,
         retryCount: int = 0
     ) -> NetworkResponse:
         """
             Sends generic http request with specified parameters
 
             Parameters
             ----------
@@ -430,25 +429,22 @@
                         "object_id": 1,
                     }
                 )
             >>> if response.hasFailed():
                     print("Failed to add the object")
         """
 
-        if headers is None:
-            headers = self._requestHeader()
-
         if parameters is None:
             parameters = {}
 
-        networkResponse = self._requestManager.genericRequest(requestType, endpoint, headers, json.dumps(parameters))
+        networkResponse = self._requestManager.genericRequest(requestType, endpoint, self._requestHeader(), json.dumps(parameters))
 
         if self.shouldRetry(retryCount, networkResponse):
             print(">> [Coretex] Retry count: {0}".format(retryCount))
-            return self.genericJSONRequest(endpoint, requestType, parameters, headers, retryCount + 1)
+            return self.genericJSONRequest(endpoint, requestType, parameters, retryCount + 1)
 
         return networkResponse
 
     def refreshToken(self) -> NetworkResponse:
         """
             Uses refresh token functionality to fetch new API access token
```

### Comparing `coretex-1.0.6/coretex/networking/network_object.py` & `coretex-1.0.7/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/network_response.py` & `coretex-1.0.7/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/request_type.py` & `coretex-1.0.7/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/requests_manager.py` & `coretex-1.0.7/coretex/networking/requests_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/networking/user_data.py` & `coretex-1.0.7/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/__init__.py` & `coretex-1.0.7/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/text.py` & `coretex-1.0.7/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/token.py` & `coretex-1.0.7/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/transcriber.py` & `coretex-1.0.7/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/transcription.py` & `coretex-1.0.7/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/nlp/utils.py` & `coretex-1.0.7/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/project/__init__.py` & `coretex-1.0.7/coretex/project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
      experimentId: int,
      datasetType: Optional[Type[DatasetType]] = None,
      metrics: Optional[List[Metric]] = None
 ) -> Experiment:
 
      experiment = ExperimentBuilder(experimentId).setDatasetType(datasetType).build()
 
-     logPath = FolderManager.instance().logs / f"{experiment.id}.log"
+     logPath = FolderManager.instance().logs / f"experiment_{experimentId}.log"
      customLogHandler = LogHandler.instance()
      customLogHandler.currentExperimentId = experiment.id
 
      # enable/disable verbose mode for experiments
      severity = LogSeverity.info
      verbose = experiment.parameters.get("verbose", False)
```

### Comparing `coretex-1.0.6/coretex/project/base.py` & `coretex-1.0.7/coretex/project/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/project/calculate_metrics.py` & `coretex-1.0.7/coretex/project/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/project/heartbeat.py` & `coretex-1.0.7/coretex/project/heartbeat.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/project/local.py` & `coretex-1.0.7/coretex/project/local.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/project/remote.py` & `coretex-1.0.7/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/qiime2/__init__.py` & `coretex-1.0.7/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/qiime2/utils.py` & `coretex-1.0.7/coretex/qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/threading/__init__.py` & `coretex-1.0.7/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/threading/threaded_data_processor.py` & `coretex-1.0.7/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/utils/__init__.py` & `coretex-1.0.7/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/utils/console_progress_bar.py` & `coretex-1.0.7/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/utils/date.py` & `coretex-1.0.7/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/utils/file.py` & `coretex-1.0.7/coretex/utils/file.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex/utils/number.py` & `coretex-1.0.7/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/coretex.egg-info/PKG-INFO` & `coretex-1.0.7/coretex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.6/coretex.egg-info/SOURCES.txt` & `coretex-1.0.7/coretex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coretex-1.0.6/pyproject.toml` & `coretex-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coretex"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" }
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
```

